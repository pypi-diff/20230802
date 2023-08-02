# Comparing `tmp/tencentcloud-sdk-python-tsf-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-tsf-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.947.tar", last modified: Tue Aug  1 00:59:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.948.tar", last modified: Wed Aug  2 00:40:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tsf-3.0.947.tar` & `tencentcloud-sdk-python-tsf-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/tsf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/tsf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/tsf/v20180326/
--rw-r--r--   0 root         (0) root         (0)   197194 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/tsf/v20180326/tsf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/tsf/v20180326/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50254 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/tsf/v20180326/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1288536 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/tsf/v20180326/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud_sdk_python_tsf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:59:22.000000 tencentcloud-sdk-python-tsf-3.0.947/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/tsf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/tsf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/tsf/v20180326/
+-rw-r--r--   0 root         (0) root         (0)   197194 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/tsf/v20180326/tsf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/tsf/v20180326/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50254 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/tsf/v20180326/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1289578 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/tsf/v20180326/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud_sdk_python_tsf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud_sdk_python_tsf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:40:45.000000 tencentcloud-sdk-python-tsf-3.0.948/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.947/setup.py` & `tencentcloud-sdk-python-tsf-3.0.948/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-tsf',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Tsf SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/tsf/v20180326/tsf_client.py` & `tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/tsf/v20180326/tsf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/tsf/v20180326/errorcodes.py` & `tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/tsf/v20180326/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.947/tencentcloud/tsf/v20180326/models.py` & `tencentcloud-sdk-python-tsf-3.0.948/tencentcloud/tsf/v20180326/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13796,14 +13796,16 @@
         :type JdkName: str
         :param _JdkVersion: JDK版本: 8或11 (openJDK只支持8)
         :type JdkVersion: str
         :param _AgentProfileList: 部署agent的类型、版本
         :type AgentProfileList: list of AgentProfile
         :param _WarmupSetting: 预热参数配置
         :type WarmupSetting: :class:`tencentcloud.tsf.v20180326.models.WarmupSetting`
+        :param _EnableBatchHealthCheck: 开启分批健康检查
+        :type EnableBatchHealthCheck: bool
         """
         self._GroupId = None
         self._PkgId = None
         self._StartupParameters = None
         self._DeployDesc = None
         self._ForceStart = None
         self._EnableHealthCheck = None
@@ -13816,14 +13818,15 @@
         self._StartScript = None
         self._StopScript = None
         self._IncrementalDeployment = None
         self._JdkName = None
         self._JdkVersion = None
         self._AgentProfileList = None
         self._WarmupSetting = None
+        self._EnableBatchHealthCheck = None
 
     @property
     def GroupId(self):
         return self._GroupId
 
     @GroupId.setter
     def GroupId(self, GroupId):
@@ -13969,14 +13972,22 @@
     def WarmupSetting(self):
         return self._WarmupSetting
 
     @WarmupSetting.setter
     def WarmupSetting(self, WarmupSetting):
         self._WarmupSetting = WarmupSetting
 
+    @property
+    def EnableBatchHealthCheck(self):
+        return self._EnableBatchHealthCheck
+
+    @EnableBatchHealthCheck.setter
+    def EnableBatchHealthCheck(self, EnableBatchHealthCheck):
+        self._EnableBatchHealthCheck = EnableBatchHealthCheck
+
 
     def _deserialize(self, params):
         self._GroupId = params.get("GroupId")
         self._PkgId = params.get("PkgId")
         self._StartupParameters = params.get("StartupParameters")
         self._DeployDesc = params.get("DeployDesc")
         self._ForceStart = params.get("ForceStart")
@@ -13999,14 +14010,15 @@
             for item in params.get("AgentProfileList"):
                 obj = AgentProfile()
                 obj._deserialize(item)
                 self._AgentProfileList.append(obj)
         if params.get("WarmupSetting") is not None:
             self._WarmupSetting = WarmupSetting()
             self._WarmupSetting._deserialize(params.get("WarmupSetting"))
+        self._EnableBatchHealthCheck = params.get("EnableBatchHealthCheck")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -43556,14 +43568,17 @@
         :type AgentProfileList: list of AgentProfile
         :param _WarmupSetting: 预热属性配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type WarmupSetting: :class:`tencentcloud.tsf.v20180326.models.WarmupSetting`
         :param _GatewayConfig: Envoy网关配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type GatewayConfig: :class:`tencentcloud.tsf.v20180326.models.GatewayConfig`
+        :param _EnableBatchHealthCheck: 批次是否开启健康检查
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EnableBatchHealthCheck: bool
         """
         self._GroupId = None
         self._GroupName = None
         self._GroupStatus = None
         self._PackageId = None
         self._PackageName = None
         self._PackageVersion = None
@@ -43595,14 +43610,15 @@
         self._PackageType = None
         self._StartScript = None
         self._StopScript = None
         self._Alias = None
         self._AgentProfileList = None
         self._WarmupSetting = None
         self._GatewayConfig = None
+        self._EnableBatchHealthCheck = None
 
     @property
     def GroupId(self):
         return self._GroupId
 
     @GroupId.setter
     def GroupId(self, GroupId):
@@ -43900,14 +43916,22 @@
     def GatewayConfig(self):
         return self._GatewayConfig
 
     @GatewayConfig.setter
     def GatewayConfig(self, GatewayConfig):
         self._GatewayConfig = GatewayConfig
 
+    @property
+    def EnableBatchHealthCheck(self):
+        return self._EnableBatchHealthCheck
+
+    @EnableBatchHealthCheck.setter
+    def EnableBatchHealthCheck(self, EnableBatchHealthCheck):
+        self._EnableBatchHealthCheck = EnableBatchHealthCheck
+
 
     def _deserialize(self, params):
         self._GroupId = params.get("GroupId")
         self._GroupName = params.get("GroupName")
         self._GroupStatus = params.get("GroupStatus")
         self._PackageId = params.get("PackageId")
         self._PackageName = params.get("PackageName")
@@ -43951,14 +43975,15 @@
                 self._AgentProfileList.append(obj)
         if params.get("WarmupSetting") is not None:
             self._WarmupSetting = WarmupSetting()
             self._WarmupSetting._deserialize(params.get("WarmupSetting"))
         if params.get("GatewayConfig") is not None:
             self._GatewayConfig = GatewayConfig()
             self._GatewayConfig._deserialize(params.get("GatewayConfig"))
+        self._EnableBatchHealthCheck = params.get("EnableBatchHealthCheck")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.948/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.947/README.rst` & `tencentcloud-sdk-python-tsf-3.0.948/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.947/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.948/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

