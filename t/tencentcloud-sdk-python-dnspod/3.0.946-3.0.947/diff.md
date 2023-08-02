# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.946.tar", last modified: Mon Jul 31 00:24:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.947.tar", last modified: Tue Aug  1 00:36:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.946.tar` & `tencentcloud-sdk-python-dnspod-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/dnspod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/dnspod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    61922 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24132 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   351981 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-31 00:24:59.000000 tencentcloud-sdk-python-dnspod-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/dnspod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/dnspod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    61922 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24132 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   351981 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-08-01 00:36:07.000000 tencentcloud-sdk-python-dnspod-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.946/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud/dnspod/v20210323/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.947/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.946/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.947/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.946/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.947/README.rst`

 * *Files identical despite different names*

