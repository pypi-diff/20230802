# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.947.tar", last modified: Tue Aug  1 00:32:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.948.tar", last modified: Wed Aug  2 00:25:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.947.tar` & `tencentcloud-sdk-python-cdb-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/cdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/cdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   146951 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19678 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   798528 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:32:39.000000 tencentcloud-sdk-python-cdb-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/cdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/cdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   146951 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19678 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   798528 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud_sdk_python_cdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-02 00:25:11.000000 tencentcloud-sdk-python-cdb-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.947/setup.py` & `tencentcloud-sdk-python-cdb-3.0.948/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cdb',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cdb SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.947/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.948/tencentcloud/cdb/v20170320/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.947/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.948/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.948/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.947/README.rst` & `tencentcloud-sdk-python-cdb-3.0.948/README.rst`

 * *Files identical despite different names*
