# Comparing `tmp/i_saas_utils-0.1.2.tar.gz` & `tmp/i_saas_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i_saas_utils-0.1.2.tar", max compression
+gzip compressed data, was "i_saas_utils-0.1.3.tar", max compression
```

## Comparing `i_saas_utils-0.1.2.tar` & `i_saas_utils-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     6254 2023-07-28 20:15:16.157658 i_saas_utils-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-28 15:49:56.000000 i_saas_utils-0.1.2/i_saas_utils/__init__.py
--rw-r--r--   0        0        0       28 2023-07-29 11:00:00.646286 i_saas_utils-0.1.2/i_saas_utils/ansible/__init__.py
--rw-r--r--   0        0        0      517 2023-07-29 11:08:59.134950 i_saas_utils-0.1.2/i_saas_utils/ansible/ansibl.py
--rw-r--r--   0        0        0       30 2023-07-29 14:27:09.403296 i_saas_utils-0.1.2/i_saas_utils/git/__init__.py
--rw-r--r--   0        0        0      680 2023-07-29 19:49:55.616690 i_saas_utils-0.1.2/i_saas_utils/git/git.py
--rw-r--r--   0        0        0     1297 2023-07-29 19:49:55.604690 i_saas_utils-0.1.2/i_saas_utils/git/project.py
--rw-r--r--   0        0        0       23 2023-07-29 11:01:01.438716 i_saas_utils-0.1.2/i_saas_utils/k8s/__init__.py
--rw-r--r--   0        0        0      916 2023-07-28 21:36:56.880915 i_saas_utils-0.1.2/i_saas_utils/k8s/kube.py
--rw-r--r--   0        0        0      134 2023-07-29 16:20:21.734883 i_saas_utils-0.1.2/i_saas_utils/saas/__init__.py
--rw-r--r--   0        0        0     3013 2023-08-01 18:30:59.609803 i_saas_utils-0.1.2/i_saas_utils/saas/saas.py
--rw-r--r--   0        0        0       57 2023-07-29 11:01:01.418716 i_saas_utils-0.1.2/i_saas_utils/templates/__init__.py
--rw-r--r--   0        0        0      646 2023-07-29 19:49:55.600690 i_saas_utils-0.1.2/i_saas_utils/templates/render.py
--rw-r--r--   0        0        0       71 2023-07-29 11:01:59.506737 i_saas_utils-0.1.2/i_saas_utils/types/__init__.py
--rw-r--r--   0        0        0      386 2023-08-01 18:31:21.538258 i_saas_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 i_saas_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6254 2023-07-28 20:15:16.157658 i_saas_utils-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 15:49:56.000000 i_saas_utils-0.1.3/i_saas_utils/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-29 11:00:00.646286 i_saas_utils-0.1.3/i_saas_utils/ansible/__init__.py
+-rw-r--r--   0        0        0      517 2023-07-29 11:08:59.134950 i_saas_utils-0.1.3/i_saas_utils/ansible/ansibl.py
+-rw-r--r--   0        0        0       87 2023-08-01 22:29:40.238936 i_saas_utils-0.1.3/i_saas_utils/git/__init__.py
+-rw-r--r--   0        0        0      494 2023-08-01 22:31:19.215972 i_saas_utils-0.1.3/i_saas_utils/git/git.py
+-rw-r--r--   0        0        0     1334 2023-08-01 22:52:52.330515 i_saas_utils-0.1.3/i_saas_utils/git/git_project.py
+-rw-r--r--   0        0        0     1297 2023-08-01 22:48:40.753722 i_saas_utils-0.1.3/i_saas_utils/git/git_repo.py
+-rw-r--r--   0        0        0       23 2023-07-29 11:01:01.438716 i_saas_utils-0.1.3/i_saas_utils/k8s/__init__.py
+-rw-r--r--   0        0        0      916 2023-07-28 21:36:56.880915 i_saas_utils-0.1.3/i_saas_utils/k8s/kube.py
+-rw-r--r--   0        0        0      148 2023-08-02 08:31:41.871839 i_saas_utils-0.1.3/i_saas_utils/saas/__init__.py
+-rw-r--r--   0        0        0     3038 2023-08-01 22:33:55.601333 i_saas_utils-0.1.3/i_saas_utils/saas/saas.py
+-rw-r--r--   0        0        0       57 2023-07-29 11:01:01.418716 i_saas_utils-0.1.3/i_saas_utils/templates/__init__.py
+-rw-r--r--   0        0        0      646 2023-07-29 19:49:55.600690 i_saas_utils-0.1.3/i_saas_utils/templates/render.py
+-rw-r--r--   0        0        0       71 2023-07-29 11:01:59.506737 i_saas_utils-0.1.3/i_saas_utils/types/__init__.py
+-rw-r--r--   0        0        0      386 2023-08-02 08:31:41.863839 i_saas_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 i_saas_utils-0.1.3/PKG-INFO
```

### Comparing `i_saas_utils-0.1.2/README.md` & `i_saas_utils-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.2/i_saas_utils/ansible/ansibl.py` & `i_saas_utils-0.1.3/i_saas_utils/ansible/ansibl.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.2/i_saas_utils/git/project.py` & `i_saas_utils-0.1.3/i_saas_utils/git/git_repo.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.2/i_saas_utils/k8s/kube.py` & `i_saas_utils-0.1.3/i_saas_utils/k8s/kube.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.2/i_saas_utils/saas/saas.py` & `i_saas_utils-0.1.3/i_saas_utils/saas/saas.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import sys
 import urllib.parse
-from importlib import import_module
 from random import shuffle
+import runpy
 
 import dns.resolver
 import requests
 
 
 def get_list_dirs(path: str):
     return [d for d in os.listdir(path) if os.path.isdir(os.path.join(path, d))]
@@ -26,33 +26,35 @@
     return list_files
 
 
 def choice_action(
     action: str = None,
     data: dict | None = None,
     path: str = "actions",
-    file_name: str = "main",
+    file_name: str = "main.py",
     function_name: str = "main",
 ):
     if action is None:
         if len(sys.argv) == 1:
             raise Exception("Action not found")
         action = sys.argv[1]
     if data is None:
         data = os.getenv("SAAS_DATA")
         if not data:
             raise Exception("Data not found")
         data = json.loads(data)
 
-    list_dirs = get_list_dirs(path)
+    list_actions = get_list_dirs(path)
+    if action not in list_actions:
+        raise Exception(f"ERROR POSSIBLE ACTION {list_actions}")
 
-    if action in list_dirs:
-        import_module(f"{action}.{file_name}").__getattr__(function_name)(data)
-    else:
-        raise Exception(f"ERROR POSSIBLE ACTION {list_dirs}")
+    module = runpy.run_path(os.path.join(path, action, file_name))
+    module.get(function_name)(data)
+
+    return module
 
 
 def check_exists_hostname(hostname: str, is_url: bool = False):
     if is_url:
         parsed_url = urllib.parse.urlparse(hostname)
         hostname = parsed_url.hostname
     try:
```

### Comparing `i_saas_utils-0.1.2/i_saas_utils/templates/render.py` & `i_saas_utils-0.1.3/i_saas_utils/templates/render.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.2/PKG-INFO` & `i_saas_utils-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i-saas-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Fedorov Stepan
 Author-email: fedorov.stepan2@wb.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dnspython (>=2.4.1,<3.0.0)
```

