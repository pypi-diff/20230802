# Comparing `tmp/async_wrapper-0.3.2.tar.gz` & `tmp/async_wrapper-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.3.2.tar", max compression
+gzip compressed data, was "async_wrapper-0.4.1.tar", max compression
```

## Comparing `async_wrapper-0.3.2.tar` & `async_wrapper-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/LICENSE
--rw-r--r--   0        0        0     1776 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/README.md
--rw-r--r--   0        0        0     3657 2023-08-02 13:23:50.142941 async_wrapper-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      288 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-08-02 13:23:50.210942 async_wrapper-0.3.2/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      109 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/__init__.py
--rw-r--r--   0        0        0     1007 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/_loky.py
--rw-r--r--   0        0        0      564 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/_thread.py
--rw-r--r--   0        0        0      409 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/base.py
--rw-r--r--   0        0        0      654 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/main.py
--rw-r--r--   0        0        0     1721 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      107 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/synclib/__init__.py
--rw-r--r--   0        0        0      983 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/synclib/_loky.py
--rw-r--r--   0        0        0     1140 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/synclib/_thread.py
--rw-r--r--   0        0        0     1136 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/synclib/base.py
--rw-r--r--   0        0        0      656 2023-08-02 13:23:32.762643 async_wrapper-0.3.2/src/async_wrapper/convert/synclib/main.py
--rw-r--r--   0        0        0        0 2023-08-02 13:23:32.762643 async_wrapper-0.3.2/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      151 2023-08-02 13:23:32.762643 async_wrapper-0.3.2/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0      104 2023-08-02 13:23:32.762643 async_wrapper-0.3.2/src/async_wrapper/task_group/exception.py
--rw-r--r--   0        0        0     4440 2023-08-02 13:23:32.762643 async_wrapper-0.3.2/src/async_wrapper/task_group/task_group.py
--rw-r--r--   0        0        0     1354 2023-08-02 13:23:32.762643 async_wrapper-0.3.2/src/async_wrapper/task_group/value.py
--rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 async_wrapper-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1776 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/README.md
+-rw-r--r--   0        0        0     3416 2023-08-02 13:46:17.846701 async_wrapper-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-02 13:46:17.890705 async_wrapper-0.4.1/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      564 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/src/async_wrapper/convert/_async.py
+-rw-r--r--   0        0        0     1140 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/src/async_wrapper/convert/_sync.py
+-rw-r--r--   0        0        0     1261 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/src/async_wrapper/convert/abc.py
+-rw-r--r--   0        0        0     1101 2023-08-02 13:46:03.961418 async_wrapper-0.4.1/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:46:03.961418 async_wrapper-0.4.1/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0      151 2023-08-02 13:46:03.961418 async_wrapper-0.4.1/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0      104 2023-08-02 13:46:03.961418 async_wrapper-0.4.1/src/async_wrapper/task_group/exception.py
+-rw-r--r--   0        0        0     4440 2023-08-02 13:46:03.961418 async_wrapper-0.4.1/src/async_wrapper/task_group/task_group.py
+-rw-r--r--   0        0        0     1354 2023-08-02 13:46:03.961418 async_wrapper-0.4.1/src/async_wrapper/task_group/value.py
+-rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 async_wrapper-0.4.1/PKG-INFO
```

### Comparing `async_wrapper-0.3.2/LICENSE` & `async_wrapper-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.2/README.md` & `async_wrapper-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.2/pyproject.toml` & `async_wrapper-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.3.2"
+version = "0.4.1"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 typing-extensions = "^4.6.3"
 anyio = "^3.7.0"
-loky = { version = "^3.4.0", optional = true }
-cloudpickle = { version = "^2.2.1", optional = true }
-psutil = { version = "^5.9.5", optional = true }
 uvloop = { version = "^0.17.0", optional = true, markers = "platform_system != 'Windows'" }
 
 [tool.poetry.extras]
-all = ['loky', "cloudpickle", "psutil", "uvloop"]
-loky = ['loky', "cloudpickle", "psutil"]
 uvloop = ['uvloop']
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.0.275"
+ruff = "0.0.282"
 black = "23.3.0"
 ipykernel = "^6.23.3"
 pytest = "^7.4.0"
 pre-commit = "^3.3.3"
 trio = "^0.22.2"
 pyyaml = ">=6.0.1"    # cython error
```

### Comparing `async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/_thread.py` & `async_wrapper-0.4.1/src/async_wrapper/convert/_async.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.2/src/async_wrapper/convert/synclib/_thread.py` & `async_wrapper-0.4.1/src/async_wrapper/convert/_sync.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.2/src/async_wrapper/task_group/task_group.py` & `async_wrapper-0.4.1/src/async_wrapper/task_group/task_group.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.2/src/async_wrapper/task_group/value.py` & `async_wrapper-0.4.1/src/async_wrapper/task_group/value.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.2/PKG-INFO` & `async_wrapper-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.3.2
+Version: 0.4.1
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: all
-Provides-Extra: loky
 Provides-Extra: uvloop
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
-Requires-Dist: cloudpickle (>=2.2.1,<3.0.0) ; extra == "all" or extra == "loky"
-Requires-Dist: loky (>=3.4.0,<4.0.0) ; extra == "all" or extra == "loky"
-Requires-Dist: psutil (>=5.9.5,<6.0.0) ; extra == "all" or extra == "loky"
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
-Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; (platform_system != "Windows") and (extra == "all" or extra == "uvloop")
+Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; (platform_system != "Windows") and (extra == "uvloop")
 Project-URL: Repository, https://github.com/phi-friday/async-wrapper
 Description-Content-Type: text/markdown
 
 # async-wrapper
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![github action](https://github.com/phi-friday/async-wrapper/actions/workflows/check.yaml/badge.svg?event=push&branch=dev)](#)
```

