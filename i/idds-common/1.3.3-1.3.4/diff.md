# Comparing `tmp/idds-common-1.3.3.tar.gz` & `tmp/idds-common-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-common-1.3.3.tar", last modified: Fri Jul 21 07:10:54 2023, max compression
+gzip compressed data, was "idds-common-1.3.4.tar", last modified: Wed Aug  2 09:00:07 2023, max compression
```

## Comparing `idds-common-1.3.3.tar` & `idds-common-1.3.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:54.956872 idds-common-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 07:10:42.000000 idds-common-1.3.3/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-21 07:10:54.956872 idds-common-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-21 07:10:42.000000 idds-common-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:54.952872 idds-common-1.3.3/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:54.952872 idds-common-1.3.3/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:54.956872 idds-common-1.3.3/lib/idds/common/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22621 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/dict_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:54.956872 idds-common-1.3.3/lib/idds/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/plugin/plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-07-21 07:10:42.000000 idds-common-1.3.3/lib/idds/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 07:10:52.000000 idds-common-1.3.3/lib/idds/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:54.956872 idds-common-1.3.3/lib/idds_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-21 07:10:54.000000 idds-common-1.3.3/lib/idds_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-21 07:10:54.000000 idds-common-1.3.3/lib/idds_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:10:54.000000 idds-common-1.3.3/lib/idds_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 07:10:54.000000 idds-common-1.3.3/lib/idds_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 07:10:54.000000 idds-common-1.3.3/lib/idds_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-21 07:10:54.956872 idds-common-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-21 07:10:42.000000 idds-common-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:54.952872 idds-common-1.3.3/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:54.956872 idds-common-1.3.3/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-21 07:10:52.000000 idds-common-1.3.3/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:07.421442 idds-common-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-02 08:59:54.000000 idds-common-1.3.4/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-02 09:00:07.421442 idds-common-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-02 08:59:54.000000 idds-common-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:07.417442 idds-common-1.3.4/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:07.417442 idds-common-1.3.4/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:07.417442 idds-common-1.3.4/lib/idds/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22621 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/dict_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:07.421442 idds-common-1.3.4/lib/idds/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/plugin/plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-08-02 08:59:54.000000 idds-common-1.3.4/lib/idds/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-02 09:00:05.000000 idds-common-1.3.4/lib/idds/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:07.421442 idds-common-1.3.4/lib/idds_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-02 09:00:07.000000 idds-common-1.3.4/lib/idds_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-02 09:00:07.000000 idds-common-1.3.4/lib/idds_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:00:07.000000 idds-common-1.3.4/lib/idds_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 09:00:07.000000 idds-common-1.3.4/lib/idds_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 09:00:07.000000 idds-common-1.3.4/lib/idds_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-02 09:00:07.421442 idds-common-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-08-02 08:59:54.000000 idds-common-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:07.417442 idds-common-1.3.4/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:07.421442 idds-common-1.3.4/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-02 09:00:05.000000 idds-common-1.3.4/tools/env/environment.yml
```

### Comparing `idds-common-1.3.3/LICENSE.rst` & `idds-common-1.3.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/PKG-INFO` & `idds-common-1.3.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-common
-Version: 1.3.3
+Version: 1.3.4
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-common-1.3.3/lib/idds/common/authentication.py` & `idds-common-1.3.4/lib/idds/common/authentication.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/lib/idds/common/cache.py` & `idds-common-1.3.4/lib/idds/common/cache.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/lib/idds/common/config.py` & `idds-common-1.3.4/lib/idds/common/config.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/lib/idds/common/constants.py` & `idds-common-1.3.4/lib/idds/common/constants.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/lib/idds/common/dict_class.py` & `idds-common-1.3.4/lib/idds/common/dict_class.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/lib/idds/common/event.py` & `idds-common-1.3.4/lib/idds/common/event.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/lib/idds/common/exceptions.py` & `idds-common-1.3.4/lib/idds/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/lib/idds/common/plugin/plugin_base.py` & `idds-common-1.3.4/lib/idds/common/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/lib/idds/common/plugin/plugin_utils.py` & `idds-common-1.3.4/lib/idds/common/plugin/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/lib/idds/common/status_utils.py` & `idds-common-1.3.4/lib/idds/common/status_utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/lib/idds/common/utils.py` & `idds-common-1.3.4/lib/idds/common/utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/lib/idds_common.egg-info/PKG-INFO` & `idds-common-1.3.4/lib/idds_common.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-common
-Version: 1.3.3
+Version: 1.3.4
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-common-1.3.3/lib/idds_common.egg-info/SOURCES.txt` & `idds-common-1.3.4/lib/idds_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-common-1.3.3/setup.py` & `idds-common-1.3.4/setup.py`

 * *Files identical despite different names*

