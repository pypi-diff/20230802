# Comparing `tmp/curlgoogle-0.0.2.tar.gz` & `tmp/curlgoogle-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curlgoogle-0.0.2.tar", last modified: Sun Jul 16 18:23:12 2023, max compression
+gzip compressed data, was "curlgoogle-0.0.3.tar", last modified: Wed Aug  2 19:47:45 2023, max compression
```

## Comparing `curlgoogle-0.0.2.tar` & `curlgoogle-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:23:12.841280 curlgoogle-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-16 18:22:58.000000 curlgoogle-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-16 18:23:12.841280 curlgoogle-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-16 18:22:58.000000 curlgoogle-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:23:12.841280 curlgoogle-0.0.2/curlgoogle/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-16 18:22:58.000000 curlgoogle-0.0.2/curlgoogle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-16 18:22:58.000000 curlgoogle-0.0.2/curlgoogle/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-16 18:22:58.000000 curlgoogle-0.0.2/curlgoogle/curlgoogledownload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-16 18:22:58.000000 curlgoogle-0.0.2/curlgoogle/curlgoogleupload.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-16 18:22:58.000000 curlgoogle-0.0.2/curlgoogle/info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:23:12.841280 curlgoogle-0.0.2/curlgoogle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-16 18:23:12.000000 curlgoogle-0.0.2/curlgoogle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-16 18:23:12.000000 curlgoogle-0.0.2/curlgoogle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:23:12.000000 curlgoogle-0.0.2/curlgoogle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-16 18:23:12.000000 curlgoogle-0.0.2/curlgoogle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 18:23:12.000000 curlgoogle-0.0.2/curlgoogle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 18:23:12.841280 curlgoogle-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-16 18:22:58.000000 curlgoogle-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:47:45.751317 curlgoogle-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 19:47:31.000000 curlgoogle-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-08-02 19:47:45.751317 curlgoogle-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-08-02 19:47:31.000000 curlgoogle-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:47:45.751317 curlgoogle-0.0.3/curlgoogle/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 19:47:31.000000 curlgoogle-0.0.3/curlgoogle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-02 19:47:31.000000 curlgoogle-0.0.3/curlgoogle/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-02 19:47:31.000000 curlgoogle-0.0.3/curlgoogle/curlgoogledownload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-08-02 19:47:31.000000 curlgoogle-0.0.3/curlgoogle/curlgoogleupload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 19:47:31.000000 curlgoogle-0.0.3/curlgoogle/info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:47:45.751317 curlgoogle-0.0.3/curlgoogle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-08-02 19:47:45.000000 curlgoogle-0.0.3/curlgoogle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-02 19:47:45.000000 curlgoogle-0.0.3/curlgoogle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:47:45.000000 curlgoogle-0.0.3/curlgoogle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-02 19:47:45.000000 curlgoogle-0.0.3/curlgoogle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 19:47:45.000000 curlgoogle-0.0.3/curlgoogle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:47:45.751317 curlgoogle-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-02 19:47:31.000000 curlgoogle-0.0.3/setup.py
```

### Comparing `curlgoogle-0.0.2/LICENSE` & `curlgoogle-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `curlgoogle-0.0.2/PKG-INFO` & `curlgoogle-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curlgoogle
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple lightweight python package for curl-based requests to google drive.
 Home-page: https://github.com/HamidrezaKmK/curlgoogle
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: MIT
 Description: # CurlGoogle
         [![PyPI](https://img.shields.io/pypi/v/curlgoogle.svg?color=green)](https://pypi.org/project/curlgoogle/)
@@ -55,23 +55,29 @@
         
         **important node**: You should extract the file or folder identifiers from their corresponding link.
         
         #### CLI
         
         Use the following format for download and upload
         ```bash
-        curlgoogle_upload <file_name> <file1> <file2> ... <fileN> (optional)<folder_id>
+        curlgoogle_upload <file/folder-1> <file/folder-2> ... <file/folder-N> (optional)<folder_id>
+        ```
+        This will upload all your files or folders into a folder with the specified identifier.
+        
+        You can also pick a bunch of folders or files, zip them into a single file with a specific name and then upload them all at once using the following convention:
+        
+        ```bash
+        curlgoogle_upload <file/folder-1> <file/folder-2> ... <file/folder-N> (optional)<folder_id> -m -n <zip_file_name>
         ```
-        `file_name` will determine the `zip` file that will be created and uploaded to your Google Drive. `file1` to `fileN` are the files that you want to upload. `file_id` is the id of the folder you want to upload to. If you do not specify a `file_id`, the file will be uploaded to the root directory of your Google Drive.
         
         For download use the following format:
         ```bash
-        curlgoogle_download <file_id>
+        curlgoogle_download <file_id1> <file_id2> ... <file_idN>
         ```
-        This will automatically download the file with the specified `file_id` to your current directory and unzip it for you.
+        This will automatically download the files and extract them.
         
         ### SDK
         
         You can also use the following functions for upload and download while development. Note that this will automatically prompt you to authenticate your Google account mid-run; therefore, it might not be the ideal use case for production.
         
         ```python
         # Uplaoding function
```

### Comparing `curlgoogle-0.0.2/README.md` & `curlgoogle-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -47,23 +47,29 @@
 
 **important node**: You should extract the file or folder identifiers from their corresponding link.
 
 #### CLI
 
 Use the following format for download and upload
 ```bash
-curlgoogle_upload <file_name> <file1> <file2> ... <fileN> (optional)<folder_id>
+curlgoogle_upload <file/folder-1> <file/folder-2> ... <file/folder-N> (optional)<folder_id>
+```
+This will upload all your files or folders into a folder with the specified identifier.
+
+You can also pick a bunch of folders or files, zip them into a single file with a specific name and then upload them all at once using the following convention:
+
+```bash
+curlgoogle_upload <file/folder-1> <file/folder-2> ... <file/folder-N> (optional)<folder_id> -m -n <zip_file_name>
 ```
-`file_name` will determine the `zip` file that will be created and uploaded to your Google Drive. `file1` to `fileN` are the files that you want to upload. `file_id` is the id of the folder you want to upload to. If you do not specify a `file_id`, the file will be uploaded to the root directory of your Google Drive.
 
 For download use the following format:
 ```bash
-curlgoogle_download <file_id>
+curlgoogle_download <file_id1> <file_id2> ... <file_idN>
 ```
-This will automatically download the file with the specified `file_id` to your current directory and unzip it for you.
+This will automatically download the files and extract them.
 
 ### SDK
 
 You can also use the following functions for upload and download while development. Note that this will automatically prompt you to authenticate your Google account mid-run; therefore, it might not be the ideal use case for production.
 
 ```python
 # Uplaoding function
```

### Comparing `curlgoogle-0.0.2/curlgoogle/console.py` & `curlgoogle-0.0.3/curlgoogle/console.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 import os 
 from .curlgoogleupload import upload as upload_sdk
 from .curlgoogledownload import download as download_sdk
 import argparse
 
-client_id = None
-client_secret = None
-
 def upload():
     # parse arguments
     parser = argparse.ArgumentParser()
-    parser.add_argument("name", help="Name for the output zip file")
     parser.add_argument("filepaths", nargs='+', help="Files or directories to include in the zip file")
     parser.add_argument("-r", "--recursive", action="store_true", 
                         help="Zip directories recursively", default=True)
     parser.add_argument("-d", "--directory_id", 
                         help="Google Drive directory ID to upload the zip file to")
     parser.add_argument("-z", "--zip", action="store_true", help="Zip the files",
                         default=True)
+    parser.add_argument("-m", "--multifile", action="store_true", help="When set to true every file will be compressed into a zip with name=name and then uploaded")
+    parser.add_argument("-n", "--name", help="Name of the zip file")
     args = parser.parse_args()
-
+    
+    if args.multifile:
+        if args.name is None:
+            print("Please specify the name of the zip to aggregate files using -n")
+            return
+    
     upload_sdk(
         filepaths=args.filepaths,
         zip=args.zip,
         recursive=args.recursive,
         name=args.name,
         directory_id=args.directory_id,
+        multifile=args.multifile,
     )
 
 def download():
     # parse arguments
     parser = argparse.ArgumentParser()
-    parser.add_argument("file_id", help="Google Drive file ID to download")
+    parser.add_argument("file_ids", nargs="+", help="Google Drive file ID to download")
     parser.add_argument("-u", "--unzip", action="store_true", 
                         help="Unzip the downloaded file if it's a zip file", default=True)
     args = parser.parse_args()
     
     download_sdk(
-        file_id=args.file_id,
+        file_ids=args.file_ids,
         unzip=args.unzip,
     )
```

### Comparing `curlgoogle-0.0.2/curlgoogle/curlgoogledownload.py` & `curlgoogle-0.0.3/curlgoogle/curlgoogledownload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 A Python script to automate file download from Google Drive and optional unzipping.
 '''
 import os, json, requests, zipfile
 from .info import get_client_info
 
 def download(
-    file_id,
+    file_ids: list,
     unzip: bool = True,
 ):
     """
     This download function sdk provides a simple interface to download files from google drive.
     Using the file_id you can download the file from google drive and if unzip is set to
     true, then the file will be unzipped automatically.
 
@@ -23,27 +23,28 @@
     cmd1 = json.loads(os.popen('curl -d "client_id=%s&scope=https://www.googleapis.com/auth/drive.file" https://oauth2.googleapis.com/device/code'%client_id).read())
     input('\n Enter %(user_code)s\n\n at %(verification_url)s \n\n Then hit Enter to continue.'%cmd1)
     input('(twice)')
 
     # get token
     cmd2 = json.loads(os.popen(('curl -d client_id=%s -d client_secret=%s -d device_code=%s -d grant_type=urn~~3Aietf~~3Aparams~~3Aoauth~~3Agrant-type~~3Adevice_code https://accounts.google.com/o/oauth2/token'%(client_id,client_secret,cmd1['device_code'])).replace('~~','%')).read())
 
-    # download the file
-    filename = 'file_from_drive.zip'
-    url = "https://www.googleapis.com/drive/v3/files/%s?alt=media" % file_id
-    headers = {"Authorization": "Bearer %s" % cmd2["access_token"]}
-    response = requests.get(url, headers=headers)
-
-    # save the file
-    with open(filename, 'wb') as f:
-        f.write(response.content)
-
-    # unzip the file if -u is specified and the file is a zip file
-    if unzip and zipfile.is_zipfile(filename):
-        with zipfile.ZipFile(filename, 'r') as zip_ref:
-            zip_ref.extractall('.')
-        print('File unzipped successfully.')
-        # remove the zip file
-        os.remove(filename)
-    else:
-        print('File downloaded successfully.')
+    for file_id in file_ids:
+        # download the file
+        filename = 'file_from_drive.zip'
+        url = "https://www.googleapis.com/drive/v3/files/%s?alt=media" % file_id
+        headers = {"Authorization": "Bearer %s" % cmd2["access_token"]}
+        response = requests.get(url, headers=headers)
+
+        # save the file
+        with open(filename, 'wb') as f:
+            f.write(response.content)
+
+        # unzip the file if -u is specified and the file is a zip file
+        if unzip and zipfile.is_zipfile(filename):
+            with zipfile.ZipFile(filename, 'r') as zip_ref:
+                zip_ref.extractall('.')
+            print('File unzipped successfully.')
+            # remove the zip file
+            os.remove(filename)
+        else:
+            print('File downloaded successfully.')
```

### Comparing `curlgoogle-0.0.2/curlgoogle/curlgoogleupload.py` & `curlgoogle-0.0.3/curlgoogle/curlgoogleupload.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 
 '''
 A Python script to automate curl->googledrive interfacing
 This should require nothing more than the system python version and curl. 
 Dan Ellis 2020
 '''
 import os, sys, json, zipfile
+import typing as th
 
 if sys.version[0] == '3':
     raw_input = lambda x: input(x)
 
 from .info import get_client_info
 
 
 def upload(
     filepaths,
-    name: str,
     directory_id: str,
+    name: th.Optional[str] = None,
     zip: bool = True,
     recursive: bool = True,
+    multifile: bool = False,
 ):
     """
     This upload function sdk provides a simple interface to upload files to google drive.
     You can enter the directory id and a set of filepaths to upload.
     If zip is set to true, then all the files will be zipped into a single file;
     then, that file would be uploaded into the directory. If recursive is set to true,
     all the files will be recursively iterated.
@@ -43,35 +45,65 @@
     raw_input('(twice)')
 
     # get token
     cmd2 = json.loads(os.popen(('curl -d client_id=%s -d client_secret=%s -d device_code=%s -d grant_type=urn~~3Aietf~~3Aparams~~3Aoauth~~3Agrant-type~~3Adevice_code https://accounts.google.com/o/oauth2/token'%(client_id,client_secret,cmd1['device_code'])).replace('~~','%')).read())
 
     # zip files if -z is specified
     remove_file_after_upload = False
-    filepath = filepaths[0] # use the first file if not zipping
-    if zip:
-        with zipfile.ZipFile('%s.zip'%name, 'w') as myzip:
-            for path in filepaths:
-                if recursive and os.path.isdir(path):
-                    for dirpath, dirnames, files in os.walk(path):
+    if not multifile:
+        for i, filepath in enumerate(filepaths):
+            # get the name of filepath if it is not a directory
+            
+            print(f"uploading file [{i+1}/{len(filepaths)}]")
+            with zipfile.ZipFile('%s.zip'%filepath, 'w') as myzip:
+                if recursive and os.path.isdir(filepath):
+                    for dirpath, dirnames, files in os.walk(filepath):
                         for name_ in files:
                             myzip.write(os.path.join(dirpath, name_))
                 else:
-                    myzip.write(path)
-        filepath = '%s.zip'%name
-        remove_file_after_upload = True
-
-    # upload to drive
-    metadata = { "name" : name }
-    if directory_id:
-        metadata["parents"] = [directory_id]
-    metadata_str = json.dumps(metadata) # use json.dumps to properly format the json string
-    cmd4 = os.popen('''
-    curl -X POST -L -H "Authorization: Bearer %s" -F 'metadata=%s;type=application/json;charset=UTF-8' -F "file=@%s;type=application/zip" "https://www.googleapis.com/upload/drive/v3/files?uploadType=multipart"
-    '''%(cmd2["access_token"],metadata_str,filepath)).read()
-    
-    if remove_file_after_upload:
-        os.remove(filepath)
+                    myzip.write(filepath)
+            file_path = '%s.zip'%filepath
+            remove_file_after_upload = True
+            # upload to drive
+            metadata = { "name" : filepath }
+            if directory_id:
+                metadata["parents"] = [directory_id]
+            metadata_str = json.dumps(metadata) # use json.dumps to properly format the json string
+            cmd4 = os.popen('''
+            curl -X POST -L -H "Authorization: Bearer %s" -F 'metadata=%s;type=application/json;charset=UTF-8' -F "file=@%s;type=application/zip" "https://www.googleapis.com/upload/drive/v3/files?uploadType=multipart"
+            '''%(cmd2["access_token"],metadata_str,file_path)).read()
+            
+            if remove_file_after_upload:
+                os.remove(file_path)
+                
+            print(cmd4)
+            print('end')
+            print("=====", end='\n\n')
+    else:
+        filepath = filepaths[0] # use the first file if not zipping
+        if zip:
+            with zipfile.ZipFile('%s.zip'%name, 'w') as myzip:
+                for path in filepaths:
+                    if recursive and os.path.isdir(path):
+                        for dirpath, dirnames, files in os.walk(path):
+                            for name_ in files:
+                                myzip.write(os.path.join(dirpath, name_))
+                    else:
+                        myzip.write(path)
+            filepath = '%s.zip'%name
+            remove_file_after_upload = True
+
+        # upload to drive
+        metadata = { "name" : name }
+        if directory_id:
+            metadata["parents"] = [directory_id]
+        metadata_str = json.dumps(metadata) # use json.dumps to properly format the json string
+        cmd4 = os.popen('''
+        curl -X POST -L -H "Authorization: Bearer %s" -F 'metadata=%s;type=application/json;charset=UTF-8' -F "file=@%s;type=application/zip" "https://www.googleapis.com/upload/drive/v3/files?uploadType=multipart"
+        '''%(cmd2["access_token"],metadata_str,filepath)).read()
         
-    print(cmd4)
-    print('end')
+        if remove_file_after_upload:
+            os.remove(filepath)
+            
+        print(cmd4)
+        print('end')
```

### Comparing `curlgoogle-0.0.2/curlgoogle.egg-info/PKG-INFO` & `curlgoogle-0.0.3/curlgoogle.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curlgoogle
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple lightweight python package for curl-based requests to google drive.
 Home-page: https://github.com/HamidrezaKmK/curlgoogle
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: MIT
 Description: # CurlGoogle
         [![PyPI](https://img.shields.io/pypi/v/curlgoogle.svg?color=green)](https://pypi.org/project/curlgoogle/)
@@ -55,23 +55,29 @@
         
         **important node**: You should extract the file or folder identifiers from their corresponding link.
         
         #### CLI
         
         Use the following format for download and upload
         ```bash
-        curlgoogle_upload <file_name> <file1> <file2> ... <fileN> (optional)<folder_id>
+        curlgoogle_upload <file/folder-1> <file/folder-2> ... <file/folder-N> (optional)<folder_id>
+        ```
+        This will upload all your files or folders into a folder with the specified identifier.
+        
+        You can also pick a bunch of folders or files, zip them into a single file with a specific name and then upload them all at once using the following convention:
+        
+        ```bash
+        curlgoogle_upload <file/folder-1> <file/folder-2> ... <file/folder-N> (optional)<folder_id> -m -n <zip_file_name>
         ```
-        `file_name` will determine the `zip` file that will be created and uploaded to your Google Drive. `file1` to `fileN` are the files that you want to upload. `file_id` is the id of the folder you want to upload to. If you do not specify a `file_id`, the file will be uploaded to the root directory of your Google Drive.
         
         For download use the following format:
         ```bash
-        curlgoogle_download <file_id>
+        curlgoogle_download <file_id1> <file_id2> ... <file_idN>
         ```
-        This will automatically download the file with the specified `file_id` to your current directory and unzip it for you.
+        This will automatically download the files and extract them.
         
         ### SDK
         
         You can also use the following functions for upload and download while development. Note that this will automatically prompt you to authenticate your Google account mid-run; therefore, it might not be the ideal use case for production.
         
         ```python
         # Uplaoding function
```

### Comparing `curlgoogle-0.0.2/setup.py` & `curlgoogle-0.0.3/setup.py`

 * *Files identical despite different names*

