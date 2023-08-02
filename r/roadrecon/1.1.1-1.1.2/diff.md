# Comparing `tmp/roadrecon-1.1.1.tar.gz` & `tmp/roadrecon-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roadrecon-1.1.1.tar", last modified: Fri Jun  9 08:05:49 2023, max compression
+gzip compressed data, was "roadrecon-1.1.2.tar", last modified: Wed Aug  2 13:30:49 2023, max compression
```

## Comparing `roadrecon-1.1.1.tar` & `roadrecon-1.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-09 08:05:49.125740 roadrecon-1.1.1/
--rw-r--r--   0 vsts      (1001) docker     (123)       85 2023-06-09 08:04:18.000000 roadrecon-1.1.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      622 2023-06-09 08:05:49.125740 roadrecon-1.1.1/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-09 08:05:49.121740 roadrecon-1.1.1/roadrecon.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      622 2023-06-09 08:05:49.000000 roadrecon-1.1.1/roadrecon.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-06-09 08:05:49.000000 roadrecon-1.1.1/roadrecon.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-09 08:05:49.000000 roadrecon-1.1.1/roadrecon.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-09 08:05:49.000000 roadrecon-1.1.1/roadrecon.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-09 08:05:47.000000 roadrecon-1.1.1/roadrecon.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      142 2023-06-09 08:05:49.000000 roadrecon-1.1.1/roadrecon.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-06-09 08:05:49.000000 roadrecon-1.1.1/roadrecon.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-09 08:05:49.121740 roadrecon-1.1.1/roadtools/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-09 08:05:49.121740 roadrecon-1.1.1/roadtools/roadrecon/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-09 08:04:18.000000 roadrecon-1.1.1/roadtools/roadrecon/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-09 08:05:49.125740 roadrecon-1.1.1/roadtools/roadrecon/dist_gui/
--rw-r--r--   0 vsts      (1001) docker     (123)    16301 2023-06-09 08:05:26.000000 roadrecon-1.1.1/roadtools/roadrecon/dist_gui/3rdpartylicenses.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-09 08:05:49.125740 roadrecon-1.1.1/roadtools/roadrecon/dist_gui/assets/
--rw-r--r--   0 vsts      (1001) docker     (123)     2191 2023-06-09 08:05:28.000000 roadrecon-1.1.1/roadtools/roadrecon/dist_gui/assets/roadicon.png
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2955 2023-06-09 08:05:28.000000 roadrecon-1.1.1/roadtools/roadrecon/dist_gui/assets/rt_logoonly_margin.svg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     4164 2023-06-09 08:05:28.000000 roadrecon-1.1.1/roadtools/roadrecon/dist_gui/assets/rt_transparent.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     7437 2023-06-09 08:05:28.000000 roadrecon-1.1.1/roadtools/roadrecon/dist_gui/index.html
--rw-r--r--   0 vsts      (1001) docker     (123)   898232 2023-06-09 08:05:26.000000 roadrecon-1.1.1/roadtools/roadrecon/dist_gui/main.1066d5fe02fb5e54.js
--rw-r--r--   0 vsts      (1001) docker     (123)    37024 2023-06-09 08:05:26.000000 roadrecon-1.1.1/roadtools/roadrecon/dist_gui/polyfills.3434510fb5b4de7e.js
--rw-r--r--   0 vsts      (1001) docker     (123)     1083 2023-06-09 08:05:26.000000 roadrecon-1.1.1/roadtools/roadrecon/dist_gui/runtime.a7446122f8b27a4d.js
--rw-r--r--   0 vsts      (1001) docker     (123)    76259 2023-06-09 08:05:26.000000 roadrecon-1.1.1/roadtools/roadrecon/dist_gui/styles.9afce2c3ef55c87a.css
--rwxr-xr-x   0 vsts      (1001) docker     (123)    31362 2023-06-09 08:04:18.000000 roadrecon-1.1.1/roadtools/roadrecon/gather.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5052 2023-06-09 08:04:18.000000 roadrecon-1.1.1/roadtools/roadrecon/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-09 08:05:49.125740 roadrecon-1.1.1/roadtools/roadrecon/plugins/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-09 08:04:18.000000 roadrecon-1.1.1/roadtools/roadrecon/plugins/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12137 2023-06-09 08:04:18.000000 roadrecon-1.1.1/roadtools/roadrecon/plugins/bloodhound.py
--rw-r--r--   0 vsts      (1001) docker     (123)    20086 2023-06-09 08:04:18.000000 roadrecon-1.1.1/roadtools/roadrecon/plugins/policies.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10032 2023-06-09 08:04:18.000000 roadrecon-1.1.1/roadtools/roadrecon/plugins/road2timeline.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2173 2023-06-09 08:04:18.000000 roadrecon-1.1.1/roadtools/roadrecon/plugins/road2timeline.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)    17455 2023-06-09 08:04:18.000000 roadrecon-1.1.1/roadtools/roadrecon/plugins/xlsexport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    23566 2023-06-09 08:04:18.000000 roadrecon-1.1.1/roadtools/roadrecon/server.py
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-09 08:05:49.125740 roadrecon-1.1.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1404 2023-06-09 08:04:18.000000 roadrecon-1.1.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 13:30:49.871862 roadrecon-1.1.2/
+-rw-r--r--   0 vsts      (1001) docker     (123)       85 2023-08-02 13:29:28.000000 roadrecon-1.1.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      622 2023-08-02 13:30:49.871862 roadrecon-1.1.2/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 13:30:49.871862 roadrecon-1.1.2/roadrecon.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      622 2023-08-02 13:30:49.000000 roadrecon-1.1.2/roadrecon.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-08-02 13:30:49.000000 roadrecon-1.1.2/roadrecon.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-02 13:30:49.000000 roadrecon-1.1.2/roadrecon.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-08-02 13:30:49.000000 roadrecon-1.1.2/roadrecon.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-02 13:30:47.000000 roadrecon-1.1.2/roadrecon.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      142 2023-08-02 13:30:49.000000 roadrecon-1.1.2/roadrecon.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-08-02 13:30:49.000000 roadrecon-1.1.2/roadrecon.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 13:30:49.867862 roadrecon-1.1.2/roadtools/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 13:30:49.871862 roadrecon-1.1.2/roadtools/roadrecon/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-02 13:29:28.000000 roadrecon-1.1.2/roadtools/roadrecon/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 13:30:49.871862 roadrecon-1.1.2/roadtools/roadrecon/dist_gui/
+-rw-r--r--   0 vsts      (1001) docker     (123)    16301 2023-08-02 13:30:28.000000 roadrecon-1.1.2/roadtools/roadrecon/dist_gui/3rdpartylicenses.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 13:30:49.871862 roadrecon-1.1.2/roadtools/roadrecon/dist_gui/assets/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2191 2023-08-02 13:30:30.000000 roadrecon-1.1.2/roadtools/roadrecon/dist_gui/assets/roadicon.png
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2955 2023-08-02 13:30:30.000000 roadrecon-1.1.2/roadtools/roadrecon/dist_gui/assets/rt_logoonly_margin.svg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     4164 2023-08-02 13:30:30.000000 roadrecon-1.1.2/roadtools/roadrecon/dist_gui/assets/rt_transparent.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     7437 2023-08-02 13:30:31.000000 roadrecon-1.1.2/roadtools/roadrecon/dist_gui/index.html
+-rw-r--r--   0 vsts      (1001) docker     (123)   898232 2023-08-02 13:30:28.000000 roadrecon-1.1.2/roadtools/roadrecon/dist_gui/main.1066d5fe02fb5e54.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    37024 2023-08-02 13:30:28.000000 roadrecon-1.1.2/roadtools/roadrecon/dist_gui/polyfills.3434510fb5b4de7e.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     1083 2023-08-02 13:30:28.000000 roadrecon-1.1.2/roadtools/roadrecon/dist_gui/runtime.a7446122f8b27a4d.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    76259 2023-08-02 13:30:28.000000 roadrecon-1.1.2/roadtools/roadrecon/dist_gui/styles.9afce2c3ef55c87a.css
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    31362 2023-08-02 13:29:28.000000 roadrecon-1.1.2/roadtools/roadrecon/gather.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5052 2023-08-02 13:29:28.000000 roadrecon-1.1.2/roadtools/roadrecon/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 13:30:49.871862 roadrecon-1.1.2/roadtools/roadrecon/plugins/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-02 13:29:28.000000 roadrecon-1.1.2/roadtools/roadrecon/plugins/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12137 2023-08-02 13:29:28.000000 roadrecon-1.1.2/roadtools/roadrecon/plugins/bloodhound.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    20158 2023-08-02 13:29:28.000000 roadrecon-1.1.2/roadtools/roadrecon/plugins/policies.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10032 2023-08-02 13:29:28.000000 roadrecon-1.1.2/roadtools/roadrecon/plugins/road2timeline.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2173 2023-08-02 13:29:28.000000 roadrecon-1.1.2/roadtools/roadrecon/plugins/road2timeline.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)    17455 2023-08-02 13:29:28.000000 roadrecon-1.1.2/roadtools/roadrecon/plugins/xlsexport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    23566 2023-08-02 13:29:28.000000 roadrecon-1.1.2/roadtools/roadrecon/server.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-02 13:30:49.871862 roadrecon-1.1.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1404 2023-08-02 13:29:28.000000 roadrecon-1.1.2/setup.py
```

### Comparing `roadrecon-1.1.1/PKG-INFO` & `roadrecon-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadrecon
-Version: 1.1.1
+Version: 1.1.2
 Summary: Azure AD recon for red and blue
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@dirkjanm.io
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `roadrecon-1.1.1/roadrecon.egg-info/PKG-INFO` & `roadrecon-1.1.2/roadrecon.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadrecon
-Version: 1.1.1
+Version: 1.1.2
 Summary: Azure AD recon for red and blue
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@dirkjanm.io
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `roadrecon-1.1.1/roadrecon.egg-info/SOURCES.txt` & `roadrecon-1.1.2/roadrecon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/dist_gui/3rdpartylicenses.txt` & `roadrecon-1.1.2/roadtools/roadrecon/dist_gui/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/dist_gui/assets/roadicon.png` & `roadrecon-1.1.2/roadtools/roadrecon/dist_gui/assets/roadicon.png`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/dist_gui/assets/rt_logoonly_margin.svg` & `roadrecon-1.1.2/roadtools/roadrecon/dist_gui/assets/rt_logoonly_margin.svg`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/dist_gui/assets/rt_transparent.svg` & `roadrecon-1.1.2/roadtools/roadrecon/dist_gui/assets/rt_transparent.svg`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/dist_gui/index.html` & `roadrecon-1.1.2/roadtools/roadrecon/dist_gui/index.html`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/dist_gui/main.1066d5fe02fb5e54.js` & `roadrecon-1.1.2/roadtools/roadrecon/dist_gui/main.1066d5fe02fb5e54.js`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/dist_gui/polyfills.3434510fb5b4de7e.js` & `roadrecon-1.1.2/roadtools/roadrecon/dist_gui/polyfills.3434510fb5b4de7e.js`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/dist_gui/runtime.a7446122f8b27a4d.js` & `roadrecon-1.1.2/roadtools/roadrecon/dist_gui/runtime.a7446122f8b27a4d.js`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/dist_gui/styles.9afce2c3ef55c87a.css` & `roadrecon-1.1.2/roadtools/roadrecon/dist_gui/styles.9afce2c3ef55c87a.css`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/gather.py` & `roadrecon-1.1.2/roadtools/roadrecon/gather.py`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/main.py` & `roadrecon-1.1.2/roadtools/roadrecon/main.py`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/plugins/bloodhound.py` & `roadrecon-1.1.2/roadtools/roadrecon/plugins/bloodhound.py`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/plugins/policies.py` & `roadrecon-1.1.2/roadtools/roadrecon/plugins/policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             if len(res) != len(aid):
                 return self.session.query(ServicePrincipal).filter(ServicePrincipal.appId.in_(aid)).all()
             else:
                 return res
         else:
             res = self.session.query(Application).filter(Application.appId == aid).first()
             # if no result, query the ServicePrincipals
-            if len(res) == 0:
+            if res is None or len(res) == 0:
                 return self.session.query(ServicePrincipal).filter(ServicePrincipal.appId == aid).first()
 
     def _get_user(self, uid):
         if isinstance(uid, list):
             return self.session.query(User).filter(User.objectId.in_(uid)).all()
         return self.session.query(User).filter(User.objectId == uid).first()
 
@@ -224,18 +224,19 @@
                     break
                 if 'None' in clist:
                     ot += 'None'
                     break
                 if 'Office365' in clist:
                     ot += 'All Office 365 applications'
                 objects = self._get_application(clist)
-                if len(objects) > 0:
-                    if ctype == 'Applications':
-                        ot += 'Applications: '
-                        ot += ', '.join([escape(uobj.displayName) for uobj in objects])
+                if objects is not None: 
+                    if len(objects) > 0:
+                        if ctype == 'Applications':
+                            ot += 'Applications: '
+                            ot += ', '.join([escape(uobj.displayName) for uobj in objects])
         return ot
 
     def _parse_platform(self, cond):
         try:
             pcond = cond['DevicePlatforms']
         except KeyError:
             return ''
```

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/plugins/road2timeline.py` & `roadrecon-1.1.2/roadtools/roadrecon/plugins/road2timeline.py`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/plugins/road2timeline.yaml` & `roadrecon-1.1.2/roadtools/roadrecon/plugins/road2timeline.yaml`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/plugins/xlsexport.py` & `roadrecon-1.1.2/roadtools/roadrecon/plugins/xlsexport.py`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/roadtools/roadrecon/server.py` & `roadrecon-1.1.2/roadtools/roadrecon/server.py`

 * *Files identical despite different names*

### Comparing `roadrecon-1.1.1/setup.py` & `roadrecon-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 setup(name='roadrecon',
-      version='1.1.1',
+      version='1.1.2',
       description='Azure AD recon for red and blue',
       author='Dirk-jan Mollema',
       author_email='dirkjan@dirkjanm.io',
       url='https://github.com/dirkjanm/ROADtools/',
       license='MIT',
       classifiers=[
           'Intended Audience :: Information Technology',
```

