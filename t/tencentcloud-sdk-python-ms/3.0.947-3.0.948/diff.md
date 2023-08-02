# Comparing `tmp/tencentcloud-sdk-python-ms-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-ms-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.947.tar", last modified: Tue Aug  1 00:52:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.948.tar", last modified: Wed Aug  2 00:34:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ms-3.0.947.tar` & `tencentcloud-sdk-python-ms-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud_sdk_python_ms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud_sdk_python_ms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1004 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/
--rw-r--r--   0 root         (0) root         (0)    21299 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/ms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5911 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   169759 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud_sdk_python_ms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      484 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud_sdk_python_ms.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud_sdk_python_ms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud/ms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud/ms/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    21439 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud/ms/v20180408/ms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud/ms/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5911 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud/ms/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   169761 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud/ms/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud/ms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-08-02 00:34:19.000000 tencentcloud-sdk-python-ms-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-ms-3.0.947/tencentcloud_sdk_python_ms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.948/tencentcloud_sdk_python_ms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.947/setup.py` & `tencentcloud-sdk-python-ms-3.0.948/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-ms',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Ms SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/ms_client.py` & `tencentcloud-sdk-python-ms-3.0.948/tencentcloud/ms/v20180408/ms_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 class MsClient(AbstractClient):
     _apiVersion = '2018-04-08'
     _endpoint = 'ms.tencentcloudapi.com'
     _service = 'ms'
 
 
     def CancelEncryptTask(self, request):
-        """该接口供渠道合作应用加固使用，接口调用有白名单用户限制，取消渠道合作加固中的任务。
+        """上错服务器了
+
+        该接口供渠道合作应用加固使用，接口调用有白名单用户限制，取消渠道合作加固中的任务。
 
         :param request: Request instance for CancelEncryptTask.
         :type request: :class:`tencentcloud.ms.v20180408.models.CancelEncryptTaskRequest`
         :rtype: :class:`tencentcloud.ms.v20180408.models.CancelEncryptTaskResponse`
 
         """
         try:
@@ -92,15 +94,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateEncryptInstance(self, request):
-        """该接口供渠道合作应用加固使用，接口调用有白名单用户限制，用于创建加固任务。
+        """上错服务器了
+
+        该接口供渠道合作应用加固使用，接口调用有白名单用户限制，用于创建加固任务。
 
         :param request: Request instance for CreateEncryptInstance.
         :type request: :class:`tencentcloud.ms.v20180408.models.CreateEncryptInstanceRequest`
         :rtype: :class:`tencentcloud.ms.v20180408.models.CreateEncryptInstanceResponse`
 
         """
         try:
@@ -115,15 +119,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOrderInstance(self, request):
-        """该接口供渠道合作应用加固使用，接口调用有白名单用户限制。
+        """上错服务器了
+
+        该接口供渠道合作应用加固使用，接口调用有白名单用户限制。
         订单类型有：免费试用、按年收费、按次收费。
         应用加固支持的平台类型有：android加固 、ios源码混淆 、sdk加固、applet小程序加固。
 
         :param request: Request instance for CreateOrderInstance.
         :type request: :class:`tencentcloud.ms.v20180408.models.CreateOrderInstanceRequest`
         :rtype: :class:`tencentcloud.ms.v20180408.models.CreateOrderInstanceResponse`
 
@@ -255,15 +261,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeEncryptInstances(self, request):
-        """该接口供渠道合作应用加固使用，接口调用有白名单用户限制，用于查询加固任务，入参中的条件过滤字段均为精准匹配。支持功能点：1. 多任务分页查询  2.根据任务Id唯一值查询单记录
+        """上错服务器了
+
+        该接口供渠道合作应用加固使用，接口调用有白名单用户限制，用于查询加固任务，入参中的条件过滤字段均为精准匹配。支持功能点：1. 多任务分页查询  2.根据任务Id唯一值查询单记录
 
         :param request: Request instance for DescribeEncryptInstances.
         :type request: :class:`tencentcloud.ms.v20180408.models.DescribeEncryptInstancesRequest`
         :rtype: :class:`tencentcloud.ms.v20180408.models.DescribeEncryptInstancesResponse`
 
         """
         try:
@@ -301,15 +309,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeOrderInstances(self, request):
-        """该接口供渠道合作应用加固使用，接口调用有白名单用户限制。 接口返回的结果为：创建订单后，订单审批状态信息，以及与订单关联的资源状态等信息，入参中的条件过滤字段均为精准匹配。
+        """上错服务器了
+
+        该接口供渠道合作应用加固使用，接口调用有白名单用户限制。 接口返回的结果为：创建订单后，订单审批状态信息，以及与订单关联的资源状态等信息，入参中的条件过滤字段均为精准匹配。
         接口功能点：
         1.支持多订单分页查询；
         2.支持唯一订单号精准匹配查询；
         3.支持唯一资源号精准匹配查询；
 
         :param request: Request instance for DescribeOrderInstances.
         :type request: :class:`tencentcloud.ms.v20180408.models.DescribeOrderInstancesRequest`
```

### Comparing `tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/errorcodes.py` & `tencentcloud-sdk-python-ms-3.0.948/tencentcloud/ms/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/models.py` & `tencentcloud-sdk-python-ms-3.0.948/tencentcloud/ms/v20180408/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,30 +137,30 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class AndroidPlan(AbstractModel):
-    """渠道合作安卓加固策略信息
+    """渠道合作Android加固策略信息
 
     """
 
     def __init__(self):
         r"""
         :param _PlanId: 非必输字段，PlanId 是指本次加固使用的配置策略Id，可通过载入上次配置接口获取。其值非0时，代表引用对应的策略。
         :type PlanId: int
         :param _AppPkgName: 本次操作的包名。
-当收费模式是安卓按年收费和安卓免费试用的在线加固和输出工具加固时，要求该字段必输，且与AndroidAppInfo.AppPkgName值相等。
+当收费模式是android按年收费和android免费试用的在线加固和输出工具加固时，要求该字段必输，且与AndroidAppInfo.AppPkgName值相等。
         :type AppPkgName: str
-        :param _AppType: 安卓app的文件类型，本次加固操作的应用类型 。 
-安卓在线加固和输出工具加固必输，其值需等于“apk”或“aab”，且与AndroidAppInfo.AppType值相等。
+        :param _AppType: android app的文件类型，本次加固操作的应用类型 。 
+android在线加固和输出工具加固必输，其值需等于“apk”或“aab”，且与AndroidAppInfo.AppType值相等。
 
         :type AppType: str
-        :param _EncryptParam: 安卓加固必输字段。
+        :param _EncryptParam: android加固必输字段。
 加固策略，json格式字符串。
 字段说明（0-关闭，1-开启）：
         "enable"=1 #DEX整体加固;
         "antiprotect"=1 #反调试;
         "antirepack"=1 #防重打包、防篡改;
         "dexsig"=1       #签名校验;
         "antimonitor"=1 #防模拟器运行保护;
@@ -320,29 +320,29 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class AndroidResult(AbstractModel):
-    """安卓加固结果
+    """Android加固结果
 
     """
 
     def __init__(self):
         r"""
         :param _ResultId: 结果Id,用于查询加固结果
         :type ResultId: str
         :param _OrderId: 与当前任务关联的订单id
         :type OrderId: str
         :param _ResourceId: 与当前任务关联的资源Id
         :type ResourceId: str
         :param _OpUin: 本次任务发起者
         :type OpUin: int
-        :param _AppType: 应用类型：安卓-apk; 安卓-aab;
+        :param _AppType: 应用类型：android-apk; android-aab;
         :type AppType: str
         :param _AppPkgName: 应用包名
         :type AppPkgName: str
         :param _BindAppPkgName: 后台资源绑定的包名
         :type BindAppPkgName: str
         :param _EncryptState: 加固结果
         :type EncryptState: int
@@ -358,43 +358,43 @@
         :type CreatTime: str
         :param _StartTime: 任务开始处理时间
         :type StartTime: str
         :param _EndTime: 任务处理结束时间
         :type EndTime: str
         :param _CostTime: 加固耗时（秒单位）
         :type CostTime: int
-        :param _AppUrl: 在线加固-安卓应用原包下载链接
+        :param _AppUrl: 在线加固-android应用原包下载链接
         :type AppUrl: str
-        :param _AppMd5: 在线加固-安卓应用文件MD5算法值
+        :param _AppMd5: 在线加固-android应用文件MD5算法值
         :type AppMd5: str
-        :param _AppName: 在线加固-安卓应用应用名称
+        :param _AppName: 在线加固-android应用应用名称
         :type AppName: str
-        :param _AppVersion: 在线加固-安卓应用版本；
+        :param _AppVersion: 在线加固-android应用版本；
         :type AppVersion: str
-        :param _AppSize: 在线加固-安卓应用大小
+        :param _AppSize: 在线加固-android应用大小
         :type AppSize: int
-        :param _OnlineToolVersion: 在线加固-安卓加固-腾讯云应用加固工具版本
+        :param _OnlineToolVersion: 在线加固-android加固-腾讯云应用加固工具版本
         :type OnlineToolVersion: str
-        :param _EncryptAppMd5: 在线加固-安卓加固，加固成功后文件md5算法值
+        :param _EncryptAppMd5: 在线加固-android加固，加固成功后文件md5算法值
         :type EncryptAppMd5: str
-        :param _EncryptAppSize: 在线加固-安卓加固，加固成功后应用大小
+        :param _EncryptAppSize: 在线加固-android加固，加固成功后应用大小
         :type EncryptAppSize: int
-        :param _EncryptPkgUrl: 在线加固-安卓加固，加固包下载链接。
+        :param _EncryptPkgUrl: 在线加固-android加固，加固包下载链接。
         :type EncryptPkgUrl: str
-        :param _OutputToolVersion: 输出工具-安卓加固-腾讯云输出工具版本
+        :param _OutputToolVersion: 输出工具-android加固-腾讯云输出工具版本
         :type OutputToolVersion: str
-        :param _OutputToolSize: 输出工具-安卓加固-工具大小
+        :param _OutputToolSize: 输出工具-android加固-工具大小
         :type OutputToolSize: int
-        :param _ToolOutputTime: 输出工具-安卓加固-工具输出时间
+        :param _ToolOutputTime: 输出工具-android加固-工具输出时间
         :type ToolOutputTime: str
-        :param _ToolExpireTime: 输出工具-安卓加固-工具到期时间
+        :param _ToolExpireTime: 输出工具-android加固-工具到期时间
         :type ToolExpireTime: str
-        :param _OutputToolUrl: 输出工具-安卓加固-输出工具下载链接
+        :param _OutputToolUrl: 输出工具-android加固-输出工具下载链接
         :type OutputToolUrl: str
-        :param _AndroidPlan: 本次安卓加固策略信息
+        :param _AndroidPlan: 本次android加固策略信息
         :type AndroidPlan: :class:`tencentcloud.ms.v20180408.models.AndroidPlan`
         """
         self._ResultId = None
         self._OrderId = None
         self._ResourceId = None
         self._OpUin = None
         self._AppType = None
@@ -4154,31 +4154,31 @@
 class EncryptResults(AbstractModel):
     """渠道合作加固结果信息
 
     """
 
     def __init__(self):
         r"""
-        :param _PlatformType: 平台类型枚举值  1-android安卓加固   2-ios源码混淆  3-sdk加固  4-applet小程序加固
+        :param _PlatformType: 平台类型枚举值  1-android加固   2-ios源码混淆  3-sdk加固  4-applet小程序加固
         :type PlatformType: int
-        :param _PlatformDesc: 平台类型描述  1-android安卓加固   2-ios源码混淆  3-sdk加固  4-applet小程序加固
+        :param _PlatformDesc: 平台类型描述  1-android加固   2-ios源码混淆  3-sdk加固  4-applet小程序加固
         :type PlatformDesc: str
         :param _OrderType: 订单采购类型枚举值， 1-免费试用 2-按年收费 3-按次收费
         :type OrderType: int
         :param _OrderTypeDesc: 订单采购类型 描述：1-免费试用 2-按年收费 3-按次收费
         :type OrderTypeDesc: str
         :param _EncryptOpType: 枚举值：1-在线加固 或 2-输出工具加固
         :type EncryptOpType: int
         :param _EncryptOpTypeDesc: 描述：1-在线加固 或 2-输出工具加固
         :type EncryptOpTypeDesc: str
         :param _ResourceId: 与当前任务关联的资源Id
         :type ResourceId: str
         :param _OrderId: 与当前任务关联的订单Id
         :type OrderId: str
-        :param _AndroidResult: 对应PlatformType平台类型值   1-android安卓加固结果
+        :param _AndroidResult: 对应PlatformType平台类型值   1-android加固结果
 注意：此字段可能返回 null，表示取不到有效值。
         :type AndroidResult: :class:`tencentcloud.ms.v20180408.models.AndroidResult`
         :param _IOSResult: 对应PlatformType平台类型值   2-ios源码混淆加固结果
 注意：此字段可能返回 null，表示取不到有效值。
         :type IOSResult: :class:`tencentcloud.ms.v20180408.models.IOSResult`
         :param _SDKResult: 对应PlatformType平台类型值   3-sdk加固结果
 注意：此字段可能返回 null，表示取不到有效值。
@@ -4503,21 +4503,21 @@
 
     def __init__(self):
         r"""
         :param _OrderId: 订单号
         :type OrderId: str
         :param _PlatformType: 平台类型整型值 
         :type PlatformType: int
-        :param _PlatformTypeDesc: 平台类型描述：  1.android安卓加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
+        :param _PlatformTypeDesc: 平台类型描述：  1.android加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
         :type PlatformTypeDesc: str
         :param _OrderType: 订单采购类型整型值
         :type OrderType: int
         :param _OrderTypeDesc: 订单采购类型描述： 1-免费试用 2-按年收费 3-按次收费
         :type OrderTypeDesc: str
-        :param _AppPkgName: 安卓包年收费加固的包名
+        :param _AppPkgName: android包年收费加固的包名
         :type AppPkgName: str
         :param _ResourceId: 资源号
         :type ResourceId: str
         :param _ResourceStatus: 资源状态整型值
         :type ResourceStatus: int
         :param _ResourceStatusDesc: 资源状态描述
 0-未生效、1-生效中、2-已失效。
```

### Comparing `tencentcloud-sdk-python-ms-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ms-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ms-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.948/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.947/README.rst` & `tencentcloud-sdk-python-ms-3.0.948/README.rst`

 * *Files identical despite different names*

