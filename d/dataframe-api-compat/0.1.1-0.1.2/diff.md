# Comparing `tmp/dataframe_api_compat-0.1.1.tar.gz` & `tmp/dataframe_api_compat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataframe_api_compat-0.1.1.tar", last modified: Tue Aug  1 14:36:56 2023, max compression
+gzip compressed data, was "dataframe_api_compat-0.1.2.tar", last modified: Wed Aug  2 13:19:47 2023, max compression
```

## Comparing `dataframe_api_compat-0.1.1.tar` & `dataframe_api_compat-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2023-05-05 10:36:05.000000 dataframe_api_compat-0.1.1/LICENSE
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1731 2023-08-01 13:22:30.000000 dataframe_api_compat-0.1.1/README.md
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/dataframe_api_compat/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-06-28 15:01:51.000000 dataframe_api_compat-0.1.1/dataframe_api_compat/__init__.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/dataframe_api_compat/pandas_standard/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3707 2023-08-01 14:35:35.000000 dataframe_api_compat-0.1.1/dataframe_api_compat/pandas_standard/__init__.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    28727 2023-08-01 14:33:46.000000 dataframe_api_compat-0.1.1/dataframe_api_compat/pandas_standard/pandas_standard.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/dataframe_api_compat/polars_standard/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3074 2023-08-01 14:35:34.000000 dataframe_api_compat-0.1.1/dataframe_api_compat/polars_standard/__init__.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    25104 2023-08-01 14:35:35.000000 dataframe_api_compat-0.1.1/dataframe_api_compat/polars_standard/polars_standard.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/dataframe_api_compat.egg-info/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-01 14:36:56.000000 dataframe_api_compat-0.1.1/dataframe_api_compat.egg-info/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      470 2023-08-01 14:36:56.000000 dataframe_api_compat-0.1.1/dataframe_api_compat.egg-info/SOURCES.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2023-08-01 14:36:56.000000 dataframe_api_compat-0.1.1/dataframe_api_compat.egg-info/dependency_links.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       21 2023-08-01 14:36:56.000000 dataframe_api_compat-0.1.1/dataframe_api_compat.egg-info/top_level.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      440 2023-08-01 13:41:52.000000 dataframe_api_compat-0.1.1/pyproject.toml
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      835 2023-08-01 14:36:56.694927 dataframe_api_compat-0.1.1/setup.cfg
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       38 2023-05-05 10:36:12.000000 dataframe_api_compat-0.1.1/setup.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2023-05-05 10:36:05.000000 dataframe_api_compat-0.1.2/LICENSE
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/PKG-INFO
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1731 2023-08-02 10:23:41.000000 dataframe_api_compat-0.1.2/README.md
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/dataframe_api_compat/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-06-28 15:01:51.000000 dataframe_api_compat-0.1.2/dataframe_api_compat/__init__.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/dataframe_api_compat/pandas_standard/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     4374 2023-08-02 13:19:17.000000 dataframe_api_compat-0.1.2/dataframe_api_compat/pandas_standard/__init__.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    28820 2023-08-02 13:19:17.000000 dataframe_api_compat-0.1.2/dataframe_api_compat/pandas_standard/pandas_standard.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/dataframe_api_compat/polars_standard/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3287 2023-08-02 10:20:54.000000 dataframe_api_compat-0.1.2/dataframe_api_compat/polars_standard/__init__.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    25207 2023-08-02 13:19:17.000000 dataframe_api_compat-0.1.2/dataframe_api_compat/polars_standard/polars_standard.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/dataframe_api_compat.egg-info/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 13:19:47.000000 dataframe_api_compat-0.1.2/dataframe_api_compat.egg-info/PKG-INFO
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      470 2023-08-02 13:19:47.000000 dataframe_api_compat-0.1.2/dataframe_api_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2023-08-02 13:19:47.000000 dataframe_api_compat-0.1.2/dataframe_api_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       21 2023-08-02 13:19:47.000000 dataframe_api_compat-0.1.2/dataframe_api_compat.egg-info/top_level.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      449 2023-08-02 10:29:22.000000 dataframe_api_compat-0.1.2/pyproject.toml
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      835 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/setup.cfg
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       74 2023-08-02 10:13:15.000000 dataframe_api_compat-0.1.2/setup.py
```

### Comparing `dataframe_api_compat-0.1.1/LICENSE` & `dataframe_api_compat-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.1/PKG-INFO` & `dataframe_api_compat-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataframe_api_compat
-Version: 0.1.1
+Version: 0.1.2
 Summary: Implementation of the DataFrame Standard for pandas and polars
 Home-page: https://github.com/data-apis/dataframe-api-compat
 Author: Marco Gorelli
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 
 # DataFrame API Compat
 
 <h1 align="center">
 	<img
 		width="400"
 		alt="standard-compliant DataFrame"
-		src="https://github.com/data-apis/dataframe-api-compat/assets/33491632/fb4bc907-2b85-4ad7-8d13-c2b9912b97f5">
+		src="https://github.com/data-apis/dataframe-api-compat/assets/33491632/2997cb92-fd10-4426-bd41-8dfd1e466ee2">
 </h1>
 
 Implementation of the [DataFrame Standard](https://data-apis.org/dataframe-api/draft/index.html)
 for pandas and polars.
 
 What's this?
 ------------
```

### Comparing `dataframe_api_compat-0.1.1/README.md` & `dataframe_api_compat-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # DataFrame API Compat
 
 <h1 align="center">
 	<img
 		width="400"
 		alt="standard-compliant DataFrame"
-		src="https://github.com/data-apis/dataframe-api-compat/assets/33491632/fb4bc907-2b85-4ad7-8d13-c2b9912b97f5">
+		src="https://github.com/data-apis/dataframe-api-compat/assets/33491632/2997cb92-fd10-4426-bd41-8dfd1e466ee2">
 </h1>
 
 Implementation of the [DataFrame Standard](https://data-apis.org/dataframe-api/draft/index.html)
 for pandas and polars.
 
 What's this?
 ------------
```

### Comparing `dataframe_api_compat-0.1.1/dataframe_api_compat/pandas_standard/__init__.py` & `dataframe_api_compat-0.1.2/dataframe_api_compat/pandas_standard/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from __future__ import annotations
 
-from typing import (
-    TYPE_CHECKING,
-    Any,
-)
+from typing import Any
+from typing import TYPE_CHECKING
 
 import pandas as pd
 
-from dataframe_api_compat.pandas_standard.pandas_standard import (
-    PandasColumn,
-    PandasDataFrame,
-    PandasGroupBy,
-)
+from dataframe_api_compat.pandas_standard.pandas_standard import PandasColumn
+from dataframe_api_compat.pandas_standard.pandas_standard import PandasDataFrame
+from dataframe_api_compat.pandas_standard.pandas_standard import PandasGroupBy
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
 Column = PandasColumn
 DataFrame = PandasDataFrame
 GroupBy = PandasGroupBy
@@ -153,14 +149,30 @@
 def column_from_sequence(
     sequence: Sequence[Any], *, dtype: Any, name: str | None = None
 ) -> PandasColumn[Any]:
     ser = pd.Series(sequence, dtype=map_standard_dtype_to_pandas_dtype(dtype))
     return PandasColumn(ser, name=name)
 
 
+def column_from_1d_array(
+    array, *, dtype: Any, name: str | None = None
+) -> PandasColumn[Any]:  # pragma: no cover
+    ser = pd.Series(array, dtype=map_standard_dtype_to_pandas_dtype(dtype), name=name)
+    return PandasColumn(ser)
+
+
+def dataframe_from_2d_array(
+    array, *, names: Sequence[str], dtypes: dict[str, Any]
+) -> PandasColumn[Any]:  # pragma: no cover
+    df = pd.DataFrame(array, columns=names).astype(
+        {key: map_standard_dtype_to_pandas_dtype(value) for key, value in dtypes.items()}
+    )
+    return PandasDataFrame(df)
+
+
 def dataframe_from_dict(data: dict[str, PandasColumn[Any]]) -> PandasDataFrame:
     for col_name, col in data.items():
         if not isinstance(col, PandasColumn):  # pragma: no cover
             raise TypeError(f"Expected PandasColumn, got {type(col)}")
         if col.name is not None and col_name != col.name:
             raise ValueError(f"Expected column name {col_name}, got {col.name}")
     return PandasDataFrame(
```

### Comparing `dataframe_api_compat-0.1.1/dataframe_api_compat/pandas_standard/pandas_standard.py` & `dataframe_api_compat-0.1.2/dataframe_api_compat/pandas_standard/pandas_standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from __future__ import annotations
 
 import collections
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Generic,
-    Literal,
-    NoReturn,
-    TypeVar,
-    cast,
-)
+from typing import Any
+from typing import cast
+from typing import Generic
+from typing import Literal
+from typing import NoReturn
+from typing import TYPE_CHECKING
+from typing import TypeVar
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_extension_array_dtype
 
 import dataframe_api_compat.pandas_standard
 
@@ -66,15 +64,15 @@
             and column.index.start == 0  # type: ignore[comparison-overlap]
             and column.index.step == 1  # type: ignore[comparison-overlap]
             and (column.index.stop == len(column))  # type: ignore[comparison-overlap]
         ):
             self._series = column
         else:
             self._series = column.reset_index(drop=True)
-        self._name = name
+        self._name = name  # or column.name
 
     def _validate_index(self, index: pd.Index) -> None:
         pd.testing.assert_index_equal(self.column.index, index)
 
     # In the standard
     def __column_namespace__(self, *, api_version: str | None = None) -> Any:
         return dataframe_api_compat.pandas_standard
```

### Comparing `dataframe_api_compat-0.1.1/dataframe_api_compat/polars_standard/__init__.py` & `dataframe_api_compat-0.1.2/dataframe_api_compat/polars_standard/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+from typing import Any
+from typing import TYPE_CHECKING
 
 import polars as pl
 
-from dataframe_api_compat.polars_standard.polars_standard import (
-    PolarsColumn,
-    PolarsDataFrame,
-    PolarsGroupBy,
-)
+from dataframe_api_compat.polars_standard.polars_standard import null  # noqa: F401
+from dataframe_api_compat.polars_standard.polars_standard import PolarsColumn
+from dataframe_api_compat.polars_standard.polars_standard import PolarsDataFrame
+from dataframe_api_compat.polars_standard.polars_standard import PolarsGroupBy
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
 Column = PolarsColumn
 DataFrame = PolarsDataFrame
 GroupBy = PolarsGroupBy
```

### Comparing `dataframe_api_compat-0.1.1/dataframe_api_compat/polars_standard/polars_standard.py` & `dataframe_api_compat-0.1.2/dataframe_api_compat/polars_standard/polars_standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 import collections
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Generic,
-    Literal,
-    NoReturn,
-    TypeVar,
-)
+from typing import Any
+from typing import Generic
+from typing import Literal
+from typing import NoReturn
+from typing import Type
+from typing import TYPE_CHECKING
+from typing import TypeVar
 
 import polars as pl
 
 import dataframe_api_compat.polars_standard
 
 _ARRAY_API_DTYPES = frozenset(
     (
@@ -49,15 +48,15 @@
         ...
 
     class GroupBy:
         ...
 
 
 null = None
-NullType = type[None]
+NullType = Type[None]
 
 
 def _is_integer_dtype(dtype: Any) -> bool:
     return any(
         dtype is _dtype
         for _dtype in (
             pl.Int64,
@@ -71,15 +70,15 @@
         )
     )
 
 
 class PolarsColumn(Column[DType]):
     def __init__(self, column: pl.Series, *, name: str | None = None) -> None:
         self._series = column
-        self._name = name
+        self._name = name  # or column.name
 
     # In the standard
     def __column_namespace__(self, *, api_version: str | None = None) -> Any:
         return dataframe_api_compat.polars_standard
 
     @property
     def name(self) -> str | None:
```

### Comparing `dataframe_api_compat-0.1.1/dataframe_api_compat.egg-info/PKG-INFO` & `dataframe_api_compat-0.1.2/dataframe_api_compat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataframe-api-compat
-Version: 0.1.1
+Version: 0.1.2
 Summary: Implementation of the DataFrame Standard for pandas and polars
 Home-page: https://github.com/data-apis/dataframe-api-compat
 Author: Marco Gorelli
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 
 # DataFrame API Compat
 
 <h1 align="center">
 	<img
 		width="400"
 		alt="standard-compliant DataFrame"
-		src="https://github.com/data-apis/dataframe-api-compat/assets/33491632/fb4bc907-2b85-4ad7-8d13-c2b9912b97f5">
+		src="https://github.com/data-apis/dataframe-api-compat/assets/33491632/2997cb92-fd10-4426-bd41-8dfd1e466ee2">
 </h1>
 
 Implementation of the [DataFrame Standard](https://data-apis.org/dataframe-api/draft/index.html)
 for pandas and polars.
 
 What's this?
 ------------
```

### Comparing `dataframe_api_compat-0.1.1/setup.cfg` & `dataframe_api_compat-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dataframe_api_compat
-version = 0.1.1
+version = 0.1.2
 description = Implementation of the DataFrame Standard for pandas and polars
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/data-apis/dataframe-api-compat
 author = Marco Gorelli
 license = MIT
 license_files = LICENSE
```

