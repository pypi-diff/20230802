# Comparing `tmp/hugg-0.0.97.tar.gz` & `tmp/hugg-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.0.97.tar", last modified: Wed Aug  2 21:31:03 2023, max compression
+gzip compressed data, was "hugg-0.0.98.tar", last modified: Wed Aug  2 21:41:09 2023, max compression
```

## Comparing `hugg-0.0.97.tar` & `hugg-0.0.98.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:31:03.266710 hugg-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 21:30:52.000000 hugg-0.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 21:31:03.266710 hugg-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 21:30:52.000000 hugg-0.0.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:31:03.262710 hugg-0.0.97/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    39654 2023-08-02 21:30:52.000000 hugg-0.0.97/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:31:03.266710 hugg-0.0.97/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 21:31:03.000000 hugg-0.0.97/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 21:31:03.000000 hugg-0.0.97/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:31:03.000000 hugg-0.0.97/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 21:31:03.000000 hugg-0.0.97/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 21:31:03.000000 hugg-0.0.97/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:31:03.266710 hugg-0.0.97/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3560 2023-08-02 21:30:52.000000 hugg-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:09.854180 hugg-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 21:40:56.000000 hugg-0.0.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 21:41:09.854180 hugg-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 21:40:56.000000 hugg-0.0.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:09.854180 hugg-0.0.98/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    39643 2023-08-02 21:40:56.000000 hugg-0.0.98/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:09.854180 hugg-0.0.98/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 21:41:09.000000 hugg-0.0.98/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 21:41:09.000000 hugg-0.0.98/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:09.000000 hugg-0.0.98/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 21:41:09.000000 hugg-0.0.98/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 21:41:09.000000 hugg-0.0.98/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:41:09.854180 hugg-0.0.98/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3560 2023-08-02 21:40:56.000000 hugg-0.0.98/setup.py
```

### Comparing `hugg-0.0.97/LICENSE` & `hugg-0.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.0.97/hugg/__init__.py` & `hugg-0.0.98/hugg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os,sys,types,importlib.machinery,shutil
+import os,sys,types,importlib.machinery,shutil,mystring
 import threading as thread
 from pathlib import Path
 from huggingface_hub import HfApi
 from abc import ABC, abstractmethod
 from github import Github
 from gitlab import Gitlab
 from zipfile import ZipFile
@@ -115,15 +115,15 @@
         for file in files:
             ext = pathlib.Path(file).suffix
             if ext not in output:
                 output[ext] = 0
             output[ext] += 1
         return output
     def wrap(self,foil):
-        import json, mystring
+        import json
         with open(foil,"r") as reader:
             content = reader.readlines()
 
         info = {
             'content':mystring.string(content).tobase64()
         }
         os.remove(foil)
@@ -133,15 +133,15 @@
             writer.write(json.dumps(info))
 
         return foil
 
     def unwrap(self,foil):
         #Checking if there is a custom wrapping around the file, and unwrapping
         if foil.endswith(".nosj"):
-            import json, mystring
+            import json
             with open(foil, 'r') as reader:
                 content = json.load(reader)
 
             os.remove(foil)
             foil = foil.replace('.nosj','')
 
             with open(foil, 'w+') as writer:
```

### Comparing `hugg-0.0.97/setup.py` & `hugg-0.0.98/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.97"
+VERSION = "0.0.98"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

