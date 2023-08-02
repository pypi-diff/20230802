# Comparing `tmp/vango-1.2.3.tar.gz` & `tmp/vango-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vango-1.2.3.tar", last modified: Tue Aug  1 02:49:47 2023, max compression
+gzip compressed data, was "dist/vango-1.2.5.tar", last modified: Wed Aug  2 07:39:19 2023, max compression
```

## Comparing `vango-1.2.3.tar` & `vango-1.2.5.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-01 02:49:47.000000 vango-1.2.3/
--rw-r--r--   0 jan        (501) staff       (20)      280 2023-08-01 02:49:47.000000 vango-1.2.3/PKG-INFO
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-01 02:49:47.000000 vango-1.2.3/VGPY.egg-info/
--rw-r--r--   0 jan        (501) staff       (20)      268 2023-07-14 07:13:48.000000 vango-1.2.3/VGPY.egg-info/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)      159 2023-07-14 07:13:48.000000 vango-1.2.3/VGPY.egg-info/SOURCES.txt
--rw-r--r--   0 jan        (501) staff       (20)        5 2023-07-14 07:13:48.000000 vango-1.2.3/VGPY.egg-info/top_level.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-14 07:13:48.000000 vango-1.2.3/VGPY.egg-info/dependency_links.txt
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-01 02:49:47.000000 vango-1.2.3/dist/
--rw-r--r--   0 jan        (501) staff       (20)     1784 2023-07-14 07:12:23.000000 vango-1.2.3/dist/VGPY-1.0.0.tar.gz
--rw-r--r--   0 jan        (501) staff       (20)    97599 2023-07-24 03:52:34.000000 vango-1.2.3/dist/vango-1.1.5.tar.gz
--rw-r--r--   0 jan        (501) staff       (20)     1932 2023-07-14 10:17:25.000000 vango-1.2.3/dist/vango-1.0.3.tar.gz
--rw-r--r--   0 jan        (501) staff       (20)    21371 2023-07-19 07:59:12.000000 vango-1.2.3/dist/vango-1.1.3.tar.gz
--rw-r--r--   0 jan        (501) staff       (20)   193495 2023-07-24 04:20:18.000000 vango-1.2.3/dist/vango-1.2.0.tar.gz
--rw-r--r--   0 jan        (501) staff       (20)   775281 2023-07-28 08:08:13.000000 vango-1.2.3/dist/vango-1.2.2.tar.gz
--rw-r--r--   0 jan        (501) staff       (20)     2045 2023-07-19 03:02:36.000000 vango-1.2.3/dist/vango-1.1.1.tar.gz
--rw-r--r--   0 jan        (501) staff       (20)    53722 2023-07-19 08:05:51.000000 vango-1.2.3/dist/vango-1.1.4.tar.gz
--rw-r--r--   0 jan        (501) staff       (20)     1787 2023-07-14 07:13:48.000000 vango-1.2.3/dist/VGPY-1.0.1.tar.gz
--rw-r--r--   0 jan        (501) staff       (20)   386945 2023-07-24 04:23:28.000000 vango-1.2.3/dist/vango-1.2.1.tar.gz
--rw-r--r--   0 jan        (501) staff       (20)     2123 2023-07-19 07:15:24.000000 vango-1.2.3/dist/vango-1.1.2.tar.gz
--rw-r--r--   0 jan        (501) staff       (20)     2199 2023-07-14 07:25:31.000000 vango-1.2.3/dist/vango-1.0.2.tar.gz
--rw-r--r--   0 jan        (501) staff       (20)     1943 2023-07-18 01:43:44.000000 vango-1.2.3/dist/vango-1.1.0.tar.gz
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-01 02:49:47.000000 vango-1.2.3/vango.egg-info/
--rw-r--r--   0 jan        (501) staff       (20)      280 2023-08-01 02:49:47.000000 vango-1.2.3/vango.egg-info/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)      773 2023-08-01 02:49:47.000000 vango-1.2.3/vango.egg-info/SOURCES.txt
--rw-r--r--   0 jan        (501) staff       (20)       11 2023-08-01 02:49:47.000000 vango-1.2.3/vango.egg-info/top_level.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2023-08-01 02:49:47.000000 vango-1.2.3/vango.egg-info/dependency_links.txt
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-01 02:49:47.000000 vango-1.2.3/vango/
--rw-r--r--   0 jan        (501) staff       (20)       16 2023-07-19 07:03:50.000000 vango-1.2.3/vango/sign.txt
--rw-r--r--   0 jan        (501) staff       (20)     5573 2023-08-01 02:49:30.000000 vango-1.2.3/vango/openapi.py
--rw-r--r--   0 jan        (501) staff       (20)       22 2023-07-14 07:25:26.000000 vango-1.2.3/vango/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)       16 2023-07-19 07:58:38.000000 vango-1.2.3/MANIFEST.in
--rw-r--r--   0 jan        (501) staff       (20)      523 2023-08-01 02:49:41.000000 vango-1.2.3/setup.py
--rw-r--r--   0 jan        (501) staff       (20)       59 2023-08-01 02:49:47.000000 vango-1.2.3/setup.cfg
--rw-r--r--   0 jan        (501) staff       (20)       74 2023-07-14 03:50:32.000000 vango-1.2.3/.pypirc
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-01 02:49:47.000000 vango-1.2.3/VGPY/
--rw-r--r--   0 jan        (501) staff       (20)     1848 2023-07-13 12:55:09.000000 vango-1.2.3/VGPY/vango_openapi.py
--rw-r--r--   0 jan        (501) staff       (20)       15 2023-07-13 11:49:35.000000 vango-1.2.3/VGPY/user.txt
--rw-r--r--   0 jan        (501) staff       (20)       28 2023-07-14 07:12:13.000000 vango-1.2.3/VGPY/__init__.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-01 02:49:47.000000 vango-1.2.3/.idea/
--rw-r--r--   0 jan        (501) staff       (20)      187 2023-07-14 03:17:15.000000 vango-1.2.3/.idea/jsLibraryMappings.xml
--rw-r--r--   0 jan        (501) staff       (20)    38409 2023-08-01 02:47:50.000000 vango-1.2.3/.idea/workspace.xml
--rw-r--r--   0 jan        (501) staff       (20)      276 2023-07-14 03:17:09.000000 vango-1.2.3/.idea/modules.xml
--rw-r--r--   0 jan        (501) staff       (20)     1540 2023-07-14 03:21:31.000000 vango-1.2.3/.idea/misc.xml
--rw-r--r--   0 jan        (501) staff       (20)      455 2023-07-14 03:17:24.000000 vango-1.2.3/.idea/vangoOpenapi.iml
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-02 07:39:19.000000 vango-1.2.5/
+-rw-r--r--   0 jan        (501) staff       (20)      280 2023-08-02 07:39:19.000000 vango-1.2.5/PKG-INFO
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-02 07:39:19.000000 vango-1.2.5/VGPY.egg-info/
+-rw-r--r--   0 jan        (501) staff       (20)      268 2023-07-14 07:13:48.000000 vango-1.2.5/VGPY.egg-info/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)      159 2023-07-14 07:13:48.000000 vango-1.2.5/VGPY.egg-info/SOURCES.txt
+-rw-r--r--   0 jan        (501) staff       (20)        5 2023-07-14 07:13:48.000000 vango-1.2.5/VGPY.egg-info/top_level.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-14 07:13:48.000000 vango-1.2.5/VGPY.egg-info/dependency_links.txt
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-02 07:39:19.000000 vango-1.2.5/dist/
+-rw-r--r--   0 jan        (501) staff       (20)     1784 2023-07-14 07:12:23.000000 vango-1.2.5/dist/VGPY-1.0.0.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)    97599 2023-07-24 03:52:34.000000 vango-1.2.5/dist/vango-1.1.5.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)     1932 2023-07-14 10:17:25.000000 vango-1.2.5/dist/vango-1.0.3.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)    21371 2023-07-19 07:59:12.000000 vango-1.2.5/dist/vango-1.1.3.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)   193495 2023-07-24 04:20:18.000000 vango-1.2.5/dist/vango-1.2.0.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)   775281 2023-07-28 08:08:13.000000 vango-1.2.5/dist/vango-1.2.2.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)     2045 2023-07-19 03:02:36.000000 vango-1.2.5/dist/vango-1.1.1.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)    53722 2023-07-19 08:05:51.000000 vango-1.2.5/dist/vango-1.1.4.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)     1787 2023-07-14 07:13:48.000000 vango-1.2.5/dist/VGPY-1.0.1.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)   386945 2023-07-24 04:23:28.000000 vango-1.2.5/dist/vango-1.2.1.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)     2123 2023-07-19 07:15:24.000000 vango-1.2.5/dist/vango-1.1.2.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)     2199 2023-07-14 07:25:31.000000 vango-1.2.5/dist/vango-1.0.2.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)     1943 2023-07-18 01:43:44.000000 vango-1.2.5/dist/vango-1.1.0.tar.gz
+-rw-r--r--   0 jan        (501) staff       (20)  1550146 2023-08-01 02:49:48.000000 vango-1.2.5/dist/vango-1.2.3.tar.gz
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-02 07:39:19.000000 vango-1.2.5/vango.egg-info/
+-rw-r--r--   0 jan        (501) staff       (20)      280 2023-08-02 07:39:19.000000 vango-1.2.5/vango.egg-info/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)      797 2023-08-02 07:39:19.000000 vango-1.2.5/vango.egg-info/SOURCES.txt
+-rw-r--r--   0 jan        (501) staff       (20)       11 2023-08-02 07:39:19.000000 vango-1.2.5/vango.egg-info/top_level.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2023-08-02 07:39:19.000000 vango-1.2.5/vango.egg-info/dependency_links.txt
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-02 07:39:19.000000 vango-1.2.5/vango/
+-rw-r--r--   0 jan        (501) staff       (20)       16 2023-07-19 07:03:50.000000 vango-1.2.5/vango/sign.txt
+-rw-r--r--   0 jan        (501) staff       (20)     5609 2023-08-02 07:39:15.000000 vango-1.2.5/vango/openapi.py
+-rw-r--r--   0 jan        (501) staff       (20)       22 2023-07-14 07:25:26.000000 vango-1.2.5/vango/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)       16 2023-07-19 07:58:38.000000 vango-1.2.5/MANIFEST.in
+-rw-r--r--   0 jan        (501) staff       (20)      523 2023-08-02 07:39:15.000000 vango-1.2.5/setup.py
+-rw-r--r--   0 jan        (501) staff       (20)       59 2023-08-02 07:39:19.000000 vango-1.2.5/setup.cfg
+-rw-r--r--   0 jan        (501) staff       (20)       74 2023-07-14 03:50:32.000000 vango-1.2.5/.pypirc
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-02 07:39:19.000000 vango-1.2.5/VGPY/
+-rw-r--r--   0 jan        (501) staff       (20)     1848 2023-07-13 12:55:09.000000 vango-1.2.5/VGPY/vango_openapi.py
+-rw-r--r--   0 jan        (501) staff       (20)       15 2023-07-13 11:49:35.000000 vango-1.2.5/VGPY/user.txt
+-rw-r--r--   0 jan        (501) staff       (20)       28 2023-07-14 07:12:13.000000 vango-1.2.5/VGPY/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-08-02 07:39:19.000000 vango-1.2.5/.idea/
+-rw-r--r--   0 jan        (501) staff       (20)      187 2023-07-14 03:17:15.000000 vango-1.2.5/.idea/jsLibraryMappings.xml
+-rw-r--r--   0 jan        (501) staff       (20)    38404 2023-08-02 06:49:57.000000 vango-1.2.5/.idea/workspace.xml
+-rw-r--r--   0 jan        (501) staff       (20)      276 2023-07-14 03:17:09.000000 vango-1.2.5/.idea/modules.xml
+-rw-r--r--   0 jan        (501) staff       (20)     1540 2023-07-14 03:21:31.000000 vango-1.2.5/.idea/misc.xml
+-rw-r--r--   0 jan        (501) staff       (20)      455 2023-07-14 03:17:24.000000 vango-1.2.5/.idea/vangoOpenapi.iml
```

### Comparing `vango-1.2.3/dist/VGPY-1.0.0.tar.gz` & `vango-1.2.5/dist/VGPY-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/dist/vango-1.1.5.tar.gz` & `vango-1.2.5/dist/vango-1.1.5.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/dist/vango-1.0.3.tar.gz` & `vango-1.2.5/dist/vango-1.0.3.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/dist/vango-1.1.3.tar.gz` & `vango-1.2.5/dist/vango-1.1.3.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/dist/vango-1.2.0.tar.gz` & `vango-1.2.5/dist/vango-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/dist/vango-1.2.2.tar.gz` & `vango-1.2.5/dist/vango-1.2.2.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/dist/vango-1.1.1.tar.gz` & `vango-1.2.5/dist/vango-1.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/dist/vango-1.1.4.tar.gz` & `vango-1.2.5/dist/vango-1.1.4.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/dist/VGPY-1.0.1.tar.gz` & `vango-1.2.5/dist/VGPY-1.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/dist/vango-1.2.1.tar.gz` & `vango-1.2.5/dist/vango-1.2.1.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/dist/vango-1.1.2.tar.gz` & `vango-1.2.5/dist/vango-1.1.2.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/dist/vango-1.0.2.tar.gz` & `vango-1.2.5/dist/vango-1.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/dist/vango-1.1.0.tar.gz` & `vango-1.2.5/dist/vango-1.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/vango.egg-info/SOURCES.txt` & `vango-1.2.5/vango.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 dist/vango-1.1.2.tar.gz
 dist/vango-1.1.3.tar.gz
 dist/vango-1.1.4.tar.gz
 dist/vango-1.1.5.tar.gz
 dist/vango-1.2.0.tar.gz
 dist/vango-1.2.1.tar.gz
 dist/vango-1.2.2.tar.gz
+dist/vango-1.2.3.tar.gz
 vango/__init__.py
 vango/openapi.py
 vango/sign.txt
 vango.egg-info/PKG-INFO
 vango.egg-info/SOURCES.txt
 vango.egg-info/dependency_links.txt
 vango.egg-info/top_level.txt
```

### Comparing `vango-1.2.3/vango/openapi.py` & `vango-1.2.5/vango/openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # 获取任务的详细信息
 # name          任务中文名      必填
 # code          资产编号        必填
 # project_name  项目名称        选填
 # asset_project 资产项目        选填
 # options       额外参数        非必填
 def get_task_detail(name, code, project_name, asset_project, options):
-    params = {"code": code, "name": name, "project_name": project_name, "asset_project": asset_project, "options": options}
+    params = {"code": code, "name": name, "project_name": project_name, "asset_project": asset_project, "options": json.dumps(options)}
 
     sign, userName, timestamp, appSign = _get_sign()
     headers = {"VG-Request-User": userName, "VG-Request-Sign": sign,
                "VG-Request-Time": str(timestamp)}
     url = 'http://mvango.37wan.com/openapi/task/detail'
 
     response = requests.get(url=url, params=params, headers=headers)
@@ -26,15 +26,15 @@
     return response.json()
 
 # 上传文件
 # task_id 任务ID 必填
 # file_path 本地文件路径 必填
 # options 额外参数 非必填
 def upload_task_file(task_id, file_path, options):
-    data = {"task_id": task_id, "options": options}
+    data = {"task_id": task_id, "options": json.dumps(options)}
 
     try:
         with open(file_path, "rb") as upload_file:
             files = {"file": upload_file}
 
             sign, userName, timestamp, appSign = _get_sign()
             headers = {"VG-Request-User": userName, "VG-Request-Sign": sign,
@@ -56,15 +56,15 @@
 # asset_project 资产项目 必填
 # asset_name 资产中文名 必填
 # code 资产编号 必填
 # path 本地文件路径 必填
 # options 额外参数 非必填
 def upload_asset_files(path, code, asset_name, asset_project, options):
     url = 'http://internal.vango-openapi.data-ad.37ops.com/openapi/asset/file_upload'
-    data = {"asset_project": asset_project, "name": asset_name, "code": code, "options": options}
+    data = {"asset_project": asset_project, "name": asset_name, "code": code, "options": json.dumps(options)}
     result = []
     sub_path = ""
     upload_asset_file_to_service(path, url, data, result, sub_path)
     return result
 
 def handle_file_upload(file_path, url, data, sub_path):
     with open(file_path, 'rb') as file_obj:
```

### Comparing `vango-1.2.3/setup.py` & `vango-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='vango',
-    version='1.2.3',
+    version='1.2.5',
     description='van go open api',
     author='JanVee',
     author_email='814107539@qq.com',
     packages=find_packages(),
     install_requires=[],
     keywords = ("vango", "VGPY"),
     long_description = "An feature extraction algorithm, van_go open api",
```

### Comparing `vango-1.2.3/VGPY/vango_openapi.py` & `vango-1.2.5/VGPY/vango_openapi.py`

 * *Files identical despite different names*

### Comparing `vango-1.2.3/.idea/workspace.xml` & `vango-1.2.5/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `vango-1.2.3/.idea/workspace.xml` & `vango-1.2.5/.idea/workspace.xml`

```diff
@@ -22,28 +22,28 @@
     </favorites_list>
   </component>
   <component name="FileEditorManager">
     <leaf SIDE_TABS_SIZE_LIMIT_KEY="300">
       <file leaf-file-name="openapi.py" pinned="false" current-in-tab="true">
         <entry file="file://$PROJECT_DIR$/vango/openapi.py">
           <provider selected="true" editor-type-id="text-editor">
-            <state relative-caret-position="180">
-              <caret line="12" column="46" selection-start-line="12" selection-start-column="46" selection-end-line="12" selection-end-column="46"/>
+            <state relative-caret-position="405">
+              <caret line="27" column="6" selection-start-line="27" selection-start-column="6" selection-end-line="27" selection-end-column="6"/>
               <folding>
                 <element signature="e#24#33#0" expanded="true"/>
               </folding>
             </state>
           </provider>
         </entry>
       </file>
       <file leaf-file-name="setup.py" pinned="false" current-in-tab="false">
         <entry file="file://$PROJECT_DIR$/setup.py">
           <provider selected="true" editor-type-id="text-editor">
-            <state relative-caret-position="105">
-              <caret line="7" column="18" selection-start-line="7" selection-start-column="18" selection-end-line="7" selection-end-column="18"/>
+            <state relative-caret-position="285">
+              <caret line="19" column="1" selection-start-line="19" selection-start-column="1" selection-end-line="19" selection-end-column="1"/>
               <folding/>
             </state>
           </provider>
         </entry>
       </file>
     </leaf>
   </component>
@@ -60,27 +60,27 @@
         <option value="$PROJECT_DIR$/__init__.py"/>
         <option value="$PROJECT_DIR$/.pypirc"/>
         <option value="$PROJECT_DIR$/VGPY/__init__.py"/>
         <option value="$PROJECT_DIR$/vango/__init__.py"/>
         <option value="$PROJECT_DIR$/vango/vango_openapi.py"/>
         <option value="$PROJECT_DIR$/vango/sign.txt"/>
         <option value="$PROJECT_DIR$/MANIFEST.in"/>
-        <option value="$PROJECT_DIR$/setup.py"/>
         <option value="$PROJECT_DIR$/vango/openapi.py"/>
+        <option value="$PROJECT_DIR$/setup.py"/>
       </list>
     </option>
   </component>
   <component name="JsBuildToolGruntFileManager" detection-done="true" sorting="DEFINITION_ORDER"/>
   <component name="JsBuildToolPackageJson" detection-done="true" sorting="DEFINITION_ORDER"/>
   <component name="JsGulpfileManager">
     <detection-done>true</detection-done>
     <sorting>DEFINITION_ORDER</sorting>
   </component>
   <component name="ProjectFrameBounds">
-    <option name="x" value="253"/>
+    <option name="x" value="702"/>
     <option name="y" value="23"/>
     <option name="width" value="1400"/>
     <option name="height" value="934"/>
   </component>
   <component name="ProjectLevelVcsManager" settingsEditedManually="false">
     <OptionsSetting value="true" id="Add"/>
     <OptionsSetting value="true" id="Remove"/>
@@ -401,25 +401,25 @@
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1689304629664</updated>
     </task>
     <servers/>
   </component>
   <component name="ToolWindowManager">
-    <frame x="253" y="23" width="1400" height="934" extended-state="0"/>
+    <frame x="702" y="23" width="1400" height="934" extended-state="0"/>
     <editor active="true"/>
     <layout>
       <window_info id="Project" active="false" anchor="left" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="true" show_stripe_button="true" weight="0.23343152" sideWeight="0.5" order="0" side_tool="false" content_ui="combo"/>
       <window_info id="TODO" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="6" side_tool="false" content_ui="tabs"/>
       <window_info id="Event Log" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="7" side_tool="true" content_ui="tabs"/>
       <window_info id="Database" active="false" anchor="right" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="3" side_tool="false" content_ui="tabs"/>
       <window_info id="Version Control" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="7" side_tool="false" content_ui="tabs"/>
       <window_info id="Python Console" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.32897863" sideWeight="0.5" order="7" side_tool="false" content_ui="tabs"/>
       <window_info id="Structure" active="false" anchor="left" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.25" sideWeight="0.5" order="1" side_tool="false" content_ui="tabs"/>
-      <window_info id="Terminal" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="true" show_stripe_button="true" weight="0.32897863" sideWeight="0.5" order="7" side_tool="false" content_ui="tabs"/>
+      <window_info id="Terminal" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.32897863" sideWeight="0.5" order="7" side_tool="false" content_ui="tabs"/>
       <window_info id="Favorites" active="false" anchor="left" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="2" side_tool="true" content_ui="tabs"/>
       <window_info id="Cvs" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.25" sideWeight="0.5" order="4" side_tool="false" content_ui="tabs"/>
       <window_info id="Message" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="0" side_tool="false" content_ui="tabs"/>
       <window_info id="Commander" active="false" anchor="right" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.4" sideWeight="0.5" order="0" side_tool="false" content_ui="tabs"/>
       <window_info id="Inspection" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.4" sideWeight="0.5" order="5" side_tool="false" content_ui="tabs"/>
       <window_info id="Run" active="false" anchor="bottom" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.33" sideWeight="0.5" order="2" side_tool="false" content_ui="tabs"/>
       <window_info id="Hierarchy" active="false" anchor="right" auto_hide="false" internal_type="DOCKED" type="DOCKED" visible="false" show_stripe_button="true" weight="0.25" sideWeight="0.5" order="2" side_tool="false" content_ui="combo"/>
@@ -731,24 +731,24 @@
           <caret line="0" column="21" selection-start-line="0" selection-start-column="21" selection-end-line="0" selection-end-column="21"/>
           <folding/>
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/setup.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="105">
-          <caret line="7" column="18" selection-start-line="7" selection-start-column="18" selection-end-line="7" selection-end-column="18"/>
+        <state relative-caret-position="285">
+          <caret line="19" column="1" selection-start-line="19" selection-start-column="1" selection-end-line="19" selection-end-column="1"/>
           <folding/>
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/vango/openapi.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="180">
-          <caret line="12" column="46" selection-start-line="12" selection-start-column="46" selection-end-line="12" selection-end-column="46"/>
+        <state relative-caret-position="405">
+          <caret line="27" column="6" selection-start-line="27" selection-start-column="6" selection-end-line="27" selection-end-column="6"/>
           <folding>
             <element signature="e#24#33#0" expanded="true"/>
           </folding>
         </state>
       </provider>
     </entry>
   </component>
```

### Comparing `vango-1.2.3/.idea/misc.xml` & `vango-1.2.5/.idea/misc.xml`

 * *Files identical despite different names*

