# Comparing `tmp/passwordless-sdk-0.0.1.tar.gz` & `tmp/passwordless-SDK-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwordless-sdk-0.0.1.tar", last modified: Tue Aug  1 22:29:46 2023, max compression
+gzip compressed data, was "passwordless-SDK-0.0.2.tar", last modified: Tue Aug  1 22:44:24 2023, max compression
```

## Comparing `passwordless-sdk-0.0.1.tar` & `passwordless-SDK-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 22:29:46.409653 passwordless-sdk-0.0.1/
--rw-rw-rw-   0        0        0      482 2023-08-01 22:29:46.409147 passwordless-sdk-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 22:29:46.408629 passwordless-sdk-0.0.1/passwordless_sdk.egg-info/
--rw-rw-rw-   0        0        0      482 2023-08-01 22:29:46.000000 passwordless-sdk-0.0.1/passwordless_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-08-01 22:29:46.000000 passwordless-sdk-0.0.1/passwordless_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 22:29:46.000000 passwordless-sdk-0.0.1/passwordless_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-08-01 22:29:46.000000 passwordless-sdk-0.0.1/passwordless_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 22:29:46.409653 passwordless-sdk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      594 2023-08-01 22:29:23.000000 passwordless-sdk-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:44:24.468047 passwordless-SDK-0.0.2/
+-rw-rw-rw-   0        0        0      482 2023-08-01 22:44:24.467541 passwordless-SDK-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 22:44:24.466508 passwordless-SDK-0.0.2/passwordless_SDK.egg-info/
+-rw-rw-rw-   0        0        0      482 2023-08-01 22:44:24.000000 passwordless-SDK-0.0.2/passwordless_SDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-08-01 22:44:24.000000 passwordless-SDK-0.0.2/passwordless_SDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 22:44:24.000000 passwordless-SDK-0.0.2/passwordless_SDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 22:44:24.000000 passwordless-SDK-0.0.2/passwordless_SDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 22:44:24.468047 passwordless-SDK-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      594 2023-08-01 22:44:20.000000 passwordless-SDK-0.0.2/setup.py
```

### Comparing `passwordless-sdk-0.0.1/setup.py` & `passwordless-SDK-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 setup(
-    name='passwordless-sdk',
-    version='0.0.1',
+    name='passwordless-SDK',
+    version='0.0.2',
     description='A placeholder for my future project.',
     author='Matthew Fiallos',
     author_email='matthew.fiallos@randstadusa.com',
     url='https://github.com/yourusername/my_project',
-    packages=['passwordless-sdk'],
+    packages=['passwordless-SDK'],
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
     ],
```

