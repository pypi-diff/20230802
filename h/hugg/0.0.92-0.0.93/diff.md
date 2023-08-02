# Comparing `tmp/hugg-0.0.92.tar.gz` & `tmp/hugg-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.0.92.tar", last modified: Wed Aug  2 17:56:46 2023, max compression
+gzip compressed data, was "hugg-0.0.93.tar", last modified: Wed Aug  2 20:32:18 2023, max compression
```

## Comparing `hugg-0.0.92.tar` & `hugg-0.0.93.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:56:46.409603 hugg-0.0.92/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 17:56:35.000000 hugg-0.0.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 17:56:46.405603 hugg-0.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 17:56:35.000000 hugg-0.0.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:56:46.405603 hugg-0.0.92/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    39407 2023-08-02 17:56:35.000000 hugg-0.0.92/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:56:46.405603 hugg-0.0.92/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 17:56:46.000000 hugg-0.0.92/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 17:56:46.000000 hugg-0.0.92/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:56:46.000000 hugg-0.0.92/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 17:56:46.000000 hugg-0.0.92/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 17:56:46.000000 hugg-0.0.92/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:56:46.409603 hugg-0.0.92/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3560 2023-08-02 17:56:35.000000 hugg-0.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:32:18.694561 hugg-0.0.93/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 20:32:07.000000 hugg-0.0.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 20:32:18.694561 hugg-0.0.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 20:32:07.000000 hugg-0.0.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:32:18.694561 hugg-0.0.93/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    39671 2023-08-02 20:32:07.000000 hugg-0.0.93/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:32:18.694561 hugg-0.0.93/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 20:32:18.000000 hugg-0.0.93/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 20:32:18.000000 hugg-0.0.93/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:32:18.000000 hugg-0.0.93/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 20:32:18.000000 hugg-0.0.93/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 20:32:18.000000 hugg-0.0.93/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:32:18.694561 hugg-0.0.93/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3560 2023-08-02 20:32:07.000000 hugg-0.0.93/setup.py
```

### Comparing `hugg-0.0.92/LICENSE` & `hugg-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.0.92/hugg/__init__.py` & `hugg-0.0.93/hugg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,27 +68,27 @@
             setattr(self,'dowraplambda',lambda foil:True)
         return getattr(self,'dowraplambda')
 
     def setWrapLambda(self, lambd):
         setattr(self,'dowraplambda',lambd)
 
     def download(self, file_path=None,download_to=None, wrap:bool=None):
-        __internal_download(file_path, download_to)
+        self.__internal_download(file_path, download_to)
 
         if self.checkwrap or self.checkWrapLambda()(download_to):
             download_to = self.unWrap(download_to)
         
         return download_to
 
     def upload(self, path=None,path_in_repo=None, wrap:bool=None):
         if self.checkWrap or self.checkWrapLambda()(path):
             path = self.wrap(path)
             path_in_repo += ".nosj"
 
-        return __internal_upload(path, path_in_repo)
+        return self.__internal_upload(path, path_in_repo)
 
     def __enter__(self):
         self.login()
         return self
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.logout()
         return self
@@ -105,14 +105,23 @@
         return self.files()
     def __contains__(self, item):
         return item in self.files()
     def __call__(self,item):
         return self.download(item) if item in self else None
     def __len__(self):
         return len(self.files())
+    def outline(self):
+        import pathlib
+        output = {}
+        for file in files:
+            ext = pathlib.Path(file).suffix
+            if ext not in output:
+                output[ext] = 0
+            output[ext] += 1
+        return output
     def wrap(self,foil):
         import json, mystring
         with open(foil,"r") as reader:
             content = reader.readlines()
 
         info = {
             'content':mystring.string(content).tobase64()
```

### Comparing `hugg-0.0.92/setup.py` & `hugg-0.0.93/setup.py`

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
-VERSION = "0.0.92"
+VERSION = "0.0.93"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

