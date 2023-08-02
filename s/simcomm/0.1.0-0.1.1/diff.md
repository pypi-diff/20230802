# Comparing `tmp/simcomm-0.1.0.tar.gz` & `tmp/simcomm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simcomm-0.1.0.tar", last modified: Wed Aug  2 10:49:32 2023, max compression
+gzip compressed data, was "simcomm-0.1.1.tar", last modified: Wed Aug  2 18:04:35 2023, max compression
```

## Comparing `simcomm-0.1.0.tar` & `simcomm-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:49:32.615615 simcomm-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 10:49:22.000000 simcomm-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-02 10:49:32.615615 simcomm-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-02 10:49:22.000000 simcomm-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-02 10:49:22.000000 simcomm-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-02 10:49:32.615615 simcomm-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-02 10:49:22.000000 simcomm-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:49:32.611615 simcomm-0.1.0/simcomm/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:49:32.611615 simcomm-0.1.0/simcomm/core/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:49:32.611615 simcomm-0.1.0/simcomm/core/fading/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/fading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/fading/rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/fading/rician.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:49:32.615615 simcomm-0.1.0/simcomm/core/propagation/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/propagation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/propagation/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/propagation/pathloss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:49:32.615615 simcomm-0.1.0/simcomm/core/system/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/system/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/system/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/system/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/system/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/system/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/core/system/transmitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:49:32.615615 simcomm-0.1.0/simcomm/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/metrics/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:49:32.615615 simcomm-0.1.0/simcomm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:49:32.615615 simcomm-0.1.0/simcomm/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-02 10:49:22.000000 simcomm-0.1.0/simcomm/visualize/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:49:32.611615 simcomm-0.1.0/simcomm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-02 10:49:32.000000 simcomm-0.1.0/simcomm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 10:49:32.000000 simcomm-0.1.0/simcomm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 10:49:32.000000 simcomm-0.1.0/simcomm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 10:49:32.000000 simcomm-0.1.0/simcomm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:49:32.615615 simcomm-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-02 10:49:22.000000 simcomm-0.1.0/tests/test_fading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-02 10:49:22.000000 simcomm-0.1.0/tests/test_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-02 10:49:22.000000 simcomm-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:04:35.159537 simcomm-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 18:04:23.000000 simcomm-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-08-02 18:04:35.159537 simcomm-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-08-02 18:04:23.000000 simcomm-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-02 18:04:23.000000 simcomm-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-02 18:04:35.159537 simcomm-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-02 18:04:23.000000 simcomm-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:04:35.155537 simcomm-0.1.1/simcomm/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:04:35.155537 simcomm-0.1.1/simcomm/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:04:35.155537 simcomm-0.1.1/simcomm/core/fading/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/fading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/fading/rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/fading/rician.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:04:35.155537 simcomm-0.1.1/simcomm/core/propagation/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/propagation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/propagation/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/propagation/pathloss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:04:35.159537 simcomm-0.1.1/simcomm/core/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/system/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/system/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/system/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/system/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/system/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/core/system/transmitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:04:35.159537 simcomm-0.1.1/simcomm/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/metrics/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:04:35.159537 simcomm-0.1.1/simcomm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:04:35.159537 simcomm-0.1.1/simcomm/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-02 18:04:23.000000 simcomm-0.1.1/simcomm/visualize/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:04:35.155537 simcomm-0.1.1/simcomm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-08-02 18:04:35.000000 simcomm-0.1.1/simcomm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 18:04:35.000000 simcomm-0.1.1/simcomm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:04:35.000000 simcomm-0.1.1/simcomm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 18:04:35.000000 simcomm-0.1.1/simcomm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:04:35.159537 simcomm-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-02 18:04:23.000000 simcomm-0.1.1/tests/test_fading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-02 18:04:23.000000 simcomm-0.1.1/tests/test_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-02 18:04:23.000000 simcomm-0.1.1/tests/test_utils.py
```

### Comparing `simcomm-0.1.0/LICENSE` & `simcomm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/setup.py` & `simcomm-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/core/fading/__init__.py` & `simcomm-0.1.1/simcomm/core/fading/__init__.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/core/fading/rayleigh.py` & `simcomm-0.1.1/simcomm/core/fading/rayleigh.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/core/fading/rician.py` & `simcomm-0.1.1/simcomm/core/fading/rician.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/core/propagation/noise.py` & `simcomm-0.1.1/simcomm/core/propagation/noise.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/core/propagation/pathloss.py` & `simcomm-0.1.1/simcomm/core/propagation/pathloss.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/core/system/channel.py` & `simcomm-0.1.1/simcomm/core/system/channel.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/core/system/link.py` & `simcomm-0.1.1/simcomm/core/system/link.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/core/system/receiver.py` & `simcomm-0.1.1/simcomm/core/system/receiver.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/core/system/star.py` & `simcomm-0.1.1/simcomm/core/system/star.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/core/system/system.py` & `simcomm-0.1.1/simcomm/core/system/system.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/core/system/transmitter.py` & `simcomm-0.1.1/simcomm/core/system/transmitter.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/metrics/common.py` & `simcomm-0.1.1/simcomm/metrics/common.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/utils/utils.py` & `simcomm-0.1.1/simcomm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm/visualize/layout.py` & `simcomm-0.1.1/simcomm/visualize/layout.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/simcomm.egg-info/SOURCES.txt` & `simcomm-0.1.1/simcomm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/tests/test_fading.py` & `simcomm-0.1.1/tests/test_fading.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/tests/test_propagation.py` & `simcomm-0.1.1/tests/test_propagation.py`

 * *Files identical despite different names*

### Comparing `simcomm-0.1.0/tests/test_utils.py` & `simcomm-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

