# Comparing `tmp/hugg-0.0.91.tar.gz` & `tmp/hugg-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.0.91.tar", last modified: Wed Aug  2 17:22:32 2023, max compression
+gzip compressed data, was "hugg-0.0.92.tar", last modified: Wed Aug  2 17:56:46 2023, max compression
```

## Comparing `hugg-0.0.91.tar` & `hugg-0.0.92.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:22:32.705981 hugg-0.0.91/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 17:22:22.000000 hugg-0.0.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 17:22:32.705981 hugg-0.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 17:22:22.000000 hugg-0.0.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:22:32.705981 hugg-0.0.91/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    39261 2023-08-02 17:22:22.000000 hugg-0.0.91/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:22:32.705981 hugg-0.0.91/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 17:22:32.000000 hugg-0.0.91/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 17:22:32.000000 hugg-0.0.91/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:22:32.000000 hugg-0.0.91/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 17:22:32.000000 hugg-0.0.91/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 17:22:32.000000 hugg-0.0.91/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:22:32.705981 hugg-0.0.91/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3560 2023-08-02 17:22:22.000000 hugg-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:56:46.409603 hugg-0.0.92/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 17:56:35.000000 hugg-0.0.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 17:56:46.405603 hugg-0.0.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 17:56:35.000000 hugg-0.0.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:56:46.405603 hugg-0.0.92/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    39407 2023-08-02 17:56:35.000000 hugg-0.0.92/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:56:46.405603 hugg-0.0.92/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 17:56:46.000000 hugg-0.0.92/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 17:56:46.000000 hugg-0.0.92/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:56:46.000000 hugg-0.0.92/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 17:56:46.000000 hugg-0.0.92/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 17:56:46.000000 hugg-0.0.92/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:56:46.409603 hugg-0.0.92/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3560 2023-08-02 17:56:35.000000 hugg-0.0.92/setup.py
```

### Comparing `hugg-0.0.91/LICENSE` & `hugg-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.0.91/hugg/__init__.py` & `hugg-0.0.92/hugg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,22 +139,22 @@
                 writer.write(
                     mystring.string.frombase64(content['contents'])
                 )
 
         return foil
 
 
-    def by(self,ext):
-        return [x for x in self.files() if str(x).endswith(ext)]
+    def find_all(self,lambda_search,download:bool=False):
+        return [self.download(x, os.path.basename(x)) if download else x for x in self.files() if lambda_search(x)]
 
-    def find_all(self,lambda_search):
-        return [x for x in self.files() if lambda_search(x)]
+    def by(self,ext,download:bool=False):
+        return self.find_all(lambda_search=lambda x:str(x).endswith(ext), download=download)
 
-    def find(self,lambda_search):
-        current = self.find_all(lambda_search,False)
+    def find(self,lambda_search,download:bool=False):
+        current = self.find_all(lambda_search,download)
         if len(current) > 1:
             print("There are too many files found")
         elif len(current) == 1:
             return current[0]
         return None
 
     def impor(self,file,delete=False):
```

### Comparing `hugg-0.0.91/setup.py` & `hugg-0.0.92/setup.py`

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
-VERSION = "0.0.91"
+VERSION = "0.0.92"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

