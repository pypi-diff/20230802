# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.947.tar", last modified: Tue Aug  1 00:37:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.948.tar", last modified: Wed Aug  2 00:29:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.947.tar` & `tencentcloud-sdk-python-ess-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    66079 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   471423 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    67109 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   477099 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:29:48.000000 tencentcloud-sdk-python-ess-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-02 00:29:47.000000 tencentcloud-sdk-python-ess-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.947/setup.py` & `tencentcloud-sdk-python-ess-3.0.948/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-ess',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Ess SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-ess-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -600,14 +600,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def CreatePersonAuthCertificateImage(self, request):
+        """本接口（CreatePersonAuthCertificateImage）用于创建个人用户证书证明图片
+
+        :param request: Request instance for CreatePersonAuthCertificateImage.
+        :type request: :class:`tencentcloud.ess.v20201111.models.CreatePersonAuthCertificateImageRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.CreatePersonAuthCertificateImageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreatePersonAuthCertificateImage", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreatePersonAuthCertificateImageResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def CreatePrepareFlow(self, request):
         """创建快速发起流程
         <br/>适用场景：用户通过API 合同文件及签署信息，并可通过我们返回的URL在页面完成签署控件等信息的编辑与确认，快速发起合同.
         <br/>注：该接口文件的resourceId 是通过上传文件之后获取的。
 
         :param request: Request instance for CreatePrepareFlow.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreatePrepareFlowRequest`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.948/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3620,14 +3620,15 @@
     def __init__(self):
         r"""
         :param _Operator: 调用方用户信息，userId 必填。支持填入集团子公司经办人 userId代发合同。
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _FlowName: 签署流程名称,最大长度200个字符
         :type FlowName: str
         :param _Approvers: 签署流程参与者信息，最大限制50方
+注意 approver中的顺序需要和模板中的顺序保持一致， 否则会导致模板中配置的信息无效。
         :type Approvers: list of FlowCreateApprover
         :param _FlowType: 签署流程的类型(如销售合同/入职合同等)，最大长度200个字符
         :type FlowType: str
         :param _ClientToken: 客户端Token，保持接口幂等性,最大长度64个字符
         :type ClientToken: str
         :param _DeadLine: 签署流程的签署截止时间。
 值为unix时间戳,精确到秒,不传默认为当前时间一年后
@@ -4565,27 +4566,30 @@
         :param _Operator: 用户信息，其中UserId为必填参数
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _TemplateId: 模板ID
         :type TemplateId: str
         :param _FlowName: 签署流程名称，最大长度不超过200字符
         :type FlowName: str
         :param _MaxFlowNum: 最大可发起签署流程份数，默认5份 
-发起流程数量超过此上限后二维码自动失效
+<br/>发起流程数量超过此上限后二维码自动失效
         :type MaxFlowNum: int
-        :param _FlowEffectiveDay: 签署流程有效天数 默认7天 最高设置不超过30天
+        :param _FlowEffectiveDay: 签署流程有效天数 
+<br/>默认7天 
+<br/>最高设置不超过30天
         :type FlowEffectiveDay: int
         :param _QrEffectiveDay: 二维码有效天数 默认7天 最高设置不超过90天
         :type QrEffectiveDay: int
-        :param _Restrictions: 限制二维码用户条件
+        :param _Restrictions: 指定的签署人信息
+<br/>指定后，则只允许指定的签署人扫码签署
         :type Restrictions: list of ApproverRestriction
-        :param _UserData: 用户自定义字段，回调的时候会进行透传，长度需要小于20480
+        :param _UserData: 用户自定义字段
+<br/>回调的时候会进行透传，长度需要小于20480
         :type UserData: str
         :param _CallbackUrl: 回调地址,最大长度1000字符串
-回调时机：
-用户通过签署二维码发起签署流程时，企业额度不足导致失败
+<br/>回调时机：用户通过签署二维码发起签署流程时，企业额度不足导致失败
         :type CallbackUrl: str
         :param _Agent: 应用信息
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param _ApproverRestrictions: 限制二维码用户条件（已弃用）
         :type ApproverRestrictions: :class:`tencentcloud.ess.v20201111.models.ApproverRestriction`
         """
         self._Operator = None
@@ -4925,14 +4929,127 @@
 
     def _deserialize(self, params):
         self._SignUrl = params.get("SignUrl")
         self._ExpiredTime = params.get("ExpiredTime")
         self._RequestId = params.get("RequestId")
 
 
+class CreatePersonAuthCertificateImageRequest(AbstractModel):
+    """CreatePersonAuthCertificateImage请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Operator: 操作人信息
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param _UserName: 个人用户名称
+        :type UserName: str
+        :param _IdCardType: 身份证件类型取值：
+ID_CARD 身居民身份证
+PASSPORT 护照
+HONGKONG_AND_MACAO 港澳居民来往内地通行证
+FOREIGN_ID_CARD 外国人永久居留身份证
+HONGKONG_MACAO_AND_TAIWAN 港澳台居民居住证(格式同居民身份证)
+        :type IdCardType: str
+        :param _IdCardNumber: 身份证件号码
+        :type IdCardNumber: str
+        """
+        self._Operator = None
+        self._UserName = None
+        self._IdCardType = None
+        self._IdCardNumber = None
+
+    @property
+    def Operator(self):
+        return self._Operator
+
+    @Operator.setter
+    def Operator(self, Operator):
+        self._Operator = Operator
+
+    @property
+    def UserName(self):
+        return self._UserName
+
+    @UserName.setter
+    def UserName(self, UserName):
+        self._UserName = UserName
+
+    @property
+    def IdCardType(self):
+        return self._IdCardType
+
+    @IdCardType.setter
+    def IdCardType(self, IdCardType):
+        self._IdCardType = IdCardType
+
+    @property
+    def IdCardNumber(self):
+        return self._IdCardNumber
+
+    @IdCardNumber.setter
+    def IdCardNumber(self, IdCardNumber):
+        self._IdCardNumber = IdCardNumber
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self._Operator = UserInfo()
+            self._Operator._deserialize(params.get("Operator"))
+        self._UserName = params.get("UserName")
+        self._IdCardType = params.get("IdCardType")
+        self._IdCardNumber = params.get("IdCardNumber")
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
+class CreatePersonAuthCertificateImageResponse(AbstractModel):
+    """CreatePersonAuthCertificateImage返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _AuthCertUrl: 个人用户证明证书的下载链接
+        :type AuthCertUrl: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._AuthCertUrl = None
+        self._RequestId = None
+
+    @property
+    def AuthCertUrl(self):
+        return self._AuthCertUrl
+
+    @AuthCertUrl.setter
+    def AuthCertUrl(self, AuthCertUrl):
+        self._AuthCertUrl = AuthCertUrl
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
+        self._AuthCertUrl = params.get("AuthCertUrl")
+        self._RequestId = params.get("RequestId")
+
+
 class CreatePrepareFlowRequest(AbstractModel):
     """CreatePrepareFlow请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10543,16 +10660,19 @@
     """
 
     def __init__(self):
         r"""
         :param _ApproverType: 参与者类型：
 0：企业
 1：个人
-3：企业静默签署
-注：类型为3（企业静默签署）时，会默认完成该签署方的签署。静默签署仅进行盖章操作，不能是手写签名。
+3：企业自动签署
+注：类型为3（企业自动签署）时，会自动完成该签署方的签署。
+自动签署仅进行盖章操作，不能是手写签名。
+本方企业自动签署的签署人会默认是当前的发起人
+他方企业自动签署的签署人是自动签模板的他方企业授权人
         :type ApproverType: int
         :param _OrganizationName: 签署人企业名称
 <br/>当approverType=1 或 approverType=3时，必须指定
 
 
         :type OrganizationName: str
         :param _ApproverName: 签署方经办人姓名
@@ -11327,16 +11447,80 @@
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class FormField(AbstractModel):
     """电子文档的控件填充信息。按照控件类型进行相应的填充。
 
+    当控件的 ComponentType='TEXT'时，FormField.ComponentValue填入文本内容
+    ```
+    FormFiled输入示例：
+    {
+        "ComponentId": "componentId1",
+        "ComponentValue": "文本内容"
+    }
+    ```
+    当控件的 ComponentType='MULTI_LINE_TEXT'时，FormField.ComponentValue填入文本内容，支持自动换行。
+    ```
+    FormFiled输入示例：
+    {
+        "ComponentId": "componentId1",
+        "ComponentValue": "多行文本内容"
+    }
+    ```
+    当控件的 ComponentType='CHECK_BOX'时，FormField.ComponentValue填入true或false文本
+    ```
+    FormFiled输入示例：
+    {
+        "ComponentId": "componentId1",
+        "ComponentValue": "true"
+    }
+    ```
+    当控件的 ComponentType='FILL_IMAGE'时，FormField.ComponentValue填入图片的资源ID
+    ```
+    FormFiled输入示例：
+    {
+        "ComponentId": "componentId1",
+        "ComponentValue": "yDwhsxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+    }
+    ```
+    当控件的 ComponentType='ATTACHMENT'时，FormField.ComponentValue填入附件图片的资源ID列表，以逗号分隔，单个附件控件最多支持6个资源ID；
+    ```
+    FormFiled输入示例：
+    {
+        "ComponentId": "componentId1",
+        "ComponentValue": "yDwhsxxxxxxxxxxxxxxxxxxxxxxxxxx1,yDwhsxxxxxxxxxxxxxxxxxxxxxxxxxx2,yDwhsxxxxxxxxxxxxxxxxxxxxxxxxxx3"
+    }
+    ```
+    当控件的 ComponentType='SELECTOR'时，FormField.ComponentValue填入选择的选项内容；
+    ```
+    FormFiled输入示例：
+    {
+        "ComponentId": "componentId1",
+        "ComponentValue": "选择的内容"
+    }
+    ```
+    当控件的 ComponentType='DATE'时，FormField.ComponentValue填入日期内容；
+    ```
+    FormFiled输入示例：
+    {
+        "ComponentId": "componentId1",
+        "ComponentValue": "2023年01月01日"
+    }
+    ```
+    当控件的 ComponentType='DISTRICT'时，FormField.ComponentValue填入省市区内容；
+    ```
+    FormFiled输入示例：
+    {
+        "ComponentId": "componentId1",
+        "ComponentValue": "广东省深圳市福田区"
+    }
+    ```
     【数据表格传参说明】
-    当模板的 ComponentType='DYNAMIC_TABLE'时，FormField.ComponentValue需要传递json格式的字符串参数，用于确定表头&填充数据表格（支持内容的单元格合并）
+    当控件的 ComponentType='DYNAMIC_TABLE'时，FormField.ComponentValue需要传递json格式的字符串参数，用于确定表头&填充数据表格（支持内容的单元格合并）
     输入示例1：
 
     ```
     {
         "headers":[
             {
                 "content":"head1"
```

### Comparing `tencentcloud-sdk-python-ess-3.0.947/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.948/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.948/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.947/README.rst` & `tencentcloud-sdk-python-ess-3.0.948/README.rst`

 * *Files identical despite different names*

