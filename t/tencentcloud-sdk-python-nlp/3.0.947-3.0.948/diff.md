# Comparing `tmp/tencentcloud-sdk-python-nlp-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-nlp-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.947.tar", last modified: Tue Aug  1 00:52:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.948.tar", last modified: Wed Aug  2 00:34:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-nlp-3.0.947.tar` & `tencentcloud-sdk-python-nlp-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:55.000000 tencentcloud-sdk-python-nlp-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:52:54.000000 tencentcloud-sdk-python-nlp-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:55.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:52:54.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:55.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud/nlp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:55.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud/nlp/v20190408/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:52:54.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud/nlp/v20190408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49259 2023-08-01 00:52:54.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud/nlp/v20190408/nlp_client.py
--rw-r--r--   0 root         (0) root         (0)     6090 2023-08-01 00:52:54.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud/nlp/v20190408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   134540 2023-08-01 00:52:54.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud/nlp/v20190408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:52:54.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud/nlp/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:52:55.000000 tencentcloud-sdk-python-nlp-3.0.947/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:55.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud_sdk_python_nlp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:52:55.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:52:55.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:52:55.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:52:55.000000 tencentcloud-sdk-python-nlp-3.0.947/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:52:55.000000 tencentcloud-sdk-python-nlp-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:52:54.000000 tencentcloud-sdk-python-nlp-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud/nlp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud/nlp/v20190408/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud/nlp/v20190408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13482 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud/nlp/v20190408/nlp_client.py
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud/nlp/v20190408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    52142 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud/nlp/v20190408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud/nlp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud_sdk_python_nlp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud_sdk_python_nlp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-02 00:34:31.000000 tencentcloud-sdk-python-nlp-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.947/setup.py` & `tencentcloud-sdk-python-nlp-3.0.948/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-nlp',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Nlp SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-nlp-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-nlp-3.0.947/tencentcloud/nlp/v20190408/errorcodes.py` & `tencentcloud-sdk-python-nlp-3.0.948/tencentcloud/nlp/v20190408/errorcodes.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,26 +10,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-# 请求头部的 Authorization 不符合腾讯云标准。
-AUTHFAILURE_INVALIDAUTHORIZATION = 'AuthFailure.InvalidAuthorization'
-
 # 操作失败。
 FAILEDOPERATION = 'FailedOperation'
 
 # 余额不足，开通失败，请充值后再开通。
 FAILEDOPERATION_BALANCEINSUFFICIENT = 'FailedOperation.BalanceInsufficient'
 
-# 非法文本输入导致返回异常
-FAILEDOPERATION_ILLEGALTEXTERROR = 'FailedOperation.IllegalTextError'
-
 # 服务内部错误，请重试。
 FAILEDOPERATION_INNERERROR = 'FailedOperation.InnerError'
 
 # 暂无春联生成，请更换关键词重试。
 FAILEDOPERATION_NOCOUPLETS = 'FailedOperation.NoCouplets'
 
 # 暂无诗词生成，请更换关键词重试。
@@ -46,56 +40,41 @@
 
 # 服务器繁忙，请稍后再试。
 FAILEDOPERATION_RESOURCEBUSY = 'FailedOperation.ResourceBusy'
 
 # RPC请求失败，一般为算法微服务故障。
 FAILEDOPERATION_RPCFAIL = 'FailedOperation.RpcFail'
 
-# 文本向量化失败
-FAILEDOPERATION_TEXTEMBEDDINGFAILED = 'FailedOperation.TextEmbeddingFailed'
-
 # 内部错误。
 FAILEDOPERATION_UNKNOWERROR = 'FailedOperation.UnKnowError'
 
 # 未知错误。
 FAILEDOPERATION_UNKNOWN = 'FailedOperation.Unknown'
 
-# 查找不到词语
-FAILEDOPERATION_WORDNOTFOUND = 'FailedOperation.WordNotFound'
-
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
-# 资源请求错误
-INTERNALERROR_RESOURCEREQUESTERROR = 'InternalError.ResourceRequestError'
-
 # 内部服务调用错误。
 INTERNALERROR_SERVICECALLERROR = 'InternalError.ServiceCallError'
 
 # 内部服务调用失败。
 INTERNALERROR_SERVICEERROR = 'InternalError.ServiceError'
 
 # 文本分类异常。
 INTERNALERROR_TEXTCLASSIFYERROR = 'InternalError.TextClassifyError'
 
 # 文本解析异常。
 INTERNALERROR_TEXTPARSINGERROR = 'InternalError.TextParsingError'
 
-# 参数错误。
-INVALIDPARAMETER = 'InvalidParameter'
-
 # 服务调用失败。
 INVALIDPARAMETER_SERVICEERROR = 'InvalidParameter.ServiceError'
 
 # 文本长度超过限制。
 INVALIDPARAMETER_TEXTTOOLONGCODE = 'InvalidParameter.TextTooLongCode'
 
-# 参数空值错误
-INVALIDPARAMETERVALUE_EMPTYVALUEERROR = 'InvalidParameterValue.EmptyValueError'
-
 # Genre非法，请参考Genre参数说明。
 INVALIDPARAMETERVALUE_GENRE = 'InvalidParameterValue.Genre'
 
 # 参数不合法。
 INVALIDPARAMETERVALUE_INVALIDPARAMETER = 'InvalidParameterValue.InvalidParameter'
 
 # PoetryType非法，请参考PoetryType参数说明。
@@ -106,59 +85,35 @@
 
 # TargetType非法，请参考TargetType参数说明。
 INVALIDPARAMETERVALUE_TARGETTYPE = 'InvalidParameterValue.TargetType'
 
 # Text非法，请参考Text参数说明。
 INVALIDPARAMETERVALUE_TEXT = 'InvalidParameterValue.Text'
 
-# 文本编码错误，不符合utf-8
-INVALIDPARAMETERVALUE_TEXTENCODEERROR = 'InvalidParameterValue.TextEncodeError'
-
-# 文本输入格式错误
-INVALIDPARAMETERVALUE_TEXTFORMATERROR = 'InvalidParameterValue.TextFormatError'
-
 # 输入文本超出数量限制
 INVALIDPARAMETERVALUE_TEXTNUMTOOMUCH = 'InvalidParameterValue.TextNumTooMuch'
 
 # 输入文本超出长度限制
 INVALIDPARAMETERVALUE_TEXTTOOLONG = 'InvalidParameterValue.TextTooLong'
 
-# 参数取值范围错误
-INVALIDPARAMETERVALUE_VALUERANGEERROR = 'InvalidParameterValue.ValueRangeError'
-
 # 资源用量达到上限。
 LIMITEXCEEDED_RESOURCEREACHEDLIMIT = 'LimitExceeded.ResourceReachedLimit'
 
 # 请求的次数超过了频率限制。
 REQUESTLIMITEXCEEDED_UINLIMITEXCEEDED = 'RequestLimitExceeded.UinLimitExceeded'
 
-# 名称已存在
-RESOURCEINUSE_NAMEEXISTS = 'ResourceInUse.NameExists'
-
-# 资源正在操作中
-RESOURCEINUSE_RESOURCEOPERATING = 'ResourceInUse.ResourceOperating'
-
 # 额度用尽，请充值后重试
 RESOURCEINSUFFICIENT_QUOTARUNOUT = 'ResourceInsufficient.QuotaRunOut'
 
 # 资源不存在。
 RESOURCENOTFOUND = 'ResourceNotFound'
 
-# 数据资源不存在
-RESOURCENOTFOUND_DATANOTFOUND = 'ResourceNotFound.DataNotFound'
-
-# 文件资源不存在
-RESOURCENOTFOUND_FILENOTFOUND = 'ResourceNotFound.FileNotFound'
-
 # 资源不可用。
 RESOURCEUNAVAILABLE = 'ResourceUnavailable'
 
-# 文件资源不可用
-RESOURCEUNAVAILABLE_FILEUNAVAILABLE = 'ResourceUnavailable.FileUnavailable'
-
 # 帐号已被冻结。
 RESOURCEUNAVAILABLE_FREEZE = 'ResourceUnavailable.Freeze'
 
 # 账号已欠费。
 RESOURCEUNAVAILABLE_INARREARS = 'ResourceUnavailable.InArrears'
 
 # 服务正在开通中，请稍等。
@@ -171,10 +126,7 @@
 RESOURCEUNAVAILABLE_RECOVER = 'ResourceUnavailable.Recover'
 
 # 您的账号尚未开通NLP服务，请登录腾讯云NLP控制台进行服务开通后再使用
 RESOURCEUNAVAILABLE_SERVICENOTOPENEDERROR = 'ResourceUnavailable.ServiceNotOpenedError'
 
 # 帐号已停服。
 RESOURCEUNAVAILABLE_STOPUSING = 'ResourceUnavailable.StopUsing'
-
-# 实名认证失败
-UNAUTHORIZEDOPERATION_AUTHENTICATEFAILED = 'UnauthorizedOperation.AuthenticateFailed'
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.947/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.948/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.948/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.947/README.rst` & `tencentcloud-sdk-python-nlp-3.0.948/README.rst`

 * *Files identical despite different names*

