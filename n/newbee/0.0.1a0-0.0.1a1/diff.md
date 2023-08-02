# Comparing `tmp/newbee-0.0.1a0.tar.gz` & `tmp/newbee-0.0.1a1.tar.gz`

## Comparing `newbee-0.0.1a0.tar` & `newbee-0.0.1a1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 newbee-0.0.1a0/.editorconfig
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 newbee-0.0.1a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 newbee-0.0.1a0/RELEASE.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 newbee-0.0.1a0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 newbee-0.0.1a0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 newbee-0.0.1a0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 newbee-0.0.1a0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 newbee-0.0.1a0/docs/Makefile
--rwxr-xr-x   0        0        0     4760 2020-02-02 00:00:00.000000 newbee-0.0.1a0/docs/conf.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 newbee-0.0.1a0/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 newbee-0.0.1a0/docs/make.bat
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 newbee-0.0.1a0/docs/usage.rst
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 newbee-0.0.1a0/newbee/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 newbee-0.0.1a0/tests/test_newbee.py
--rw-r--r--   0        0        0    10128 2020-02-02 00:00:00.000000 newbee-0.0.1a0/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 newbee-0.0.1a0/LICENSE
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 newbee-0.0.1a0/README.md
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 newbee-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 newbee-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.editorconfig
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 newbee-0.0.1a1/RELEASE.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 newbee-0.0.1a1/dev/Dockerfile
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 newbee-0.0.1a1/docker/Dockerfile
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 newbee-0.0.1a1/docs/Makefile
+-rwxr-xr-x   0        0        0     4760 2020-02-02 00:00:00.000000 newbee-0.0.1a1/docs/conf.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 newbee-0.0.1a1/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 newbee-0.0.1a1/docs/make.bat
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 newbee-0.0.1a1/docs/usage.rst
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 newbee-0.0.1a1/newbee/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 newbee-0.0.1a1/tests/test_newbee.py
+-rw-r--r--   0        0        0    10128 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 newbee-0.0.1a1/LICENSE
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 newbee-0.0.1a1/README.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 newbee-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 newbee-0.0.1a1/PKG-INFO
```

### Comparing `newbee-0.0.1a0/.pre-commit-config.yaml` & `newbee-0.0.1a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a0/RELEASE.md` & `newbee-0.0.1a1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a0/.github/workflows/python-package.yml` & `newbee-0.0.1a1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a0/docs/Makefile` & `newbee-0.0.1a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a0/docs/conf.py` & `newbee-0.0.1a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a0/docs/make.bat` & `newbee-0.0.1a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a0/.gitignore` & `newbee-0.0.1a1/.gitignore`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a0/LICENSE` & `newbee-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a0/README.md` & `newbee-0.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a0/pyproject.toml` & `newbee-0.0.1a1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 requires = ["hatchling", ]
 build-backend = "hatchling.build"
 
 [project]
 name = "newbee"
 description = "newbee"
 keywords = ["newbee"]
-requires-python = ">=3.7"
+requires-python = ">= 3.8"
 dependencies = [
 ]
 dynamic = ["version", ]
 classifiers = [
-    "Programming Language :: Python :: 3",
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
 ]
 [project.optional-dependencies]
 test = [
     "pytest",
 ]
```

### Comparing `newbee-0.0.1a0/PKG-INFO` & `newbee-0.0.1a1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: newbee
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: newbee
 Project-URL: Source, https://github.com/wh1isper/newbee
 Author-email: wh1isper <9573586@qq.com>
 License: BSD license
 License-File: LICENSE
 Keywords: newbee
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 ![](https://img.shields.io/github/license/wh1isper/newbee)
 ![](https://img.shields.io/github/v/release/wh1isper/newbee)
 ![](https://img.shields.io/pypi/dm/newbee)
```

