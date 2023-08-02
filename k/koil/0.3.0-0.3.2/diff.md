# Comparing `tmp/koil-0.3.0.tar.gz` & `tmp/koil-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koil-0.3.0.tar", max compression
+gzip compressed data, was "koil-0.3.2.tar", max compression
```

## Comparing `koil-0.3.0.tar` & `koil-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3475 2022-03-02 12:09:12.548451 koil-0.3.0/README.md
--rw-r--r--   0        0        0      359 2022-04-12 08:39:04.407565 koil-0.3.0/koil/__init__.py
--rw-r--r--   0        0        0      116 2023-02-06 15:33:56.814184 koil-0.3.0/koil/composition/__init__.py
--rw-r--r--   0        0        0     2978 2023-07-26 13:35:45.096944 koil-0.3.0/koil/composition/base.py
--rw-r--r--   0        0        0     1052 2022-11-21 11:44:34.168046 koil-0.3.0/koil/composition/qt.py
--rw-r--r--   0        0        0     2980 2023-07-26 09:17:59.601113 koil-0.3.0/koil/decorators.py
--rw-r--r--   0        0        0      771 2023-07-19 16:54:53.430108 koil-0.3.0/koil/errors.py
--rw-r--r--   0        0        0    10113 2023-08-02 10:19:59.698656 koil-0.3.0/koil/helpers.py
--rw-r--r--   0        0        0     5131 2023-07-26 09:20:25.845722 koil-0.3.0/koil/koil.py
--rw-r--r--   0        0        0     1014 2023-07-19 14:15:35.493961 koil-0.3.0/koil/predicates.py
--rw-r--r--   0        0        0     8909 2023-08-02 09:46:40.942885 koil-0.3.0/koil/process.py
--rw-r--r--   0        0        0    10689 2023-07-26 09:17:59.909114 koil-0.3.0/koil/qt.py
--rw-r--r--   0        0        0     4501 2022-11-21 11:44:34.184046 koil-0.3.0/koil/task.py
--rw-r--r--   0        0        0      391 2022-03-28 11:51:32.994673 koil-0.3.0/koil/types.py
--rw-r--r--   0        0        0     6824 2022-03-25 16:39:20.667020 koil-0.3.0/koil/utils.py
--rw-r--r--   0        0        0     1164 2023-08-02 09:53:47.865048 koil-0.3.0/koil/vars.py
--rw-r--r--   0        0        0     1103 2023-08-02 11:58:11.021788 koil-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4256 1970-01-01 00:00:00.000000 koil-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3475 2022-03-02 12:09:12.548451 koil-0.3.2/README.md
+-rw-r--r--   0        0        0      359 2022-04-12 08:39:04.407565 koil-0.3.2/koil/__init__.py
+-rw-r--r--   0        0        0      116 2023-02-06 15:33:56.814184 koil-0.3.2/koil/composition/__init__.py
+-rw-r--r--   0        0        0     2978 2023-07-26 13:35:45.096944 koil-0.3.2/koil/composition/base.py
+-rw-r--r--   0        0        0     1052 2022-11-21 11:44:34.168046 koil-0.3.2/koil/composition/qt.py
+-rw-r--r--   0        0        0     2980 2023-07-26 09:17:59.601113 koil-0.3.2/koil/decorators.py
+-rw-r--r--   0        0        0      771 2023-07-19 16:54:53.430108 koil-0.3.2/koil/errors.py
+-rw-r--r--   0        0        0    10113 2023-08-02 10:19:59.698656 koil-0.3.2/koil/helpers.py
+-rw-r--r--   0        0        0     5131 2023-07-26 09:20:25.845722 koil-0.3.2/koil/koil.py
+-rw-r--r--   0        0        0     1014 2023-07-19 14:15:35.493961 koil-0.3.2/koil/predicates.py
+-rw-r--r--   0        0        0     8909 2023-08-02 09:46:40.942885 koil-0.3.2/koil/process.py
+-rw-r--r--   0        0        0    10689 2023-07-26 09:17:59.909114 koil-0.3.2/koil/qt.py
+-rw-r--r--   0        0        0     4501 2022-11-21 11:44:34.184046 koil-0.3.2/koil/task.py
+-rw-r--r--   0        0        0      391 2022-03-28 11:51:32.994673 koil-0.3.2/koil/types.py
+-rw-r--r--   0        0        0     6824 2022-03-25 16:39:20.667020 koil-0.3.2/koil/utils.py
+-rw-r--r--   0        0        0     1164 2023-08-02 09:53:47.865048 koil-0.3.2/koil/vars.py
+-rw-r--r--   0        0        0     1183 2023-08-02 12:01:14.266847 koil-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4301 1970-01-01 00:00:00.000000 koil-0.3.2/PKG-INFO
```

### Comparing `koil-0.3.0/README.md` & `koil-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/koil/composition/base.py` & `koil-0.3.2/koil/composition/base.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/koil/composition/qt.py` & `koil-0.3.2/koil/composition/qt.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/koil/decorators.py` & `koil-0.3.2/koil/decorators.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/koil/errors.py` & `koil-0.3.2/koil/errors.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/koil/helpers.py` & `koil-0.3.2/koil/helpers.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/koil/koil.py` & `koil-0.3.2/koil/koil.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/koil/predicates.py` & `koil-0.3.2/koil/predicates.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/koil/process.py` & `koil-0.3.2/koil/process.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/koil/qt.py` & `koil-0.3.2/koil/qt.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/koil/task.py` & `koil-0.3.2/koil/task.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/koil/utils.py` & `koil-0.3.2/koil/utils.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/koil/vars.py` & `koil-0.3.2/koil/vars.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.0/pyproject.toml` & `koil-0.3.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 [tool.poetry]
 name = "koil"
-version = "0.3.0"
+version = "0.3.2"
 readme = "README.md"
 description = "Async for a sync world"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "koil" }]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 qtpy = { version = ">1", optional = true }
 uvloop = { version = "^0.16.0", optional = true }
 janus = "^1.0.0"
-cloudpickle = "^2.2.1"
+cloudpickle = { version = "^2.2.1", optional = true }
 
 [tool.poetry.extras]
 qtpy = ["qt"]
 uvloop = ["uvloop"]
+process = ["cloudpickle"]
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.2.0"
 black = "^22.10.0"
 pytest-cov = "^4.0.0"
 pytest-qt = "^4.2.0"
 QtPy = "^2.3.0"
 pytest-asyncio = "^0.20.2"
 pydantic = "^1.10.2"
 autoflake = "^1.7.7"
 mypy = "^1.4.1"
+cloudpickle = "^2.2.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
```

### Comparing `koil-0.3.0/PKG-INFO` & `koil-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: koil
-Version: 0.3.0
+Version: 0.3.2
 Summary: Async for a sync world
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: process
 Provides-Extra: qtpy
 Provides-Extra: uvloop
-Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
+Requires-Dist: cloudpickle (>=2.2.1,<3.0.0) ; extra == "process"
 Requires-Dist: janus (>=1.0.0,<2.0.0)
 Requires-Dist: qtpy (>1)
 Requires-Dist: uvloop (>=0.16.0,<0.17.0) ; extra == "uvloop"
 Description-Content-Type: text/markdown
 
 # koil
```

