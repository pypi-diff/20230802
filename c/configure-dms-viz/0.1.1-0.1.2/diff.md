# Comparing `tmp/configure_dms_viz-0.1.1.tar.gz` & `tmp/configure_dms_viz-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configure_dms_viz-0.1.1.tar", max compression
+gzip compressed data, was "configure_dms_viz-0.1.2.tar", max compression
```

## Comparing `configure_dms_viz-0.1.1.tar` & `configure_dms_viz-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2023-08-02 02:00:23.592861 configure_dms_viz-0.1.1/LICENSE
--rw-r--r--   0        0        0    10211 2023-08-02 02:00:23.592861 configure_dms_viz-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-08-02 02:00:23.592861 configure_dms_viz-0.1.1/configure_dms_viz/__init__.py
--rwxr-xr-x   0        0        0    27295 2023-08-02 02:00:23.592861 configure_dms_viz-0.1.1/configure_dms_viz/configure_dms_viz.py
--rw-r--r--   0        0        0     7584 2023-08-02 02:00:23.592861 configure_dms_viz-0.1.1/configure_dms_viz/pdb_utils.py
--rw-r--r--   0        0        0     1103 2023-08-02 02:00:23.592861 configure_dms_viz-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    10838 1970-01-01 00:00:00.000000 configure_dms_viz-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-08-02 16:58:17.001446 configure_dms_viz-0.1.2/LICENSE
+-rw-r--r--   0        0        0    10211 2023-08-02 16:58:17.001446 configure_dms_viz-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 16:58:17.001446 configure_dms_viz-0.1.2/configure_dms_viz/__init__.py
+-rwxr-xr-x   0        0        0    27295 2023-08-02 16:58:17.001446 configure_dms_viz-0.1.2/configure_dms_viz/configure_dms_viz.py
+-rw-r--r--   0        0        0     7584 2023-08-02 16:58:17.001446 configure_dms_viz-0.1.2/configure_dms_viz/pdb_utils.py
+-rw-r--r--   0        0        0     1103 2023-08-02 16:58:17.001446 configure_dms_viz-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 configure_dms_viz-0.1.2/PKG-INFO
```

### Comparing `configure_dms_viz-0.1.1/LICENSE` & `configure_dms_viz-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-0.1.1/README.md` & `configure_dms_viz-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-0.1.1/configure_dms_viz/configure_dms_viz.py` & `configure_dms_viz-0.1.2/configure_dms_viz/configure_dms_viz.py`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-0.1.1/configure_dms_viz/pdb_utils.py` & `configure_dms_viz-0.1.2/configure_dms_viz/pdb_utils.py`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-0.1.1/pyproject.toml` & `configure_dms_viz-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "configure-dms-viz"
-version = "0.1.1"
+version = "0.1.2"
 description = "Configure your data for visualization with dms-viz.github.io"
 authors = ["Will Hannon <hannonww@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "configure_dms_viz" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.6"
-pandas = "^2.0.3"
-biopython = "^1.81"
-requests = "^2.31.0"
+pandas = ">=2.0.0"
+biopython = ">=1.0"
+requests = ">2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 ruff = "^0.0.282"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `configure_dms_viz-0.1.1/PKG-INFO` & `configure_dms_viz-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: configure-dms-viz
-Version: 0.1.1
+Version: 0.1.2
 Summary: Configure your data for visualization with dms-viz.github.io
 License: MIT
 Author: Will Hannon
 Author-email: hannonww@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: biopython (>=1.81,<2.0)
+Requires-Dist: biopython (>=1.0)
 Requires-Dist: click (>=8.1.6,<9.0.0)
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: pandas (>=2.0.0)
+Requires-Dist: requests (>2.0.0)
 Description-Content-Type: text/markdown
 
 # `configure_dms_viz`
 
 ![License](https://img.shields.io/github/license/matsengrp/multidms)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

