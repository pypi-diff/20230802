# Comparing `tmp/propertysync-0.7.1.tar.gz` & `tmp/propertysync-0.8.0.tar.gz`

## Comparing `propertysync-0.7.1.tar` & `propertysync-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 propertysync-0.7.1/CHANGELOG.md
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.7.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.7.1/.pytest_cache/README.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 propertysync-0.7.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.7.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.7.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/__about__.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/__init__.py
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/api.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/batch.py
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/document.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/search.py
--rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.7.1/propertysync/titlesearch_batch.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.7.1/tests/test_batch.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.7.1/tests/test_document.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.7.1/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.7.1/LICENSE
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.7.1/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 propertysync-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.8.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.8.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.8.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.8.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.8.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/__about__.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/__init__.py
+-rw-r--r--   0        0        0    18750 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/api.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/batch.py
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/document.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/search.py
+-rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/titlesearch_batch.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.8.0/tests/test_batch.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.8.0/tests/test_document.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.8.0/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.8.0/PKG-INFO
```

### Comparing `propertysync-0.7.1/CHANGELOG.md` & `propertysync-0.8.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,36 +3,41 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Generated by [`auto-changelog`](https://github.com/CookPete/auto-changelog).
 
+## [v0.8.0](https://gitlab.com/propertysync/tools/python-api-client/compare/v0.7.0...v0.8.0) - 2023-08-02
+
+### Commits
+
+- new land validation paging [`264c15d`](https://gitlab.com/propertysync/tools/python-api-client/commit/264c15d95334c379e6bd63f9835fa63aae029512)
+- Prevent modifying document when validating [`d944238`](https://gitlab.com/propertysync/tools/python-api-client/commit/d94423880d4febfcf0f3b4e2f6a094a8f23eb97c)
+- New version [`478d40a`](https://gitlab.com/propertysync/tools/python-api-client/commit/478d40ac9feb94ee7f74167cba445eab92b8a23f)
+
 ## [v0.7.0](https://gitlab.com/propertysync/tools/python-api-client/compare/0.5.0...v0.7.0) - 2023-07-21
 
 ### Commits
 
 - add validate_document method [`56c3ef9`](https://gitlab.com/propertysync/tools/python-api-client/commit/56c3ef94907cbebc4b24023d8af077acfb52e3dc)
 - auto-changelog [`490e736`](https://gitlab.com/propertysync/tools/python-api-client/commit/490e736661e73c38df6f51cc0b464511e6de3ae5)
 - changelog / versioning [`7e5338e`](https://gitlab.com/propertysync/tools/python-api-client/commit/7e5338edd842a38b7fd5ee6346f3e24dc6668eed)
 
-<!-- auto-changelog-above -->
+## [0.5.0](https://gitlab.com/propertysync/tools/python-api-client/compare/v0.5.0...0.5.0) - 2023-05-10
 
-## [0.5.0] - 2023-05-10
+## v0.5.0 - 2023-05-10
 
-### Added
-- Lots of work to Batch and Document classes to support find and replace
-- Tests added for Batch and Document classes
-- New API method (get_document_pdf) to retrieve document PDFs
+### Commits
 
-### Changed
-- Do not automatically inject indexingRecordId in TitleSearchBatch helper
+- Initial updates [`e7122c0`](https://gitlab.com/propertysync/tools/python-api-client/commit/e7122c0d498bd7bc366c24e5dcdf1a47941326ef)
+- More work on new classes [`86c71fe`](https://gitlab.com/propertysync/tools/python-api-client/commit/86c71fee5ae87b1e64acd822d3bec6755b6042a4)
+- Updates [`36ef543`](https://gitlab.com/propertysync/tools/python-api-client/commit/36ef543fabfecc45199605742a8c7aea4f1afb05)
 
-### Removed
-- Old batch replace method from Batch class
+<!-- auto-changelog-above -->
 
 ## [0.4.1] - 2023-04-17
 
 ### Changed
 - Minor adjustments to TitleSearchBatch helper for default naming and date format
 
 ## [0.4.0] - 2023-04-17
```

### Comparing `propertysync-0.7.1/propertysync/api.py` & `propertysync-0.8.0/propertysync/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -255,30 +255,60 @@
         body = {
             "type":type,
             "value":value
         }
         return self.api_call("POST", url, body=body)
     
     # get landvalidations
-    def get_landvalidations(self, type=None):
+    def get_landvalidations(self, type=None, pageSize=10000, page=None):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/land-validations"
         params = {}
 
         if type is not None:
             params["type"] = type
 
-        validations = self.api_call("GET", url, params=params)
+        # always get the compact version
+        params["compact"] = 1
 
-        # strip out all fields that are not "id" or "json"
-        for validation in validations:
-            for key in list(validation.keys()):
-                if key != "id" and key != "json":
-                    del validation[key]
+        # default to 10000
+        params["size"] = pageSize
 
-        return validations
+        # if page is not set, assume they want them all. Get the first page to determine the total number of pages
+        if page is None:
+            page = 1
+            params["page"] = page
+            
+            # get the first page, this will tell us how many pages there are
+            validationsPage = self.api_call("GET", url, params=params)
+            validations = validationsPage["data"]
+
+            total = validationsPage["total"]
+            totalPages = total // pageSize
+
+            # if there is a remainder, add one to the total pages
+            if total % pageSize > 0:
+                totalPages += 1
+
+            # if there is more than one page, get the rest of the pages
+            if totalPages > 1:
+                # loop through the rest of the pages
+                for page in range(2,totalPages+1):
+                    params["page"] = page
+
+                    validationsPage = self.api_call("GET", url, params=params)
+
+                    validations += validationsPage["data"]
+
+        else:
+            # they only want a single page
+            params["page"] = page
+            validationsPage = self.api_call("GET", url, params=params)
+            validations = validationsPage["data"]
+
+        return landvalidations
 
     # get document IDs from a search ID
     def get_document_ids_from_search(self, search_id):
         url = f"{self.search_url}/document-groups/{self.document_group_id}/searches/{search_id}/document-ids"
         return self.api_call("GET", url)
     
     # get JSON from a document ID
```

### Comparing `propertysync-0.7.1/propertysync/batch.py` & `propertysync-0.8.0/propertysync/batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.1/propertysync/document.py` & `propertysync-0.8.0/propertysync/document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.1/propertysync/search.py` & `propertysync-0.8.0/propertysync/search.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.1/propertysync/titlesearch_batch.py` & `propertysync-0.8.0/propertysync/titlesearch_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.1/tests/test_batch.py` & `propertysync-0.8.0/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.1/tests/test_document.py` & `propertysync-0.8.0/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.1/LICENSE` & `propertysync-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.1/README.md` & `propertysync-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.1/pyproject.toml` & `propertysync-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propertysync-0.7.1/PKG-INFO` & `propertysync-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertysync
-Version: 0.7.1
+Version: 0.8.0
 Summary: A package for interacting with the PropertySync API.
 Project-URL: Documentation, https://developer.propertysync.com/python/index.html
 Author-email: Rob Martinson <rob@limelyte.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

