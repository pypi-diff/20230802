# Comparing `tmp/pystasis-0.0.2.tar.gz` & `tmp/pystasis-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystasis-0.0.2.tar", max compression
+gzip compressed data, was "pystasis-0.0.3.tar", max compression
```

## Comparing `pystasis-0.0.2.tar` & `pystasis-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      290 2023-07-28 11:09:39.851240 pystasis-0.0.2/README.md
--rw-r--r--   0        0        0      525 2023-07-28 14:07:55.356812 pystasis-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-28 10:59:57.553241 pystasis-0.0.2/pystasis/__init__.py
--rw-r--r--   0        0        0       69 2023-07-28 13:34:07.119732 pystasis-0.0.2/pystasis/__main__.py
--rw-r--r--   0        0        0     2045 2023-07-28 14:05:10.191002 pystasis-0.0.2/pystasis/cli.py
--rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 pystasis-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      290 2023-07-28 11:09:39.851240 pystasis-0.0.3/README.md
+-rw-r--r--   0        0        0      544 2023-08-02 14:25:24.902392 pystasis-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 10:59:57.553241 pystasis-0.0.3/pystasis/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-28 13:34:07.119732 pystasis-0.0.3/pystasis/__main__.py
+-rw-r--r--   0        0        0     2752 2023-08-02 14:24:52.396049 pystasis-0.0.3/pystasis/cli.py
+-rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 pystasis-0.0.3/PKG-INFO
```

### Comparing `pystasis-0.0.2/pyproject.toml` & `pystasis-0.0.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "pystasis"
-version = "0.0.2"
+version = "0.0.3"
 description = "Detect breaking changes in Python projects"
 authors = ["Regan Koopmans <regan@koopmans.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 git-python = "^1.0.3"
 click = "^8.1.6"
+colored = "^2.2.3"
 
 [tool.poetry.scripts]
 pystasis = "pystasis.cli:main"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 isort = "^5.12.0"
```

### Comparing `pystasis-0.0.2/pystasis/cli.py` & `pystasis-0.0.3/pystasis/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import ast
 import logging
+import sys
 from logging import info, warning
 
+from colored import Fore, Style
 from git import Repo
 
 FORMAT = "%(levelname)s - %(message)s"
 logging.basicConfig(format=FORMAT)
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 
@@ -14,57 +16,75 @@
     for item in ast.walk(tree):
         if item.__class__.__name__ == "ClassDef" and item.name == name:
             return item
 
 
 def find_assign(name, children):
     for child in children:
-        if child.__class__.__name__ == "AnnAssign":
-            if child.target.id == name:
-                return True
+        if child.__class__.__name__ == "AnnAssign" and child.target.id == name:
+            return True
     return False
 
 
-def compare(ast_1, ast_2):
+def compare(filename, ast_1, ast_2):
+    any_missing = False
     for item in ast.walk(ast_1):
         if item.__class__.__name__ == "ClassDef":
             class_to_search = item.name
-            info(f"Checking {class_to_search}")
             new_class = find(ast_2, class_to_search)
-            children_old = [child for child in ast.iter_child_nodes(item)]
-            children_new = [child for child in ast.iter_child_nodes(new_class)]
-            for child in children_old:
-                if child.__class__.__name__ == "AnnAssign":
-                    to_search = child.target.id
-                    if not find_assign(to_search, children_new):
-                        warning(
-                            f'Possible breaking change: "{to_search}" '
-                            f"has been removed or renamed"
-                        )
+            old_assignments = []
+            new_assignments = []
+            for child in ast.iter_child_nodes(item):
+                if child.__class__.__name__ in ["AnnAssign"]:
+                    old_assignments.append(child.target.id)
+                if child.__class__.__name__ in ["Assign"]:
+                    old_assignments += [assign.id for assign in child.targets]
+
+            for child in ast.iter_child_nodes(new_class):
+                if child.__class__.__name__ in ["AnnAssign"]:
+                    new_assignments.append(child.target.id)
+                if child.__class__.__name__ in ["Assign"]:
+                    new_assignments += [assign.id for assign in child.targets]
+            missing = [
+                assign
+                for assign in old_assignments
+                if assign not in new_assignments
+            ]
+            for assign in missing:
+                any_missing = True
+                warning(
+                    f"{Fore.cyan}{assign}{Style.reset} has been renamed or "
+                    f"removed in {Fore.cyan}{class_to_search}{Style.reset}"
+                    f" ({filename})"
+                )
+    return any_missing
 
 
 def scan():
     repo = Repo(".")
-    changedFiles = [
+    changed_files = [
         item.a_path
-        for item in repo.index.diff(None)
+        for item in repo.index.diff("HEAD")
         if item.a_path.endswith(".py")
     ]
 
-    if len(changedFiles) == 0:
+    if len(changed_files) == 0:
         info("Nothing to do.")
 
-    for file in changedFiles:
+    any_missing = False
+    for file in changed_files:
         try:
-            source_old = repo.commit("Head").tree[file].data_stream.read()
+            source_old = repo.commit("HEAD").tree[file].data_stream.read()
             with open(file, "r") as f:
                 source_new = f.read()
-            info(f"Scanning in {file}...")
             tree_old = ast.parse(source_old)
             tree_new = ast.parse(source_new)
-            compare(tree_old, tree_new)
+            if compare(file, tree_old, tree_new):
+                any_missing = True
         except KeyError:
             pass
+    if any_missing:
+        sys.exit(1)
 
 
 def main():
     scan()
```

### Comparing `pystasis-0.0.2/PKG-INFO` & `pystasis-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pystasis
-Version: 0.0.2
+Version: 0.0.3
 Summary: Detect breaking changes in Python projects
 Author: Regan Koopmans
 Author-email: regan@koopmans.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.6,<9.0.0)
+Requires-Dist: colored (>=2.2.3,<3.0.0)
 Requires-Dist: git-python (>=1.0.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # pystasis
 
 pystasis is a tool to help you catch breaking changes in your Python projects.
 It does this by comparing AST (abstract-syntax tree) changes between commits
```

