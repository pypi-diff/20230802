# Comparing `tmp/pitot-0.3.0.tar.gz` & `tmp/pitot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pitot-0.3.0.tar", max compression
+gzip compressed data, was "pitot-0.3.1.tar", max compression
```

## Comparing `pitot-0.3.0.tar` & `pitot-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1080 2023-07-24 13:23:13.766199 pitot-0.3.0/license.txt
--rw-r--r--   0        0        0     2453 2023-07-24 13:23:13.770199 pitot-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1998 2023-07-24 13:23:13.770199 pitot-0.3.0/readme.md
--rw-r--r--   0        0        0      410 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/__init__.py
--rw-r--r--   0        0        0     3537 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/aero.py
--rw-r--r--   0        0        0      885 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/airac.py
--rw-r--r--   0        0        0     3610 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/geodesy.py
--rw-r--r--   0        0        0     2604 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/geodesy.pyi
--rw-r--r--   0        0        0     4314 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/isa.py
--rw-r--r--   0        0        0        0 2023-07-24 13:23:13.770199 pitot-0.3.0/src/pitot/py.typed
--rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 pitot-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-08-02 21:32:54.189161 pitot-0.3.1/license.txt
+-rw-r--r--   0        0        0     2410 2023-08-02 21:32:54.193162 pitot-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1998 2023-08-02 21:32:54.193162 pitot-0.3.1/readme.md
+-rw-r--r--   0        0        0      410 2023-08-02 21:32:54.193162 pitot-0.3.1/src/pitot/__init__.py
+-rw-r--r--   0        0        0     3537 2023-08-02 21:32:54.193162 pitot-0.3.1/src/pitot/aero.py
+-rw-r--r--   0        0        0      885 2023-08-02 21:32:54.193162 pitot-0.3.1/src/pitot/airac.py
+-rw-r--r--   0        0        0     3610 2023-08-02 21:32:54.193162 pitot-0.3.1/src/pitot/geodesy.py
+-rw-r--r--   0        0        0     3169 2023-08-02 21:32:54.193162 pitot-0.3.1/src/pitot/geodesy.pyi
+-rw-r--r--   0        0        0     4314 2023-08-02 21:32:54.193162 pitot-0.3.1/src/pitot/isa.py
+-rw-r--r--   0        0        0        0 2023-08-02 21:32:54.193162 pitot-0.3.1/src/pitot/py.typed
+-rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 pitot-0.3.1/PKG-INFO
```

### Comparing `pitot-0.3.0/license.txt` & `pitot-0.3.1/license.txt`

 * *Files identical despite different names*

### Comparing `pitot-0.3.0/pyproject.toml` & `pitot-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pitot"
-version = "0.3.0"
+version = "0.3.1"
 description = "Toolbox for aeronautic units and conversions"
 authors = ["Xavier Olive <git@xoolive.org>", "Junzi Sun <junzisun@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Information Technology",
@@ -27,33 +27,32 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = ">=1.23.0"
 pandas = ">=1.4.3"
 typing-extensions = ">=4.3.0"
 pyproj = ">=3.3.1"
-impunity = ">=1.0.2"
+impunity = ">=1.0.3"
 # impunity = { path = "../impunity", develop = true }
 
 [tool.poetry.group.dev.dependencies]
 mypy = ">=0.991"
-isort = ">=5.10.1"
 black = ">=22.12.0"
 pytest = ">=7.1.2"
 pytest-cov = ">=4.0.0"
 pre-commit = ">=2.20.0"
-ruff = "^0.0.253"
+ruff = ">=0.0.253"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 80
-target_version = ['py37', 'py38', 'py39']
+target_version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''
 /(
     __pycache__
   | \.git
   | \.mypy_cache
   | \.ipynb_checkpoints
@@ -74,17 +73,14 @@
 ]
 line-length = 80
 target-version = "py38"
 
 [tool.ruff.isort]
 known-first-party = ["numpy", "pandas", "pyproj", "shapely"]
 
-# [tool.isort]
-# skip = ["*.pyi"]
-
 [tool.mypy]
 python_version = 3.8
 platform = "posix"
 
 color_output = true
 pretty = true
 show_column_numbers = true
```

### Comparing `pitot-0.3.0/readme.md` & `pitot-0.3.1/readme.md`

 * *Files identical despite different names*

### Comparing `pitot-0.3.0/src/pitot/aero.py` & `pitot-0.3.1/src/pitot/aero.py`

 * *Files identical despite different names*

### Comparing `pitot-0.3.0/src/pitot/airac.py` & `pitot-0.3.1/src/pitot/airac.py`

 * *Files identical despite different names*

### Comparing `pitot-0.3.0/src/pitot/geodesy.py` & `pitot-0.3.1/src/pitot/geodesy.py`

 * *Files identical despite different names*

### Comparing `pitot-0.3.0/src/pitot/geodesy.pyi` & `pitot-0.3.1/src/pitot/geodesy.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,29 @@
 ) -> tuple[
     Annotated[float, "degree"],
     Annotated[float, "degree"],
     Annotated[float, "degree"],
 ]: ...
 @overload
 def destination(
+    lon: Annotated[float | Sequence[float] | npt.NDArray[np.float64], "degree"],
+    lat: Annotated[float | Sequence[float] | npt.NDArray[np.float64], "degree"],
+    bearing: Annotated[
+        float | Sequence[float] | npt.NDArray[np.float64], "degree"
+    ],
+    distance: Annotated[Sequence[float] | npt.NDArray[np.float64], "m"],
+    *args: Any,
+    **kwargs: Any,
+) -> tuple[
+    Annotated[npt.NDArray[np.float64], "degree"],
+    Annotated[npt.NDArray[np.float64], "degree"],
+    Annotated[npt.NDArray[np.float64], "degree"],
+]: ...
+@overload
+def destination(
     lon: Annotated[Sequence[float] | npt.NDArray[np.float64], "degree"],
     lat: Annotated[Sequence[float] | npt.NDArray[np.float64], "degree"],
     bearing: Annotated[
         float | Sequence[float] | npt.NDArray[np.float64], "degree"
     ],
     distance: Annotated[float | Sequence[float] | npt.NDArray[np.float64], "m"],
     *args: Any,
```

### Comparing `pitot-0.3.0/src/pitot/isa.py` & `pitot-0.3.1/src/pitot/isa.py`

 * *Files identical despite different names*

### Comparing `pitot-0.3.0/PKG-INFO` & `pitot-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pitot
-Version: 0.3.0
+Version: 0.3.1
 Summary: Toolbox for aeronautic units and conversions
 License: MIT
 Author: Xavier Olive
 Author-email: git@xoolive.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Dist: impunity (>=1.0.2)
+Requires-Dist: impunity (>=1.0.3)
 Requires-Dist: numpy (>=1.23.0)
 Requires-Dist: pandas (>=1.4.3)
 Requires-Dist: pyproj (>=3.3.1)
 Requires-Dist: typing-extensions (>=4.3.0)
 Description-Content-Type: text/markdown
 
 # pitot
```

