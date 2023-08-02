# Comparing `tmp/pysnyk-0.9.7.tar.gz` & `tmp/pysnyk-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnyk-0.9.7.tar", max compression
+gzip compressed data, was "pysnyk-0.9.8.tar", max compression
```

## Comparing `pysnyk-0.9.7.tar` & `pysnyk-0.9.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1057 2023-07-31 08:05:18.373277 pysnyk-0.9.7/LICENSE
--rw-r--r--   0        0        0    11993 2023-07-31 08:05:18.373277 pysnyk-0.9.7/README.md
--rw-r--r--   0        0        0      913 2023-07-31 08:05:18.373277 pysnyk-0.9.7/pyproject.toml
--rw-r--r--   0        0        0      679 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/__init__.py
--rw-r--r--   0        0        0      219 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/__version__.py
--rw-r--r--   0        0        0     8969 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/client.py
--rw-r--r--   0        0        0      655 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/errors.py
--rw-r--r--   0        0        0    17705 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/managers.py
--rw-r--r--   0        0        0    24867 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/models.py
--rw-r--r--   0        0        0    12805 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_client.py
--rw-r--r--   0        0        0      497 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/organizations.json
--rw-r--r--   0        0        0     2172 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/projects.json
--rw-r--r--   0        0        0      397 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/rest_groups.json
--rw-r--r--   0        0        0     3340 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/rest_targets_page1.json
--rw-r--r--   0        0        0     3359 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/rest_targets_page2.json
--rw-r--r--   0        0        0     3339 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/rest_targets_page3.json
--rw-r--r--   0        0        0      397 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/v3_groups.json
--rw-r--r--   0        0        0     3340 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/v3_targets_page1.json
--rw-r--r--   0        0        0     3359 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/v3_targets_page2.json
--rw-r--r--   0        0        0     3339 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/v3_targets_page3.json
--rw-r--r--   0        0        0      460 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_manager.py
--rw-r--r--   0        0        0    34583 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_models.py
--rw-r--r--   0        0        0      722 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_utils.py
--rw-r--r--   0        0        0     1253 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/utils.py
--rw-r--r--   0        0        0    12893 1970-01-01 00:00:00.000000 pysnyk-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-08-02 14:35:54.775160 pysnyk-0.9.8/LICENSE
+-rw-r--r--   0        0        0    11993 2023-08-02 14:35:54.775160 pysnyk-0.9.8/README.md
+-rw-r--r--   0        0        0      913 2023-08-02 14:35:54.779160 pysnyk-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0      679 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/__init__.py
+-rw-r--r--   0        0        0      219 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/__version__.py
+-rw-r--r--   0        0        0     8969 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/client.py
+-rw-r--r--   0        0        0      655 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/errors.py
+-rw-r--r--   0        0        0    17670 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/managers.py
+-rw-r--r--   0        0        0    24867 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/models.py
+-rw-r--r--   0        0        0    12805 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_client.py
+-rw-r--r--   0        0        0      497 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_data/organizations.json
+-rw-r--r--   0        0        0     2172 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_data/projects.json
+-rw-r--r--   0        0        0      397 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_data/rest_groups.json
+-rw-r--r--   0        0        0     3340 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_data/rest_targets_page1.json
+-rw-r--r--   0        0        0     3359 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_data/rest_targets_page2.json
+-rw-r--r--   0        0        0     3339 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_data/rest_targets_page3.json
+-rw-r--r--   0        0        0      397 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_data/v3_groups.json
+-rw-r--r--   0        0        0     3340 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_data/v3_targets_page1.json
+-rw-r--r--   0        0        0     3359 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_data/v3_targets_page2.json
+-rw-r--r--   0        0        0     3339 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_data/v3_targets_page3.json
+-rw-r--r--   0        0        0      460 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_manager.py
+-rw-r--r--   0        0        0    34583 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_models.py
+-rw-r--r--   0        0        0      722 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/test_utils.py
+-rw-r--r--   0        0        0     1253 2023-08-02 14:35:54.779160 pysnyk-0.9.8/snyk/utils.py
+-rw-r--r--   0        0        0    12893 1970-01-01 00:00:00.000000 pysnyk-0.9.8/PKG-INFO
```

### Comparing `pysnyk-0.9.7/LICENSE` & `pysnyk-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/README.md` & `pysnyk-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/pyproject.toml` & `pysnyk-0.9.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnyk"
-version = "0.9.7"
+version = "0.9.8"
 description = "A Python client for the Snyk API"
 authors = [
   "Gareth Rushgrove <garethr@snyk.io>",
 ]
 license = "MIT"
 packages = [
   { include = "snyk" },
```

### Comparing `pysnyk-0.9.7/snyk/__init__.py` & `pysnyk-0.9.8/snyk/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/client.py` & `pysnyk-0.9.8/snyk/client.py`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/errors.py` & `pysnyk-0.9.8/snyk/errors.py`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/managers.py` & `pysnyk-0.9.8/snyk/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,17 +148,15 @@
             "name": attributes.get("name"),
             "id": project.get("id"),
             "created": attributes.get("created"),
             "origin": attributes.get("origin"),
             "type": attributes.get("type"),
             "readOnly": attributes.get("read_only"),
             "testFrequency": recurring_tests.get("frequency"),
-            "isMonitored": True
-            if project.get("meta", {}).get("cli_monitored_at")
-            else False,
+            "isMonitored": True if attributes.get("status") == "active" else False,
             "issueCountsBySeverity": {
                 "low": issue_counts.get("low"),
                 "medium": issue_counts.get("medium"),
                 "high": issue_counts.get("high"),
                 "critical": issue_counts.get("critical"),
             },
             "targetReference": attributes.get("target_reference"),
```

### Comparing `pysnyk-0.9.7/snyk/models.py` & `pysnyk-0.9.8/snyk/models.py`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/test_client.py` & `pysnyk-0.9.8/snyk/test_client.py`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/test_data/projects.json` & `pysnyk-0.9.8/snyk/test_data/projects.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/test_data/rest_targets_page1.json` & `pysnyk-0.9.8/snyk/test_data/rest_targets_page1.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/test_data/rest_targets_page2.json` & `pysnyk-0.9.8/snyk/test_data/rest_targets_page2.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/test_data/rest_targets_page3.json` & `pysnyk-0.9.8/snyk/test_data/rest_targets_page3.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/test_data/v3_targets_page1.json` & `pysnyk-0.9.8/snyk/test_data/v3_targets_page1.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/test_data/v3_targets_page2.json` & `pysnyk-0.9.8/snyk/test_data/v3_targets_page2.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/test_data/v3_targets_page3.json` & `pysnyk-0.9.8/snyk/test_data/v3_targets_page3.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/test_models.py` & `pysnyk-0.9.8/snyk/test_models.py`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/test_utils.py` & `pysnyk-0.9.8/snyk/test_utils.py`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/snyk/utils.py` & `pysnyk-0.9.8/snyk/utils.py`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.7/PKG-INFO` & `pysnyk-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnyk
-Version: 0.9.7
+Version: 0.9.8
 Summary: A Python client for the Snyk API
 Home-page: https://github.com/snyk-labs/pysnyk
 License: MIT
 Author: Gareth Rushgrove
 Author-email: garethr@snyk.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

