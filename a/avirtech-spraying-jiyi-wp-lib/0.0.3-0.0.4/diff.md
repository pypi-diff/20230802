# Comparing `tmp/avirtech_spraying_jiyi_wp_lib-0.0.3.tar.gz` & `tmp/avirtech_spraying_jiyi_wp_lib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avirtech_spraying_jiyi_wp_lib-0.0.3.tar", last modified: Wed Aug  2 13:09:43 2023, max compression
+gzip compressed data, was "avirtech_spraying_jiyi_wp_lib-0.0.4.tar", last modified: Wed Aug  2 13:12:37 2023, max compression
```

## Comparing `avirtech_spraying_jiyi_wp_lib-0.0.3.tar` & `avirtech_spraying_jiyi_wp_lib-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 13:09:43.583176 avirtech_spraying_jiyi_wp_lib-0.0.3/
--rw-rw-rw-   0        0        0     1447 2023-08-02 13:09:43.582014 avirtech_spraying_jiyi_wp_lib-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      648 2023-08-02 13:03:59.000000 avirtech_spraying_jiyi_wp_lib-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 13:09:43.548801 avirtech_spraying_jiyi_wp_lib-0.0.3/avirtech_spraying_jiyi_wp_lib/
--rw-rw-rw-   0        0        0       50 2023-08-02 13:06:00.000000 avirtech_spraying_jiyi_wp_lib-0.0.3/avirtech_spraying_jiyi_wp_lib/__init__.py
--rw-rw-rw-   0        0        0    32888 2023-08-02 12:38:47.000000 avirtech_spraying_jiyi_wp_lib-0.0.3/avirtech_spraying_jiyi_wp_lib/avirtech_spraying_jiyi_wp.py
-drwxrwxrwx   0        0        0        0 2023-08-02 13:09:43.579719 avirtech_spraying_jiyi_wp_lib-0.0.3/avirtech_spraying_jiyi_wp_lib.egg-info/
--rw-rw-rw-   0        0        0     1447 2023-08-02 13:09:42.000000 avirtech_spraying_jiyi_wp_lib-0.0.3/avirtech_spraying_jiyi_wp_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-08-02 13:09:43.000000 avirtech_spraying_jiyi_wp_lib-0.0.3/avirtech_spraying_jiyi_wp_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 13:09:42.000000 avirtech_spraying_jiyi_wp_lib-0.0.3/avirtech_spraying_jiyi_wp_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-08-02 13:09:42.000000 avirtech_spraying_jiyi_wp_lib-0.0.3/avirtech_spraying_jiyi_wp_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-08-02 13:09:42.000000 avirtech_spraying_jiyi_wp_lib-0.0.3/avirtech_spraying_jiyi_wp_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 13:09:43.583176 avirtech_spraying_jiyi_wp_lib-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1450 2023-08-02 13:09:32.000000 avirtech_spraying_jiyi_wp_lib-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:12:37.380312 avirtech_spraying_jiyi_wp_lib-0.0.4/
+-rw-rw-rw-   0        0        0     1441 2023-08-02 13:12:37.379389 avirtech_spraying_jiyi_wp_lib-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2023-08-02 13:12:21.000000 avirtech_spraying_jiyi_wp_lib-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 13:12:37.349398 avirtech_spraying_jiyi_wp_lib-0.0.4/avirtech_spraying_jiyi_wp_lib/
+-rw-rw-rw-   0        0        0       50 2023-08-02 13:06:00.000000 avirtech_spraying_jiyi_wp_lib-0.0.4/avirtech_spraying_jiyi_wp_lib/__init__.py
+-rw-rw-rw-   0        0        0    32888 2023-08-02 12:38:47.000000 avirtech_spraying_jiyi_wp_lib-0.0.4/avirtech_spraying_jiyi_wp_lib/avirtech_spraying_jiyi_wp.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:12:37.376359 avirtech_spraying_jiyi_wp_lib-0.0.4/avirtech_spraying_jiyi_wp_lib.egg-info/
+-rw-rw-rw-   0        0        0     1441 2023-08-02 13:12:35.000000 avirtech_spraying_jiyi_wp_lib-0.0.4/avirtech_spraying_jiyi_wp_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-08-02 13:12:37.000000 avirtech_spraying_jiyi_wp_lib-0.0.4/avirtech_spraying_jiyi_wp_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 13:12:36.000000 avirtech_spraying_jiyi_wp_lib-0.0.4/avirtech_spraying_jiyi_wp_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-08-02 13:12:36.000000 avirtech_spraying_jiyi_wp_lib-0.0.4/avirtech_spraying_jiyi_wp_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-08-02 13:12:36.000000 avirtech_spraying_jiyi_wp_lib-0.0.4/avirtech_spraying_jiyi_wp_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 13:12:37.381310 avirtech_spraying_jiyi_wp_lib-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1450 2023-08-02 13:12:08.000000 avirtech_spraying_jiyi_wp_lib-0.0.4/setup.py
```

### Comparing `avirtech_spraying_jiyi_wp_lib-0.0.3/PKG-INFO` & `avirtech_spraying_jiyi_wp_lib-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avirtech_spraying_jiyi_wp_lib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Avirtech Python Library to Generate JIYI Drone Spraying Track Using Waypoint Data From Avirplaner
 Home-page: 
 Author: Mohammad ILham R
 Author-email: ilhamr.mohammad@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -24,12 +24,12 @@
 Data yang dibutuhkan adalah (.waypoint) hasil dari avirplaner. 
 Bila menggunakan data DSM(.tif) boleh menggunakan koordinat WGS_1984, maupun koordinat UTM.
 
 Data tersebut dilanjutkan di software Qgis, untuk diconvert menjadi (.kml), lalu di "dissolve".
 Data hasil dissolve dapat digunakan dalam aplikasi "AgriAsistant"
 
 Install
-pip install avirtech_spraying_jiyi_waypoint_lib
+pip install avirtech_spraying_jiyi_wp_lib
 
 Usage
 from avirtech_spraying_jiyi_wp_lib.avirtech_spraying_jiyi_wp import autocorrect
```

### Comparing `avirtech_spraying_jiyi_wp_lib-0.0.3/README.md` & `avirtech_spraying_jiyi_wp_lib-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 Data yang dibutuhkan adalah (.waypoint) hasil dari avirplaner. 
 Bila menggunakan data DSM(.tif) boleh menggunakan koordinat WGS_1984, maupun koordinat UTM.
 
 Data tersebut dilanjutkan di software Qgis, untuk diconvert menjadi (.kml), lalu di "dissolve".
 Data hasil dissolve dapat digunakan dalam aplikasi "AgriAsistant"
 
 Install
-pip install avirtech_spraying_jiyi_waypoint_lib
+pip install avirtech_spraying_jiyi_wp_lib
 
 Usage
 from avirtech_spraying_jiyi_wp_lib.avirtech_spraying_jiyi_wp import autocorrect
```

### Comparing `avirtech_spraying_jiyi_wp_lib-0.0.3/avirtech_spraying_jiyi_wp_lib/avirtech_spraying_jiyi_wp.py` & `avirtech_spraying_jiyi_wp_lib-0.0.4/avirtech_spraying_jiyi_wp_lib/avirtech_spraying_jiyi_wp.py`

 * *Files identical despite different names*

### Comparing `avirtech_spraying_jiyi_wp_lib-0.0.3/avirtech_spraying_jiyi_wp_lib.egg-info/PKG-INFO` & `avirtech_spraying_jiyi_wp_lib-0.0.4/avirtech_spraying_jiyi_wp_lib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avirtech-spraying-jiyi-wp-lib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Avirtech Python Library to Generate JIYI Drone Spraying Track Using Waypoint Data From Avirplaner
 Home-page: 
 Author: Mohammad ILham R
 Author-email: ilhamr.mohammad@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -24,12 +24,12 @@
 Data yang dibutuhkan adalah (.waypoint) hasil dari avirplaner. 
 Bila menggunakan data DSM(.tif) boleh menggunakan koordinat WGS_1984, maupun koordinat UTM.
 
 Data tersebut dilanjutkan di software Qgis, untuk diconvert menjadi (.kml), lalu di "dissolve".
 Data hasil dissolve dapat digunakan dalam aplikasi "AgriAsistant"
 
 Install
-pip install avirtech_spraying_jiyi_waypoint_lib
+pip install avirtech_spraying_jiyi_wp_lib
 
 Usage
 from avirtech_spraying_jiyi_wp_lib.avirtech_spraying_jiyi_wp import autocorrect
```

### Comparing `avirtech_spraying_jiyi_wp_lib-0.0.3/setup.py` & `avirtech_spraying_jiyi_wp_lib-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup( 
     name="avirtech_spraying_jiyi_wp_lib",
-    version="0.0.3",
+    version="0.0.4",
     description="Avirtech Python Library to Generate JIYI Drone Spraying Track Using Waypoint Data From Avirplaner",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Mohammad ILham R",
     author_email="ilhamr.mohammad@gmail.com",
     license="MIT",
```

