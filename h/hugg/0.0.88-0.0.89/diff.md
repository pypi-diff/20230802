# Comparing `tmp/hugg-0.0.88.tar.gz` & `tmp/hugg-0.0.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.0.88.tar", last modified: Sun Apr  9 17:26:59 2023, max compression
+gzip compressed data, was "hugg-0.0.89.tar", last modified: Wed Aug  2 16:46:47 2023, max compression
```

## Comparing `hugg-0.0.88.tar` & `hugg-0.0.89.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:26:59.650752 hugg-0.0.88/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 17:26:49.000000 hugg-0.0.88/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 17:26:59.650752 hugg-0.0.88/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-09 17:26:49.000000 hugg-0.0.88/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:26:59.650752 hugg-0.0.88/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-09 17:26:49.000000 hugg-0.0.88/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:26:59.650752 hugg-0.0.88/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 17:26:59.000000 hugg-0.0.88/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-09 17:26:59.000000 hugg-0.0.88/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:26:59.000000 hugg-0.0.88/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 17:26:59.000000 hugg-0.0.88/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 17:26:59.000000 hugg-0.0.88/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 17:26:59.650752 hugg-0.0.88/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-04-09 17:26:49.000000 hugg-0.0.88/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:46:47.174200 hugg-0.0.89/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 16:46:34.000000 hugg-0.0.89/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 16:46:47.174200 hugg-0.0.89/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 16:46:34.000000 hugg-0.0.89/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:46:47.174200 hugg-0.0.89/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    37424 2023-08-02 16:46:34.000000 hugg-0.0.89/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:46:47.174200 hugg-0.0.89/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 16:46:47.000000 hugg-0.0.89/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 16:46:47.000000 hugg-0.0.89/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:46:47.000000 hugg-0.0.89/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-02 16:46:47.000000 hugg-0.0.89/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 16:46:47.000000 hugg-0.0.89/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:46:47.174200 hugg-0.0.89/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3546 2023-08-02 16:46:34.000000 hugg-0.0.89/setup.py
```

### Comparing `hugg-0.0.88/LICENSE` & `hugg-0.0.89/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.0.88/hugg/__init__.py` & `hugg-0.0.89/hugg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import ruamel.std.zipfile as zipfileextra
 import fnmatch
 if sys.version_info[0] < 3: 
     from StringIO import StringIO
 else:
     from io import StringIO
 # https://pypi.org/project/ruamel.std.zipfile/
+from ephfile import ephfile
 
 def split(a, n):
     """
     https://stackoverflow.com/questions/2130016/splitting-a-list-into-n-parts-of-approximately-equal-length
 
     >>> list(split(range(11), 3))
     [[0, 1, 2, 3], [4, 5, 6, 7], [8, 9, 10]]
@@ -983,14 +984,52 @@
     def delete_file(self,path_in_repo=None):
         if not os.path.exists(self.location):
             return
 
         zipfileextra.delete_from_zip_file(self.location, file_names=[path_in_repo])
         return True
 
+class subRemote(mem):
+    #https://docs.python.org/3/library/zipfile.html
+    def __init__(self,identifyFile:str):
+        self.identifyFile = identifyFile
+        __name__ = ''
+
+        self.files = []
+        self.download = None
+
+        if os.path.exists(self.identifyFile):
+            self.mod = __import__(self.identifyFile)
+            self.download = self.mod.download
+            self.files = self.mod.info()
+
+    def url(self):
+        self.location = zyp_file
+
+    def login(self):
+        return
+    
+    def logout(self):
+        return
+
+    def files(self):
+        return self.files
+    
+    def upload(self, file_path=None,path_in_repo=None):
+        return False
+    
+    def download(self, file_path=None,download_to=None):
+        if self.download == None:
+            return False
+        self.download(file_path, download_to)
+    
+    def delete_file(self,path_in_repo=None):
+        return False
+
+
 def redundant(klass):
     """
     #Example:
     source = hugg.redundant([
         hugg.face(xxx, yyy),
         hugg.ghub(xxx, yyy),
     ])
```

### Comparing `hugg-0.0.88/setup.py` & `hugg-0.0.89/setup.py`

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
-VERSION = "0.0.88"
+VERSION = "0.0.89"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -116,14 +116,15 @@
 	python_requires=REQUIRES_PYTHON,
 	url=URL,
 	packages=find_packages(
 		exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
 	entry_points={
 	},
 	install_requires=[
+		"ephfile",
 		"datasets",
 		"huggingface_hub",
 		"PyGithub", #https://pypi.org/project/PyGithub/
 		"python-gitlab",
 		"ruamel.std.zipfile"
 	],
 	include_package_data=True,
```

