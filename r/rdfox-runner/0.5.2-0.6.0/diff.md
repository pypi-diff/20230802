# Comparing `tmp/rdfox_runner-0.5.2.tar.gz` & `tmp/rdfox_runner-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfox_runner-0.5.2.tar", max compression
+gzip compressed data, was "rdfox_runner-0.6.0.tar", max compression
```

## Comparing `rdfox_runner-0.5.2.tar` & `rdfox_runner-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2022-09-22 22:12:50.581454 rdfox_runner-0.5.2/LICENSE
--rw-r--r--   0        0        0      720 2023-07-19 15:53:59.103582 rdfox_runner-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      626 2022-09-22 22:12:50.587333 rdfox_runner-0.5.2/src/rdfox_runner/__init__.py
--rw-r--r--   0        0        0    11122 2023-02-26 22:51:13.795239 rdfox_runner-0.5.2/src/rdfox_runner/command_runner.py
--rw-r--r--   0        0        0     9748 2023-07-19 15:43:57.865140 rdfox_runner-0.5.2/src/rdfox_runner/rdfox_endpoint.py
--rw-r--r--   0        0        0    12015 2023-02-26 22:50:50.464757 rdfox_runner-0.5.2/src/rdfox_runner/run_rdfox.py
--rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 rdfox_runner-0.5.2/setup.py
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 rdfox_runner-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-09-22 22:12:50.581454 rdfox_runner-0.6.0/LICENSE
+-rw-r--r--   0        0        0      486 2023-08-02 17:04:25.299763 rdfox_runner-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      626 2022-09-22 22:12:50.587333 rdfox_runner-0.6.0/src/rdfox_runner/__init__.py
+-rw-r--r--   0        0        0    11122 2023-02-26 22:51:13.795239 rdfox_runner-0.6.0/src/rdfox_runner/command_runner.py
+-rw-r--r--   0        0        0    10045 2023-08-02 17:01:26.278983 rdfox_runner-0.6.0/src/rdfox_runner/rdfox_endpoint.py
+-rw-r--r--   0        0        0    12015 2023-02-26 22:50:50.464757 rdfox_runner-0.6.0/src/rdfox_runner/run_rdfox.py
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 rdfox_runner-0.6.0/setup.py
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 rdfox_runner-0.6.0/PKG-INFO
```

### Comparing `rdfox_runner-0.5.2/LICENSE` & `rdfox_runner-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdfox_runner-0.5.2/src/rdfox_runner/__init__.py` & `rdfox_runner-0.6.0/src/rdfox_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `rdfox_runner-0.5.2/src/rdfox_runner/command_runner.py` & `rdfox_runner-0.6.0/src/rdfox_runner/command_runner.py`

 * *Files identical despite different names*

### Comparing `rdfox_runner-0.5.2/src/rdfox_runner/rdfox_endpoint.py` & `rdfox_runner-0.6.0/src/rdfox_runner/rdfox_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 This aims to hide the complexity of setting up RDFox, loading data, adding
 rules, answering queries, behind a simple function that maps data -> answers.
 """
 
 import logging
 import re
 import requests
+from urllib.error import HTTPError
 from textwrap import indent
 from rdflib import Graph, Literal, URIRef
 from rdflib.plugins.stores.sparqlstore import SPARQLUpdateStore
 
 # Pandas is optional, but convenient if available
 try:
     import pandas as pd
@@ -175,14 +176,19 @@
                 qs = urllib.parse.urlparse(err.request.url).query
                 full_query = urllib.parse.parse_qs(qs)["query"][0]
                 logger.error("Query:")
                 for i, line in enumerate(full_query.splitlines()):
                     logger.error(f"Line {i+1}: {line}")
                 raise ParsingError(query=full_query, message=err.response.text)
             raise
+        except ValueError as err:
+            # RDFlib version 6 swallows the error which is not helpful. Run the
+            # query using `query_raw` and hope it gives the same error.
+            self.query_raw(query_object, *args, **kwargs)
+            raise
 
     def query_dataframe(self, query_object, n3=True, *args, **kwargs):
         """Query the SPARQL endpoint, returning a pandas DataFrame.
 
         Because this is often useful for human-readable output, the default is
         to serialise results in N3 notation, using defined prefixes.
```

### Comparing `rdfox_runner-0.5.2/src/rdfox_runner/run_rdfox.py` & `rdfox_runner-0.6.0/src/rdfox_runner/run_rdfox.py`

 * *Files identical despite different names*

### Comparing `rdfox_runner-0.5.2/setup.py` & `rdfox_runner-0.6.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,25 +7,22 @@
 packages = \
 ['rdfox_runner']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['packaging>=15.0',
- 'pyparsing>=2.4.0,<3.0.0',
- 'rdflib>=5.0.0,<6.0.0',
- 'requests>=2.25.1,<3.0.0']
+['packaging>=15.0', 'rdflib>=6.0.0,<7.0.0', 'requests>=2.25.1,<3.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=1.0']}
 
 setup_kwargs = {
     'name': 'rdfox-runner',
-    'version': '0.5.2',
+    'version': '0.6.0',
     'description': '',
     'long_description': 'None',
     'author': 'Rick Lupton',
     'author_email': 'mail@ricklupton.name',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rdfox_runner-0.5.2/PKG-INFO` & `rdfox_runner-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: rdfox-runner
-Version: 0.5.2
+Version: 0.6.0
 Summary: 
 Author: Rick Lupton
 Author-email: mail@ricklupton.name
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: importlib-metadata (>=1.0); python_version < "3.8"
 Requires-Dist: packaging (>=15.0)
-Requires-Dist: pyparsing (>=2.4.0,<3.0.0)
-Requires-Dist: rdflib (>=5.0.0,<6.0.0)
+Requires-Dist: rdflib (>=6.0.0,<7.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
```

