# Comparing `tmp/tencentcloud-sdk-python-ticm-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-ticm-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ticm-3.0.947.tar", last modified: Tue Aug  1 00:57:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ticm-3.0.948.tar", last modified: Wed Aug  2 00:39:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ticm-3.0.947.tar` & `tencentcloud-sdk-python-ticm-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/ticm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/ticm/v20181127/
--rw-r--r--   0 root         (0) root         (0)     4025 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/ticm/v20181127/ticm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/ticm/v20181127/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1329 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/ticm/v20181127/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80377 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/ticm/v20181127/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/ticm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud_sdk_python_ticm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud_sdk_python_ticm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud_sdk_python_ticm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud_sdk_python_ticm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/tencentcloud_sdk_python_ticm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-08-01 00:57:58.000000 tencentcloud-sdk-python-ticm-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/ticm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/ticm/v20181127/
+-rw-r--r--   0 root         (0) root         (0)     4025 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/ticm/v20181127/ticm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/ticm/v20181127/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1329 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/ticm/v20181127/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80377 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/ticm/v20181127/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/ticm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud_sdk_python_ticm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud_sdk_python_ticm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      506 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud_sdk_python_ticm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud_sdk_python_ticm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud_sdk_python_ticm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/tencentcloud_sdk_python_ticm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-02 00:39:26.000000 tencentcloud-sdk-python-ticm-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-ticm-3.0.947/setup.py` & `tencentcloud-sdk-python-ticm-3.0.948/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-ticm',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Ticm SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/ticm/v20181127/ticm_client.py` & `tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/ticm/v20181127/ticm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/ticm/v20181127/errorcodes.py` & `tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/ticm/v20181127/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/ticm/v20181127/models.py` & `tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/ticm/v20181127/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ticm-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ticm-3.0.948/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.947'
+__version__ = '3.0.948'
```

### Comparing `tencentcloud-sdk-python-ticm-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-ticm-3.0.948/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ticm
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Ticm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ticm-3.0.947/tencentcloud_sdk_python_ticm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ticm-3.0.948/tencentcloud_sdk_python_ticm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ticm
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Ticm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ticm-3.0.947/README.rst` & `tencentcloud-sdk-python-ticm-3.0.948/README.rst`

 * *Files identical despite different names*

