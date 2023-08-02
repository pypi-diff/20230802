# Comparing `tmp/dask_awkward-2023.8.0.tar.gz` & `tmp/dask_awkward-2023.8.1.tar.gz`

## Comparing `dask_awkward-2023.8.0.tar` & `dask_awkward-2023.8.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/_utils.py
--rw-r--r--   0        0        0    77173 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    16591 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    30209 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/unproject_layout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    17007 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/LICENSE
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/README.md
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/pyproject.toml
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/_utils.py
+-rw-r--r--   0        0        0    77173 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    16591 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    30209 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/unproject_layout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    17007 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/LICENSE
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 dask_awkward-2023.8.1/PKG-INFO
```

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/__init__.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from dask_awkward import config  # isort:skip; load awkward config
-
 from dask_awkward.lib.core import Array, PartitionCompatibility, Record, Scalar
 from dask_awkward.lib.core import _type as type
 from dask_awkward.lib.core import (
     compatible_partitions,
     map_partitions,
     partition_compatibility,
     typetracer_from_form,
@@ -82,8 +80,7 @@
     with_field,
     with_name,
     with_parameter,
     without_parameters,
     zeros_like,
     zip,
 )
-from dask_awkward.version import __version__
```

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.8.1/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/typing.py` & `dask_awkward-2023.8.1/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/utils.py` & `dask_awkward-2023.8.1/src/dask_awkward/utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.8.1/src/dask_awkward/layers/layers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.8.1/src/dask_awkward/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+from dask_awkward import config  # isort:skip; load awkward config
+
+import dask_awkward.lib.core as core
+import dask_awkward.lib.describe as describe
+import dask_awkward.lib.inspect as inspect
+import dask_awkward.lib.operations as operations
+import dask_awkward.lib.optimize as optimize
+import dask_awkward.lib.reducers as reducers
+import dask_awkward.lib.structure as structure
 from dask_awkward.lib.core import Array, PartitionCompatibility, Record, Scalar
 from dask_awkward.lib.core import _type as type
 from dask_awkward.lib.core import (
     compatible_partitions,
     map_partitions,
     partition_compatibility,
     typetracer_from_form,
@@ -80,7 +89,8 @@
     with_field,
     with_name,
     with_parameter,
     without_parameters,
     zeros_like,
     zip,
 )
+from dask_awkward.version import __version__
```

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/_utils.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/_utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/core.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/core.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/inspect.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/inspect.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/operations.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/optimize.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/optimize.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/reducers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/structure.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/unproject_layout.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/unproject_layout.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/io/io.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/io/json.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.8.1/src/dask_awkward/lib/io/parquet.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/.gitignore` & `dask_awkward-2023.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/LICENSE` & `dask_awkward-2023.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/README.md` & `dask_awkward-2023.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.8.0/pyproject.toml` & `dask_awkward-2023.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -49,19 +49,22 @@
   "dask-awkward[complete]",
   "dask-sphinx-theme >=3.0.2",
   "sphinx-design",
   "requests >=2.27.1",
 ]
 test = [
   "dask-awkward[complete]",
+  "dask-histogram",
   "distributed",
+  "hist",
   "pandas",
   "pytest >=6.0",
   "pytest-cov >=3.0.0",
   "requests >=2.27.1",
+  "uproot",
 ]
 
 [project.entry-points."dask.sizeof"]
 awkward = "dask_awkward.sizeof:register"
 
 [tool.hatch.version]
 source = "vcs"
```

### Comparing `dask_awkward-2023.8.0/PKG-INFO` & `dask_awkward-2023.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.8.0
+Version: 2023.8.1
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
@@ -27,19 +27,22 @@
 Requires-Dist: requests>=2.27.1; extra == 'docs'
 Requires-Dist: sphinx-design; extra == 'docs'
 Provides-Extra: io
 Requires-Dist: aiohttp; extra == 'io'
 Requires-Dist: pyarrow; extra == 'io'
 Provides-Extra: test
 Requires-Dist: dask-awkward[complete]; extra == 'test'
+Requires-Dist: dask-histogram; extra == 'test'
 Requires-Dist: distributed; extra == 'test'
+Requires-Dist: hist; extra == 'test'
 Requires-Dist: pandas; extra == 'test'
 Requires-Dist: pytest-cov>=3.0.0; extra == 'test'
 Requires-Dist: pytest>=6.0; extra == 'test'
 Requires-Dist: requests>=2.27.1; extra == 'test'
+Requires-Dist: uproot; extra == 'test'
 Description-Content-Type: text/markdown
 
 dask-awkward
 ============
 
 > Connecting [awkward-array](https://awkward-array.org) and
 [Dask](https://dask.org/).
```

