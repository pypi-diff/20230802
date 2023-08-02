# Comparing `tmp/watchful-3.5.2.tar.gz` & `tmp/watchful-3.6.0.tar.gz`

## Comparing `watchful-3.5.2.tar` & `watchful-3.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 watchful-3.5.2/src/watchful/__about__.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 watchful-3.5.2/src/watchful/__init__.py
--rw-r--r--   0        0        0    40216 2020-02-02 00:00:00.000000 watchful-3.5.2/src/watchful/attributes.py
--rw-r--r--   0        0        0    48875 2020-02-02 00:00:00.000000 watchful-3.5.2/src/watchful/client.py
--rw-r--r--   0        0        0    17219 2020-02-02 00:00:00.000000 watchful-3.5.2/src/watchful/client2.py
--rw-r--r--   0        0        0    16002 2020-02-02 00:00:00.000000 watchful-3.5.2/src/watchful/enrich.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 watchful-3.5.2/src/watchful/enricher.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 watchful-3.5.2/src/watchful/types.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 watchful-3.5.2/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 watchful-3.5.2/LICENSE
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 watchful-3.5.2/README.md
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 watchful-3.5.2/pyproject.toml
--rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 watchful-3.5.2/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 watchful-3.6.0/src/watchful/__about__.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 watchful-3.6.0/src/watchful/__init__.py
+-rw-r--r--   0        0        0    40216 2020-02-02 00:00:00.000000 watchful-3.6.0/src/watchful/attributes.py
+-rw-r--r--   0        0        0    47044 2020-02-02 00:00:00.000000 watchful-3.6.0/src/watchful/client.py
+-rw-r--r--   0        0        0    17219 2020-02-02 00:00:00.000000 watchful-3.6.0/src/watchful/client2.py
+-rw-r--r--   0        0        0    16002 2020-02-02 00:00:00.000000 watchful-3.6.0/src/watchful/enrich.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 watchful-3.6.0/src/watchful/enricher.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 watchful-3.6.0/src/watchful/types.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 watchful-3.6.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 watchful-3.6.0/LICENSE
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 watchful-3.6.0/README.md
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 watchful-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 watchful-3.6.0/PKG-INFO
```

### Comparing `watchful-3.5.2/src/watchful/__init__.py` & `watchful-3.6.0/src/watchful/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,22 +34,18 @@
     base_rate,
     await_plabels,
     hinter_async,
     hinter,
     delete,
     delete_class,
     get,
-    external_hinter,
     upload_attributes,
     load_attributes,
     dump,
     dump_dicts,
-    hint,
-    apply_hints,
-    hint_all,
     export_stream,
     export_dataset_to_path,
     export_async,
     export,
     export_preview,
     export_project,
     is_utf8,
```

### Comparing `watchful-3.5.2/src/watchful/attributes.py` & `watchful-3.6.0/src/watchful/attributes.py`

 * *Files identical despite different names*

### Comparing `watchful-3.5.2/src/watchful/client.py` & `watchful-3.6.0/src/watchful/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -859,41 +859,14 @@
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     return api("nop")
 
 
-def external_hinter(class__: str, name: str, weight: int) -> Optional[Dict]:
-    """
-    This function creates an external hinter.
-
-    :param class__: The class for the hinter.
-    :type class__: str
-    :param name: The name for the hinter.
-    :type name: str
-    :param weight: The weight for the hinter.
-    :type weight: int
-    :return: The dictionary of the HTTP response from the connection request.
-    :rtype: Dict, optional
-    """
-
-    _assert_success(
-        api(
-            "hinter",
-            query="[external]",
-            name=name,
-            label=class__,
-            weight=weight,
-        )
-    )
-
-    return await_plabels()
-
-
 def upload_attributes(
     dataset_id: str,
     attributes_filepath: str,
 ) -> Dict:
     """
     This function uploads the attributes for the ``dataset_id`` to the remote
     Watchful application, where the Watchful application then saves it to a
@@ -988,67 +961,14 @@
     """
 
     field_names = get()["field_names"]
     for c in dump():
         yield dict(zip(field_names, c))
 
 
-def hint(name: str, offset: int, values: List[bool]) -> Optional[Dict]:
-    """
-    This function adds the hints for an external hinter.
-
-    :param name: The hinter name.
-    :type name: str
-    :param offset: The offset.
-    :type offset: int
-    :param values: The hints.
-    :type values: List[bool]
-    :return: The dictionary of the HTTP response from the connection request.
-    :rtype: Dict, optional
-
-    TODO: Come up with a better streaming Python API here.
-    """
-
-    values = list(map(lambda x: x, values))
-
-    return _assert_success(api("hint", name=name, offset=offset, values=values))
-
-
-def apply_hints(name: str) -> Optional[Dict]:
-    """
-    This function applies the hints for an external hinter.
-
-    :param name: The hinter name.
-    :type name: str
-    :return: The dictionary of the HTTP response from the connection request.
-    :rtype: Dict, optional
-    """
-
-    _assert_success(api("apply_hints", name=name))
-
-    return await_plabels()
-
-
-def hint_all(name: str, values: List[bool]) -> Optional[Dict]:
-    """
-    This function applies the hints for an external hinter.
-
-    :param name: The hinter name.
-    :type name: str
-    :param values: The hints.
-    :type values: List[bool]
-    :return: The dictionary of the HTTP response from the connection request.
-    :rtype: Dict, optional
-    """
-
-    hint(name, 0, values)
-
-    return apply_hints(name)
-
-
 def export_stream(
     content_type: str = "text/csv",
     mode: str = "ftc",
 ) -> requests.models.Response:
     """
     This function begins the export using the export_stream call. The result is
     not JSON, but is data to be processed directly.
@@ -1082,37 +1002,39 @@
         200 == response.status_code
     ), f"Request could have failed with status {response.status_code}."
 
     return response
 
 
 def export_dataset_to_path(
-    out_file: str, fields: Optional[List[str]] = None
+    out_file: str, fields: Optional[List[str]] = None, export_mode: str = "ftc"
 ) -> None:
     """
     This function exports the original dataset via a buffered stream to the
     specified output file path. It takes ``fields`` as an optional argument for
     the header (column names), for the case where the callee expects to use
     specific columns; otherwise it uses the column names returned by the
     Watchful application. An exception is raised when the dataset's column names
     do not match the user's expected column names.
 
     :param out_file: The file path to export the original dataset to.
     :type out_file: str
     :param fields: The list of column names to use for the dataset export.
     :type fields: List, optional
+    :param export_mode: Allowed values - "ftc", "ner", and "data"
+    :type export_mode: str
     """
 
     if fields is None:
         fields = get()["field_names"]
     n_cols = len(fields)
 
     with open(out_file, "w", encoding="utf-8") as f:
         writer = csv.writer(f)
-        stream = export_stream().raw
+        stream = export_stream(mode=export_mode).raw
         stream.auto_close = False
         reader = csv.reader(
             io.TextIOWrapper(stream, encoding="utf-8", newline="")
         )
         header = next(reader)
         if header[:n_cols] != fields:
             raise ValueError(
@@ -1120,36 +1042,36 @@
                 f"column names {fields}."
             )
         writer.writerow(fields)
         for row in reader:
             writer.writerow(row[:n_cols])
 
 
-def export_async() -> Optional[Dict]:
+def export_async(export_mode: str = "ftc") -> Optional[Dict]:
     """
     This function exports the dataset. As it is asynchronous, the immediate HTTP
     response is likely not updated yet.
 
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
-    return api("export", query="", content_type="text/csv")
+    return api("export", query="", content_type="text/csv", mode=export_mode)
 
 
-def export() -> Optional[Dict]:
+def export(export_mode: str = "ftc") -> Optional[Dict]:
     """
     This function exports the dataset and returns an updated HTTP response.
 
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     n_exports = len(get()["exports"])
-    export_async()
+    export_async(export_mode)
 
     return await_summary(lambda s: len(s["exports"]) == n_exports + 1)
 
 
 def export_preview(mode: str = "ftc") -> Optional[Dict]:
     """
     Returns a preview of the export.
```

### Comparing `watchful-3.5.2/src/watchful/client2.py` & `watchful-3.6.0/src/watchful/client2.py`

 * *Files identical despite different names*

### Comparing `watchful-3.5.2/src/watchful/enrich.py` & `watchful-3.6.0/src/watchful/enrich.py`

 * *Files identical despite different names*

### Comparing `watchful-3.5.2/src/watchful/enricher.py` & `watchful-3.6.0/src/watchful/enricher.py`

 * *Files identical despite different names*

### Comparing `watchful-3.5.2/LICENSE` & `watchful-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `watchful-3.5.2/README.md` & `watchful-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `watchful-3.5.2/pyproject.toml` & `watchful-3.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `watchful-3.5.2/PKG-INFO` & `watchful-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchful
-Version: 3.5.2
+Version: 3.6.0
 Summary: Watchful API for Interacting with Watchful Environment
 Project-URL: Bug Tracker, https://github.com/Watchfulio/watchful-py/issues
 Project-URL: Homepage, https://github.com/Watchfulio/watchful-py
 Author: Inc.
 Author-email: Watchful <engineering@watchful.io>
 License-Expression: MIT
 License-File: LICENSE
```

