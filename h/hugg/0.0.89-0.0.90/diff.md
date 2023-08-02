# Comparing `tmp/hugg-0.0.89.tar.gz` & `tmp/hugg-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.0.89.tar", last modified: Wed Aug  2 16:46:47 2023, max compression
+gzip compressed data, was "hugg-0.0.90.tar", last modified: Wed Aug  2 16:51:21 2023, max compression
```

## Comparing `hugg-0.0.89.tar` & `hugg-0.0.90.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:46:47.174200 hugg-0.0.89/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 16:46:34.000000 hugg-0.0.89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 16:46:47.174200 hugg-0.0.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 16:46:34.000000 hugg-0.0.89/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:46:47.174200 hugg-0.0.89/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    37424 2023-08-02 16:46:34.000000 hugg-0.0.89/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:46:47.174200 hugg-0.0.89/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 16:46:47.000000 hugg-0.0.89/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 16:46:47.000000 hugg-0.0.89/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:46:47.000000 hugg-0.0.89/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-02 16:46:47.000000 hugg-0.0.89/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 16:46:47.000000 hugg-0.0.89/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:46:47.174200 hugg-0.0.89/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3546 2023-08-02 16:46:34.000000 hugg-0.0.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:51:21.672230 hugg-0.0.90/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 16:51:10.000000 hugg-0.0.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 16:51:21.672230 hugg-0.0.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 16:51:10.000000 hugg-0.0.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:51:21.672230 hugg-0.0.90/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    37823 2023-08-02 16:51:10.000000 hugg-0.0.90/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:51:21.672230 hugg-0.0.90/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 16:51:21.000000 hugg-0.0.90/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 16:51:21.000000 hugg-0.0.90/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:51:21.000000 hugg-0.0.90/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-02 16:51:21.000000 hugg-0.0.90/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 16:51:21.000000 hugg-0.0.90/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:51:21.672230 hugg-0.0.90/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3546 2023-08-02 16:51:10.000000 hugg-0.0.90/setup.py
```

### Comparing `hugg-0.0.89/LICENSE` & `hugg-0.0.90/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.0.89/hugg/__init__.py` & `hugg-0.0.90/hugg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1017,14 +1017,25 @@
     def upload(self, file_path=None,path_in_repo=None):
         return False
     
     def download(self, file_path=None,download_to=None):
         if self.download == None:
             return False
         self.download(file_path, download_to)
+
+        #Checking if there is a custom wrapping around the file, and unwrapping
+        if file_path.endswith(".nosj"):
+            import json
+            with open(download_to, 'r') as reader:
+                content = json.load(reader)
+
+            os.remove(download_to)
+
+            with open(download_to.replace('.nosj',''), 'w+') as writer:
+                writer.write(content['contents'])
     
     def delete_file(self,path_in_repo=None):
         return False
 
 
 def redundant(klass):
     """
```

### Comparing `hugg-0.0.89/setup.py` & `hugg-0.0.90/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.89"
+VERSION = "0.0.90"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

