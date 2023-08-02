# Comparing `tmp/castor-orsay-2023.8.2.tar.gz` & `tmp/castor-orsay-2023.8.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castor-orsay-2023.8.2.tar", last modified: Wed Aug  2 11:28:59 2023, max compression
+gzip compressed data, was "castor-orsay-2023.8.2.1.tar", last modified: Wed Aug  2 11:46:33 2023, max compression
```

## Comparing `castor-orsay-2023.8.2.tar` & `castor-orsay-2023.8.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:28:59.184083 castor-orsay-2023.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-02 11:28:59.184083 castor-orsay-2023.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:28:59.180082 castor-orsay-2023.8.2/castor/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:28:59.180082 castor-orsay-2023.8.2/castor/_console_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1910 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/align.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/align_spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22987 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/exoplanet_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7616 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/pointing_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2205 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/prepare.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3587 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/rotate_spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2429 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/_console_scripts/wavelength_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/alignment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:28:59.180082 castor-orsay-2023.8.2/castor/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/data/instruments.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/files_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/mount_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/preparation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/castor/spectroscopy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:28:59.184083 castor-orsay-2023.8.2/castor_orsay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-02 11:28:59.000000 castor-orsay-2023.8.2/castor_orsay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-02 11:28:59.000000 castor-orsay-2023.8.2/castor_orsay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:28:59.000000 castor-orsay-2023.8.2/castor_orsay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 11:28:59.000000 castor-orsay-2023.8.2/castor_orsay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-02 11:28:59.000000 castor-orsay-2023.8.2/castor_orsay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 11:28:59.000000 castor-orsay-2023.8.2/castor_orsay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 11:28:59.184083 castor-orsay-2023.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-02 11:28:49.000000 castor-orsay-2023.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:33.060971 castor-orsay-2023.8.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-02 11:46:33.060971 castor-orsay-2023.8.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:33.060971 castor-orsay-2023.8.2.1/castor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:33.060971 castor-orsay-2023.8.2.1/castor/_console_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/_console_scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1910 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/_console_scripts/align.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/_console_scripts/align_spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22987 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/_console_scripts/exoplanet_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7616 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/_console_scripts/pointing_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2205 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/_console_scripts/prepare.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3587 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/_console_scripts/rotate_spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2429 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/_console_scripts/wavelength_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/alignment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:33.060971 castor-orsay-2023.8.2.1/castor/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/data/instruments.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/files_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/mount_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/preparation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/castor/spectroscopy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:33.060971 castor-orsay-2023.8.2.1/castor_orsay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-02 11:46:33.000000 castor-orsay-2023.8.2.1/castor_orsay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-02 11:46:33.000000 castor-orsay-2023.8.2.1/castor_orsay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:46:33.000000 castor-orsay-2023.8.2.1/castor_orsay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 11:46:33.000000 castor-orsay-2023.8.2.1/castor_orsay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-02 11:46:33.000000 castor-orsay-2023.8.2.1/castor_orsay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 11:46:33.000000 castor-orsay-2023.8.2.1/castor_orsay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 11:46:33.060971 castor-orsay-2023.8.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-02 11:46:23.000000 castor-orsay-2023.8.2.1/setup.py
```

### Comparing `castor-orsay-2023.8.2/LICENSE.txt` & `castor-orsay-2023.8.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/PKG-INFO` & `castor-orsay-2023.8.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castor-orsay
-Version: 2023.8.2
+Version: 2023.8.2.1
 Summary: Codes pour l’ASTronomie à ORsay
 Home-page: https://github.com/coupole-orsay/castor
 Author: Gabriel Pelouze, Aurélien Stcherbinine
 Author-email: gabriel.pelouze@ias.u-psud.fr, aurelien.stcherbinine@ias.u-psud.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `castor-orsay-2023.8.2/README.md` & `castor-orsay-2023.8.2.1/README.md`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/__init__.py` & `castor-orsay-2023.8.2.1/castor/__init__.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/_console_scripts/align.py` & `castor-orsay-2023.8.2.1/castor/_console_scripts/align.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/_console_scripts/align_spectra.py` & `castor-orsay-2023.8.2.1/castor/_console_scripts/align_spectra.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/_console_scripts/exoplanet_analysis.py` & `castor-orsay-2023.8.2.1/castor/_console_scripts/exoplanet_analysis.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/_console_scripts/pointing_analysis.py` & `castor-orsay-2023.8.2.1/castor/_console_scripts/pointing_analysis.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/_console_scripts/prepare.py` & `castor-orsay-2023.8.2.1/castor/_console_scripts/prepare.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/_console_scripts/rotate_spectra.py` & `castor-orsay-2023.8.2.1/castor/_console_scripts/rotate_spectra.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/_console_scripts/wavelength_calibration.py` & `castor-orsay-2023.8.2.1/castor/_console_scripts/wavelength_calibration.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/alignment.py` & `castor-orsay-2023.8.2.1/castor/alignment.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/data/instruments.yml` & `castor-orsay-2023.8.2.1/castor/data/instruments.yml`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/files_handling.py` & `castor-orsay-2023.8.2.1/castor/files_handling.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/mount_alignment.py` & `castor-orsay-2023.8.2.1/castor/mount_alignment.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/photometry.py` & `castor-orsay-2023.8.2.1/castor/photometry.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/preparation.py` & `castor-orsay-2023.8.2.1/castor/preparation.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor/spectroscopy.py` & `castor-orsay-2023.8.2.1/castor/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/castor_orsay.egg-info/PKG-INFO` & `castor-orsay-2023.8.2.1/castor_orsay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castor-orsay
-Version: 2023.8.2
+Version: 2023.8.2.1
 Summary: Codes pour l’ASTronomie à ORsay
 Home-page: https://github.com/coupole-orsay/castor
 Author: Gabriel Pelouze, Aurélien Stcherbinine
 Author-email: gabriel.pelouze@ias.u-psud.fr, aurelien.stcherbinine@ias.u-psud.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `castor-orsay-2023.8.2/castor_orsay.egg-info/SOURCES.txt` & `castor-orsay-2023.8.2.1/castor_orsay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `castor-orsay-2023.8.2/setup.py` & `castor-orsay-2023.8.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 package_data = {
     '': ['data/*'],
     }
 
 setuptools.setup(
     name='castor-orsay',
-    version='2023.8.2',
+    version='2023.8.2.1',
     author='Gabriel Pelouze, Aurélien Stcherbinine',
     author_email='gabriel.pelouze@ias.u-psud.fr, aurelien.stcherbinine@ias.u-psud.fr',
     description='Codes pour l’ASTronomie à ORsay',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/coupole-orsay/castor',
     packages=setuptools.find_packages(),
```

