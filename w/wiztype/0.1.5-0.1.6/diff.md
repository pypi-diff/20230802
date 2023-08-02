# Comparing `tmp/wiztype-0.1.5.tar.gz` & `tmp/wiztype-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiztype-0.1.5.tar", max compression
+gzip compressed data, was "wiztype-0.1.6.tar", max compression
```

## Comparing `wiztype-0.1.5.tar` & `wiztype-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1065 2022-11-08 04:07:06.627021 wiztype-0.1.5/LICENSE
--rw-r--r--   0        0        0     1164 2022-11-08 04:07:06.627021 wiztype-0.1.5/README.md
--rw-r--r--   0        0        0      472 2022-11-16 23:47:13.952850 wiztype-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      107 2022-11-08 04:07:06.627021 wiztype-0.1.5/wiztype/__init__.py
--rw-r--r--   0        0        0     1296 2022-11-08 04:07:06.627021 wiztype-0.1.5/wiztype/__main__.py
--rw-r--r--   0        0        0        0 2022-11-08 04:07:06.627021 wiztype-0.1.5/wiztype/cli.py
--rw-r--r--   0        0        0       96 2022-11-08 04:07:06.627021 wiztype-0.1.5/wiztype/memory/__init__.py
--rw-r--r--   0        0        0     7375 2022-11-16 18:23:20.386773 wiztype-0.1.5/wiztype/memory/properties.py
--rw-r--r--   0        0        0     2536 2022-11-16 23:46:50.372369 wiztype-0.1.5/wiztype/memory/types.py
--rw-r--r--   0        0        0     6009 2022-11-08 04:07:06.627021 wiztype-0.1.5/wiztype/type_dump.py
--rw-r--r--   0        0        0     1850 2022-11-08 04:07:06.627021 wiztype-0.1.5/wiztype/type_tree.py
--rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 wiztype-0.1.5/setup.py
--rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 wiztype-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-02 20:32:48.138529 wiztype-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1164 2023-08-02 20:32:48.138529 wiztype-0.1.6/README.md
+-rw-r--r--   0        0        0      481 2023-08-02 20:34:07.533935 wiztype-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-08-02 20:32:48.138529 wiztype-0.1.6/wiztype/__init__.py
+-rw-r--r--   0        0        0     1326 2023-08-02 20:33:56.664743 wiztype-0.1.6/wiztype/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-02 20:32:48.138529 wiztype-0.1.6/wiztype/cli.py
+-rw-r--r--   0        0        0       96 2023-08-02 20:32:48.138529 wiztype-0.1.6/wiztype/memory/__init__.py
+-rw-r--r--   0        0        0     7375 2023-08-02 20:32:48.138529 wiztype-0.1.6/wiztype/memory/properties.py
+-rw-r--r--   0        0        0     2536 2023-08-02 20:32:48.138529 wiztype-0.1.6/wiztype/memory/types.py
+-rw-r--r--   0        0        0     6009 2023-08-02 20:32:48.138529 wiztype-0.1.6/wiztype/type_dump.py
+-rw-r--r--   0        0        0     1850 2023-08-02 20:32:48.138529 wiztype-0.1.6/wiztype/type_tree.py
+-rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 wiztype-0.1.6/PKG-INFO
```

### Comparing `wiztype-0.1.5/LICENSE` & `wiztype-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wiztype-0.1.5/README.md` & `wiztype-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `wiztype-0.1.5/wiztype/__main__.py` & `wiztype-0.1.6/wiztype/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     revision_file = wiz_bin / "revision.dat"
 
     if not revision_file.exists():
         raise FileNotFoundError(f"revision.dat not found in {wiz_bin}")
 
     revision = revision_file.read_text().strip()
 
-    if str(outfile) == "use revision":
+    if str(outfile) == "use revision" or outfile == b"use revision":
         outfile = Path(revision.replace(".", "_") + ".json")
 
     click.echo(f"dumping types for revision {revision} to {outfile}")
 
     tree = wiztype.get_type_tree()
     dumper = dump_type(tree)
```

### Comparing `wiztype-0.1.5/wiztype/memory/properties.py` & `wiztype-0.1.6/wiztype/memory/properties.py`

 * *Files identical despite different names*

### Comparing `wiztype-0.1.5/wiztype/memory/types.py` & `wiztype-0.1.6/wiztype/memory/types.py`

 * *Files identical despite different names*

### Comparing `wiztype-0.1.5/wiztype/type_dump.py` & `wiztype-0.1.6/wiztype/type_dump.py`

 * *Files identical despite different names*

### Comparing `wiztype-0.1.5/wiztype/type_tree.py` & `wiztype-0.1.6/wiztype/type_tree.py`

 * *Files identical despite different names*

### Comparing `wiztype-0.1.5/PKG-INFO` & `wiztype-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: wiztype
-Version: 0.1.5
+Version: 0.1.6
 Summary: A type dumper for wizard101
 Home-page: https://github.com/StarrFox/wiztype
 License: MIT
 Author: StarrFox
 Author-email: starrfox6312@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: iced-x86 (>=1.17.0,<2.0.0)
-Requires-Dist: memobj (>=0.8.1,<0.9.0)
+Requires-Dist: memobj (>=0.8.1,<0.10.0)
 Project-URL: Repository, https://github.com/StarrFox/wiztype
 Description-Content-Type: text/markdown
 
 # wiztype
 A type dumper for wizard101
 
 ## install
```

