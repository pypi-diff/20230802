# Comparing `tmp/iam_actions-1.2.20230801.tar.gz` & `tmp/iam_actions-1.2.20230802.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230801.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230802.tar", max compression
```

## Comparing `iam_actions-1.2.20230801.tar` & `iam_actions-1.2.20230802.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/LICENSE
--rw-r--r--   0        0        0     2302 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/README.md
--rw-r--r--   0        0        0      228 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/__init__.py
--rw-r--r--   0        0        0  4384975 2023-08-01 02:34:00.833726 iam_actions-1.2.20230801/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-08-01 02:32:04.645722 iam_actions-1.2.20230801/iam_actions/generate/services.py
--rw-r--r--   0        0        0   565668 2023-08-01 02:34:00.833726 iam_actions-1.2.20230801/iam_actions/policies.json
--rw-r--r--   0        0        0   196374 2023-08-01 02:34:00.833726 iam_actions-1.2.20230801/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   548714 2023-08-01 02:34:00.833726 iam_actions-1.2.20230801/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-08-01 02:34:01.697726 iam_actions-1.2.20230801/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230801/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230801/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-02 02:20:03.814925 iam_actions-1.2.20230802/LICENSE
+-rw-r--r--   0        0        0     2302 2023-08-02 02:20:03.814925 iam_actions-1.2.20230802/README.md
+-rw-r--r--   0        0        0      228 2023-08-02 02:20:03.814925 iam_actions-1.2.20230802/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4385500 2023-08-02 02:21:59.721633 iam_actions-1.2.20230802/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-08-02 02:20:03.814925 iam_actions-1.2.20230802/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-08-02 02:20:03.814925 iam_actions-1.2.20230802/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-08-02 02:20:03.814925 iam_actions-1.2.20230802/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-08-02 02:20:03.814925 iam_actions-1.2.20230802/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-08-02 02:20:03.814925 iam_actions-1.2.20230802/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-08-02 02:20:03.814925 iam_actions-1.2.20230802/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-08-02 02:20:03.814925 iam_actions-1.2.20230802/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-08-02 02:20:03.814925 iam_actions-1.2.20230802/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   565668 2023-08-02 02:21:59.721633 iam_actions-1.2.20230802/iam_actions/policies.json
+-rw-r--r--   0        0        0   196374 2023-08-02 02:21:59.721633 iam_actions-1.2.20230802/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   548714 2023-08-02 02:21:59.721633 iam_actions-1.2.20230802/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-08-02 02:22:00.669655 iam_actions-1.2.20230802/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230802/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230802/PKG-INFO
```

### Comparing `iam_actions-1.2.20230801/LICENSE` & `iam_actions-1.2.20230802/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230801/README.md` & `iam_actions-1.2.20230802/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230801/iam_actions/actions.json` & `iam_actions-1.2.20230802/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999884072548346%*

 * *Differences: {"'medialive'": "{'DescribeAccountConfiguration': {'access_level': 'Read', 'description': 'Grants "*

 * *                "permission to view the account configuration of the customer'}, "*

 * *                "'DescribeThumbnails': {'access_level': 'Read', 'description': 'Grants permission "*

 * *                "to view the thumbnails for a channel', 'resources': ['channel']}, "*

 * *                "'UpdateAccountConfiguration': {'access_level': 'Write', 'description': "*

 * *                '"Grants permission to update a custom […]*

```diff
@@ -96717,18 +96717,18 @@
                 "input",
                 "input-security-group",
                 "multiplex",
                 "reservation"
             ]
         },
         "DescribeAccountConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeAccountConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to view the account configuration of the customer",
             "orphan": false,
             "resources": []
         },
         "DescribeChannel": {
             "access_level": "Read",
             "action": "DescribeChannel",
             "condition_keys": [],
@@ -96825,20 +96825,22 @@
             "description": "Grants permission to view a list of actions scheduled on a channel",
             "orphan": false,
             "resources": [
                 "channel"
             ]
         },
         "DescribeThumbnails": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeThumbnails",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to view the thumbnails for a channel",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "channel"
+            ]
         },
         "ListChannels": {
             "access_level": "List",
             "action": "ListChannels",
             "condition_keys": [],
             "description": "Grants permission to list channels",
             "orphan": false,
@@ -97013,18 +97015,18 @@
             "description": "Grants permission to transfer an input device",
             "orphan": false,
             "resources": [
                 "input-device"
             ]
         },
         "UpdateAccountConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateAccountConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a customer's account configuration",
             "orphan": false,
             "resources": []
         },
         "UpdateChannel": {
             "access_level": "Write",
             "action": "UpdateChannel",
             "condition_keys": [],
@@ -145102,21 +145104,33 @@
         }
     },
     "sts": {
         "AssumeRole": {
             "access_level": "Write",
             "action": "AssumeRole",
             "condition_keys": [
+                "accounts.google.com:aud",
+                "accounts.google.com:sub",
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
+                "cognito-identity.amazonaws.com:amr",
+                "cognito-identity.amazonaws.com:aud",
+                "cognito-identity.amazonaws.com:sub",
+                "graph.facebook.com:app_id",
+                "graph.facebook.com:id",
                 "iam:ResourceTag/${TagKey}",
+                "saml:namequalifier",
+                "saml:sub",
+                "saml:sub_type",
                 "sts:ExternalId",
                 "sts:RoleSessionName",
                 "sts:SourceIdentity",
-                "sts:TransitiveTagKeys"
+                "sts:TransitiveTagKeys",
+                "www.amazon.com:app_id",
+                "www.amazon.com:user_id"
             ],
             "description": "Grants permission to obtain a set of temporary security credentials that you can use to access AWS resources that you might not normally have access to",
             "orphan": false,
             "resources": [
                 "role"
             ]
         },
@@ -153975,18 +153989,18 @@
             "action": "UpdateUser",
             "condition_keys": [],
             "description": "Grants permission to update the specified attributes of the specified user, and grants or revokes administrative privileges to the Amazon WorkDocs site",
             "orphan": false,
             "resources": []
         },
         "UpdateUserAdministrativeSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateUserAdministrativeSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update the administrative settings for a user",
             "orphan": false,
             "resources": []
         }
     },
     "worklink": {
         "AssociateDomain": {
             "access_level": "Write",
```

### Comparing `iam_actions-1.2.20230801/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230802/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230801/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230802/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230801/iam_actions/generate/generate.py` & `iam_actions-1.2.20230802/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230801/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230802/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230801/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230802/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230801/iam_actions/generate/services.py` & `iam_actions-1.2.20230802/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230801/iam_actions/policies.json` & `iam_actions-1.2.20230802/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230801/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230802/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230801/iam_actions/services.json` & `iam_actions-1.2.20230802/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230801/pyproject.toml` & `iam_actions-1.2.20230802/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230801"
+version = "1.2.20230802"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230801/setup.py` & `iam_actions-1.2.20230802/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230801',
+    'version': '1.2.20230802',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230801/PKG-INFO` & `iam_actions-1.2.20230802/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230801
+Version: 1.2.20230802
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

