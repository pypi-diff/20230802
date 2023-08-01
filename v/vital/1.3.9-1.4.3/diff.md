# Comparing `tmp/vital-1.3.9.tar.gz` & `tmp/vital-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-1.3.9.tar", max compression
+gzip compressed data, was "vital-1.4.3.tar", max compression
```

## Comparing `vital-1.3.9.tar` & `vital-1.4.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      388 2023-05-23 08:44:09.363236 vital-1.3.9/README.md
--rw-r--r--   0        0        0     1123 2023-05-23 08:44:09.363236 vital-1.3.9/pyproject.toml
--rw-r--r--   0        0        0      107 2023-05-23 08:44:09.363236 vital-1.3.9/vital/__init__.py
--rw-r--r--   0        0        0      702 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/__init__.py
--rw-r--r--   0        0        0     1531 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/activity.py
--rw-r--r--   0        0        0      142 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/api.py
--rw-r--r--   0        0        0     2904 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/athome_phlebotomy.py
--rw-r--r--   0        0        0     1515 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/body.py
--rw-r--r--   0        0        0      598 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/devices.py
--rw-r--r--   0        0        0     2656 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/labtests.py
--rw-r--r--   0        0        0     3093 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/link.py
--rw-r--r--   0        0        0      823 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/meals.py
--rw-r--r--   0        0        0      820 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/profile.py
--rw-r--r--   0        0        0        0 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/schema/__init__.py
--rw-r--r--   0        0        0     1719 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/schema/athome_phlebotomy.py
--rw-r--r--   0        0        0     2259 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/sleep.py
--rw-r--r--   0        0        0     2287 2023-05-23 08:44:09.367236 vital-1.3.9/vital/api/user.py
--rw-r--r--   0        0        0     3866 2023-05-23 08:44:09.367236 vital-1.3.9/vital/api/vitals.py
--rw-r--r--   0        0        0      632 2023-05-23 08:44:09.367236 vital-1.3.9/vital/api/webhooks.py
--rw-r--r--   0        0        0     1318 2023-05-23 08:44:09.367236 vital-1.3.9/vital/api/workouts.py
--rw-r--r--   0        0        0     5888 2023-05-23 08:44:09.367236 vital-1.3.9/vital/client.py
--rw-r--r--   0        0        0     3118 2023-05-23 08:44:09.367236 vital-1.3.9/vital/errors.py
--rw-r--r--   0        0        0        0 2023-05-23 08:44:09.367236 vital-1.3.9/vital/internal/__init__.py
--rw-r--r--   0        0        0     2363 2023-05-23 08:44:09.367236 vital-1.3.9/vital/internal/requester.py
--rw-r--r--   0        0        0       80 2023-05-23 08:44:09.367236 vital-1.3.9/vital/internal/utils.py
--rw-r--r--   0        0        0     2762 2023-05-23 08:44:09.367236 vital-1.3.9/vital/internal/webhook.py
--rw-r--r--   0        0        0      359 2023-05-23 08:44:09.367236 vital-1.3.9/vital/types.py
--rw-r--r--   0        0        0      239 2023-05-23 08:44:09.367236 vital-1.3.9/vital/version.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 vital-1.3.9/setup.py
--rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 vital-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0      388 2023-08-01 23:30:56.806006 vital-1.4.3/README.md
+-rw-r--r--   0        0        0     1123 2023-08-01 23:30:56.806006 vital-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-08-01 23:30:56.810006 vital-1.4.3/vital/__init__.py
+-rw-r--r--   0        0        0      702 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/__init__.py
+-rw-r--r--   0        0        0     1531 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/activity.py
+-rw-r--r--   0        0        0      142 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/api.py
+-rw-r--r--   0        0        0     2904 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/athome_phlebotomy.py
+-rw-r--r--   0        0        0     1515 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/body.py
+-rw-r--r--   0        0        0      598 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/devices.py
+-rw-r--r--   0        0        0     3306 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/labtests.py
+-rw-r--r--   0        0        0     3093 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/link.py
+-rw-r--r--   0        0        0      823 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/meals.py
+-rw-r--r--   0        0        0      820 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/profile.py
+-rw-r--r--   0        0        0        0 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/schema/__init__.py
+-rw-r--r--   0        0        0     1719 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/schema/athome_phlebotomy.py
+-rw-r--r--   0        0        0     2259 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/sleep.py
+-rw-r--r--   0        0        0     2287 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/user.py
+-rw-r--r--   0        0        0     3866 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/vitals.py
+-rw-r--r--   0        0        0      632 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/webhooks.py
+-rw-r--r--   0        0        0     1318 2023-08-01 23:30:56.810006 vital-1.4.3/vital/api/workouts.py
+-rw-r--r--   0        0        0     5888 2023-08-01 23:30:56.810006 vital-1.4.3/vital/client.py
+-rw-r--r--   0        0        0     3118 2023-08-01 23:30:56.810006 vital-1.4.3/vital/errors.py
+-rw-r--r--   0        0        0        0 2023-08-01 23:30:56.810006 vital-1.4.3/vital/internal/__init__.py
+-rw-r--r--   0        0        0     2363 2023-08-01 23:30:56.810006 vital-1.4.3/vital/internal/requester.py
+-rw-r--r--   0        0        0       80 2023-08-01 23:30:56.810006 vital-1.4.3/vital/internal/utils.py
+-rw-r--r--   0        0        0     2762 2023-08-01 23:30:56.810006 vital-1.4.3/vital/internal/webhook.py
+-rw-r--r--   0        0        0      359 2023-08-01 23:30:56.810006 vital-1.4.3/vital/types.py
+-rw-r--r--   0        0        0      239 2023-08-01 23:30:56.810006 vital-1.4.3/vital/version.py
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 vital-1.4.3/setup.py
+-rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 vital-1.4.3/PKG-INFO
```

### Comparing `vital-1.3.9/pyproject.toml` & `vital-1.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vital"
-version = "1.3.9"
+version = "1.4.3"
 description = ""
 authors = ["maitham <maitham@tryvital.io>"]
 license = "GNU"
 readme = "README.md"
 homepage = "https://github.com/adeptlabs/vital-python"
 repository = "https://github.com/adeptlabs/vital-python"
 keywords = ["vital", "tryvital", "python"]
```

### Comparing `vital-1.3.9/vital/api/__init__.py` & `vital-1.4.3/vital/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/api/activity.py` & `vital-1.4.3/vital/api/activity.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/api/athome_phlebotomy.py` & `vital-1.4.3/vital/api/athome_phlebotomy.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/api/body.py` & `vital-1.4.3/vital/api/body.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/api/devices.py` & `vital-1.4.3/vital/api/devices.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/api/labtests.py` & `vital-1.4.3/vital/api/labtests.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,27 +10,51 @@
         self,
         user_id: str,
         patient_details: Dict,
         patient_address: Dict,
         lab_test_id: str,
         physician: Optional[Dict],
         health_insurance: Optional[Dict] = None,
+        priority: Optional[bool] = None,
     ) -> Mapping[str, str]:
         """Create new order"""
         params = {
             "user_id": user_id,
             "patient_details": patient_details,
             "patient_address": patient_address,
             "lab_test_id": lab_test_id,
             "physician": physician,
         }
         if health_insurance:
             params["health_insurance"] = health_insurance
+        if priority:
+            params["priority"] = priority
 
         return self.client.post("/order", params, api_version="v3")
+    
+    def create_test(
+        self,
+        name: str,
+        description: str,
+        markers: list[str],
+        lab_id: int,
+        method: str,
+        sample_type: str,
+    ) -> Mapping[str, str]:
+        """Create new lab test"""
+        params = {
+            "name": name,
+            "description": description,
+            "lab_id": lab_id,
+            "method": method,
+            "sample_type": sample_type,
+            "marker_ids": markers,
+        }
+
+        return self.client.post("/lab_tests", params, api_version="v3")
 
     def get_orders(self, page: int = 1, size: int = 50) -> Mapping[str, str]:
         """Get all orders"""
         return self.client.get(
             "/orders",
             {"page": page, "size": size},
             api_version="v3",
```

### Comparing `vital-1.3.9/vital/api/link.py` & `vital-1.4.3/vital/api/link.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/api/meals.py` & `vital-1.4.3/vital/api/meals.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/api/profile.py` & `vital-1.4.3/vital/api/profile.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/api/schema/athome_phlebotomy.py` & `vital-1.4.3/vital/api/schema/athome_phlebotomy.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/api/sleep.py` & `vital-1.4.3/vital/api/sleep.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/api/user.py` & `vital-1.4.3/vital/api/user.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/api/vitals.py` & `vital-1.4.3/vital/api/vitals.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,9 +120,9 @@
         """
         Get blood oxygen values from the API
         :param str user_id: user's id
         :param str start_date: date in ISO format
         :param str end_date: date in ISO format
         """
         return self._timeseries_request(
-            user_id, start_date, end_date, "blood_oxygen", provider
+            user_id, start_date, "blood_oxygen", end_date, provider
         )
```

### Comparing `vital-1.3.9/vital/api/webhooks.py` & `vital-1.4.3/vital/api/webhooks.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/api/workouts.py` & `vital-1.4.3/vital/api/workouts.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/client.py` & `vital-1.4.3/vital/client.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/errors.py` & `vital-1.4.3/vital/errors.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/internal/requester.py` & `vital-1.4.3/vital/internal/requester.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/vital/internal/webhook.py` & `vital-1.4.3/vital/internal/webhook.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.9/setup.py` & `vital-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pydantic>=1.10.7,<2.0.0',
  'requests',
  'svix>=0.41.2,<0.42.0',
  'typed-ast>=1.5.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'vital',
-    'version': '1.3.9',
+    'version': '1.4.3',
     'description': '',
     'long_description': "# vital-python\n\nThe official Python Library for [Vital API](https://docs.tryvital.io)\n\n# Install\n\n```\npip install vital\n```\n\n# Installing locally\n\n```\npoetry build --format sdist\ntar -xvf dist/*-`poetry version -s`.tar.gz -O '*/setup.py' > setup.py\n```\n\n## Documentation\n\nPlease refer to the official [Vital docs](https://docs.tryvital.io) provide a full reference on using this library.\n",
     'author': 'maitham',
     'author_email': 'maitham@tryvital.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/adeptlabs/vital-python',
```

### Comparing `vital-1.3.9/PKG-INFO` & `vital-1.4.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vital
-Version: 1.3.9
+Version: 1.4.3
 Summary: 
 Home-page: https://github.com/adeptlabs/vital-python
 License: GNU
 Keywords: vital,tryvital,python
 Author: maitham
 Author-email: maitham@tryvital.io
 Requires-Python: >=3.8,<4.0
```

