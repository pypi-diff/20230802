# Comparing `tmp/bridgeql-0.2.1.tar.gz` & `tmp/bridgeql-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bridgeql-0.2.1.tar", last modified: Fri May 19 13:51:20 2023, max compression
+gzip compressed data, was "bridgeql-0.2.2.tar", last modified: Wed Aug  2 11:01:15 2023, max compression
```

## Comparing `bridgeql-0.2.1.tar` & `bridgeql-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 priyanksi   (501) staff       (20)        0 2023-05-19 13:51:20.267971 bridgeql-0.2.1/
--rw-r--r--   0 priyanksi   (501) staff       (20)     1512 2023-03-23 06:35:39.000000 bridgeql-0.2.1/LICENSE
--rw-r--r--   0 priyanksi   (501) staff       (20)      403 2023-03-17 14:43:32.000000 bridgeql-0.2.1/NOTICE
--rw-r--r--   0 priyanksi   (501) staff       (20)     6636 2023-05-19 13:51:20.267564 bridgeql-0.2.1/PKG-INFO
--rw-r--r--   0 priyanksi   (501) staff       (20)     5457 2023-05-16 11:17:14.000000 bridgeql-0.2.1/README.md
-drwxr-xr-x   0 priyanksi   (501) staff       (20)        0 2023-05-19 13:51:20.255346 bridgeql-0.2.1/bridgeql/
--rw-r--r--   0 priyanksi   (501) staff       (20)      647 2023-05-19 11:26:04.000000 bridgeql-0.2.1/bridgeql/__init__.py
-drwxr-xr-x   0 priyanksi   (501) staff       (20)        0 2023-05-19 13:51:20.265448 bridgeql-0.2.1/bridgeql/django/
--rw-r--r--   0 priyanksi   (501) staff       (20)      173 2023-04-18 04:55:32.000000 bridgeql-0.2.1/bridgeql/django/__init__.py
--rw-r--r--   0 priyanksi   (501) staff       (20)     1391 2023-05-16 11:17:14.000000 bridgeql-0.2.1/bridgeql/django/auth.py
--rw-r--r--   0 priyanksi   (501) staff       (20)     3309 2023-05-19 11:26:04.000000 bridgeql-0.2.1/bridgeql/django/bridge.py
--rw-r--r--   0 priyanksi   (501) staff       (20)     1269 2023-05-16 11:17:14.000000 bridgeql-0.2.1/bridgeql/django/exceptions.py
--rw-r--r--   0 priyanksi   (501) staff       (20)      749 2023-05-04 09:12:29.000000 bridgeql-0.2.1/bridgeql/django/fields.py
--rw-r--r--   0 priyanksi   (501) staff       (20)     2293 2023-05-16 11:17:14.000000 bridgeql-0.2.1/bridgeql/django/helpers.py
--rw-r--r--   0 priyanksi   (501) staff       (20)    13017 2023-05-19 11:26:31.000000 bridgeql-0.2.1/bridgeql/django/models.py
--rw-r--r--   0 priyanksi   (501) staff       (20)     1405 2023-05-04 09:12:29.000000 bridgeql-0.2.1/bridgeql/django/query.py
--rw-r--r--   0 priyanksi   (501) staff       (20)     1040 2023-05-04 09:12:29.000000 bridgeql-0.2.1/bridgeql/django/schema.py
--rw-r--r--   0 priyanksi   (501) staff       (20)     3598 2023-05-16 11:46:14.000000 bridgeql-0.2.1/bridgeql/django/settings.py
--rw-r--r--   0 priyanksi   (501) staff       (20)     1312 2023-05-19 11:26:04.000000 bridgeql-0.2.1/bridgeql/django/urls.py
--rw-r--r--   0 priyanksi   (501) staff       (20)     1700 2023-05-04 09:12:29.000000 bridgeql-0.2.1/bridgeql/django/views.py
-drwxr-xr-x   0 priyanksi   (501) staff       (20)        0 2023-05-19 13:51:20.251021 bridgeql-0.2.1/bridgeql/templates/
-drwxr-xr-x   0 priyanksi   (501) staff       (20)        0 2023-05-19 13:51:20.267176 bridgeql-0.2.1/bridgeql/templates/bridgeql/
--rw-r--r--   0 priyanksi   (501) staff       (20)      504 2023-04-18 14:44:49.000000 bridgeql-0.2.1/bridgeql/templates/bridgeql/index.html
--rw-r--r--   0 priyanksi   (501) staff       (20)     2308 2023-05-04 09:12:29.000000 bridgeql-0.2.1/bridgeql/templates/bridgeql/schema.html
--rw-r--r--   0 priyanksi   (501) staff       (20)      221 2023-05-04 09:12:29.000000 bridgeql-0.2.1/bridgeql/types.py
--rw-r--r--   0 priyanksi   (501) staff       (20)     1459 2023-04-03 10:34:25.000000 bridgeql-0.2.1/bridgeql/utils.py
-drwxr-xr-x   0 priyanksi   (501) staff       (20)        0 2023-05-19 13:51:20.257640 bridgeql-0.2.1/bridgeql.egg-info/
--rw-rw-rw-   0 priyanksi   (501) staff       (20)     6636 2023-05-19 13:51:20.000000 bridgeql-0.2.1/bridgeql.egg-info/PKG-INFO
--rw-rw-rw-   0 priyanksi   (501) staff       (20)      627 2023-05-19 13:51:20.000000 bridgeql-0.2.1/bridgeql.egg-info/SOURCES.txt
--rw-rw-rw-   0 priyanksi   (501) staff       (20)        1 2023-05-19 13:51:20.000000 bridgeql-0.2.1/bridgeql.egg-info/dependency_links.txt
--rw-rw-rw-   0 priyanksi   (501) staff       (20)        9 2023-05-19 13:51:20.000000 bridgeql-0.2.1/bridgeql.egg-info/top_level.txt
--rw-r--r--   0 priyanksi   (501) staff       (20)       84 2023-03-17 14:43:32.000000 bridgeql-0.2.1/pyproject.toml
--rw-r--r--   0 priyanksi   (501) staff       (20)       38 2023-05-19 13:51:20.268018 bridgeql-0.2.1/setup.cfg
--rw-r--r--   0 priyanksi   (501) staff       (20)     1789 2023-04-06 17:49:48.000000 bridgeql-0.2.1/setup.py
+drwxr-xr-x   0 piyusk     (502) staff       (20)        0 2023-08-02 11:01:15.652611 bridgeql-0.2.2/
+-rw-r--r--   0 piyusk     (502) staff       (20)     1512 2023-04-18 14:03:59.000000 bridgeql-0.2.2/LICENSE
+-rw-r--r--   0 piyusk     (502) staff       (20)      403 2023-04-18 14:03:59.000000 bridgeql-0.2.2/NOTICE
+-rw-r--r--   0 piyusk     (502) staff       (20)     6800 2023-08-02 11:01:15.651239 bridgeql-0.2.2/PKG-INFO
+-rw-r--r--   0 piyusk     (502) staff       (20)     5621 2023-05-24 13:19:47.000000 bridgeql-0.2.2/README.md
+drwxr-xr-x   0 piyusk     (502) staff       (20)        0 2023-08-02 11:01:15.629947 bridgeql-0.2.2/bridgeql/
+-rw-r--r--   0 piyusk     (502) staff       (20)      647 2023-05-24 13:19:47.000000 bridgeql-0.2.2/bridgeql/__init__.py
+drwxr-xr-x   0 piyusk     (502) staff       (20)        0 2023-08-02 11:01:15.645902 bridgeql-0.2.2/bridgeql/django/
+-rw-r--r--   0 piyusk     (502) staff       (20)      173 2023-04-18 14:03:59.000000 bridgeql-0.2.2/bridgeql/django/__init__.py
+-rw-r--r--   0 piyusk     (502) staff       (20)     1391 2023-05-18 11:09:44.000000 bridgeql-0.2.2/bridgeql/django/auth.py
+-rw-r--r--   0 piyusk     (502) staff       (20)     3309 2023-05-19 10:40:24.000000 bridgeql-0.2.2/bridgeql/django/bridge.py
+-rw-r--r--   0 piyusk     (502) staff       (20)     1269 2023-05-18 11:09:44.000000 bridgeql-0.2.2/bridgeql/django/exceptions.py
+-rw-r--r--   0 piyusk     (502) staff       (20)      749 2023-04-27 11:57:21.000000 bridgeql-0.2.2/bridgeql/django/fields.py
+-rw-r--r--   0 piyusk     (502) staff       (20)     2293 2023-05-18 11:09:44.000000 bridgeql-0.2.2/bridgeql/django/helpers.py
+-rw-r--r--   0 piyusk     (502) staff       (20)    13008 2023-05-24 13:19:47.000000 bridgeql-0.2.2/bridgeql/django/models.py
+-rw-r--r--   0 piyusk     (502) staff       (20)     1405 2023-04-27 11:57:21.000000 bridgeql-0.2.2/bridgeql/django/query.py
+-rw-r--r--   0 piyusk     (502) staff       (20)     1040 2023-04-27 11:57:21.000000 bridgeql-0.2.2/bridgeql/django/schema.py
+-rw-r--r--   0 piyusk     (502) staff       (20)     3598 2023-05-18 11:09:44.000000 bridgeql-0.2.2/bridgeql/django/settings.py
+-rw-r--r--   0 piyusk     (502) staff       (20)     1325 2023-08-02 11:00:26.000000 bridgeql-0.2.2/bridgeql/django/urls.py
+-rw-r--r--   0 piyusk     (502) staff       (20)     1700 2023-04-27 11:57:21.000000 bridgeql-0.2.2/bridgeql/django/views.py
+drwxr-xr-x   0 piyusk     (502) staff       (20)        0 2023-08-02 11:01:15.623405 bridgeql-0.2.2/bridgeql/templates/
+drwxr-xr-x   0 piyusk     (502) staff       (20)        0 2023-08-02 11:01:15.648799 bridgeql-0.2.2/bridgeql/templates/bridgeql/
+-rw-r--r--   0 piyusk     (502) staff       (20)      504 2023-04-18 14:03:59.000000 bridgeql-0.2.2/bridgeql/templates/bridgeql/index.html
+-rw-r--r--   0 piyusk     (502) staff       (20)     2308 2023-04-27 11:57:21.000000 bridgeql-0.2.2/bridgeql/templates/bridgeql/schema.html
+-rw-r--r--   0 piyusk     (502) staff       (20)      221 2023-04-27 11:57:21.000000 bridgeql-0.2.2/bridgeql/types.py
+-rw-r--r--   0 piyusk     (502) staff       (20)     1459 2023-04-18 14:03:59.000000 bridgeql-0.2.2/bridgeql/utils.py
+drwxr-xr-x   0 piyusk     (502) staff       (20)        0 2023-08-02 11:01:15.633568 bridgeql-0.2.2/bridgeql.egg-info/
+-rw-rw-rw-   0 piyusk     (502) staff       (20)     6800 2023-08-02 11:01:15.000000 bridgeql-0.2.2/bridgeql.egg-info/PKG-INFO
+-rw-rw-rw-   0 piyusk     (502) staff       (20)      627 2023-08-02 11:01:15.000000 bridgeql-0.2.2/bridgeql.egg-info/SOURCES.txt
+-rw-rw-rw-   0 piyusk     (502) staff       (20)        1 2023-08-02 11:01:15.000000 bridgeql-0.2.2/bridgeql.egg-info/dependency_links.txt
+-rw-rw-rw-   0 piyusk     (502) staff       (20)        9 2023-08-02 11:01:15.000000 bridgeql-0.2.2/bridgeql.egg-info/top_level.txt
+-rw-r--r--   0 piyusk     (502) staff       (20)       84 2023-04-18 14:03:59.000000 bridgeql-0.2.2/pyproject.toml
+-rw-r--r--   0 piyusk     (502) staff       (20)       38 2023-08-02 11:01:15.652917 bridgeql-0.2.2/setup.cfg
+-rw-r--r--   0 piyusk     (502) staff       (20)     1789 2023-04-18 14:03:59.000000 bridgeql-0.2.2/setup.py
```

### Comparing `bridgeql-0.2.1/LICENSE` & `bridgeql-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/PKG-INFO` & `bridgeql-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: bridgeql
-Version: 0.2.1
+Version: 0.2.2
 Summary: Query language to bridge the gap between REST API and ORM capability
 Home-page: https://github.com/vmware/bridgeql
 Author: Piyus Kumar
 Author-email: piyusk@vmware.com
 License: BSD-2
 Project-URL: Bug Tracker, https://github.com/vmware/bridgeql/issues
 Keywords: django
 Platform: Any
-Classifier: Framework :: Django :: 1.11
-Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django :: 4.1
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django :: 3.2
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Framework :: Django :: 2.2
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Framework :: Django :: 4.1
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Framework :: Django :: 1.11
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # BridgeQL
 
@@ -88,40 +88,48 @@
 urlpatterns = [
     ...
     path('api/bridgeql/', include(bridgeql_urls)),
     ...
 ]
 ...
 ```
-This way your app will be ready to serve the REST API to expose model query, you can request an API like follows:
+This way your app will be ready to serve the REST API to expose model query, you can request the API
+to perform basic CRUD operations using one of the following URLs
+- Create: `create/db_name/app_name/model_name`
+- Read: `read/db_name/app_name/model_name/<?pk>`
+- Update: `update/db_name/app_name/model_name/pk`
+- Delete: `delete/db_name/app_name/model_name/pk`
+
+Example Usage:
+
 ```python
-    params = {
-       'db_name': 'db1',
-       'app_name': 'machine', # required
-       'model_name': 'Machine', # required
-       'filter': {
-           'os__name': 'os-name-1'
-        },
-        'fields': ['ip', 'name', 'id'],
-        'exclude': {
-           'name': 'machine-name-11'
-        },
-        'order_by': ['ip'],
-        'limit': 5,
-        'offset': 10, # default 0
-    }
-    api_url = '<yoursite.com>/api/bridgeql/dj_read'
-    resp = make_get_api_call(api_url, {'payload': json.dumps(params)})
-    result = resp.json()
+import requests
+
+params = {
+    'filter': {
+        'os__name': 'os-name-1'
+    },
+    'fields': ['ip', 'name', 'id'],
+    'exclude': {
+        'name': 'machine-name-11'
+    },
+    'order_by': ['ip'],
+    'limit': 5,
+    'offset': 10,  # default 0
+}
+# db_name could be default
+api_url = '<yoursite.com>/api/bridgeql/read/default/machine/Machine'
+resp = requests.get(api_url, {'payload': json.dumps(params)})
+result = resp.json()
 ```
 
 The above parameters will translate into running the model query for `Machine` model of `machine` django app.
 
 ```python
-Machine.objects.using('db1')
+Machine.objects.using('default')
                 .filter(os__name = 'os-name-1')
                 .exclude(name = 'machine-name-11')
                 .values(['ip', 'name', 'id'])
                 .order_by('ip')[10:15] # offset: offset + limit
 ```
 
 ____
```

### Comparing `bridgeql-0.2.1/README.md` & `bridgeql-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -56,40 +56,48 @@
 urlpatterns = [
     ...
     path('api/bridgeql/', include(bridgeql_urls)),
     ...
 ]
 ...
 ```
-This way your app will be ready to serve the REST API to expose model query, you can request an API like follows:
+This way your app will be ready to serve the REST API to expose model query, you can request the API
+to perform basic CRUD operations using one of the following URLs
+- Create: `create/db_name/app_name/model_name`
+- Read: `read/db_name/app_name/model_name/<?pk>`
+- Update: `update/db_name/app_name/model_name/pk`
+- Delete: `delete/db_name/app_name/model_name/pk`
+
+Example Usage:
+
 ```python
-    params = {
-       'db_name': 'db1',
-       'app_name': 'machine', # required
-       'model_name': 'Machine', # required
-       'filter': {
-           'os__name': 'os-name-1'
-        },
-        'fields': ['ip', 'name', 'id'],
-        'exclude': {
-           'name': 'machine-name-11'
-        },
-        'order_by': ['ip'],
-        'limit': 5,
-        'offset': 10, # default 0
-    }
-    api_url = '<yoursite.com>/api/bridgeql/dj_read'
-    resp = make_get_api_call(api_url, {'payload': json.dumps(params)})
-    result = resp.json()
+import requests
+
+params = {
+    'filter': {
+        'os__name': 'os-name-1'
+    },
+    'fields': ['ip', 'name', 'id'],
+    'exclude': {
+        'name': 'machine-name-11'
+    },
+    'order_by': ['ip'],
+    'limit': 5,
+    'offset': 10,  # default 0
+}
+# db_name could be default
+api_url = '<yoursite.com>/api/bridgeql/read/default/machine/Machine'
+resp = requests.get(api_url, {'payload': json.dumps(params)})
+result = resp.json()
 ```
 
 The above parameters will translate into running the model query for `Machine` model of `machine` django app.
 
 ```python
-Machine.objects.using('db1')
+Machine.objects.using('default')
                 .filter(os__name = 'os-name-1')
                 .exclude(name = 'machine-name-11')
                 .values(['ip', 'name', 'id'])
                 .order_by('ip')[10:15] # offset: offset + limit
 ```
 
 ____
```

### Comparing `bridgeql-0.2.1/bridgeql/__init__.py` & `bridgeql-0.2.2/bridgeql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
  | |_) | |  | | (_| | (_| |  __/ |__| | |____
  |____/|_|  |_|\__,_|\__, |\___|\___\_\______|
                       __/ |
                      |___/
 """
 
 __title__ = 'BridgeQL'
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 __license__ = 'BSD 2-Clause'
 __copyright__ = 'Copyright © 2023 VMware, Inc.  All rights reserved.'
 
 # VERSION available outside module
 VERSION = __version__
```

### Comparing `bridgeql-0.2.1/bridgeql/django/auth.py` & `bridgeql-0.2.2/bridgeql/django/auth.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/bridgeql/django/bridge.py` & `bridgeql-0.2.2/bridgeql/django/bridge.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/bridgeql/django/exceptions.py` & `bridgeql-0.2.2/bridgeql/django/exceptions.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/bridgeql/django/fields.py` & `bridgeql-0.2.2/bridgeql/django/fields.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/bridgeql/django/helpers.py` & `bridgeql-0.2.2/bridgeql/django/helpers.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/bridgeql/django/models.py` & `bridgeql-0.2.2/bridgeql/django/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,32 +173,32 @@
             for key, val in params.items():
                 if hasattr(self.instance, key):
                     setattr(self.instance, key, val)
                 else:
                     raise InvalidRequest('%s does not have field %s'
                                          % (self.instance._meta.model.__name__,
                                             key))
-                setattr(self.instance, key, val)
             # Perform validation
             self.instance.validate_unique()
             self.instance.save()
-        except (ValidationError, IntegrityError, AttributeError) as e:
+        except (AttributeError, IntegrityError,
+                ValidationError, ValueError) as e:
             raise InvalidRequest(str(e))
         return self.instance
 
     def create(self, params):
         # TODO validate data
         save_kwargs = {'using': self.db_name}
         # if db_name is None then save() function will use default db
         self.instance = self.model_config.model(**params)
         # Perform validation
         try:
             self.instance.validate_unique()
             self.instance.save(**save_kwargs)
-        except (ValidationError, IntegrityError) as e:
+        except (IntegrityError, ValidationError, ValueError) as e:
             raise InvalidRequest(str(e))
         return self.instance
 
     def delete(self):
         return self.instance.delete()
```

### Comparing `bridgeql-0.2.1/bridgeql/django/query.py` & `bridgeql-0.2.2/bridgeql/django/query.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/bridgeql/django/schema.py` & `bridgeql-0.2.2/bridgeql/django/schema.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/bridgeql/django/settings.py` & `bridgeql-0.2.2/bridgeql/django/settings.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/bridgeql/django/urls.py` & `bridgeql-0.2.2/bridgeql/django/urls.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2023 VMware, Inc.  All rights reserved.
 # SPDX-License-Identifier: BSD-2-Clause
-
 try:
-    from django.urls import path
+    from django.urls import re_path as url
 except ImportError:
-    from django.conf.urls import url as path
+    from django.conf.urls import url
 
 from bridgeql.django import bridge
 from bridgeql.django.settings import bridgeql_settings
 from bridgeql.django.views import index, generate_bridgeql_schema
 
 bridgeql_settings.validate()
 
 urlpatterns = [
-    path('create/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/',
+    url(r'^create/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/$',
          bridge.create_django_model, name='bridgeql_django_create'),
-    path('read/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/(?P<pk>\w+)/',
+    url(r'^read/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/(?P<pk>\w+)/$',
          bridge.read_django_model, name='bridgeql_django_read_pk'),
-    path('read/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/',
+    url(r'^read/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/$',
          bridge.read_django_model, name='bridgeql_django_read'),
-    path('update/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/(?P<pk>\w+)/',
+    url(r'^update/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/(?P<pk>\w+)/$',
          bridge.update_django_model, name='bridgeql_django_update'),
-    path('delete/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/(?P<pk>\w+)/',
+    url(r'^delete/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/(?P<pk>\w+)/$',
          bridge.delete_django_model, name='bridgeql_django_delete'),
-    path('schema/', generate_bridgeql_schema, name='generate_bridgeql_schema'),
-    path('', index, name='bridgeql_django_index'),
+    url(r'^schema/$', generate_bridgeql_schema, name='generate_bridgeql_schema'),
+    url(r'', index, name='bridgeql_django_index'),
 ]
```

### Comparing `bridgeql-0.2.1/bridgeql/django/views.py` & `bridgeql-0.2.2/bridgeql/django/views.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/bridgeql/templates/bridgeql/schema.html` & `bridgeql-0.2.2/bridgeql/templates/bridgeql/schema.html`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/bridgeql/utils.py` & `bridgeql-0.2.2/bridgeql/utils.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/bridgeql.egg-info/PKG-INFO` & `bridgeql-0.2.2/bridgeql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: bridgeql
-Version: 0.2.1
+Version: 0.2.2
 Summary: Query language to bridge the gap between REST API and ORM capability
 Home-page: https://github.com/vmware/bridgeql
 Author: Piyus Kumar
 Author-email: piyusk@vmware.com
 License: BSD-2
 Project-URL: Bug Tracker, https://github.com/vmware/bridgeql/issues
 Keywords: django
 Platform: Any
-Classifier: Framework :: Django :: 1.11
-Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django :: 4.1
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django :: 3.2
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Framework :: Django :: 2.2
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Framework :: Django :: 4.1
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Framework :: Django :: 1.11
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # BridgeQL
 
@@ -88,40 +88,48 @@
 urlpatterns = [
     ...
     path('api/bridgeql/', include(bridgeql_urls)),
     ...
 ]
 ...
 ```
-This way your app will be ready to serve the REST API to expose model query, you can request an API like follows:
+This way your app will be ready to serve the REST API to expose model query, you can request the API
+to perform basic CRUD operations using one of the following URLs
+- Create: `create/db_name/app_name/model_name`
+- Read: `read/db_name/app_name/model_name/<?pk>`
+- Update: `update/db_name/app_name/model_name/pk`
+- Delete: `delete/db_name/app_name/model_name/pk`
+
+Example Usage:
+
 ```python
-    params = {
-       'db_name': 'db1',
-       'app_name': 'machine', # required
-       'model_name': 'Machine', # required
-       'filter': {
-           'os__name': 'os-name-1'
-        },
-        'fields': ['ip', 'name', 'id'],
-        'exclude': {
-           'name': 'machine-name-11'
-        },
-        'order_by': ['ip'],
-        'limit': 5,
-        'offset': 10, # default 0
-    }
-    api_url = '<yoursite.com>/api/bridgeql/dj_read'
-    resp = make_get_api_call(api_url, {'payload': json.dumps(params)})
-    result = resp.json()
+import requests
+
+params = {
+    'filter': {
+        'os__name': 'os-name-1'
+    },
+    'fields': ['ip', 'name', 'id'],
+    'exclude': {
+        'name': 'machine-name-11'
+    },
+    'order_by': ['ip'],
+    'limit': 5,
+    'offset': 10,  # default 0
+}
+# db_name could be default
+api_url = '<yoursite.com>/api/bridgeql/read/default/machine/Machine'
+resp = requests.get(api_url, {'payload': json.dumps(params)})
+result = resp.json()
 ```
 
 The above parameters will translate into running the model query for `Machine` model of `machine` django app.
 
 ```python
-Machine.objects.using('db1')
+Machine.objects.using('default')
                 .filter(os__name = 'os-name-1')
                 .exclude(name = 'machine-name-11')
                 .values(['ip', 'name', 'id'])
                 .order_by('ip')[10:15] # offset: offset + limit
 ```
 
 ____
```

### Comparing `bridgeql-0.2.1/bridgeql.egg-info/SOURCES.txt` & `bridgeql-0.2.2/bridgeql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.1/setup.py` & `bridgeql-0.2.2/setup.py`

 * *Files identical despite different names*

