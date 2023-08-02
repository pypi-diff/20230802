# Comparing `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1.tar.gz` & `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1.tar", last modified: Tue Aug  1 18:28:11 2023, max compression
+gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2.tar", last modified: Wed Aug  2 18:28:12 2023, max compression
```

## Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1.tar` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:28:11.902136 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-01 18:28:00.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 18:28:00.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-01 18:28:11.902136 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-01 18:28:00.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-01 18:28:00.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:28:11.902136 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-01 18:28:00.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:28:11.898136 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:28:11.898136 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:28:11.902136 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-08-01 18:28:00.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:28:11.902136 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-01 18:28:00.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20779 2023-08-01 18:28:00.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.7.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:28:00.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:28:11.902136 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-01 18:28:11.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-01 18:28:11.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:28:11.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 18:28:11.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 18:28:11.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:12.809539 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 18:27:58.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 18:27:58.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-02 18:28:12.809539 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-02 18:27:58.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 18:27:58.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:28:12.809539 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-02 18:27:58.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:12.805539 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:12.805539 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:12.805539 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-08-02 18:27:58.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:12.809539 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 18:27:58.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20780 2023-08-02 18:27:58.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.7.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:27:58.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:12.805539 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-02 18:28:12.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-02 18:28:12.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:28:12.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 18:28:12.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 18:28:12.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/LICENSE` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 0.7.1
+Version: 0.7.2
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/README.md` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/setup.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-frontend-web-app-cloudfront-distribution",
-    "version": "0.7.1",
+    "version": "0.7.2",
     "description": "AWS CloudFront distribution for frontend web app (spa) optimized.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution",
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii": [
-            "aws-secure-frontend-web-app-cloudfront-distribution@0.7.1.jsii.tgz"
+            "aws-secure-frontend-web-app-cloudfront-distribution@0.7.2.jsii.tgz"
         ],
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.43.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.85.0, <2.0.0",
+        "jsii>=1.86.1, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 0.7.1
+Version: 0.7.2
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.1/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.2/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
-src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.7.1.jsii.tgz
+src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.7.2.jsii.tgz
```
