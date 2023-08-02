# Comparing `tmp/tencentcloud-sdk-python-facefusion-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-facefusion-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-facefusion-3.0.946.tar", last modified: Mon Jul 31 00:26:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-facefusion-3.0.948.tar", last modified: Wed Aug  2 00:30:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-facefusion-3.0.946.tar` & `tencentcloud-sdk-python-facefusion-3.0.948.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      708 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3394 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/facefusion_client.py
--rw-r--r--   0 root         (0) root         (0)     5459 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    24611 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5785 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/facefusion_client.py
--rw-r--r--   0 root         (0) root         (0)     6738 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    39231 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud_sdk_python_facefusion.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud_sdk_python_facefusion.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      765 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud_sdk_python_facefusion.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud_sdk_python_facefusion.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20220927/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20220927/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20220927/facefusion_client.py
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20220927/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    24611 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20220927/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20181201/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20181201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20181201/facefusion_client.py
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20181201/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39231 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20181201/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      758 2023-08-02 00:30:02.000000 tencentcloud-sdk-python-facefusion-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.946/setup.py` & `tencentcloud-sdk-python-facefusion-3.0.948/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-facefusion',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Facefusion SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 tencentcloud/facefusion/v20220927/__init__.py
 tencentcloud/facefusion/v20220927/errorcodes.py
 tencentcloud/facefusion/v20220927/facefusion_client.py
 tencentcloud/facefusion/v20220927/models.py
 tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO
 tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt
 tencentcloud_sdk_python_facefusion.egg-info/dependency_links.txt
+tencentcloud_sdk_python_facefusion.egg-info/requires.txt
 tencentcloud_sdk_python_facefusion.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO` & `tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-facefusion
-Version: 3.0.946
+Version: 3.0.948
 Summary: Tencent Cloud Facefusion SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/facefusion_client.py` & `tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20220927/facefusion_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/errorcodes.py` & `tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20220927/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 # 人脸融合失败，请更换图片后重试。
 FAILEDOPERATION_FACEFUSIONERROR = 'FailedOperation.FaceFusionError'
 
 # 人脸框不合法。
 FAILEDOPERATION_FACERECTINVALID = 'FailedOperation.FaceRectInvalid'
 
+# 人脸配准失败。
+FAILEDOPERATION_FACESHAPEFAILED = 'FailedOperation.FaceShapeFailed'
+
 # 人脸因太小被过滤，建议人脸分辨率不小于34*34。
 FAILEDOPERATION_FACESIZETOOSMALL = 'FailedOperation.FaceSizeTooSmall'
 
 # 操作太频繁，触发频控。
 FAILEDOPERATION_FUSEFREQCTRL = 'FailedOperation.FuseFreqCtrl'
 
 # 图像处理出错。
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/models.py` & `tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20220927/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/facefusion_client.py` & `tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20181201/facefusion_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/errorcodes.py` & `tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20181201/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
 # 人脸姿态检测失败。
 FAILEDOPERATION_FACEPOSEFAILED = 'FailedOperation.FacePoseFailed'
 
 # 人脸框不合法。
 FAILEDOPERATION_FACERECTINVALID = 'FailedOperation.FaceRectInvalid'
 
+# 人脸配准失败。
+FAILEDOPERATION_FACESHAPEFAILED = 'FailedOperation.FaceShapeFailed'
+
 # 人脸配准点不合法。
 FAILEDOPERATION_FACESHAPEINVALID = 'FailedOperation.FaceShapeInvalid'
 
 # 人脸因太小被过滤，建议人脸分辨率不小于34*34。
 FAILEDOPERATION_FACESIZETOOSMALL = 'FailedOperation.FaceSizeTooSmall'
 
 # 人脸融合后端服务异常。
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/models.py` & `tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/facefusion/v20181201/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-facefusion-3.0.948/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.946'
+__version__ = '3.0.948'
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-facefusion-3.0.948/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-facefusion
-Version: 3.0.946
+Version: 3.0.948
 Summary: Tencent Cloud Facefusion SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.946/README.rst` & `tencentcloud-sdk-python-facefusion-3.0.948/README.rst`

 * *Files identical despite different names*

