# Comparing `tmp/sdk_test_sdk-1.0.0.tar.gz` & `tmp/sdk_test_sdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdk_test_sdk-1.0.0.tar", last modified: Wed Aug  2 07:17:05 2023, max compression
+gzip compressed data, was "sdk_test_sdk-2.0.0.tar", last modified: Wed Aug  2 08:08:21 2023, max compression
```

## Comparing `sdk_test_sdk-1.0.0.tar` & `sdk_test_sdk-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhuwankang   (501) staff       (20)        0 2023-08-02 07:17:05.190354 sdk_test_sdk-1.0.0/
--rw-r--r--   0 zhuwankang   (501) staff       (20)     1310 2023-08-02 07:06:04.000000 sdk_test_sdk-1.0.0/LICENSE.txt
--rw-r--r--   0 zhuwankang   (501) staff       (20)      763 2023-08-02 07:17:05.190210 sdk_test_sdk-1.0.0/PKG-INFO
--rw-r--r--   0 zhuwankang   (501) staff       (20)      273 2023-08-02 07:07:05.000000 sdk_test_sdk-1.0.0/README.md
-drwxr-xr-x   0 zhuwankang   (501) staff       (20)        0 2023-08-02 07:17:05.189429 sdk_test_sdk-1.0.0/sdk_test_sdk/
--rw-r--r--   0 zhuwankang   (501) staff       (20)       76 2023-08-02 07:06:04.000000 sdk_test_sdk-1.0.0/sdk_test_sdk/__init__.py
--rw-r--r--   0 zhuwankang   (501) staff       (20)      172 2023-08-02 07:06:04.000000 sdk_test_sdk-1.0.0/sdk_test_sdk/core.py
-drwxr-xr-x   0 zhuwankang   (501) staff       (20)        0 2023-08-02 07:17:05.190047 sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/
--rw-r--r--   0 zhuwankang   (501) staff       (20)      763 2023-08-02 07:17:05.000000 sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/PKG-INFO
--rw-r--r--   0 zhuwankang   (501) staff       (20)      255 2023-08-02 07:17:05.000000 sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 zhuwankang   (501) staff       (20)        1 2023-08-02 07:17:05.000000 sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 zhuwankang   (501) staff       (20)       14 2023-08-02 07:17:05.000000 sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/requires.txt
--rw-r--r--   0 zhuwankang   (501) staff       (20)       13 2023-08-02 07:17:05.000000 sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/top_level.txt
--rw-r--r--   0 zhuwankang   (501) staff       (20)       38 2023-08-02 07:17:05.190396 sdk_test_sdk-1.0.0/setup.cfg
--rw-r--r--   0 zhuwankang   (501) staff       (20)     3784 2023-08-02 07:16:57.000000 sdk_test_sdk-1.0.0/setup.py
+drwxr-xr-x   0 zhuwankang   (501) staff       (20)        0 2023-08-02 08:08:21.774808 sdk_test_sdk-2.0.0/
+-rw-r--r--   0 zhuwankang   (501) staff       (20)     1310 2023-08-02 07:06:04.000000 sdk_test_sdk-2.0.0/LICENSE.txt
+-rw-r--r--   0 zhuwankang   (501) staff       (20)      772 2023-08-02 08:08:21.774686 sdk_test_sdk-2.0.0/PKG-INFO
+-rw-r--r--   0 zhuwankang   (501) staff       (20)      282 2023-08-02 07:17:35.000000 sdk_test_sdk-2.0.0/README.md
+drwxr-xr-x   0 zhuwankang   (501) staff       (20)        0 2023-08-02 08:08:21.774003 sdk_test_sdk-2.0.0/sdk_test_sdk/
+-rw-r--r--   0 zhuwankang   (501) staff       (20)       89 2023-08-02 08:08:13.000000 sdk_test_sdk-2.0.0/sdk_test_sdk/__init__.py
+-rw-r--r--   0 zhuwankang   (501) staff       (20)      219 2023-08-02 08:08:13.000000 sdk_test_sdk-2.0.0/sdk_test_sdk/core.py
+drwxr-xr-x   0 zhuwankang   (501) staff       (20)        0 2023-08-02 08:08:21.774522 sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/
+-rw-r--r--   0 zhuwankang   (501) staff       (20)      772 2023-08-02 08:08:21.000000 sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 zhuwankang   (501) staff       (20)      255 2023-08-02 08:08:21.000000 sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuwankang   (501) staff       (20)        1 2023-08-02 08:08:21.000000 sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuwankang   (501) staff       (20)       14 2023-08-02 08:08:21.000000 sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/requires.txt
+-rw-r--r--   0 zhuwankang   (501) staff       (20)       13 2023-08-02 08:08:21.000000 sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/top_level.txt
+-rw-r--r--   0 zhuwankang   (501) staff       (20)       38 2023-08-02 08:08:21.774864 sdk_test_sdk-2.0.0/setup.cfg
+-rw-r--r--   0 zhuwankang   (501) staff       (20)     3813 2023-08-02 07:57:38.000000 sdk_test_sdk-2.0.0/setup.py
```

### Comparing `sdk_test_sdk-1.0.0/LICENSE.txt` & `sdk_test_sdk-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sdk_test_sdk-1.0.0/PKG-INFO` & `sdk_test_sdk-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdk_test_sdk
-Version: 1.0.0
+Version: 2.0.0
 Summary: An awesome SDK to say hello!
 Home-page: https://github.com/your/repo
 Author: Your Name
 Author-email: your@email.com
 License: MIT
 Keywords: python sample project example
 Platform: UNKNOWN
@@ -14,39 +14,19 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # 添加关于SDK的说明和用法等信息，文件主要是用来对此次发行的包的详细说明，包括用法和注意事项等
 
 
+# 安装
+pip install sdk_test_sdk-1.0.0-py3-none-any.whl
+
+
 # 使用
 import sdk_test_sdk
 
 
 sdk_test_sdk.test_numpy()
 sdk_test_sdk.test_hello()
 
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-# 安装
-pip install my_sdk
-
-
-
-
```

### Comparing `sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/PKG-INFO` & `sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdk-test-sdk
-Version: 1.0.0
+Version: 2.0.0
 Summary: An awesome SDK to say hello!
 Home-page: https://github.com/your/repo
 Author: Your Name
 Author-email: your@email.com
 License: MIT
 Keywords: python sample project example
 Platform: UNKNOWN
@@ -14,39 +14,19 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # 添加关于SDK的说明和用法等信息，文件主要是用来对此次发行的包的详细说明，包括用法和注意事项等
 
 
+# 安装
+pip install sdk_test_sdk-1.0.0-py3-none-any.whl
+
+
 # 使用
 import sdk_test_sdk
 
 
 sdk_test_sdk.test_numpy()
 sdk_test_sdk.test_hello()
 
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-# 安装
-pip install my_sdk
-
-
-
-
```

### Comparing `sdk_test_sdk-1.0.0/setup.py` & `sdk_test_sdk-2.0.0/setup.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-# 指定SDK的打包信息，为打包做准备的设置文件, 约定此次分发的包的版本号、名称、作者、联系方式、项目地址、python版本要求等信息
+# 指定SDK的打包信息，为打包做准备的设置文件, 约定此次分发的包的版本号、名称、作者、联系方式、项目地址、python版本要求等信息
```
