# Comparing `tmp/gs_xcom_backend_triggerer-0.0.4.tar.gz` & `tmp/gs_xcom_backend_triggerer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs_xcom_backend_triggerer-0.0.4.tar", last modified: Wed Aug  2 11:54:55 2023, max compression
+gzip compressed data, was "gs_xcom_backend_triggerer-0.0.5.tar", last modified: Wed Aug  2 12:11:28 2023, max compression
```

## Comparing `gs_xcom_backend_triggerer-0.0.4.tar` & `gs_xcom_backend_triggerer-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 11:54:55.152614 gs_xcom_backend_triggerer-0.0.4/
--rw-rw-rw-   0        0        0      536 2023-08-02 11:54:55.151614 gs_xcom_backend_triggerer-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 11:54:55.128643 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend/
--rw-rw-rw-   0        0        0        0 2023-08-01 04:44:48.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend/__init__.py
--rw-rw-rw-   0        0        0     3653 2023-08-02 11:49:05.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend/deferrer.py
--rw-rw-rw-   0        0        0     1289 2023-08-01 05:25:23.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend/triggerer.py
-drwxrwxrwx   0        0        0        0 2023-08-02 11:54:55.149439 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend_triggerer.egg-info/
--rw-rw-rw-   0        0        0      536 2023-08-02 11:54:54.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend_triggerer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-08-02 11:54:55.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend_triggerer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 11:54:54.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend_triggerer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-02 11:54:54.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend_triggerer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 11:54:55.153609 gs_xcom_backend_triggerer-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-08-02 11:54:46.000000 gs_xcom_backend_triggerer-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:11:28.320174 gs_xcom_backend_triggerer-0.0.5/
+-rw-rw-rw-   0        0        0      536 2023-08-02 12:11:28.318176 gs_xcom_backend_triggerer-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 12:11:28.293592 gs_xcom_backend_triggerer-0.0.5/gs_xcom_backend/
+-rw-rw-rw-   0        0        0        0 2023-08-01 04:44:48.000000 gs_xcom_backend_triggerer-0.0.5/gs_xcom_backend/__init__.py
+-rw-rw-rw-   0        0        0     3648 2023-08-02 12:07:37.000000 gs_xcom_backend_triggerer-0.0.5/gs_xcom_backend/deferrer.py
+-rw-rw-rw-   0        0        0     1289 2023-08-01 05:25:23.000000 gs_xcom_backend_triggerer-0.0.5/gs_xcom_backend/triggerer.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:11:28.312174 gs_xcom_backend_triggerer-0.0.5/gs_xcom_backend_triggerer.egg-info/
+-rw-rw-rw-   0        0        0      536 2023-08-02 12:11:28.000000 gs_xcom_backend_triggerer-0.0.5/gs_xcom_backend_triggerer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-08-02 12:11:28.000000 gs_xcom_backend_triggerer-0.0.5/gs_xcom_backend_triggerer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 12:11:28.000000 gs_xcom_backend_triggerer-0.0.5/gs_xcom_backend_triggerer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-02 12:11:28.000000 gs_xcom_backend_triggerer-0.0.5/gs_xcom_backend_triggerer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 12:11:28.320174 gs_xcom_backend_triggerer-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      841 2023-08-02 12:10:57.000000 gs_xcom_backend_triggerer-0.0.5/setup.py
```

### Comparing `gs_xcom_backend_triggerer-0.0.4/PKG-INFO` & `gs_xcom_backend_triggerer-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs_xcom_backend_triggerer
-Version: 0.0.4
+Version: 0.0.5
 Summary: triggerer gs_xcom_backend module file
 Author: imvj202
 Author-email: imvj202@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend/deferrer.py` & `gs_xcom_backend_triggerer-0.0.5/gs_xcom_backend/deferrer.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.kwargs = kwargs
         self.log.info(f"args: {args}")
         self.log.info(f"kwargs: {kwargs}")
         super().__init__(*args, **kwargs)
 
     def serialize(self) -> Dict[str, Any]:
         return (
-            "herald.reimage.defer_operator.ReImageTrigger",
+            "gs_xcom_backend.deferrer.ReImageTrigger",
             {
                 "job_id": self.job_id,
                 "xcom_task_id": self.xcom_task_id,
                 "moment": self.moment,
                 "attempt": self.attempt,
                 "hosts_info": self.hosts_info,
                 "failed_hosts_info": self.failed_hosts_info,
```

### Comparing `gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend/triggerer.py` & `gs_xcom_backend_triggerer-0.0.5/gs_xcom_backend/triggerer.py`

 * *Files identical despite different names*

### Comparing `gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend_triggerer.egg-info/PKG-INFO` & `gs_xcom_backend_triggerer-0.0.5/gs_xcom_backend_triggerer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-xcom-backend-triggerer
-Version: 0.0.4
+Version: 0.0.5
 Summary: triggerer gs_xcom_backend module file
 Author: imvj202
 Author-email: imvj202@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `gs_xcom_backend_triggerer-0.0.4/setup.py` & `gs_xcom_backend_triggerer-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'triggerer gs_xcom_backend module file'
 LONG_DESCRIPTION = 'triggerer gs_xcom_backend module file'
 
 # Setting up
 setup(
     name="gs_xcom_backend_triggerer",
     version=VERSION,
```

