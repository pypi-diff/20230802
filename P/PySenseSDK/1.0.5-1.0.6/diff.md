# Comparing `tmp/PySenseSDK-1.0.5.tar.gz` & `tmp/PySenseSDK-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Nathan\PycharmProjects\PySense\dist\.tmp-5iocp1m4\PySenseSDK-1.0.5.tar", last modified: Sat Nov 26 21:05:10 2022, max compression
+gzip compressed data, was "PySenseSDK-1.0.6.tar", last modified: Tue Aug  1 23:49:38 2023, max compression
```

## Comparing `PySenseSDK-1.0.5.tar` & `PySenseSDK-1.0.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2022-11-26 21:05:10.791272 PySenseSDK-1.0.5/
--rw-rw-rw-   0        0        0    35821 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     3356 2022-11-26 21:05:10.791272 PySenseSDK-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-11-26 21:05:10.755368 PySenseSDK-1.0.5/PySense/
--rw-rw-rw-   0        0        0     6029 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySense.py
--rw-rw-rw-   0        0        0     2522 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseAuthentication.py
--rw-rw-rw-   0        0        0     1058 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseBloxAction.py
--rw-rw-rw-   0        0        0      526 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseBranding.py
--rw-rw-rw-   0        0        0     1268 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseBuildTask.py
--rw-rw-rw-   0        0        0      600 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseConnection.py
--rw-rw-rw-   0        0        0    20711 2021-08-25 20:52:26.000000 PySenseSDK-1.0.5/PySense/PySenseDashboard.py
--rw-rw-rw-   0        0        0     5159 2022-11-26 20:49:26.000000 PySenseSDK-1.0.5/PySense/PySenseDataModel.py
--rw-rw-rw-   0        0        0     3376 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseDataSet.py
--rw-rw-rw-   0        0        0    20105 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseElasticube.py
--rw-rw-rw-   0        0        0      122 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseException.py
--rw-rw-rw-   0        0        0      802 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseFolder.py
--rw-rw-rw-   0        0        0     2010 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseGroup.py
-drwxrwxrwx   0        0        0        0 2022-11-26 21:05:10.784290 PySenseSDK-1.0.5/PySense/PySenseMixIns/
--rw-rw-rw-   0        0        0      503 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseMixIns/BrandingMixIn.py
--rw-rw-rw-   0        0        0     2583 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseMixIns/ConnectionMixIn.py
--rw-rw-rw-   0        0        0    10364 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseMixIns/DashboardMixIn.py
--rw-rw-rw-   0        0        0     7673 2022-11-26 20:49:31.000000 PySenseSDK-1.0.5/PySense/PySenseMixIns/DataModelMixIn.py
--rw-rw-rw-   0        0        0     2925 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseMixIns/ElasticubeMixIn.py
--rw-rw-rw-   0        0        0     3794 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseMixIns/FolderMixIn.py
--rw-rw-rw-   0        0        0     4056 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseMixIns/GroupMixIn.py
--rw-rw-rw-   0        0        0     3464 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseMixIns/PluginMixIn.py
--rw-rw-rw-   0        0        0      946 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseMixIns/RoleMixIn.py
--rw-rw-rw-   0        0        0      456 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseMixIns/SettingsMixIn.py
--rw-rw-rw-   0        0        0     6980 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseMixIns/UserMixIn.py
--rw-rw-rw-   0        0        0        0 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseMixIns/__init__.py
--rw-rw-rw-   0        0        0     1557 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySensePlugin.py
--rw-rw-rw-   0        0        0     5102 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseRestConnector.py
--rw-rw-rw-   0        0        0     5328 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseRule.py
--rw-rw-rw-   0        0        0     2701 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseTable.py
--rw-rw-rw-   0        0        0     4635 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseUser.py
--rw-rw-rw-   0        0        0     2027 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseUtils.py
--rw-rw-rw-   0        0        0     3412 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/PySenseWidget.py
--rw-rw-rw-   0        0        0     1077 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/SisenseRole.py
--rw-rw-rw-   0        0        0      206 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/SisenseVersion.py
--rw-rw-rw-   0        0        0        0 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/PySense/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-26 21:05:10.772323 PySenseSDK-1.0.5/PySenseSDK.egg-info/
--rw-rw-rw-   0        0        0     3356 2022-11-26 21:05:10.000000 PySenseSDK-1.0.5/PySenseSDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2022-11-26 21:05:10.000000 PySenseSDK-1.0.5/PySenseSDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-26 21:05:10.000000 PySenseSDK-1.0.5/PySenseSDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-11-26 21:05:10.000000 PySenseSDK-1.0.5/PySenseSDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-11-26 21:05:10.000000 PySenseSDK-1.0.5/PySenseSDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2891 2022-11-26 20:53:49.000000 PySenseSDK-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2022-11-26 21:05:10.792269 PySenseSDK-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      758 2022-11-26 20:52:21.000000 PySenseSDK-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-26 21:05:10.789277 PySenseSDK-1.0.5/test/
--rw-rw-rw-   0        0        0     4346 2021-04-02 04:25:49.000000 PySenseSDK-1.0.5/test/TestMain.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:49:38.704229 PySenseSDK-1.0.6/
+-rw-rw-rw-   0        0        0    35821 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3164 2023-08-01 23:49:38.703232 PySenseSDK-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 23:49:38.678300 PySenseSDK-1.0.6/PySense/
+-rw-rw-rw-   0        0        0     6029 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySense.py
+-rw-rw-rw-   0        0        0     2522 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseAuthentication.py
+-rw-rw-rw-   0        0        0     1058 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseBloxAction.py
+-rw-rw-rw-   0        0        0      526 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseBranding.py
+-rw-rw-rw-   0        0        0     1268 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseBuildTask.py
+-rw-rw-rw-   0        0        0      600 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseConnection.py
+-rw-rw-rw-   0        0        0    20711 2021-08-25 20:52:26.000000 PySenseSDK-1.0.6/PySense/PySenseDashboard.py
+-rw-rw-rw-   0        0        0     5159 2022-11-26 20:49:26.000000 PySenseSDK-1.0.6/PySense/PySenseDataModel.py
+-rw-rw-rw-   0        0        0     3376 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseDataSet.py
+-rw-rw-rw-   0        0        0    20105 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseElasticube.py
+-rw-rw-rw-   0        0        0      122 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseException.py
+-rw-rw-rw-   0        0        0      802 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseFolder.py
+-rw-rw-rw-   0        0        0     2010 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseGroup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:49:38.701238 PySenseSDK-1.0.6/PySense/PySenseMixIns/
+-rw-rw-rw-   0        0        0      503 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseMixIns/BrandingMixIn.py
+-rw-rw-rw-   0        0        0     2583 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseMixIns/ConnectionMixIn.py
+-rw-rw-rw-   0        0        0    10364 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseMixIns/DashboardMixIn.py
+-rw-rw-rw-   0        0        0     7673 2022-11-26 20:49:31.000000 PySenseSDK-1.0.6/PySense/PySenseMixIns/DataModelMixIn.py
+-rw-rw-rw-   0        0        0     2925 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseMixIns/ElasticubeMixIn.py
+-rw-rw-rw-   0        0        0     3794 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseMixIns/FolderMixIn.py
+-rw-rw-rw-   0        0        0     4056 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseMixIns/GroupMixIn.py
+-rw-rw-rw-   0        0        0     3464 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseMixIns/PluginMixIn.py
+-rw-rw-rw-   0        0        0      946 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseMixIns/RoleMixIn.py
+-rw-rw-rw-   0        0        0      456 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseMixIns/SettingsMixIn.py
+-rw-rw-rw-   0        0        0     6980 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseMixIns/UserMixIn.py
+-rw-rw-rw-   0        0        0        0 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseMixIns/__init__.py
+-rw-rw-rw-   0        0        0     1557 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySensePlugin.py
+-rw-rw-rw-   0        0        0     5102 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseRestConnector.py
+-rw-rw-rw-   0        0        0     5328 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseRule.py
+-rw-rw-rw-   0        0        0     2701 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseTable.py
+-rw-rw-rw-   0        0        0     4634 2023-08-01 23:42:26.000000 PySenseSDK-1.0.6/PySense/PySenseUser.py
+-rw-rw-rw-   0        0        0     2027 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseUtils.py
+-rw-rw-rw-   0        0        0     3412 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/PySenseWidget.py
+-rw-rw-rw-   0        0        0     1077 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/SisenseRole.py
+-rw-rw-rw-   0        0        0      206 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/SisenseVersion.py
+-rw-rw-rw-   0        0        0        0 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/PySense/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:49:38.688273 PySenseSDK-1.0.6/PySenseSDK.egg-info/
+-rw-rw-rw-   0        0        0     3164 2023-08-01 23:49:38.000000 PySenseSDK-1.0.6/PySenseSDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2023-08-01 23:49:38.000000 PySenseSDK-1.0.6/PySenseSDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 23:49:38.000000 PySenseSDK-1.0.6/PySenseSDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-01 23:49:38.000000 PySenseSDK-1.0.6/PySenseSDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-01 23:49:38.000000 PySenseSDK-1.0.6/PySenseSDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2699 2023-08-01 23:46:19.000000 PySenseSDK-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 23:49:38.704229 PySenseSDK-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-08-01 23:48:24.000000 PySenseSDK-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:49:38.702235 PySenseSDK-1.0.6/test/
+-rw-rw-rw-   0        0        0     4346 2021-04-02 04:25:49.000000 PySenseSDK-1.0.6/test/TestMain.py
```

### Comparing `PySenseSDK-1.0.5/LICENSE` & `PySenseSDK-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PKG-INFO` & `PySenseSDK-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySenseSDK
-Version: 1.0.5
+Version: 1.0.6
 Summary: Sisense Python SDK
 Home-page: https://github.com/nathangiusti/PySense
 Author: Nathan Giusti
 Author-email: nathanggiusti@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -63,23 +63,22 @@
 If you need help installing Python/PyCharm, see our [tutorial](https://github.com/nathangiusti/PySense/raw/master/Installing%20Python.pptx)
 
 Install PySense with pip:
 - pip install PySenseSDK
 
 [Tutorial Videos](https://www.youtube.com/playlist?list=PL0xO3VH5OF2JD2KiZs_41zvKvPyebg6MW)
 
-**V 1.0.5 Release Notes**
+**V 1.0.6 Release Notes**
 
 - Breaking changes
     - None
 
 - Additions
-    - Datamodel exports can now return as a string. Before these changes you could only save the model to a file.
-    - Split up the import_schema function from DataModelMixIn to provide functionality to upload a schema from dictionary.
-        
-- Fixes
     - None
+  
+- Fixes
+    - Resolve issue with id vs oid in User.update()
     
 - Known Issues
     - REST API sometimes becomes unresponsive on Linux builds
     - REST API sometimes fails uploading sdata files
```

### Comparing `PySenseSDK-1.0.5/PySense/PySense.py` & `PySenseSDK-1.0.6/PySense/PySense.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseAuthentication.py` & `PySenseSDK-1.0.6/PySense/PySenseAuthentication.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseBloxAction.py` & `PySenseSDK-1.0.6/PySense/PySenseBloxAction.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseBranding.py` & `PySenseSDK-1.0.6/PySense/PySenseBranding.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseBuildTask.py` & `PySenseSDK-1.0.6/PySense/PySenseBuildTask.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseConnection.py` & `PySenseSDK-1.0.6/PySense/PySenseConnection.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseDashboard.py` & `PySenseSDK-1.0.6/PySense/PySenseDashboard.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseDataModel.py` & `PySenseSDK-1.0.6/PySense/PySenseDataModel.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseDataSet.py` & `PySenseSDK-1.0.6/PySense/PySenseDataSet.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseElasticube.py` & `PySenseSDK-1.0.6/PySense/PySenseElasticube.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseFolder.py` & `PySenseSDK-1.0.6/PySense/PySenseFolder.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseGroup.py` & `PySenseSDK-1.0.6/PySense/PySenseGroup.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseMixIns/ConnectionMixIn.py` & `PySenseSDK-1.0.6/PySense/PySenseMixIns/ConnectionMixIn.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseMixIns/DashboardMixIn.py` & `PySenseSDK-1.0.6/PySense/PySenseMixIns/DashboardMixIn.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseMixIns/DataModelMixIn.py` & `PySenseSDK-1.0.6/PySense/PySenseMixIns/DataModelMixIn.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseMixIns/ElasticubeMixIn.py` & `PySenseSDK-1.0.6/PySense/PySenseMixIns/ElasticubeMixIn.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseMixIns/FolderMixIn.py` & `PySenseSDK-1.0.6/PySense/PySenseMixIns/FolderMixIn.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseMixIns/GroupMixIn.py` & `PySenseSDK-1.0.6/PySense/PySenseMixIns/GroupMixIn.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseMixIns/PluginMixIn.py` & `PySenseSDK-1.0.6/PySense/PySenseMixIns/PluginMixIn.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseMixIns/RoleMixIn.py` & `PySenseSDK-1.0.6/PySense/PySenseMixIns/RoleMixIn.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseMixIns/UserMixIn.py` & `PySenseSDK-1.0.6/PySense/PySenseMixIns/UserMixIn.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySensePlugin.py` & `PySenseSDK-1.0.6/PySense/PySensePlugin.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseRestConnector.py` & `PySenseSDK-1.0.6/PySense/PySenseRestConnector.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseRule.py` & `PySenseSDK-1.0.6/PySense/PySenseRule.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseTable.py` & `PySenseSDK-1.0.6/PySense/PySenseTable.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseUser.py` & `PySenseSDK-1.0.6/PySense/PySenseUser.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             groups (list[Group]): (Optional) New set of groups for user
             preferences (JSON): (Optional) Preferences to be updated for user
         """
 
         user_groups = groups if groups is not None else self.get_groups()
         group_arr = []
         for group in PySenseUtils.make_iterable(user_groups):
-            group_arr.append(group.get_oid())
+            group_arr.append(group.get_id())
 
         user_json = {
                 'email': email if email else self.get_email(),
                 'userName': user_name if user_name else self.get_user_name(),
                 'firstName': first_name if first_name else self.get_first_name(),
                 'lastName': last_name if last_name else self.get_last_name(),
                 'roleId': self.py_client.get_role_id(role) if role else self.get_role_id(),
```

### Comparing `PySenseSDK-1.0.5/PySense/PySenseUtils.py` & `PySenseSDK-1.0.6/PySense/PySenseUtils.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/PySenseWidget.py` & `PySenseSDK-1.0.6/PySense/PySenseWidget.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySense/SisenseRole.py` & `PySenseSDK-1.0.6/PySense/SisenseRole.py`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/PySenseSDK.egg-info/PKG-INFO` & `PySenseSDK-1.0.6/PySenseSDK.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySenseSDK
-Version: 1.0.5
+Version: 1.0.6
 Summary: Sisense Python SDK
 Home-page: https://github.com/nathangiusti/PySense
 Author: Nathan Giusti
 Author-email: nathanggiusti@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -63,23 +63,22 @@
 If you need help installing Python/PyCharm, see our [tutorial](https://github.com/nathangiusti/PySense/raw/master/Installing%20Python.pptx)
 
 Install PySense with pip:
 - pip install PySenseSDK
 
 [Tutorial Videos](https://www.youtube.com/playlist?list=PL0xO3VH5OF2JD2KiZs_41zvKvPyebg6MW)
 
-**V 1.0.5 Release Notes**
+**V 1.0.6 Release Notes**
 
 - Breaking changes
     - None
 
 - Additions
-    - Datamodel exports can now return as a string. Before these changes you could only save the model to a file.
-    - Split up the import_schema function from DataModelMixIn to provide functionality to upload a schema from dictionary.
-        
-- Fixes
     - None
+  
+- Fixes
+    - Resolve issue with id vs oid in User.update()
     
 - Known Issues
     - REST API sometimes becomes unresponsive on Linux builds
     - REST API sometimes fails uploading sdata files
```

### Comparing `PySenseSDK-1.0.5/PySenseSDK.egg-info/SOURCES.txt` & `PySenseSDK-1.0.6/PySenseSDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySenseSDK-1.0.5/README.md` & `PySenseSDK-1.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -49,23 +49,22 @@
 If you need help installing Python/PyCharm, see our [tutorial](https://github.com/nathangiusti/PySense/raw/master/Installing%20Python.pptx)
 
 Install PySense with pip:
 - pip install PySenseSDK
 
 [Tutorial Videos](https://www.youtube.com/playlist?list=PL0xO3VH5OF2JD2KiZs_41zvKvPyebg6MW)
 
-**V 1.0.5 Release Notes**
+**V 1.0.6 Release Notes**
 
 - Breaking changes
     - None
 
 - Additions
-    - Datamodel exports can now return as a string. Before these changes you could only save the model to a file.
-    - Split up the import_schema function from DataModelMixIn to provide functionality to upload a schema from dictionary.
-        
-- Fixes
     - None
+  
+- Fixes
+    - Resolve issue with id vs oid in User.update()
     
 - Known Issues
     - REST API sometimes becomes unresponsive on Linux builds
     - REST API sometimes fails uploading sdata files
```

### Comparing `PySenseSDK-1.0.5/setup.py` & `PySenseSDK-1.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PySenseSDK",
-    version="1.0.5",
+    version="1.0.6",
     author="Nathan Giusti",
     author_email="nathanggiusti@gmail.com",
     description="Sisense Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nathangiusti/PySense",
     packages=setuptools.find_packages(),
```

### Comparing `PySenseSDK-1.0.5/test/TestMain.py` & `PySenseSDK-1.0.6/test/TestMain.py`

 * *Files identical despite different names*

