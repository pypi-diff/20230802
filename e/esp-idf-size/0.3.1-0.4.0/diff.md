# Comparing `tmp/esp-idf-size-0.3.1.tar.gz` & `tmp/esp-idf-size-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-size/esp-idf-size/dist/.tmp-zosoa97p/esp-idf-size-0.3.1.tar", last modified: Thu May 18 09:54:53 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-size/esp-idf-size/dist/.tmp-jfzxdncb/esp-idf-size-0.4.0.tar", last modified: Wed Aug  2 11:59:27 2023, max compression
```

## Comparing `esp-idf-size-0.3.1.tar` & `esp-idf-size-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32c2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32c3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32c6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32h2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32h4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32s2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32s3.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    56338 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/test/test_idf_size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:27.000000 esp-idf-size-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-02 11:59:27.000000 esp-idf-size-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:27.000000 esp-idf-size-0.4.0/esp_idf_size/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/esp_idf_size/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/esp_idf_size/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:27.000000 esp-idf-size-0.4.0/esp_idf_size/chip_info/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/esp_idf_size/chip_info/esp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/esp_idf_size/chip_info/esp32c2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/esp_idf_size/chip_info/esp32c3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/esp_idf_size/chip_info/esp32c6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/esp_idf_size/chip_info/esp32h2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/esp_idf_size/chip_info/esp32h4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/esp_idf_size/chip_info/esp32p4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/esp_idf_size/chip_info/esp32s2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/esp_idf_size/chip_info/esp32s3.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56338 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/esp_idf_size/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:27.000000 esp-idf-size-0.4.0/esp_idf_size.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-02 11:59:27.000000 esp-idf-size-0.4.0/esp_idf_size.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-02 11:59:27.000000 esp-idf-size-0.4.0/esp_idf_size.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:59:27.000000 esp-idf-size-0.4.0/esp_idf_size.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-02 11:59:27.000000 esp-idf-size-0.4.0/esp_idf_size.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 11:59:27.000000 esp-idf-size-0.4.0/esp_idf_size.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 11:59:27.000000 esp-idf-size-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:27.000000 esp-idf-size-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-02 11:59:03.000000 esp-idf-size-0.4.0/test/test_idf_size.py
```

### Comparing `esp-idf-size-0.3.1/LICENSE` & `esp-idf-size-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-size-0.3.1/PKG-INFO` & `esp-idf-size-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-size
-Version: 0.3.1
+Version: 0.4.0
 Summary: Firmware size analysis for ESP-IDF
 Home-page: https://github.com/espressif/esp-idf-size
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,size
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32.yaml` & `esp-idf-size-0.4.0/esp_idf_size/chip_info/esp32.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32s2.yaml` & `esp-idf-size-0.4.0/esp_idf_size/chip_info/esp32s2.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32s3.yaml` & `esp-idf-size-0.4.0/esp_idf_size/chip_info/esp32s3.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-0.3.1/esp_idf_size/core.py` & `esp-idf-size-0.4.0/esp_idf_size/core.py`

 * *Files identical despite different names*

### Comparing `esp-idf-size-0.3.1/esp_idf_size.egg-info/PKG-INFO` & `esp-idf-size-0.4.0/esp_idf_size.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-size
-Version: 0.3.1
+Version: 0.4.0
 Summary: Firmware size analysis for ESP-IDF
 Home-page: https://github.com/espressif/esp-idf-size
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,size
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-size-0.3.1/esp_idf_size.egg-info/SOURCES.txt` & `esp-idf-size-0.4.0/esp_idf_size.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 esp_idf_size.egg-info/top_level.txt
 esp_idf_size/chip_info/esp32.yaml
 esp_idf_size/chip_info/esp32c2.yaml
 esp_idf_size/chip_info/esp32c3.yaml
 esp_idf_size/chip_info/esp32c6.yaml
 esp_idf_size/chip_info/esp32h2.yaml
 esp_idf_size/chip_info/esp32h4.yaml
+esp_idf_size/chip_info/esp32p4.yaml
 esp_idf_size/chip_info/esp32s2.yaml
 esp_idf_size/chip_info/esp32s3.yaml
 test/test_idf_size.py
```

### Comparing `esp-idf-size-0.3.1/setup.py` & `esp-idf-size-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `esp-idf-size-0.3.1/test/test_idf_size.py` & `esp-idf-size-0.4.0/test/test_idf_size.py`

 * *Files identical despite different names*

