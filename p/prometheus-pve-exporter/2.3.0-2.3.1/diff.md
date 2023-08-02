# Comparing `tmp/prometheus-pve-exporter-2.3.0.tar.gz` & `tmp/prometheus-pve-exporter-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus-pve-exporter-2.3.0.tar", last modified: Wed Apr 26 12:22:08 2023, max compression
+gzip compressed data, was "prometheus-pve-exporter-2.3.1.tar", last modified: Wed Aug  2 17:18:17 2023, max compression
```

## Comparing `prometheus-pve-exporter-2.3.0.tar` & `prometheus-pve-exporter-2.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:22:08.393193 prometheus-pve-exporter-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-04-26 12:22:08.393193 prometheus-pve-exporter-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 12:22:08.397193 prometheus-pve-exporter-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:22:08.389193 prometheus-pve-exporter-2.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:22:08.393193 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-04-26 12:22:08.000000 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-26 12:22:08.000000 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:22:08.000000 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 12:22:08.000000 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 12:22:08.000000 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 12:22:08.000000 prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:22:08.393193 prometheus-pve-exporter-2.3.0/src/pve_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/src/pve_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/src/pve_exporter/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4641 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/src/pve_exporter/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/src/pve_exporter/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/src/pve_exporter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-26 12:21:55.000000 prometheus-pve-exporter-2.3.0/src/pve_exporter/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:18:17.224260 prometheus-pve-exporter-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 17:18:05.000000 prometheus-pve-exporter-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-08-02 17:18:17.224260 prometheus-pve-exporter-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-08-02 17:18:05.000000 prometheus-pve-exporter-2.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:18:17.224260 prometheus-pve-exporter-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-02 17:18:05.000000 prometheus-pve-exporter-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:18:17.220260 prometheus-pve-exporter-2.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:18:17.224260 prometheus-pve-exporter-2.3.1/src/prometheus_pve_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-08-02 17:18:17.000000 prometheus-pve-exporter-2.3.1/src/prometheus_pve_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-02 17:18:17.000000 prometheus-pve-exporter-2.3.1/src/prometheus_pve_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:18:17.000000 prometheus-pve-exporter-2.3.1/src/prometheus_pve_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 17:18:17.000000 prometheus-pve-exporter-2.3.1/src/prometheus_pve_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 17:18:17.000000 prometheus-pve-exporter-2.3.1/src/prometheus_pve_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 17:18:17.000000 prometheus-pve-exporter-2.3.1/src/prometheus_pve_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:18:17.224260 prometheus-pve-exporter-2.3.1/src/pve_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:18:05.000000 prometheus-pve-exporter-2.3.1/src/pve_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-02 17:18:05.000000 prometheus-pve-exporter-2.3.1/src/pve_exporter/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4641 2023-08-02 17:18:05.000000 prometheus-pve-exporter-2.3.1/src/pve_exporter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-08-02 17:18:05.000000 prometheus-pve-exporter-2.3.1/src/pve_exporter/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-08-02 17:18:05.000000 prometheus-pve-exporter-2.3.1/src/pve_exporter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-08-02 17:18:05.000000 prometheus-pve-exporter-2.3.1/src/pve_exporter/http.py
```

### Comparing `prometheus-pve-exporter-2.3.0/LICENSE` & `prometheus-pve-exporter-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-2.3.0/PKG-INFO` & `prometheus-pve-exporter-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 2.3.0
+Version: 2.3.1
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Home-page: https://github.com/prometheus-pve/prometheus-pve-exporter
 Author: Lorenz Schori
 Author-email: lo@znerol.ch
 License: Apache Software License 2.0
 Keywords: prometheus exporter network monitoring proxmox
 Platform: UNKNOWN
```

### Comparing `prometheus-pve-exporter-2.3.0/README.rst` & `prometheus-pve-exporter-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-2.3.0/setup.py` & `prometheus-pve-exporter-2.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="prometheus-pve-exporter",
-    version="2.3.0",
+    version="2.3.1",
     author="Lorenz Schori",
     author_email="lo@znerol.ch",
     description=("Proxmox VE exporter for the Prometheus monitoring system."),
     long_description=open('README.rst').read(),
     license="Apache Software License 2.0",
     keywords="prometheus exporter network monitoring proxmox",
     url="https://github.com/prometheus-pve/prometheus-pve-exporter",
```

### Comparing `prometheus-pve-exporter-2.3.0/src/prometheus_pve_exporter.egg-info/PKG-INFO` & `prometheus-pve-exporter-2.3.1/src/prometheus_pve_exporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 2.3.0
+Version: 2.3.1
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Home-page: https://github.com/prometheus-pve/prometheus-pve-exporter
 Author: Lorenz Schori
 Author-email: lo@znerol.ch
 License: Apache Software License 2.0
 Keywords: prometheus exporter network monitoring proxmox
 Platform: UNKNOWN
```

### Comparing `prometheus-pve-exporter-2.3.0/src/pve_exporter/cli.py` & `prometheus-pve-exporter-2.3.1/src/pve_exporter/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-2.3.0/src/pve_exporter/collector.py` & `prometheus-pve-exporter-2.3.1/src/pve_exporter/collector.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-2.3.0/src/pve_exporter/config.py` & `prometheus-pve-exporter-2.3.1/src/pve_exporter/config.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-2.3.0/src/pve_exporter/http.py` & `prometheus-pve-exporter-2.3.1/src/pve_exporter/http.py`

 * *Files identical despite different names*

