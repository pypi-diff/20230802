# Comparing `tmp/bootloader_core_library-0.0.6.tar.gz` & `tmp/bootloader_core_library-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootloader_core_library-0.0.6.tar", max compression
+gzip compressed data, was "bootloader_core_library-0.0.7.tar", max compression
```

## Comparing `bootloader_core_library-0.0.6.tar` & `bootloader_core_library-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      863 2023-08-01 15:46:21.346633 bootloader_core_library-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 bootloader_core_library-0.0.6/LICENSE.md
--rw-r--r--   0        0        0      138 2023-08-01 09:48:11.340859 bootloader_core_library-0.0.6/README.md
--rw-r--r--   0        0        0      905 2023-08-01 15:46:21.354932 bootloader_core_library-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 bootloader_core_library-0.0.6/src/bootloader/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.992853 bootloader_core_library-0.0.6/src/bootloader/ue/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.6/src/bootloader/ue/constant/__init__.py
--rw-r--r--   0        0        0    17232 2023-08-01 14:15:12.075340 bootloader_core_library-0.0.6/src/bootloader/ue/constant/ue_asset.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.6/src/bootloader/ue/model/__init__.py
--rw-r--r--   0        0        0    15017 2023-08-01 15:45:54.887029 bootloader_core_library-0.0.6/src/bootloader/ue/model/ue_asset.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.6/setup.py
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      986 2023-08-02 01:31:31.449458 bootloader_core_library-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 bootloader_core_library-0.0.7/LICENSE.md
+-rw-r--r--   0        0        0      138 2023-08-01 09:48:11.340859 bootloader_core_library-0.0.7/README.md
+-rw-r--r--   0        0        0      905 2023-08-02 01:31:37.634661 bootloader_core_library-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 bootloader_core_library-0.0.7/src/bootloader/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.992853 bootloader_core_library-0.0.7/src/bootloader/ue/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.7/src/bootloader/ue/constant/__init__.py
+-rw-r--r--   0        0        0    17232 2023-08-01 14:15:12.075340 bootloader_core_library-0.0.7/src/bootloader/ue/constant/ue_asset.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.7/src/bootloader/ue/model/__init__.py
+-rw-r--r--   0        0        0    15563 2023-08-02 01:30:11.913814 bootloader_core_library-0.0.7/src/bootloader/ue/model/ue_asset.py
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.7/setup.py
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.7/PKG-INFO
```

### Comparing `bootloader_core_library-0.0.6/CHANGELOG.md` & `bootloader_core_library-0.0.7/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), 
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [0.0.7] - 2024-08-02
+### Added
+- Add the method "__str__" to stringify the representation of an asset or an asset file
+
 ## [0.0.6] - 2024-08-02
 ### Added
 - Add the properties "object_status", "references", "tags", "update_time", and "version_code"
 
 ## [0.0.5] - 2024-08-02
 ### Added
 - Allow the properties "asset_name" and "package_name" to be updated
```

### Comparing `bootloader_core_library-0.0.6/LICENSE.md` & `bootloader_core_library-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.6/pyproject.toml` & `bootloader_core_library-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 keywords = ["core", "library"]
 license = "SEE LICENSE IN <LICENSE.md>"
 name = "bootloader-core-library"
 packages = [{include = "bootloader", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/bootloader-studio/bootloader-core-python-library"
-version = "0.0.6"
+version = "0.0.7"
 
 [tool.poetry.dependencies]
 perseus-core-library = "^1.19.4"
 python = "^3.10"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `bootloader_core_library-0.0.6/src/bootloader/__init__.py` & `bootloader_core_library-0.0.7/src/bootloader/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.6/src/bootloader/ue/__init__.py` & `bootloader_core_library-0.0.7/src/bootloader/ue/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.6/src/bootloader/ue/constant/__init__.py` & `bootloader_core_library-0.0.7/src/bootloader/ue/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.6/src/bootloader/ue/constant/ue_asset.py` & `bootloader_core_library-0.0.7/src/bootloader/ue/constant/ue_asset.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.6/src/bootloader/ue/model/__init__.py` & `bootloader_core_library-0.0.7/src/bootloader/ue/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.6/src/bootloader/ue/model/ue_asset.py` & `bootloader_core_library-0.0.7/src/bootloader/ue/model/ue_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import logging
 import os
 from abc import abstractmethod
 from pathlib import Path
 from uuid import UUID
 
 from majormode.perseus.constant.obj import ObjectStatus
+from majormode.perseus.model import obj
 from majormode.perseus.model.date import ISO8601DateTime
 from majormode.perseus.utils import cast
 
 from bootloader.ue.constant.ue_asset import ASSET_CLASS_NAME_MAPPING
 from bootloader.ue.constant.ue_asset import UnrealEngineAssetClass
 
 
@@ -102,14 +103,23 @@
         self.__dependencies = dependencies
         self.__references = references
         self.__tags = tags
         self.__object_status = object_status
         self.__update_time = update_time
         self.__version_code = version_code
 
+    def __str__(self):
+        """
+        Return the string representation of this asset.
+
+
+        :return: Return a stringified JSON expression of this asset.
+        """
+        return json.dumps(obj.stringify(self.to_json(), trimmable=True))
+
     @property
     def asset_class(self) -> UnrealEngineAssetClass:
         """
         Return the asset's class.
 
         For example, the class of a `/Script/Engine/SkeletalMesh` asset is
         `AssetClass.SkeletalMesh`
@@ -325,14 +335,23 @@
             self,
             asset: UnrealEngineAsset):
         """
         Build a new {@link UAsset}.
         """
         self.__asset = asset
 
+    def __str__(self):
+        """
+        Return the string representation of this asset file.
+
+
+        :return: Return a stringified JSON expression of this asset file.
+        """
+        return json.dumps(obj.stringify(self.to_json(), trimmable=True))
+
     @property
     def asset(self) -> UnrealEngineAsset:
         """
         Return the information of the asset contained in this file.
 
 
         :return: An asset.
```

### Comparing `bootloader_core_library-0.0.6/setup.py` & `bootloader_core_library-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['perseus-core-library>=1.19.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'bootloader-core-library',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'Repository of reusable Python components to be shared by Python projects using the Bootloader services',
     'long_description': '# Bootloader Core Python Library\n\nRepository of reusable Python components to be shared by Python projects using the Bootloader services.\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel@bootloader.studio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bootloader-studio/bootloader-core-python-library',
```

### Comparing `bootloader_core_library-0.0.6/PKG-INFO` & `bootloader_core_library-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootloader-core-library
-Version: 0.0.6
+Version: 0.0.7
 Summary: Repository of reusable Python components to be shared by Python projects using the Bootloader services
 Home-page: https://github.com/bootloader-studio/bootloader-core-python-library
 License: SEE LICENSE IN <LICENSE.md>
 Keywords: core,library
 Author: Daniel CAUNE
 Author-email: daniel@bootloader.studio
 Requires-Python: >=3.10,<4.0
```

