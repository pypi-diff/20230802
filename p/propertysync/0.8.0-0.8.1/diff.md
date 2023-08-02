# Comparing `tmp/propertysync-0.8.0.tar.gz` & `tmp/propertysync-0.8.1.tar.gz`

## Comparing `propertysync-0.8.0.tar` & `propertysync-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 propertysync-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.8.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.8.0/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.8.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.8.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.8.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/__about__.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/__init__.py
--rw-r--r--   0        0        0    18750 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/api.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/batch.py
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/document.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/search.py
--rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.8.0/propertysync/titlesearch_batch.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.8.0/tests/test_batch.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.8.0/tests/test_document.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.8.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.8.0/LICENSE
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.8.0/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 propertysync-0.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.8.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.8.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.8.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.8.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.8.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/__about__.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/__init__.py
+-rw-r--r--   0        0        0    18746 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/api.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/batch.py
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/document.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/search.py
+-rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/titlesearch_batch.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.8.1/tests/test_batch.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.8.1/tests/test_document.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.8.1/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.8.1/PKG-INFO
```

### Comparing `propertysync-0.8.0/CHANGELOG.md` & `propertysync-0.8.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Generated by [`auto-changelog`](https://github.com/CookPete/auto-changelog).
 
+## [v0.8.1](https://gitlab.com/propertysync/tools/python-api-client/compare/v0.8.0...v0.8.1) - 2023-08-02
+
+### Commits
+
+- new version [`4d85d5f`](https://gitlab.com/propertysync/tools/python-api-client/commit/4d85d5f429180dee32845c322bf9f4d3abd37d7d)
+- doc updates [`c9ea065`](https://gitlab.com/propertysync/tools/python-api-client/commit/c9ea065bd5e8fa5646536c221e8c19dbd214edd7)
+- fix to validation return [`4b0b4b7`](https://gitlab.com/propertysync/tools/python-api-client/commit/4b0b4b725f594be70c2a4bd11d1323a877b1ac82)
+
 ## [v0.8.0](https://gitlab.com/propertysync/tools/python-api-client/compare/v0.7.0...v0.8.0) - 2023-08-02
 
 ### Commits
 
 - new land validation paging [`264c15d`](https://gitlab.com/propertysync/tools/python-api-client/commit/264c15d95334c379e6bd63f9835fa63aae029512)
 - Prevent modifying document when validating [`d944238`](https://gitlab.com/propertysync/tools/python-api-client/commit/d94423880d4febfcf0f3b4e2f6a094a8f23eb97c)
 - New version [`478d40a`](https://gitlab.com/propertysync/tools/python-api-client/commit/478d40ac9feb94ee7f74167cba445eab92b8a23f)
```

### Comparing `propertysync-0.8.0/propertysync/api.py` & `propertysync-0.8.1/propertysync/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
 
         else:
             # they only want a single page
             params["page"] = page
             validationsPage = self.api_call("GET", url, params=params)
             validations = validationsPage["data"]
 
-        return landvalidations
+        return validations
 
     # get document IDs from a search ID
     def get_document_ids_from_search(self, search_id):
         url = f"{self.search_url}/document-groups/{self.document_group_id}/searches/{search_id}/document-ids"
         return self.api_call("GET", url)
     
     # get JSON from a document ID
```

### Comparing `propertysync-0.8.0/propertysync/batch.py` & `propertysync-0.8.1/propertysync/batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.0/propertysync/document.py` & `propertysync-0.8.1/propertysync/document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.0/propertysync/search.py` & `propertysync-0.8.1/propertysync/search.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.0/propertysync/titlesearch_batch.py` & `propertysync-0.8.1/propertysync/titlesearch_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.0/tests/test_batch.py` & `propertysync-0.8.1/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.0/tests/test_document.py` & `propertysync-0.8.1/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.0/LICENSE` & `propertysync-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.0/README.md` & `propertysync-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.0/pyproject.toml` & `propertysync-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.0/PKG-INFO` & `propertysync-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertysync
-Version: 0.8.0
+Version: 0.8.1
 Summary: A package for interacting with the PropertySync API.
 Project-URL: Documentation, https://developer.propertysync.com/python/index.html
 Author-email: Rob Martinson <rob@limelyte.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

