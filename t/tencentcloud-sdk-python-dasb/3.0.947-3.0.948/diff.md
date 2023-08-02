# Comparing `tmp/tencentcloud-sdk-python-dasb-3.0.947.tar.gz` & `tmp/tencentcloud-sdk-python-dasb-3.0.948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.947.tar", last modified: Tue Aug  1 00:35:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.948.tar", last modified: Wed Aug  2 00:27:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dasb-3.0.947.tar` & `tencentcloud-sdk-python-dasb-3.0.948.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/dasb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/dasb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/dasb/v20191018/
--rw-r--r--   0 root         (0) root         (0)    45781 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/dasb/v20191018/dasb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/dasb/v20191018/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/dasb/v20191018/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   259761 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/dasb/v20191018/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud_sdk_python_dasb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-08-01 00:35:23.000000 tencentcloud-sdk-python-dasb-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/dasb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/dasb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/dasb/v20191018/
+-rw-r--r--   0 root         (0) root         (0)    45781 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/dasb/v20191018/dasb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/dasb/v20191018/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/dasb/v20191018/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   260513 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/dasb/v20191018/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud_sdk_python_dasb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      506 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud_sdk_python_dasb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-02 00:27:53.000000 tencentcloud-sdk-python-dasb-3.0.948/README.rst
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.947/setup.py` & `tencentcloud-sdk-python-dasb-3.0.948/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-dasb',
+    install_requires=["tencentcloud-sdk-python-common==3.0.948"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Dasb SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/dasb/v20191018/dasb_client.py` & `tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/dasb/v20191018/dasb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/dasb/v20191018/errorcodes.py` & `tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/dasb/v20191018/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/dasb/v20191018/models.py` & `tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/dasb/v20191018/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5043,14 +5043,17 @@
         :type SubnetId: str
         :param _Resource: 堡垒机服务信息，注意没有绑定服务时为null
 注意：此字段可能返回 null，表示取不到有效值。
         :type Resource: :class:`tencentcloud.dasb.v20191018.models.Resource`
         :param _Department: 资产所属部门
 注意：此字段可能返回 null，表示取不到有效值。
         :type Department: :class:`tencentcloud.dasb.v20191018.models.Department`
+        :param _IpPortSet: 数据库资产的多节点
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IpPortSet: list of str
         """
         self._Id = None
         self._InstanceId = None
         self._Name = None
         self._PublicIp = None
         self._PrivateIp = None
         self._ApCode = None
@@ -5059,14 +5062,15 @@
         self._Port = None
         self._GroupSet = None
         self._AccountCount = None
         self._VpcId = None
         self._SubnetId = None
         self._Resource = None
         self._Department = None
+        self._IpPortSet = None
 
     @property
     def Id(self):
         return self._Id
 
     @Id.setter
     def Id(self, Id):
@@ -5180,14 +5184,22 @@
     def Department(self):
         return self._Department
 
     @Department.setter
     def Department(self, Department):
         self._Department = Department
 
+    @property
+    def IpPortSet(self):
+        return self._IpPortSet
+
+    @IpPortSet.setter
+    def IpPortSet(self, IpPortSet):
+        self._IpPortSet = IpPortSet
+
 
     def _deserialize(self, params):
         self._Id = params.get("Id")
         self._InstanceId = params.get("InstanceId")
         self._Name = params.get("Name")
         self._PublicIp = params.get("PublicIp")
         self._PrivateIp = params.get("PrivateIp")
@@ -5206,14 +5218,15 @@
         self._SubnetId = params.get("SubnetId")
         if params.get("Resource") is not None:
             self._Resource = Resource()
             self._Resource._deserialize(params.get("Resource"))
         if params.get("Department") is not None:
             self._Department = Department()
             self._Department._deserialize(params.get("Department"))
+        self._IpPortSet = params.get("IpPortSet")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -5314,20 +5327,23 @@
         :type Ip: str
         :param _Port: 管理端口
         :type Port: int
         :param _Name: 主机名，可为空
         :type Name: str
         :param _DepartmentId: 资产所属的部门ID
         :type DepartmentId: str
+        :param _IpPortSet: 资产多节点：字段ip和端口
+        :type IpPortSet: list of str
         """
         self._OsName = None
         self._Ip = None
         self._Port = None
         self._Name = None
         self._DepartmentId = None
+        self._IpPortSet = None
 
     @property
     def OsName(self):
         return self._OsName
 
     @OsName.setter
     def OsName(self, OsName):
@@ -5361,21 +5377,30 @@
     def DepartmentId(self):
         return self._DepartmentId
 
     @DepartmentId.setter
     def DepartmentId(self, DepartmentId):
         self._DepartmentId = DepartmentId
 
+    @property
+    def IpPortSet(self):
+        return self._IpPortSet
+
+    @IpPortSet.setter
+    def IpPortSet(self, IpPortSet):
+        self._IpPortSet = IpPortSet
+
 
     def _deserialize(self, params):
         self._OsName = params.get("OsName")
         self._Ip = params.get("Ip")
         self._Port = params.get("Port")
         self._Name = params.get("Name")
         self._DepartmentId = params.get("DepartmentId")
+        self._IpPortSet = params.get("IpPortSet")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.947/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dasb-3.0.948/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dasb-3.0.947/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.948/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.947/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.948/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.947
+Version: 3.0.948
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.947/README.rst` & `tencentcloud-sdk-python-dasb-3.0.948/README.rst`

 * *Files identical despite different names*

