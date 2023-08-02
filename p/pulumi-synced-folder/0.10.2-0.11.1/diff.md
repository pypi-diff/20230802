# Comparing `tmp/pulumi_synced_folder-0.10.2.tar.gz` & `tmp/pulumi_synced_folder-0.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_synced_folder-0.10.2.tar", last modified: Thu Feb 16 19:25:41 2023, max compression
+gzip compressed data, was "pulumi_synced_folder-0.11.1.tar", last modified: Wed Aug  2 21:14:38 2023, max compression
```

## Comparing `pulumi_synced_folder-0.10.2.tar` & `pulumi_synced_folder-0.11.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:25:41.453765 pulumi_synced_folder-0.10.2/
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-02-16 19:25:41.453765 pulumi_synced_folder-0.10.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:25:41.453765 pulumi_synced_folder-0.10.2/pulumi_synced_folder/
--rw-------   0 runner    (1001) docker     (123)      881 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder/__init__.py
--rw-------   0 runner    (1001) docker     (123)     8061 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder/_utilities.py
--rw-------   0 runner    (1001) docker     (123)    11220 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder/azure_blob_folder.py
--rw-------   0 runner    (1001) docker     (123)     8907 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder/google_cloud_folder.py
--rw-------   0 runner    (1001) docker     (123)     2751 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder/provider.py
--rw-------   0 runner    (1001) docker     (123)       50 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder/py.typed
--rw-------   0 runner    (1001) docker     (123)     9967 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder/s3_bucket_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:25:41.453765 pulumi_synced_folder-0.10.2/pulumi_synced_folder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/pulumi_synced_folder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 19:25:41.453765 pulumi_synced_folder-0.10.2/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     2172 2023-02-16 19:25:41.000000 pulumi_synced_folder-0.10.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:14:38.138530 pulumi_synced_folder-0.11.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-08-02 21:14:38.138530 pulumi_synced_folder-0.11.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-08-02 21:14:37.000000 pulumi_synced_folder-0.11.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:14:38.138530 pulumi_synced_folder-0.11.1/pulumi_synced_folder/
+-rw-------   0 runner    (1001) docker     (123)      881 2023-08-02 21:14:37.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     8061 2023-08-02 21:14:37.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)    11220 2023-08-02 21:14:37.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder/azure_blob_folder.py
+-rw-------   0 runner    (1001) docker     (123)     8907 2023-08-02 21:14:37.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder/google_cloud_folder.py
+-rw-------   0 runner    (1001) docker     (123)     2751 2023-08-02 21:14:37.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder/provider.py
+-rw-------   0 runner    (1001) docker     (123)       50 2023-08-02 21:14:37.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-08-02 21:14:37.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder/py.typed
+-rw-------   0 runner    (1001) docker     (123)     9967 2023-08-02 21:14:37.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder/s3_bucket_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:14:38.138530 pulumi_synced_folder-0.11.1/pulumi_synced_folder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-08-02 21:14:38.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-02 21:14:38.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:14:38.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:14:38.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 21:14:38.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 21:14:38.000000 pulumi_synced_folder-0.11.1/pulumi_synced_folder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:14:38.138530 pulumi_synced_folder-0.11.1/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2203 2023-08-02 21:14:37.000000 pulumi_synced_folder-0.11.1/setup.py
```

### Comparing `pulumi_synced_folder-0.10.2/PKG-INFO` & `pulumi_synced_folder-0.11.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_synced_folder
-Version: 0.10.2
+Version: 0.11.1
 Summary: A Pulumi component that synchronizes a local folder to Amazon S3, Azure Blob Storage, or Google Cloud Storage.
 Home-page: https://pulumi.com
 License: UNKNOWN
 Project-URL: Repository, https://github.com/pulumi/pulumi-synced-folder
 Keywords: pulumi aws azure gcp category/cloud kind/component
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # synced-folder
 
 A Pulumi component that synchronizes a local folder to Amazon S3, Azure Blob Storage, or Google Cloud Storage.
 
 ## Installing
@@ -50,15 +51,15 @@
   s3-bucket:
     type: aws:s3:Bucket
     properties:
       acl: public-read
       website:
         indexDocument: index.html
         errorDocument: error.html
-  
+
   # 👇
   synced-bucket-folder:
     type: synced-folder:index:S3BucketFolder
     properties:
       path: ./site
       bucketName: ${s3-bucket.bucket}
       acl: public-read
@@ -128,18 +129,18 @@
       location: US
       website:
         mainPageSuffix: index.html
         notFoundPage: error.html
 
   gcp-bucket-iam-binding:
     type: gcp:storage:BucketIAMBinding
-    properties: 
+    properties:
       bucket: ${gcp-bucket.name}
       role: roles/storage.objectViewer
-      members: 
+      members:
         - allUsers
 
   # 👇
   synced-google-cloud-folder:
     type: synced-folder:index:GoogleCloudFolder
     properties:
       path: ./site
@@ -150,40 +151,40 @@
 ```
 
 ## Configuration
 
 
 The following input properties are common to all three resource types:
 
-| Property | Type | Description | 
-| -------- | ---- | ----------- | 
-| `path` | `string` | The path (relative or fully-qualified) to the folder containing the files to be synced. Required. | 
+| Property | Type | Description |
+| -------- | ---- | ----------- |
+| `path` | `string` | The path (relative or fully-qualified) to the folder containing the files to be synced. Required. |
 | `managedObjects` | `boolean` | Whether to have Pulumi manage files as individual cloud resources. Defaults to `true`. See below for details. |
 
 Additional resource-specific properties are listed below.
 
 ### `S3BucketFolder` properties
 
-| Property | Type | Description | 
-| -------- | ---- | ----------- | 
+| Property | Type | Description |
+| -------- | ---- | ----------- |
 | `bucketName` | `string` | The name of the S3 bucket to sync to (e.g., `my-bucket` in `s3://my-bucket`). Required. |
 | `acl` | `string` | The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to apply to each file (e.g., `public-read`). Required. |
 
 ### `AzureBlobFolder` properties
 
-| Property | Type | Description | 
-| -------- | ---- | ----------- | 
+| Property | Type | Description |
+| -------- | ---- | ----------- |
 | `containerName` | `string` | The name of the Azure storage container to sync to. Required. |
 | `storageAccountName` | `string` | The name of the Azure storage account that the container belongs to. Required. |
 | `resourceGroupName` | `string` | The name of the Azure resource group that the storage account belongs to. Required. |
 
 ### `GoogleCloudFolder` properties
 
-| Property | Type | Description | 
-| -------- | ---- | ----------- | 
+| Property | Type | Description |
+| -------- | ---- | ----------- |
 | `bucketName` | `string` | The name of the Google Cloud Storage bucket to sync to (e.g., `my-bucket` in `gs://my-bucket`). Required. |
 
 ## Notes
 
 ### Using the `managedObjects` property
 
 By default, the component manages your files as individual Pulumi cloud resources, but you can opt out of this behavior by setting the component's `managedObjects` property to `false`. When you do this, the component assumes you've installed the appropriate CLI tool &mdash; [`aws`](https://aws.amazon.com/cli/), [`az`](https://docs.microsoft.com/en-us/cli/azure/), or [`gcloud`/`gsutil`](https://cloud.google.com/storage/docs/gsutil), depending on the cloud &mdash; and uses the [Command](https://www.pulumi.com/registry/packages/command/) provider to issue commands on that tool directly. Files are one-way synchronized only (local to remote), and files that exist remotely but not locally are deleted. All files are deleted from remote storage on `pulumi destroy`.
@@ -192,19 +193,19 @@
 
 ```yaml
 # ...
 
 resources:
 
   # The original bucket and synced-folder resources, using managed file objects.
-  # 
+  #
   # my-first-bucket:
   #   type: aws:s3:Bucket
   #   properties:
-  #     acl: public-read  
+  #     acl: public-read
   #     website:
   #       indexDocument: index.html
   #       errorDocument: error.html
   #
   # my-first-synced-folder:
   #   type: synced-folder:index:S3BucketFolder
   #   properties:
@@ -223,15 +224,15 @@
 
   changed-my-mind-synced-folder:
     type: synced-folder:index:S3BucketFolder
     properties:
       path: ./stuff
       bucketName: ${changed-my-mind-bucket.bucket}
       acl: public-read
-      managedObjects: false 
+      managedObjects: false
 
 outputs:
 
   # An updated program reference pointing to the new bucket.
   url: http://${changed-my-mind-bucket.websiteEndpoint}
 ```
```

### Comparing `pulumi_synced_folder-0.10.2/README.md` & `pulumi_synced_folder-0.11.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
   s3-bucket:
     type: aws:s3:Bucket
     properties:
       acl: public-read
       website:
         indexDocument: index.html
         errorDocument: error.html
-  
+
   # 👇
   synced-bucket-folder:
     type: synced-folder:index:S3BucketFolder
     properties:
       path: ./site
       bucketName: ${s3-bucket.bucket}
       acl: public-read
@@ -117,18 +117,18 @@
       location: US
       website:
         mainPageSuffix: index.html
         notFoundPage: error.html
 
   gcp-bucket-iam-binding:
     type: gcp:storage:BucketIAMBinding
-    properties: 
+    properties:
       bucket: ${gcp-bucket.name}
       role: roles/storage.objectViewer
-      members: 
+      members:
         - allUsers
 
   # 👇
   synced-google-cloud-folder:
     type: synced-folder:index:GoogleCloudFolder
     properties:
       path: ./site
@@ -139,40 +139,40 @@
 ```
 
 ## Configuration
 
 
 The following input properties are common to all three resource types:
 
-| Property | Type | Description | 
-| -------- | ---- | ----------- | 
-| `path` | `string` | The path (relative or fully-qualified) to the folder containing the files to be synced. Required. | 
+| Property | Type | Description |
+| -------- | ---- | ----------- |
+| `path` | `string` | The path (relative or fully-qualified) to the folder containing the files to be synced. Required. |
 | `managedObjects` | `boolean` | Whether to have Pulumi manage files as individual cloud resources. Defaults to `true`. See below for details. |
 
 Additional resource-specific properties are listed below.
 
 ### `S3BucketFolder` properties
 
-| Property | Type | Description | 
-| -------- | ---- | ----------- | 
+| Property | Type | Description |
+| -------- | ---- | ----------- |
 | `bucketName` | `string` | The name of the S3 bucket to sync to (e.g., `my-bucket` in `s3://my-bucket`). Required. |
 | `acl` | `string` | The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to apply to each file (e.g., `public-read`). Required. |
 
 ### `AzureBlobFolder` properties
 
-| Property | Type | Description | 
-| -------- | ---- | ----------- | 
+| Property | Type | Description |
+| -------- | ---- | ----------- |
 | `containerName` | `string` | The name of the Azure storage container to sync to. Required. |
 | `storageAccountName` | `string` | The name of the Azure storage account that the container belongs to. Required. |
 | `resourceGroupName` | `string` | The name of the Azure resource group that the storage account belongs to. Required. |
 
 ### `GoogleCloudFolder` properties
 
-| Property | Type | Description | 
-| -------- | ---- | ----------- | 
+| Property | Type | Description |
+| -------- | ---- | ----------- |
 | `bucketName` | `string` | The name of the Google Cloud Storage bucket to sync to (e.g., `my-bucket` in `gs://my-bucket`). Required. |
 
 ## Notes
 
 ### Using the `managedObjects` property
 
 By default, the component manages your files as individual Pulumi cloud resources, but you can opt out of this behavior by setting the component's `managedObjects` property to `false`. When you do this, the component assumes you've installed the appropriate CLI tool &mdash; [`aws`](https://aws.amazon.com/cli/), [`az`](https://docs.microsoft.com/en-us/cli/azure/), or [`gcloud`/`gsutil`](https://cloud.google.com/storage/docs/gsutil), depending on the cloud &mdash; and uses the [Command](https://www.pulumi.com/registry/packages/command/) provider to issue commands on that tool directly. Files are one-way synchronized only (local to remote), and files that exist remotely but not locally are deleted. All files are deleted from remote storage on `pulumi destroy`.
@@ -181,19 +181,19 @@
 
 ```yaml
 # ...
 
 resources:
 
   # The original bucket and synced-folder resources, using managed file objects.
-  # 
+  #
   # my-first-bucket:
   #   type: aws:s3:Bucket
   #   properties:
-  #     acl: public-read  
+  #     acl: public-read
   #     website:
   #       indexDocument: index.html
   #       errorDocument: error.html
   #
   # my-first-synced-folder:
   #   type: synced-folder:index:S3BucketFolder
   #   properties:
@@ -212,14 +212,14 @@
 
   changed-my-mind-synced-folder:
     type: synced-folder:index:S3BucketFolder
     properties:
       path: ./stuff
       bucketName: ${changed-my-mind-bucket.bucket}
       acl: public-read
-      managedObjects: false 
+      managedObjects: false
 
 outputs:
 
   # An updated program reference pointing to the new bucket.
   url: http://${changed-my-mind-bucket.websiteEndpoint}
 ```
```

### Comparing `pulumi_synced_folder-0.10.2/pulumi_synced_folder/__init__.py` & `pulumi_synced_folder-0.11.1/pulumi_synced_folder/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_synced_folder-0.10.2/pulumi_synced_folder/_utilities.py` & `pulumi_synced_folder-0.11.1/pulumi_synced_folder/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_synced_folder-0.10.2/pulumi_synced_folder/azure_blob_folder.py` & `pulumi_synced_folder-0.11.1/pulumi_synced_folder/azure_blob_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_synced_folder-0.10.2/pulumi_synced_folder/google_cloud_folder.py` & `pulumi_synced_folder-0.11.1/pulumi_synced_folder/google_cloud_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_synced_folder-0.10.2/pulumi_synced_folder/provider.py` & `pulumi_synced_folder-0.11.1/pulumi_synced_folder/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_synced_folder-0.10.2/pulumi_synced_folder/s3_bucket_folder.py` & `pulumi_synced_folder-0.11.1/pulumi_synced_folder/s3_bucket_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_synced_folder-0.10.2/pulumi_synced_folder.egg-info/PKG-INFO` & `pulumi_synced_folder-0.11.1/pulumi_synced_folder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-synced-folder
-Version: 0.10.2
+Version: 0.11.1
 Summary: A Pulumi component that synchronizes a local folder to Amazon S3, Azure Blob Storage, or Google Cloud Storage.
 Home-page: https://pulumi.com
 License: UNKNOWN
 Project-URL: Repository, https://github.com/pulumi/pulumi-synced-folder
 Keywords: pulumi aws azure gcp category/cloud kind/component
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # synced-folder
 
 A Pulumi component that synchronizes a local folder to Amazon S3, Azure Blob Storage, or Google Cloud Storage.
 
 ## Installing
@@ -50,15 +51,15 @@
   s3-bucket:
     type: aws:s3:Bucket
     properties:
       acl: public-read
       website:
         indexDocument: index.html
         errorDocument: error.html
-  
+
   # 👇
   synced-bucket-folder:
     type: synced-folder:index:S3BucketFolder
     properties:
       path: ./site
       bucketName: ${s3-bucket.bucket}
       acl: public-read
@@ -128,18 +129,18 @@
       location: US
       website:
         mainPageSuffix: index.html
         notFoundPage: error.html
 
   gcp-bucket-iam-binding:
     type: gcp:storage:BucketIAMBinding
-    properties: 
+    properties:
       bucket: ${gcp-bucket.name}
       role: roles/storage.objectViewer
-      members: 
+      members:
         - allUsers
 
   # 👇
   synced-google-cloud-folder:
     type: synced-folder:index:GoogleCloudFolder
     properties:
       path: ./site
@@ -150,40 +151,40 @@
 ```
 
 ## Configuration
 
 
 The following input properties are common to all three resource types:
 
-| Property | Type | Description | 
-| -------- | ---- | ----------- | 
-| `path` | `string` | The path (relative or fully-qualified) to the folder containing the files to be synced. Required. | 
+| Property | Type | Description |
+| -------- | ---- | ----------- |
+| `path` | `string` | The path (relative or fully-qualified) to the folder containing the files to be synced. Required. |
 | `managedObjects` | `boolean` | Whether to have Pulumi manage files as individual cloud resources. Defaults to `true`. See below for details. |
 
 Additional resource-specific properties are listed below.
 
 ### `S3BucketFolder` properties
 
-| Property | Type | Description | 
-| -------- | ---- | ----------- | 
+| Property | Type | Description |
+| -------- | ---- | ----------- |
 | `bucketName` | `string` | The name of the S3 bucket to sync to (e.g., `my-bucket` in `s3://my-bucket`). Required. |
 | `acl` | `string` | The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to apply to each file (e.g., `public-read`). Required. |
 
 ### `AzureBlobFolder` properties
 
-| Property | Type | Description | 
-| -------- | ---- | ----------- | 
+| Property | Type | Description |
+| -------- | ---- | ----------- |
 | `containerName` | `string` | The name of the Azure storage container to sync to. Required. |
 | `storageAccountName` | `string` | The name of the Azure storage account that the container belongs to. Required. |
 | `resourceGroupName` | `string` | The name of the Azure resource group that the storage account belongs to. Required. |
 
 ### `GoogleCloudFolder` properties
 
-| Property | Type | Description | 
-| -------- | ---- | ----------- | 
+| Property | Type | Description |
+| -------- | ---- | ----------- |
 | `bucketName` | `string` | The name of the Google Cloud Storage bucket to sync to (e.g., `my-bucket` in `gs://my-bucket`). Required. |
 
 ## Notes
 
 ### Using the `managedObjects` property
 
 By default, the component manages your files as individual Pulumi cloud resources, but you can opt out of this behavior by setting the component's `managedObjects` property to `false`. When you do this, the component assumes you've installed the appropriate CLI tool &mdash; [`aws`](https://aws.amazon.com/cli/), [`az`](https://docs.microsoft.com/en-us/cli/azure/), or [`gcloud`/`gsutil`](https://cloud.google.com/storage/docs/gsutil), depending on the cloud &mdash; and uses the [Command](https://www.pulumi.com/registry/packages/command/) provider to issue commands on that tool directly. Files are one-way synchronized only (local to remote), and files that exist remotely but not locally are deleted. All files are deleted from remote storage on `pulumi destroy`.
@@ -192,19 +193,19 @@
 
 ```yaml
 # ...
 
 resources:
 
   # The original bucket and synced-folder resources, using managed file objects.
-  # 
+  #
   # my-first-bucket:
   #   type: aws:s3:Bucket
   #   properties:
-  #     acl: public-read  
+  #     acl: public-read
   #     website:
   #       indexDocument: index.html
   #       errorDocument: error.html
   #
   # my-first-synced-folder:
   #   type: synced-folder:index:S3BucketFolder
   #   properties:
@@ -223,15 +224,15 @@
 
   changed-my-mind-synced-folder:
     type: synced-folder:index:S3BucketFolder
     properties:
       path: ./stuff
       bucketName: ${changed-my-mind-bucket.bucket}
       acl: public-read
-      managedObjects: false 
+      managedObjects: false
 
 outputs:
 
   # An updated program reference pointing to the new bucket.
   url: http://${changed-my-mind-bucket.websiteEndpoint}
 ```
```

### Comparing `pulumi_synced_folder-0.10.2/pulumi_synced_folder.egg-info/SOURCES.txt` & `pulumi_synced_folder-0.11.1/pulumi_synced_folder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_synced_folder-0.10.2/setup.py` & `pulumi_synced_folder-0.11.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.10.2"
-PLUGIN_VERSION = "0.10.2"
+VERSION = "0.11.1"
+PLUGIN_VERSION = "0.11.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'synced-folder', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "synced-folder Pulumi Package - Development Version"
 
 
 setup(name='pulumi_synced_folder',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi component that synchronizes a local folder to Amazon S3, Azure Blob Storage, or Google Cloud Storage.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

