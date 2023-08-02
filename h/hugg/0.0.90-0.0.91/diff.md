# Comparing `tmp/hugg-0.0.90.tar.gz` & `tmp/hugg-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.0.90.tar", last modified: Wed Aug  2 16:51:21 2023, max compression
+gzip compressed data, was "hugg-0.0.91.tar", last modified: Wed Aug  2 17:22:32 2023, max compression
```

## Comparing `hugg-0.0.90.tar` & `hugg-0.0.91.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:51:21.672230 hugg-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 16:51:10.000000 hugg-0.0.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 16:51:21.672230 hugg-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 16:51:10.000000 hugg-0.0.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:51:21.672230 hugg-0.0.90/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    37823 2023-08-02 16:51:10.000000 hugg-0.0.90/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:51:21.672230 hugg-0.0.90/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 16:51:21.000000 hugg-0.0.90/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 16:51:21.000000 hugg-0.0.90/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:51:21.000000 hugg-0.0.90/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-02 16:51:21.000000 hugg-0.0.90/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 16:51:21.000000 hugg-0.0.90/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:51:21.672230 hugg-0.0.90/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3546 2023-08-02 16:51:10.000000 hugg-0.0.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:22:32.705981 hugg-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 17:22:22.000000 hugg-0.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 17:22:32.705981 hugg-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 17:22:22.000000 hugg-0.0.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:22:32.705981 hugg-0.0.91/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    39261 2023-08-02 17:22:22.000000 hugg-0.0.91/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:22:32.705981 hugg-0.0.91/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 17:22:32.000000 hugg-0.0.91/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 17:22:32.000000 hugg-0.0.91/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:22:32.000000 hugg-0.0.91/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 17:22:32.000000 hugg-0.0.91/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 17:22:32.000000 hugg-0.0.91/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:22:32.705981 hugg-0.0.91/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3560 2023-08-02 17:22:22.000000 hugg-0.0.91/setup.py
```

### Comparing `hugg-0.0.90/LICENSE` & `hugg-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.0.90/hugg/__init__.py` & `hugg-0.0.91/hugg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     foil_name = str(foil.split('/')[-1]).replace('.py','')
 
     loader = importlib.machinery.SourceFileLoader(foil_name, os.path.abspath(foil_name))
     module = types.ModuleType(loader.name)
     loader.exec_module(module)
     return module
 
-class mem(object):     
+class mem(object):
     @abstractmethod
     def url(self):
         pass
 
     @abstractmethod
     def login(self):
         pass
@@ -48,25 +48,48 @@
         pass
 
     @abstractmethod
     def files(self):
         pass
     
     @abstractmethod
-    def upload(self, path=None,path_in_repo=None):
+    def __internal_upload(self, path=None,path_in_repo=None):
         pass
 
     @abstractmethod
-    def download(self, file_path=None,download_to=None):
+    def __internal_download(self, file_path=None,download_to=None):
         pass
 
     @abstractmethod
     def delete_file(self,path_in_repo=None):
         pass
-    
+
+    def checkWrapLambda(self):
+        if not hasattr(self,'dowraplambda'):
+            setattr(self,'dowraplambda',lambda foil:True)
+        return getattr(self,'dowraplambda')
+
+    def setWrapLambda(self, lambd):
+        setattr(self,'dowraplambda',lambd)
+
+    def download(self, file_path=None,download_to=None, wrap:bool=None):
+        __internal_download(file_path, download_to)
+
+        if self.checkwrap or self.checkWrapLambda()(download_to):
+            download_to = self.unWrap(download_to)
+        
+        return download_to
+
+    def upload(self, path=None,path_in_repo=None, wrap:bool=None):
+        if self.checkWrap or self.checkWrapLambda()(path):
+            path = self.wrap(path)
+            path_in_repo += ".nosj"
+
+        return __internal_upload(path, path_in_repo)
+
     def __enter__(self):
         self.login()
         return self
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.logout()
         return self
     def __iadd__(self, path):
@@ -82,14 +105,47 @@
         return self.files()
     def __contains__(self, item):
         return item in self.files()
     def __call__(self,item):
         return self.download(item) if item in self else None
     def __len__(self):
         return len(self.files())
+    def wrap(self,foil):
+        import json, mystring
+        with open(foil,"r") as reader:
+            content = reader.readlines()
+
+        info = {
+            'content':mystring.string(content).tobase64()
+        }
+        os.remove(foil)
+        foil = foil+".nosj"
+
+        with open(foil, "w+") as writer:
+            writer.write(json.dumps(info))
+
+        return foil
+
+    def unwrap(self,foil):
+        #Checking if there is a custom wrapping around the file, and unwrapping
+        if foil.endswith(".nosj"):
+            import json, mystring
+            with open(foil, 'r') as reader:
+                content = json.load(reader)
+
+            os.remove(foil)
+            foil = foil.replace('.nosj','')
+
+            with open(foil, 'w+') as writer:
+                writer.write(
+                    mystring.string.frombase64(content['contents'])
+                )
+
+        return foil
+
 
     def by(self,ext):
         return [x for x in self.files() if str(x).endswith(ext)]
 
     def find_all(self,lambda_search):
         return [x for x in self.files() if lambda_search(x)]
 
@@ -479,15 +535,15 @@
                 except Exception as e:
                     print("Failed to remove the cached file " +str(foil))
                     print(e)
                     pass
         self.clearcache()
         return
 
-    def download(self, file_path=None,download_to=None):
+    def __internal_download(self, file_path=None,download_to=None):
         download_to = download_to or os.path.basename(file_path)
         if not self.opened:
             self.login()
         #https://huggingface.co/docs/huggingface_hub/v0.9.0/en/package_reference/file_download#huggingface_hub.hf_hub_download
         if file_path and isinstance(file_path,str):
             from huggingface_hub import hf_hub_download
             current_file = hf_hub_download(
@@ -549,15 +605,15 @@
                         repo_id=self.repo,
                         repo_type=self.repo_type,
                         token=self.auth,
                         discussion_num=pr.num,
                         new_status='closed'
                     )
 
-    def upload(self, path=None,path_in_repo=None, auto_accept_all_pull_requests=True,use_pull_request = True):
+    def __internal_upload(self, path=None,path_in_repo=None, auto_accept_all_pull_requests=True,use_pull_request = True):
         if not self.opened:
             self.login()
         #Because HuggingFace_hub will get pissed if we don't use it
         if path:
             if isinstance(path,str) and os.path.isfile(path):
                 #https://huggingface.co/docs/huggingface_hub/v0.9.0/en/package_reference/hf_api#huggingface_hub.HfApi.upload_file
                 self.api.upload_file(
@@ -785,15 +841,15 @@
         try:
             repo = self.github_access.get_repo(repo)
             output = True
         except:
             output = False
         return output
     
-    def download(self, file_path=None,download_to=None, encoding="utf-8"):
+    def __internal_download(self, file_path=None,download_to=None, encoding="utf-8"):
         download_to = download_to or os.path.basename(file_path)
         if download_to is None:
             download_to = os.path.join(os.curdir,file_path.split("/")[-1])
         if file_path and isinstance(file_path,str):
             current_contents = self.repo.get_contents(file_path, ref=self.branch)
 
             print(":> "+str(encoding))
@@ -811,15 +867,15 @@
                 current_contents = base64.b64decode(bytearray(current_contents.content, "utf-8"))
                 encode_writing = "wb+"
 
             with open(download_to,encode_writing) as writer:
                 writer.write(current_contents)
         return download_to
     
-    def upload(self, file_path=None,path_in_repo=None):
+    def __internal_upload(self, file_path=None,path_in_repo=None):
         from pathlib import Path
         new_contents = Path(file_path).read_text()
         if path_in_repo in self: #Update
             contents = self.repo.get_contents(path_in_repo, ref=self.branch) #https://github.com/PyGithub/PyGithub/blob/001970d4a828017f704f6744a5775b4207a6523c/github/Repository.py#L1803
             self.repo.update_file(contents.path, "Updating the file {}".format(path_in_repo), new_contents, contents.sha, branch=self.branch) #https://github.com/PyGithub/PyGithub/blob/001970d4a828017f704f6744a5775b4207a6523c/github/Repository.py#L2134
         else: #Create #https://github.com/PyGithub/PyGithub/blob/001970d4a828017f704f6744a5775b4207a6523c/github/Repository.py#L2074
             self.repo.create_file(path_in_repo, "Creating the file {}".format(path_in_repo), new_contents, branch=self.branch)
@@ -870,27 +926,27 @@
 
     def login(self):
         return
     
     def logout(self):
         return
     
-    def download(self, file_path=None,download_to=None):
+    def __internal_download(self, file_path=None,download_to=None):
         download_to = download_to or os.path.basename(file_path)
         #https://python-gitlab.readthedocs.io/en/stable/gl_objects/projects.html#id7
 
         if download_to is None:
             download_to = os.path.join(os.curdir,file_path.split("/")[-1])
 
         if file_path and isinstance(file_path,str):
             with open(download_to,"wb+") as writer:
                 self.project.files.raw(file_path=file_path, ref=self.branch,streamed=True,action=writer.write)
         return download_to
     
-    def upload(self, file_path=None,path_in_repo=None):
+    def __internal_upload(self, file_path=None,path_in_repo=None):
         #https://python-gitlab.readthedocs.io/en/stable/gl_objects/projects.html
         with open(file_path, 'r') as my_file:
             file_content = my_file.read()
 
         if path_in_repo in self: #Update
             f = self.project.files.get(file_path=path_in_repo, ref=self.branch)
             f.content = file_content
@@ -925,20 +981,20 @@
 
     def login(self):
         return
     
     def logout(self):
         return
     
-    def download(self, file_path=None,download_to=None):
+    def __internal_download(self, file_path=None,download_to=None):
         download_to = download_to or os.path.basename(file_path)
         shutil.copy(file_path, download_to)
         return download_to
     
-    def upload(self, file_path=None,path_in_repo=None):
+    def __internal_upload(self, file_path=None,path_in_repo=None):
         shutil.copy(file_path, path_in_repo)
         return True
     
     def delete_file(self,path_in_repo=None):
         if path_in_repo in self.files():
             os.remove(path_in_repo)
         return True
@@ -955,27 +1011,27 @@
 
     def login(self):
         return
     
     def logout(self):
         return
     
-    def download(self, file_path=None,download_to=None):
+    def __internal_download(self, file_path=None,download_to=None):
         if not os.path.exists(self.location):
             print("Zip File Does Not Exist")
             return
 
         download_to = download_to or os.path.basename(file_path)
         with ZipFile(self.location) as z:
             print(download_to)
             with open(download_to, 'wb') as f:
                 f.write(z.read(file_path))
         return download_to
     
-    def upload(self, file_path=None,path_in_repo=None):
+    def __internal_upload(self, file_path=None,path_in_repo=None):
         editing_mode = 'a' if os.path.exists(self.location) else 'w'
 
         if path_in_repo in self.files():
             del self[path_in_repo]
 
         with ZipFile(self.location,editing_mode) as myzip:
             myzip.write(file_path,path_in_repo)
@@ -1010,32 +1066,21 @@
     
     def logout(self):
         return
 
     def files(self):
         return self.files
     
-    def upload(self, file_path=None,path_in_repo=None):
+    def __internal_upload(self, file_path=None,path_in_repo=None):
         return False
     
-    def download(self, file_path=None,download_to=None):
+    def __internal_download(self, file_path=None,download_to=None):
         if self.download == None:
             return False
         self.download(file_path, download_to)
-
-        #Checking if there is a custom wrapping around the file, and unwrapping
-        if file_path.endswith(".nosj"):
-            import json
-            with open(download_to, 'r') as reader:
-                content = json.load(reader)
-
-            os.remove(download_to)
-
-            with open(download_to.replace('.nosj',''), 'w+') as writer:
-                writer.write(content['contents'])
     
     def delete_file(self,path_in_repo=None):
         return False
 
 
 def redundant(klass):
     """
```

### Comparing `hugg-0.0.90/setup.py` & `hugg-0.0.91/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.90"
+VERSION = "0.0.91"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -121,15 +121,16 @@
 	},
 	install_requires=[
 		"ephfile",
 		"datasets",
 		"huggingface_hub",
 		"PyGithub", #https://pypi.org/project/PyGithub/
 		"python-gitlab",
-		"ruamel.std.zipfile"
+		"ruamel.std.zipfile",
+		"mystring"
 	],
 	include_package_data=True,
 	classifiers=[
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 3',
 		'Programming Language :: Python :: 3.8',
 	],
```

