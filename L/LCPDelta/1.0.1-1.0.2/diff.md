# Comparing `tmp/LCPDelta-1.0.1.tar.gz` & `tmp/LCPDelta-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LCPDelta-1.0.1.tar", last modified: Wed Aug  2 11:53:23 2023, max compression
+gzip compressed data, was "LCPDelta-1.0.2.tar", last modified: Wed Aug  2 11:58:15 2023, max compression
```

## Comparing `LCPDelta-1.0.1.tar` & `LCPDelta-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 11:53:23.620742 LCPDelta-1.0.1/
--rw-rw-rw-   0        0        0      132 2023-08-02 11:28:18.000000 LCPDelta-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2402 2023-08-02 11:53:23.618785 LCPDelta-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1914 2023-08-02 11:41:22.000000 LCPDelta-1.0.1/README.md
--rw-rw-rw-   0        0        0      645 2023-08-02 11:53:01.000000 LCPDelta-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-02 11:53:23.620742 LCPDelta-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-02 11:53:23.553756 LCPDelta-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-02 11:53:23.564715 LCPDelta-1.0.1/src/LCPDelta/
-drwxrwxrwx   0        0        0        0 2023-08-02 11:53:23.616782 LCPDelta-1.0.1/src/LCPDelta/Enact/
--rw-rw-rw-   0        0        0    29435 2023-08-02 10:47:49.000000 LCPDelta-1.0.1/src/LCPDelta/Enact/APIHelper.py
--rw-rw-rw-   0        0        0     3688 2023-08-02 10:13:35.000000 LCPDelta-1.0.1/src/LCPDelta/Enact/CredentialsHolder.py
--rw-rw-rw-   0        0        0     4019 2023-08-02 10:47:38.000000 LCPDelta-1.0.1/src/LCPDelta/Enact/DPSHelper.py
--rw-rw-rw-   0        0        0      118 2023-08-02 10:21:02.000000 LCPDelta-1.0.1/src/LCPDelta/Enact/__init__.py
--rw-rw-rw-   0        0        0      275 2023-08-02 10:27:03.000000 LCPDelta-1.0.1/src/LCPDelta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 11:53:23.606830 LCPDelta-1.0.1/src/LCPDelta.egg-info/
--rw-rw-rw-   0        0        0     2402 2023-08-02 11:53:23.000000 LCPDelta-1.0.1/src/LCPDelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-08-02 11:53:23.000000 LCPDelta-1.0.1/src/LCPDelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 11:53:23.000000 LCPDelta-1.0.1/src/LCPDelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-08-02 11:53:23.000000 LCPDelta-1.0.1/src/LCPDelta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-02 11:53:23.000000 LCPDelta-1.0.1/src/LCPDelta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 11:58:15.906524 LCPDelta-1.0.2/
+-rw-rw-rw-   0        0        0      132 2023-08-02 11:28:18.000000 LCPDelta-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2405 2023-08-02 11:58:15.904529 LCPDelta-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1917 2023-08-02 11:57:14.000000 LCPDelta-1.0.2/README.md
+-rw-rw-rw-   0        0        0      645 2023-08-02 11:57:50.000000 LCPDelta-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 11:58:15.906524 LCPDelta-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 11:58:15.840886 LCPDelta-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 11:58:15.853887 LCPDelta-1.0.2/src/LCPDelta/
+drwxrwxrwx   0        0        0        0 2023-08-02 11:58:15.901526 LCPDelta-1.0.2/src/LCPDelta/Enact/
+-rw-rw-rw-   0        0        0    29435 2023-08-02 10:47:49.000000 LCPDelta-1.0.2/src/LCPDelta/Enact/APIHelper.py
+-rw-rw-rw-   0        0        0     3688 2023-08-02 10:13:35.000000 LCPDelta-1.0.2/src/LCPDelta/Enact/CredentialsHolder.py
+-rw-rw-rw-   0        0        0     4019 2023-08-02 10:47:38.000000 LCPDelta-1.0.2/src/LCPDelta/Enact/DPSHelper.py
+-rw-rw-rw-   0        0        0      118 2023-08-02 10:21:02.000000 LCPDelta-1.0.2/src/LCPDelta/Enact/__init__.py
+-rw-rw-rw-   0        0        0      275 2023-08-02 10:27:03.000000 LCPDelta-1.0.2/src/LCPDelta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:58:15.891523 LCPDelta-1.0.2/src/LCPDelta.egg-info/
+-rw-rw-rw-   0        0        0     2405 2023-08-02 11:58:15.000000 LCPDelta-1.0.2/src/LCPDelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-08-02 11:58:15.000000 LCPDelta-1.0.2/src/LCPDelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 11:58:15.000000 LCPDelta-1.0.2/src/LCPDelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-08-02 11:58:15.000000 LCPDelta-1.0.2/src/LCPDelta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 11:58:15.000000 LCPDelta-1.0.2/src/LCPDelta.egg-info/top_level.txt
```

### Comparing `LCPDelta-1.0.1/PKG-INFO` & `LCPDelta-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: LCPDelta
-Version: 1.0.1
+Version: 1.0.2
 Summary: LCPDelta Python Package
 Author-email: Sushanth Kolluru <enact.helpdesk@lcp.uk.com>
 Project-URL: Homepage, https://portal.lcpdelta.com/
 Keywords: LCPDelta,Enact,Flextrack,Storetrack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LCPDelta Python Package
 This is the python wrapper to interact with all LCPDelta products through their API or DPS. To get started, install the latest version of the LCPDelta package. 
 
-To find out more about LCPDelta's data products, click [**here**][LCPDelta_homepage_link].
+To find out more about LCPDelta's data products, click [**here**][LCPDelta_data_portal_link].
 To find out more about Enact, click [**here**][Enact_Homepage].
 ## Enact API and DPS Instructions
 
 Full instructions on how to utilise Enact's full API and DPS can be found [**here**][Enact_instructions_link]. Below are some examples to get you started. 
 
 ### API Example Code
```

### Comparing `LCPDelta-1.0.1/README.md` & `LCPDelta-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # LCPDelta Python Package
 This is the python wrapper to interact with all LCPDelta products through their API or DPS. To get started, install the latest version of the LCPDelta package. 
 
-To find out more about LCPDelta's data products, click [**here**][LCPDelta_homepage_link].
+To find out more about LCPDelta's data products, click [**here**][LCPDelta_data_portal_link].
 To find out more about Enact, click [**here**][Enact_Homepage].
 ## Enact API and DPS Instructions
 
 Full instructions on how to utilise Enact's full API and DPS can be found [**here**][Enact_instructions_link]. Below are some examples to get you started. 
 
 ### API Example Code
```

### Comparing `LCPDelta-1.0.1/pyproject.toml` & `LCPDelta-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LCPDelta"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Sushanth Kolluru", email="enact.helpdesk@lcp.uk.com" },
 ]
 description = "LCPDelta Python Package"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["LCPDelta", "Enact", "Flextrack", "Storetrack"]
```

### Comparing `LCPDelta-1.0.1/src/LCPDelta/Enact/APIHelper.py` & `LCPDelta-1.0.2/src/LCPDelta/Enact/APIHelper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.0.1/src/LCPDelta/Enact/CredentialsHolder.py` & `LCPDelta-1.0.2/src/LCPDelta/Enact/CredentialsHolder.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.0.1/src/LCPDelta/Enact/DPSHelper.py` & `LCPDelta-1.0.2/src/LCPDelta/Enact/DPSHelper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.0.1/src/LCPDelta.egg-info/PKG-INFO` & `LCPDelta-1.0.2/src/LCPDelta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: LCPDelta
-Version: 1.0.1
+Version: 1.0.2
 Summary: LCPDelta Python Package
 Author-email: Sushanth Kolluru <enact.helpdesk@lcp.uk.com>
 Project-URL: Homepage, https://portal.lcpdelta.com/
 Keywords: LCPDelta,Enact,Flextrack,Storetrack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LCPDelta Python Package
 This is the python wrapper to interact with all LCPDelta products through their API or DPS. To get started, install the latest version of the LCPDelta package. 
 
-To find out more about LCPDelta's data products, click [**here**][LCPDelta_homepage_link].
+To find out more about LCPDelta's data products, click [**here**][LCPDelta_data_portal_link].
 To find out more about Enact, click [**here**][Enact_Homepage].
 ## Enact API and DPS Instructions
 
 Full instructions on how to utilise Enact's full API and DPS can be found [**here**][Enact_instructions_link]. Below are some examples to get you started. 
 
 ### API Example Code
```

