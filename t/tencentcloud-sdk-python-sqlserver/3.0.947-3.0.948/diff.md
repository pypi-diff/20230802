# Comparing `tmp/tencentcloud-sdk-python-sqlserver-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-sqlserver-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.947.tar", last modified: Tue Aug  1 00:55:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.948.tar", last modified: Wed Aug  2 00:36:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sqlserver-3.0.947.tar` & `tencentcloud-sdk-python-sqlserver-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:55:15.000000 tencentcloud-sdk-python-sqlserver-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1018 2023-08-01 00:55:14.000000 tencentcloud-sdk-python-sqlserver-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:55:15.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:55:14.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:55:15.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/sqlserver/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:55:15.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/sqlserver/v20180328/
--rw-r--r--   0 root         (0) root         (0)   109131 2023-08-01 00:55:14.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/sqlserver/v20180328/sqlserver_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:55:14.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/sqlserver/v20180328/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9722 2023-08-01 00:55:14.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/sqlserver/v20180328/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   572158 2023-08-01 00:55:14.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/sqlserver/v20180328/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:55:14.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/sqlserver/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:55:15.000000 tencentcloud-sdk-python-sqlserver-3.0.947/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:55:15.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud_sdk_python_sqlserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:55:15.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-08-01 00:55:15.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-08-01 00:55:15.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:55:15.000000 tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-08-01 00:55:15.000000 tencentcloud-sdk-python-sqlserver-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      755 2023-08-01 00:55:14.000000 tencentcloud-sdk-python-sqlserver-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/sqlserver/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/sqlserver/v20180328/
+-rw-r--r--   0 root         (0) root         (0)   110110 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/sqlserver/v20180328/sqlserver_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/sqlserver/v20180328/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9722 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/sqlserver/v20180328/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   575362 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/sqlserver/v20180328/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/sqlserver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud_sdk_python_sqlserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      561 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud_sdk_python_sqlserver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      755 2023-08-02 00:36:42.000000 tencentcloud-sdk-python-sqlserver-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.947/setup.py` & `tencentcloud-sdk-python-sqlserver-3.0.948/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-sqlserver',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Sqlserver SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/sqlserver/v20180328/sqlserver_client.py` & `tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/sqlserver/v20180328/sqlserver_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1057,14 +1057,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeInstanceByOrders(self, request):
+        """本接口（DescribeInstanceByOrders）用于根据订单号查询资源ID
+
+        :param request: Request instance for DescribeInstanceByOrders.
+        :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeInstanceByOrdersRequest`
+        :rtype: :class:`tencentcloud.sqlserver.v20180328.models.DescribeInstanceByOrdersResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeInstanceByOrders", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeInstanceByOrdersResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeInstanceParamRecords(self, request):
         """该接口（DescribeInstanceParamRecords）用于查询实例参数修改历史。
 
         :param request: Request instance for DescribeInstanceParamRecords.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.DescribeInstanceParamRecordsRequest`
         :rtype: :class:`tencentcloud.sqlserver.v20180328.models.DescribeInstanceParamRecordsResponse`
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/sqlserver/v20180328/errorcodes.py` & `tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/sqlserver/v20180328/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud/sqlserver/v20180328/models.py` & `tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud/sqlserver/v20180328/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6019,14 +6019,59 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DealInstance(AbstractModel):
+    """订单号对应的资源ID列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID
+        :type InstanceId: list of str
+        :param _DealName: 订单号
+        :type DealName: str
+        """
+        self._InstanceId = None
+        self._DealName = None
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+    @property
+    def DealName(self):
+        return self._DealName
+
+    @DealName.setter
+    def DealName(self, DealName):
+        self._DealName = DealName
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._DealName = params.get("DealName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DeleteAccountRequest(AbstractModel):
     """DeleteAccount请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9250,14 +9295,89 @@
             for item in params.get("IncrementalMigrationSet"):
                 obj = Migration()
                 obj._deserialize(item)
                 self._IncrementalMigrationSet.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeInstanceByOrdersRequest(AbstractModel):
+    """DescribeInstanceByOrders请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DealNames: 订单号集合
+        :type DealNames: list of str
+        """
+        self._DealNames = None
+
+    @property
+    def DealNames(self):
+        return self._DealNames
+
+    @DealNames.setter
+    def DealNames(self, DealNames):
+        self._DealNames = DealNames
+
+
+    def _deserialize(self, params):
+        self._DealNames = params.get("DealNames")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeInstanceByOrdersResponse(AbstractModel):
+    """DescribeInstanceByOrders返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DealInstance: 资源ID集合
+        :type DealInstance: list of DealInstance
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._DealInstance = None
+        self._RequestId = None
+
+    @property
+    def DealInstance(self):
+        return self._DealInstance
+
+    @DealInstance.setter
+    def DealInstance(self, DealInstance):
+        self._DealInstance = DealInstance
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
+        if params.get("DealInstance") is not None:
+            self._DealInstance = []
+            for item in params.get("DealInstance"):
+                obj = DealInstance()
+                obj._deserialize(item)
+                self._DealInstance.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeInstanceParamRecordsRequest(AbstractModel):
     """DescribeInstanceParamRecords请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.947/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.948/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.948/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.947/README.rst` & `tencentcloud-sdk-python-sqlserver-3.0.948/README.rst`

 * *Files identical despite different names*

