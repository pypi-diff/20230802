# Comparing `tmp/plbm_liumou_stable-1.3.8.tar.gz` & `tmp/plbm_liumou_stable-1.3.9.tar.gz`

## Comparing `plbm_liumou_stable-1.3.8.tar` & `plbm_liumou_stable-1.3.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/DemoModule.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/UploadToPypi.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/demo.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/install.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/req.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/requirements.txt
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/demo/package.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/disk/DiskInformation.py
--rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/file/7z.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/file/Rename.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/model/docker.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/model/install_pac_list.py
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/model/package.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/model/pacman.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/model/pip.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/model/source.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/network/ReplaceIP.py
--rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/AptManage.py
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Cmd.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Docker.py
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Dpkg.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/FileManagement.py
--rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Iptables.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Jurisdiction.py
--rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/NetManagement.py
--rw-r--r--   0        0        0     7160 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/NetStatus.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/OsInfo.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Package.py
--rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/README.md
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Service.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Source.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Yum.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/base.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/get.py
--rw-r--r--   0        0        0     8742 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/logger.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/requirements.txt
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/txt.log
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/security/__init__.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/security/firewalld.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/LICENSE
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/README.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/DemoModule.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/UploadToPypi.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/demo.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/install.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/req.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/requirements.txt
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/demo/package.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/disk/DiskInformation.py
+-rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/file/7z.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/file/Rename.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/model/docker.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/model/install_pac_list.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/model/package.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/model/pacman.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/model/pip.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/model/source.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/network/ReplaceIP.py
+-rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/AptManage.py
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Cmd.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Docker.py
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Dpkg.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/FileManagement.py
+-rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Iptables.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Jurisdiction.py
+-rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/NetManagement.py
+-rw-r--r--   0        0        0     7160 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/NetStatus.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/OsInfo.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Package.py
+-rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/README.md
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Service.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Source.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Yum.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/base.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/get.py
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/logger.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/requirements.txt
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/txt.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/security/__init__.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/security/firewalld.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/LICENSE
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/PKG-INFO
```

### Comparing `plbm_liumou_stable-1.3.8/DemoModule.py` & `plbm_liumou_stable-1.3.9/DemoModule.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/UploadToPypi.py` & `plbm_liumou_stable-1.3.9/UploadToPypi.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/demo.py` & `plbm_liumou_stable-1.3.9/demo.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/install.py` & `plbm_liumou_stable-1.3.9/install.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/demo/package.py` & `plbm_liumou_stable-1.3.9/demo/package.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/disk/DiskInformation.py` & `plbm_liumou_stable-1.3.9/disk/DiskInformation.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/file/7z.py` & `plbm_liumou_stable-1.3.9/file/7z.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/file/Rename.py` & `plbm_liumou_stable-1.3.9/file/Rename.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/model/docker.py` & `plbm_liumou_stable-1.3.9/model/docker.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/model/install_pac_list.py` & `plbm_liumou_stable-1.3.9/model/install_pac_list.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/model/package.py` & `plbm_liumou_stable-1.3.9/model/package.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/model/pacman.py` & `plbm_liumou_stable-1.3.9/model/pacman.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/model/pip.py` & `plbm_liumou_stable-1.3.9/model/pip.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/model/source.py` & `plbm_liumou_stable-1.3.9/model/source.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/network/ReplaceIP.py` & `plbm_liumou_stable-1.3.9/network/ReplaceIP.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/AptManage.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/AptManage.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Cmd.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Cmd.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Docker.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Docker.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Dpkg.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Dpkg.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/FileManagement.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/FileManagement.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Iptables.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Iptables.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Jurisdiction.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Jurisdiction.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/NetManagement.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/NetManagement.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/NetStatus.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/NetStatus.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/OsInfo.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/OsInfo.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Package.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Package.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/README.md` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/README.md`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Service.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Service.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Source.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Source.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/Yum.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Yum.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/__init__.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .OsInfo import *
 from .OsInfo import OsInfo
 from .Package import PackageManagement
 from .Service import ServiceManagement
 from .Yum import YumManager
 from .get import headers, cookies
 from .base import ListGetLen, ListRemoveNone
-from .logger import ColorLogger
+from .logger import ColorLogger, log
 
 __all__ = ["Command", "AptManagement", "DpkgManagement", "FileManagement", "Jurisdiction",
            "NetManagement", "NetStatus", "PackageManagement", "ServiceManagement", "YumManager", "IpTables",
-           "OsInfo", "NetworkCardInfo", "ListGetLen", "ListRemoveNone", "ColorLogger"]
+           "OsInfo", "NetworkCardInfo", "ListGetLen", "ListRemoveNone", "ColorLogger", "log"]
 
 if platform.system().lower() != 'linux'.lower():
 	print('Plmb模块仅支持Linux系统')
```

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/get.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/get.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/logger.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 		if self.format_line:
 			msg1 = str(msg1) + "  line: " + str(self.line_)
 		if self.class_name is not None and self.format_class:
 			msg1 = str(msg1) + " - Class: " + str(self.class_name)
 		if self.module_name != '<module>' and self.format_fun:
 			msg1 = str(msg1) + " Function: " + self.module_name
 		if self.format_level:
-			msg1 = str(msg1) + " - %s : " % level + msg
+			msg1 = str(msg1) + " - %s : " % str(level) + str(msg)
 		self.msg1 = msg1
 
 	def _wr(self):
 		try:
 			# 如果开启了文本日志
 			if self.txt_mode:
 				self.txt_wr.write(self.msg1)
```

### Comparing `plbm_liumou_stable-1.3.8/src/plbm_liumou_Stable/security/firewalld.py` & `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/security/firewalld.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/LICENSE` & `plbm_liumou_stable-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.8/README.md` & `plbm_liumou_stable-1.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 * 完全使用内置模块进行开发，拿来即用
 * 使用Python基础语法进行编写，兼容新旧版本Python3，告别语法冲突(例如3.5及以下版本无法使用f"{}"语法)
 * 完全开源、永久免费
 
 
 # 更新内容
 
-## `1.3.8`
+## `1.3.9`
 
-* 暴露`ColorLogger`类
+* 修正日志无法输出的问题
 
 
 # 使用方法
 
 ## 安装
 
 具体可以访问Pypi项目地址[https://pypi.org/project/plbm-liumou-Stable/](https://pypi.org/project/plbm-liumou-Stable/)
@@ -62,14 +62,15 @@
 @Homepage : https://liumou.site
 @Desc    :   当前文件作用
 """
 from plbm_liumou_Stable import PackageManagement
 from ColorInfo import ColorLogger
 
 
+
 class ServiceManager:
 	def __init__(self, pac, password):
 		self.package = pac
 		self.pac = PackageManagement(password=password, package="vsftpd")
 		self.logger = ColorLogger(class_name=self.__class__.__name__)
 
 	def remove(self):
```

### Comparing `plbm_liumou_stable-1.3.8/pyproject.toml` & `plbm_liumou_stable-1.3.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "plbm_liumou_Stable"
-version = "1.3.8"
+version = "1.3.9"
 authors = [
   { name="坐公交也用券", email="liumou.site@qq.com" },
 ]
 description = "使用Python3进行编写的一个开源系统管理工具， 通过封装Linux系统都软件包管理、磁盘管理、文件管理、网络管理、安全管理、服务管理等内容从而实现快速开发的效果"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `plbm_liumou_stable-1.3.8/PKG-INFO` & `plbm_liumou_stable-1.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plbm_liumou_Stable
-Version: 1.3.8
+Version: 1.3.9
 Summary: 使用Python3进行编写的一个开源系统管理工具， 通过封装Linux系统都软件包管理、磁盘管理、文件管理、网络管理、安全管理、服务管理等内容从而实现快速开发的效果
 Project-URL: Homepage, https://gitee.com/liumou_site/plbm
 Project-URL: Bug Tracker, https://gitee.com/liumou_site/plbm/issues
 Author-email: 坐公交也用券 <liumou.site@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,17 +28,17 @@
 * 完全使用内置模块进行开发，拿来即用
 * 使用Python基础语法进行编写，兼容新旧版本Python3，告别语法冲突(例如3.5及以下版本无法使用f"{}"语法)
 * 完全开源、永久免费
 
 
 # 更新内容
 
-## `1.3.8`
+## `1.3.9`
 
-* 暴露`ColorLogger`类
+* 修正日志无法输出的问题
 
 
 # 使用方法
 
 ## 安装
 
 具体可以访问Pypi项目地址[https://pypi.org/project/plbm-liumou-Stable/](https://pypi.org/project/plbm-liumou-Stable/)
@@ -76,14 +76,15 @@
 @Homepage : https://liumou.site
 @Desc    :   当前文件作用
 """
 from plbm_liumou_Stable import PackageManagement
 from ColorInfo import ColorLogger
 
 
+
 class ServiceManager:
 	def __init__(self, pac, password):
 		self.package = pac
 		self.pac = PackageManagement(password=password, package="vsftpd")
 		self.logger = ColorLogger(class_name=self.__class__.__name__)
 
 	def remove(self):
```

