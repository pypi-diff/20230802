# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.947.tar", last modified: Tue Aug  1 00:53:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.948.tar", last modified: Wed Aug  2 00:34:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.947.tar` & `tencentcloud-sdk-python-ocr-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5802 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   113546 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)   807406 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/ocr/v20181119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:53:13.000000 tencentcloud-sdk-python-ocr-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   113546 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)   807406 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:34:48.000000 tencentcloud-sdk-python-ocr-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-02 00:34:47.000000 tencentcloud-sdk-python-ocr-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.947/setup.py` & `tencentcloud-sdk-python-ocr-3.0.948/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-ocr',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Ocr SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 # 非指定卡类别图片
 FAILEDOPERATION_IMAGENOSPECIFIEDCARD = 'FailedOperation.ImageNoSpecifiedCard'
 
 # 图片中未检测到文本。
 FAILEDOPERATION_IMAGENOTEXT = 'FailedOperation.ImageNoText'
 
-# 图片尺寸过大，请参考输出参数中关于图片大小限制的说明。
+# 图片尺寸过大，请参考输入参数中关于图片大小限制的说明。
 FAILEDOPERATION_IMAGESIZETOOLARGE = 'FailedOperation.ImageSizeTooLarge'
 
 # 发票数据不一致。温馨提示：新版发票核验接口功能更完整，请尽快切换，如已切换请忽略。
 FAILEDOPERATION_INVOICEMISMATCH = 'FailedOperation.InvoiceMismatch'
 
 # 输入的Language不支持。
 FAILEDOPERATION_LANGUAGENOTSUPPORT = 'FailedOperation.LanguageNotSupport'
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.947/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.948/tencentcloud/ocr/v20181119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.947/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.948/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.948/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.947/README.rst` & `tencentcloud-sdk-python-ocr-3.0.948/README.rst`

 * *Files identical despite different names*

