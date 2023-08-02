# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.947.tar", last modified: Tue Aug  1 00:37:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.948.tar", last modified: Wed Aug  2 00:29:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.947.tar` & `tencentcloud-sdk-python-essbasic-3.0.948.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    56676 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   393237 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54057 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    56676 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   393412 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      733 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:29:54.000000 tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.947/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.948/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-essbasic',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Essbasic SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2341,21 +2341,24 @@
         :param _Agent: 应用相关信息。
 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _TemplateId: 模版ID
         :type TemplateId: str
         :param _FlowName: 签署流程名称，最大长度200个字符。
         :type FlowName: str
-        :param _MaxFlowNum: 最大可发起签署流程份数，默认5份；发起签署流程数量超过此上限后，二维码自动失效。
+        :param _MaxFlowNum: 最大可发起签署流程份数
+<br/>默认5份
+<br/>备注：发起签署流程数量超过此上限后，二维码自动失效。
         :type MaxFlowNum: int
         :param _FlowEffectiveDay: 签署流程有效天数 默认7天 最高设置不超过30天
         :type FlowEffectiveDay: int
         :param _QrEffectiveDay: 二维码有效天数 默认7天 最高设置不超过90天
         :type QrEffectiveDay: int
-        :param _Restrictions: 限制二维码用户条件
+        :param _Restrictions: 指定的签署二维码签署人
+<br/>指定后，只允许知道的人操作和签署
         :type Restrictions: list of ApproverRestriction
         :param _CallbackUrl: 回调地址，最大长度1000个字符
 不传默认使用第三方应用号配置的回调地址
 回调时机:用户通过签署二维码发起合同时，企业额度不足导致失败
         :type CallbackUrl: str
         :param _ApproverRestrictions: 限制二维码用户条件（已弃用）
         :type ApproverRestrictions: :class:`tencentcloud.essbasic.v20210526.models.ApproverRestriction`
@@ -6687,17 +6690,18 @@
     """
 
     def __init__(self):
         r"""
         :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowIds: 合同(流程)编号数组，最多支持100个。
-（备注：该参数和合同组编号必须二选一, 如果填写FlowGroupId则忽略此FlowIds的入参）
+<br/>备注：该参数和合同组编号必须二选一, 如果填写FlowGroupId则忽略此FlowIds的入参
         :type FlowIds: list of str
-        :param _FlowGroupId: 合同组编号（备注：该参数和合同(流程)编号数组必须二选一）
+        :param _FlowGroupId: 合同组编号
+<br/>备注：该参数和合同(流程)编号数组必须二选一
         :type FlowGroupId: str
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
         self._FlowIds = None
         self._FlowGroupId = None
@@ -7726,36 +7730,37 @@
         :type Mobile: str
         :param _SignOrder: 签署人签署顺序
         :type SignOrder: int
         :param _ApproveName: 签署人姓名
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproveName: str
         :param _ApproveStatus: 当前签署人的状态, 状态如下
-
-PENDING 待签署	
-FILLPENDING 待填写
-FILLACCEPT 填写完成	
-FILLREJECT 拒绝填写	
-WAITPICKUP 待领取	
-ACCEPT 已签署	
-REJECT 拒签 
-DEADLINE 过期没人处理 
-CANCEL 流程已撤回	
-FORWARD 已经转他人处理
-STOP 流程已终止	
-RELIEVED 解除协议（已解除）
+<br/>PENDING 待签署	
+<br/>FILLPENDING 待填写
+<br/>FILLACCEPT 填写完成	
+<br/>FILLREJECT 拒绝填写	
+<br/>WAITPICKUP 待领取	
+<br/>ACCEPT 已签署	
+<br/>REJECT 拒签 
+<br/>DEADLINE 过期没人处理 
+<br/>CANCEL 流程已撤回	
+<br/>FORWARD 已经转他人处理
+<br/>STOP 流程已终止	
+<br/>RELIEVED 解除协议（已解除）
 
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproveStatus: str
-        :param _ApproveMessage: 签署人信息
+        :param _ApproveMessage: 签署人自定义信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproveMessage: str
         :param _ApproveTime: 签署人签署时间戳，单位秒
         :type ApproveTime: int
-        :param _ApproveType: 参与者类型 (ORGANIZATION企业/PERSON个人)
+        :param _ApproveType: 参与者类型 
+<br/>ORGANIZATION：企业签署人
+<br/>PERSON：个人签署人
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproveType: str
         """
         self._ReceiptId = None
         self._ProxyOrganizationOpenId = None
         self._ProxyOperatorOpenId = None
         self._ProxyOrganizationName = None
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.948/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.947/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.948/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 tencentcloud/essbasic/v20210526/__init__.py
 tencentcloud/essbasic/v20210526/errorcodes.py
 tencentcloud/essbasic/v20210526/essbasic_client.py
 tencentcloud/essbasic/v20210526/models.py
 tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
 tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
 tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+tencentcloud_sdk_python_essbasic.egg-info/requires.txt
 tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.948/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

