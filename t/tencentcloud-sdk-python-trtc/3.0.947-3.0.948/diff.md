# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.947.tar", last modified: Tue Aug  1 00:59:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.948.tar", last modified: Wed Aug  2 00:40:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.947.tar` & `tencentcloud-sdk-python-trtc-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9679 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    65738 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)   289132 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:59:11.000000 tencentcloud-sdk-python-trtc-3.0.947/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    65928 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)   289147 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      506 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud_sdk_python_trtc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:40:34.000000 tencentcloud-sdk-python-trtc-3.0.948/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.947/setup.py` & `tencentcloud-sdk-python-trtc-3.0.948/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-trtc',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Trtc SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,16 +508,17 @@
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTrtcRoomUsage(self, request):
         """查询TRTC音视频房间维度用量。
         - 单次只能查询一天数据，返回查询时间段内的汇总数据；通过多次查询可以查不同天数据。若查询跨天用量，由于统计延迟等原因，返回数据可能不够准确。
-        - 该接口只用于历史用量数据统计或核对数据使用，关键业务逻辑不能使用。
+        - 该接口只用于历史用量数据统计或核对数据使用，关键业务逻辑不能使用，不可用于账单核对，如需对账请使用账号/应用维度用量API：DescribeTrtcUsage。
         - 默认接口请求频率限制：1次/15秒。
+        - 数据最早可查日期为2023年4月1日0点，最大可查范围近3个月。
 
         :param request: Request instance for DescribeTrtcRoomUsage.
         :type request: :class:`tencentcloud.trtc.v20190722.models.DescribeTrtcRoomUsageRequest`
         :rtype: :class:`tencentcloud.trtc.v20190722.models.DescribeTrtcRoomUsageResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/trtc/v20190722/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2723,15 +2723,15 @@
 class DescribeTrtcRoomUsageResponse(AbstractModel):
     """DescribeTrtcRoomUsage返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Data: 房间维度用量数据，csv文件格式。
+        :param _Data: 房间维度用量数据，csv文件格式，单位：秒。
         :type Data: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
         self._RequestId = None
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.948/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.947/README.rst` & `tencentcloud-sdk-python-trtc-3.0.948/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.947/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.948/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

