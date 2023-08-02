# Comparing `tmp/tencentcloud-sdk-python-tag-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-tag-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tag-3.0.947.tar", last modified: Tue Aug  1 00:55:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tag-3.0.948.tar", last modified: Wed Aug  2 00:37:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tag-3.0.947.tar` & `tencentcloud-sdk-python-tag-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud/tag/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud/tag/v20180813/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud/tag/v20180813/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud/tag/v20180813/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28668 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud/tag/v20180813/tag_client.py
--rw-r--r--   0 root         (0) root         (0)   121329 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud/tag/v20180813/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud/tag/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud_sdk_python_tag.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud_sdk_python_tag.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud_sdk_python_tag.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud_sdk_python_tag.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/tencentcloud_sdk_python_tag.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:55:53.000000 tencentcloud-sdk-python-tag-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud/tag/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud/tag/v20180813/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud/tag/v20180813/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud/tag/v20180813/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28668 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud/tag/v20180813/tag_client.py
+-rw-r--r--   0 root         (0) root         (0)   121329 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud/tag/v20180813/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud/tag/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud_sdk_python_tag.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud_sdk_python_tag.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud_sdk_python_tag.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud_sdk_python_tag.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud_sdk_python_tag.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/tencentcloud_sdk_python_tag.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-02 00:37:22.000000 tencentcloud-sdk-python-tag-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-tag-3.0.947/setup.py` & `tencentcloud-sdk-python-tag-3.0.948/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-tag',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Tag SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-tag-3.0.947/tencentcloud/tag/v20180813/errorcodes.py` & `tencentcloud-sdk-python-tag-3.0.948/tencentcloud/tag/v20180813/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tag-3.0.947/tencentcloud/tag/v20180813/tag_client.py` & `tencentcloud-sdk-python-tag-3.0.948/tencentcloud/tag/v20180813/tag_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tag-3.0.947/tencentcloud/tag/v20180813/models.py` & `tencentcloud-sdk-python-tag-3.0.948/tencentcloud/tag/v20180813/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tag-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tag-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tag-3.0.947/tencentcloud_sdk_python_tag.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tag-3.0.948/tencentcloud_sdk_python_tag.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tag
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Tag SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tag-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-tag-3.0.948/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tag
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Tag SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tag-3.0.947/README.rst` & `tencentcloud-sdk-python-tag-3.0.948/README.rst`

 * *Files identical despite different names*
