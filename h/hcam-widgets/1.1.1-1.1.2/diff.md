# Comparing `tmp/hcam_widgets-1.1.1.tar.gz` & `tmp/hcam_widgets-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcam_widgets-1.1.1.tar", last modified: Thu Jul 27 22:10:41 2023, max compression
+gzip compressed data, was "hcam_widgets-1.1.2.tar", last modified: Wed Aug  2 08:24:57 2023, max compression
```

## Comparing `hcam_widgets-1.1.1.tar` & `hcam_widgets-1.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:10:41.543339 hcam_widgets-1.1.1/
--rw-r--r--   0 sl         (501) staff       (20)      166 2017-11-13 13:48:04.000000 hcam_widgets-1.1.1/AUTHORS.rst
--rw-r--r--   0 sl         (501) staff       (20)     3303 2017-11-13 15:08:00.000000 hcam_widgets-1.1.1/CONTRIBUTING.rst
--rw-r--r--   0 sl         (501) staff       (20)       89 2017-11-13 13:48:04.000000 hcam_widgets-1.1.1/HISTORY.rst
--rw-r--r--   0 sl         (501) staff       (20)     1077 2017-11-13 13:48:08.000000 hcam_widgets-1.1.1/LICENSE
--rw-r--r--   0 sl         (501) staff       (20)      303 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/MANIFEST.in
--rw-r--r--   0 sl         (501) staff       (20)     3306 2023-07-27 22:10:41.543400 hcam_widgets-1.1.1/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     2299 2018-02-15 16:29:54.000000 hcam_widgets-1.1.1/README.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:10:41.541643 hcam_widgets-1.1.1/hcam_widgets/
--rw-r--r--   0 sl         (501) staff       (20)      246 2023-07-27 22:09:32.000000 hcam_widgets-1.1.1/hcam_widgets/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     8880 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/astro.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:10:41.542708 hcam_widgets-1.1.1/hcam_widgets/compo/
--rw-r--r--   0 sl         (501) staff       (20)        0 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/compo/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)    15204 2023-07-27 22:08:39.000000 hcam_widgets-1.1.1/hcam_widgets/compo/utils.py
--rw-r--r--   0 sl         (501) staff       (20)    27122 2023-07-21 10:52:00.000000 hcam_widgets-1.1.1/hcam_widgets/compo/widgets.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:10:41.542834 hcam_widgets-1.1.1/hcam_widgets/data/
--rw-r--r--   0 sl         (501) staff       (20)     1704 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/data/compo_lens_offset.csv
--rw-r--r--   0 sl         (501) staff       (20)     7024 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/globals.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:10:41.543242 hcam_widgets-1.1.1/hcam_widgets/hardware/
--rw-r--r--   0 sl         (501) staff       (20)    17450 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/hardware/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     6312 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/hardware/alarms.py
--rw-r--r--   0 sl         (501) staff       (20)     4751 2023-07-21 10:52:00.000000 hcam_widgets-1.1.1/hcam_widgets/hardware/ccds.py
--rw-r--r--   0 sl         (501) staff       (20)     9157 2023-07-21 10:52:00.000000 hcam_widgets-1.1.1/hcam_widgets/hardware/slide.py
--rw-r--r--   0 sl         (501) staff       (20)    70257 2023-07-27 21:58:00.000000 hcam_widgets-1.1.1/hcam_widgets/hcam.py
--rw-r--r--   0 sl         (501) staff       (20)     4036 2018-02-15 16:29:54.000000 hcam_widgets-1.1.1/hcam_widgets/logs.py
--rw-r--r--   0 sl         (501) staff       (20)      370 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/mimic.py
--rw-r--r--   0 sl         (501) staff       (20)    20264 2023-07-27 22:08:39.000000 hcam_widgets-1.1.1/hcam_widgets/misc.py
--rw-r--r--   0 sl         (501) staff       (20)     2087 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/tcs.py
--rw-r--r--   0 sl         (501) staff       (20)     1880 2017-11-22 14:17:48.000000 hcam_widgets-1.1.1/hcam_widgets/tkutils.py
--rw-r--r--   0 sl         (501) staff       (20)    22334 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/ucam.py
--rw-r--r--   0 sl         (501) staff       (20)    36505 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/uspec.py
--rw-r--r--   0 sl         (501) staff       (20)   149251 2023-07-27 21:10:09.000000 hcam_widgets-1.1.1/hcam_widgets/widgets.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:10:41.542393 hcam_widgets-1.1.1/hcam_widgets.egg-info/
--rw-r--r--   0 sl         (501) staff       (20)     3306 2023-07-27 22:10:41.000000 hcam_widgets-1.1.1/hcam_widgets.egg-info/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)      827 2023-07-27 22:10:41.000000 hcam_widgets-1.1.1/hcam_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-27 22:10:41.000000 hcam_widgets-1.1.1/hcam_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-27 22:10:41.000000 hcam_widgets-1.1.1/hcam_widgets.egg-info/not-zip-safe
--rw-r--r--   0 sl         (501) staff       (20)       71 2023-07-27 22:10:41.000000 hcam_widgets-1.1.1/hcam_widgets.egg-info/requires.txt
--rw-r--r--   0 sl         (501) staff       (20)       13 2023-07-27 22:10:41.000000 hcam_widgets-1.1.1/hcam_widgets.egg-info/top_level.txt
--rw-r--r--   0 sl         (501) staff       (20)      313 2023-07-27 22:10:41.543620 hcam_widgets-1.1.1/setup.cfg
--rw-r--r--   0 sl         (501) staff       (20)     1909 2023-07-27 22:09:32.000000 hcam_widgets-1.1.1/setup.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:24:57.877961 hcam_widgets-1.1.2/
+-rw-r--r--   0 sl         (501) staff       (20)      166 2017-11-13 13:48:04.000000 hcam_widgets-1.1.2/AUTHORS.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3303 2017-11-13 15:08:00.000000 hcam_widgets-1.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 sl         (501) staff       (20)       89 2017-11-13 13:48:04.000000 hcam_widgets-1.1.2/HISTORY.rst
+-rw-r--r--   0 sl         (501) staff       (20)     1077 2017-11-13 13:48:08.000000 hcam_widgets-1.1.2/LICENSE
+-rw-r--r--   0 sl         (501) staff       (20)      303 2021-05-26 10:14:11.000000 hcam_widgets-1.1.2/MANIFEST.in
+-rw-r--r--   0 sl         (501) staff       (20)     3306 2023-08-02 08:24:57.878037 hcam_widgets-1.1.2/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     2299 2018-02-15 16:29:54.000000 hcam_widgets-1.1.2/README.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:24:57.876142 hcam_widgets-1.1.2/hcam_widgets/
+-rw-r--r--   0 sl         (501) staff       (20)      246 2023-08-02 08:24:50.000000 hcam_widgets-1.1.2/hcam_widgets/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     8880 2021-05-26 10:14:11.000000 hcam_widgets-1.1.2/hcam_widgets/astro.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:24:57.877251 hcam_widgets-1.1.2/hcam_widgets/compo/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2021-05-26 10:14:11.000000 hcam_widgets-1.1.2/hcam_widgets/compo/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)    15187 2023-08-02 08:24:16.000000 hcam_widgets-1.1.2/hcam_widgets/compo/utils.py
+-rw-r--r--   0 sl         (501) staff       (20)    27122 2023-07-21 10:52:00.000000 hcam_widgets-1.1.2/hcam_widgets/compo/widgets.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:24:57.877371 hcam_widgets-1.1.2/hcam_widgets/data/
+-rw-r--r--   0 sl         (501) staff       (20)     1704 2021-05-26 10:14:11.000000 hcam_widgets-1.1.2/hcam_widgets/data/compo_lens_offset.csv
+-rw-r--r--   0 sl         (501) staff       (20)     7024 2021-05-26 10:14:11.000000 hcam_widgets-1.1.2/hcam_widgets/globals.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:24:57.877833 hcam_widgets-1.1.2/hcam_widgets/hardware/
+-rw-r--r--   0 sl         (501) staff       (20)    17450 2021-05-26 10:14:11.000000 hcam_widgets-1.1.2/hcam_widgets/hardware/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     6312 2021-05-26 10:14:11.000000 hcam_widgets-1.1.2/hcam_widgets/hardware/alarms.py
+-rw-r--r--   0 sl         (501) staff       (20)     4751 2023-07-21 10:52:00.000000 hcam_widgets-1.1.2/hcam_widgets/hardware/ccds.py
+-rw-r--r--   0 sl         (501) staff       (20)     9157 2023-07-21 10:52:00.000000 hcam_widgets-1.1.2/hcam_widgets/hardware/slide.py
+-rw-r--r--   0 sl         (501) staff       (20)    70320 2023-07-27 23:49:10.000000 hcam_widgets-1.1.2/hcam_widgets/hcam.py
+-rw-r--r--   0 sl         (501) staff       (20)     4036 2018-02-15 16:29:54.000000 hcam_widgets-1.1.2/hcam_widgets/logs.py
+-rw-r--r--   0 sl         (501) staff       (20)      370 2021-05-26 10:14:11.000000 hcam_widgets-1.1.2/hcam_widgets/mimic.py
+-rw-r--r--   0 sl         (501) staff       (20)    20264 2023-07-27 22:08:39.000000 hcam_widgets-1.1.2/hcam_widgets/misc.py
+-rw-r--r--   0 sl         (501) staff       (20)     2087 2021-05-26 10:14:11.000000 hcam_widgets-1.1.2/hcam_widgets/tcs.py
+-rw-r--r--   0 sl         (501) staff       (20)     1880 2017-11-22 14:17:48.000000 hcam_widgets-1.1.2/hcam_widgets/tkutils.py
+-rw-r--r--   0 sl         (501) staff       (20)    22334 2021-05-26 10:14:11.000000 hcam_widgets-1.1.2/hcam_widgets/ucam.py
+-rw-r--r--   0 sl         (501) staff       (20)    36505 2021-05-26 10:14:11.000000 hcam_widgets-1.1.2/hcam_widgets/uspec.py
+-rw-r--r--   0 sl         (501) staff       (20)   149251 2023-07-27 21:10:09.000000 hcam_widgets-1.1.2/hcam_widgets/widgets.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:24:57.876951 hcam_widgets-1.1.2/hcam_widgets.egg-info/
+-rw-r--r--   0 sl         (501) staff       (20)     3306 2023-08-02 08:24:57.000000 hcam_widgets-1.1.2/hcam_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)      827 2023-08-02 08:24:57.000000 hcam_widgets-1.1.2/hcam_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-08-02 08:24:57.000000 hcam_widgets-1.1.2/hcam_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-08-02 08:24:57.000000 hcam_widgets-1.1.2/hcam_widgets.egg-info/not-zip-safe
+-rw-r--r--   0 sl         (501) staff       (20)       71 2023-08-02 08:24:57.000000 hcam_widgets-1.1.2/hcam_widgets.egg-info/requires.txt
+-rw-r--r--   0 sl         (501) staff       (20)       13 2023-08-02 08:24:57.000000 hcam_widgets-1.1.2/hcam_widgets.egg-info/top_level.txt
+-rw-r--r--   0 sl         (501) staff       (20)      313 2023-08-02 08:24:57.878275 hcam_widgets-1.1.2/setup.cfg
+-rw-r--r--   0 sl         (501) staff       (20)     1909 2023-08-02 08:24:50.000000 hcam_widgets-1.1.2/setup.py
```

### Comparing `hcam_widgets-1.1.1/CONTRIBUTING.rst` & `hcam_widgets-1.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/LICENSE` & `hcam_widgets-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/PKG-INFO` & `hcam_widgets-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam_widgets
-Version: 1.1.1
+Version: 1.1.2
 Summary: Common Tkinter widgets for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_widgets
-Download-URL: https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.1.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.2.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_widgets
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_widgets-1.1.1/README.rst` & `hcam_widgets-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/astro.py` & `hcam_widgets-1.1.2/hcam_widgets/astro.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/compo/utils.py` & `hcam_widgets-1.1.2/hcam_widgets/compo/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import print_function, unicode_literals, absolute_import, division
-import importlib
 
 # non-standard imports
 from astropy import units as u
 from astropy.coordinates.matrix_utilities import rotation_matrix
 from astropy.coordinates import CartesianRepresentation
 from astropy.utils import lazyproperty
 from scipy.interpolate import interp1d
```

### Comparing `hcam_widgets-1.1.1/hcam_widgets/compo/widgets.py` & `hcam_widgets-1.1.2/hcam_widgets/compo/widgets.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/data/compo_lens_offset.csv` & `hcam_widgets-1.1.2/hcam_widgets/data/compo_lens_offset.csv`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/globals.py` & `hcam_widgets-1.1.2/hcam_widgets/globals.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/hardware/__init__.py` & `hcam_widgets-1.1.2/hcam_widgets/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/hardware/alarms.py` & `hcam_widgets-1.1.2/hcam_widgets/hardware/alarms.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/hardware/ccds.py` & `hcam_widgets-1.1.2/hcam_widgets/hardware/ccds.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/hardware/slide.py` & `hcam_widgets-1.1.2/hcam_widgets/hardware/slide.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/hcam.py` & `hcam_widgets-1.1.2/hcam_widgets/hcam.py`

 * *Files 0% similar despite different names*

```diff
@@ -670,15 +670,16 @@
         status = True
         g = get_root(self).globals
 
         # if we've just enabled COMPO, then raise window if exists
         if self.compo():
             compo_hw_widget = getattr(g, "compo_hw", None)
             if compo_hw_widget is not None:
-                compo_hw_widget.deiconify()
+                if compo_hw_widget.state() == "withdrawn":
+                    compo_hw_widget.deiconify()
 
         # clear errors on binning (may be set later if FF)
         xbinw, ybinw = self.wframe.xbin, self.wframe.ybin
         xbinw.config(bg=g.COL["main"])
         ybinw.config(bg=g.COL["main"])
 
         # keep binning factors of drift mode and windowed mode up to date
```

### Comparing `hcam_widgets-1.1.1/hcam_widgets/logs.py` & `hcam_widgets-1.1.2/hcam_widgets/logs.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/misc.py` & `hcam_widgets-1.1.2/hcam_widgets/misc.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/tcs.py` & `hcam_widgets-1.1.2/hcam_widgets/tcs.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/tkutils.py` & `hcam_widgets-1.1.2/hcam_widgets/tkutils.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/ucam.py` & `hcam_widgets-1.1.2/hcam_widgets/ucam.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/uspec.py` & `hcam_widgets-1.1.2/hcam_widgets/uspec.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets/widgets.py` & `hcam_widgets-1.1.2/hcam_widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/hcam_widgets.egg-info/PKG-INFO` & `hcam_widgets-1.1.2/hcam_widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam-widgets
-Version: 1.1.1
+Version: 1.1.2
 Summary: Common Tkinter widgets for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_widgets
-Download-URL: https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.1.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.2.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_widgets
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_widgets-1.1.1/hcam_widgets.egg-info/SOURCES.txt` & `hcam_widgets-1.1.2/hcam_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.1/setup.py` & `hcam_widgets-1.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
 requirements = [
     "astropy",
     "requests",
     "twisted",
-    "hcam_devices>=1.0.0",
+    "hcam_devices>=1.0.1",
     "matplotlib",
     "scipy",
     "autobahn",
 ]
 
 test_requirements = [
     # TODO: put package test requirements here
@@ -30,21 +30,21 @@
     fname
     for fname in glob.glob(os.path.join("scripts", "*"))
     if os.path.basename(fname) != "README.rst"
 ]
 
 setup(
     name="hcam_widgets",
-    version="1.1.1",
+    version="1.1.2",
     description="Common Tkinter widgets for HiPerCAM",
     long_description=readme + "\n\n" + history,
     author="Stuart Littlefair",
     author_email="s.littlefair@shef.ac.uk",
     url="https://github.com/HiPERCAM/hcam_widgets",
-    download_url="https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.1.tar.gz",
+    download_url="https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.2.tar.gz",
     packages=["hcam_widgets", "hcam_widgets.compo", "hcam_widgets.hardware"],
     package_dir={"hcam_widgets": "hcam_widgets"},
     include_package_data=True,
     install_requires=requirements,
     license="MIT license",
     zip_safe=False,
     keywords="hcam_widgets",
```

