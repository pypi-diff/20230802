# Comparing `tmp/django_nats_client-0.4.1.tar.gz` & `tmp/django_nats_client-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_nats_client-0.4.1.tar", max compression
+gzip compressed data, was "django_nats_client-0.4.2.tar", max compression
```

## Comparing `django_nats_client-0.4.1.tar` & `django_nats_client-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/LICENSE
--rw-r--r--   0        0        0     6037 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/README.md
--rw-r--r--   0        0        0       79 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/__init__.py
--rw-r--r--   0        0        0       96 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/apps.py
--rw-r--r--   0        0        0     2246 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/clients.py
--rw-r--r--   0        0        0      114 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/exceptions.py
--rw-r--r--   0        0        0      473 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/handlers.py
--rw-r--r--   0        0        0     5545 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/management/commands/nats_listener.py
--rw-r--r--   0        0        0     1336 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/registry.py
--rw-r--r--   0        0        0       84 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/types.py
--rw-r--r--   0        0        0      849 2023-06-10 19:35:53.608993 django_nats_client-0.4.1/nats_client/utils.py
--rw-r--r--   0        0        0      901 2023-06-10 19:36:07.825202 django_nats_client-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6805 1970-01-01 00:00:00.000000 django_nats_client-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-02 08:30:10.599753 django_nats_client-0.4.2/LICENSE
+-rw-r--r--   0        0        0     6037 2023-08-02 08:30:10.599753 django_nats_client-0.4.2/README.md
+-rw-r--r--   0        0        0       79 2023-08-02 08:30:10.599753 django_nats_client-0.4.2/nats_client/__init__.py
+-rw-r--r--   0        0        0       96 2023-08-02 08:30:10.599753 django_nats_client-0.4.2/nats_client/apps.py
+-rw-r--r--   0        0        0     2246 2023-08-02 08:30:10.599753 django_nats_client-0.4.2/nats_client/clients.py
+-rw-r--r--   0        0        0      114 2023-08-02 08:30:10.599753 django_nats_client-0.4.2/nats_client/exceptions.py
+-rw-r--r--   0        0        0      473 2023-08-02 08:30:10.599753 django_nats_client-0.4.2/nats_client/handlers.py
+-rw-r--r--   0        0        0     5495 2023-08-02 08:30:10.599753 django_nats_client-0.4.2/nats_client/management/commands/nats_listener.py
+-rw-r--r--   0        0        0     1336 2023-08-02 08:30:10.599753 django_nats_client-0.4.2/nats_client/registry.py
+-rw-r--r--   0        0        0       84 2023-08-02 08:30:10.599753 django_nats_client-0.4.2/nats_client/types.py
+-rw-r--r--   0        0        0      849 2023-08-02 08:30:10.599753 django_nats_client-0.4.2/nats_client/utils.py
+-rw-r--r--   0        0        0      901 2023-08-02 08:30:37.683870 django_nats_client-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6805 1970-01-01 00:00:00.000000 django_nats_client-0.4.2/PKG-INFO
```

### Comparing `django_nats_client-0.4.1/LICENSE` & `django_nats_client-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_nats_client-0.4.1/README.md` & `django_nats_client-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `django_nats_client-0.4.1/nats_client/clients.py` & `django_nats_client-0.4.2/nats_client/clients.py`

 * *Files identical despite different names*

### Comparing `django_nats_client-0.4.1/nats_client/management/commands/nats_listener.py` & `django_nats_client-0.4.2/nats_client/management/commands/nats_listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
 import json
-import traceback
 
 import jsonpickle
 import nats.errors
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.core.management import BaseCommand
 from django.core.serializers.json import DjangoJSONEncoder
@@ -126,15 +125,14 @@
             print(f'     - {full_name}' + (' (JetStream)' if data['js'] else ''))
 
     async def handler(self, func_name: str, body, reply=None):
         try:
             data = json.loads(body)
             r = await nats_handler(func_name, data)
         except Exception as e:  # pylint: disable=broad-except
-            traceback.print_exc()
             if reply:
                 if isinstance(e, ValidationError):
                     message = e.message_dict
                 else:
                     message = str(e)
                     try:
                         message = json.loads(message)
@@ -146,11 +144,11 @@
                     json.dumps({
                         'success': False,
                         'error': e.__class__.__name__,
                         'message': message,
                         'pickled_exc': jsonpickle.encode(e),
                     }).encode()
                 )
-            return
+            raise e
 
         if reply:
             await self.nats.publish(reply, json.dumps({'success': True, 'result': r}, cls=DjangoJSONEncoder).encode())
```

### Comparing `django_nats_client-0.4.1/nats_client/registry.py` & `django_nats_client-0.4.2/nats_client/registry.py`

 * *Files identical despite different names*

### Comparing `django_nats_client-0.4.1/nats_client/utils.py` & `django_nats_client-0.4.2/nats_client/utils.py`

 * *Files identical despite different names*

### Comparing `django_nats_client-0.4.1/pyproject.toml` & `django_nats_client-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-nats-client"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["CODIUM <support@codium.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/C0D1UM/django-nats-client"
 keywords = ["django", "nats", "listener", "python"]
 packages = [
```

### Comparing `django_nats_client-0.4.1/PKG-INFO` & `django_nats_client-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nats-client
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Home-page: https://github.com/C0D1UM/django-nats-client
 License: MIT
 Keywords: django,nats,listener,python
 Author: CODIUM
 Author-email: support@codium.co
 Requires-Python: >=3.8,<4.0
```

