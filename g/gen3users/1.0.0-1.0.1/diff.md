# Comparing `tmp/gen3users-1.0.0.tar.gz` & `tmp/gen3users-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3users-1.0.0.tar", max compression
+gzip compressed data, was "gen3users-1.0.1.tar", max compression
```

## Comparing `gen3users-1.0.0.tar` & `gen3users-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11358 2023-07-28 20:10:49.637672 gen3users-1.0.0/LICENSE
--rw-r--r--   0        0        0      558 2023-07-28 20:10:49.637672 gen3users-1.0.0/NOTICE
--rw-r--r--   0        0        0     1101 2023-07-28 20:10:49.637672 gen3users-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-07-28 20:10:49.637672 gen3users-1.0.0/gen3users/__init__.py
--rw-r--r--   0        0        0     2303 2023-07-28 20:10:49.637672 gen3users-1.0.0/gen3users/base_abac.json
--rw-r--r--   0        0        0     8661 2023-07-28 20:10:49.637672 gen3users-1.0.0/gen3users/conversion.py
--rw-r--r--   0        0        0     1438 2023-07-28 20:10:49.637672 gen3users-1.0.0/gen3users/main.py
--rw-r--r--   0        0        0    22130 2023-07-28 20:10:49.637672 gen3users-1.0.0/gen3users/validation.py
--rw-r--r--   0        0        0      566 2023-07-28 20:10:49.637672 gen3users-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 gen3users-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-08-02 20:49:21.489245 gen3users-1.0.1/LICENSE
+-rw-r--r--   0        0        0      558 2023-08-02 20:49:21.489245 gen3users-1.0.1/NOTICE
+-rw-r--r--   0        0        0     1101 2023-08-02 20:49:21.489245 gen3users-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 20:49:21.489245 gen3users-1.0.1/gen3users/__init__.py
+-rw-r--r--   0        0        0     2303 2023-08-02 20:49:21.489245 gen3users-1.0.1/gen3users/base_abac.json
+-rw-r--r--   0        0        0     8661 2023-08-02 20:49:21.489245 gen3users-1.0.1/gen3users/conversion.py
+-rw-r--r--   0        0        0     1438 2023-08-02 20:49:21.489245 gen3users-1.0.1/gen3users/main.py
+-rw-r--r--   0        0        0    22175 2023-08-02 20:49:21.489245 gen3users-1.0.1/gen3users/validation.py
+-rw-r--r--   0        0        0      566 2023-08-02 20:49:21.489245 gen3users-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 gen3users-1.0.1/PKG-INFO
```

### Comparing `gen3users-1.0.0/LICENSE` & `gen3users-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3users-1.0.0/NOTICE` & `gen3users-1.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `gen3users-1.0.0/README.md` & `gen3users-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gen3users-1.0.0/gen3users/base_abac.json` & `gen3users-1.0.1/gen3users/base_abac.json`

 * *Files identical despite different names*

### Comparing `gen3users-1.0.0/gen3users/conversion.py` & `gen3users-1.0.1/gen3users/conversion.py`

 * *Files identical despite different names*

### Comparing `gen3users-1.0.0/gen3users/main.py` & `gen3users-1.0.1/gen3users/main.py`

 * *Files identical despite different names*

### Comparing `gen3users-1.0.0/gen3users/validation.py` & `gen3users-1.0.1/gen3users/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,14 +636,15 @@
     may allow users to access things in services that were not intended to be accessible. For example:
     - Anonymous users have access to public project "projectA". We use a "reader" role with "service = *".
     - If a user has "read" access for service "requestor" in a project, the Requestor service allows them
     to see access requests for the project.
     - Because of "service = *", anonymous users can see who requested access to "projectA", and whether their
     access was approved!
     """
+    logger.info("- Checking roles security")
     ok = True
 
     all_policies_dict = {
         e["id"]: e for e in user_yaml_dict["authz"].get("policies", [])
     }
     all_roles_dict = {e["id"]: e for e in user_yaml_dict["authz"].get("roles", [])}
```

### Comparing `gen3users-1.0.0/pyproject.toml` & `gen3users-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gen3users"
-version = "1.0.0"
+version = "1.0.1"
 description = "Utils for Gen3 Commons user management"
 authors = ["CTDS UChicago <cdis@uchicago.edu>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/uc-cdis/gen3utils"
 include = [
   "CHANGELOG.md",
```

### Comparing `gen3users-1.0.0/PKG-INFO` & `gen3users-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3users
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utils for Gen3 Commons user management
 Home-page: https://github.com/uc-cdis/gen3utils
 License: Apache-2.0
 Author: CTDS UChicago
 Author-email: cdis@uchicago.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

