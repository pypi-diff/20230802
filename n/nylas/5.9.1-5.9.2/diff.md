# Comparing `tmp/nylas-5.9.1.tar.gz` & `tmp/nylas-5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nylas-5.9.1.tar", last modified: Tue Jun 21 15:15:06 2022, max compression
+gzip compressed data, was "dist/nylas-5.9.2.tar", last modified: Thu Jun 30 19:42:48 2022, max compression
```

## Comparing `nylas-5.9.1.tar` & `nylas-5.9.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 moose      (502) staff       (20)        0 2022-06-21 15:15:06.714216 nylas-5.9.1/
--rw-r--r--   0 moose      (502) staff       (20)     1127 2022-06-21 15:15:06.714418 nylas-5.9.1/PKG-INFO
--rw-r--r--   0 moose      (502) staff       (20)     3100 2021-06-15 18:57:25.000000 nylas-5.9.1/README.md
-drwxr-xr-x   0 moose      (502) staff       (20)        0 2022-06-21 15:15:06.684529 nylas-5.9.1/nylas/
--rw-r--r--   0 moose      (502) staff       (20)      169 2021-05-11 17:31:07.000000 nylas-5.9.1/nylas/__init__.py
--rw-r--r--   0 moose      (502) staff       (20)       22 2022-06-21 14:39:11.000000 nylas-5.9.1/nylas/_client_sdk_version.py
-drwxr-xr-x   0 moose      (502) staff       (20)        0 2022-06-21 15:15:06.695569 nylas-5.9.1/nylas/client/
--rw-r--r--   0 moose      (502) staff       (20)      130 2021-05-11 17:31:07.000000 nylas-5.9.1/nylas/client/__init__.py
--rw-r--r--   0 moose      (502) staff       (20)     9736 2022-06-21 14:28:25.000000 nylas-5.9.1/nylas/client/authentication_models.py
--rw-r--r--   0 moose      (502) staff       (20)    28124 2022-06-21 14:28:25.000000 nylas-5.9.1/nylas/client/client.py
--rw-r--r--   0 moose      (502) staff       (20)     6534 2022-02-15 17:46:53.000000 nylas-5.9.1/nylas/client/delta_collection.py
--rw-r--r--   0 moose      (502) staff       (20)     1653 2022-02-15 17:46:53.000000 nylas-5.9.1/nylas/client/delta_models.py
--rw-r--r--   0 moose      (502) staff       (20)     1079 2022-01-31 20:29:44.000000 nylas-5.9.1/nylas/client/errors.py
--rw-r--r--   0 moose      (502) staff       (20)     6461 2022-03-31 18:39:43.000000 nylas-5.9.1/nylas/client/neural_api_models.py
--rw-r--r--   0 moose      (502) staff       (20)     6078 2022-03-07 16:48:36.000000 nylas-5.9.1/nylas/client/outbox_models.py
--rw-r--r--   0 moose      (502) staff       (20)     6113 2022-04-13 20:08:40.000000 nylas-5.9.1/nylas/client/restful_model_collection.py
--rw-r--r--   0 moose      (502) staff       (20)    31877 2022-06-21 14:28:25.000000 nylas-5.9.1/nylas/client/restful_models.py
--rw-r--r--   0 moose      (502) staff       (20)     1674 2021-11-24 21:47:27.000000 nylas-5.9.1/nylas/client/scheduler_models.py
--rw-r--r--   0 moose      (502) staff       (20)     2374 2021-11-24 22:50:21.000000 nylas-5.9.1/nylas/client/scheduler_restful_model_collection.py
--rw-r--r--   0 moose      (502) staff       (20)     2035 2022-03-31 18:39:43.000000 nylas-5.9.1/nylas/utils.py
-drwxr-xr-x   0 moose      (502) staff       (20)        0 2022-06-21 15:15:06.686520 nylas-5.9.1/nylas.egg-info/
--rw-r--r--   0 moose      (502) staff       (20)     1127 2022-06-21 15:15:06.000000 nylas-5.9.1/nylas.egg-info/PKG-INFO
--rw-r--r--   0 moose      (502) staff       (20)     1166 2022-06-21 15:15:06.000000 nylas-5.9.1/nylas.egg-info/SOURCES.txt
--rw-r--r--   0 moose      (502) staff       (20)        1 2022-06-21 15:15:06.000000 nylas-5.9.1/nylas.egg-info/dependency_links.txt
--rw-r--r--   0 moose      (502) staff       (20)      175 2022-06-21 15:15:06.000000 nylas-5.9.1/nylas.egg-info/requires.txt
--rw-r--r--   0 moose      (502) staff       (20)       12 2022-06-21 15:15:06.000000 nylas-5.9.1/nylas.egg-info/top_level.txt
--rw-r--r--   0 moose      (502) staff       (20)       66 2022-06-21 15:15:06.714935 nylas-5.9.1/setup.cfg
--rw-r--r--   0 moose      (502) staff       (20)     4106 2022-02-15 17:46:58.000000 nylas-5.9.1/setup.py
-drwxr-xr-x   0 moose      (502) staff       (20)        0 2022-06-21 15:15:06.713341 nylas-5.9.1/tests/
--rw-r--r--   0 moose      (502) staff       (20)        0 2021-05-11 17:31:07.000000 nylas-5.9.1/tests/__init__.py
--rw-r--r--   0 moose      (502) staff       (20)    81892 2022-03-31 20:58:57.000000 nylas-5.9.1/tests/conftest.py
--rw-r--r--   0 moose      (502) staff       (20)     4882 2021-12-29 22:01:16.000000 nylas-5.9.1/tests/test_accounts.py
--rw-r--r--   0 moose      (502) staff       (20)     9359 2022-03-31 20:08:24.000000 nylas-5.9.1/tests/test_authentication.py
--rw-r--r--   0 moose      (502) staff       (20)     9705 2022-04-13 20:08:40.000000 nylas-5.9.1/tests/test_client.py
--rw-r--r--   0 moose      (502) staff       (20)     2739 2021-11-24 23:14:48.000000 nylas-5.9.1/tests/test_components.py
--rw-r--r--   0 moose      (502) staff       (20)     6836 2022-06-21 14:28:25.000000 nylas-5.9.1/tests/test_contacts.py
--rw-r--r--   0 moose      (502) staff       (20)     6028 2022-02-15 17:46:53.000000 nylas-5.9.1/tests/test_delta.py
--rw-r--r--   0 moose      (502) staff       (20)     4307 2021-07-08 22:50:40.000000 nylas-5.9.1/tests/test_drafts.py
--rw-r--r--   0 moose      (502) staff       (20)    23828 2022-05-10 17:02:08.000000 nylas-5.9.1/tests/test_events.py
--rw-r--r--   0 moose      (502) staff       (20)     2456 2021-05-11 17:31:07.000000 nylas-5.9.1/tests/test_files.py
--rw-r--r--   0 moose      (502) staff       (20)     2625 2021-07-08 22:35:20.000000 nylas-5.9.1/tests/test_filter.py
--rw-r--r--   0 moose      (502) staff       (20)      972 2021-12-21 15:44:20.000000 nylas-5.9.1/tests/test_folders.py
--rw-r--r--   0 moose      (502) staff       (20)     1449 2021-12-23 17:31:47.000000 nylas-5.9.1/tests/test_job_status.py
--rw-r--r--   0 moose      (502) staff       (20)     1055 2021-05-11 17:31:07.000000 nylas-5.9.1/tests/test_labels.py
--rw-r--r--   0 moose      (502) staff       (20)     5396 2021-12-08 20:24:58.000000 nylas-5.9.1/tests/test_messages.py
--rw-r--r--   0 moose      (502) staff       (20)     7093 2021-11-04 19:19:25.000000 nylas-5.9.1/tests/test_neural.py
--rw-r--r--   0 moose      (502) staff       (20)     4723 2022-03-07 16:51:16.000000 nylas-5.9.1/tests/test_outbox.py
--rw-r--r--   0 moose      (502) staff       (20)      951 2021-12-14 20:29:23.000000 nylas-5.9.1/tests/test_resources.py
--rw-r--r--   0 moose      (502) staff       (20)    12312 2021-11-24 22:41:47.000000 nylas-5.9.1/tests/test_scheduler.py
--rw-r--r--   0 moose      (502) staff       (20)      981 2022-03-31 15:19:14.000000 nylas-5.9.1/tests/test_search.py
--rw-r--r--   0 moose      (502) staff       (20)     3058 2021-05-11 17:31:07.000000 nylas-5.9.1/tests/test_send_error_handling.py
--rw-r--r--   0 moose      (502) staff       (20)     5411 2021-05-11 17:31:07.000000 nylas-5.9.1/tests/test_threads.py
--rw-r--r--   0 moose      (502) staff       (20)     3213 2022-02-15 17:46:58.000000 nylas-5.9.1/tests/test_webhooks.py
+drwxr-xr-x   0 moose      (502) staff       (20)        0 2022-06-30 19:42:48.360297 nylas-5.9.2/
+-rw-r--r--   0 moose      (502) staff       (20)     1127 2022-06-30 19:42:48.360481 nylas-5.9.2/PKG-INFO
+-rw-r--r--   0 moose      (502) staff       (20)     3100 2021-06-15 18:57:25.000000 nylas-5.9.2/README.md
+drwxr-xr-x   0 moose      (502) staff       (20)        0 2022-06-30 19:42:48.330791 nylas-5.9.2/nylas/
+-rw-r--r--   0 moose      (502) staff       (20)      169 2021-05-11 17:31:07.000000 nylas-5.9.2/nylas/__init__.py
+-rw-r--r--   0 moose      (502) staff       (20)       22 2022-06-30 19:38:53.000000 nylas-5.9.2/nylas/_client_sdk_version.py
+drwxr-xr-x   0 moose      (502) staff       (20)        0 2022-06-30 19:42:48.342977 nylas-5.9.2/nylas/client/
+-rw-r--r--   0 moose      (502) staff       (20)      130 2021-05-11 17:31:07.000000 nylas-5.9.2/nylas/client/__init__.py
+-rw-r--r--   0 moose      (502) staff       (20)     9944 2022-06-27 14:44:38.000000 nylas-5.9.2/nylas/client/authentication_models.py
+-rw-r--r--   0 moose      (502) staff       (20)    28124 2022-06-27 14:41:44.000000 nylas-5.9.2/nylas/client/client.py
+-rw-r--r--   0 moose      (502) staff       (20)     6534 2022-02-15 17:46:53.000000 nylas-5.9.2/nylas/client/delta_collection.py
+-rw-r--r--   0 moose      (502) staff       (20)     1653 2022-02-15 17:46:53.000000 nylas-5.9.2/nylas/client/delta_models.py
+-rw-r--r--   0 moose      (502) staff       (20)     1079 2022-01-31 20:29:44.000000 nylas-5.9.2/nylas/client/errors.py
+-rw-r--r--   0 moose      (502) staff       (20)     6461 2022-03-31 18:39:43.000000 nylas-5.9.2/nylas/client/neural_api_models.py
+-rw-r--r--   0 moose      (502) staff       (20)     6078 2022-03-07 16:48:36.000000 nylas-5.9.2/nylas/client/outbox_models.py
+-rw-r--r--   0 moose      (502) staff       (20)     6113 2022-04-13 20:08:40.000000 nylas-5.9.2/nylas/client/restful_model_collection.py
+-rw-r--r--   0 moose      (502) staff       (20)    32206 2022-06-27 14:44:38.000000 nylas-5.9.2/nylas/client/restful_models.py
+-rw-r--r--   0 moose      (502) staff       (20)     1698 2022-06-27 14:44:38.000000 nylas-5.9.2/nylas/client/scheduler_models.py
+-rw-r--r--   0 moose      (502) staff       (20)     2374 2021-11-24 22:50:21.000000 nylas-5.9.2/nylas/client/scheduler_restful_model_collection.py
+-rw-r--r--   0 moose      (502) staff       (20)     2035 2022-03-31 18:39:43.000000 nylas-5.9.2/nylas/utils.py
+drwxr-xr-x   0 moose      (502) staff       (20)        0 2022-06-30 19:42:48.333300 nylas-5.9.2/nylas.egg-info/
+-rw-r--r--   0 moose      (502) staff       (20)     1127 2022-06-30 19:42:48.000000 nylas-5.9.2/nylas.egg-info/PKG-INFO
+-rw-r--r--   0 moose      (502) staff       (20)     1166 2022-06-30 19:42:48.000000 nylas-5.9.2/nylas.egg-info/SOURCES.txt
+-rw-r--r--   0 moose      (502) staff       (20)        1 2022-06-30 19:42:48.000000 nylas-5.9.2/nylas.egg-info/dependency_links.txt
+-rw-r--r--   0 moose      (502) staff       (20)      175 2022-06-30 19:42:48.000000 nylas-5.9.2/nylas.egg-info/requires.txt
+-rw-r--r--   0 moose      (502) staff       (20)       12 2022-06-30 19:42:48.000000 nylas-5.9.2/nylas.egg-info/top_level.txt
+-rw-r--r--   0 moose      (502) staff       (20)       66 2022-06-30 19:42:48.361018 nylas-5.9.2/setup.cfg
+-rw-r--r--   0 moose      (502) staff       (20)     4106 2022-02-15 17:46:58.000000 nylas-5.9.2/setup.py
+drwxr-xr-x   0 moose      (502) staff       (20)        0 2022-06-30 19:42:48.359529 nylas-5.9.2/tests/
+-rw-r--r--   0 moose      (502) staff       (20)        0 2021-05-11 17:31:07.000000 nylas-5.9.2/tests/__init__.py
+-rw-r--r--   0 moose      (502) staff       (20)    81892 2022-03-31 20:58:57.000000 nylas-5.9.2/tests/conftest.py
+-rw-r--r--   0 moose      (502) staff       (20)     4882 2021-12-29 22:01:16.000000 nylas-5.9.2/tests/test_accounts.py
+-rw-r--r--   0 moose      (502) staff       (20)     9359 2022-03-31 20:08:24.000000 nylas-5.9.2/tests/test_authentication.py
+-rw-r--r--   0 moose      (502) staff       (20)     9705 2022-04-13 20:08:40.000000 nylas-5.9.2/tests/test_client.py
+-rw-r--r--   0 moose      (502) staff       (20)     2739 2021-11-24 23:14:48.000000 nylas-5.9.2/tests/test_components.py
+-rw-r--r--   0 moose      (502) staff       (20)     6836 2022-06-21 14:28:25.000000 nylas-5.9.2/tests/test_contacts.py
+-rw-r--r--   0 moose      (502) staff       (20)     6028 2022-02-15 17:46:53.000000 nylas-5.9.2/tests/test_delta.py
+-rw-r--r--   0 moose      (502) staff       (20)     4307 2021-07-08 22:50:40.000000 nylas-5.9.2/tests/test_drafts.py
+-rw-r--r--   0 moose      (502) staff       (20)    23828 2022-05-10 17:02:08.000000 nylas-5.9.2/tests/test_events.py
+-rw-r--r--   0 moose      (502) staff       (20)     2456 2021-05-11 17:31:07.000000 nylas-5.9.2/tests/test_files.py
+-rw-r--r--   0 moose      (502) staff       (20)     2625 2021-07-08 22:35:20.000000 nylas-5.9.2/tests/test_filter.py
+-rw-r--r--   0 moose      (502) staff       (20)      972 2021-12-21 15:44:20.000000 nylas-5.9.2/tests/test_folders.py
+-rw-r--r--   0 moose      (502) staff       (20)     1449 2021-12-23 17:31:47.000000 nylas-5.9.2/tests/test_job_status.py
+-rw-r--r--   0 moose      (502) staff       (20)     1055 2021-05-11 17:31:07.000000 nylas-5.9.2/tests/test_labels.py
+-rw-r--r--   0 moose      (502) staff       (20)     5396 2021-12-08 20:24:58.000000 nylas-5.9.2/tests/test_messages.py
+-rw-r--r--   0 moose      (502) staff       (20)     7093 2021-11-04 19:19:25.000000 nylas-5.9.2/tests/test_neural.py
+-rw-r--r--   0 moose      (502) staff       (20)     4723 2022-03-07 16:51:16.000000 nylas-5.9.2/tests/test_outbox.py
+-rw-r--r--   0 moose      (502) staff       (20)      951 2021-12-14 20:29:23.000000 nylas-5.9.2/tests/test_resources.py
+-rw-r--r--   0 moose      (502) staff       (20)    12312 2021-11-24 22:41:47.000000 nylas-5.9.2/tests/test_scheduler.py
+-rw-r--r--   0 moose      (502) staff       (20)      981 2022-03-31 15:19:14.000000 nylas-5.9.2/tests/test_search.py
+-rw-r--r--   0 moose      (502) staff       (20)     3058 2021-05-11 17:31:07.000000 nylas-5.9.2/tests/test_send_error_handling.py
+-rw-r--r--   0 moose      (502) staff       (20)     5411 2021-05-11 17:31:07.000000 nylas-5.9.2/tests/test_threads.py
+-rw-r--r--   0 moose      (502) staff       (20)     3213 2022-02-15 17:46:58.000000 nylas-5.9.2/tests/test_webhooks.py
```

### Comparing `nylas-5.9.1/PKG-INFO` & `nylas-5.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nylas
-Version: 5.9.1
+Version: 5.9.2
 Summary: Python bindings for Nylas, the next-generation email platform.
 Home-page: https://github.com/nylas/nylas-python
 Author: Nylas Team
 Author-email: support@nylas.com
 License: MIT
 Description: 
         # Nylas REST API Python bindings
```

### Comparing `nylas-5.9.1/README.md` & `nylas-5.9.2/README.md`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/nylas/client/authentication_models.py` & `nylas-5.9.2/nylas/client/authentication_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,16 +49,19 @@
             kwargs = kwargs.get("data")
         obj = super(Integration, cls).create(api, **kwargs)
         if "provider" in kwargs:
             obj["id"] = kwargs.get("provider")
 
         return obj
 
-    def as_json(self):
-        dct = super(Integration, self).as_json()
+    def as_json(self, enforce_read_only=True):
+        dct = super(Integration, self).as_json(enforce_read_only)
+        if enforce_read_only is False:
+            return dct
+
         if not self.id:
             if isinstance(self.provider, Authentication.Provider):
                 dct["provider"] = self.provider.value
             else:
                 dct["provider"] = self.provider
 
         return dct
@@ -104,16 +107,19 @@
     @classmethod
     def create(cls, api, **kwargs):
         if "data" in kwargs:
             kwargs = kwargs.get("data")
         obj = super(Grant, cls).create(api, **kwargs)
         return obj
 
-    def as_json(self):
-        dct = super(Grant, self).as_json()
+    def as_json(self, enforce_read_only=True):
+        dct = super(Grant, self).as_json(enforce_read_only)
+        if enforce_read_only is False:
+            return dct
+
         # provider and state can not be updated
         if self.id:
             del dct["provider"]
             del dct["state"]
         else:
             if isinstance(self.provider, Authentication.Provider):
                 dct["provider"] = self.provider.value
```

### Comparing `nylas-5.9.1/nylas/client/client.py` & `nylas-5.9.2/nylas/client/client.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/nylas/client/delta_collection.py` & `nylas-5.9.2/nylas/client/delta_collection.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/nylas/client/delta_models.py` & `nylas-5.9.2/nylas/client/delta_models.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/nylas/client/errors.py` & `nylas-5.9.2/nylas/client/errors.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/nylas/client/neural_api_models.py` & `nylas-5.9.2/nylas/client/neural_api_models.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/nylas/client/outbox_models.py` & `nylas-5.9.2/nylas/client/outbox_models.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/nylas/client/restful_model_collection.py` & `nylas-5.9.2/nylas/client/restful_model_collection.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/nylas/client/restful_models.py` & `nylas-5.9.2/nylas/client/restful_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -687,16 +687,19 @@
                 "owner",
                 "status",
                 "master_event_id",
                 "original_start_time",
             }
         )
 
-    def as_json(self):
-        dct = NylasAPIObject.as_json(self)
+    def as_json(self, enforce_read_only=True):
+        dct = NylasAPIObject.as_json(self, enforce_read_only)
+        if enforce_read_only is False:
+            return dct
+
         # Filter some parameters we got from the API
         if dct.get("when"):
             # Currently, the event (self) and the dict (dct) share the same
             # reference to the `'when'` dict.  We need to clone the dict so
             # that when we remove the object key, the original event's
             # `'when'` reference is unmodified.
             dct["when"] = dct["when"].copy()
@@ -916,16 +919,19 @@
             {
                 "public_application_id",
                 "created_at",
                 "updated_at",
             }
         )
 
-    def as_json(self):
-        dct = NylasAPIObject.as_json(self)
+    def as_json(self, enforce_read_only=True):
+        dct = NylasAPIObject.as_json(self, enforce_read_only)
+        if enforce_read_only is False:
+            return dct
+
         # "type" cannot be modified after created
         if self.id:
             dct.pop("type")
         return dct
 
 
 class Webhook(NylasAPIObject):
@@ -941,21 +947,21 @@
     collection_name = "webhooks"
     api_root = "a"
 
     def __init__(self, api):
         NylasAPIObject.__init__(self, Webhook, api)
         self.read_only_attrs.update({"application_id", "version"})
 
-    def as_json(self):
+    def as_json(self, enforce_read_only=True):
         dct = {}
         # Only 'state' can get updated
-        if self.id:
+        if self.id and enforce_read_only is True:
             dct["state"] = self.state
         else:
-            dct = NylasAPIObject.as_json(self)
+            dct = NylasAPIObject.as_json(self, enforce_read_only)
         return dct
 
     class Trigger(str, Enum):
         """
         This is an Enum representing all the possible webhook triggers
 
         see more: https://developer.nylas.com/docs/developer-tools/webhooks/available-webhooks
@@ -1031,17 +1037,19 @@
     ]
 
     collection_name = "accounts"
 
     def __init__(self, api):
         NylasAPIObject.__init__(self, Account, api)
 
-    def as_json(self):
-        dct = {"metadata": self.metadata}
-        return dct
+    def as_json(self, enforce_read_only=True):
+        if enforce_read_only is False:
+            return NylasAPIObject.as_json(self, enforce_read_only)
+        else:
+            return {"metadata": self.metadata}
 
     def upgrade(self):
         return self.api._call_resource_method(self, self.account_id, "upgrade", None)
 
     def downgrade(self):
         return self.api._call_resource_method(self, self.account_id, "downgrade", None)
 
@@ -1060,15 +1068,11 @@
     datetime_attrs = {"linked_at": "linked_at"}
 
     collection_name = "accounts"
 
     def __init__(self, api):
         NylasAPIObject.__init__(self, APIAccount, api)
 
-    def as_json(self):
-        dct = NylasAPIObject.as_json(self)
-        return dct
-
 
 class SingletonAccount(APIAccount):
     # This is an APIAccount that lives under /account.
     collection_name = "account"
```

### Comparing `nylas-5.9.1/nylas/client/scheduler_models.py` & `nylas-5.9.2/nylas/client/scheduler_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         "timezone",
         "slot",
     ]
 
     def __init__(self, api):
         RestfulModel.__init__(self, SchedulerBookingRequest, api)
 
-    def as_json(self):
+    def as_json(self, enforce_read_only=True):
         dct = RestfulModel.as_json(self)
         if "additional_values" not in dct or dct["additional_values"] is None:
             dct["additional_values"] = {}
         if "additional_emails" not in dct or dct["additional_emails"] is None:
             dct["additional_emails"] = []
         if "slot" in dct and isinstance(dct["slot"], SchedulerTimeSlot):
             dct["slot"] = dct["slot"].as_json()
```

### Comparing `nylas-5.9.1/nylas/client/scheduler_restful_model_collection.py` & `nylas-5.9.2/nylas/client/scheduler_restful_model_collection.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/nylas/utils.py` & `nylas-5.9.2/nylas/utils.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/nylas.egg-info/PKG-INFO` & `nylas-5.9.2/nylas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nylas
-Version: 5.9.1
+Version: 5.9.2
 Summary: Python bindings for Nylas, the next-generation email platform.
 Home-page: https://github.com/nylas/nylas-python
 Author: Nylas Team
 Author-email: support@nylas.com
 License: MIT
 Description: 
         # Nylas REST API Python bindings
```

### Comparing `nylas-5.9.1/nylas.egg-info/SOURCES.txt` & `nylas-5.9.2/nylas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/setup.py` & `nylas-5.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/conftest.py` & `nylas-5.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_accounts.py` & `nylas-5.9.2/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_authentication.py` & `nylas-5.9.2/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_client.py` & `nylas-5.9.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_components.py` & `nylas-5.9.2/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_contacts.py` & `nylas-5.9.2/tests/test_contacts.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_delta.py` & `nylas-5.9.2/tests/test_delta.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_drafts.py` & `nylas-5.9.2/tests/test_drafts.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_events.py` & `nylas-5.9.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_files.py` & `nylas-5.9.2/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_filter.py` & `nylas-5.9.2/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_folders.py` & `nylas-5.9.2/tests/test_folders.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_job_status.py` & `nylas-5.9.2/tests/test_job_status.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_labels.py` & `nylas-5.9.2/tests/test_labels.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_messages.py` & `nylas-5.9.2/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_neural.py` & `nylas-5.9.2/tests/test_neural.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_outbox.py` & `nylas-5.9.2/tests/test_outbox.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_resources.py` & `nylas-5.9.2/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_scheduler.py` & `nylas-5.9.2/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_search.py` & `nylas-5.9.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_send_error_handling.py` & `nylas-5.9.2/tests/test_send_error_handling.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_threads.py` & `nylas-5.9.2/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `nylas-5.9.1/tests/test_webhooks.py` & `nylas-5.9.2/tests/test_webhooks.py`

 * *Files identical despite different names*

