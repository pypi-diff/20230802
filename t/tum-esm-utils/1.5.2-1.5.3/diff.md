# Comparing `tmp/tum_esm_utils-1.5.2.tar.gz` & `tmp/tum_esm_utils-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_utils-1.5.2.tar", max compression
+gzip compressed data, was "tum_esm_utils-1.5.3.tar", max compression
```

## Comparing `tum_esm_utils-1.5.2.tar` & `tum_esm_utils-1.5.3.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0    34523 2023-03-19 02:25:01.728953 tum_esm_utils-1.5.2/LICENSE
--rw-r--r--   0        0        0     1480 2023-05-08 20:48:53.107394 tum_esm_utils-1.5.2/README.md
--rw-r--r--   0        0        0     1405 2023-05-08 20:50:40.883720 tum_esm_utils-1.5.2/pyproject.toml
--rw-r--r--   0        0        0      484 2023-05-08 20:20:03.808107 tum_esm_utils-1.5.2/tum_esm_utils/__init__.py
--rw-r--r--   0        0        0      661 2023-05-08 20:26:45.351232 tum_esm_utils-1.5.2/tum_esm_utils/context.py
--rw-r--r--   0        0        0     3252 2023-05-08 20:27:26.142823 tum_esm_utils-1.5.2/tum_esm_utils/datastructures.py
--rw-r--r--   0        0        0     1174 2023-05-08 20:28:19.090171 tum_esm_utils-1.5.2/tum_esm_utils/decorators.py
--rw-r--r--   0        0        0     3877 2023-05-08 20:30:33.784545 tum_esm_utils-1.5.2/tum_esm_utils/files.py
--rw-r--r--   0        0        0      717 2023-05-08 20:35:56.495234 tum_esm_utils-1.5.2/tum_esm_utils/github.py
--rw-r--r--   0        0        0       64 2023-04-25 03:34:37.353328 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/.gitignore
--rw-r--r--   0        0        0     2462 2023-03-24 21:29:53.767147 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
--rw-r--r--   0        0        0     2459 2023-03-24 21:29:53.777058 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/glob_prepro4.F90
--rw-r--r--   0        0        0    28408 2023-04-25 03:08:42.468142 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/ifg_parser.F90
--rw-r--r--   0        0        0      758 2023-04-25 02:57:45.344815 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/ifg_parser.template.inp
--rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.798327 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/refspec.dat
--rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.802664 tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/refspec2.dat
--rw-r--r--   0        0        0     4860 2023-05-08 20:38:33.304237 tum_esm_utils-1.5.2/tum_esm_utils/interferograms.py
--rw-r--r--   0        0        0     7975 2023-05-08 20:39:29.079052 tum_esm_utils-1.5.2/tum_esm_utils/logger.py
--rw-r--r--   0        0        0      380 2023-05-08 20:39:43.895368 tum_esm_utils-1.5.2/tum_esm_utils/mathematics.py
--rw-r--r--   0        0        0     1696 2023-05-08 20:40:10.752208 tum_esm_utils-1.5.2/tum_esm_utils/processes.py
--rw-r--r--   0        0        0        0 2023-03-18 12:27:05.965015 tum_esm_utils-1.5.2/tum_esm_utils/py.typed
--rw-r--r--   0        0        0     3098 2023-05-08 20:41:20.520764 tum_esm_utils-1.5.2/tum_esm_utils/shell.py
--rw-r--r--   0        0        0     1465 2023-05-08 20:42:11.004755 tum_esm_utils-1.5.2/tum_esm_utils/system.py
--rw-r--r--   0        0        0     1276 2023-05-08 20:43:17.097835 tum_esm_utils-1.5.2/tum_esm_utils/testing.py
--rw-r--r--   0        0        0     3362 2023-05-08 20:45:20.705055 tum_esm_utils-1.5.2/tum_esm_utils/text.py
--rw-r--r--   0        0        0     6912 2023-05-08 20:46:28.696498 tum_esm_utils-1.5.2/tum_esm_utils/validators.py
--rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 tum_esm_utils-1.5.2/setup.py
--rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 tum_esm_utils-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-08-02 15:33:55.474182 tum_esm_utils-1.5.3/LICENSE
+-rw-r--r--   0        0        0     1480 2023-08-02 15:33:55.474299 tum_esm_utils-1.5.3/README.md
+-rw-r--r--   0        0        0     1366 2023-08-02 15:36:02.377867 tum_esm_utils-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0      484 2023-08-02 15:33:55.495835 tum_esm_utils-1.5.3/tum_esm_utils/__init__.py
+-rw-r--r--   0        0        0      661 2023-08-02 15:33:55.495899 tum_esm_utils-1.5.3/tum_esm_utils/context.py
+-rw-r--r--   0        0        0     3252 2023-08-02 15:33:55.495978 tum_esm_utils-1.5.3/tum_esm_utils/datastructures.py
+-rw-r--r--   0        0        0     1174 2023-08-02 15:33:55.496039 tum_esm_utils-1.5.3/tum_esm_utils/decorators.py
+-rw-r--r--   0        0        0     3877 2023-08-02 15:33:55.496108 tum_esm_utils-1.5.3/tum_esm_utils/files.py
+-rw-r--r--   0        0        0      717 2023-08-02 15:33:55.496172 tum_esm_utils-1.5.3/tum_esm_utils/github.py
+-rw-r--r--   0        0        0       64 2023-08-02 15:33:55.496271 tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/.gitignore
+-rw-r--r--   0        0        0     2462 2023-08-02 15:33:55.496337 tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
+-rw-r--r--   0        0        0     2459 2023-08-02 15:33:55.496400 tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/glob_prepro4.F90
+-rw-r--r--   0        0        0    28408 2023-08-02 15:33:55.496530 tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/ifg_parser.F90
+-rw-r--r--   0        0        0      758 2023-08-02 15:33:55.496606 tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/ifg_parser.template.inp
+-rw-r--r--   0        0        0   983040 2023-08-02 15:33:55.499240 tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/refspec.dat
+-rw-r--r--   0        0        0   983040 2023-08-02 15:33:55.501952 tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/refspec2.dat
+-rw-r--r--   0        0        0     4860 2023-08-02 15:33:55.502051 tum_esm_utils-1.5.3/tum_esm_utils/interferograms.py
+-rw-r--r--   0        0        0     7975 2023-08-02 15:33:55.502164 tum_esm_utils-1.5.3/tum_esm_utils/logger.py
+-rw-r--r--   0        0        0      380 2023-08-02 15:33:55.502224 tum_esm_utils-1.5.3/tum_esm_utils/mathematics.py
+-rw-r--r--   0        0        0     1696 2023-08-02 15:33:55.502290 tum_esm_utils-1.5.3/tum_esm_utils/processes.py
+-rw-r--r--   0        0        0        0 2023-08-02 15:33:55.502312 tum_esm_utils-1.5.3/tum_esm_utils/py.typed
+-rw-r--r--   0        0        0     3098 2023-08-02 15:33:55.502402 tum_esm_utils-1.5.3/tum_esm_utils/shell.py
+-rw-r--r--   0        0        0     1465 2023-08-02 15:33:55.502464 tum_esm_utils-1.5.3/tum_esm_utils/system.py
+-rw-r--r--   0        0        0     1276 2023-08-02 15:33:55.502527 tum_esm_utils-1.5.3/tum_esm_utils/testing.py
+-rw-r--r--   0        0        0     3362 2023-08-02 15:33:55.502591 tum_esm_utils-1.5.3/tum_esm_utils/text.py
+-rw-r--r--   0        0        0     6912 2023-08-02 15:33:55.502669 tum_esm_utils-1.5.3/tum_esm_utils/validators.py
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 tum_esm_utils-1.5.3/PKG-INFO
```

### Comparing `tum_esm_utils-1.5.2/LICENSE` & `tum_esm_utils-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/README.md` & `tum_esm_utils-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/pyproject.toml` & `tum_esm_utils-1.5.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 [tool.poetry]
 name = "tum_esm_utils"
-version = "1.5.2"
+version = "1.5.3"
 description = "Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich"
 authors = ["Moritz Makowski <moritz.makowski@tum.de>"]
 readme = "README.md"
 packages = [
-    {include = "tum_esm_utils"},
-    {include = "tum_esm_utils/py.typed"}
-]
-keywords = [
-    "python",
-    "library",
-    "utilities",
-    "lazydocs",
-    "docsify"
+    { include = "tum_esm_utils" },
+    { include = "tum_esm_utils/py.typed" },
 ]
+keywords = ["python", "library", "utilities", "lazydocs", "docsify"]
 license = "AGPL-3.0-only"
 documentation = "https://tum-esm.github.io/utils"
 repository = "https://github.com/tum-esm/utils"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 filelock = "^3.10.0"
 requests = "^2.28.2"
 psutil = "^5.9.4"
 pendulum = "^2.1.2"
-polars = "^0.17.11"
+polars = "^0.18.11"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pytest = "^7.2.2"
@@ -38,29 +32,22 @@
 types-requests = "^2.28.11.15"
 pytest-ordering = "^0.6"
 pydocstyle = "^6.3.0"
 lazydocs = "^0.4.8"
 
 
 [tool.pytest.ini_options]
-filterwarnings = [
-    "ignore::pytest.PytestUnhandledThreadExceptionWarning"
-]
-markers = [
-    "last: provided by the `pytest-ordering` library"
-]
+filterwarnings = ["ignore::pytest.PytestUnhandledThreadExceptionWarning"]
+markers = ["last: provided by the `pytest-ordering` library"]
 
 [tool.mypy]
 strict = true
 implicit_reexport = true
 no_warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
-module = [
-    "pendulum",
-    "polars"
-]
+module = ["pendulum", "polars"]
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/context.py` & `tum_esm_utils-1.5.3/tum_esm_utils/context.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/datastructures.py` & `tum_esm_utils-1.5.3/tum_esm_utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/decorators.py` & `tum_esm_utils-1.5.3/tum_esm_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/files.py` & `tum_esm_utils-1.5.3/tum_esm_utils/files.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/github.py` & `tum_esm_utils-1.5.3/tum_esm_utils/github.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/glob_OPUSparms.F90` & `tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/glob_OPUSparms.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/glob_prepro4.F90` & `tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/glob_prepro4.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/ifg_parser.F90` & `tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/ifg_parser.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/ifg_parser.template.inp` & `tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/ifg_parser.template.inp`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/refspec.dat` & `tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/refspec.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/ifg_parser/refspec2.dat` & `tum_esm_utils-1.5.3/tum_esm_utils/ifg_parser/refspec2.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/interferograms.py` & `tum_esm_utils-1.5.3/tum_esm_utils/interferograms.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/logger.py` & `tum_esm_utils-1.5.3/tum_esm_utils/logger.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/processes.py` & `tum_esm_utils-1.5.3/tum_esm_utils/processes.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/shell.py` & `tum_esm_utils-1.5.3/tum_esm_utils/shell.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/system.py` & `tum_esm_utils-1.5.3/tum_esm_utils/system.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/testing.py` & `tum_esm_utils-1.5.3/tum_esm_utils/testing.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/text.py` & `tum_esm_utils-1.5.3/tum_esm_utils/text.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/tum_esm_utils/validators.py` & `tum_esm_utils-1.5.3/tum_esm_utils/validators.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.5.2/PKG-INFO` & `tum_esm_utils-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tum-esm-utils
-Version: 1.5.2
+Version: 1.5.3
 Summary: Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich
 Home-page: https://github.com/tum-esm/utils
 License: AGPL-3.0-only
 Keywords: python,library,utilities,lazydocs,docsify
 Author: Moritz Makowski
 Author-email: moritz.makowski@tum.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: filelock (>=3.10.0,<4.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
-Requires-Dist: polars (>=0.17.11,<0.18.0)
+Requires-Dist: polars (>=0.18.11,<0.19.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Documentation, https://tum-esm.github.io/utils
 Project-URL: Repository, https://github.com/tum-esm/utils
 Description-Content-Type: text/markdown
 
 # 🔬 &nbsp;TUM ESM Python Utilities
```

