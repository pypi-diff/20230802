# Comparing `tmp/tencentcloud-sdk-python-rp-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-rp-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-rp-3.0.947.tar", last modified: Tue Aug  1 00:54:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-rp-3.0.948.tar", last modified: Wed Aug  2 00:35:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-rp-3.0.947.tar` & `tencentcloud-sdk-python-rp-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud/rp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud/rp/v20200224/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud/rp/v20200224/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2224 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud/rp/v20200224/rp_client.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud/rp/v20200224/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    16086 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud/rp/v20200224/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud/rp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud_sdk_python_rp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud_sdk_python_rp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud_sdk_python_rp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud_sdk_python_rp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/tencentcloud_sdk_python_rp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-08-01 00:54:15.000000 tencentcloud-sdk-python-rp-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:35:54.000000 tencentcloud-sdk-python-rp-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-08-02 00:35:53.000000 tencentcloud-sdk-python-rp-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:35:54.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:35:54.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud/rp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:35:54.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud/rp/v20200224/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:35:53.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud/rp/v20200224/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2023-08-02 00:35:53.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud/rp/v20200224/rp_client.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-08-02 00:35:53.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud/rp/v20200224/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    16086 2023-08-02 00:35:53.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud/rp/v20200224/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:35:53.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud/rp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:35:53.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:35:54.000000 tencentcloud-sdk-python-rp-3.0.948/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:35:54.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud_sdk_python_rp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:35:54.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud_sdk_python_rp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      484 2023-08-02 00:35:54.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud_sdk_python_rp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:35:54.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud_sdk_python_rp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-08-02 00:35:54.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud_sdk_python_rp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:35:54.000000 tencentcloud-sdk-python-rp-3.0.948/tencentcloud_sdk_python_rp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-08-02 00:35:54.000000 tencentcloud-sdk-python-rp-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-08-02 00:35:53.000000 tencentcloud-sdk-python-rp-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-rp-3.0.947/setup.py` & `tencentcloud-sdk-python-rp-3.0.948/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-rp',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Rp SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-rp-3.0.947/tencentcloud/rp/v20200224/rp_client.py` & `tencentcloud-sdk-python-rp-3.0.948/tencentcloud/rp/v20200224/rp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rp-3.0.947/tencentcloud/rp/v20200224/errorcodes.py` & `tencentcloud-sdk-python-rp-3.0.948/tencentcloud/rp/v20200224/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rp-3.0.947/tencentcloud/rp/v20200224/models.py` & `tencentcloud-sdk-python-rp-3.0.948/tencentcloud/rp/v20200224/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rp-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-rp-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-rp-3.0.947/tencentcloud_sdk_python_rp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-rp-3.0.948/tencentcloud_sdk_python_rp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rp
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Rp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rp-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-rp-3.0.948/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rp
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Rp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rp-3.0.947/README.rst` & `tencentcloud-sdk-python-rp-3.0.948/README.rst`

 * *Files identical despite different names*

