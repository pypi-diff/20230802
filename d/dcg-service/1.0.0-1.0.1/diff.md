# Comparing `tmp/dcg_service-1.0.0.tar.gz` & `tmp/dcg_service-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcg_service-1.0.0.tar", last modified: Sat Jul 29 08:43:55 2023, max compression
+gzip compressed data, was "dcg_service-1.0.1.tar", last modified: Wed Aug  2 12:58:59 2023, max compression
```

## Comparing `dcg_service-1.0.0.tar` & `dcg_service-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-29 08:43:55.249016 dcg_service-1.0.0/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1073 2023-07-12 05:37:10.000000 dcg_service-1.0.0/LICENCE
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6879 2023-07-29 08:43:55.249016 dcg_service-1.0.0/PKG-INFO
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6376 2023-07-12 07:13:10.000000 dcg_service-1.0.0/README.md
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      585 2023-07-29 04:19:47.000000 dcg_service-1.0.0/pyproject.toml
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      116 2023-07-29 04:20:53.000000 dcg_service-1.0.0/requirement.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       38 2023-07-29 08:43:55.249016 dcg_service-1.0.0/setup.cfg
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-29 08:43:55.241016 dcg_service-1.0.0/src/
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-29 08:43:55.245016 dcg_service-1.0.0/src/dcg_service/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-12 05:23:41.000000 dcg_service-1.0.0/src/dcg_service/__init__.py
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-29 08:43:55.249016 dcg_service-1.0.0/src/dcg_service/core/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      298 2023-07-10 10:49:06.000000 dcg_service-1.0.0/src/dcg_service/core/__init__.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2683 2023-07-18 12:26:17.000000 dcg_service-1.0.0/src/dcg_service/core/authentication.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2378 2023-07-29 05:43:24.000000 dcg_service-1.0.0/src/dcg_service/core/encryption.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     8115 2023-07-29 04:46:39.000000 dcg_service-1.0.0/src/dcg_service/core/events.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     4988 2023-07-29 05:42:10.000000 dcg_service-1.0.0/src/dcg_service/core/exceptions.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2319 2023-07-10 09:24:25.000000 dcg_service-1.0.0/src/dcg_service/core/filters.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      618 2023-07-10 10:39:56.000000 dcg_service-1.0.0/src/dcg_service/core/logger.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2926 2023-07-19 06:15:57.000000 dcg_service-1.0.0/src/dcg_service/core/permissions.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     3038 2023-07-18 12:25:40.000000 dcg_service-1.0.0/src/dcg_service/core/request_client.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1341 2023-07-13 06:38:22.000000 dcg_service-1.0.0/src/dcg_service/core/response.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)    16746 2023-07-29 08:31:31.000000 dcg_service-1.0.0/src/dcg_service/core/services.py
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     7789 2023-07-29 05:38:38.000000 dcg_service-1.0.0/src/dcg_service/core/utils.py
-drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-29 08:43:55.245016 dcg_service-1.0.0/src/dcg_service.egg-info/
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6879 2023-07-29 08:43:55.000000 dcg_service-1.0.0/src/dcg_service.egg-info/PKG-INFO
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      677 2023-07-29 08:43:55.000000 dcg_service-1.0.0/src/dcg_service.egg-info/SOURCES.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        1 2023-07-29 08:43:55.000000 dcg_service-1.0.0/src/dcg_service.egg-info/dependency_links.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      117 2023-07-29 08:43:55.000000 dcg_service-1.0.0/src/dcg_service.egg-info/requires.txt
--rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       12 2023-07-29 08:43:55.000000 dcg_service-1.0.0/src/dcg_service.egg-info/top_level.txt
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-08-02 12:58:59.643688 dcg_service-1.0.1/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1073 2023-07-12 05:37:10.000000 dcg_service-1.0.1/LICENCE
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6879 2023-08-02 12:58:59.643688 dcg_service-1.0.1/PKG-INFO
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6376 2023-07-12 07:13:10.000000 dcg_service-1.0.1/README.md
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      585 2023-08-02 12:54:08.000000 dcg_service-1.0.1/pyproject.toml
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      116 2023-07-29 04:20:53.000000 dcg_service-1.0.1/requirement.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       38 2023-08-02 12:58:59.643688 dcg_service-1.0.1/setup.cfg
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-08-02 12:58:59.635688 dcg_service-1.0.1/src/
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-08-02 12:58:59.635688 dcg_service-1.0.1/src/dcg_service/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        0 2023-07-12 05:23:41.000000 dcg_service-1.0.1/src/dcg_service/__init__.py
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-08-02 12:58:59.643688 dcg_service-1.0.1/src/dcg_service/core/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      298 2023-07-10 10:49:06.000000 dcg_service-1.0.1/src/dcg_service/core/__init__.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2803 2023-08-02 11:30:14.000000 dcg_service-1.0.1/src/dcg_service/core/authentication.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2378 2023-07-29 05:43:24.000000 dcg_service-1.0.1/src/dcg_service/core/encryption.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     8441 2023-08-02 12:17:01.000000 dcg_service-1.0.1/src/dcg_service/core/events.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     4988 2023-07-29 05:42:10.000000 dcg_service-1.0.1/src/dcg_service/core/exceptions.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2319 2023-07-10 09:24:25.000000 dcg_service-1.0.1/src/dcg_service/core/filters.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      618 2023-07-10 10:39:56.000000 dcg_service-1.0.1/src/dcg_service/core/logger.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     2926 2023-07-19 06:15:57.000000 dcg_service-1.0.1/src/dcg_service/core/permissions.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     3038 2023-07-18 12:25:40.000000 dcg_service-1.0.1/src/dcg_service/core/request_client.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     1341 2023-07-13 06:38:22.000000 dcg_service-1.0.1/src/dcg_service/core/response.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)    16746 2023-07-29 08:31:31.000000 dcg_service-1.0.1/src/dcg_service/core/services.py
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     7931 2023-08-02 12:52:27.000000 dcg_service-1.0.1/src/dcg_service/core/utils.py
+drwxrwxr-x   0 zapbuild  (1000) zapbuild  (1000)        0 2023-08-02 12:58:59.635688 dcg_service-1.0.1/src/dcg_service.egg-info/
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)     6879 2023-08-02 12:58:59.000000 dcg_service-1.0.1/src/dcg_service.egg-info/PKG-INFO
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      677 2023-08-02 12:58:59.000000 dcg_service-1.0.1/src/dcg_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)        1 2023-08-02 12:58:59.000000 dcg_service-1.0.1/src/dcg_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)      117 2023-08-02 12:58:59.000000 dcg_service-1.0.1/src/dcg_service.egg-info/requires.txt
+-rw-rw-r--   0 zapbuild  (1000) zapbuild  (1000)       12 2023-08-02 12:58:59.000000 dcg_service-1.0.1/src/dcg_service.egg-info/top_level.txt
```

### Comparing `dcg_service-1.0.0/LICENCE` & `dcg_service-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `dcg_service-1.0.0/PKG-INFO` & `dcg_service-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcg_service
-Version: 1.0.0
+Version: 1.0.1
 Summary: DCG DOT Compliance Group
 Author-email: Aman Kumar <amankumar@zapbuild.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcg_service-1.0.0/README.md` & `dcg_service-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dcg_service-1.0.0/pyproject.toml` & `dcg_service-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dcg_service"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Aman Kumar", email="amankumar@zapbuild.com" },
 ]
 description = "DCG DOT Compliance Group"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcg_service-1.0.0/src/dcg_service/core/authentication.py` & `dcg_service-1.0.1/src/dcg_service/core/authentication.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,17 @@
 
 
 def authenticate(token):
     """
     Returns a two-tuple of `User` and token if a valid signature has been
     supplied using JWT-based authentication.  Otherwise, returns `None`.
     """
+    if not token:
+        raise AuthException(
+            _('Invalid Authorization header. No credentials provided.'))
     auth = token.split()
     auth_header_prefix = 'bearer'
     if auth[0].lower() != auth_header_prefix:
         raise AuthException(_('Invalid prefix.'))
     if len(auth) == 1:
         raise AuthException(
             _('Invalid Authorization header. No credentials provided.'))
```

### Comparing `dcg_service-1.0.0/src/dcg_service/core/encryption.py` & `dcg_service-1.0.1/src/dcg_service/core/encryption.py`

 * *Files identical despite different names*

### Comparing `dcg_service-1.0.0/src/dcg_service/core/events.py` & `dcg_service-1.0.1/src/dcg_service/core/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,30 +105,38 @@
             response = search.execute()
             hits = response.hits
 
             if hits:
                 # Retrieve the first matching document and update the activity array
                 hit = hits[0]
                 index_id = hit.meta.id
+                data = hit.to_dict()
                 existing_activities = json.loads(
-                    getattr(hit, 'Activities', "[]"))  # Deserialize existing_activities if present.
+                    data.get('Activities', "[]") or "[]")  # Deserialize existing_activities if present.
                 existing_activities.append(activity_data)
                 update_body = {
                     "doc": {
                         "Activities": json.dumps(existing_activities)  # Serialize existing_activities before updating.
                     }
                 }
+                if not request_id:
+                    update_body['UserName'] = 'System'
+                    update_body['UserType'] = 'SYSTEM'
+
                 EsClient.update(index=ACTIVITY_INDEX, id=index_id, body=update_body)
                 EsClient.indices.refresh(index=ACTIVITY_INDEX)
             else:
                 log_body = {
                     "RequestID": request_id,
                     "Activities": json.dumps([activity_data])
                     # Serialize activity_data before inserting a new document.
                 }
+                if not request_id:
+                    log_body['UserName'] = 'System'
+                    log_body['UserType'] = 'SYSTEM'
                 EsClient.index(index=ACTIVITY_INDEX, body=log_body)
                 EsClient.indices.refresh(index=ACTIVITY_INDEX)
         except Exception as error:
             print("Error saving activity: %s" % str(error))
 
     @classmethod
     def get_history(cls, mapped_obj, target, column):
```

### Comparing `dcg_service-1.0.0/src/dcg_service/core/exceptions.py` & `dcg_service-1.0.1/src/dcg_service/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcg_service-1.0.0/src/dcg_service/core/filters.py` & `dcg_service-1.0.1/src/dcg_service/core/filters.py`

 * *Files identical despite different names*

### Comparing `dcg_service-1.0.0/src/dcg_service/core/logger.py` & `dcg_service-1.0.1/src/dcg_service/core/logger.py`

 * *Files identical despite different names*

### Comparing `dcg_service-1.0.0/src/dcg_service/core/permissions.py` & `dcg_service-1.0.1/src/dcg_service/core/permissions.py`

 * *Files identical despite different names*

### Comparing `dcg_service-1.0.0/src/dcg_service/core/request_client.py` & `dcg_service-1.0.1/src/dcg_service/core/request_client.py`

 * *Files identical despite different names*

### Comparing `dcg_service-1.0.0/src/dcg_service/core/response.py` & `dcg_service-1.0.1/src/dcg_service/core/response.py`

 * *Files identical despite different names*

### Comparing `dcg_service-1.0.0/src/dcg_service/core/services.py` & `dcg_service-1.0.1/src/dcg_service/core/services.py`

 * *Files identical despite different names*

### Comparing `dcg_service-1.0.0/src/dcg_service/core/utils.py` & `dcg_service-1.0.1/src/dcg_service/core/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     try:
         from . import EsClient, APP_NAME
         error_string = error
         if not error:
             error_string = traceback.format_exc()
         headers = getattr(request, 'headers', {})
         request_id = headers.get("Request-Id")
-        request_user = getattr(request, 'user')
+        request_user = getattr(request, 'user', None)
         body = {
             "Path": getattr(request, 'full_path', None) or getattr(request, 'path', None),
             "Method": getattr(request, 'method', None),
             "Entity": APP_NAME,
             "Data": str(error_string),
             "StatusCode": 500,
             "Timestamp": datetime.now(),
@@ -124,38 +124,43 @@
           to be imported from the module (specified by the '.' in the import statement).
         - The function uses the `datetime.now()` method to record the current timestamp for the log entry.
 
     :param kwargs:
     :return:
     """
     try:
-        from . import ACTIVITY_INDEX, EsClient, APP_NAME
+        from . import EsClient, ACTIVITY_INDEX, APP_NAME
         options = kwargs
-        headers = getattr(request, 'headers', options.get('headers', {})) or {}
-        request_id = headers.get("Request-Id")
         request_user = getattr(request, 'user', None)
 
         request_company_id = None
         if options.get('body') and ('company_id' in options['body'] or 'organisation_id' in options['body']):
             request_company_id = options['body'].get('company_id') or options['body'].get('organisation_id')
 
+        if options.get('response') and type(options.get('response')) == dict:
+            options['response']['action'] = options.get('action')
+        else:
+            options['response'] = {
+                'action': options.get('action')
+            }
+
         body = {
             "LogType": "API",
             "Method": getattr(request, 'method', None),
             "Path": getattr(request, 'full_path', None) or getattr(request, 'path', None),
             "URL": getattr(request, 'url', None),
-            "RequestID": request_id,
+            "RequestID": None,
             "RequestBody": json.dumps(options.get('body', {}) or {}),
-            "Headers": getattr(request, 'headers', options.get('headers', {})),
-            "StatusCode": options.get('status_code'),
+            "Headers": dict(getattr(request, 'headers', options.get('headers', {}))),
+            "StatusCode": options.get('status_code') or 200,
             "RequestCompanyID": request_company_id or options.get('request_company_id'),
             "Response": json.dumps(options.get('response', {}) or {}),
             "UserID": getattr(request_user, 'id', options.get('user_id')),
             "UserType": getattr(request_user, 'user_type', options.get('user_type')),
-            "UserName": getattr(request_user, 'first_name', options.get('first_name')),
+            "UserName": getattr(request_user, 'first_name', options.get('user_name')),
             "ApplicationID": getattr(request_user, 'application_id', options.get('application_id')),
             "CompanyID": getattr(request_user, 'company_id', options.get('company_id')),
             "Service": APP_NAME,
             "LoginID":  getattr(request_user, 'login_id', options.get('login_id')),
             "Timestamp": datetime.now(),
             "Activities": options.get('activities') or [],
             "Action": options.get('action')
```

### Comparing `dcg_service-1.0.0/src/dcg_service.egg-info/PKG-INFO` & `dcg_service-1.0.1/src/dcg_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcg-service
-Version: 1.0.0
+Version: 1.0.1
 Summary: DCG DOT Compliance Group
 Author-email: Aman Kumar <amankumar@zapbuild.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcg_service-1.0.0/src/dcg_service.egg-info/SOURCES.txt` & `dcg_service-1.0.1/src/dcg_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

