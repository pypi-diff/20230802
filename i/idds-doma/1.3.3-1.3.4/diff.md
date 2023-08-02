# Comparing `tmp/idds-doma-1.3.3.tar.gz` & `tmp/idds-doma-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-doma-1.3.3.tar", last modified: Fri Jul 21 07:10:58 2023, max compression
+gzip compressed data, was "idds-doma-1.3.4.tar", last modified: Wed Aug  2 09:00:11 2023, max compression
```

## Comparing `idds-doma-1.3.3.tar` & `idds-doma-1.3.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:58.824865 idds-doma-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 07:10:42.000000 idds-doma-1.3.3/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-21 07:10:58.824865 idds-doma-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-21 07:10:42.000000 idds-doma-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:58.824865 idds-doma-1.3.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-07-21 07:10:42.000000 idds-doma-1.3.3/bin/setup_panda_token
--rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-07-21 07:10:42.000000 idds-doma-1.3.3/bin/setup_panda_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:58.820865 idds-doma-1.3.3/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:58.824865 idds-doma-1.3.3/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-doma-1.3.3/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:58.824865 idds-doma-1.3.3/lib/idds/doma/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-doma-1.3.3/lib/idds/doma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 07:10:52.000000 idds-doma-1.3.3/lib/idds/doma/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:58.824865 idds-doma-1.3.3/lib/idds/doma/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-doma-1.3.3/lib/idds/doma/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-07-21 07:10:42.000000 idds-doma-1.3.3/lib/idds/doma/workflow/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:58.824865 idds-doma-1.3.3/lib/idds/doma/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-doma-1.3.3/lib/idds/doma/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-21 07:10:42.000000 idds-doma-1.3.3/lib/idds/doma/workflowv2/domaeventmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    39387 2023-07-21 07:10:42.000000 idds-doma-1.3.3/lib/idds/doma/workflowv2/domapandaeswork.py
--rw-r--r--   0 runner    (1001) docker     (123)    59948 2023-07-21 07:10:42.000000 idds-doma-1.3.3/lib/idds/doma/workflowv2/domapandawork.py
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-07-21 07:10:42.000000 idds-doma-1.3.3/lib/idds/doma/workflowv2/domatree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:58.824865 idds-doma-1.3.3/lib/idds_doma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-21 07:10:58.000000 idds-doma-1.3.3/lib/idds_doma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-21 07:10:58.000000 idds-doma-1.3.3/lib/idds_doma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:10:58.000000 idds-doma-1.3.3/lib/idds_doma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-21 07:10:58.000000 idds-doma-1.3.3/lib/idds_doma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 07:10:58.000000 idds-doma-1.3.3/lib/idds_doma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-21 07:10:58.824865 idds-doma-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-21 07:10:42.000000 idds-doma-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:58.820865 idds-doma-1.3.3/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:58.824865 idds-doma-1.3.3/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-21 07:10:52.000000 idds-doma-1.3.3/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:11.645532 idds-doma-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-02 08:59:54.000000 idds-doma-1.3.4/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-02 09:00:11.645532 idds-doma-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-02 08:59:54.000000 idds-doma-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:11.645532 idds-doma-1.3.4/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-08-02 08:59:54.000000 idds-doma-1.3.4/bin/setup_panda_token
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-08-02 08:59:54.000000 idds-doma-1.3.4/bin/setup_panda_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:11.645532 idds-doma-1.3.4/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:11.645532 idds-doma-1.3.4/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-doma-1.3.4/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:11.645532 idds-doma-1.3.4/lib/idds/doma/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-doma-1.3.4/lib/idds/doma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-02 09:00:05.000000 idds-doma-1.3.4/lib/idds/doma/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:11.645532 idds-doma-1.3.4/lib/idds/doma/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-doma-1.3.4/lib/idds/doma/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-08-02 08:59:54.000000 idds-doma-1.3.4/lib/idds/doma/workflow/domapandawork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:11.645532 idds-doma-1.3.4/lib/idds/doma/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-doma-1.3.4/lib/idds/doma/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-08-02 08:59:54.000000 idds-doma-1.3.4/lib/idds/doma/workflowv2/domaeventmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39387 2023-08-02 08:59:54.000000 idds-doma-1.3.4/lib/idds/doma/workflowv2/domapandaeswork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59948 2023-08-02 08:59:54.000000 idds-doma-1.3.4/lib/idds/doma/workflowv2/domapandawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-08-02 08:59:54.000000 idds-doma-1.3.4/lib/idds/doma/workflowv2/domatree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:11.645532 idds-doma-1.3.4/lib/idds_doma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-02 09:00:11.000000 idds-doma-1.3.4/lib/idds_doma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-02 09:00:11.000000 idds-doma-1.3.4/lib/idds_doma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:00:11.000000 idds-doma-1.3.4/lib/idds_doma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 09:00:11.000000 idds-doma-1.3.4/lib/idds_doma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 09:00:11.000000 idds-doma-1.3.4/lib/idds_doma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-02 09:00:11.645532 idds-doma-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-02 08:59:54.000000 idds-doma-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:11.645532 idds-doma-1.3.4/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:11.645532 idds-doma-1.3.4/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-02 09:00:05.000000 idds-doma-1.3.4/tools/env/environment.yml
```

### Comparing `idds-doma-1.3.3/LICENSE.rst` & `idds-doma-1.3.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.3/PKG-INFO` & `idds-doma-1.3.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
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

### Comparing `idds-doma-1.3.3/bin/setup_panda_token` & `idds-doma-1.3.4/bin/setup_panda_token`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.3/bin/setup_panda_token.py` & `idds-doma-1.3.4/bin/setup_panda_token.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.3/lib/idds/doma/workflow/domapandawork.py` & `idds-doma-1.3.4/lib/idds/doma/workflow/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.3/lib/idds/doma/workflowv2/domaeventmap.py` & `idds-doma-1.3.4/lib/idds/doma/workflowv2/domaeventmap.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.3/lib/idds/doma/workflowv2/domapandaeswork.py` & `idds-doma-1.3.4/lib/idds/doma/workflowv2/domapandaeswork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.3/lib/idds/doma/workflowv2/domapandawork.py` & `idds-doma-1.3.4/lib/idds/doma/workflowv2/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.3/lib/idds/doma/workflowv2/domatree.py` & `idds-doma-1.3.4/lib/idds/doma/workflowv2/domatree.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.3/lib/idds_doma.egg-info/PKG-INFO` & `idds-doma-1.3.4/lib/idds_doma.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
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

### Comparing `idds-doma-1.3.3/lib/idds_doma.egg-info/SOURCES.txt` & `idds-doma-1.3.4/lib/idds_doma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-doma-1.3.3/setup.py` & `idds-doma-1.3.4/setup.py`

 * *Files identical despite different names*

