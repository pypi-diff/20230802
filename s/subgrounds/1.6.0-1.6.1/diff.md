# Comparing `tmp/subgrounds-1.6.0.tar.gz` & `tmp/subgrounds-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subgrounds-1.6.0.tar", max compression
+gzip compressed data, was "subgrounds-1.6.1.tar", max compression
```

## Comparing `subgrounds-1.6.0.tar` & `subgrounds-1.6.1.tar`

### file list

```diff
@@ -1,34 +1,39 @@
--rw-r--r--   0        0        0    11357 2023-05-25 20:34:48.645267 subgrounds-1.6.0/LICENSE
--rw-r--r--   0        0        0     4035 2023-05-25 20:34:48.645267 subgrounds-1.6.0/README.md
--rw-r--r--   0        0        0     1929 2023-05-25 20:35:16.361624 subgrounds-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      317 2023-05-25 20:35:16.337624 subgrounds-1.6.0/subgrounds/__init__.py
--rw-r--r--   0        0        0     4527 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/client.py
--rw-r--r--   0        0        0     1895 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/contrib/README.md
--rw-r--r--   0        0        0      349 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/contrib/dash/__init__.py
--rw-r--r--   0        0        0      399 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/contrib/dash/abcs.py
--rw-r--r--   0        0        0     3893 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/contrib/dash/components.py
--rw-r--r--   0        0        0     1285 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/contrib/plotly/__init__.py
--rw-r--r--   0        0        0     1316 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/contrib/plotly/figure.py
--rw-r--r--   0        0        0     5866 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/contrib/plotly/traces.py
--rw-r--r--   0        0        0      873 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/contrib/pyodide.py
--rw-r--r--   0        0        0      438 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/dash_wrappers.py
--rw-r--r--   0        0        0    10062 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/dataframe_utils.py
--rw-r--r--   0        0        0      395 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/errors.py
--rw-r--r--   0        0        0     1027 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/pagination/__init__.py
--rw-r--r--   0        0        0     4761 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/pagination/pagination.py
--rw-r--r--   0        0        0    12577 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/pagination/preprocess.py
--rw-r--r--   0        0        0    17155 2023-05-25 20:34:48.645267 subgrounds-1.6.0/subgrounds/pagination/strategies.py
--rw-r--r--   0        0        0     2901 2023-05-25 20:34:48.649267 subgrounds-1.6.0/subgrounds/pagination/utils.py
--rw-r--r--   0        0        0     1460 2023-05-25 20:34:48.649267 subgrounds-1.6.0/subgrounds/plotly_wrappers.py
--rw-r--r--   0        0        0    62357 2023-05-25 20:34:48.649267 subgrounds-1.6.0/subgrounds/query.py
--rw-r--r--   0        0        0    13291 2023-05-25 20:34:48.649267 subgrounds-1.6.0/subgrounds/schema.py
--rw-r--r--   0        0        0      308 2023-05-25 20:34:48.649267 subgrounds-1.6.0/subgrounds/subgraph/__init__.py
--rw-r--r--   0        0        0    38793 2023-05-25 20:34:48.649267 subgrounds-1.6.0/subgrounds/subgraph/fieldpath.py
--rw-r--r--   0        0        0     1669 2023-05-25 20:34:48.649267 subgrounds-1.6.0/subgrounds/subgraph/filter.py
--rw-r--r--   0        0        0     4754 2023-05-25 20:34:48.649267 subgrounds-1.6.0/subgrounds/subgraph/object.py
--rw-r--r--   0        0        0     2550 2023-05-25 20:34:48.649267 subgrounds-1.6.0/subgrounds/subgraph/subgraph.py
--rw-r--r--   0        0        0    22021 2023-05-25 20:34:48.649267 subgrounds-1.6.0/subgrounds/subgrounds.py
--rw-r--r--   0        0        0    20072 2023-05-25 20:34:48.649267 subgrounds-1.6.0/subgrounds/transform.py
--rw-r--r--   0        0        0     7865 2023-05-25 20:34:48.649267 subgrounds-1.6.0/subgrounds/utils.py
--rw-r--r--   0        0        0     5318 1970-01-01 00:00:00.000000 subgrounds-1.6.0/setup.py
--rw-r--r--   0        0        0     5112 1970-01-01 00:00:00.000000 subgrounds-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 23:09:23.329542 subgrounds-1.6.1/LICENSE
+-rw-r--r--   0        0        0     3971 2023-08-01 23:09:23.329542 subgrounds-1.6.1/README.md
+-rw-r--r--   0        0        0     1932 2023-08-01 23:11:38.426428 subgrounds-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      317 2023-08-01 23:11:38.390427 subgrounds-1.6.1/subgrounds/__init__.py
+-rw-r--r--   0        0        0     4490 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/client.py
+-rw-r--r--   0        0        0     1895 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/contrib/README.md
+-rw-r--r--   0        0        0      349 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/contrib/dash/__init__.py
+-rw-r--r--   0        0        0      399 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/contrib/dash/abcs.py
+-rw-r--r--   0        0        0     3893 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/contrib/dash/components.py
+-rw-r--r--   0        0        0     1285 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/contrib/plotly/__init__.py
+-rw-r--r--   0        0        0     1316 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/contrib/plotly/figure.py
+-rw-r--r--   0        0        0     5866 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/contrib/plotly/traces.py
+-rw-r--r--   0        0        0      873 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/contrib/pyodide.py
+-rw-r--r--   0        0        0      438 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/dash_wrappers.py
+-rw-r--r--   0        0        0     7169 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/dataframe_utils.py
+-rw-r--r--   0        0        0      395 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/errors.py
+-rw-r--r--   0        0        0     1061 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/pagination/__init__.py
+-rw-r--r--   0        0        0     1626 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/pagination/pagination.py
+-rw-r--r--   0        0        0    12382 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/pagination/preprocess.py
+-rw-r--r--   0        0        0    19592 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/pagination/strategies.py
+-rw-r--r--   0        0        0     1426 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/pagination/utils.py
+-rw-r--r--   0        0        0     1460 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/plotly_wrappers.py
+-rw-r--r--   0        0        0    63130 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/query.py
+-rw-r--r--   0        0        0    12792 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/schema.py
+-rw-r--r--   0        0        0      308 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/subgraph/__init__.py
+-rw-r--r--   0        0        0    36800 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/subgraph/fieldpath.py
+-rw-r--r--   0        0        0     1669 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/subgraph/filter.py
+-rw-r--r--   0        0        0     4845 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/subgraph/object.py
+-rw-r--r--   0        0        0     2550 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/subgraph/subgraph.py
+-rw-r--r--   0        0        0    19443 2023-08-01 23:09:23.333542 subgrounds-1.6.1/subgrounds/subgrounds.py
+-rw-r--r--   0        0        0      430 2023-08-01 23:09:23.337542 subgrounds-1.6.1/subgrounds/transform/__init__.py
+-rw-r--r--   0        0        0     2171 2023-08-01 23:09:23.337542 subgrounds-1.6.1/subgrounds/transform/abcs.py
+-rw-r--r--   0        0        0     3683 2023-08-01 23:09:23.337542 subgrounds-1.6.1/subgrounds/transform/apply.py
+-rw-r--r--   0        0        0      491 2023-08-01 23:09:23.337542 subgrounds-1.6.1/subgrounds/transform/defaults.py
+-rw-r--r--   0        0        0    14148 2023-08-01 23:09:23.337542 subgrounds-1.6.1/subgrounds/transform/transforms.py
+-rw-r--r--   0        0        0     2095 2023-08-01 23:09:23.337542 subgrounds-1.6.1/subgrounds/transform/utils.py
+-rw-r--r--   0        0        0     9631 2023-08-01 23:09:23.337542 subgrounds-1.6.1/subgrounds/utils.py
+-rw-r--r--   0        0        0     5327 1970-01-01 00:00:00.000000 subgrounds-1.6.1/setup.py
+-rw-r--r--   0        0        0     5124 1970-01-01 00:00:00.000000 subgrounds-1.6.1/PKG-INFO
```

### Comparing `subgrounds-1.6.0/LICENSE` & `subgrounds-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `subgrounds-1.6.0/README.md` & `subgrounds-1.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 - **Automated**: Automatically handle pagination and schema introspection for effortless data retrieval.
 - **Powerful**: Create sophisticated queries using the `SyntheticFields` transformation system.
 <!-- end elevator-pitch -->
 
 ## Resources
 - [**Subgrounds Docs**](http://docs.playgrounds.network/): User guide and API documentation
 - [**Examples**](https://github.com/0xPlaygrounds/subgrounds/tree/main/examples): A list of examples showcasing Subgrounds integration with Dash and Plotly
-- [**Community projects**](http://docs.playgrounds.network/subgrounds/examples/): An ever growing list of projects created by our community members
-- [**MetricsDAO Subgrounds Workshop**](https://docs.metricsdao.xyz/get-involved/workshops/2022-03-30+-subgrounds-workshop-series): Subgrounds workshop series hosted by MetricsDAO 
+- [**Tutorials**](https://docs.playgrounds.network/subgrounds/tutorials/): Subgrounds video workshops and tutorials
+- [**Community Projects**](http://docs.playgrounds.network/subgrounds/examples/): An ever growing list of projects created by our community members
 
 ## Installation
 > Subgrounds **requires** atleast Python 3.10+
 
 Subgrounds is available on PyPi. To install it, run the following:<br>
 `pip install subgrounds`.
```

### Comparing `subgrounds-1.6.0/pyproject.toml` & `subgrounds-1.6.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "subgrounds"
-version = "1.6.0"
+version = "1.6.1"
 description = "A Pythonic data access layer for applications querying data from The Graph Network."
 authors = [
     "cvauclair <cvauclair@playgrounds.network>",
     "0xMochan <mochan@playgrounds.network>",
 ]
 repository = "https://github.com/0xPlaygrounds/subgrounds"
 
@@ -16,14 +16,16 @@
 requests = "^2.27.1"
 pandas = "^1.4.2"
 pipe = "^2.0"
 pydantic = "^1.10.2"
 dash = { version = "^2.3.1", optional = true }
 plotly = { version = "^5.14.1", optional = true }
 pyodide-http = { version = "^0.2.1", optional = true }
+gql = "^3.4.0"
+aiohttp = "^3.8.4"
 
 [tool.poetry.extras]
 dash = ["dash"]
 plotly = ["plotly"]
 pyodide = ["pyodide-http"]
 all = ["dash", "plotly", "pyodide-http"]
 
@@ -34,32 +36,37 @@
 ipykernel = "^6.13.0"
 mypy = "^0.950"
 nose2 = "^0.11.0"
 pytest = "^7.1.2"
 pytest-mock = "^3.8.2"
 python-semantic-release = "^7.33.1"
 ruff = "^0.0.253"
+pytest-insta = "^0.2.0"
 
 [tool.poe.tasks]
-format = { shell = "black subgrounds examples tests" }
-check = { shell = "black subgrounds examples tests --check; ruff check subgrounds examples tests" }
-develop = { shell = "mudkip develop" }
+format = "black subgrounds examples tests"
+
+_black = "black subgrounds examples tests --check"
+_ruff = "ruff check subgrounds examples tests"
+check.sequence = ["_black", "_ruff"]
+check.ignore_fail = "return_zero"
+
 test = "pytest"
-generate-api-docs = { shell = "sphinx-apidoc --output docs/api subgrounds --separate --force" }
 
 [tool.semantic_release]
 branch = "main"
 upload_to_pypi = true
 version_variable = ["subgrounds/__init__.py:__version__"]
 version_toml = "pyproject.toml:tool.poetry.version"
 major_on_zero = false
 build_command = "poetry build"
 
 [tool.ruff]
 
 [tool.ruff.per-file-ignores]
+"tests/*" = ["E501"]
 "subgrounds/plotly_wrappers" = ["F405", "F403"]
 "subgrounds/dash_wrappers" = ["F405", "F403"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `subgrounds-1.6.0/subgrounds/client.py` & `subgrounds-1.6.1/subgrounds/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """
 
 import logging
 from typing import Any
 
 import requests
 
+from subgrounds.query import Document, DocumentResponse
+
 from .errors import GraphQLError, ServerError
 from .utils import default_header
 
 logger = logging.getLogger("subgrounds")
 
 
 INTROSPECTION_QUERY: str = """
@@ -106,23 +108,23 @@
 
 def get_schema(url: str, headers: dict[str, Any]) -> dict[str, Any]:
     """Runs the introspection query on the GraphQL API served localed at
     :attr:`url` and returns the result. In case of errors, an exception containing
     the error message is thrown.
 
     Args:
-      url (str): The url of the GraphQL API
+      url: The url of the GraphQL API
 
     Raises:
       HttpError: If the request response resulted in an error
       ServerError: If server responds back non-json content
       GraphQLError: If the GraphQL query failed or other grapql server errors
 
     Returns:
-      dict[str, Any]: The GraphQL API's schema in JSON
+      The GraphQL API's schema in JSON
     """
 
     resp = requests.post(
         url,
         json={"query": INTROSPECTION_QUERY},
         headers=default_header(url) | headers,
     )
@@ -141,60 +143,55 @@
 
     if (data := raw_data.get("data")) is None:
         raise GraphQLError(raw_data.get("errors", "Unknown Error(s) Found"))
 
     return data
 
 
-def query(
-    url: str,
-    query_str: str,
-    variables: dict[str, Any] = {},
-    headers: dict[str, Any] = {},
-) -> dict[str, Any]:
+def query(doc: Document, headers: dict[str, Any] = {}) -> DocumentResponse:
     """Executes the GraphQL query :attr:`query_str` with variables
     :attr:`variables` against the API served at :attr:`url` and returns the
     response data. In case of errors, an exception containing the error message is
     thrown.
 
     Args:
-      url (str): The URL of the GraphQL API
-      query_str (str): The GraphQL query string
-      variables (dict[str, Any], optional): Variables for the GraphQL query.
-        Defaults to {}.
+      url: The URL of the GraphQL API
+      query_str: The GraphQL query string
+      variables: Variables for the GraphQL query. Defaults to {}.
 
     Raises:
       HttpError: If the request response resulted in an error
       ServerError: If server responds back non-json content
       GraphQLError: If the GraphQL query failed or other grapql server errors
 
     Returns:
-      dict[str, Any]: Response data
+      Response data
     """
 
-    logger.info(f"client.query: url = {url}, variables = {variables}\n{query_str}")
+    logger.info(
+        f"client.query: url = {doc.url}, variables = {doc.variables}\n{doc.graphql}"
+    )
     resp = requests.post(
-        url,
+        doc.url,
         json=(
-            {"query": query_str}
-            if variables == {}
-            else {"query": query_str, "variables": variables}
+            {"query": doc.graphql}
+            | ({"variables": doc.variables} if doc.variables else {})
         ),
-        headers=default_header(url) | headers,
+        headers=default_header(doc.url) | headers,
     )
 
     resp.raise_for_status()
 
     try:
         raw_data = resp.json()
 
     except requests.JSONDecodeError:
         raise ServerError(
-            f"Server ({url}) did not respond with proper JSON"
+            f"Server ({doc.url}) did not respond with proper JSON"
             f"\nDid you query a proper GraphQL endpoint?"
             f"\n\n{resp.content}"
         )
 
     if (data := raw_data.get("data")) is None:
         raise GraphQLError(raw_data.get("errors", "Unknown Error(s) Found"))
 
-    return data
+    return DocumentResponse(data=data, url=doc.url)
```

### Comparing `subgrounds-1.6.0/subgrounds/contrib/README.md` & `subgrounds-1.6.1/subgrounds/contrib/README.md`

 * *Files identical despite different names*

### Comparing `subgrounds-1.6.0/subgrounds/contrib/dash/components.py` & `subgrounds-1.6.1/subgrounds/contrib/dash/components.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.6.0/subgrounds/contrib/plotly/__init__.py` & `subgrounds-1.6.1/subgrounds/contrib/plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.6.0/subgrounds/contrib/plotly/figure.py` & `subgrounds-1.6.1/subgrounds/contrib/plotly/figure.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.6.0/subgrounds/contrib/plotly/traces.py` & `subgrounds-1.6.1/subgrounds/contrib/plotly/traces.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.6.0/subgrounds/contrib/pyodide.py` & `subgrounds-1.6.1/subgrounds/contrib/pyodide.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.6.0/subgrounds/dataframe_utils.py` & `subgrounds-1.6.1/subgrounds/dataframe_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 formatting of GraphQL JSON data into DataFrames.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from functools import partial
-from typing import Any, Optional
+from itertools import cycle
+from typing import Any
 
 import pandas as pd
 from pipe import dedup, groupby, map, traverse, where
+from typing_extensions import Self
 
 from subgrounds.query import Selection
 from subgrounds.subgraph import FieldPath
-from subgrounds.utils import loop_generator, union
+from subgrounds.utils import union
 
 
 def gen_columns(data: list | dict, prefix: str = "") -> list[str]:
     match data:
         case dict():
             return list(
                 list(data.keys())
@@ -43,39 +45,38 @@
 @dataclass
 class DataFrameColumns:
     """Helper class that holds data related to the shape of a DataFrame"""
 
     key: str
     fpaths: list[str]
 
-    def combine(self, other: DataFrameColumns) -> DataFrameColumns:
+    def combine(self, other: Self) -> Self:
         """Returns new DataFrameColumns containing the union of :attr:`self` and
         :attr:`other`'s columns
 
         Args:
-          other (DataFrameColumns): Columns to be combined to :attr:`self`
+          other: Columns to be combined to :attr:`self`
 
         Returns:
-          DataFrameColumns: New :class:`DataFrameColumns` containing the union of
-            :attr:`self` and :attr:`other`
+          New :class:`Self` containing the union of :attr:`self` and :attr:`other`
         """
         return DataFrameColumns(self.key, union(self.fpaths, other.fpaths))
 
     def mk_df(
         self, data: list[dict[str, Any]], path_map: dict[str, FieldPath]
     ) -> pd.DataFrame:
         """Formats the JSON data :attr:`data` into a DataFrame containing the columns
         defined in :attr:`self`.
 
         Args:
-          data (list[dict[str, Any]]): The JSON data to be formatted into a dataframe
-          path_map (dict[str, FieldPath]): A dictionary of :attr:`(key-FieldPath)` pairs
+          data: The JSON data to be formatted into a dataframe
+          path_map: A dictionary of :attr:`(key-FieldPath)` pairs
 
         Returns:
-          pd.DataFrame: The JSON data formatted into a DataFrame
+          The JSON data formatted into a DataFrame
         """
         cols_data = {
             col: path_map[col]._extract_data(data)
             for col in self.fpaths
             if col in path_map
         }
 
@@ -98,80 +99,23 @@
                         row=row | non_list_items,
                     )
 
         mk_rows(cols_data, row={})
         return pd.DataFrame(data=rows_data)
 
 
-# def columns_of_json(data: dict) -> list[str]:
-#   # Helper function to combine result of list items columns
-#   def merge(
-#     cols1: DataFrameColumns | list[DataFrameColumns],
-#     cols2: DataFrameColumns | list[DataFrameColumns]
-#   ) -> DataFrameColumns | list[DataFrameColumns]:
-#     # print(f'merge: cols1 = {cols1}, cols2 = {cols2}')
-#     match cols1, cols2:
-#       case list(), list():
-#         return list(zip(cols1, cols2) | map(lambda cols: merge(cols[0], cols[1])))
-#       case DataFrameColumns(), DataFrameColumns():
-#         return DataFrameColumns.combine(cols1, cols2)
-
-#   def columns_of_json(data: dict, keys: list[str] = [], fpaths: list[str] = []):
-#     # Subset of the `data` dictionary containing only key-value pairs whose value
-#     # if not a list, nor contains a nested list
-#     values_dict = flatten_dict({key: value for key, value in data.items() if not contains_list(value)})
-
-#     # List names identifiyng the values in `values_dict`
-#     values_fpaths = ['_'.join([*keys, key]) for key in values_dict]
-
-#     # Subset of the `data` dictionary containing only key-value pairs whose value
-#     # either is a list, or contains a nested list
-#     list_dict = {key: value for key, value in data.items() if contains_list(value) and value != []}
-
-#     if list_dict == {}:
-#       return [DataFrameColumns('_'.join(keys), values_fpaths + fpaths)]
-#     else:
-#       dfs: list[DataFrameColumns] = []
-#       for key, value in data.items():
-#         match value:
-#           case dict():
-#             dfs.append(columns_of_json(value, [*keys, key], fpaths + values_fpaths))
-#           case list() if len(value) == 0:
-#             continue
-#           case list() if len(value) == 1:
-#             dfs.append(columns_of_json(value[0], [*keys, key], fpaths + values_fpaths))
-#           case list():
-#             inner = list(
-#               value
-#               | map(partial(columns_of_json, keys=[*keys, key], fpaths=fpaths + values_fpaths))
-#               | map(lambda l: list(l | traverse) if type(l) == list else l)
-#             )
-#             dfs.append(reduce(
-#               merge,
-#               list(
-#                 value
-#                 | map(partial(columns_of_json, keys=[*keys, key], fpaths=fpaths + values_fpaths))
-#                 | map(lambda l: list(l | traverse) if type(l) == list else l)
-#               )
-#             ))
-
-#     return dfs
-
-#   return list(columns_of_json(data) | traverse)
-
-
 def columns_of_selections(selections: list[Selection]) -> list[DataFrameColumns]:
     """Generates a list of DataFrame columns specifications based on a list of
     :class:`Selection` trees.
 
     Args:
-      selections (list[Selection]): The selection trees
+      selections: The selection trees
 
     Returns:
-      list[DataFrameColumns]: The list of DataFrame columns specifications
+      The list of DataFrame columns specifications
     """
 
     def columns_of_selections(
         selections: list[Selection], keys: list[str] = [], fpaths: list[str] = []
     ) -> list[DataFrameColumns]:
         if len(selections) > 0:
             non_list_selections = [
@@ -207,15 +151,15 @@
 
     return list(columns_of_selections(selections) | traverse)
 
 
 def df_of_json(
     json_data: list[dict[str, Any]],
     fpaths: list[FieldPath],
-    columns: Optional[list[str]] = None,
+    columns: list[str] | None = None,
     concat: bool = False,
 ) -> pd.DataFrame | list[pd.DataFrame]:
     """Formats the JSON data :attr:`json_data` into Pandas DataFrames,
     flattening the data in the process.
 
     Depending on the request's fieldpaths, either one or multiple dataframes will
     be returned based on how flattenable the response data is.
@@ -229,45 +173,47 @@
 
     :attr:`concat` indicates whether or not the resulting dataframes should be
     concatenated together. The dataframes must have the same number of columns,
     as well as the same column names (which can be set using the :attr:`columns`
     argument).
 
     Args:
-      json_data (list[dict[str, Any]]): Response data
-      fpaths (list[FieldPath]): Fieldpaths that yielded the response data
-      columns (Optional[list[str]], optional): Column names. Defaults to None.
-      concat (bool, optional): Flag indicating whether or not to concatenate the
-        resulting dataframes, if there are more than one. Defaults to False.
+      json_data: Response data
+      fpaths: Fieldpaths that yielded the response data
+      columns: Column names. Defaults to None.
+      concat: Flag indicating whether or not to concatenate the resulting dataframes,
+        if there are more than one. Defaults to False.
 
     Returns:
-      pd.DataFrame | list[pd.DataFrame]: The resulting dataframe(s)
+      The resulting dataframe(s)
     """
+
     if columns is None:
         columns = list(fpaths | map(lambda fpath: fpath._name()))
 
-    col_fpaths = zip(fpaths, loop_generator(columns))
+    col_fpaths = zip(fpaths, cycle(columns))
     col_map = {fpath._name(use_aliases=True): colname for fpath, colname in col_fpaths}
 
     path_map = {fpath._name(use_aliases=True): fpath for fpath in fpaths}
 
     dfs = list(
         fpaths
         | groupby(lambda fpath: fpath._subgraph._url)
         | map(lambda group: FieldPath._merge(group[1]))
         | map(columns_of_selections)
         | traverse
         | map(partial(DataFrameColumns.mk_df, data=json_data, path_map=path_map))
     )
 
-    match (len(dfs), concat):
-        case (0, _):
-            return pd.DataFrame(columns=columns, data=[])
-        case (1, _):
-            return fmt_cols(dfs[0], col_map)
-        case (_, False):
-            return list(dfs | map(lambda df: fmt_cols(df, col_map)))
-        case (_, True):
-            dfs = list(dfs | map(lambda df: fmt_cols(df, col_map)))
-            return pd.concat(dfs, ignore_index=True)
+    if len(dfs) == 0:
+        return pd.DataFrame(columns=columns, data=[])
+
+    if len(dfs) == 1:
+        return fmt_cols(dfs[0], col_map)
+
+    if concat:
+        return pd.concat(
+            list(dfs | map(lambda df: fmt_cols(df, col_map))),
+            ignore_index=True,
+        )
 
-    assert False  # Suppress mypy missing return statement warning
+    return list(dfs | map(lambda df: fmt_cols(df, col_map)))
```

### Comparing `subgrounds-1.6.0/subgrounds/pagination/__init__.py` & `subgrounds-1.6.1/subgrounds/pagination/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-""" This module contains all code related to automatic pagination.
+"""This module contains all code related to automatic pagination.
 
-The ``pagination`` module contains the pagination algorithms (both regular and iterative)
-that make use of ``PaginationStrategies``.
+The `pagination` module contains the pagination algorithms (both regular and iterative)
+  that make use of `PaginationStrategies`.
 
-The ``preprocess`` and ``strategties`` modules implement the currently supported ``PaginationStrategies``:
-``LegacyStrategy`` and ``ShallowStrategy``.
+The `preprocess` and `strategties` modules implement the currently supported
+  `PaginationStrategies`: `LegacyStrategy` and `ShallowStrategy`.
 
-The ``utils`` module contains some generic functions that are useful in the context of pagination.
+The `utils` module contains some generic functions that are useful in the context of
+  pagination.
 """
 
 from subgrounds.pagination.pagination import (
     PaginationError,
     PaginationStrategy,
     paginate,
-    paginate_iter,
 )
 from subgrounds.pagination.preprocess import (
     PaginationNode,
     generate_pagination_nodes,
-    normalize,
     prune_doc,
 )
-from subgrounds.pagination.strategies import LegacyStrategy, ShallowStrategy
+from subgrounds.pagination.strategies import (
+    LegacyStrategy,
+    ShallowStrategy,
+    SkipStrategy,
+    normalize_strategy,
+)
 
 __all__ = [
     "generate_pagination_nodes",
     "LegacyStrategy",
-    "normalize",
-    "paginate_iter",
+    "normalize_strategy",
+    "paginate",
     "paginate",
     "PaginationError",
     "PaginationNode",
     "PaginationStrategy",
     "prune_doc",
     "ShallowStrategy",
+    "SkipStrategy",
 ]
```

### Comparing `subgrounds-1.6.0/subgrounds/pagination/preprocess.py` & `subgrounds-1.6.1/subgrounds/pagination/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,58 +16,56 @@
     InputValue,
     Selection,
     VariableDefinition,
 )
 from subgrounds.schema import SchemaMeta, TypeMeta, TypeRef
 from subgrounds.utils import accumulate
 
-from .utils import DEFAULT_NUM_ENTITIES, merge_input_value_object_metas
+from .utils import merge_input_value_object_metas
+
+DEFAULT_NUM_ENTITIES = 100
 
 
 @dataclass(frozen=True)
 class PaginationNode:
     """Class representing the pagination config for a single GraphQL list field.
 
     Attributes:
-      node_idx (int): Index of PaginationNode, used to label pagination arguments
-        for this node.
-      filter_field (str): Name of the node's filter field, e.g.: if
-        ``filter_name`` is ``timestamp_gt``, then :attr:`filter_field`
-        is ``timestamp``
-      first_value (int): Initial value of the ``first`` argument
-      skip_value (int): Initial value of the ``skip`` argument
-      filter_value (Any): Initial value of the filter argument
+      node_idx: Index of PaginationNode, used to label pagination arguments for
+        this node.
+      filter_field : Name of the node's filter field, e.g.: if ``filter_name`` is
+        ``timestamp_gt``, then :attr:`filter_field` is ``timestamp``
+      first_value: Initial value of the ``first`` argument
+      skip_value: Initial value of the ``skip`` argument
+      filter_value: Initial value of the filter argument
         (i.e.: ``where: {filter: FILTER_VALUE}``)
-      filter_value_type (TypeRef.T): Type of the filter value
-      key_path (list[str]): Location in the list field to which this pagination
-        node refers to in the initial query
-      inner (list[PaginationNode]): Nested pagination nodes (if any).
+      filter_value_type: Type of the filter value
+      key_path: Location in the list field to which this pagination node refers to in
+        the initial query
+      inner: Nested pagination nodes (if any).
     """
 
     node_idx: int
     filter_field: str
 
     first_value: int
     skip_value: int
     filter_value: Any
     filter_value_type: TypeRef.T
 
     key_path: list[str]
     inner: list[PaginationNode] = field(default_factory=list)
 
-    def get_vardefs(self: PaginationNode) -> list[VariableDefinition]:
+    def get_vardefs(self) -> list[VariableDefinition]:
         """Returns a list of variable definitions corresponding to this pagination
         node's pagination arguments as well as the variable definitions related
         to any nested pagination nodes.
 
-        Args:
-          self (PaginationNode): The current PaginationNode
-
         Returns:
-          list[VariableDefinition]: _description_
+          _description_
         """
         vardefs = [
             VariableDefinition(
                 f"first{self.node_idx}", TypeRef.Named(name="Int", kind="SCALAR")
             ),
             VariableDefinition(
                 f"skip{self.node_idx}", TypeRef.Named(name="Int", kind="SCALAR")
```

### Comparing `subgrounds-1.6.0/subgrounds/pagination/strategies.py` & `subgrounds-1.6.1/subgrounds/pagination/strategies.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,42 +65,84 @@
    selections (and sub-selections) containing undefined variables are removed.
 
 Depending on the strategy, the variable values computed at step 3 will change.
 """
 
 from __future__ import annotations
 
-from ast import Tuple
 from dataclasses import dataclass, field
 from functools import partial
 from itertools import count
-from typing import Any, Callable, Iterator, Literal, Optional
+from typing import Any, Callable, Iterator, Literal, Optional, Protocol
 
 from pipe import map, traverse
 
 from subgrounds.pagination.preprocess import (
     PaginationNode,
     generate_pagination_nodes,
     normalize,
     prune_doc,
 )
-from subgrounds.pagination.utils import PAGE_SIZE
 from subgrounds.query import Document
 from subgrounds.schema import SchemaMeta
 from subgrounds.utils import extract_data
 
+PAGE_SIZE = 900
+
 
 class StopPagination(Exception):
-    def __init__(self, *args: object) -> None:
-        super().__init__(*args)
+    """Raise within :class:`PaginationStategy` when pagination is completed, usually
+    within :func:`subgrounds.pagination.pagination.PaginationStrategy.step`.
+
+    Causes :func:`subgrounds.pagination.pagination.paginate` to be stopped.
+    """
 
 
 class SkipPagination(Exception):
-    def __init__(self, *args: object) -> None:
-        super().__init__(*args)
+    """Raise within :class:`PaginationStategy` should be skipped, usually within
+    :func:`subgrounds.pagination.pagination.PaginationStrategy.__init___`.
+
+    Causes :func:`subgrounds.pagination.pagination.paginate` to be skipped.
+    """
+
+
+class PaginationStrategy(Protocol):
+    def __init__(self, schema: SchemaMeta, document: Document) -> None:
+        """Initializes the pagination strategy. If there is no need for pagination given
+        the provided :class:`Document` ``document``, then the constructor should raise a
+        :class:`SkipPagination` exception.
+
+        Args:
+            schema: The schema of the API against which ``document`` will be executed
+            document: The query document
+        """
+        ...
+
+    def step(
+        self, page_data: dict[str, Any] | None = None
+    ) -> tuple[Document, dict[str, Any]]:
+        """Returns the new query document and its variables which will be executed to
+        get the next page of data.
+
+        If this is the first query made as part of the pagination strategy, then
+          ``page_data`` will be ``None``.
+
+        If pagination should be interupted (e.g.: if enough entities have been queried),
+        then this method should raise a :class:`StopPagination` exception.
+
+        Args:
+            page_data: The previous query's response data. If this is the first query
+              (i.e.: the first page of data), then it will be `None`. Defaults to None.
+
+        Returns:
+            tuple: A tuple `(doc, vars)` where `doc` is the query document that will be
+              executed to fetch the next page of data and `vars` are the variables for
+              that document.
+        """
+        ...
 
 
 @dataclass
 class LegacyStrategyArgGenerator:
     cursor: list[Cursor]
     active_idx: int = 0
 
@@ -122,21 +164,24 @@
             self.inner = list(page_node.inner | map(LegacyStrategyArgGenerator.Cursor))
             self.reset()
 
         @property
         def is_leaf(self):
             return len(self.inner) == 0
 
-        def update(self, data: dict) -> None:
-            """Moves ``self`` cursor forward according to previous response data ``data``
+        def update(self, data: dict[str, Any]) -> None:
+            """Moves `self` cursor forward according to previous response data `data`
+
             Args:
-              data (dict): Previous response data
+              data: Previous response data
+
             Raises:
               StopIteration: _description_
             """
+
             # Current node step
             index_field_data = list(
                 extract_data(
                     [
                         *self.page_node.key_path,
                         *self.page_node.filter_field.split("__"),
                     ],
@@ -163,19 +208,20 @@
             if (
                 (self.is_leaf and num_entities < PAGE_SIZE)
                 or (not self.is_leaf and num_entities == 0)
                 or (self.queried_entities == self.page_node.first_value)
             ):
                 raise StopPagination
 
-        def step(self, data: dict) -> None:
+        def step(self, data: dict[str, Any]) -> None:
             """Updates either ``self`` cursor or inner state machine depending on
             whether the inner state machine has reached its limit
+
             Args:
-              data (dict): _description_
+              data: _description_
             """
             if self.is_leaf:
                 self.update(data)
             else:
                 try:
                     self.inner[self.inner_idx].step(data)
                 except StopPagination:
@@ -193,19 +239,22 @@
                     self.page_node.first_value - self.queried_entities
                     if self.page_node.first_value - self.queried_entities < PAGE_SIZE
                     else PAGE_SIZE
                 )
             else:
                 return 1
 
-        def args(self) -> dict:
-            """Returns the pagination arguments for the current state of the state machine
+        def args(self) -> dict[str, Any]:
+            """Returns the pagination arguments for the current state of the
+             state machine
+
             Returns:
-                dict: _description_
+              _description_
             """
+
             args = {}
             args[f"first{self.page_node.node_idx}"] = self.first_arg_value()
 
             args[f"skip{self.page_node.node_idx}"] = (
                 self.page_node.skip_value if self.page_count == 0 else 0
             )
 
@@ -216,14 +265,15 @@
                 return args
             else:
                 inner_args = self.inner[self.inner_idx].args()
                 return args | inner_args
 
         def reset(self):
             """Reset state machine"""
+
             self.inner_idx = 0
             self.filter_value = self.page_node.filter_value
             self.queried_entities = 0
             self.stop = False
             self.page_count = 0
             self.keys = set()
 
@@ -257,44 +307,46 @@
         if len(pagination_nodes) == 0:
             raise SkipPagination
 
         self.arg_generator = LegacyStrategyArgGenerator(pagination_nodes)
         self.normalized_doc = normalize(schema, document, pagination_nodes)
 
     def step(
-        self, page_data: Optional[dict[str, Any]] = None
+        self, page_data: dict[str, Any] | None = None
     ) -> tuple[Document, dict[str, Any]]:
         args = self.arg_generator.step(page_data)
         trimmed_doc = prune_doc(self.normalized_doc, args)
-        return (trimmed_doc, args)
+        return trimmed_doc, args
 
 
 @dataclass
 class ShallowStrategyArgGenerator:
     @dataclass
     class Cursor:
-        # TODO: Add GreedyStrategy doc
         """Class used to generate the pagination variables for a given tree of
         ``PaginationNode`` objects.
 
         Attributes:
           page_node: The ``PaginationNode`` object which this cursor is iterating
-            through.
-          inner: The cursors for nested ``PaginationNodes``, if any.
+            through
+          inner: The cursors for nested ``PaginationNodes``, if any
           inner_idx: The index of the inner ``PaginationNode`` through which this cursor
-            iterating.
-          filter_value: The previous page's index value used to query the next data page.
+            iterating
+          filter_value: The previous page's index value used to query the next data page
             Depends on ``page_node.filter_field``, e.g.: if ``page_node.filter_field``
             is ``timestamp_gt``, then ``filter_value`` will be the highest timestamp
             the entities returned in the previous data page.
-          queried_entities: Counter keeping track of the total number of queried entities.
-          stop: Flag indicating whether or not to stop the cursor.
-          page_count: Counter keeping track of the total number data pages queried.
-          keys: Set keeping track of the keys of all queried entities to avoid duplicates.
+          queried_entities: Counter for the total number of queried entities
+          stop: Flag indicating whether or not to stop the cursor
+          page_count: Counter keeping track of the total number data pages queried
+          keys: Set of keys of all queried entities to avoid duplicates
+
+        # TODO: Add GreedyStrategy doc
         """
+
         page_node: PaginationNode
 
         inner: list[ShallowStrategyArgGenerator.Cursor]
         inner_idx: int = 0
 
         filter_value: Any = None
         queried_entities: int = 0
@@ -337,15 +389,15 @@
         def mapi(
             self,
             map_f: Callable[
                 [int, ShallowStrategyArgGenerator.Cursor],
                 ShallowStrategyArgGenerator.Cursor,
             ],
             priority: Literal["self"] | Literal["children"] = "self",
-            counter: Optional(count[int]) = None,
+            counter: count[int] | None = None,
         ) -> ShallowStrategyArgGenerator.Cursor:
             if counter is None:
                 counter = count()
 
             match priority:
                 case "self":
                     new_cursor = map_f(next(counter), self)
@@ -481,12 +533,38 @@
         if len(pagination_nodes) == 0:
             raise SkipPagination
 
         self.arg_generator = ShallowStrategyArgGenerator(pagination_nodes)
         self.normalized_doc = normalize(schema, document, pagination_nodes)
 
     def step(
-        self, page_data: Optional[dict[str, Any]] = None
-    ) -> Tuple[Document, dict[str, Any]]:
+        self, page_data: dict[str, Any] | None = None
+    ) -> tuple[Document, dict[str, Any]]:
         args = self.arg_generator.step(page_data)
         trimmed_doc = prune_doc(self.normalized_doc, args)
         return (trimmed_doc, args)
+
+
+class SkipStrategy:
+    """This strategy always raises a :class:`~subgrounds.pagination.SkipPagination`
+      when constructed or if *somehow* `step` is called.
+
+    This is the default if `None` is passed to the strategy (default for non-subgraphs).
+    """
+
+    def __init__(self, schema: SchemaMeta, document: Document) -> None:
+        raise SkipPagination
+
+    def step(
+        self, page_data: Optional[dict[str, Any]] = None
+    ) -> tuple[Document, dict[str, Any]]:
+        raise SkipPagination
+
+
+def normalize_strategy(
+    strategy: type[PaginationStrategy] | None = LegacyStrategy,
+    is_subgraph: bool = True,
+):
+    if strategy is not None and is_subgraph:
+        return strategy
+
+    return SkipStrategy
```

### Comparing `subgrounds-1.6.0/subgrounds/plotly_wrappers.py` & `subgrounds-1.6.1/subgrounds/plotly_wrappers.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.6.0/subgrounds/query.py` & `subgrounds-1.6.1/subgrounds/query.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,27 +20,29 @@
               └── Selection
 """
 
 from __future__ import annotations
 
 import logging
 import warnings
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, replace
 from functools import partial, reduce
-from typing import Any, Callable, Iterator, Literal, Optional, Protocol, TypeVar
+from typing import Any, Callable, Iterator, Literal, Protocol, TypeVar
 
 from pipe import map, take, traverse, where
+from typing_extensions import Self
 
 from .errors import SubgroundsError
 from .schema import SchemaMeta, TypeMeta, TypeRef
 from .utils import (
     extract_data,
     filter_map,
     filter_none,
     identity,
+    merge,
     rel_complement,
     union,
 )
 
 logger = logging.getLogger("subgrounds")
 warnings.simplefilter("default")
 
@@ -51,33 +53,33 @@
 class InputValue:
     class T(Protocol):
         @property
         def graphql(self) -> str:
             """Returns a GraphQL string representation of the input value
 
             Returns:
-              str: The GraphQL string representation of the input value
+              The GraphQL string representation of the input value
             """
             ...
 
         @property
         def is_variable(self) -> bool:
             """Returns True i.f.f. the input value is of type Variable
 
             Returns:
-              bool: True i.f.f. the input value is of type Variable, otherwise False
+              True i.f.f. the input value is of type Variable, otherwise False
             """
             ...
 
         @property
         def is_number(self) -> bool:
             """Returns True i.f.f. the input value is of type Float or Int
 
             Returns:
-              bool: True i.f.f. the input value is of type Float or Int, otherwise False
+              True i.f.f. the input value is of type Float or Int, otherwise False
             """
             ...
 
         def iter(self) -> Iterator[InputValue.T]:
             ...
 
     @dataclass(frozen=True)
@@ -259,23 +261,22 @@
 
 
 @dataclass(frozen=True)
 class VariableDefinition:
     """Representation of a GraphQL variable definition
 
     Attributes:
-      name (str): Name of the argument
-      type_ (TypeRef.T): GraphQL type of the argument
-      default (InputValue.T, optional): Default value of the variable.
-        Defaults to None.
+      name: Name of the argument
+      type_: GraphQL type of the argument
+      default: Default value of the variable. Defaults to None.
     """
 
     name: str
     type_: TypeRef.T
-    default: Optional[InputValue.T] = None
+    default: InputValue.T | None = None
 
     @property
     def graphql(self) -> str:
         """Returns the GraphQL string representation of the variable definition
 
         Example:
 
@@ -284,15 +285,15 @@
         ...   type_=TypeRef.NonNull(TypeRef.Named(name="Int", kind="SCALAR")),
         ...   default=InputValue.Int(100)
         ... )
         >>> print(vardef.graphql)
         $foo: Int! = 100
 
         Returns:
-            str: The GraphQL string representation of the variable definition
+          The GraphQL string representation of the variable definition
         """
 
         if self.default is None:
             return f"${self.name}: {TypeRef.graphql(self.type_)}"
         else:
             return (
                 f"${self.name}: {TypeRef.graphql(self.type_)} = {self.default.graphql}"
@@ -327,47 +328,45 @@
 
     def exists(self, predicate: Callable[[InputValue.T], bool]) -> bool:
         return any(self.iter() | map(predicate))
 
     def exists_vars(self, predicate: Callable[[InputValue.Variable], bool]) -> bool:
         return any(self.iter_vars() | map(predicate))
 
-    def find(self, predicate: Callable[[InputValue.T], bool]) -> Optional[InputValue.T]:
+    def find(self, predicate: Callable[[InputValue.T], bool]) -> InputValue.T | None:
         try:
             return next(self.iter() | where(predicate))
         except StopIteration:
             return None
 
     def find_var(
         self, predicate: Callable[[InputValue.Variable], bool]
-    ) -> Optional[InputValue.T]:
+    ) -> InputValue.T | None:
         try:
             return next(self.iter_vars() | where(predicate))
         except StopIteration:
             return None
 
     def all_defined(self, variables: Iterator[str]) -> bool:
         return self.for_all_vars(lambda var: var.name in variables)
 
 
 @dataclass(frozen=True)
 class Selection:
     """Represents a GraphQL field selection.
 
     Attributes:
-      fmeta (TypeMeta.FieldMeta): The type definition of the field being selected.
-      alias (str, optional): The alias of the field selection. Defaults to None.
-      arguments (list[Argument]): The arguments, if any, of the field selection.
-        Defaults to [].
-      selection (list[Selection]): The inner field selections, if any.
-        Defaults to [].
+      fmeta: The type definition of the field being selected.
+      alias: The alias of the field selection. Defaults to None.
+      arguments: The arguments, if any, of the field selection. Defaults to [].
+      selection: The inner field selections, if any. Defaults to [].
     """
 
     fmeta: TypeMeta.FieldMeta
-    alias: Optional[str] = None
+    alias: str | None = None
     arguments: list[Argument] = field(default_factory=list)
     selection: list[Selection] = field(default_factory=list)
 
     @property
     def key(self):
         if self.alias is not None:
             return self.alias
@@ -432,42 +431,45 @@
         return list(f(self))
 
     # ================================================================
     # Generic functions
     # ================================================================
     def iter(self) -> Iterator[Selection]:
         """Returns an iterator over all ``Selections`` of the current selection tree."""
+
         yield self
         for inner in self.selection:
             yield from inner.iter()
 
     def iter_args(self, recurse: bool = True) -> Iterator[Argument]:
         """Returns an iterator over all ``Arguments`` of the current ``Selection``.
 
         If ``recurse == True``, then the iterator also includes ``Arguments`` of
         inner ``Selections``.
         """
+
         for arg in self.arguments:
             yield arg
 
         if recurse:
             for inner in self.selection:
                 yield from inner.iter_args()
 
-    def filter(self, predicate: Callable[[Selection], bool]) -> Optional[Selection]:
+    def filter(self, predicate: Callable[[Selection], bool]) -> Selection | None:
         """Returns a new ``Selection`` object containing all attributes of the current
         ``Selection`` if ``predicate(self) == True`` and ``None`` otherwise. The
         function if also applied recursively to inner ``Selections``.
 
         Args:
-            predicate (Callable[[Selection], bool]): _description_
+          predicate: _description_
 
         Returns:
-            Optional[Selection]: _description_
+          _description_
         """
+
         if predicate(self):
             return Selection(
                 fmeta=self.fmeta,
                 alias=self.alias,
                 arguments=self.arguments,
                 selection=list(
                     self.selection
@@ -484,19 +486,19 @@
         the current ``Selection`` except for ``Arguments`` for which
         ``predicate(arg) == True``.
 
         If ``recurse == True``, then the function is applied recursively to
         inner ``Selections``
 
         Args:
-            predicate (Callable[[Argument], bool]): _description_
-            recurse (bool, optional): _description_. Defaults to True.
+          predicate: _description_
+          recurse: _description_. Defaults to True.
 
         Returns:
-            Selection: _description_
+          _description_
         """
         return Selection(
             fmeta=self.fmeta,
             alias=self.alias,
             arguments=list(self.arguments | where(predicate)),
             selection=list(
                 self.selection
@@ -512,20 +514,20 @@
         priority: Literal["self"] | Literal["children"] = "self",
     ) -> Selection:
         """Returns a new ``Selection`` object containing the same selection tree
         as the current ``Selection`` where each ``Selection`` object ``s`` is
         ``map_f(s)``
 
         Args:
-            map_f (Callable[[Selection], Selection]): Mapping function to apply
-              to each ``Selection``
+          map_f: Mapping function to apply to each ``Selection``
 
         Returns:
-            Selection: _description_
+          _description_
         """
+
         match priority:
             case "self":
                 new_selection = map_f(self)
 
                 return Selection(
                     fmeta=new_selection.fmeta,
                     alias=new_selection.alias,
@@ -553,43 +555,45 @@
                 raise SubgroundsError(f"map: invalid priority {priority}")
 
     def map_args(
         self,
         map_f: Callable[[Argument], Argument | list[Argument]],
         recurse: bool = True,
     ) -> Selection:
-        """Replaces each ``Argument`` ``arg`` in the current ``Selection`` with ``map_f(arg)``
-        and returns a new ``Selection`` object containinf the modified arguments.
+        """Replaces each ``Argument`` ``arg`` in the current ``Selection`` with
+         ``map_f(arg)`` and returns a new ``Selection`` object containing
+         the modified arguments.
 
         If ``recurse == True``, then the function is applied recursively to inner
         ``Selections``.
 
         Args:
-            map_f (Callable[[Argument], Argument | list[Argument]]): _description_
-            recurse (bool, optional): _description_. Defaults to True.
+          map_f: _description_
+          recurse: _description_. Defaults to True.
 
         Returns:
-            Selection: _description_
+          _description_
         """
+
         return Selection(
             fmeta=self.fmeta,
             alias=self.alias,
             arguments=list(self.arguments | map(map_f)),
             selection=list(
                 self.selection
                 | map(partial(Selection.map_args, map_f=map_f))
                 | traverse
             )
             if recurse
             else self.selection,
         )
 
     def filter_map(
-        self, map_f: Callable[[Selection], Optional[Selection]]
-    ) -> Optional[Selection]:
+        self, map_f: Callable[[Selection], Selection | None]
+    ) -> Selection | None:
         new_selection = map_f(self)
 
         if new_selection is not None:
             return Selection(
                 fmeta=new_selection.fmeta,
                 alias=new_selection.alias,
                 arguments=new_selection.arguments,
@@ -599,15 +603,15 @@
                 ),
             )
 
         return None
 
     def filter_map_args(
         self,
-        map_f: Callable[[Argument], Optional[Argument | list[Argument]]],
+        map_f: Callable[[Argument], Argument | list[Argument | None]],
         recurse: bool = True,
     ) -> Selection:
         return Selection(
             fmeta=self.fmeta,
             alias=self.alias,
             arguments=list(self.arguments | filter_map(map_f) | traverse),
             selection=list(
@@ -655,23 +659,23 @@
             return any(
                 self.selection
                 | map(partial(Selection.exists_args, predicate=predicate))
             )
 
         return False
 
-    def find(self, predicate: Callable[[Selection], bool]) -> Optional[Selection]:
+    def find(self, predicate: Callable[[Selection], bool]) -> Selection | None:
         try:
             return next(self.iter() | where(predicate))
         except StopIteration:
             return None
 
     def find_args(
         self, predicate: Callable[[Argument], bool], recurse: bool = True
-    ) -> Optional[Argument]:
+    ) -> Argument | None:
         try:
             return next(self.iter_args(recurse=recurse) | where(predicate))
         except StopIteration:
             return None
 
     def find_all(self, predicate: Callable[[Selection], bool]) -> list[Selection]:
         return list(self.iter() | where(predicate))
@@ -691,28 +695,28 @@
         inner = list(
             self.selection
             | map(partial(Selection.fold, fold_f=fold_f, parents=[*parents, self]))
             | traverse
         )
         return fold_f(self, parents, inner)
 
-    def contains_list(self: Selection) -> bool:
+    def contains_list(self) -> bool:
         """Returns True i.f.f. the selection :attr:`self` selects a field of type
         list.
 
         Args:
-          self (Selection): The selection to traverse
+          self: The selection to traverse
 
         Returns:
-          bool: True if selection or nested selections selects a list field. False otherwise.
+          True if selection or nested selections selects a list field. False otherwise.
         """
 
         return self.exists(lambda select: select.fmeta.type_.is_list)
 
-    def split(self: Selection) -> list[Selection]:
+    def split(self) -> list[Selection]:
         """Returns a list of selections where each of the selections corresponds
         to a single selection path from the root to a leaf for each leaf selected
         in :attr:`self`.
 
         Example (simplified, does not show all attributes):
 
         >>> select = Selection('foo', inner=[
@@ -720,24 +724,27 @@
         ...     Selection('field0', inner=[]),
         ...     Selection('field1', inner=[]),
         ...   ]),
         ...   Selection('x', inner=[])
         ... ])
         >>> split(select)
         [
-          Selection('foo', inner=[Selection('bar', inner=[Selection('field0', inner=[])])]),
-          Selection('foo', inner=[Selection('bar', inner=[Selection('field1', inner=[])])]),
-          Selection('foo', inner=[Selection('x', inner=[])]),
+          Selection(
+            'foo', inner=[Selection('bar', inner=[Selection('field0', inner=[])])]),
+          Selection(
+            'foo', inner=[Selection('bar', inner=[Selection('field1', inner=[])])]),
+          Selection(
+            'foo', inner=[Selection('x', inner=[])]),
         ]
 
         Args:
-          self (Selection): The selection to split
+          self: The selection to split
 
         Returns:
-          list[Selection]: The split selections
+          The split selections
         """
 
         match self:
             case Selection(_, _, _, [] | None):
                 return [self]
             case Selection(fmeta, alias, args, inner_select):
                 return list(
@@ -748,62 +755,62 @@
                         lambda inner_select: Selection(fmeta, alias, args, inner_select)
                     )
                 )
 
     def extract_data(self: Selection, data: dict | list[dict]) -> list[Any] | Any:
         return extract_data(self.data_path, data)
 
-    def add(self: Selection, new_selections: Selection | list[Selection]) -> Selection:
+    def add(self, new_selections: Selection | list[Selection]) -> Selection:
         """Returns a new selection consisting of a copy of :attr:`self` expanded
         with the selection(s) :attr:`new_selections`. It is assumed that
         :attr:`new_selections` are inner selections of the root selection
         :attr:`self`.
 
         Args:
-          self (Selection): The Selection object to be expanded
-          new_selections (Selection | list[Selection]): A single or multiple
-            Selection object(s) to be added to :attr:`self`
+          self: The Selection object to be expanded
+          new_selections: A single or multiple Selection object(s) to be added to
+            :attr:`self`
 
         Returns:
-          Selection: The resulting new selection, i.e.: :attr:`self`
-            expanded with :attr:`new_selections`
+          The resulting new selection, i.e.: :attr:`self` expanded with
+            :attr:`new_selections`
         """
 
         match new_selections:
             case Selection() as new_selection:
                 return self.add([new_selection])
 
             case list() as new_selections:
                 return Selection(
                     fmeta=self.fmeta,
                     alias=self.alias,
+                    arguments=self.arguments,
                     selection=union(
                         self.selection,
                         new_selections,
                         key=lambda select: select.fmeta.name,
                         combine=Selection.combine,
                     ),
                 )
 
-    def remove(self: Selection, to_remove: Selection | list[Selection]) -> Selection:
+    def remove(self, to_remove: Selection | list[Selection]) -> Selection:
         """Returns a new Selection object consisting of a copy of :attr:`self`
         without the selections in :attr:`selections_to_remove`.
 
         Args:
-          to_remove (Selection | list[Selection]): The selection(s) to remove from
-            :attr:`self`
+          to_remove: The selection(s) to remove from :attr:`self`
 
         Returns:
-          Selection: The new trimmed down selection, i.e.: :attr:`self` without
+          The new trimmed down selection, i.e.: :attr:`self` without
             :attr:`selections_to_remove`
         """
 
         def combine(
             select: Selection, selection_to_remove: Selection
-        ) -> Optional[Selection]:
+        ) -> Selection | None:
             if selection_to_remove.selection == []:
                 return None
             else:
                 return select.remove(selection_to_remove.selection)
 
         # TODO: Resolve mypy complaints
         match to_remove:
@@ -829,18 +836,18 @@
         """Returns all arguments in the current selection which have been given a
         variable as value.
 
         If ``recurse == True``, then the function is applied recursively to inner
         selections.
 
         Args:
-            recurse (bool, optional): _description_. Defaults to True.
+          recurse: _description_. Defaults to True.
 
         Returns:
-            list[Argument]: _description_
+          _description_
         """
         for arg in self.iter_args(recurse=recurse):
             if type(arg.value) == InputValue.Variable:
                 yield arg
 
     def infer_variable_definitions(self: Selection) -> list[VariableDefinition]:
         def vardef_of_arg(arg):
@@ -889,18 +896,18 @@
 
     @staticmethod
     def merge(selections: list[Selection]) -> list[Selection]:
         """Returns a list of Selection objects resulting from merging
         :attr:`selections` to the extent possible.
 
         Args:
-          selections (list[Selection]): The selections to be merged
+          selections The selections to be merged
 
         Returns:
-          list[Selection]: _description_
+          _description_
         """
 
         def f(selections: list[Selection], other: Selection) -> list[Selection]:
             try:
                 next(selections | where(lambda select: select.key == other.key))
                 return list(
                     selections
@@ -911,24 +918,24 @@
                     )
                 )
             except StopIteration:
                 return selections + [other]
 
         return reduce(f, selections, [])
 
-    def contains(self: Selection, other: Selection) -> bool:
+    def contains(self, other: Selection) -> bool:
         """Returns True i.f.f. the Selection :attr:`other` is a subtree of the
         Selection :attr:`self` and False otherwise
 
         Args:
-          self (Selection): The selection
-          other (Selection): The subselection
+          self: The selection
+          other: The subselection
 
         Returns:
-          bool: True i.f.f. :attr:`other` is in :attr:`self`
+          True i.f.f. :attr:`other` is in :attr:`self`
         """
 
         if (
             self.fmeta == other.fmeta
             and rel_complement(
                 other.selection, self.selection, key=lambda s: s.fmeta.name
             )
@@ -946,109 +953,100 @@
                         s,
                     )
                 )
             )
         else:
             return False
 
-    def contains_argument(self: Selection, argname: str, recurse: bool = True) -> bool:
+    def contains_argument(self, argname: str, recurse: bool = True) -> bool:
         """Returns True i.f.f. there is an Argument object in :attr:`self` named
         :attr:`argname`. If :attr:`recurse` is True, then the method also checks the
         nested selections for an argument named :attr:`argname`.
 
         Args:
-          self (Selection): The selection
-          argname (str): The name of the argument
-          recurse (bool, optional): Flag indicating whether or not the method should
-            be run recursively on nested selections. Defaults to True.
+          argname: The name of the argument
+          recurse: Flag indicating whether or not the method should be run recursively
+            on nested selections. Defaults to True.
 
         Returns:
-          bool: True i.f.f. there is an argument named :attr:`argname` in :attr:`self`
+          True i.f.f. there is an argument named :attr:`argname` in :attr:`self`
         """
 
         return self.exists_args(lambda arg: arg.name == argname, recurse=recurse)
 
-    def get_argument(
-        self: Selection, argname: str, recurse: bool = True
-    ) -> Optional[Argument]:
+    def get_argument(self, argname: str, recurse: bool = True) -> Argument | None:
         """Returns an Argument object corresponding to the argument in the Selection
         object :attr:`select` with name :attr:`argname`. If :attr:`select` does not
         contain such an argument and :attr:`recurse` is True, then the function is
         called recursively on :attr:`select`'s inner selections. If no such argument
         is found in :attr:`select` or its inner selections, then the function raises
         an exception.
 
         Args:
-          select (Selection): The selection to scan
-          argname (str): The name of the argument to find
-          recurse (bool, optional): Flag indicating whether or not the method should
-            be run recursively on nested selections. Defaults to True.
+          argname: The name of the argument to find
+          recurse: Flag indicating whether or not the method should be run recursively
+            on nested selections. Defaults to True.
 
         Raises:
           KeyError: If no argument named :attr:`argname` exists in the selection
             :attr:`self`.
 
         Returns:
-          Argument: The argument in :attr:`select` with name :attr:`argname` (if any).
+          The argument in :attr:`select` with name :attr:`argname` (if any).
         """
 
         return self.find_args(lambda arg: arg.name == argname, recurse=recurse)
 
     def get_argument_by_variable(
-        self: Selection, varname: str, recurse: bool = True
-    ) -> Optional[Argument]:
+        self, varname: str, recurse: bool = True
+    ) -> Argument | None:
         """Returns an Argument object corresponding to the argument in the Selection
         object :attr:`select` whose value is a variable named :attr:`varname`. If
         :attr:`select` does not contain such an argument and :attr:`recurse` is True,
         then the function is called recursively on :attr:`select`'s inner selections.
         If no such argument is found in :attr:`select` or its inner selections, then
         the function raises an exception
 
         Args:
-          select (Selection): The selection to scan
-          varname (str): The name of the variable to find
-          recurse (bool, optional): Flag indicating whether or not the function
-            should be run recursively. Defaults to True.
+          varname: The name of the variable to find
+          recurse: Flag indicating whether or not the method should be run recursively.
+            Defaults to True.
 
         Raises:
           KeyError: If no argument with variable value named :attr:`varname` exists
             in the selection :attr:`self`.
 
         Returns:
-          Argument: The argument in :attr:`select` with variable value named
-            :attr:`varname` if it exists
+          The argument in :attr:`select` with variable value named :attr:`varname`
+            if it exists
         """
 
         return self.find_args(
             lambda arg: arg.exists_vars(lambda var: var.name == varname),
             recurse=recurse,
         )
 
     # TODO: Replace substitute_arg calls by map_args call
     def substitute_arg(
-        self: Selection,
-        argname: str,
-        replacement: Argument | list[Argument],
-        recurse: bool = True,
+        self, argname: str, replacement: Argument | list[Argument], recurse: bool = True
     ) -> Selection:
         """Returns a new Selection object containing the same data as :attr:`self`
         with the argument named :attr:`argname` replaced with :attr:`replacement`.
         If :attr:`recurse` is True, then the method is called recursively on
         :attr:`self`'s inner selections and the substitution is also applied to the
         latter.
 
         Args:
-          self (Selection): _description_
-          argname (str): The name of the argument to substitute.
-          replacement (Argument | list[Argument]): The argument(s) replacement
-          recurse (bool, optional): Flag indicating whether or not the method
-            should be run recursively. Defaults to True.
+          argname: The name of the argument to substitute.
+          replacement: The argument(s) replacement
+          recurse: Flag indicating whether or not the method should be run recursively.
+            Defaults to True.
 
         Returns:
-          Selection: _description_
+          _description_
         """
 
         return self.map_args(
             lambda arg: replacement if arg.name == argname else arg, recurse=recurse
         )
 
     def select(self: Selection, other: Selection) -> Selection:
@@ -1068,57 +1066,52 @@
                             | map(lambda s_: Selection.select(s_, s))
                             | take(1)
                         )
                     )
                 ),
             )
 
-    def prune_undefined(self, variables: Iterator[str]) -> Optional[Selection]:
+    def prune_undefined(self, variables: Iterator[str]) -> Selection | None:
         """Return a new ``Selection`` containing the subtree of the current
         ``Selection`` where all argument ``InputValues`` are defined,
         i.e.: each argument's ``InputValue`` is either
             1) not of type ``InputValue.Variable``
             or
             2) of type ``InputValue.Variable``
             and
             the variable name is contained in ``variables``.
 
         Args:
-            variables (Iterator[str]): An iterator over defined variables
+          variables: An iterator over defined variables
 
         Returns:
-            Selection: A new pruned ``Selection`` object
+          A new pruned ``Selection`` object
         """
 
         return self.filter(
             lambda select: select.for_all_args(
                 lambda arg: arg.all_defined(variables), recurse=False
             )
         )
 
-    # TODO: Function to recover an approximate selection from a JSON data object
-    # @staticmethod
-    # def of_json(data: dict) -> Selection:
-    #   pass
-
 
 @dataclass(frozen=True)
 class Query:
-    name: Optional[str] = None
+    name: str | None = None
     selection: list[Selection] = field(default_factory=list)
 
     # Variables as query arguments, not the values of those variables
     variables: list[VariableDefinition] = field(default_factory=list)
 
     @property
     def graphql(self) -> str:
         """Returns a string containing a GraphQL query matching the current query
 
         Returns:
-          str: The string containing the GraphQL query
+          The string containing the GraphQL query
         """
 
         selection_str = "\n".join(
             [select.graphql(level=1) for select in self.selection]
         )
 
         if len(self.variables) > 0:
@@ -1153,38 +1146,38 @@
             yield vardef
 
     def filter(self, predicate: Callable[[Selection], bool]) -> Query:
         """Returns a new ``Query`` object containing all selections ``s`` that satisfy
         ``predicate(s) == True``.
 
         Args:
-            predicate (Callable[[Selection], bool]): _description_
+          predicate: _description_
 
         Returns:
-            Query: _description_
+          _description_
         """
 
         return Query(
             name=self.name,
             selection=list(
                 self.selection
                 | filter_map(partial(Selection.filter, predicate=predicate))
             ),
             variables=self.variables,
         )
 
     def filter_args(self, predicate: Callable[[Argument], bool]) -> Query:
-        """Returns a new ``Query`` object containing all selections arguments ``arg`` that satisfy
-        ``predicate(arg) == True``.
+        """Returns a new ``Query`` object containing all selections arguments ``arg``
+        that satisfy ``predicate(arg) == True``.
 
         Args:
-            predicate (Callable[[Argument], bool]): _description_
+          predicate: _description_
 
         Returns:
-            Query: _description_
+          _description_
         """
 
         return Query(
             name=self.name,
             selection=list(
                 self.selection
                 | map(partial(Selection.filter_args, predicate=predicate))
@@ -1201,42 +1194,43 @@
 
     def map(
         self,
         map_f: Callable[[Selection], Selection],
         priority: Literal["self"] | Literal["children"] = "self",
     ) -> Query:
         """Applies the function ``map_f`` to each ``Selection`` in the current
-        ``Query`` and returns a new ``Query`` object containing the resulting ``Selections``.
+         ``Query`` and returns a new ``Query`` object containing the resulting
+         ``Selections``.
 
         Args:
-            map_f (Callable[[Selection], Selection]): Mapping function to apply
-              to each ``Selection``
+          map_f: Mapping function to apply to each ``Selection``
 
         Returns:
-            Query: _description_
+          _description_
         """
 
         return Query(
             name=self.name,
             selection=list(
                 self.selection
                 | map(partial(Selection.map, map_f=map_f, priority=priority))
             ),
             variables=self.variables,
         )
 
     def map_args(self, map_f: Callable[[Argument], Argument]) -> Query:
         """Applies the function ``map_f`` to each ``Argument`` in the current
-        ``Query`` and returns a new ``Query`` object containing the resulting ``Arguments``.
+         ``Query`` and returns a new ``Query`` object containing the resulting
+         ``Arguments``.
 
         Args:
-            map_f (Callable[[Argument], Argument]): _description_
+          map_f: _description_
 
         Returns:
-            Selection: _description_
+          _description_
         """
 
         return Query(
             name=self.name,
             selection=list(
                 self.selection | map(partial(Selection.map_args, map_f=map_f))
             ),
@@ -1248,34 +1242,34 @@
     ) -> Query:
         return Query(
             name=self.name,
             selection=self.selection,
             variables=list(self.variables | map(map_f)),
         )
 
-    def filter_map(self, map_f: Callable[[Selection], Optional[Selection]]) -> Query:
+    def filter_map(self, map_f: Callable[[Selection], Selection | None]) -> Query:
         return Query(
             name=self.name,
             selection=list(
                 self.selection | filter_map(partial(Selection.filter_map, map_f=map_f))
             ),
             variables=self.variables,
         )
 
-    def filter_map_args(self, map_f: Callable[[Argument], Optional[Argument]]) -> Query:
+    def filter_map_args(self, map_f: Callable[[Argument], Argument | None]) -> Query:
         return Query(
             name=self.name,
             selection=list(
                 self.selection | map(partial(Selection.filter_map_args, map_f=map_f))
             ),
             variables=self.variables,
         )
 
     def filter_map_vardefs(
-        self, map_f: Callable[[VariableDefinition], Optional[VariableDefinition]]
+        self, map_f: Callable[[VariableDefinition], VariableDefinition | None]
     ) -> Query:
         return Query(
             name=self.name,
             selection=self.selection,
             variables=list(self.variables | filter_map(map_f)),
         )
 
@@ -1299,29 +1293,29 @@
         return any(
             self.selection | map(partial(Selection.exists_args, predicate=predicate))
         )
 
     def exists_vardefs(self, predicate: Callable[[VariableDefinition], bool]) -> bool:
         return any(self.variables | map(predicate))
 
-    def find(self, predicate: Callable[[Selection], bool]) -> Optional[Selection]:
+    def find(self, predicate: Callable[[Selection], bool]) -> Selection | None:
         try:
             return next(self.iter() | where(predicate))
         except StopIteration:
             return None
 
-    def find_args(self, predicate: Callable[[Argument], bool]) -> Optional[Argument]:
+    def find_args(self, predicate: Callable[[Argument], bool]) -> Argument | None:
         try:
             return next(self.iter_args() | where(predicate))
         except StopIteration:
             return None
 
     def find_vardefs(
         self, predicate: Callable[[VariableDefinition], bool]
-    ) -> Optional[VariableDefinition]:
+    ) -> VariableDefinition | None:
         try:
             return next(self.iter_vardefs() | where(predicate))
         except StopIteration:
             return None
 
     T = TypeVar("T")
 
@@ -1337,20 +1331,19 @@
         )
 
     def add(self: Query, other: Query | Selection | list[Selection]) -> Query:
         """Returns a new Query containing all selections in :attr:'self' along with
         the new selections in :attr:`other`
 
         Args:
-          self (Query): The query to which new selection(s) or query are to be added
-          other (Query | Selection | list[Selection]): The new selection(s)
-          or query to be added to the query
+          self: The query to which new selection(s) or query are to be added
+          other: The new selection(s) or query to be added to the query
 
         Returns:
-          Query: A new `Query` objects containing all selections
+          A new `Query` objects containing all selections
         """
 
         match other:
             case Selection() as new_selection:
                 return self.add([new_selection])
 
             case Query() as query:
@@ -1384,38 +1377,108 @@
         :attr:`self` minus the subquery or selection(s) specified in :attr:`other`.
 
         Note: :attr:`other` does not need to be a "full" selection (i.e.: a
         selection all the way to leaves of the GraphQL schema).
 
         Example:
 
-        >>> og_selection = Selection(TypeMeta.FieldMeta('pair', description="", args=[], type=TypeRef.non_null_list("Pair", kind="OBJECT")), None, [], [
-        ...   Selection(TypeMeta.FieldMeta('token0', description="", args=[], type=TypeRef.Named(name="Token", kind="OBJECT")), None, [], [
-        ...     Selection(TypeMeta.FieldMeta('id', description="", args=[], type=TypeRef.Named(name="String", kind="SCALAR")), None, [], []),
-        ...     Selection(TypeMeta.FieldMeta('name', description="", args=[], type=TypeRef.Named(name="String", kind="SCALAR")), None, [], []),
-        ...     Selection(TypeMeta.FieldMeta('symbol', description="", args=[], type=TypeRef.Named(name="String", kind="SCALAR")), None, [], []),
-        ...   ])
-        ... ])
-        >>> selection_to_remove = Selection(TypeMeta.FieldMeta('token0', description="", args=[], type=TypeRef.Named(name="Token", kind="OBJECT")), None, [], [])
+        >>> og_selection = Selection(
+        ...     TypeMeta.FieldMeta(
+        ...         'pair',
+        ...         description="",
+        ...         args=[],
+        ...         type=TypeRef.non_null_list("Pair", kind="OBJECT")
+        ...     ),
+        ...     None,
+        ...     [],
+        ...     [
+        ...         Selection(
+        ...             TypeMeta.FieldMeta(
+        ...                 'token0',
+        ...                 description="",
+        ...                 args=[],
+        ...                 type=TypeRef.Named(name="Token", kind="OBJECT")
+        ...             ),
+        ...             None,
+        ...             [],
+        ...             [
+        ...                 Selection(
+        ...                     TypeMeta.FieldMeta(
+        ...                         'id',
+        ...                         description="",
+        ...                         args=[],
+        ...                         type=TypeRef.Named(name="String", kind="SCALAR")
+        ...                     ),
+        ...                     None,
+        ...                     [],
+        ...                     []
+        ...                 ),
+        ...                 Selection(
+        ...                     TypeMeta.FieldMeta(
+        ...                         'name',
+        ...                         description="",
+        ...                         args=[],
+        ...                         type=TypeRef.Named(name="String", kind="SCALAR")
+        ...                     ),
+        ...                     None,
+        ...                     [],
+        ...                     []
+        ...                 ),
+        ...                 Selection(
+        ...                     TypeMeta.FieldMeta(
+        ...                         'symbol',
+        ...                         description="",
+        ...                         args=[],
+        ...                         type=TypeRef.Named(name="String", kind="SCALAR")
+        ...                     ),
+        ...                     None,
+        ...                     [],
+        ...                     []
+        ...                 ),
+        ...             ]
+        ...         )
+        ...     ]
+        ... )
+        >>> selection_to_remove = Selection(
+        ...     TypeMeta.FieldMeta(
+        ...         'token0',
+        ...         description="",
+        ...         args=[],
+        ...         type=TypeRef.Named(name="Token", kind="OBJECT")
+        ...     ),
+        ...     None,
+        ...     [],
+        ...     []
+        ... )
         >>> og_selection.remove(selection_to_remove)
-        Selection(TypeMeta.FieldMeta('pair', description="", args=[], type=TypeRef.non_null_list("Pair", kind="OBJECT")), None, [], [])
+        Selection(
+            TypeMeta.FieldMeta(
+                'pair',
+                description="",
+                args=[],
+                type=TypeRef.non_null_list("Pair", kind="OBJECT")
+            ),
+            None,
+            [],
+            []
+        )
 
         Args:
           query (Query): The query to which a selection has to be removed
           other (Query | Selection | list[Selection]): The subquery or
             selection(s) to remove from :attr:`self`
 
         Returns:
           Query: A new `Query` object containing the original query selections
             minus :attr:`other`
         """
 
         def combine(
             select: Selection, selection_to_remove: Selection
-        ) -> Optional[Selection]:
+        ) -> Selection | None:
             if selection_to_remove.selection == []:
                 return None
             else:
                 return select.remove(selection_to_remove.selection)
 
         match other:
             case Selection() as to_remove:
@@ -1469,15 +1532,15 @@
         return any(
             self.selection | map(lambda select: Selection.contains(select, selection))
         )
 
     def contains_argument(self, argname: str) -> bool:
         return self.exists_args(lambda arg: arg.name == argname)
 
-    def get_argument(self, argname: str) -> Optional[Argument]:
+    def get_argument(self, argname: str) -> Argument | None:
         return self.find_args(lambda arg: arg.name == argname)
 
     # TODO: Replace substitute_arg calls by map_args call
     @staticmethod
     def substitute_arg(
         query: Query, arg_name: str, replacement: Argument | list[Argument]
     ) -> Query:
@@ -1495,26 +1558,27 @@
             ),
             variables=query.variables,
         )
 
     # TODO: Cleanup select
     @staticmethod
     def contains(query: Query, other: Query) -> bool:
-        """Returns True i.f.f. all selections in `other` are contained in `query`. In other words,
-        returns true i.f.f. `other` is a subset of `query`.
+        """Returns True i.f.f. all selections in `other` are contained in `query`.
+        In other words, returns true i.f.f. `other` is a subset of `query`.
 
-        Note: `other` does not need to include "full" selections (i.e.: selections all the way to
-        leaves of the GraphQL schema).
+        Note: `other` does not need to include "full" selections
+        (i.e.: selections all the way to leaves of the GraphQL schema).
 
         Args:
           query (Query): The query that is to be checked
           other (Query): The query that has to be in `query`
 
         Returns:
-          bool: True i.f.f. all selections in `other` are contained in `query`, otherwise False
+          bool: True i.f.f. all selections in `other` are contained in `query`,
+           otherwise False
         """
 
         return all(other.selection | map(partial(Query.contains_selection, query)))
 
     # TODO: Cleanup select
     @staticmethod
     def select(query: Query, other: Query) -> Query:
@@ -1649,15 +1713,15 @@
         return Document(
             url=self.url,
             query=self.query.map_args(map_f),
             fragments=self.fragments,  # TODO: Add mapping to fragments
             variables=self.variables,
         )
 
-    def filter_map(self, map_f: Callable[[Selection], Optional[Selection]]) -> Document:
+    def filter_map(self, map_f: Callable[[Selection], Selection | None]) -> Document:
         return Document(
             url=self.url,
             query=self.query.filter_map(map_f),
             fragments=self.fragments,  # TODO: Add mapping to fragments
             variables=self.variables,
         )
 
@@ -1705,49 +1769,64 @@
             query=self.query.prune_undefined(variables),
             fragments=self.fragments,
             variables=variables,
         )
 
 
 @dataclass(frozen=True)
+class DocumentResponse:
+    # TODO: update to recursive json dict w/ pydantic 2.0
+    url: str
+    data: dict[str, Any] = field(default_factory=dict)
+
+    def combine(self: Self, other: Self):
+        return replace(self, data=merge(self.data, other.data))
+
+
+@dataclass(frozen=True)
 class DataRequest:
     documents: list[Document] = field(default_factory=list)
 
     @property
     def graphql(self):
         return "\n".join(list(self.documents | map(lambda doc: doc.graphql)))
 
-    @staticmethod
-    def combine(req: DataRequest, other: DataRequest) -> None:
-        return DataRequest(
+    @classmethod
+    def combine(cls, req: DataRequest, other: DataRequest):
+        return cls(
             documents=union(
                 req.documents,
                 other.documents,
                 key=lambda doc: doc.url,
                 combine=Document.combine,
             )
         )
 
-    @staticmethod
-    def transform(req: DataRequest, f: Callable[[Document], Document]) -> DataRequest:
-        return DataRequest(documents=list(req.documents | map(f)))
+    @classmethod
+    def transform(cls, req: DataRequest, f: Callable[[Document], Document]):
+        return cls(documents=list(req.documents | map(f)))
+
+    @classmethod
+    def single_query(cls, url: str, query: Query):
+        return cls([Document(url, query)])
+
+    @classmethod
+    def single_document(cls, doc: Document):
+        return cls([doc])
 
-    @staticmethod
-    def single_query(url: str, query: Query) -> DataRequest:
-        return DataRequest([Document(url, query)])
+    def add_documents(self, docs: Document | list[Document]):
+        return replace(self, documents=list((self.documents, docs) | traverse))
 
-    @staticmethod
-    def single_document(doc: Document) -> DataRequest:
-        return DataRequest([doc])
 
-    @staticmethod
-    def add_documents(
-        self: DataRequest, docs: Document | list[Document]
-    ) -> DataRequest:
-        return DataRequest(list([self.documents, docs] | traverse))
+@dataclass(frozen=True)
+class DataResponse:
+    responses: list[DocumentResponse] = field(default_factory=list)
+
+    def add_responses(self, resps: DocumentResponse | list[DocumentResponse]):
+        return replace(self, responses=list((self.responses, resps) | traverse))
 
 
 # ================================================================
 # Utility functions
 # ================================================================
 def selections_of_object(
     schema: SchemaMeta, object_: TypeMeta.ObjectMeta | TypeMeta.InterfaceMeta
@@ -1826,36 +1905,38 @@
             case (value, typ, non_null):
                 raise TypeError(f"mk_input_value({value}, {typ}, {non_null})")
 
     return fmt_value(argmeta.type_, value)
 
 
 def arguments_of_field_args(
-    schema: SchemaMeta, field: TypeMeta.FieldMeta, args: Optional[dict[str, Any]]
+    schema: SchemaMeta, field: TypeMeta.FieldMeta, args: dict[str, Any] | None
 ) -> list[Argument]:
     if args is None:
         args = {}
 
-    def f(arg_meta: TypeMeta.ArgumentMeta) -> Optional[Argument]:
+    def f(arg_meta: TypeMeta.ArgumentMeta) -> Argument | None:
         if arg_meta.name in args:
             return Argument(
                 arg_meta.name,
                 input_value_of_argument(schema, arg_meta, args[arg_meta.name]),
             )
         else:
             if (arg_meta.default_value) or (not TypeRef.is_non_null(arg_meta.type_)):
                 return None
             else:
                 raise TypeError(
-                    f"arguments_of_field_args: Argument {arg_meta.name} of field {field.name} is required but not provided!"
+                    f"arguments_of_field_args: Argument {arg_meta.name} of field"
+                    f" {field.name} is required but not provided!"
                 )
 
     # TODO: Add warnings if arguments are not used
 
     match field:
         case TypeMeta.FieldMeta() as field:
             args = [f(arg_meta) for arg_meta in field.arguments]
             return list(filter(lambda arg: arg is not None, args))
         case _:
             raise TypeError(
-                f"arguments_of_field_args: TypeMeta {field.name} is not of type FieldMeta"
+                f"arguments_of_field_args: TypeMeta {field.name}"
+                " is not of type FieldMeta"
             )
```

### Comparing `subgrounds-1.6.0/subgrounds/schema.py` & `subgrounds-1.6.1/subgrounds/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,20 +89,18 @@
             inner=TypeRef.List(
                 inner=TypeRef.NonNull(inner=TypeRef.Named(name=name, kind=kind))
             )
         )
 
     @staticmethod
     def root_type_name(type_: TypeRef.T) -> str:
-        # warnings.warn("`TypeRef.root_type_name` will be deprecated! Use `TypeRef.T.name` instead", DeprecationWarning)
         return type_.name
 
     @staticmethod
     def is_non_null(type_: TypeRef.T) -> bool:
-        # warnings.warn("`TypeRef.is_non_null` will be deprecated! Use `TypeRef.T.is_non_null` instead", DeprecationWarning)
         return type_.is_non_null
 
     @staticmethod
     def is_list(type_: TypeRef.T) -> bool:
         return type_.is_list
 
     @staticmethod
@@ -126,15 +124,15 @@
 
 
 class TypeMeta:
     class T(BaseModel):
         """Base class of all GraphQL schema types."""
 
         name: str
-        description: str | None
+        description: str | None = ""
 
         @property
         def is_object(self) -> bool:
             return False
 
     class ArgumentMeta(T):
         """Class representing a field argument definition."""
@@ -160,15 +158,16 @@
                 return next(
                     self.arguments
                     | where(lambda argmeta: argmeta.name == argname)
                     | map(lambda arg: arg.type_)
                 )
             except StopIteration:
                 raise SchemaError(
-                    f"TypeMeta.FieldMeta.type_of_arg: no argument named {argname} for field {self.name}"
+                    f"TypeMeta.FieldMeta.type_of_arg: no argument named {argname}"
+                    f" for field {self.name}"
                 )
 
     class ScalarMeta(T):
         kind: Literal["SCALAR"] = "SCALAR"
         """ Class representing an scalar definition."""
 
     class ObjectMeta(T):
@@ -184,58 +183,62 @@
         def interfaces(self) -> list[str]:
             return list(self.interfaces_ | map(lambda intf: intf["name"]))
 
         @property
         def is_object(self) -> bool:
             return True
 
-        def field(self: TypeMeta.ObjectMeta, fname: str) -> TypeMeta.FieldMeta:
-            """Returns the field definition of object :attr:`self` with name :attr:`fname`, if any.
+        def field(self, fname: str) -> TypeMeta.FieldMeta:
+            """Returns the field definition of object :attr:`self` with name
+             :attr:`fname`, if any.
 
             Args:
-                self (TypeMeta.ObjectMeta): The object type
-                fname (str): The name of the desired field definition
+                fname: The name of the desired field definition
 
             Raises:
-                KeyError: If no field named :attr:`fname` is defined for object :attr:`self`.
+                KeyError: If no field named :attr:`fname` is defined for object
+                  :attr:`self`.
 
             Returns:
-                TypeMeta.FieldMeta: The field definition
+                The field definition
             """
 
             try:
                 return next(self.fields | where(lambda fmeta: fmeta.name == fname))
             except StopIteration:
                 raise KeyError(
-                    f"TypeMeta.ObjectMeta.field: no field named {fname} for interface {self.name}"
+                    f"TypeMeta.ObjectMeta.field: no field named {fname} for"
+                    f" interface {self.name}"
                 )
 
-        def type_of_field(self: TypeMeta.ObjectMeta, fname: str) -> TypeRef.T:
-            """Returns the type reference of the field of object :attr:`self` with name :attr:`fname`, if any.
+        def type_of_field(self, fname: str) -> TypeRef.T:
+            """Returns the type reference of the field of object :attr:`self`
+             with name :attr:`fname`, if any.
 
             Args:
-                self (TypeMeta.ObjectMeta): The object type
-                fname (str): The name of the desired field type
+                fname: The name of the desired field type
 
             Raises:
-                KeyError: If no field named :attr:`fname` is defined for object :attr:`self`.
+                KeyError: If no field named :attr:`fname` is defined for object
+                 :attr:`self`.
 
             Returns:
-                TypeRef.T: The field type reference
+                The field type reference
             """
 
             try:
                 return next(
                     self.fields
                     | where(lambda fmeta: fmeta.name == fname)
                     | map(lambda fmeta: fmeta.type_)
                 )
             except StopIteration:
                 raise KeyError(
-                    f"TypeMeta.ObjectMeta.type_of_field: no field named {fname} for object {self.name}"
+                    f"TypeMeta.ObjectMeta.type_of_field: no field named {fname}"
+                    f" for object {self.name}"
                 )
 
     class EnumValueMeta(T):
         """Class representing an enum value definition."""
 
         pass
 
@@ -251,73 +254,74 @@
         kind: Literal["INTERFACE"] = "INTERFACE"
         fields: list[TypeMeta.FieldMeta]
 
         @property
         def is_object(self) -> bool:
             return False
 
-        def field(self: TypeMeta.InterfaceMeta, fname: str) -> TypeMeta.FieldMeta:
-            """Returns the field definition of interface `self` with name `fname`, if any.
+        def field(self, fname: str) -> TypeMeta.FieldMeta:
+            """Returns the field definition of interface `self` with name `fname`,
+             if any.
 
             Args:
-                self (TypeMeta.InterfaceMeta): The interface type
-                fname (str): The name of the desired field definition
+                self: The interface type
+                fname: The name of the desired field definition
 
             Raises:
-                KeyError: If no field named :attr:`fname` is defined for interface :attr:`self`.
+                KeyError: If no field named :attr:`fname` is defined for interface
+                  :attr:`self`.
 
             Returns:
-                TypeMeta.FieldMeta: The field definition
+                The field definition
             """
 
             try:
                 return next(self.fields | where(lambda fmeta: fmeta.name == fname))
             except StopIteration:
                 raise KeyError(
-                    f"TypeMeta.InterfaceMeta.field: no field named {fname} for interface {self.name}"
+                    f"TypeMeta.InterfaceMeta.field: no field named {fname}"
+                    f" for interface {self.name}"
                 )
 
     class UnionMeta(T):
         """Class representing an union definition."""
 
         kind: Literal["UNION"] = "UNION"
         types: list[str] = Field(alias="possibleTypes")
 
     class InputObjectMeta(T):
         """Class representing an input object definition."""
 
         kind: Literal["INPUT_OBJECT"] = "INPUT_OBJECT"
         input_fields: list[TypeMeta.ArgumentMeta] = Field(alias="inputFields")
 
-        def type_of_input_field(
-            self: TypeMeta.InputObjectMeta, fname: str
-        ) -> TypeRef.T:
+        def type_of_input_field(self, fname: str) -> TypeRef.T:
             """Returns the type reference of the input field named `fname` in the
             input object `self`, if any.
 
             Args:
-                self (TypeMeta.InputObjectMeta): The input object
-                fname (str): The name of the input field
+                fname: The name of the input field
 
             Raises:
                 KeyError: If `fname` is not an input field of input object `self`
 
             Returns:
-                TypeRef.T: The type reference for input field `fname`
+                The type reference for input field `fname`
             """
 
             try:
                 return next(
                     self.input_fields
                     | where(lambda infield: infield.name == fname)
                     | map(lambda infield: infield.type_)
                 )
             except StopIteration:
                 raise KeyError(
-                    f"TypeMeta.InputObjectMeta.type_of_input_field: no input field named {fname} for input object {self.name}"
+                    f"TypeMeta.InputObjectMeta.type_of_input_field: no input field"
+                    f" named {fname} for input object {self.name}"
                 )
 
 
 TypeMeta_T = Annotated[
     TypeMeta.ScalarMeta | TypeMeta.ObjectMeta
     # | TypeMeta.EnumValueMeta
     | TypeMeta.EnumMeta
@@ -378,29 +382,29 @@
     @root_validator(allow_reuse=True)
     def type_map_generator(cls, values):
         if "types" in values and len(values["types"]) > 0:
             values["type_map"] = {type_.name: type_ for type_ in values["types"]}
 
         return values
 
-    def type_of_typeref(self: SchemaMeta, typeref: TypeRef.T) -> TypeMeta_T:
+    def type_of_typeref(self, typeref: TypeRef.T) -> TypeMeta_T:
         """Returns the type information of the type reference `typeref`
 
         Args:
-        self (SchemaMeta): The schema.
-        typeref (TypeRef.T): The type reference pointing to the type of interest.
+            typeref: The type reference pointing to the type of interest.
 
         Raises:
-        KeyError: If the type reference refers to a non-existant type
+            KeyError: If the type reference refers to a non-existant type
 
         Returns:
-        TypeMeta.T: _description_
+            Type information
         """
 
         tname = TypeRef.root_type_name(typeref)
+
         try:
             return self.type_map[tname]
         except KeyError:
             raise KeyError(
                 f"SchemaMeta.type_of_typeref: No type named {typeref.name} in schema!"
             )
```

### Comparing `subgrounds-1.6.0/subgrounds/subgraph/fieldpath.py` & `subgrounds-1.6.1/subgrounds/subgraph/fieldpath.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import logging
 import operator
 import warnings
 from dataclasses import dataclass
 from datetime import datetime
 from functools import partial, reduce
 from hashlib import blake2b
-from typing import TYPE_CHECKING, Any, Callable, ClassVar, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Callable, ClassVar
 
 from pipe import map, traverse
+from typing_extensions import Self  # 3.10 support
 
 from subgrounds.query import Query, Selection, arguments_of_field_args
 from subgrounds.schema import SchemaMeta, TypeMeta, TypeRef
 from subgrounds.subgraph.filter import Filter
 from subgrounds.utils import extract_data
 
 if TYPE_CHECKING:
@@ -213,19 +214,19 @@
 def fieldpaths_of_object(
     subgraph: Subgraph, object_: TypeMeta.ObjectMeta | TypeMeta.InterfaceMeta
 ):
     """Returns generator of FieldPath objects that selects all non-list fields of
     GraphQL Object of Interface :attr:`object_`.
 
     Args:
-      schema (SchemaMeta): _description_
-      object_ (TypeMeta.ObjectMeta | TypeMeta.InterfaceMeta): _description_
+      schema: _description_
+      object_: _description_
 
     Yields:
-      _type_: _description_
+      _description_
     """
     for fmeta in object_.fields:
         if not fmeta.type_.is_list and len(fmeta.arguments) == 0:
             match subgraph._schema.type_of_typeref(fmeta.type_):
                 case TypeMeta.ObjectMeta() | TypeMeta.InterfaceMeta():
                     yield subgraph.__getattribute__(object_.name).__getattribute__(
                         fmeta.name
@@ -238,25 +239,25 @@
 
 
 @dataclass
 class FieldPath(FieldOperatorMixin):
     _subgraph: Subgraph
     _root_type: TypeRef.T
     _type: TypeRef.T
-    _path: list[Tuple[Optional[dict[str, Any]], TypeMeta.FieldMeta]]
+    _path: list[tuple[dict[str, Any] | None, TypeMeta.FieldMeta]]
 
     # Purely for testing
     __test_mode: ClassVar[bool] = False
 
     def __init__(
         self,
         subgraph: Subgraph,
         root_type: TypeRef.T,
         type_: TypeRef.T,
-        path: list[Tuple[Optional[dict[str, Any]], TypeMeta.FieldMeta]],
+        path: list[tuple[dict[str, Any] | None, TypeMeta.FieldMeta]],
     ) -> None:
         self._subgraph = subgraph
         self._root_type = root_type
         self._type = type_
         self._path = path
 
         # Add fields as attributes if leaf is object
@@ -298,65 +299,64 @@
 
     @property
     def _root(self) -> TypeMeta.FieldMeta:
         """Returns the type information of the root field of the current
         :class:`FieldPath`
 
         Returns:
-          TypeMeta.FieldMeta: Type information of the root field of the current
-          :class:`FieldPath`
+          Type information of the root field of the current :class:`FieldPath`
         """
         return self._path[0][1]
 
     @property
     def _leaf(self) -> TypeMeta.FieldMeta:
         """Returns the type information of the leaf field of the current
         :class:`FieldPath`
 
         Returns:
-          TypeMeta.FieldMeta: Type information of the leaf field of the current
-          :class:`FieldPath`
+          Type information of the leaf field of the current :class:`FieldPath`
         """
         return self._path[-1][1]
 
     @staticmethod
     def _hash(msg: str) -> str:
         h = blake2b(digest_size=8)
         h.update(msg.encode("UTF-8"))
         return "x" + h.hexdigest()
 
     @staticmethod
     def _merge(fpaths: list[FieldPath]) -> list[Selection]:
         """Returns a Selection tree containing all selection paths in `fpaths`.
-        This function assumes that all fieldpaths in `fpaths` belong to the same subgraph
+        Note: Assumes that all fieldpaths in `fpaths` belong to the same subgraph
 
         Args:
-          fpaths (list[FieldPath]): _description_
+          fpaths: _description_
 
         Returns:
-          list[Selection]: _description_
+          _description_
         """
+
         query = reduce(Query.add, fpaths | map(FieldPath._selection), Query())
         return query.selection
 
     def _name_path(self, use_aliases: bool = False) -> list[str]:
         """Returns a list of strings correspoding to the names of all fields
         selected in the current :class:`FieldPath`. If :attr:`use_aliases` is True,
         then if a field has an automatically generated alias, the alias will be
         returned.
 
         Args:
-          use_aliases (bool, optional): Flag indicating wether of not to use the
-          fields' automatically generated alias (if present). Defaults to False.
+          use_aliases: Flag indicating wether of not to use the fields' automatically
+            generated alias (if present). Defaults to False.
 
         Returns:
-          list[str]: List of field names selected in the current :class:`FieldPath`
+          List of field names selected in the current :class:`FieldPath`
         """
 
-        def gen_alias(ele: Tuple[Optional[dict[str, Any]], TypeMeta.FieldMeta]) -> str:
+        def gen_alias(ele: tuple[dict[str, Any] | None, TypeMeta.FieldMeta]) -> str:
             if ele[0] != {} and ele[0] is not None:
                 return FieldPath._hash(ele[1].name + str(ele[0]))
             else:
                 return ele[1].name
 
         return list(
             self._path | map(lambda ele: gen_alias(ele) if use_aliases else ele[1].name)
@@ -364,56 +364,59 @@
 
     def _name(self, use_aliases: bool = False) -> str:
         """Generates the name of the current :class:`FieldPath` using the names of
         the fields it selects. If :attr:`use_aliases` is True, then if a field has
         an automatically generated alias, the alias will be used.
 
         Args:
-          use_aliases (bool, optional): Flag indicating wether of not to use the
-          fields' automatically generated alias (if present). Defaults to False.
+          use_aliases: Flag indicating wether of not to use the fields' automatically
+            generated alias (if present). Defaults to False.
 
         Returns:
-          str: The generated name of the current :class:`FieldPath`.
+          The generated name of the current :class:`FieldPath`.
         """
+
         return "_".join(self._name_path(use_aliases=use_aliases))
 
     def _auto_select(self) -> FieldPath | list[FieldPath]:
         match self._subgraph._schema.type_of_typeref(self._leaf.type_):
             case TypeMeta.ObjectMeta() | TypeMeta.InterfaceMeta() as obj:
                 return list(
                     fieldpaths_of_object(self._subgraph, obj)
                     | map(partial(FieldPath._extend, self))
                 )
 
             case _:
                 return self
 
-    def _extract_data(self, data: dict | list[dict]) -> list[Any] | Any:
+    def _extract_data(
+        self, data: dict[str, Any] | list[dict[str, Any]]
+    ) -> list[Any] | Any:
         """Extract the data corresponding to the current :class:`FieldPath` from
         the dictionary :attr:`data`.
 
         Args:
-          data (dict | list[dict]): Data dictionary that contains the data
-          corresponding to the current :class:`FieldPath`.
+          data: Data dictionary that contains the data corresponding to the current
+            :class:`FieldPath`.
 
         Returns:
-          list[Any] | Any: Data corresponding to the current :class:`FieldPath`.
+          Data corresponding to the current :class:`FieldPath`.
         """
         return extract_data(self._name_path(use_aliases=True), data)
 
     def _selection(self) -> Selection | list[Selection]:
         """Returns a selection or list of selections corresponding to the current
         :class:`FieldPath`.
 
         Returns:
           Selection | list[Selection]: _description_
         """
 
         def f(
-            path: list[Tuple[Optional[dict[str, Any]], TypeMeta.FieldMeta]]
+            path: list[tuple[dict[str, Any] | None, TypeMeta.FieldMeta]]
         ) -> list[Selection]:
             match path:
                 case [
                     (args, TypeMeta.FieldMeta() as fmeta),
                     *rest,
                 ] if args == {} or args is None:
                     return [Selection(fmeta, selection=f(rest))]
@@ -441,19 +444,19 @@
     def _set_arguments(
         self, args: dict[str, Any], selection: list[FieldPath] = []
     ) -> FieldPath | list[FieldPath]:
         """Set the arguments to the leaf of the current :class:`FieldPath`. The
         method returns the :attr:`self`.
 
         Args:
-          args (dict[str, Any]): _description_
-          selection (list[FieldPath], optional): _description_. Defaults to [].
+          args: _description_
+          selection: _description_. Defaults to [].
 
         Returns:
-          FieldPath: _description_
+          _description_
         """
 
         def fmt_arg(name, raw_arg):
             match (name, raw_arg):
                 case ("where", [Filter(), *_] as filters):
                     return Filter.to_dict(filters)
                 case ("orderBy", FieldPath() as fpath):
@@ -475,28 +478,32 @@
                     return self
             case _:
                 raise TypeError(f"Unexpected type for FieldPath {self}")
 
     def _select(self, name: str) -> FieldPath:
         """Returns a new FieldPath corresponding to the FieldPath `self` extended with
         an additional selection on the field named `name`.
+
         Args:
-          name (str): The name of the field to expand on the leaf of `fpath`
+          name: The name of the field to expand on the leaf of `fpath`
+
         Raises:
           TypeError: [description]
           TypeError: [description]
           TypeError: [description]
+
         Returns:
-          FieldPath: A new FieldPath containing `fpath` extended with the field named `name`
+          A new FieldPath containing `fpath` extended with the field named `name`
         """
         match self._schema.type_of_typeref(self._type):
             # If the FieldPath fpath
             case TypeMeta.EnumMeta() | TypeMeta.ScalarMeta():
                 raise TypeError(
-                    f"FieldPath: path {self} ends with a scalar field! cannot select field {name}"
+                    f"FieldPath: path {self} ends with a scalar field!"
+                    f" cannot select field {name}"
                 )
 
             case TypeMeta.ObjectMeta() | TypeMeta.InterfaceMeta() as obj:
                 field = obj.field(name)
 
                 match self._schema.type_of_typeref(field.type_):
                     case (
@@ -514,37 +521,39 @@
                             subgraph=self._subgraph,
                             root_type=self._root_type,
                             type_=field.type_,
                             path=path,
                         )
                     case _:
                         raise TypeError(
-                            f"FieldPath: field {name} is not a valid field for object {self._type.name} at path {self}"
+                            f"FieldPath: field {name} is not a valid field for object"
+                            f" {self._type.name} at path {self}"
                         )
 
             case _:
                 raise TypeError(
-                    f"FieldPath: Unexpected type {self._type.name} when selection {name} on {self}"
+                    f"FieldPath: Unexpected type {self._type.name}"
+                    f" when selection {name} on {self}"
                 )
 
     def _extend(self, ext: FieldPath) -> FieldPath:
         """Extends the current :class:`FieldPath` with the :class:`FieldPath`
         :attr:`ext`. :attr:`ext` must start where the current :class:`FieldPath` ends.
 
         Args:
-          ext (FieldPath): The :class:`FieldPath` representing the extension
+          ext: The :class:`FieldPath` representing the extension
 
         Raises:
           TypeError: [description]
           TypeError: [description]
           TypeError: [description]
 
         Returns:
-          FieldPath: A new :class:`FieldPath` containing the initial current
-          :class:`FieldPath` extended with :attr:`ext`
+          A new :class:`FieldPath` containing the initial current :class:`FieldPath`
+            extended with :attr:`ext`
         """
         match self._leaf:
             case TypeMeta.FieldMeta() as fmeta:
                 match self._schema.type_of_typeref(fmeta.type_):
                     case TypeMeta.ObjectMeta(name=name) | TypeMeta.InterfaceMeta(
                         name=name
                     ):
@@ -553,43 +562,47 @@
                                 subgraph=self._subgraph,
                                 root_type=self._root_type,
                                 type_=ext._type,
                                 path=self._path + ext._path,
                             )
                         else:
                             raise TypeError(
-                                f"extend: FieldPath {ext} does not start at the same type from where FieldPath {self} ends"
+                                f"extend: FieldPath {ext} does not start at the"
+                                f" same type from where FieldPath {self} ends"
                             )
                     case _:
                         raise TypeError(f"extend: FieldPath {self} is not object field")
             case _:
                 raise TypeError(f"extend: FieldPath {self} is not an object field")
 
     # ================================================================
     # Overloaded magic functions
     # ================================================================
     # When setting arguments
     def __call__(self, **kwargs: Any) -> Any:
         """Sets field arguments and expand subfields. The updated FieldPath is returned.
+
         Example:
-        >>> aaveV2 = sg.load_subgraph("https://api.thegraph.com/subgraphs/name/aave/protocol-v2")
+        >>> aaveV2 = sg.load_subgraph(
+        ...     "https://api.thegraph.com/subgraphs/name/aave/protocol-v2"
+        ... )
         >>> query = aaveV2.Query.borrows(
         ...   first=10,
         ...   order_by=aaveV2.Borrow.timestamp,
         ...   order_direction="desc",
         ...   selection=[
         ...     aaveV2.Borrow.id,
         ...     aaveV2.Borrow.timestamp,
         ...     aaveV2.Borrow.amount
         ...   ]
         ... )
+
         Returns:
-          FieldPath | list[FieldPath]: The updated field path if :attr:`selection`
-            is not specified, or a list of fieldpaths when :attr:`selection` is
-            specified.
+          The updated field path if :attr:`selection` is not specified, or a list of
+            fieldpaths when :attr:`selection` is specified.
         """
         selection = kwargs.pop("selection", [])
         return self._set_arguments(kwargs, selection)
 
     # Field selection
     def __getattribute__(self, __name: str) -> Any:
         # Small hack to get code completion to work while allowing updates to FieldPath
@@ -631,15 +644,16 @@
         return Filter.mk_filter(self, Filter.Operator.GTE, value)
 
     # Utility
     def __str__(self) -> str:
         return ".".join(self._path | map(lambda ele: ele[1].name))
 
     def __repr__(self) -> str:
-        return f"FieldPath({self._subgraph._url}, {self._root_type.name}, {self._name_path()})"
+        vars = f"{self._subgraph._url}, {self._root_type.name}, {self._name_path()}"
+        return f"FieldPath({vars})"
 
 
 @dataclass
 class SyntheticField(FieldOperatorMixin):
     STRING: ClassVar[TypeRef.Named] = TypeRef.Named(name="String", kind="SCALAR")
     INT: ClassVar[TypeRef.Named] = TypeRef.Named(name="Int", kind="SCALAR")
     FLOAT: ClassVar[TypeRef.Named] = TypeRef.Named(name="Float", kind="SCALAR")
@@ -660,29 +674,30 @@
         default: Any = None,
     ) -> None:
         deps = list([deps] | traverse)
 
         def mk_deps(
             deps: list[FieldPath | SyntheticField],
             f: Callable,
-            acc: list[Tuple[Optional[Callable], int]] = [],
-        ) -> Tuple[Callable, list[FieldPath]]:
-            """If all dependencies are field paths, then this function does nothing. If the dependencies contain
-            one or more other synthetic fields, as is the case when chaining binary operators, then the synthetic
-            field tree is flattened to a single synthetic field containing all leaf dependencies.
+            acc: list[tuple[Callable | None, int]] = [],
+        ) -> tuple[Callable, list[FieldPath]]:
+            """If all dependencies are field paths, then this function does nothing.
+             If the dependencies contain one or more other synthetic fields, as is the
+             case when chaining binary operators, then the synthetic field tree is
+             flattened to a single synthetic field containing all leaf dependencies.
 
             Args:
-              deps (list): Initial dependencies for synthetic field
-              f (Callable): Function to apply to the values of those dependencies
-              acc (list[Tuple[Optional[Callable], list[FieldPath]]], optional): Accumulator. Defaults to [].
+              deps: Initial dependencies for synthetic field
+              f: Function to apply to the values of those dependencies
+              acc: Accumulator. Defaults to [].
 
             Returns:
-              Tuple[Callable, list[FieldPath]]: A tuple containing the potentially modified
-              function and dependency list.
+              A tuple containing the potentially modified function and dependency list.
             """
+
             match deps:
                 case []:
 
                     def new_f(*args):
                         new_args = []
                         _counter = 0
                         for f_, deps in acc:
@@ -750,24 +765,24 @@
             case "Float":
                 return 0.0
             case "Boolean":
                 return False
             case _:
                 return 0
 
-    @staticmethod
-    def constant(value: str | int | float | bool) -> SyntheticField:
+    @classmethod
+    def constant(cls, value: str | int | float | bool) -> SyntheticField:
         """Returns a constant ``SyntheticField`` with value ``value``.
         Useful for injecting additional static data to a schema or merging entities.
 
         Args:
-          value (str | int | float | bool): The constant field's value
+          value: The constant field's value
 
         Returns:
-          SyntheticField: The constant ``SyntheticField``
+          The constant ``SyntheticField``
 
         Example:
 
         .. code-block:: python
 
             >>> from subgrounds.subgrounds import Subgrounds
             >>> from subgrounds.subgraph import SyntheticField
@@ -791,87 +806,92 @@
             ...     orderBy=univ3.Burn.timestamp,
             ...     orderDirection='desc'
             ... )
 
             # Query mints and burns. Notice that we merge the two entity tables by
             # setting `concat=True` and overwriting the column names (columns must
             # match the `FieldPaths`)
-            >>> df = sg.query_df([
-            ...     mints.transaction.id,
-            ...     mints.timestamp,
-            ...     mints.tx_type,
-            ...     mints.origin,
-            ...     mints.amountUSD,
-            ...     burns.transaction.id,
-            ...     burns.timestamp,
-            ...     burns.tx_type,
-            ...     burns.origin,
-            ...     burns.amountUSD,
-            ... ], columns=['tx_hash', 'timestamp', 'tx_type', 'origin', 'amount_USD'], concat=True)
+            >>> df = sg.query_df(
+            ...     [
+            ...         mints.transaction.id,
+            ...         mints.timestamp,
+            ...         mints.tx_type,
+            ...         mints.origin,
+            ...         mints.amountUSD,
+            ...         burns.transaction.id,
+            ...         burns.timestamp,
+            ...         burns.tx_type,
+            ...         burns.origin,
+            ...         burns.amountUSD,
+            ...     ],
+            ...     columns=['tx_hash', 'timestamp', 'tx_type', 'origin', 'amount_USD'],
+            ...     concat=True
+            ..  )
 
-            # Sort the DataFrame
+            # Sort the DataFrame (output is truncated)
             >>> df.sort_values(by=['timestamp'], ascending=False)
-                                                          tx_hash   timestamp tx_type                                      origin    amount_USD
-            0   0xcbe1bacacc1e64fe613ae5eef2063563bd0057d1e3df...  1656016553    MINT  0x3435e7946d40b1a83c0cf154326fc6b3ca908952  7.879784e+03
-            1   0xdddaaddf59e5a3abff4feadef83b3ceb023a74424ea7...  1656016284    MINT  0xc747962e7e416e2a582813b1d7ad59eb83077fa6  5.110840e+04
-            10  0xa7671452c34a3b083083ef81e364489c2c9ee801a3b8...  1656016284    BURN  0xd40db77990bbb30514276b5ac17c3ce5cc9c951f  2.804573e+05
-            2   0xc132e73975e77c2c2c91fcf332018dfb01aac0ca9471...  1656015853    MINT  0xc747962e7e416e2a582813b1d7ad59eb83077fa6  5.122569e+04
-            3   0x1444744f4021a2046787c1b7b88cd9ac21f071c65acc...  1656015773    MINT  0xd11aa2e3a000275ed12b87515c9ac0d67b32e7b9  8.897983e+03
-            4   0x3315617d426fc2b0db5d8dbccd549efaa8f1ae2969ca...  1656015693    MINT  0xb7dd4d134b1794ee848e1af1a62b85d7b2ea9301  0.000000e+00
-            11  0xcc713daa2dc58cd1f2218c8f438e7fcf04d2e9c7c83d...  1656015278    BURN  0xa7c43e2057d89b6946b8865efc8bee3a4ea7d28d  1.254942e+06
-            5   0x7bbfae86f0c3c983651bd0671557cd851fc301317c06...  1656015111    MINT  0xac56cee8ccd00d0c1d72ce3415140874552e80f4  3.432075e+04
-            12  0xea21c3a68a8f0c6a2721a3072e0c8b2edc77f4d2f0d9...  1656014785    BURN  0x0709b103d46d71458a71e5d81230dd688809a53d  2.059106e+04
-            6   0x3bd369bf45c55cab40c62db81bb3e0684fd85fe2b662...  1656014120    MINT  0x509984bfc0fb24e2d1377cfec224d3afec4c341e  2.517578e+03
-            13  0x1ea59da77c442479af8fb51501a931260d473e249de7...  1656014018    BURN  0x509984bfc0fb24e2d1377cfec224d3afec4c341e  0.000000e+00
-            7   0xb9d31ef78b8bf786b422d948dd1fba246710078abff8...  1656013998    MINT  0x22dfec183294d257f80c15d3c9cd47495bdc728c  8.365750e+04
-            14  0xc5e3ec84a2860e3c3a055ccdced435a67b4aff4dd3be...  1656013946    BURN  0xac56cee8ccd00d0c1d72ce3415140874552e80f4  3.363809e+04
-            8   0x7c736255d9a4ebf4781069a1b2a929ad89100f1af980...  1656013913    MINT  0x4ce6aea89f059915ae5efbf34a2a8adc544ae09e  4.837287e+04
-            15  0x95cf56b9eb69aa45048a9b7b3e472df5bc3bfad591cd...  1656013728    BURN  0x4ce6aea89f059915ae5efbf34a2a8adc544ae09e  5.110010e+04
-            9   0x76dd2bbf43485c224471dd823c2992178f031f27194b...  1656013599    MINT  0x234a644868c419ce0dcdd9fd539762eba47f3759  5.363896e+03
-            16  0x47e595b02fdcb51ff42a5008e53be7ee3bdf8063b580...  1656013580    BURN  0xaf0fdd39e5d92499b0ed9f68693da99c0ec1e92e  0.000000e+00
-            17  0xe20ec9702f455d74b3cc1f54fe2f3450604ca5037a72...  1656013455    BURN  0xaf0fdd39e5d92499b0ed9f68693da99c0ec1e92e  0.000000e+00
-            18  0xac3e95666be3a45fdfbbfa513a114136ea6ecffb9de2...  1656013237    BURN  0x665d2d2444f2384fb3d96aaa0ea3536b92984dce  2.254100e+05
-            19  0x01c3424a48c36104ea388482723347f15c0bc1bb1a80...  1656013034    BURN  0x0084ee6c8893c01e252198b56ec127443dc27464  0.000000e+00
-
+             tx_hash   timestamp    tx_type  origin     amount_USD
+            0xcbe1...  1656016553    MINT  0x3435....  7.879784e+03
+            0xddda...  1656016284    MINT  0xc747....  5.110840e+04
+            0xa767...  1656016284    BURN  0xd40d....  2.804573e+05
+            0xc132...  1656015853    MINT  0xc747....  5.122569e+04
+            0x1444...  1656015773    MINT  0xd11a....  8.897983e+03
+            0x3315...  1656015693    MINT  0xb7dd....  0.000000e+00
+            0xcc71...  1656015278    BURN  0xa7c4....  1.254942e+06
+            0x7bbf...  1656015111    MINT  0xac56....  3.432075e+04
+            0xea21...  1656014785    BURN  0x0709....  2.059106e+04
+            0x3bd3...  1656014120    MINT  0x5099....  2.517578e+03
+            0x1ea5...  1656014018    BURN  0x5099....  0.000000e+00
+            0xb9d3...  1656013998    MINT  0x22df....  8.365750e+04
+            0xc5e3...  1656013946    BURN  0xac56....  3.363809e+04
+            0x7c73...  1656013913    MINT  0x4ce6....  4.837287e+04
+            0x95cf...  1656013728    BURN  0x4ce6....  5.110010e+04
+            0x76dd...  1656013599    MINT  0x234a....  5.363896e+03
+            0x47e5...  1656013580    BURN  0xaf0f....  0.000000e+00
+            0xe20e...  1656013455    BURN  0xaf0f....  0.000000e+00
+            0xac3e...  1656013237    BURN  0x665d....  2.254100e+05
+            0x01c3...  1656013034    BURN  0x0084....  0.000000e+00
         """
+
         match value:
             case str():
-                return SyntheticField(lambda: value, SyntheticField.STRING, [])
+                return cls(lambda: value, cls.STRING, [])
             case int():
-                return SyntheticField(lambda: value, SyntheticField.INT, [])
+                return cls(lambda: value, cls.INT, [])
             case float():
-                return SyntheticField(lambda: value, SyntheticField.FLOAT, [])
+                return cls(lambda: value, cls.FLOAT, [])
             case bool():
-                return SyntheticField(lambda: value, SyntheticField.BOOL, [])
+                return cls(lambda: value, cls.BOOL, [])
 
-    @staticmethod
-    def datetime_of_timestamp(timestamp: FieldPath | SyntheticField) -> SyntheticField:
-        """Returns a ``SyntheticField`` that will transform the ``FieldPath`` ``timestamp``
-        into a human-readable ISO8601 string.
+    @classmethod
+    def datetime_of_timestamp(cls, timestamp: FieldPath | SyntheticField) -> Self:
+        """Returns a ``SyntheticField`` that will transform the ``FieldPath``
+        ``timestamp`` into a human-readable ISO8601 string.
 
         Args:
-          timestamp (FieldPath | SyntheticField): A ``FieldPath`` representing a
-              Unix timestamp field.
+          timestamp: A ``FieldPath`` representing a Unix timestamp field.
 
         Returns:
-          SyntheticField: An ISO8601 datetime string ``SyntheticField``.
+          An ISO8601 datetime string ``SyntheticField``.
 
         Example:
 
         .. code-block:: python
 
             >>> from subgrounds.subgrounds import Subgrounds
             >>> from subgrounds.subgraph import SyntheticField
             >>> sg = Subgrounds()
             >>> univ3 = sg.load_subgraph(
             ...     'https://api.thegraph.com/subgraphs/name/uniswap/uniswap-v3'
             ... )
 
             # Create datetime SyntheticField
-            >>> univ3.Swap.datetime = SyntheticField.datetime_of_timestamp(univ3.Swap.timestamp)
+            >>> univ3.Swap.datetime = SyntheticField.datetime_of_timestamp(
+            ...     univ3.Swap.timestamp
+            ... )
 
             # Query 100 swaps
             >>> sg.query_df([
             ...     univ3.Query.swaps.timestamp,
             ...     univ3.Query.swaps.datetime,
             ... ])
                 swaps_timestamp       swaps_datetime
@@ -883,42 +903,42 @@
             ..              ...                  ...
             95       1646128326  2022-03-01 04:52:06
             96       1646128326  2022-03-01 04:52:06
             97       1626416555  2021-07-16 02:22:35
             98       1626416555  2021-07-16 02:22:35
             99       1625837291  2021-07-09 09:28:11
         """
+
         return SyntheticField(
             lambda timestamp: str(datetime.fromtimestamp(timestamp)),
             SyntheticField.STRING,
             timestamp,
         )
 
-    @staticmethod
+    @classmethod
     def map(
+        cls,
         dict: dict[Any, Any],
         type_: TypeRef.T,
         fpath: FieldPath | SyntheticField,
-        default: Optional[Any] = None,
-    ) -> SyntheticField:
+        default: Any | None = None,
+    ) -> Self:
         """Returns a SyntheticField that will map the values of ``fpath`` using the
         key value pairs in ``dict``. If a value is not in the dictionary, then
         ``default`` will be used instead.
 
         Args:
-          dict (dict[Any, Any]): The dictionary containing the key value pairs used
-              to map ``fpath``'s values
-          type_ (TypeRef.T): The type of the resulting field
-          fpath (FieldPath | SyntheticField): The FieldPath whose values will be
-              mapped using the dictionary
-          default (Optional[Any]): Default value used when a value is not in the
-              provided dictionary
+          dict: The dictionary containing the key value pairs used to map
+            ``fpath``'s values
+          type_: The type of the resulting field
+          fpath: The FieldPath whose values will be mapped using the dictionary
+          default: Default value used when a value is not in the provided dictionary
 
         Returns:
-            SyntheticField: A map SyntheticField
+            A map SyntheticField
 
         Example:
 
         .. code-block:: python
 
             >>> from subgrounds.subgrounds import Subgrounds
             >>> from subgrounds.subgraph import SyntheticField
@@ -964,10 +984,11 @@
             6  0xcbcdf9626bc03e24f779434178a73a0b4bad62ed       UNKNOWN
             7  0xc63b0708e2f7e69cb8a1df0e1389a98c35a76d52       UNKNOWN
             8  0x4585fe77225b41b697c938b018e2ac67ac5a20c0       UNKNOWN
             9  0x4e68ccd3e89f51c3074ca5072bbac773960dfa36       UNKNOWN
 
 
         """
+
         return SyntheticField(
             lambda value: dict[value] if value in dict else default, type_, fpath
         )
```

### Comparing `subgrounds-1.6.0/subgrounds/subgraph/filter.py` & `subgrounds-1.6.1/subgrounds/subgraph/filter.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.6.0/subgrounds/subgraph/object.py` & `subgrounds-1.6.1/subgrounds/subgraph/object.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,21 +32,21 @@
         return self._subgraph._schema
 
     def _select(self, name: str) -> FieldPath:
         """Selects the field from ``self`` with name ``name`` and returns the field
         as a :class:`FieldPath`.
 
         Args:
-          name (str): The name of the field
+          name: The name of the field
 
         Raises:
           TypeError: _description_
 
         Returns:
-          FieldPath: _description_
+          _description_
         """
 
         field = self._object.field(name)
 
         match self._schema.type_of_typeref(field.type_):
             case (
                 TypeMeta.ObjectMeta()
@@ -59,45 +59,50 @@
                     TypeRef.Named(name=self._object.name, kind="OBJECT"),
                     field.type_,
                     [(None, field)],
                 )
 
             case TypeMeta.T as type_:
                 raise TypeError(
-                    f"Object: Unexpected type {type_.name} when selection {name} on {self}"
+                    f"Object: Unexpected type {type_.name}"
+                    f" when selection {name} on {self}"
                 )
 
         assert False  # Suppress mypy missing return statement warning
 
     def _add_field(self, name: str, fpath: FieldPath) -> None:
         sfield = SyntheticField(identity, fpath._type, fpath)
         self._subgraph._add_synthetic_field(self._object, name, sfield)
 
     def _add_sfield(self, name: str, sfield: SyntheticField) -> None:
         # TODO: Add check to make sure obj has the deps of sfield
         # obj_fields = [field.name for field in obj.object_.fields]
         # sfield_deps = [fpath.leaf.name for fpath in sfield.deps]
         # for dep in sfield_deps:
         #   if dep not in obj_fields:
-        #     raise Exception(f'SyntheticField {obj.object_.name}.{name}: {obj.object_.name} does not have the field {dep}')
+        #     raise Exception(
+        #       f'SyntheticField {obj.object_.name}.{name}: {obj.object_.name}'
+        #        ' does not have the field {dep}'
+        #     )
 
         def f(
             obj_: TypeMeta.ObjectMeta | TypeMeta.InterfaceMeta, path: list[str]
         ) -> None:
             match path:
                 case [field_name, *rest]:
                     try:
                         field: TypeMeta.FieldMeta = next(
                             obj_.fields | where(lambda field: field.name == field_name)
                         )
 
                         f(self._schema.type_map[field.type_.name], rest)
                     except StopIteration:
                         raise Exception(
-                            f"SyntheticField {self._object.name}.{name}: {obj_.name} does not have the field {field_name}"
+                            f"SyntheticField {self._object.name}.{name}: {obj_.name}"
+                            f" does not have the field {field_name}"
                         )
                 case []:
                     return
 
         for fpath in sfield._deps:
             f(self._object, fpath._name_path())
```

### Comparing `subgrounds-1.6.0/subgrounds/subgraph/subgraph.py` & `subgrounds-1.6.1/subgrounds/subgraph/subgraph.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.6.0/subgrounds/subgrounds.py` & `subgrounds-1.6.1/subgrounds/subgrounds.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,36 +7,34 @@
 import functools
 import json
 import logging
 import warnings
 from dataclasses import dataclass, field
 from functools import reduce
 from pathlib import Path
-from typing import Any, Iterator, Optional, Type
+from typing import Any, Iterator, Type, cast
 
 import pandas as pd
-from pipe import groupby, map, traverse, where
+from pipe import groupby, map, traverse
 
 import subgrounds.client as client
-from subgrounds.dataframe_utils import df_of_json
-from subgrounds.errors import SubgroundsError
-from subgrounds.pagination import paginate, paginate_iter
-from subgrounds.pagination.pagination import PaginationStrategy
-from subgrounds.pagination.strategies import LegacyStrategy
-from subgrounds.query import DataRequest, Document, Query
-from subgrounds.schema import SchemaMeta
-from subgrounds.subgraph.fieldpath import FieldPath
-from subgrounds.subgraph.subgraph import Subgraph
-from subgrounds.transform import (
+
+from .dataframe_utils import df_of_json
+from .errors import SubgroundsError
+from .pagination import LegacyStrategy, PaginationStrategy, normalize_strategy, paginate
+from .query import DataRequest, DataResponse, Document, DocumentResponse, Query
+from .schema import SchemaMeta
+from .subgraph import FieldPath, Subgraph
+from .transform import (
     DEFAULT_GLOBAL_TRANSFORMS,
     DEFAULT_SUBGRAPH_TRANSFORMS,
-    DocumentTransform,
     RequestTransform,
+    apply_transforms,
 )
-from subgrounds.utils import PLAYGROUNDS_APP_URL
+from .utils import PLAYGROUNDS_APP_URL
 
 logger = logging.getLogger("subgrounds")
 warnings.simplefilter("default")
 
 
 def store_schema(schema: dict[str, Any], path: Path):
     with path.open("w") as f:
@@ -124,38 +122,38 @@
 
         return self.load(url, save_schema, cache_dir, True)
 
     def load_api(
         self, url: str, save_schema: bool = False, cache_dir: str = "schemas/"
     ) -> Subgraph:
         """Performs introspection on the provided GraphQL API ``url`` to get the
-        schema, stores the schema if ``save_schema`` is ``True`` and returns a
-        generated class representing the GraphQL endpoint with all its entities.
+         schema, stores the schema if ``save_schema`` is ``True`` and returns a
+         generated class representing the GraphQL endpoint with all its entities.
 
         Args:
-          url (str): The url of the API
-          save_schema (bool, optional): Flag indicating whether or not the schema
-            should be saved to disk. Defaults to False.
+          url: The url of the API
+          save_schema: Flag indicating whether or not the schema should be saved
+           to disk. Defaults to False.
 
         Returns:
-          Subgraph: A generated class representing the subgraph and its entities
+          A generated class representing the subgraph and its entities
         """
 
         return self.load(url, save_schema, cache_dir, False)
 
     def mk_request(self, fpaths: FieldPath | list[FieldPath]) -> DataRequest:
         """Creates a :class:`DataRequest` object by combining one or more
         :class:`FieldPath` objects.
 
         Args:
-          fpaths (FieldPath | list[FieldPath]): One or more :class:`FieldPath`
-            objects that should be included in the request
+          fpaths: One or more :class:`FieldPath` objects that should be included
+           in the request
 
         Returns:
-          DataRequest: A new :class:`DataRequest` object
+          Brand new request
         """
 
         fpaths = list([fpaths] | traverse | map(FieldPath._auto_select) | traverse)
 
         return DataRequest(
             documents=list(
                 fpaths
@@ -170,195 +168,155 @@
                 )
             )
         )
 
     def execute(
         self,
         req: DataRequest,
-        pagination_strategy: Optional[Type[PaginationStrategy]] = LegacyStrategy,
-    ) -> list[dict]:
-        """Executes a :class:`DataRequest` object, sending the underlying
-        query(ies) to the server and returning a data blob (list of Python
-        dictionaries, one per actual query).
+        pagination_strategy: Type[PaginationStrategy] | None = LegacyStrategy,
+    ) -> DataResponse:
+        """Same as `execute`, except that an iterator is returned which will iterate
+        the data pages.
 
         Args:
-            req (DataRequest): The :class:`DataRequest` object to be executed
-            pagination_strategy (Optional[Type[PaginationStrategy]], optional): A Class
-              implementing the :class:`PaginationStrategy` ``Protocol``. If ``None``, then
-              automatic pagination is disabled. Defaults to :class:`LegacyStrategy`.
+          req: The :class:`DataRequest` object to be executed
+          pagination_strategy: A Class implementing the :class:`PaginationStrategy`
+            ``Protocol``. If ``None``, then automatic pagination is disabled.
+            Defaults to :class:`LegacyStrategy`.
 
         Returns:
-            list[dict]: The reponse data
+          A :class:`DataResponse` object representing the response
         """
 
-        def execute_document(doc: Document) -> dict:
-            subgraph: Subgraph = next(
-                self.subgraphs.values() | where(lambda sg: sg._url == doc.url)
-            )
-            if pagination_strategy is not None and subgraph._is_subgraph:
-                return paginate(
-                    subgraph._schema,
-                    doc,
-                    pagination_strategy=pagination_strategy,
-                    headers=self.headers,
-                )
-            else:
-                return client.query(
-                    doc.url, doc.graphql, variables=doc.variables, headers=self.headers
-                )
+        document_transforms = {
+            url: subgraph._transforms for url, subgraph in self.subgraphs.items()
+        }
+        transformer = apply_transforms(self.global_transforms, document_transforms, req)
+        strategy = normalize_strategy(pagination_strategy)
 
-        def transform_doc(transforms: list[DocumentTransform], doc: Document) -> dict:
-            logger.debug(f"execute.transform_doc: doc = \n{doc.graphql}")
-            match transforms:
-                case []:
-                    return execute_document(doc)
-                case [transform, *rest]:
-                    new_doc = transform.transform_document(doc)
-                    data = transform_doc(rest, new_doc)
-                    return transform.transform_response(doc, data)
-
-            assert False  # Suppress mypy missing return statement warning
-
-        def transform_req(
-            transforms: list[RequestTransform], req: DataRequest
-        ) -> list[dict]:
-            match transforms:
-                case []:
-                    return list(
-                        req.documents
-                        | map(
-                            lambda doc: transform_doc(
-                                self.subgraphs[doc.url]._transforms, doc
-                            )
-                        )
-                    )
-                case [transform, *rest]:
-                    new_req = transform.transform_request(req)
-                    data = transform_req(rest, new_req)
-                    return transform.transform_response(req, data)
+        data_resp = DataResponse(responses=[])
+        data_req = cast(DataRequest, next(transformer))
+
+        for doc in data_req.documents:
+            paginator = paginate(self.subgraphs[doc.url]._schema, doc, strategy)
+            paginated_doc = next(paginator)
+            doc_resp = DocumentResponse(url=doc.url, data={})
+
+            while True:
+                resp = client.query(paginated_doc, headers=self.headers)
+                doc_resp = doc_resp.combine(resp)
 
-            assert False  # Suppress mypy missing return statement warning
+                try:
+                    paginated_doc = paginator.send(resp)
+                except StopIteration:
+                    break
 
-        return transform_req(self.global_transforms, req)
+            data_resp = data_resp.add_responses(doc_resp)
+
+        next(transformer)  # toss empty None
+        return cast(DataResponse, transformer.send(data_resp))
 
     def execute_iter(
         self,
         req: DataRequest,
-        pagination_strategy: Optional[Type[PaginationStrategy]] = LegacyStrategy,
-    ) -> Iterator[dict[str, Any]]:
+        pagination_strategy: Type[PaginationStrategy] | None = LegacyStrategy,
+    ) -> Iterator[DocumentResponse]:
         """Same as `execute`, except that an iterator is returned which will iterate
         the data pages.
 
         Args:
-          req (DataRequest): The :class:`DataRequest` object to be executed
-          pagination_strategy (Optional[Type[PaginationStrategy]], optional): A Class
-            implementing the :class:`PaginationStrategy` ``Protocol``. If ``None``, then
-            automatic pagination is disabled. Defaults to :class:`LegacyStrategy`.
-
-        Returns:
-          Iterator[dict]: An iterator over the reponse data pages
-        """
-
-        def execute_document(doc: Document) -> Iterator[dict[str, Any]]:
-            subgraph: Subgraph = next(
-                self.subgraphs.values() | where(lambda sg: sg._url == doc.url)
-            )
-            if pagination_strategy is not None and subgraph._is_subgraph:
-                yield from paginate_iter(
-                    subgraph._schema,
-                    doc,
-                    pagination_strategy=pagination_strategy,
-                    headers=self.headers,
+          req: The :class:`DataRequest` object to be executed
+          pagination_strategy: A Class implementing the :class:`PaginationStrategy`
+           ``Protocol``. If ``None``, then automatic pagination is disabled.
+           Defaults to :class:`LegacyStrategy`.
+
+        Returns:
+          An iterator over the :class:`DocumentResponse` pages.
+
+        ⚠️ DOES NOT apply global transforms across multiple documents or their pages.
+         Since we yield each page as we get it, it's not possible to accurately perform
+         the transforms since we don't collect the pages. This means transforms
+         expecting multiple documents or pages of documents will be inaccurate.
+        """
+
+        document_transforms = {
+            url: subgraph._transforms for url, subgraph in self.subgraphs.items()
+        }
+        transformer = apply_transforms(self.global_transforms, document_transforms, req)
+        strategy = normalize_strategy(pagination_strategy)
+
+        data_req = cast(DataRequest, next(transformer))
+        for doc in data_req.documents:
+            paginator = paginate(self.subgraphs[doc.url]._schema, doc, strategy)
+            paginated_doc = next(paginator)
+            while True:
+                resp = client.query(paginated_doc, headers=self.headers)
+
+                next(transformer)  # toss empty None
+                data_resp = cast(
+                    DataResponse, transformer.send(DataResponse(responses=[resp]))
                 )
-            else:
-                yield client.query(
-                    doc.url,
-                    doc.graphql,
-                    variables=doc.variables,
-                    headers=self.headers,
-                )
-
-        def transform_doc(
-            transforms: list[DocumentTransform], doc: Document
-        ) -> Iterator[dict[str, Any]]:
-            logger.debug(f"execute_iter.transform_doc: doc = \n{doc.graphql}")
-            match transforms:
-                case []:
-                    yield from execute_document(doc)
-                case [transform, *rest]:
-                    new_doc = transform.transform_document(doc)
-                    for data in transform_doc(rest, new_doc):
-                        yield transform.transform_response(doc, data)
-
-        def transform_req(
-            transforms: list[RequestTransform], req: DataRequest
-        ) -> Iterator[dict[str, Any]]:
-            match transforms:
-                case []:
-                    for doc in req.documents:
-                        yield from transform_doc(
-                            self.subgraphs[doc.url]._transforms, doc
-                        )
-                case [transform, *rest]:
-                    new_req = transform.transform_request(req)
-                    for data in transform_req(rest, new_req):
-                        yield transform.transform_response(req, data)
+                yield from data_resp.responses  # should only be one
 
-        yield from transform_req(self.global_transforms, req)
+                try:
+                    paginated_doc = paginator.send(resp)
+                except StopIteration:
+                    break
 
     def query_json(
         self,
         fpaths: FieldPath | list[FieldPath],
-        pagination_strategy: Optional[Type[PaginationStrategy]] = LegacyStrategy,
+        pagination_strategy: Type[PaginationStrategy] | None = LegacyStrategy,
     ) -> list[dict[str, Any]]:
-        """Equivalent to ``Subgrounds.execute(Subgrounds.mk_request(fpaths), pagination_strategy)``.
+        """Equivalent to
+         ``Subgrounds.execute(Subgrounds.mk_request(fpaths), pagination_strategy)``.
 
         Args:
-          fpaths (FieldPath | list[FieldPath]): One or more :class:`FieldPath` objects that should be
-            included in the request.
-          pagination_strategy (Optional[Type[PaginationStrategy]], optional): A Class
-            implementing the :class:`PaginationStrategy` ``Protocol``. If ``None``, then
-            automatic pagination is disabled. Defaults to :class:`LegacyStrategy`.
+          fpaths: One or more :class:`FieldPath` objects
+            that should be included in the request.
+          pagination_strategy: A Class implementing the :class:`PaginationStrategy`
+            ``Protocol``. If ``None``, then automatic pagination is disabled.
+            Defaults to :class:`LegacyStrategy`.
 
         Returns:
-          list[dict[str, Any]]: The reponse data
+          The reponse data
         """
 
         fpaths = list([fpaths] | traverse | map(FieldPath._auto_select) | traverse)
         req = self.mk_request(fpaths)
-        return self.execute(req, pagination_strategy=pagination_strategy)
+        return [doc.data for doc in self.execute(req, pagination_strategy).responses]
 
     def query_json_iter(
         self,
         fpaths: FieldPath | list[FieldPath],
-        pagination_strategy: Optional[Type[PaginationStrategy]] = LegacyStrategy,
+        pagination_strategy: Type[PaginationStrategy] | None = LegacyStrategy,
     ) -> Iterator[dict[str, Any]]:
-        """Same as `query_json` except an iterator over the response data pages is returned.
+        """Same as `query_json` returns an iterator over the response data pages.
 
         Args:
-          fpaths (FieldPath | list[FieldPath]): One or more :class:`FieldPath` objects
-            that should be included in the request.
-          pagination_strategy (Optional[Type[PaginationStrategy]], optional): A Class
-            implementing the :class:`PaginationStrategy` ``Protocol``. If ``None``, then
-            automatic pagination is disabled. Defaults to :class:`LegacyStrategy`.
+          fpaths: One or more :class:`FieldPath` objects that should be included
+            in the request.
+          pagination_strategy: A Class implementing the :class:`PaginationStrategy`
+            ``Protocol``. If ``None``, then automatic pagination is disabled.
+            Defaults to :class:`LegacyStrategy`.
 
         Returns:
           list[dict[str, Any]]: The reponse data
         """
 
         fpaths = list([fpaths] | traverse | map(FieldPath._auto_select) | traverse)
         req = self.mk_request(fpaths)
-        yield from self.execute_iter(req, pagination_strategy=pagination_strategy)
+        yield from (resp.data for resp in self.execute_iter(req, pagination_strategy))
 
     def query_df(
         self,
         fpaths: FieldPath | list[FieldPath],
-        columns: Optional[list[str]] = None,
+        columns: list[str] | None = None,
         concat: bool = False,
-        pagination_strategy: Optional[Type[PaginationStrategy]] = LegacyStrategy,
+        pagination_strategy: Type[PaginationStrategy] | None = LegacyStrategy,
     ) -> pd.DataFrame | list[pd.DataFrame]:
         """Same as :func:`Subgrounds.query` but formats the response data into a
         Pandas DataFrame. If the response data cannot be flattened to a single query
         (e.g.: when querying multiple list fields that return different entities),
         then multiple dataframes are returned
 
         ``fpaths`` is a list of :class:`FieldPath` objects that indicate which
@@ -370,32 +328,32 @@
 
         ``concat`` indicates whether or not the resulting dataframes should be
         concatenated together. The dataframes must have the same number of columns,
         as well as the same column names and types (the names can be set using the
         ``columns`` argument).
 
         Args:
-          fpaths (FieldPath | list[FieldPath]): One or more `FieldPath` objects that
-            should be included in the request.
-          columns (Optional[list[str]], optional): The column labels. Defaults to None.
-          merge (bool, optional): Whether or not to merge resulting dataframes.
-          pagination_strategy (Optional[Type[PaginationStrategy]], optional): A Class
-            implementing the :class:`PaginationStrategy` ``Protocol``. If ``None``, then
-            automatic pagination is disabled. Defaults to :class:`LegacyStrategy`.
+          fpaths: One or more `FieldPath` objects that should be included in the request
+          columns: The column labels. Defaults to None.
+          merge: Whether or not to merge resulting dataframes.
+          pagination_strategy: A Class implementing the :class:`PaginationStrategy`
+            ``Protocol``. If ``None``, then automatic pagination is disabled.
+            Defaults to :class:`LegacyStrategy`.
 
         Returns:
-          pd.DataFrame | list[pd.DataFrame]: A DataFrame containing the reponse data
+          A :class:`pandas.DataFrame` containing the reponse data.
 
         Example:
 
         .. code-block:: python
 
             >>> from subgrounds import Subgrounds
             >>> sg = Subgrounds()
-            >>> univ3 = sg.load_subgraph('https://api.thegraph.com/subgraphs/name/uniswap/uniswap-v3')
+            >>> univ3 = sg.load_subgraph(
+            ...    'https://api.thegraph.com/subgraphs/name/uniswap/uniswap-v3')
 
             # Define price SyntheticField
             >>> univ3.Swap.price = abs(univ3.Swap.amount0) / abs(univ3.Swap.amount1)
 
             # Query last 10 swaps from the ETH/USDC pool
             >>> eth_usdc = univ3.Query.swaps(
             ...     orderBy=univ3.Swap.timestamp,
@@ -425,63 +383,65 @@
         fpaths = list([fpaths] | traverse | map(FieldPath._auto_select) | traverse)
         json_data = self.query_json(fpaths, pagination_strategy=pagination_strategy)
         return df_of_json(json_data, fpaths, columns, concat)
 
     def query_df_iter(
         self,
         fpaths: FieldPath | list[FieldPath],
-        pagination_strategy: Optional[Type[PaginationStrategy]] = LegacyStrategy,
-    ) -> Iterator[pd.DataFrame]:
-        """Same as `query_df` except an iterator over the response data pages is returned
-        Args:
-          fpaths (FieldPath | list[FieldPath]): One or more `FieldPath` objects that
-            should be included in the request
-          columns (Optional[list[str]], optional): The column labels. Defaults to None.
-          merge (bool, optional): Whether or not to merge resulting dataframes.
-          pagination_strategy (Optional[Type[PaginationStrategy]], optional): A Class
-            implementing the :class:`PaginationStrategy` ``Protocol``. If ``None``, then
-            automatic pagination is disabled. Defaults to :class:`LegacyStrategy`.
+        pagination_strategy: Type[PaginationStrategy] | None = LegacyStrategy,
+    ) -> Iterator[pd.DataFrame | list[pd.DataFrame]]:
+        """Same as `query_df` except returns an iterator over the response data pages
+
+        Args:
+          fpaths: One or more `FieldPath` objects that should be included in the request
+          columns: The column labels. Defaults to None.
+          merge: Whether or not to merge resulting dataframes.
+          pagination_strategy: A Class implementing the :class:`PaginationStrategy`
+            ``Protocol``. If ``None``, then automatic pagination is disabled.
+            Defaults to :class:`LegacyStrategy`.
 
         Returns:
-          Iterator[pd.DataFrame]: An iterator over the response data pages, each as a  DataFrame
+          An iterator over the response data pages, each as a :class:`pandas.DataFrame`.
         """
 
         fpaths = list([fpaths] | traverse | map(FieldPath._auto_select) | traverse)
         for page in self.query_json_iter(
             fpaths, pagination_strategy=pagination_strategy
         ):
             yield df_of_json(page, fpaths, None, False)
 
     def query(
         self,
         fpaths: FieldPath | list[FieldPath],
         unwrap: bool = True,
-        pagination_strategy: Optional[Type[PaginationStrategy]] = LegacyStrategy,
+        pagination_strategy: Type[PaginationStrategy] | None = LegacyStrategy,
     ) -> str | int | float | bool | list | tuple | None:
-        """Executes one or multiple ``FieldPath`` objects immediately and return the data (as a tuple if multiple ``FieldPath`` objects are provided).
+        """Executes one or multiple ``FieldPath`` objects immediately and returns the
+        data (as a tuple if multiple ``FieldPath`` objects are provided).
 
         Args:
-          fpaths (FieldPath | list[FieldPath]): One or more ``FieldPath`` object(s) to query.
-          unwrap (bool, optional): Flag indicating whether or not, in the case where
-            the returned data is a list of one element, the element itself should be
-            returned instead of the list. Defaults to ``True``.
-          pagination_strategy (Optional[Type[PaginationStrategy]], optional): A Class
-            implementing the :class:`PaginationStrategy` ``Protocol``. If ``None``, then
-            automatic pagination is disabled. Defaults to :class:`LegacyStrategy`.
+          fpaths: One or more ``FieldPath`` object(s) to query.
+          unwrap: Flag indicating whether or not, in the case where the returned data
+            is a list of one element, the element itself should be returned instead of
+            the list. Defaults to ``True``.
+          pagination_strategy: A Class implementing the :class:`PaginationStrategy`
+            ``Protocol``. If ``None``, then automatic pagination is disabled.
+            Defaults to :class:`LegacyStrategy`.
 
         Returns:
-          [type]: The ``FieldPath`` object(s) data
+          The ``FieldPath`` object(s) data
 
         Example:
 
         .. code-block:: python
 
           >>> from subgrounds import Subgrounds
           >>> sg = Subgrounds()
-          >>> univ3 = sg.load_subgraph('https://api.thegraph.com/subgraphs/name/uniswap/uniswap-v3')
+          >>> univ3 = sg.load_subgraph(
+          ...  'https://api.thegraph.com/subgraphs/name/uniswap/uniswap-v3')
 
           # Define price SyntheticField
           >>> univ3.Swap.price = abs(univ3.Swap.amount0) / abs(univ3.Swap.amount1)
 
           # Construct FieldPath to get price of last swap on ETH/USDC pool
           >>> eth_usdc_last = univ3.Query.swaps(
           ...     orderBy=univ3.Swap.timestamp,
@@ -491,15 +451,14 @@
           ...         univ3.Swap.pool == '0x8ad599c3a0ff1de082011efddc58f1908eb6e6d8'
           ...     ]
           ... ).price
 
           # Query last price FieldPath
           >>> sg.query(eth_usdc_last)
           2628.975030015892
-
         """
 
         fpaths = list([fpaths] | traverse | map(FieldPath._auto_select) | traverse)
         blob = self.query_json(fpaths, pagination_strategy=pagination_strategy)
 
         def f(fpath: FieldPath) -> dict[str, Any]:
             data = fpath._extract_data(blob)
@@ -515,41 +474,45 @@
         else:
             return data
 
     def query_iter(
         self,
         fpaths: FieldPath | list[FieldPath],
         unwrap: bool = True,
-        pagination_strategy: Optional[Type[PaginationStrategy]] = LegacyStrategy,
-    ) -> str | int | float | bool | list | tuple | None:
+        pagination_strategy: Type[PaginationStrategy] | None = LegacyStrategy,
+    ) -> Iterator[str | int | float | bool | list[Any] | tuple | None]:
         """Same as `query` except an iterator over the resonse data pages is returned.
 
         Args:
-          fpath (FieldPath | list[FieldPath]): One or more ``FieldPath`` object(s) to query.
-          unwrap (bool, optional): Flag indicating whether or not, in the case where
+          fpath: One or more ``FieldPath`` object(s) to query.
+          unwrap: Flag indicating whether or not, in the case where
             the returned data is a list of one element, the element itself should be
             returned instead of the list. Defaults to ``True``.
-          pagination_strategy (Optional[Type[PaginationStrategy]], optional): A Class
-            implementing the :class:`PaginationStrategy` ``Protocol``. If ``None``, then
-            automatic pagination is disabled. Defaults to :class:`LegacyStrategy`.
+          pagination_strategy: A Class implementing the :class:`PaginationStrategy`
+            ``Protocol``. If ``None``, then automatic pagination is disabled.
+            Defaults to :class:`LegacyStrategy`.
 
         Returns:
-          Iterator[type]: An iterator over the ``FieldPath`` object(s)' data pages
+          An iterator over the ``FieldPath`` object(s)' data pages
         """
 
         def f(fpath: FieldPath, blob: dict[str, Any]) -> dict[str, Any]:
             data = fpath._extract_data(blob)
             if type(data) == list and len(data) == 1 and unwrap:
                 return data[0]
             else:
                 return data
 
         fpaths = list([fpaths] | traverse | map(FieldPath._auto_select) | traverse)
-        for page in self.query_json_iter(
-            fpaths, pagination_strategy=pagination_strategy
-        ):
+        for page in self.query_json_iter(fpaths, pagination_strategy):
+            data = tuple(fpaths | map(functools.partial(f, blob=page)))
+
+            if len(data) == 1:
+                yield data[0]
+            else:
+                yield data
             data = tuple(fpaths | map(functools.partial(f, blob=page)))
 
             if len(data) == 1:
                 yield data[0]
             else:
                 yield data
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `subgrounds-1.6.0/subgrounds/utils.py` & `subgrounds-1.6.1/subgrounds/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,26 @@
 
 import os
 import platform
 import warnings
 from functools import cache
 from itertools import accumulate as _accumulate
 from itertools import filterfalse
-from typing import Any, Callable, Iterator, Optional, Tuple, TypeVar
+from operator import itemgetter
+from typing import (
+    Any,
+    Callable,
+    Generator,
+    Iterator,
+    ParamSpec,
+    Tuple,
+    TypeVar,
+    cast,
+    overload,
+)
 
 from pipe import Pipe, map
 
 PLAYGROUNDS_APP_URL = "https://app.playgrounds.network/"
 PLAYGROUNDS_API_URL = "https://api.playgrounds.network/"
 PLAYGROUNDS_ENV_VAR = "PLAYGROUNDS_API_KEY"
 
@@ -25,21 +36,25 @@
 
 def identity(x):
     return x
 
 
 T = TypeVar("T")
 U = TypeVar("U")
+V = TypeVar("V")
+P = ParamSpec("P")
 
+Container = list[T] | dict[str, T]
 
-def fst(tup: Tuple[T, U]) -> T:
+
+def fst(tup: Tuple[T, Any]) -> T:
     return tup[0]
 
 
-def snd(tup: Tuple[T, U]) -> U:
+def snd(tup: Tuple[Any, T]) -> T:
     return tup[1]
 
 
 # ================================================================
 # Set utility functions
 # ================================================================
 def intersection(
@@ -77,39 +92,85 @@
     return (
         rel_complement(l1, l2, key)
         + intersection(l1, l2, key, combine)
         + rel_complement(l2, l1, key)
     )
 
 
+@overload
+def merge(data1: list[T], data2: list[T]) -> list[T]:
+    ...
+
+
+@overload
+def merge(data1: dict[str, T], data2: dict[str, T]) -> dict[str, T]:
+    ...
+
+
+def merge(data1: Container, data2: Container) -> Container:
+    """Merges ``data1`` and ``data2`` and returns the combined result.
+
+    ``data1`` and ``data2`` must be of the same type. Either both are
+    ``dict`` or ``list``.
+
+    >>> a = {'a': 1, 'b': {'c': 2, 'd': 3}}
+    >>> b = {'b': {'e': 4}, 'f': 5}
+    >>> merge(a, b)
+    {'a': 1, 'b': {'c': 2, 'd': 3, 'e': 4}, 'f': 5}
+
+    Args:
+      data1 (list[T] | dict[str, T]): First data blob
+      data2 (list[T] | dict[str, T]): Second data blob
+
+    Returns:
+        list[T] | dict[str, T]: Combined data blob
+    """
+
+    match data1, data2:
+        case list(l1), list(l2):
+            return union(l1, l2, itemgetter("id"), combine=merge)
+
+        case dict(d1), dict(d2):
+            data = d1.copy()
+
+            for key in d1:
+                if key in d2:
+                    data[key] = merge(d1[key], d2[key])
+
+            for key in d2:
+                if key not in data:
+                    data[key] = d2[key]
+
+            return data
+
+        case (dict(), _) | (_, dict()) | (list(), _) | (_, list()):
+            raise TypeError(
+                f"merge: incompatible data types!"
+                f"type(data1): {type(data1)} != type(data2): {type(data2)}"
+            )
+
+        case val1, _:
+            return val1
+
+
 # ================================================================
 # Misc
 # ================================================================
-def filter_none(items: list[Optional[T]]) -> list[T]:
+def filter_none(items: list[T | None]) -> list[T]:
     return list(filter(None, items))
 
 
 @Pipe
-def filter_map(items: Iterator[T], mapping: Callable[[T], Optional[T]]) -> Iterator[T]:
+def filter_map(items: Iterator[T], mapping: Callable[[T], T | None]) -> Iterator[T]:
     for item in items:
         new_item = mapping(item)
         if new_item is not None:
             yield new_item
 
 
-def loop_generator(items: list):
-    while True:
-        for item in items:
-            yield item
-
-
-def repeat(value: T, n: int) -> list[T]:
-    return [value for _ in range(n)]
-
-
 # ================================================================
 # Dictionary related utility functions
 # ================================================================
 def extract_data(
     keys: list[str], data: dict[str, Any] | list[dict[str, Any]]
 ) -> list[Any] | Any:
     def f(keys: list[str], data: dict | list | Any):
@@ -122,15 +183,16 @@
                         return f(rest, data[name])
                     case list():
                         return list(data | map(lambda row: f(rest, row[name])))
                     case None:
                         return None
                     case _:
                         raise Exception(
-                            f"extract_data: unexpected state! path = {keys}, data = {data}"
+                            f"extract_data: unexpected state!"
+                            f" path = {keys}, data = {data}"
                         )
 
     match data:
         case dict():
             return f(keys, data)
         case list():
             for doc_data in data:
@@ -141,36 +203,38 @@
             raise Exception(f"extract_data: not found! path = {keys}, data = {data}")
         case _:
             raise Exception("extract_data: data is not dict or list")
 
 
 def flatten_dict(data: dict[str, Any], keys: list[str] = []) -> dict:
     """Takes a dictionary containing key-value pairs where all values are of type
-    other than `list` and flattens it such that all key-value pairs in nested dictionaries
-    are now at depth 1.
+    other than `list` and flattens it such that all key-value pairs in nested
+    dictionaries are now at depth 1.
 
     Args:
-      data (dict): Dictionary containing non-list values
-      keys (list[str], optional): Keys of `data` if `data` is a nested `dict` (`len(keys)` == depth of `data`). Defaults to [].
+      data Dictionary containing non-list values
+      keys: Keys of `data` if `data` is a nested `dict`
+        (`len(keys)` == depth of `data`).  Defaults to [].
 
     Returns:
-      dict: Flat dictionary containing all key-value pairs in `data` and its nested dictionaries
+      dict: Flat dictionary containing all key-value pairs in `data` and its nested
+        dictionaries
     """
     flat_dict: dict[str, Any] = {}
     for key, value in data.items():
         match value:
             case dict():
                 flat_dict = flat_dict | flatten_dict(value, [*keys, key])
             case value:
                 flat_dict["_".join([*keys, key])] = value
 
     return flat_dict
 
 
-def contains_list(data: dict | list | str | int | float | bool) -> bool:
+def contains_list(data: dict[str, Any] | list[Any] | str | int | float | bool) -> bool:
     """Returns `True` if `data` contains a value of type `list` in its nested data
     and `False` otherwise
 
     Args:
       data (dict | list | str | int | float | bool): Data
 
     Returns:
@@ -184,26 +248,38 @@
             return any(data.values() | map(contains_list))
         case set():
             return any(data | map(contains_list))
         case str() | int() | float() | bool():
             return False
 
 
-# def columns_of_json(data: dict, keys: list[str] = []) -> list[str]:
-#   columns: list[str] = []
-#   for key, value in data.items():
-#     match value:
-#       case dict():
-#         columns.append(columns_of_json(value, [*keys, key]))
-#       case list():
-#         columns.append(reduce(union, value | map(partial(columns_of_json, keys=[*keys, key])) | map(lambda x: list(x | traverse)), []))
-#       case value:
-#         columns.append('_'.join([*keys, key]))
+def coroutine_generator(
+    func: Callable[..., Generator[T | None, U, V]]
+) -> Callable[..., Generator[T, U, V]]:
+    """This defines a coroutine styled generator.
+
+    All this does is *start* the generator via a `next` call allowing you to use `.send`
+     immediately instead of needing to use `gen.send(None)` or `next` first.
+
+    Inspired from: http://www.dabeaz.com/coroutines/Coroutines.pdf (p. 27)
+
+    Essentially, the logic is as follows:
+    >>> def start(*args, **kwargs):
+    ...     gen = func(*args, **kwargs)
+    ...     next(gen)
+    ...     return gen
+    """
+
+    def start(*args: P.args, **kwargs: P.kwargs) -> Generator[T, U, V]:
+        gen = func(*args, **kwargs)
+        next(gen)
+        return cast(Generator[T, U, V], gen)
+
+    return start
 
-#   return columns
 
 # ================================================================
 # User Agent / Headers
 # ================================================================
 
 
 @cache
```

### Comparing `subgrounds-1.6.0/setup.py` & `subgrounds-1.6.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,38 +3,41 @@
 
 packages = \
 ['subgrounds',
  'subgrounds.contrib',
  'subgrounds.contrib.dash',
  'subgrounds.contrib.plotly',
  'subgrounds.pagination',
- 'subgrounds.subgraph']
+ 'subgrounds.subgraph',
+ 'subgrounds.transform']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pandas>=1.4.2,<2.0.0',
+['aiohttp>=3.8.4,<4.0.0',
+ 'gql>=3.4.0,<4.0.0',
+ 'pandas>=1.4.2,<2.0.0',
  'pipe>=2.0,<3.0',
  'pydantic>=1.10.2,<2.0.0',
  'requests>=2.27.1,<3.0.0']
 
 extras_require = \
 {'all': ['dash>=2.3.1,<3.0.0',
          'plotly>=5.14.1,<6.0.0',
          'pyodide-http>=0.2.1,<0.3.0'],
  'dash': ['dash>=2.3.1,<3.0.0'],
  'plotly': ['plotly>=5.14.1,<6.0.0'],
  'pyodide': ['pyodide-http>=0.2.1,<0.3.0']}
 
 setup_kwargs = {
     'name': 'subgrounds',
-    'version': '1.6.0',
+    'version': '1.6.1',
     'description': 'A Pythonic data access layer for applications querying data from The Graph Network.',
-    'long_description': "# Subgrounds\n<!-- [![GitHub Actions](https://github.com/0xPlaygrounds/subgrounds/workflows/CI/badge.svg)](https://github.com/0xPlaygrounds/subgrounds/actions) -->\n[![PyPI](https://img.shields.io/pypi/v/subgrounds.svg)](https://pypi.org/project/subgrounds/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/subgrounds.svg)](https://pypi.org/project/subgrounds/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![CI](https://github.com/0xPlaygrounds/subgrounds/actions/workflows/main.yml/badge.svg)](https://github.com/0xPlaygrounds/subgrounds/actions/workflows/main.yml)\n<br>\n\n[![Discord](https://img.shields.io/discord/896944341598208070?color=7289DA&label=discord&logo=discord&logoColor=fff)](https://discord.gg/gMSSh5bjvk)\n[![Twitter Follow](https://img.shields.io/badge/Playgrounds-Analytics-31fa1f2Playgrounds0x?color=%231fa1f2&logo=Twitter&logoColor=1fa1f2&style=flat)](https://twitter.com/Playgrounds0x)\n\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/0xPlaygrounds/subgrounds/blob/main/examples/notebook.ipynb)\n[![Github Codepsaces](https://img.shields.io/badge/Github-Codespaces-24292f.svg?logo=Github)](https://codespaces.new/0xPlaygrounds/subgrounds-template?quickstart=1)\n\n<!-- start elevator-pitch -->\nAn intuitive python library for interfacing with Subgraphs.\n\n## Features\n- **Simple**: Leverage a Pythonic API to easily build queries and transformations without the need for raw GraphQL manipulation.\n- **Automated**: Automatically handle pagination and schema introspection for effortless data retrieval.\n- **Powerful**: Create sophisticated queries using the `SyntheticFields` transformation system.\n<!-- end elevator-pitch -->\n\n## Resources\n- [**Subgrounds Docs**](http://docs.playgrounds.network/): User guide and API documentation\n- [**Examples**](https://github.com/0xPlaygrounds/subgrounds/tree/main/examples): A list of examples showcasing Subgrounds integration with Dash and Plotly\n- [**Community projects**](http://docs.playgrounds.network/subgrounds/examples/): An ever growing list of projects created by our community members\n- [**MetricsDAO Subgrounds Workshop**](https://docs.metricsdao.xyz/get-involved/workshops/2022-03-30+-subgrounds-workshop-series): Subgrounds workshop series hosted by MetricsDAO \n\n## Installation\n> Subgrounds **requires** atleast Python 3.10+\n\nSubgrounds is available on PyPi. To install it, run the following:<br>\n`pip install subgrounds`.\n\nSubgrounds also comes bundled with extra modules that may require extra libraries. You can get all functionality of `subgrounds` via the following:<br>\n`pip install subgrounds[all]`.\n\n## Simple example\n<!-- start simple-example -->\n```python\n>>> from subgrounds import Subgrounds\n\n>>> sg = Subgrounds()\n\n>>> # Load\n>>> aave_v2 = sg.load_subgraph('https://api.thegraph.com/subgraphs/name/messari/aave-v2-ethereum')\n\n>>> # Construct the query\n>>> latest = aave_v2.Query.markets(\n  orderBy=aave_v2.Market.totalValueLockedUSD,\n  orderDirection='desc',\n  first=5,\n)\n\n>>> # Return query to a dataframe\n>>> sg.query_df([\n  latest.name,\n  latest.totalValueLockedUSD,\n])\n                  markets_name  markets_totalValueLockedUSD\n0  Aave interest bearing STETH                 1.522178e+09\n1   Aave interest bearing WETH                 1.221299e+09\n2   Aave interest bearing USDC                 8.140547e+08\n3   Aave interest bearing WBTC                 6.615692e+08\n4   Aave interest bearing USDT                 3.734017e+08\n```\n<!-- end simple-example -->\n\n\n## About Us\nPlaygrounds Analytics is a data solutions company providing serverless on-chain data infrastructures and services for data teams, analysts, and engineers. Checkout us out [here](https://playgrounds.network/) to learn more!\n\n\n## Acknowledgments\nThis software project would not be possible without the support of The Graph Foundation. You can learn more about The Graph and its mission [here](https://thegraph.com/).\n",
+    'long_description': "# Subgrounds\n<!-- [![GitHub Actions](https://github.com/0xPlaygrounds/subgrounds/workflows/CI/badge.svg)](https://github.com/0xPlaygrounds/subgrounds/actions) -->\n[![PyPI](https://img.shields.io/pypi/v/subgrounds.svg)](https://pypi.org/project/subgrounds/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/subgrounds.svg)](https://pypi.org/project/subgrounds/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![CI](https://github.com/0xPlaygrounds/subgrounds/actions/workflows/main.yml/badge.svg)](https://github.com/0xPlaygrounds/subgrounds/actions/workflows/main.yml)\n<br>\n\n[![Discord](https://img.shields.io/discord/896944341598208070?color=7289DA&label=discord&logo=discord&logoColor=fff)](https://discord.gg/gMSSh5bjvk)\n[![Twitter Follow](https://img.shields.io/badge/Playgrounds-Analytics-31fa1f2Playgrounds0x?color=%231fa1f2&logo=Twitter&logoColor=1fa1f2&style=flat)](https://twitter.com/Playgrounds0x)\n\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/0xPlaygrounds/subgrounds/blob/main/examples/notebook.ipynb)\n[![Github Codepsaces](https://img.shields.io/badge/Github-Codespaces-24292f.svg?logo=Github)](https://codespaces.new/0xPlaygrounds/subgrounds-template?quickstart=1)\n\n<!-- start elevator-pitch -->\nAn intuitive python library for interfacing with Subgraphs.\n\n## Features\n- **Simple**: Leverage a Pythonic API to easily build queries and transformations without the need for raw GraphQL manipulation.\n- **Automated**: Automatically handle pagination and schema introspection for effortless data retrieval.\n- **Powerful**: Create sophisticated queries using the `SyntheticFields` transformation system.\n<!-- end elevator-pitch -->\n\n## Resources\n- [**Subgrounds Docs**](http://docs.playgrounds.network/): User guide and API documentation\n- [**Examples**](https://github.com/0xPlaygrounds/subgrounds/tree/main/examples): A list of examples showcasing Subgrounds integration with Dash and Plotly\n- [**Tutorials**](https://docs.playgrounds.network/subgrounds/tutorials/): Subgrounds video workshops and tutorials\n- [**Community Projects**](http://docs.playgrounds.network/subgrounds/examples/): An ever growing list of projects created by our community members\n\n## Installation\n> Subgrounds **requires** atleast Python 3.10+\n\nSubgrounds is available on PyPi. To install it, run the following:<br>\n`pip install subgrounds`.\n\nSubgrounds also comes bundled with extra modules that may require extra libraries. You can get all functionality of `subgrounds` via the following:<br>\n`pip install subgrounds[all]`.\n\n## Simple example\n<!-- start simple-example -->\n```python\n>>> from subgrounds import Subgrounds\n\n>>> sg = Subgrounds()\n\n>>> # Load\n>>> aave_v2 = sg.load_subgraph('https://api.thegraph.com/subgraphs/name/messari/aave-v2-ethereum')\n\n>>> # Construct the query\n>>> latest = aave_v2.Query.markets(\n  orderBy=aave_v2.Market.totalValueLockedUSD,\n  orderDirection='desc',\n  first=5,\n)\n\n>>> # Return query to a dataframe\n>>> sg.query_df([\n  latest.name,\n  latest.totalValueLockedUSD,\n])\n                  markets_name  markets_totalValueLockedUSD\n0  Aave interest bearing STETH                 1.522178e+09\n1   Aave interest bearing WETH                 1.221299e+09\n2   Aave interest bearing USDC                 8.140547e+08\n3   Aave interest bearing WBTC                 6.615692e+08\n4   Aave interest bearing USDT                 3.734017e+08\n```\n<!-- end simple-example -->\n\n\n## About Us\nPlaygrounds Analytics is a data solutions company providing serverless on-chain data infrastructures and services for data teams, analysts, and engineers. Checkout us out [here](https://playgrounds.network/) to learn more!\n\n\n## Acknowledgments\nThis software project would not be possible without the support of The Graph Foundation. You can learn more about The Graph and its mission [here](https://thegraph.com/).\n",
     'author': 'cvauclair',
     'author_email': 'cvauclair@playgrounds.network',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xPlaygrounds/subgrounds',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `subgrounds-1.6.0/PKG-INFO` & `subgrounds-1.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: subgrounds
-Version: 1.6.0
+Version: 1.6.1
 Summary: A Pythonic data access layer for applications querying data from The Graph Network.
 Home-page: https://github.com/0xPlaygrounds/subgrounds
 Keywords: graph,subgrounds,graphql,subgraph
 Author: cvauclair
 Author-email: cvauclair@playgrounds.network
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: dash
 Provides-Extra: plotly
 Provides-Extra: pyodide
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: dash (>=2.3.1,<3.0.0) ; extra == "dash" or extra == "all"
+Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: pipe (>=2.0,<3.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0) ; extra == "plotly" or extra == "all"
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyodide-http (>=0.2.1,<0.3.0) ; extra == "pyodide" or extra == "all"
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Project-URL: Repository, https://github.com/0xPlaygrounds/subgrounds
@@ -46,16 +48,16 @@
 - **Automated**: Automatically handle pagination and schema introspection for effortless data retrieval.
 - **Powerful**: Create sophisticated queries using the `SyntheticFields` transformation system.
 <!-- end elevator-pitch -->
 
 ## Resources
 - [**Subgrounds Docs**](http://docs.playgrounds.network/): User guide and API documentation
 - [**Examples**](https://github.com/0xPlaygrounds/subgrounds/tree/main/examples): A list of examples showcasing Subgrounds integration with Dash and Plotly
-- [**Community projects**](http://docs.playgrounds.network/subgrounds/examples/): An ever growing list of projects created by our community members
-- [**MetricsDAO Subgrounds Workshop**](https://docs.metricsdao.xyz/get-involved/workshops/2022-03-30+-subgrounds-workshop-series): Subgrounds workshop series hosted by MetricsDAO 
+- [**Tutorials**](https://docs.playgrounds.network/subgrounds/tutorials/): Subgrounds video workshops and tutorials
+- [**Community Projects**](http://docs.playgrounds.network/subgrounds/examples/): An ever growing list of projects created by our community members
 
 ## Installation
 > Subgrounds **requires** atleast Python 3.10+
 
 Subgrounds is available on PyPi. To install it, run the following:<br>
 `pip install subgrounds`.
```

