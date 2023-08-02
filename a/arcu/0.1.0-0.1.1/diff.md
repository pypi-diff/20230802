# Comparing `tmp/arcu-0.1.0.tar.gz` & `tmp/arcu-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcu-0.1.0.tar", last modified: Fri Jul 28 20:13:57 2023, max compression
+gzip compressed data, was "arcu-0.1.1.tar", last modified: Wed Aug  2 15:59:47 2023, max compression
```

## Comparing `arcu-0.1.0.tar` & `arcu-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 20:13:57.443989 arcu-0.1.0/
--rw-rw-rw-   0        0        0     1071 2023-07-28 20:04:59.000000 arcu-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      957 2023-07-28 20:13:57.441988 arcu-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       72 2023-07-28 20:05:09.000000 arcu-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 20:13:57.438990 arcu-0.1.0/arcu.egg-info/
--rw-rw-rw-   0        0        0      957 2023-07-28 20:13:56.000000 arcu-0.1.0/arcu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2023-07-28 20:13:57.000000 arcu-0.1.0/arcu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 20:13:56.000000 arcu-0.1.0/arcu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-28 20:13:56.000000 arcu-0.1.0/arcu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 20:13:56.000000 arcu-0.1.0/arcu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 20:13:57.443989 arcu-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1176 2023-07-28 20:13:50.000000 arcu-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:59:47.319359 arcu-0.1.1/
+-rw-rw-rw-   0        0        0     3283 2023-08-02 15:59:47.319359 arcu-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1952 2023-07-31 19:57:35.000000 arcu-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 15:59:47.301470 arcu-0.1.1/arcu/
+-rw-rw-rw-   0        0        0     5304 2023-07-31 19:57:35.000000 arcu-0.1.1/arcu/arcu.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:59:47.316425 arcu-0.1.1/arcu.egg-info/
+-rw-rw-rw-   0        0        0     3283 2023-08-02 15:59:47.000000 arcu-0.1.1/arcu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-08-02 15:59:47.000000 arcu-0.1.1/arcu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 15:59:47.000000 arcu-0.1.1/arcu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-08-02 15:59:47.000000 arcu-0.1.1/arcu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-02 15:59:47.000000 arcu-0.1.1/arcu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 15:59:47.320356 arcu-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1199 2023-08-02 15:58:30.000000 arcu-0.1.1/setup.py
```

### Comparing `arcu-0.1.0/setup.py` & `arcu-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='arcu',
-    version='0.1.0',
+    packages=['arcu'],
+    version='0.1.1',
     description='Find representative subpopulations in single cell imaging data.',
     author='Harris Davis',
     author_email='harris.davis@outlook.com',
     url='https://github.com/harrismdavis/arcu',
     license='MIT',
     python_requires='>=3.6',
     long_description=long_description,
```

