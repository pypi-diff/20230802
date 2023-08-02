# Comparing `tmp/tencentcloud-sdk-python-batch-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-batch-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.946.tar", last modified: Mon Jul 31 00:19:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.947.tar", last modified: Tue Aug  1 00:19:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-batch-3.0.946.tar` & `tencentcloud-sdk-python-batch-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud/batch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud/batch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud/batch/v20170312/
--rw-r--r--   0 root         (0) root         (0)    31661 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud/batch/v20170312/batch_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud/batch/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8635 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud/batch/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   299742 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud/batch/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud_sdk_python_batch.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/tencentcloud_sdk_python_batch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-31 00:19:29.000000 tencentcloud-sdk-python-batch-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud/batch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud/batch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud/batch/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    31661 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud/batch/v20170312/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud/batch/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8635 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud/batch/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   299742 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud/batch/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud_sdk_python_batch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/tencentcloud_sdk_python_batch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-08-01 00:19:44.000000 tencentcloud-sdk-python-batch-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-batch-3.0.946/setup.py` & `tencentcloud-sdk-python-batch-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-batch-3.0.947/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.946'
+__version__ = '3.0.947'
```

### Comparing `tencentcloud-sdk-python-batch-3.0.946/tencentcloud/batch/v20170312/batch_client.py` & `tencentcloud-sdk-python-batch-3.0.947/tencentcloud/batch/v20170312/batch_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.946/tencentcloud/batch/v20170312/errorcodes.py` & `tencentcloud-sdk-python-batch-3.0.947/tencentcloud/batch/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.946/tencentcloud/batch/v20170312/models.py` & `tencentcloud-sdk-python-batch-3.0.947/tencentcloud/batch/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.946/tencentcloud_sdk_python_batch.egg-info/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.947/tencentcloud_sdk_python_batch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.947/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.946/README.rst` & `tencentcloud-sdk-python-batch-3.0.947/README.rst`

 * *Files identical despite different names*

