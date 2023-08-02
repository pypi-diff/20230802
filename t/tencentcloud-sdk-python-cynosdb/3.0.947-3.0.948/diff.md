# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.947.tar", last modified: Tue Aug  1 00:35:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.948.tar", last modified: Wed Aug  2 00:27:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.947.tar` & `tencentcloud-sdk-python-cynosdb-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)   119006 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11292 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   687592 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:35:17.000000 tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)   120018 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11292 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   688377 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud_sdk_python_cynosdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:27:47.000000 tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.947/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.948/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cynosdb',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cynosdb SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2460,14 +2460,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def OpenClusterReadOnlyInstanceGroupAccess(self, request):
+        """开启只读实例组接入
+
+        :param request: Request instance for OpenClusterReadOnlyInstanceGroupAccess.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.OpenClusterReadOnlyInstanceGroupAccessRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.OpenClusterReadOnlyInstanceGroupAccessResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("OpenClusterReadOnlyInstanceGroupAccess", params, headers=headers)
+            response = json.loads(body)
+            model = models.OpenClusterReadOnlyInstanceGroupAccessResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def OpenReadOnlyInstanceExclusiveAccess(self, request):
         """开通只读实例独有访问接入组
 
         :param request: Request instance for OpenReadOnlyInstanceExclusiveAccess.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.OpenReadOnlyInstanceExclusiveAccessRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.OpenReadOnlyInstanceExclusiveAccessResponse`
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud/cynosdb/v20190107/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -18797,14 +18797,45 @@
 
 
     def _deserialize(self, params):
         self._FlowId = params.get("FlowId")
         self._RequestId = params.get("RequestId")
 
 
+class OpenClusterReadOnlyInstanceGroupAccessRequest(AbstractModel):
+    """OpenClusterReadOnlyInstanceGroupAccess请求参数结构体
+
+    """
+
+
+class OpenClusterReadOnlyInstanceGroupAccessResponse(AbstractModel):
+    """OpenClusterReadOnlyInstanceGroupAccess返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._RequestId = params.get("RequestId")
+
+
 class OpenReadOnlyInstanceExclusiveAccessRequest(AbstractModel):
     """OpenReadOnlyInstanceExclusiveAccess请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.948/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.947/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.948/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.947/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.948/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

