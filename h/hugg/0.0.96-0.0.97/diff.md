# Comparing `tmp/hugg-0.0.96.tar.gz` & `tmp/hugg-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.0.96.tar", last modified: Wed Aug  2 21:01:34 2023, max compression
+gzip compressed data, was "hugg-0.0.97.tar", last modified: Wed Aug  2 21:31:03 2023, max compression
```

## Comparing `hugg-0.0.96.tar` & `hugg-0.0.97.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:01:34.188835 hugg-0.0.96/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 21:01:23.000000 hugg-0.0.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 21:01:34.188835 hugg-0.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 21:01:23.000000 hugg-0.0.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:01:34.188835 hugg-0.0.96/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    39653 2023-08-02 21:01:23.000000 hugg-0.0.96/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:01:34.188835 hugg-0.0.96/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 21:01:34.000000 hugg-0.0.96/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 21:01:34.000000 hugg-0.0.96/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:01:34.000000 hugg-0.0.96/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 21:01:34.000000 hugg-0.0.96/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 21:01:34.000000 hugg-0.0.96/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:01:34.188835 hugg-0.0.96/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3560 2023-08-02 21:01:23.000000 hugg-0.0.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:31:03.266710 hugg-0.0.97/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 21:30:52.000000 hugg-0.0.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 21:31:03.266710 hugg-0.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 21:30:52.000000 hugg-0.0.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:31:03.262710 hugg-0.0.97/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    39654 2023-08-02 21:30:52.000000 hugg-0.0.97/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:31:03.266710 hugg-0.0.97/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 21:31:03.000000 hugg-0.0.97/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 21:31:03.000000 hugg-0.0.97/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:31:03.000000 hugg-0.0.97/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 21:31:03.000000 hugg-0.0.97/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 21:31:03.000000 hugg-0.0.97/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:31:03.266710 hugg-0.0.97/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3560 2023-08-02 21:30:52.000000 hugg-0.0.97/setup.py
```

### Comparing `hugg-0.0.96/LICENSE` & `hugg-0.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.0.96/hugg/__init__.py` & `hugg-0.0.97/hugg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     @abstractmethod
     def delete_file(self,path_in_repo=None):
         pass
 
     def checkWrapLambda(self):
         if not hasattr(self,'dowraplambda'):
-            setattr(self,'dowraplambda',lambda foil:True)
+            setattr(self,'dowraplambda',lambda foil:False)
         return getattr(self,'dowraplambda')
 
     def setWrapLambda(self, lambd):
         setattr(self,'dowraplambda',lambd)
 
     def download(self, file_path=None,download_to=None, wrap:bool=False):
         self.__internal_download(file_path, download_to)
```

### Comparing `hugg-0.0.96/setup.py` & `hugg-0.0.97/setup.py`

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
-VERSION = "0.0.96"
+VERSION = "0.0.97"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

