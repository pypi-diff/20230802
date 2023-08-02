# Comparing `tmp/dataframe_api_compat-0.1.2.tar.gz` & `tmp/dataframe_api_compat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataframe_api_compat-0.1.2.tar", last modified: Wed Aug  2 13:19:47 2023, max compression
+gzip compressed data, was "dataframe_api_compat-0.1.3.tar", last modified: Wed Aug  2 18:57:31 2023, max compression
```

## Comparing `dataframe_api_compat-0.1.2.tar` & `dataframe_api_compat-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2023-05-05 10:36:05.000000 dataframe_api_compat-0.1.2/LICENSE
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1731 2023-08-02 10:23:41.000000 dataframe_api_compat-0.1.2/README.md
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/dataframe_api_compat/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-06-28 15:01:51.000000 dataframe_api_compat-0.1.2/dataframe_api_compat/__init__.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/dataframe_api_compat/pandas_standard/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     4374 2023-08-02 13:19:17.000000 dataframe_api_compat-0.1.2/dataframe_api_compat/pandas_standard/__init__.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    28820 2023-08-02 13:19:17.000000 dataframe_api_compat-0.1.2/dataframe_api_compat/pandas_standard/pandas_standard.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/dataframe_api_compat/polars_standard/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3287 2023-08-02 10:20:54.000000 dataframe_api_compat-0.1.2/dataframe_api_compat/polars_standard/__init__.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    25207 2023-08-02 13:19:17.000000 dataframe_api_compat-0.1.2/dataframe_api_compat/polars_standard/polars_standard.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/dataframe_api_compat.egg-info/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 13:19:47.000000 dataframe_api_compat-0.1.2/dataframe_api_compat.egg-info/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      470 2023-08-02 13:19:47.000000 dataframe_api_compat-0.1.2/dataframe_api_compat.egg-info/SOURCES.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2023-08-02 13:19:47.000000 dataframe_api_compat-0.1.2/dataframe_api_compat.egg-info/dependency_links.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       21 2023-08-02 13:19:47.000000 dataframe_api_compat-0.1.2/dataframe_api_compat.egg-info/top_level.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      449 2023-08-02 10:29:22.000000 dataframe_api_compat-0.1.2/pyproject.toml
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      835 2023-08-02 13:19:47.707683 dataframe_api_compat-0.1.2/setup.cfg
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       74 2023-08-02 10:13:15.000000 dataframe_api_compat-0.1.2/setup.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 18:57:31.168066 dataframe_api_compat-0.1.3/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2023-05-05 10:36:05.000000 dataframe_api_compat-0.1.3/LICENSE
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 18:57:31.168066 dataframe_api_compat-0.1.3/PKG-INFO
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1731 2023-08-02 10:23:41.000000 dataframe_api_compat-0.1.3/README.md
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 18:57:31.168066 dataframe_api_compat-0.1.3/dataframe_api_compat/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      184 2023-08-02 18:57:06.000000 dataframe_api_compat-0.1.3/dataframe_api_compat/__init__.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 18:57:31.168066 dataframe_api_compat-0.1.3/dataframe_api_compat/pandas_standard/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     4298 2023-08-02 15:50:33.000000 dataframe_api_compat-0.1.3/dataframe_api_compat/pandas_standard/__init__.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    28860 2023-08-02 15:50:34.000000 dataframe_api_compat-0.1.3/dataframe_api_compat/pandas_standard/pandas_standard.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 18:57:31.168066 dataframe_api_compat-0.1.3/dataframe_api_compat/polars_standard/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3740 2023-08-02 15:47:51.000000 dataframe_api_compat-0.1.3/dataframe_api_compat/polars_standard/__init__.py
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    25380 2023-08-02 16:45:27.000000 dataframe_api_compat-0.1.3/dataframe_api_compat/polars_standard/polars_standard.py
+drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 18:57:31.168066 dataframe_api_compat-0.1.3/dataframe_api_compat.egg-info/
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2365 2023-08-02 18:57:31.000000 dataframe_api_compat-0.1.3/dataframe_api_compat.egg-info/PKG-INFO
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      470 2023-08-02 18:57:31.000000 dataframe_api_compat-0.1.3/dataframe_api_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2023-08-02 18:57:31.000000 dataframe_api_compat-0.1.3/dataframe_api_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       21 2023-08-02 18:57:31.000000 dataframe_api_compat-0.1.3/dataframe_api_compat.egg-info/top_level.txt
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      449 2023-08-02 10:29:22.000000 dataframe_api_compat-0.1.3/pyproject.toml
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      835 2023-08-02 18:57:31.168066 dataframe_api_compat-0.1.3/setup.cfg
+-rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       74 2023-08-02 10:13:15.000000 dataframe_api_compat-0.1.3/setup.py
```

### Comparing `dataframe_api_compat-0.1.2/LICENSE` & `dataframe_api_compat-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.2/PKG-INFO` & `dataframe_api_compat-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataframe_api_compat
-Version: 0.1.2
+Version: 0.1.3
 Summary: Implementation of the DataFrame Standard for pandas and polars
 Home-page: https://github.com/data-apis/dataframe-api-compat
 Author: Marco Gorelli
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dataframe_api_compat-0.1.2/README.md` & `dataframe_api_compat-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.2/dataframe_api_compat/pandas_standard/__init__.py` & `dataframe_api_compat-0.1.3/dataframe_api_compat/pandas_standard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,42 +143,45 @@
             axis=0,
             ignore_index=True,
         )
     )
 
 
 def column_from_sequence(
-    sequence: Sequence[Any], *, dtype: Any, name: str | None = None
+    sequence: Sequence[Any],
+    *,
+    dtype: Any,
+    name: str,
 ) -> PandasColumn[Any]:
-    ser = pd.Series(sequence, dtype=map_standard_dtype_to_pandas_dtype(dtype))
-    return PandasColumn(ser, name=name)
+    ser = pd.Series(sequence, dtype=map_standard_dtype_to_pandas_dtype(dtype), name=name)
+    return PandasColumn(ser)
 
 
 def column_from_1d_array(
-    array, *, dtype: Any, name: str | None = None
+    data: Any, *, dtype: Any, name: str | None = None
 ) -> PandasColumn[Any]:  # pragma: no cover
-    ser = pd.Series(array, dtype=map_standard_dtype_to_pandas_dtype(dtype), name=name)
+    ser = pd.Series(data, dtype=map_standard_dtype_to_pandas_dtype(dtype), name=name)
     return PandasColumn(ser)
 
 
 def dataframe_from_2d_array(
-    array, *, names: Sequence[str], dtypes: dict[str, Any]
-) -> PandasColumn[Any]:  # pragma: no cover
-    df = pd.DataFrame(array, columns=names).astype(
+    data: Any, *, names: Sequence[str], dtypes: dict[str, Any]
+) -> PandasDataFrame:  # pragma: no cover
+    df = pd.DataFrame(data, columns=names).astype(  # type: ignore[call-overload]
         {key: map_standard_dtype_to_pandas_dtype(value) for key, value in dtypes.items()}
     )
     return PandasDataFrame(df)
 
 
 def dataframe_from_dict(data: dict[str, PandasColumn[Any]]) -> PandasDataFrame:
-    for col_name, col in data.items():
+    for _, col in data.items():
         if not isinstance(col, PandasColumn):  # pragma: no cover
             raise TypeError(f"Expected PandasColumn, got {type(col)}")
-        if col.name is not None and col_name != col.name:
-            raise ValueError(f"Expected column name {col_name}, got {col.name}")
     return PandasDataFrame(
-        pd.DataFrame({label: column.column for label, column in data.items()})
+        pd.DataFrame(
+            {label: column.column.rename(label) for label, column in data.items()}
+        )
     )
 
 
 def is_null(value: Any) -> bool:
     return value is pd.NA
```

### Comparing `dataframe_api_compat-0.1.2/dataframe_api_compat/pandas_standard/pandas_standard.py` & `dataframe_api_compat-0.1.3/dataframe_api_compat/pandas_standard/pandas_standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,38 +52,35 @@
 
     class GroupBy:
         ...
 
 
 class PandasColumn(Column[DType]):
     # private, not technically part of the standard
-    def __init__(
-        self, column: pd.Series, *, name: str | None = None  # type: ignore[type-arg]
-    ) -> None:
+    def __init__(self, column: pd.Series[Any]) -> None:
         if (
             isinstance(column.index, pd.RangeIndex)
             and column.index.start == 0  # type: ignore[comparison-overlap]
             and column.index.step == 1  # type: ignore[comparison-overlap]
             and (column.index.stop == len(column))  # type: ignore[comparison-overlap]
         ):
             self._series = column
         else:
             self._series = column.reset_index(drop=True)
-        self._name = name  # or column.name
 
     def _validate_index(self, index: pd.Index) -> None:
         pd.testing.assert_index_equal(self.column.index, index)
 
     # In the standard
     def __column_namespace__(self, *, api_version: str | None = None) -> Any:
         return dataframe_api_compat.pandas_standard
 
     @property
-    def name(self) -> str | None:
-        return self._name
+    def name(self) -> str:
+        return self.column.name  # type: ignore[return-value]
 
     @property
     def column(self) -> pd.Series[Any]:
         return self._series
 
     def __len__(self) -> int:
         return len(self.column)
@@ -297,14 +294,17 @@
     def to_array_object(self, dtype: str) -> Any:
         if dtype not in _ARRAY_API_DTYPES:
             raise ValueError(
                 f"Invalid dtype {dtype}. Expected one of {_ARRAY_API_DTYPES}"
             )
         return self.column.to_numpy(dtype=dtype)
 
+    def rename(self, name: str | None) -> PandasColumn[DType]:
+        return PandasColumn(self.column.rename(name))
+
 
 class PandasGroupBy(GroupBy):
     def __init__(self, df: pd.DataFrame, keys: Sequence[str]) -> None:
         self.df = df
         self.grouped = df.groupby(list(keys), sort=False, as_index=False)
         self.keys = list(keys)
```

### Comparing `dataframe_api_compat-0.1.2/dataframe_api_compat/polars_standard/__init__.py` & `dataframe_api_compat-0.1.3/dataframe_api_compat/polars_standard/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -99,29 +99,48 @@
     dfs = []
     for _df in dataframes:
         dfs.append(_df.dataframe)
     return PolarsDataFrame(pl.concat(dfs))
 
 
 def dataframe_from_dict(data: dict[str, PolarsColumn[Any]]) -> PolarsDataFrame:
-    for col_name, col in data.items():
+    for _, col in data.items():
         if not isinstance(col, PolarsColumn):  # pragma: no cover
             raise TypeError(f"Expected PolarsColumn, got {type(col)}")
-        if col.name is not None and col_name != col.name:
-            raise ValueError(f"Expected column name {col_name}, got {col.name}")
     return PolarsDataFrame(
-        pl.DataFrame({label: column.column for label, column in data.items()})
+        pl.DataFrame(
+            {label: column.column.rename(label) for label, column in data.items()}
+        )
     )
 
 
+def column_from_1d_array(
+    data: Any, *, dtype: Any, name: str
+) -> PolarsColumn[Any]:  # pragma: no cover
+    ser = pl.Series(values=data, dtype=_map_standard_to_polars_dtypes(dtype), name=name)
+    return PolarsColumn(ser)
+
+
+def dataframe_from_2d_array(
+    data: Any, *, names: Sequence[str], dtypes: dict[str, Any]
+) -> PolarsDataFrame:  # pragma: no cover
+    df = pl.DataFrame(
+        data,
+        schema={
+            key: _map_standard_to_polars_dtypes(value) for key, value in dtypes.items()
+        },
+    )
+    return PolarsDataFrame(df)
+
+
 def column_from_sequence(
     sequence: Sequence[Any], *, dtype: Any, name: str | None = None
 ) -> PolarsColumn[Any]:
     return PolarsColumn(
-        pl.Series(sequence, dtype=_map_standard_to_polars_dtypes(dtype)), name=name
+        pl.Series(values=sequence, dtype=_map_standard_to_polars_dtypes(dtype), name=name)
     )
 
 
 def convert_to_standard_compliant_dataframe(
     df: pl.DataFrame, api_version: str | None = None
 ) -> PolarsDataFrame:
     if api_version is None:
```

### Comparing `dataframe_api_compat-0.1.2/dataframe_api_compat/polars_standard/polars_standard.py` & `dataframe_api_compat-0.1.3/dataframe_api_compat/polars_standard/polars_standard.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,25 +68,24 @@
             pl.UInt16,
             pl.UInt8,
         )
     )
 
 
 class PolarsColumn(Column[DType]):
-    def __init__(self, column: pl.Series, *, name: str | None = None) -> None:
+    def __init__(self, column: pl.Series) -> None:
         self._series = column
-        self._name = name  # or column.name
 
     # In the standard
     def __column_namespace__(self, *, api_version: str | None = None) -> Any:
         return dataframe_api_compat.polars_standard
 
     @property
-    def name(self) -> str | None:
-        return self._name
+    def name(self) -> str:
+        return self.column.name
 
     @property
     def column(self) -> pl.Series:
         return self._series
 
     def __len__(self) -> int:
         return len(self.column)
@@ -303,14 +302,17 @@
     def to_array_object(self, dtype: str) -> Any:
         if dtype not in _ARRAY_API_DTYPES:
             raise ValueError(
                 f"Invalid dtype {dtype}. Expected one of {_ARRAY_API_DTYPES}"
             )
         return self.column.to_numpy().astype(dtype)
 
+    def rename(self, name: str | None) -> PolarsColumn[DType]:
+        return PolarsColumn(self.column.rename(name or ""))
+
 
 class PolarsGroupBy(GroupBy):
     def __init__(self, df: pl.DataFrame, keys: Sequence[str]) -> None:
         for key in keys:
             if key not in df.columns:
                 raise KeyError(f"key {key} not present in DataFrame's columns")
         self.df = df
@@ -666,8 +668,10 @@
         return PolarsDataFrame(df)
 
     def to_array_object(self, dtype: str) -> Any:
         if dtype not in _ARRAY_API_DTYPES:
             raise ValueError(
                 f"Invalid dtype {dtype}. Expected one of {_ARRAY_API_DTYPES}"
             )
+        if isinstance(self.dataframe, pl.LazyFrame):
+            return self.dataframe.collect().to_numpy().astype(dtype)
         return self.dataframe.to_numpy().astype(dtype)
```

### Comparing `dataframe_api_compat-0.1.2/dataframe_api_compat.egg-info/PKG-INFO` & `dataframe_api_compat-0.1.3/dataframe_api_compat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataframe-api-compat
-Version: 0.1.2
+Version: 0.1.3
 Summary: Implementation of the DataFrame Standard for pandas and polars
 Home-page: https://github.com/data-apis/dataframe-api-compat
 Author: Marco Gorelli
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dataframe_api_compat-0.1.2/setup.cfg` & `dataframe_api_compat-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dataframe_api_compat
-version = 0.1.2
+version = 0.1.3
 description = Implementation of the DataFrame Standard for pandas and polars
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/data-apis/dataframe-api-compat
 author = Marco Gorelli
 license = MIT
 license_files = LICENSE
```

