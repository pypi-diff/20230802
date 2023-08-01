# Comparing `tmp/photerr-1.1.0.tar.gz` & `tmp/photerr-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photerr-1.1.0.tar", max compression
+gzip compressed data, was "photerr-1.1.1.tar", max compression
```

## Comparing `photerr-1.1.0.tar` & `photerr-1.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1079 2023-04-26 05:38:04.335104 photerr-1.1.0/LICENSE
--rw-r--r--   0        0        0    11784 2023-04-26 05:38:04.335104 photerr-1.1.0/README.md
--rw-r--r--   0        0        0      337 2023-04-26 05:38:04.335104 photerr-1.1.0/photerr/__init__.py
--rw-r--r--   0        0        0     1362 2023-04-26 05:38:04.335104 photerr-1.1.0/photerr/euclid.py
--rw-r--r--   0        0        0     2218 2023-04-26 05:38:04.335104 photerr-1.1.0/photerr/lsst.py
--rw-r--r--   0        0        0    18351 2023-04-26 05:38:04.335104 photerr-1.1.0/photerr/model.py
--rw-r--r--   0        0        0    19273 2023-04-26 05:38:04.335104 photerr-1.1.0/photerr/params.py
--rw-r--r--   0        0        0     1424 2023-04-26 05:38:04.335104 photerr-1.1.0/photerr/roman.py
--rw-r--r--   0        0        0     1312 2023-04-26 05:38:04.339104 photerr-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    12414 1970-01-01 00:00:00.000000 photerr-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-08-01 23:40:17.858289 photerr-1.1.1/LICENSE
+-rw-r--r--   0        0        0    11784 2023-08-01 23:40:17.858289 photerr-1.1.1/README.md
+-rw-r--r--   0        0        0      337 2023-08-01 23:40:17.858289 photerr-1.1.1/photerr/__init__.py
+-rw-r--r--   0        0        0     1363 2023-08-01 23:40:17.858289 photerr-1.1.1/photerr/euclid.py
+-rw-r--r--   0        0        0     2250 2023-08-01 23:40:17.858289 photerr-1.1.1/photerr/lsst.py
+-rw-r--r--   0        0        0    18351 2023-08-01 23:40:17.858289 photerr-1.1.1/photerr/model.py
+-rw-r--r--   0        0        0    19281 2023-08-01 23:40:17.858289 photerr-1.1.1/photerr/params.py
+-rw-r--r--   0        0        0     1425 2023-08-01 23:40:17.858289 photerr-1.1.1/photerr/roman.py
+-rw-r--r--   0        0        0     1312 2023-08-01 23:40:17.858289 photerr-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12414 1970-01-01 00:00:00.000000 photerr-1.1.1/PKG-INFO
```

### Comparing `photerr-1.1.0/LICENSE` & `photerr-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `photerr-1.1.0/README.md` & `photerr-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `photerr-1.1.0/photerr/euclid.py` & `photerr-1.1.1/photerr/euclid.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     gamma: Dict[str, float] = field(
         default_factory=lambda: {
             "Y": 0.04,
             "J": 0.04,
             "H": 0.04,
         }
     )
+
     m5: Dict[str, float] = field(
         default_factory=lambda: {
             "Y": 24.0,
             "J": 24.2,
             "H": 23.9,
         }
     )
```

### Comparing `photerr-1.1.0/photerr/lsst.py` & `photerr-1.1.1/photerr/lsst.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Photometric error model for LSST."""
 from dataclasses import dataclass, field
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from photerr.model import ErrorModel
 from photerr.params import ErrorParams, param_docstring
 
 
 @dataclass
 class LsstErrorParams(ErrorParams):
     """Parameters for the LSST photometric error model.
 
     Default values taken from pages 11, 12, 26 of Ivezic 2019.
     """
 
     __doc__ += param_docstring
 
-    tvis: float = 30.0
     nYrObs: float = 10.0
     nVisYr: Dict[str, float] = field(
         default_factory=lambda: {
             "u": 5.6,
             "g": 8.0,
             "r": 18.4,
             "i": 18.4,
@@ -33,16 +32,19 @@
             "g": 0.039,
             "r": 0.039,
             "i": 0.039,
             "z": 0.039,
             "y": 0.039,
         }
     )
-    airmass: float = 1.2
+
     m5: Dict[str, float] = field(default_factory=lambda: {})
+
+    tvis: Optional[float] = 30.0
+    airmass: Optional[float] = 1.2
     Cm: Dict[str, float] = field(
         default_factory=lambda: {
             "u": 23.09,
             "g": 24.42,
             "r": 24.44,
             "i": 24.32,
             "z": 24.16,
```

### Comparing `photerr-1.1.0/photerr/model.py` & `photerr-1.1.1/photerr/model.py`

 * *Files identical despite different names*

### Comparing `photerr-1.1.0/photerr/params.py` & `photerr-1.1.1/photerr/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Parameter objects for the error model."""
 from __future__ import annotations
 
 from copy import deepcopy
 from dataclasses import InitVar, dataclass, field
-from typing import Any, Dict, Union
+from typing import Any, Dict, Optional, Union
 
 import numpy as np
 
 param_docstring = """
 
     Parameters
     ----------
@@ -181,16 +181,16 @@
 
     nYrObs: float
     nVisYr: Dict[str, float]
     gamma: Dict[str, float]
 
     m5: Dict[str, float] = field(default_factory=lambda: {})
 
-    tvis: float = None  # type: ignore
-    airmass: float = None  # type: ignore
+    tvis: Optional[float] = None
+    airmass: Optional[float] = None
     Cm: Dict[str, float] = field(default_factory=lambda: {})
     msky: Dict[str, float] = field(default_factory=lambda: {})
     theta: Dict[str, float] = field(default_factory=lambda: {})
     km: Dict[str, float] = field(default_factory=lambda: {})
 
     sigmaSys: float = 0.005
 
@@ -207,15 +207,15 @@
 
     decorrelate: bool = True
     highSNR: bool = False
     scale: Dict[str, float] = field(default_factory=lambda: {})
 
     errLoc: str = "after"
 
-    renameDict: InitVar[Dict[str, str]] = None
+    renameDict: InitVar[Optional[Dict[str, str]]] = None
     validate: InitVar[bool] = True
 
     def __post_init__(
         self, renameDict: Union[Dict[str, str], None], validate: bool
     ) -> None:
         """Rename bands and remove duplicate parameters."""
         # if renameDict was provided, rename the bands
```

### Comparing `photerr-1.1.0/photerr/roman.py` & `photerr-1.1.1/photerr/roman.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         default_factory=lambda: {
             "Y": 0.04,
             "J": 0.04,
             "H": 0.04,
             "F": 0.04,
         }
     )
+
     m5: Dict[str, float] = field(
         default_factory=lambda: {
             "Y": 26.9,
             "J": 26.95,
             "H": 26.9,
             "F": 26.25,
         }
```

### Comparing `photerr-1.1.0/pyproject.toml` & `photerr-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "photerr"
-version = "1.1.0"
+version = "1.1.1"
 description = "Photometric error model for astronomical imaging surveys"
 authors = ["John Franklin Crenshaw <jfcrenshaw@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jfcrenshaw/photerr"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `photerr-1.1.0/PKG-INFO` & `photerr-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photerr
-Version: 1.1.0
+Version: 1.1.1
 Summary: Photometric error model for astronomical imaging surveys
 Home-page: https://github.com/jfcrenshaw/photerr
 Author: John Franklin Crenshaw
 Author-email: jfcrenshaw@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

