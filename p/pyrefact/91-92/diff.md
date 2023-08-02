# Comparing `tmp/pyrefact-91.tar.gz` & `tmp/pyrefact-92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrefact-91.tar", last modified: Tue Jul 11 19:09:11 2023, max compression
+gzip compressed data, was "pyrefact-92.tar", last modified: Wed Aug  2 19:42:51 2023, max compression
```

## Comparing `pyrefact-91.tar` & `pyrefact-92.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:09:11.063552 pyrefact-91/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 19:08:57.000000 pyrefact-91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-07-11 19:09:11.063552 pyrefact-91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-11 19:08:57.000000 pyrefact-91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-11 19:08:57.000000 pyrefact-91/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:09:11.063552 pyrefact-91/pyrefact/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27069 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/abstractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    35301 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/core.py
--rw-r--r--   0 runner    (1001) docker     (123)   135094 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/logs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13323 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/object_oriented.py
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/performance_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/performance_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    28522 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    33436 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/symbolic_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    18094 2023-07-11 19:08:57.000000 pyrefact-91/pyrefact/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:09:11.063552 pyrefact-91/pyrefact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-07-11 19:09:11.000000 pyrefact-91/pyrefact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 19:09:11.000000 pyrefact-91/pyrefact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:09:11.000000 pyrefact-91/pyrefact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 19:09:11.000000 pyrefact-91/pyrefact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 19:09:11.000000 pyrefact-91/pyrefact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 19:09:11.000000 pyrefact-91/pyrefact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:09:11.063552 pyrefact-91/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:09:11.063552 pyrefact-91/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-11 19:08:57.000000 pyrefact-91/tests/testing_infra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:42:51.771619 pyrefact-92/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-02 19:42:40.000000 pyrefact-92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-08-02 19:42:51.767619 pyrefact-92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-08-02 19:42:40.000000 pyrefact-92/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-02 19:42:40.000000 pyrefact-92/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:42:51.767619 pyrefact-92/pyrefact/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27069 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/abstractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35301 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/logs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13373 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/object_oriented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/performance_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/performance_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28522 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33436 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/symbolic_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18094 2023-08-02 19:42:40.000000 pyrefact-92/pyrefact/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:42:51.767619 pyrefact-92/pyrefact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-08-02 19:42:51.000000 pyrefact-92/pyrefact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 19:42:51.000000 pyrefact-92/pyrefact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:42:51.000000 pyrefact-92/pyrefact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 19:42:51.000000 pyrefact-92/pyrefact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-02 19:42:51.000000 pyrefact-92/pyrefact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 19:42:51.000000 pyrefact-92/pyrefact.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:42:51.771619 pyrefact-92/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:42:51.767619 pyrefact-92/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-02 19:42:40.000000 pyrefact-92/tests/testing_infra.py
```

### Comparing `pyrefact-91/LICENSE` & `pyrefact-92/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrefact-91/PKG-INFO` & `pyrefact-92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrefact
-Version: 91
+Version: 92
 Summary: Automated Python refactoring
 Author: Olle Lindgren
 Author-email: olle.ln@outlook.com
 License: MIT License
         
         Copyright (c) 2022 OlleLindgren
         
@@ -26,14 +26,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repository, https://github.com/OlleLindgren/pyrefact
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # pyrefact
 
 Pyrefact does advanced python refactoring, with the goal of simplifying complicated code, deleting dead code, and improving performance.
 
 Unlike emerging AI tools, pyrefact is entirely rule based and does not share your code with any third parties. Pyrefact can however break your code in some cases, and is not suitable for CI or other automated workflows.
```

### Comparing `pyrefact-91/README.md` & `pyrefact-92/README.md`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyproject.toml` & `pyrefact-92/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrefact"
-version = "91"
+version = "92"
 description = "Automated Python refactoring"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {email = "olle.ln@outlook.com"},
     {name = "Olle Lindgren"}
@@ -18,14 +18,17 @@
     "black>=23.1.0",
     "compactify>=2",
     "rmspace>=7",
     "sympy>=1.11.0",
     'astunparse==1.6.3; python_version<"3.9"'
 ]
 
+[project.optional-dependencies]
+dev = ["astunparse==1.6.3", "pylint==2.17.5"]
+
 [project.urls]
 repository="https://github.com/OlleLindgren/pyrefact"
 
 [project.scripts]
 pyrefact = "pyrefact.__main__:main"
 
 [tool.setuptools.packages.find]
```

### Comparing `pyrefact-91/pyrefact/abstractions.py` & `pyrefact-92/pyrefact/abstractions.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact/constants.py` & `pyrefact-92/pyrefact/constants.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact/core.py` & `pyrefact-92/pyrefact/core.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact/fixes.py` & `pyrefact-92/pyrefact/fixes.py`

 * *Files 0% similar despite different names*

```diff
@@ -3660,7 +3660,24 @@
         {{variable}} = False
     else:
         {{variable}} = True
     """
     replace = "{{variable}} = not {{condition}}"
 
     yield from processing.find_replace(source, find, replace, transaction=2)
+
+
+@processing.fix
+def fix_raise_missing_from(source: str) -> str:
+    find = """
+    try:
+        {{stuff}}
+    except {{exception}}:
+        raise {{something}}
+    """
+    replace = """
+    try:
+        {{stuff}}
+    except {{exception}} as error:
+        raise {{something}} from error
+    """
+    yield from processing.find_replace(source, find, replace)
```

### Comparing `pyrefact-91/pyrefact/formatting.py` & `pyrefact-92/pyrefact/formatting.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact/logs.py` & `pyrefact-92/pyrefact/logs.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact/main.py` & `pyrefact-92/pyrefact/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 
     Returns:
         str: Modified code
     """
     source = fixes.delete_commented_code(source)
     source = fixes.remove_dead_ifs(source)
     source = fixes.delete_unreachable_code(source)
+    source = fixes.fix_raise_missing_from(source)
     source = fixes.undefine_unused_variables(source, preserve=preserve)
     source = fixes.delete_pointless_statements(source)
     source = fixes.move_before_loop(source)
 
     source = fixes.delete_unused_functions_and_classes(source, preserve=preserve)
 
     source = object_oriented.remove_unused_self_cls(source)
```

### Comparing `pyrefact-91/pyrefact/object_oriented.py` & `pyrefact-92/pyrefact/object_oriented.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact/parsing.py` & `pyrefact-92/pyrefact/parsing.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact/performance.py` & `pyrefact-92/pyrefact/performance.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,14 +121,39 @@
         )
         for key, values in inner_outer_redundancy_mapping.items()
     )
 
     for node in core.walk(root, templates):
         yield node, node.args[0]
 
+    reversed_sorted_template = ast.Call(
+        func=ast.Name(id="reversed"), args=[ast.Call(func=ast.Name(id="sorted"))]
+    )
+    for node in core.walk(root, reversed_sorted_template):
+        replacement = node.args[0]
+        for i, kw in enumerate(replacement.keywords):
+            if kw.arg == "reverse":
+                kw.value = ast.UnaryOp(op=ast.Not(), operand=kw.value)
+                break
+        else:
+            i = len(replacement.keywords)
+            replacement.keywords.append(ast.keyword(arg="reverse", value=ast.Constant(value=True, kind=None)))
+
+        try:
+            value = core.literal_value(replacement.keywords[i].value)
+        except ValueError:
+            pass
+        else:
+            if value:
+                replacement.keywords[i].value = ast.Constant(value=bool(value), kind=None)
+            else:
+                del replacement.keywords[i]
+
+        yield node, replacement
+
 
 def _slice_of(node: ast.Subscript) -> ast.AST:
     node_slice = node.slice
     if constants.PYTHON_VERSION < (3, 9):
         if isinstance(node_slice, ast.Index):
             return node_slice.value
         if isinstance(node_slice, ast.ExtSlice):
```

### Comparing `pyrefact-91/pyrefact/performance_numpy.py` & `pyrefact-92/pyrefact/performance_numpy.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact/performance_pandas.py` & `pyrefact-92/pyrefact/performance_pandas.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact/processing.py` & `pyrefact-92/pyrefact/processing.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact/style.py` & `pyrefact-92/pyrefact/style.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact/symbolic_math.py` & `pyrefact-92/pyrefact/symbolic_math.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact/tracing.py` & `pyrefact-92/pyrefact/tracing.py`

 * *Files identical despite different names*

### Comparing `pyrefact-91/pyrefact.egg-info/PKG-INFO` & `pyrefact-92/pyrefact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrefact
-Version: 91
+Version: 92
 Summary: Automated Python refactoring
 Author: Olle Lindgren
 Author-email: olle.ln@outlook.com
 License: MIT License
         
         Copyright (c) 2022 OlleLindgren
         
@@ -26,14 +26,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repository, https://github.com/OlleLindgren/pyrefact
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # pyrefact
 
 Pyrefact does advanced python refactoring, with the goal of simplifying complicated code, deleting dead code, and improving performance.
 
 Unlike emerging AI tools, pyrefact is entirely rule based and does not share your code with any third parties. Pyrefact can however break your code in some cases, and is not suitable for CI or other automated workflows.
```

### Comparing `pyrefact-91/pyrefact.egg-info/SOURCES.txt` & `pyrefact-92/pyrefact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrefact-91/tests/testing_infra.py` & `pyrefact-92/tests/testing_infra.py`

 * *Files identical despite different names*

