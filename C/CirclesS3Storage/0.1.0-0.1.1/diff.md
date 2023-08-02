# Comparing `tmp/CirclesS3Storage-0.1.0.tar.gz` & `tmp/CirclesS3Storage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CirclesS3Storage-0.1.0.tar", last modified: Tue Aug  1 13:48:48 2023, max compression
+gzip compressed data, was "CirclesS3Storage-0.1.1.tar", last modified: Wed Aug  2 12:41:27 2023, max compression
```

## Comparing `CirclesS3Storage-0.1.0.tar` & `CirclesS3Storage-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:48:48.134770 CirclesS3Storage-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:48:48.130770 CirclesS3Storage-0.1.0/CirclesS3Storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-01 13:48:48.000000 CirclesS3Storage-0.1.0/CirclesS3Storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-01 13:48:48.000000 CirclesS3Storage-0.1.0/CirclesS3Storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:48:48.000000 CirclesS3Storage-0.1.0/CirclesS3Storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 13:48:48.000000 CirclesS3Storage-0.1.0/CirclesS3Storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-01 13:48:48.134770 CirclesS3Storage-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:48:48.134770 CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/AWSStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/CirclesStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/FileTypeDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/StorageDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/StorageInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:48:48.134770 CirclesS3Storage-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:48:48.134770 CirclesS3Storage-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/tests/test_S3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 13:48:28.000000 CirclesS3Storage-0.1.0/tests/test_circles_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:27.164023 CirclesS3Storage-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:27.160023 CirclesS3Storage-0.1.1/CirclesS3Storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-02 12:41:27.000000 CirclesS3Storage-0.1.1/CirclesS3Storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 12:41:27.000000 CirclesS3Storage-0.1.1/CirclesS3Storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:41:27.000000 CirclesS3Storage-0.1.1/CirclesS3Storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 12:41:27.000000 CirclesS3Storage-0.1.1/CirclesS3Storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-02 12:41:27.164023 CirclesS3Storage-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:27.164023 CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/AWSStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/CirclesStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/FileTypeDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/StorageDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/StorageInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 12:41:27.164023 CirclesS3Storage-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:27.164023 CirclesS3Storage-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/tests/test_S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-08-02 12:41:05.000000 CirclesS3Storage-0.1.1/tests/test_circles_storage.py
```

### Comparing `CirclesS3Storage-0.1.0/CirclesS3Storage.egg-info/SOURCES.txt` & `CirclesS3Storage-0.1.1/CirclesS3Storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/AWSStorage.py` & `CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/AWSStorage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-
 import os
 import boto3
 
 from circles_local_aws_s3_storage_python.StorageInterface import StorageInterface
 from circles_local_aws_s3_storage_python.StorageDB import StorageDB
-
+from circles_local_aws_s3_storage_python import constants
 
 class AwsS3Storage(StorageInterface):
 
     def __init__(self, bucket_name, region):
         self.region = region
         self.bucket_name = bucket_name
         self.database = StorageDB()
@@ -28,16 +27,16 @@
         response = self.client.put_object(
             Bucket=self.bucket_name,
             Key=remote_path+filename,
             Body=file_contents,
             ChecksumAlgorithm='crc32'
         )
         if 'ETag' in response:
-            id = self.database.uploadToDataBase(
-                remote_path, filename, self.region, created_user_id, 2, 2, 2)  # One's needs to be replaced by parameter
+            id = self.database.uploadToDatabase(
+                remote_path, filename, self.region, created_user_id, constants.STORAGE_TYPE_ID, constants.FILE_TYPE_ID, constants.EXTENSION_ID)  # Constants needs to be replaced by parameter
             return id
         return None
 
     # download a file from s3 to local_path
     def download_file(self, remote_path, local_path):
         self.client.download_file(self.bucket_name, remote_path, local_path)
```

### Comparing `CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/CirclesStorage.py` & `CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/CirclesStorage.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,28 +54,26 @@
         """
         # Use a regular expression to match only letters (A-Z and a-z)
         pattern = r"[^a-zA-Z\s]"
         preserved_string = re.sub(pattern, "", input_string)
         return preserved_string
 
 
-    def download_storage_id(self, storage_id):
+    def download_by_storage_id(self, storage_id):
         """Downlaods file from S3 to local computer using only storage id
 
         Args:
             storage_id int: Row number to get information from storage_table
         """
-        entity_reference={"Profile Image":1,"Coverage Image":2,"Personal Introduction Video":3,"Scanned Driving License":4,"Scanned Passport":5}
         select_stmt = "SELECT created_user_id, path, filename FROM storage.storage_table WHERE id = %s"
         select_data = (storage_id)
         self.db.cursor.execute(select_stmt, [select_data])
-        profile_id, entity_type, file_name = self.db.cursor.fetchall()[0]
-        entity_type_id = entity_reference[self.preserve_letters(entity_type)]
-        path = os.path.join(os.getcwd(), file_name)
-        self.download(profile_id, entity_type_id, file_name, path)
+        profile_id, folder, file_name = self.db.cursor.fetchall()[0]
+        path_local = os.path.join(os.getcwd(), file_name)
+        self.s3.download_file(folder+file_name,path_local)
         
 
 
     def download(self, profile_id, entity_type_id, file_name, local_path):
         """Downlaods file from S3 to local computer
 
         Args:
```

### Comparing `CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/FileTypeDB.py` & `CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/FileTypeDB.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,9 +13,8 @@
             database=os.getenv("RDS_DB_NAME")
         )
         self.cursor = self.mydb.cursor()
 
     def select_from_DB(self, select_stmt, select_data):
         self.cursor.execute(select_stmt, [select_data])
         folder = self.cursor.fetchone()[0]
-        print(folder)
         return folder
```

### Comparing `CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/StorageDB.py` & `CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/StorageDB.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,30 +10,25 @@
             host=os.getenv("RDS_HOSTNAME"),
             user=os.getenv("RDS_USERNAME"),
             passwd=os.getenv("RDS_PASSWORD"),
             database=os.getenv("RDS_DB_NAME")
         )
         self.cursor = self.mydb.cursor(buffered=True)
 
-    def uploadToDataBase(self, file_path, filename,  region, created_user_id, storage_type_id, file_type_id, extension_id) -> int:
-        print(file_path,filename,created_user_id)
-        print("(path, filename, region, created_user_id, updated_user_id, storage_type_id, file_type_id, file_extension_id) ")
-        print("VALUES (%s, %s, %s, %s, %s, %s, %s, %s)" % (file_path, filename, region, created_user_id,
-                        created_user_id, storage_type_id, file_type_id, extension_id))
+    def uploadToDatabase(self, file_path, filename,  region, created_user_id, storage_type_id, file_type_id, extension_id) -> int:
         add_storage = ("INSERT INTO storage.storage_table "
                        "(path, filename, region, created_user_id, updated_user_id, storage_type_id, file_type_id, file_extension_id) "
                        "VALUES (%s, %s, %s, %s, %s, %s, %s, %s)")
         storage_data = (file_path, filename, region, created_user_id,
                         created_user_id, storage_type_id, file_type_id, extension_id)
         self.cursor.execute(add_storage, storage_data)
         self.mydb.commit()
         select_stmt = "SELECT LAST_INSERT_ID()"
         self.cursor.execute(select_stmt)
         last_insert_id = self.cursor.fetchone()[0]
-        print(last_insert_id)
         return int(last_insert_id)
 
     def closeConnection(self):
         if (self.mydb != None):
             self.mydb.close
 
     def logicalDelete(self, remote_path, filename, region, updated_user_id) -> int:
```

### Comparing `CirclesS3Storage-0.1.0/circles_local_aws_s3_storage_python/StorageInterface.py` & `CirclesS3Storage-0.1.1/circles_local_aws_s3_storage_python/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `CirclesS3Storage-0.1.0/setup.py` & `CirclesS3Storage-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 setuptools.setup(
     name='CirclesS3Storage',
-    version='0.1.0', # https://pypi.org/project/storage-local/
+    version='0.1.1', # https://pypi.org/project/storage-local/
     author="Circles",
     author_email="info@circle.zone",
-    description="PyPI Package for Circles S3 functions",
+    description="PyPI Package for Circles Storage functions",
     long_description="This is a package for sharing common S3 function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/javatechy/dokr",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
          "License :: Other/Proprietary License",
```

### Comparing `CirclesS3Storage-0.1.0/tests/test_S3.py` & `CirclesS3Storage-0.1.1/tests/test_S3.py`

 * *Files identical despite different names*

### Comparing `CirclesS3Storage-0.1.0/tests/test_circles_storage.py` & `CirclesS3Storage-0.1.1/tests/test_circles_storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from circles_local_aws_s3_storage_python import constants
 from circles_local_aws_s3_storage_python.CirclesStorage import circles_storage
+from circles_local_aws_s3_storage_python.StorageDB import StorageDB
 import os
 import unittest
 from dotenv.main import load_dotenv
+import pytest
 load_dotenv()
 
 PROFILE_ID = 1
 
-
 class circles_storage_test(unittest.TestCase):
     def setUp(self) -> None:
         self.circles_storage = circles_storage()
-        print("REGION:"+str(os.getenv("REGION")))
+        self.db=StorageDB()
+        self.test = 0
+        #print("REGION:"+str(os.getenv("REGION")))
 
     def test_get_folder(self):
         actual_folder = self.circles_storage._get_folder(
             constants.PROFILE_IMAGE)
         expected_folder = 'Profile Image'
         self.assertEqual(actual_folder, expected_folder)
 
@@ -32,21 +35,20 @@
         id = self.circles_storage.put(profile_id=PROFILE_ID, entity_type_id=constants.PROFILE_IMAGE, file_name='circles_test.txt',
                                       local_file_path=filepath)
         self.assertGreater(id, 0)
 
     def test_download(self):
         cwd = os.getcwd()
         filepath = os.path.join(cwd, 'download_test.txt')
-        print(filepath)
         self.circles_storage.download(
             entity_type_id=constants.PROFILE_IMAGE, profile_id=PROFILE_ID, file_name='circles_test.txt', local_path=filepath)
         assert os.path.isfile(
             filepath)
 
     def test_download_storage_id(self):
         cwd=os.getcwd()
         filepath = os.path.join(cwd, 'download_test.txt')
-        self.circles_storage.download_storage_id(22)
+        self.circles_storage.download_by_storage_id(self.db.getLastId())
         assert os.path.isfile(filepath)
 
 if __name__ == '__main__':
     unittest.main()
```

