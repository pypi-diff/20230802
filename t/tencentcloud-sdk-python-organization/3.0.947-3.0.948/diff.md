# Comparing `tmp/tencentcloud-sdk-python-organization-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-organization-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-organization-3.0.947.tar", last modified: Tue Aug  1 00:53:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-organization-3.0.948.tar", last modified: Wed Aug  2 00:34:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-organization-3.0.947.tar` & `tencentcloud-sdk-python-organization-3.0.948.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud_sdk_python_organization.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      738 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud_sdk_python_organization.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud_sdk_python_organization.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1024 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20181225/
--rw-r--r--   0 root         (0) root         (0)    19700 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20181225/organization_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20181225/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20181225/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    46488 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20181225/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20210331/
--rw-r--r--   0 root         (0) root         (0)    24514 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20210331/organization_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20210331/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10898 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20210331/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   118580 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20210331/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1704 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      764 2023-08-01 00:53:23.000000 tencentcloud-sdk-python-organization-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud_sdk_python_organization.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      797 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud_sdk_python_organization.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud_sdk_python_organization.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud_sdk_python_organization.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20181225/
+-rw-r--r--   0 root         (0) root         (0)    19700 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20181225/organization_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20181225/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20181225/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    46488 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20181225/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20210331/
+-rw-r--r--   0 root         (0) root         (0)    24514 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20210331/organization_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20210331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10898 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20210331/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   118580 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20210331/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      764 2023-08-02 00:34:58.000000 tencentcloud-sdk-python-organization-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-organization-3.0.947/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-organization-3.0.948/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 tencentcloud/organization/v20210331/__init__.py
 tencentcloud/organization/v20210331/errorcodes.py
 tencentcloud/organization/v20210331/models.py
 tencentcloud/organization/v20210331/organization_client.py
 tencentcloud_sdk_python_organization.egg-info/PKG-INFO
 tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
 tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
+tencentcloud_sdk_python_organization.egg-info/requires.txt
 tencentcloud_sdk_python_organization.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-organization-3.0.947/tencentcloud_sdk_python_organization.egg-info/PKG-INFO` & `tencentcloud-sdk-python-organization-3.0.948/tencentcloud_sdk_python_organization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-organization
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Organization SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-organization-3.0.947/setup.py` & `tencentcloud-sdk-python-organization-3.0.948/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-organization',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Organization SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-organization-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-organization-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20181225/organization_client.py` & `tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20181225/organization_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20181225/errorcodes.py` & `tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20181225/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20181225/models.py` & `tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20181225/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20210331/organization_client.py` & `tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20210331/organization_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20210331/errorcodes.py` & `tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20210331/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.947/tencentcloud/organization/v20210331/models.py` & `tencentcloud-sdk-python-organization-3.0.948/tencentcloud/organization/v20210331/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-organization-3.0.948/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-organization
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Organization SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-organization-3.0.947/README.rst` & `tencentcloud-sdk-python-organization-3.0.948/README.rst`

 * *Files identical despite different names*

