# Comparing `tmp/emcstream-0.1.tar.gz` & `tmp/emcstream-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emcstream-0.1.tar", last modified: Sun Jul 30 11:48:35 2023, max compression
+gzip compressed data, was "emcstream-0.2.tar", last modified: Wed Aug  2 19:08:57 2023, max compression
```

## Comparing `emcstream-0.1.tar` & `emcstream-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-07-30 11:48:35.923260 emcstream-0.1/
--rw-rw-r--   0 leyla     (1000) leyla     (1000)     1076 2023-07-30 11:31:21.000000 emcstream-0.1/LICENSE
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       26 2023-07-30 11:26:24.000000 emcstream-0.1/MANIFEST.in
--rw-rw-r--   0 leyla     (1000) leyla     (1000)      340 2023-07-30 11:48:35.923260 emcstream-0.1/PKG-INFO
--rw-rw-r--   0 leyla     (1000) leyla     (1000)     8175 2023-07-30 11:37:20.000000 emcstream-0.1/README.md
-drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-07-30 11:48:35.923260 emcstream-0.1/emcstream.egg-info/
--rw-rw-r--   0 leyla     (1000) leyla     (1000)      340 2023-07-30 11:48:35.000000 emcstream-0.1/emcstream.egg-info/PKG-INFO
--rw-rw-r--   0 leyla     (1000) leyla     (1000)      219 2023-07-30 11:48:35.000000 emcstream-0.1/emcstream.egg-info/SOURCES.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)        1 2023-07-30 11:48:35.000000 emcstream-0.1/emcstream.egg-info/dependency_links.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       56 2023-07-30 11:48:35.000000 emcstream-0.1/emcstream.egg-info/requires.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)        1 2023-07-30 11:48:35.000000 emcstream-0.1/emcstream.egg-info/top_level.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       58 2023-07-30 11:29:22.000000 emcstream-0.1/requirements.txt
--rw-rw-r--   0 leyla     (1000) leyla     (1000)       38 2023-07-30 11:48:35.923260 emcstream-0.1/setup.cfg
--rw-rw-r--   0 leyla     (1000) leyla     (1000)      520 2023-07-30 11:45:29.000000 emcstream-0.1/setup.py
+drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 19:08:57.573519 emcstream-0.2/
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)     1076 2023-07-30 11:31:21.000000 emcstream-0.2/LICENSE
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       26 2023-07-30 11:26:24.000000 emcstream-0.2/MANIFEST.in
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)      340 2023-08-02 19:08:57.573519 emcstream-0.2/PKG-INFO
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)     8175 2023-07-30 11:37:20.000000 emcstream-0.2/README.md
+drwxrwxr-x   0 leyla     (1000) leyla     (1000)        0 2023-08-02 19:08:57.573519 emcstream-0.2/emcstream.egg-info/
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)      340 2023-08-02 19:08:57.000000 emcstream-0.2/emcstream.egg-info/PKG-INFO
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)      219 2023-08-02 19:08:57.000000 emcstream-0.2/emcstream.egg-info/SOURCES.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)        1 2023-08-02 19:08:57.000000 emcstream-0.2/emcstream.egg-info/dependency_links.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       61 2023-08-02 19:08:57.000000 emcstream-0.2/emcstream.egg-info/requires.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)        1 2023-08-02 19:08:57.000000 emcstream-0.2/emcstream.egg-info/top_level.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       58 2023-07-30 11:29:22.000000 emcstream-0.2/requirements.txt
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)       38 2023-08-02 19:08:57.573519 emcstream-0.2/setup.cfg
+-rw-rw-r--   0 leyla     (1000) leyla     (1000)      525 2023-08-02 19:08:40.000000 emcstream-0.2/setup.py
```

### Comparing `emcstream-0.1/LICENSE` & `emcstream-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emcstream-0.1/README.md` & `emcstream-0.2/README.md`

 * *Files identical despite different names*

### Comparing `emcstream-0.1/setup.py` & `emcstream-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='emcstream',
-    version='0.1',
+    version='0.2',
     url='https://gitlab.com/alaettinzubaroglu/emcstream',
     author='Alaettin Zubaroğlu',
     author_email='alaettinzubaroglu@gmail.com',
     description='A python implementation for online embedding and clustering of evolving data streams',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scikit-learn',
         'umap-learn',
-        'sklearn',
+        'scikit-learn',
         'statistics',
         'pandas'
     ],
 )
```

