# Comparing `tmp/arrrgs-2.0.0.tar.gz` & `tmp/arrrgs-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrrgs-2.0.0.tar", last modified: Wed Mar 29 15:13:46 2023, max compression
+gzip compressed data, was "arrrgs-3.0.0.tar", last modified: Wed Aug  2 12:01:16 2023, max compression
```

## Comparing `arrrgs-2.0.0.tar` & `arrrgs-3.0.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-03-29 15:13:46.009695 arrrgs-2.0.0/
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-03-29 15:13:46.002663 arrrgs-2.0.0/.github/
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-03-29 15:13:46.004664 arrrgs-2.0.0/.github/workflows/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      302 2023-02-11 21:11:19.000000 arrrgs-2.0.0/.github/workflows/qa.yaml
--rw-r--r--   0 mishamyrt   (501) staff       (20)       66 2023-03-29 13:47:46.000000 arrrgs-2.0.0/.gitignore
--rw-r--r--   0 mishamyrt   (501) staff       (20)        6 2023-03-29 15:13:41.000000 arrrgs-2.0.0/.version
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1073 2023-03-29 13:12:20.000000 arrrgs-2.0.0/LICENSE
--rw-r--r--   0 mishamyrt   (501) staff       (20)      834 2023-03-29 15:08:35.000000 arrrgs-2.0.0/Makefile
--rw-r--r--   0 mishamyrt   (501) staff       (20)     3940 2023-03-29 15:13:46.009530 arrrgs-2.0.0/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)     3545 2023-03-29 13:53:36.000000 arrrgs-2.0.0/README.md
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-03-29 15:13:46.004950 arrrgs-2.0.0/assets/
--rw-r--r--   0 mishamyrt   (501) staff       (20)    15275 2023-02-11 21:11:19.000000 arrrgs-2.0.0/assets/logo@2x.png
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-03-29 15:13:46.006769 arrrgs-2.0.0/examples/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      423 2023-02-11 21:11:19.000000 arrrgs-2.0.0/examples/args.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      227 2023-02-11 21:13:12.000000 arrrgs-2.0.0/examples/basic.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      530 2023-02-11 21:14:43.000000 arrrgs-2.0.0/examples/context.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      194 2023-02-15 22:46:00.000000 arrrgs-2.0.0/examples/custom_name.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      480 2023-02-11 21:11:19.000000 arrrgs-2.0.0/examples/environment.py
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)      491 2023-03-29 14:23:48.000000 arrrgs-2.0.0/examples/root_command.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      260 2023-03-29 13:54:26.000000 arrrgs-2.0.0/examples/subcommand.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      963 2023-03-29 15:13:36.000000 arrrgs-2.0.0/pyproject.toml
--rw-r--r--   0 mishamyrt   (501) staff       (20)       56 2023-03-29 15:09:24.000000 arrrgs-2.0.0/requirements.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-03-29 15:13:46.009743 arrrgs-2.0.0/setup.cfg
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-03-29 15:13:46.003041 arrrgs-2.0.0/src/
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-03-29 15:13:46.008510 arrrgs-2.0.0/src/arrrgs/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      136 2023-03-29 13:50:09.000000 arrrgs-2.0.0/src/arrrgs/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      659 2023-03-29 14:50:37.000000 arrrgs-2.0.0/src/arrrgs/arguments.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      775 2023-03-29 14:51:13.000000 arrrgs-2.0.0/src/arrrgs/command.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      405 2023-03-29 13:41:43.000000 arrrgs-2.0.0/src/arrrgs/log.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      229 2023-03-29 14:11:08.000000 arrrgs-2.0.0/src/arrrgs/parser.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2238 2023-03-29 14:59:41.000000 arrrgs-2.0.0/src/arrrgs/run.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-03-29 15:13:46.009281 arrrgs-2.0.0/src/arrrgs.egg-info/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     3940 2023-03-29 15:13:45.000000 arrrgs-2.0.0/src/arrrgs.egg-info/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)      569 2023-03-29 15:13:46.000000 arrrgs-2.0.0/src/arrrgs.egg-info/SOURCES.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-03-29 15:13:45.000000 arrrgs-2.0.0/src/arrrgs.egg-info/dependency_links.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        9 2023-03-29 15:13:45.000000 arrrgs-2.0.0/src/arrrgs.egg-info/requires.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        7 2023-03-29 15:13:45.000000 arrrgs-2.0.0/src/arrrgs.egg-info/top_level.txt
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.026501 arrrgs-3.0.0/
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.021976 arrrgs-3.0.0/.github/
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.023548 arrrgs-3.0.0/.github/workflows/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      302 2023-02-11 21:11:19.000000 arrrgs-3.0.0/.github/workflows/qa.yaml
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       66 2023-03-29 13:47:46.000000 arrrgs-3.0.0/.gitignore
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        6 2023-08-02 12:01:10.000000 arrrgs-3.0.0/.version
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1073 2023-03-29 13:12:20.000000 arrrgs-3.0.0/LICENSE
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      886 2023-08-02 12:00:21.000000 arrrgs-3.0.0/Makefile
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     3940 2023-08-02 12:01:16.026339 arrrgs-3.0.0/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     3545 2023-03-29 13:53:36.000000 arrrgs-3.0.0/README.md
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.023682 arrrgs-3.0.0/assets/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)    15275 2023-02-11 21:11:19.000000 arrrgs-3.0.0/assets/logo@2x.png
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.024566 arrrgs-3.0.0/examples/
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      446 2023-08-02 11:59:10.000000 arrrgs-3.0.0/examples/args.py
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      252 2023-08-02 11:59:02.000000 arrrgs-3.0.0/examples/basic.py
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      554 2023-08-02 11:58:59.000000 arrrgs-3.0.0/examples/context.py
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      218 2023-08-02 11:58:56.000000 arrrgs-3.0.0/examples/custom_name.py
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      505 2023-08-02 11:58:53.000000 arrrgs-3.0.0/examples/environment.py
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)      487 2023-08-02 11:57:33.000000 arrrgs-3.0.0/examples/root_command.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      963 2023-03-29 15:14:56.000000 arrrgs-3.0.0/pyproject.toml
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       56 2023-03-29 15:09:24.000000 arrrgs-3.0.0/requirements.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-08-02 12:01:16.026551 arrrgs-3.0.0/setup.cfg
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.022378 arrrgs-3.0.0/src/
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.025391 arrrgs-3.0.0/src/arrrgs/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      122 2023-08-02 11:17:14.000000 arrrgs-3.0.0/src/arrrgs/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      659 2023-03-29 14:50:37.000000 arrrgs-3.0.0/src/arrrgs/arguments.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      975 2023-08-02 11:57:26.000000 arrrgs-3.0.0/src/arrrgs/command.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      405 2023-03-29 13:41:43.000000 arrrgs-3.0.0/src/arrrgs/log.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      229 2023-08-02 11:49:49.000000 arrrgs-3.0.0/src/arrrgs/parser.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2238 2023-03-29 14:59:41.000000 arrrgs-3.0.0/src/arrrgs/run.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 12:01:16.026121 arrrgs-3.0.0/src/arrrgs.egg-info/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     3940 2023-08-02 12:01:15.000000 arrrgs-3.0.0/src/arrrgs.egg-info/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      546 2023-08-02 12:01:16.000000 arrrgs-3.0.0/src/arrrgs.egg-info/SOURCES.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-08-02 12:01:15.000000 arrrgs-3.0.0/src/arrrgs.egg-info/dependency_links.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        9 2023-08-02 12:01:15.000000 arrrgs-3.0.0/src/arrrgs.egg-info/requires.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        7 2023-08-02 12:01:15.000000 arrrgs-3.0.0/src/arrrgs.egg-info/top_level.txt
```

### Comparing `arrrgs-2.0.0/LICENSE` & `arrrgs-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrrgs-2.0.0/Makefile` & `arrrgs-3.0.0/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-VERSION = 2.0.0
+VERSION = 3.0.0
 VENV_PATH = ./venv
 VENV = . $(VENV_PATH)/bin/activate;
 SRC := \
 	$(wildcard src/arrrgs/*.py)
 
 .PHONY: publish
-publish: clean build
+publish:
+	make clean
+	make build
+	git tag "v$(VERSION)"
+	git push --tags
 	$(VENV) python3 -m twine upload --repository pypi dist/* -umishamyrt
 
 .PHONY: clean
 clean:
 	rm -rf *.egg-info
 	rm -rf build
 	rm -rf dist
```

### Comparing `arrrgs-2.0.0/PKG-INFO` & `arrrgs-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrrgs
-Version: 2.0.0
+Version: 3.0.0
 Summary: The library for easily writing feature-rich Python scripts
 Author-email: Mikhael Khrustik <misha@myrt.co>
 License: MIT
 Keywords: cli,command-line-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `arrrgs-2.0.0/README.md` & `arrrgs-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `arrrgs-2.0.0/assets/logo@2x.png` & `arrrgs-3.0.0/assets/logo@2x.png`

 * *Files identical despite different names*

### Comparing `arrrgs-2.0.0/examples/context.py` & `arrrgs-3.0.0/examples/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+#!/usr/bin/env python3
 """Arrrgs arguments example"""
 from arrrgs import command, run
 
+
 class User:
     """Represents user"""
 
     def __init__(self, name):
         self._name = name
 
     def get_name(self):
```

### Comparing `arrrgs-2.0.0/pyproject.toml` & `arrrgs-3.0.0/pyproject.toml`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arrrgs"
-readme = "README.md"
 authors = [
     {name = "Mikhael Khrustik", email = "misha@myrt.co"},
 ]
 description = "The library for easily writing feature-rich Python scripts"
+readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["cli", "command-line-tool"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License"
 ]
```

### Comparing `arrrgs-2.0.0/src/arrrgs/arguments.py` & `arrrgs-3.0.0/src/arrrgs/arguments.py`

 * *Files identical despite different names*

### Comparing `arrrgs-2.0.0/src/arrrgs/run.py` & `arrrgs-3.0.0/src/arrrgs/run.py`

 * *Files identical despite different names*

### Comparing `arrrgs-2.0.0/src/arrrgs.egg-info/PKG-INFO` & `arrrgs-3.0.0/src/arrrgs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrrgs
-Version: 2.0.0
+Version: 3.0.0
 Summary: The library for easily writing feature-rich Python scripts
 Author-email: Mikhael Khrustik <misha@myrt.co>
 License: MIT
 Keywords: cli,command-line-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

