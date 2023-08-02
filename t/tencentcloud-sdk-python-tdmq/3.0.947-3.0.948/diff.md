# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.947.tar", last modified: Tue Aug  1 00:57:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.948.tar", last modified: Wed Aug  2 00:38:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.947.tar` & `tencentcloud-sdk-python-tdmq-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95480 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10019 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   596365 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      506 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud_sdk_python_tdmq.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    96407 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10019 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   599574 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-02 00:38:48.000000 tencentcloud-sdk-python-tdmq-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.947/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.948/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-tdmq',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Tdmq SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -781,14 +781,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DeleteRocketMQVipInstance(self, request):
+        """删除RocketMQ专享实例
+
+        :param request: Request instance for DeleteRocketMQVipInstance.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRocketMQVipInstanceRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.DeleteRocketMQVipInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteRocketMQVipInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteRocketMQVipInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DeleteRoles(self, request):
         """删除角色，支持批量。
 
         :param request: Request instance for DeleteRoles.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRolesRequest`
         :rtype: :class:`tencentcloud.tdmq.v20200217.models.DeleteRolesResponse`
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/tdmq/v20200217/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1562,27 +1562,31 @@
 （1）BACKOFF_RETRY，退避重试。每隔一定时间重试一次，重试够一定次数后，就把该消息丢弃，继续推送下一条消息；
 （2）EXPONENTIAL_DECAY_RETRY，指数衰退重试。每次重试的间隔是指数递增的，例如开始 1s，后面是 2s，4s，8s...由于 Topic 消息的周期是一天，所以最多重试一天就把消息丢弃。默认值是 EXPONENTIAL_DECAY_RETRY。
 注意：此字段可能返回 null，表示取不到有效值。
         :type NotifyStrategy: str
         :param _NotifyContentFormat: 推送内容的格式。取值：（1）JSON；（2）SIMPLIFIED，即 raw 格式。如果 protocol 是 queue，则取值必须为 SIMPLIFIED。如果 protocol 是 HTTP，两个值均可以，默认值是 JSON。
 注意：此字段可能返回 null，表示取不到有效值。
         :type NotifyContentFormat: str
+        :param _TopicName: 订阅所属的主题名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TopicName: str
         """
         self._SubscriptionName = None
         self._SubscriptionId = None
         self._TopicOwner = None
         self._MsgCount = None
         self._LastModifyTime = None
         self._CreateTime = None
         self._BindingKey = None
         self._Endpoint = None
         self._FilterTags = None
         self._Protocol = None
         self._NotifyStrategy = None
         self._NotifyContentFormat = None
+        self._TopicName = None
 
     @property
     def SubscriptionName(self):
         return self._SubscriptionName
 
     @SubscriptionName.setter
     def SubscriptionName(self, SubscriptionName):
@@ -1672,28 +1676,37 @@
     def NotifyContentFormat(self):
         return self._NotifyContentFormat
 
     @NotifyContentFormat.setter
     def NotifyContentFormat(self, NotifyContentFormat):
         self._NotifyContentFormat = NotifyContentFormat
 
+    @property
+    def TopicName(self):
+        return self._TopicName
+
+    @TopicName.setter
+    def TopicName(self, TopicName):
+        self._TopicName = TopicName
+
 
     def _deserialize(self, params):
         self._SubscriptionName = params.get("SubscriptionName")
         self._SubscriptionId = params.get("SubscriptionId")
         self._TopicOwner = params.get("TopicOwner")
         self._MsgCount = params.get("MsgCount")
         self._LastModifyTime = params.get("LastModifyTime")
         self._CreateTime = params.get("CreateTime")
         self._BindingKey = params.get("BindingKey")
         self._Endpoint = params.get("Endpoint")
         self._FilterTags = params.get("FilterTags")
         self._Protocol = params.get("Protocol")
         self._NotifyStrategy = params.get("NotifyStrategy")
         self._NotifyContentFormat = params.get("NotifyContentFormat")
+        self._TopicName = params.get("TopicName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -1753,14 +1766,17 @@
         :type NamespaceName: str
         :param _Status: 集群状态，0:创建中，1:正常，2:销毁中，3:已删除，4: 隔离中，5:创建失败，6: 删除失败
 注意：此字段可能返回 null，表示取不到有效值。
         :type Status: int
         :param _BrokerType: 0表示pulsar，1表示rocketmq
 注意：此字段可能返回 null，表示取不到有效值。
         :type BrokerType: int
+        :param _SubscriptionCount: 订阅数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubscriptionCount: int
         """
         self._TopicId = None
         self._TopicName = None
         self._MsgRetentionSeconds = None
         self._MaxMsgSize = None
         self._Qps = None
         self._FilterType = None
@@ -1770,14 +1786,15 @@
         self._CreateUin = None
         self._Tags = None
         self._Trace = None
         self._TenantId = None
         self._NamespaceName = None
         self._Status = None
         self._BrokerType = None
+        self._SubscriptionCount = None
 
     @property
     def TopicId(self):
         return self._TopicId
 
     @TopicId.setter
     def TopicId(self, TopicId):
@@ -1899,14 +1916,22 @@
     def BrokerType(self):
         return self._BrokerType
 
     @BrokerType.setter
     def BrokerType(self, BrokerType):
         self._BrokerType = BrokerType
 
+    @property
+    def SubscriptionCount(self):
+        return self._SubscriptionCount
+
+    @SubscriptionCount.setter
+    def SubscriptionCount(self, SubscriptionCount):
+        self._SubscriptionCount = SubscriptionCount
+
 
     def _deserialize(self, params):
         self._TopicId = params.get("TopicId")
         self._TopicName = params.get("TopicName")
         self._MsgRetentionSeconds = params.get("MsgRetentionSeconds")
         self._MaxMsgSize = params.get("MaxMsgSize")
         self._Qps = params.get("Qps")
@@ -1922,14 +1947,15 @@
                 obj._deserialize(item)
                 self._Tags.append(obj)
         self._Trace = params.get("Trace")
         self._TenantId = params.get("TenantId")
         self._NamespaceName = params.get("NamespaceName")
         self._Status = params.get("Status")
         self._BrokerType = params.get("BrokerType")
+        self._SubscriptionCount = params.get("SubscriptionCount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -5573,14 +5599,72 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class DeleteRocketMQVipInstanceRequest(AbstractModel):
+    """DeleteRocketMQVipInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ClusterId: 实例的集群ID
+        :type ClusterId: str
+        """
+        self._ClusterId = None
+
+    @property
+    def ClusterId(self):
+        return self._ClusterId
+
+    @ClusterId.setter
+    def ClusterId(self, ClusterId):
+        self._ClusterId = ClusterId
+
+
+    def _deserialize(self, params):
+        self._ClusterId = params.get("ClusterId")
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
+class DeleteRocketMQVipInstanceResponse(AbstractModel):
+    """DeleteRocketMQVipInstance返回参数结构体
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
 class DeleteRolesRequest(AbstractModel):
     """DeleteRoles请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6969,19 +7053,26 @@
         :type TopicName: str
         :param _Offset: 分页时本页获取主题列表的起始位置。如果填写了该值，必须也要填写 limit 。该值缺省时，后台取默认值 0
         :type Offset: int
         :param _Limit: 分页时本页获取主题的个数，如果不传递该参数，则该参数默认为20，最大值为50。
         :type Limit: int
         :param _SubscriptionName: 根据SubscriptionName进行模糊搜索
         :type SubscriptionName: str
+        :param _QueueName: 队列名称，订阅绑定的endpoint
+        :type QueueName: str
+        :param _QueryType: 查询类型。取值：（1）topic；（2）queue。
+默认值是topic。如果 queryType 是 topic，则查询主题下的订阅列表；如果 queryType 是 queue，则查询队列绑定的订阅列表。
+        :type QueryType: str
         """
         self._TopicName = None
         self._Offset = None
         self._Limit = None
         self._SubscriptionName = None
+        self._QueueName = None
+        self._QueryType = None
 
     @property
     def TopicName(self):
         return self._TopicName
 
     @TopicName.setter
     def TopicName(self, TopicName):
@@ -7007,20 +7098,38 @@
     def SubscriptionName(self):
         return self._SubscriptionName
 
     @SubscriptionName.setter
     def SubscriptionName(self, SubscriptionName):
         self._SubscriptionName = SubscriptionName
 
+    @property
+    def QueueName(self):
+        return self._QueueName
+
+    @QueueName.setter
+    def QueueName(self, QueueName):
+        self._QueueName = QueueName
+
+    @property
+    def QueryType(self):
+        return self._QueryType
+
+    @QueryType.setter
+    def QueryType(self, QueryType):
+        self._QueryType = QueryType
+
 
     def _deserialize(self, params):
         self._TopicName = params.get("TopicName")
         self._Offset = params.get("Offset")
         self._Limit = params.get("Limit")
         self._SubscriptionName = params.get("SubscriptionName")
+        self._QueueName = params.get("QueueName")
+        self._QueryType = params.get("QueryType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.948/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.947/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.948/README.rst`

 * *Files identical despite different names*

