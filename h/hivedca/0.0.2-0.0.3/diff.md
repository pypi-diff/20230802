# Comparing `tmp/hivedca-0.0.2.tar.gz` & `tmp/hivedca-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivedca-0.0.2.tar", last modified: Wed Aug  2 05:02:35 2023, max compression
+gzip compressed data, was "hivedca-0.0.3.tar", last modified: Wed Aug  2 05:07:51 2023, max compression
```

## Comparing `hivedca-0.0.2.tar` & `hivedca-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 05:02:35.477664 hivedca-0.0.2/
--rw-rw-rw-   0        0        0      410 2023-08-02 05:02:35.475593 hivedca-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-02 04:45:04.000000 hivedca-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 05:02:35.432210 hivedca-0.0.2/dca/
--rw-rw-rw-   0        0        0        0 2023-08-02 04:55:56.000000 hivedca-0.0.2/dca/__init__.py
--rw-rw-rw-   0        0        0     3271 2023-07-21 00:45:49.000000 hivedca-0.0.2/dca/backbones.py
--rw-rw-rw-   0        0        0    13406 2023-07-21 00:45:49.000000 hivedca-0.0.2/dca/common.py
--rw-rw-rw-   0        0        0    12145 2023-07-28 06:34:18.000000 hivedca-0.0.2/dca/dataloader.py
--rw-rw-rw-   0        0        0     2800 2023-07-21 00:47:02.000000 hivedca-0.0.2/dca/metrics.py
--rw-rw-rw-   0        0        0     2032 2023-08-02 04:35:34.000000 hivedca-0.0.2/dca/patch_core.py
--rw-rw-rw-   0        0        0    11776 2023-08-02 04:33:04.000000 hivedca-0.0.2/dca/patchcore.py
--rw-rw-rw-   0        0        0     7326 2023-07-28 00:59:22.000000 hivedca-0.0.2/dca/sampler.py
--rw-rw-rw-   0        0        0     2214 2023-08-02 04:30:12.000000 hivedca-0.0.2/dca/training.py
--rw-rw-rw-   0        0        0     5653 2023-07-27 23:56:32.000000 hivedca-0.0.2/dca/training_backup.py
--rw-rw-rw-   0        0        0     3968 2023-07-28 02:28:37.000000 hivedca-0.0.2/dca/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 05:02:35.469949 hivedca-0.0.2/hivedca.egg-info/
--rw-rw-rw-   0        0        0      410 2023-08-02 05:02:35.000000 hivedca-0.0.2/hivedca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-08-02 05:02:35.000000 hivedca-0.0.2/hivedca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 05:02:35.000000 hivedca-0.0.2/hivedca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-08-02 05:02:35.000000 hivedca-0.0.2/hivedca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 05:02:35.478650 hivedca-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-08-02 05:02:25.000000 hivedca-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:07:51.057479 hivedca-0.0.3/
+-rw-rw-rw-   0        0        0      410 2023-08-02 05:07:51.053427 hivedca-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-02 04:45:04.000000 hivedca-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 05:07:51.037318 hivedca-0.0.3/dca/
+-rw-rw-rw-   0        0        0      495 2023-08-02 05:07:11.000000 hivedca-0.0.3/dca/__init__.py
+-rw-rw-rw-   0        0        0     3271 2023-07-21 00:45:49.000000 hivedca-0.0.3/dca/backbones.py
+-rw-rw-rw-   0        0        0    13406 2023-07-21 00:45:49.000000 hivedca-0.0.3/dca/common.py
+-rw-rw-rw-   0        0        0    12145 2023-07-28 06:34:18.000000 hivedca-0.0.3/dca/dataloader.py
+-rw-rw-rw-   0        0        0     2800 2023-07-21 00:47:02.000000 hivedca-0.0.3/dca/metrics.py
+-rw-rw-rw-   0        0        0     2032 2023-08-02 04:35:34.000000 hivedca-0.0.3/dca/patch_core.py
+-rw-rw-rw-   0        0        0    11776 2023-08-02 04:33:04.000000 hivedca-0.0.3/dca/patchcore.py
+-rw-rw-rw-   0        0        0     7326 2023-07-28 00:59:22.000000 hivedca-0.0.3/dca/sampler.py
+-rw-rw-rw-   0        0        0     2214 2023-08-02 04:30:12.000000 hivedca-0.0.3/dca/training.py
+-rw-rw-rw-   0        0        0     5653 2023-07-27 23:56:32.000000 hivedca-0.0.3/dca/training_backup.py
+-rw-rw-rw-   0        0        0     3968 2023-07-28 02:28:37.000000 hivedca-0.0.3/dca/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:07:51.050407 hivedca-0.0.3/hivedca.egg-info/
+-rw-rw-rw-   0        0        0      410 2023-08-02 05:07:50.000000 hivedca-0.0.3/hivedca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-08-02 05:07:50.000000 hivedca-0.0.3/hivedca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 05:07:50.000000 hivedca-0.0.3/hivedca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-08-02 05:07:50.000000 hivedca-0.0.3/hivedca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 05:07:51.057479 hivedca-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-08-02 05:07:14.000000 hivedca-0.0.3/setup.py
```

### Comparing `hivedca-0.0.2/dca/backbones.py` & `hivedca-0.0.3/dca/backbones.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.2/dca/common.py` & `hivedca-0.0.3/dca/common.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.2/dca/dataloader.py` & `hivedca-0.0.3/dca/dataloader.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.2/dca/metrics.py` & `hivedca-0.0.3/dca/metrics.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.2/dca/patch_core.py` & `hivedca-0.0.3/dca/patch_core.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.2/dca/patchcore.py` & `hivedca-0.0.3/dca/patchcore.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.2/dca/sampler.py` & `hivedca-0.0.3/dca/sampler.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.2/dca/training.py` & `hivedca-0.0.3/dca/training.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.2/dca/training_backup.py` & `hivedca-0.0.3/dca/training_backup.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.2/dca/utils.py` & `hivedca-0.0.3/dca/utils.py`

 * *Files identical despite different names*

### Comparing `hivedca-0.0.2/setup.py` & `hivedca-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hivedca", # Replace with your own username
-    version="0.0.2",
+    version="0.0.3",
     author="Example Author",
     author_email="author@example.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

