# Comparing `tmp/airscript-0.0.5.tar.gz` & `tmp/airscript-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airscript-0.0.5.tar", last modified: Tue May 30 09:21:44 2023, max compression
+gzip compressed data, was "airscript-0.0.6.tar", last modified: Wed Aug  2 04:26:44 2023, max compression
```

## Comparing `airscript-0.0.5.tar` & `airscript-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.671075 airscript-0.0.5/
--rw-rw-rw-   0        0        0      431 2023-05-30 09:21:44.670077 airscript-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-30 06:39:59.000000 airscript-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.652050 airscript-0.0.5/airscript/
--rw-rw-rw-   0        0        0        0 2023-05-30 08:18:07.000000 airscript-0.0.5/airscript/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.663075 airscript-0.0.5/airscript/action/
--rw-rw-rw-   0        0        0      454 2023-05-30 08:07:48.000000 airscript-0.0.5/airscript/action/__init__.py
--rw-rw-rw-   0        0        0      266 2023-05-30 08:02:07.000000 airscript-0.0.5/airscript/action/gesture.py
--rw-rw-rw-   0        0        0     1376 2023-05-30 08:11:36.000000 airscript-0.0.5/airscript/action/key.py
--rw-rw-rw-   0        0        0     1272 2023-05-30 08:04:45.000000 airscript-0.0.5/airscript/action/path.py
--rw-rw-rw-   0        0        0      165 2023-05-30 06:31:48.000000 airscript-0.0.5/airscript/action/touch.py
--rw-rw-rw-   0        0        0      157 2023-05-30 09:11:25.000000 airscript-0.0.5/airscript/data.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.664074 airscript-0.0.5/airscript/graphics/
--rw-rw-rw-   0        0        0       85 2023-05-30 06:27:00.000000 airscript-0.0.5/airscript/graphics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.665074 airscript-0.0.5/airscript/intent/
--rw-rw-rw-   0        0        0      111 2023-05-30 09:15:39.000000 airscript-0.0.5/airscript/intent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.665074 airscript-0.0.5/airscript/screen/
--rw-rw-rw-   0        0        0     3960 2023-05-30 08:44:26.000000 airscript-0.0.5/airscript/screen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.666074 airscript-0.0.5/airscript/system/
--rw-rw-rw-   0        0        0      716 2023-05-30 09:21:23.000000 airscript-0.0.5/airscript/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.668075 airscript-0.0.5/airscript/ui/
--rw-rw-rw-   0        0        0      631 2023-05-30 09:03:49.000000 airscript-0.0.5/airscript/ui/__init__.py
--rw-rw-rw-   0        0        0      961 2023-05-30 09:03:44.000000 airscript-0.0.5/airscript/ui/dialog.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:21:44.657064 airscript-0.0.5/airscript.egg-info/
--rw-rw-rw-   0        0        0      431 2023-05-30 09:21:44.000000 airscript-0.0.5/airscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-05-30 09:21:44.000000 airscript-0.0.5/airscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 09:21:44.000000 airscript-0.0.5/airscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 09:21:44.000000 airscript-0.0.5/airscript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 09:21:44.671075 airscript-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      692 2023-05-30 09:21:23.000000 airscript-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.995959 airscript-0.0.6/
+-rw-rw-rw-   0        0        0      493 2023-08-02 04:26:43.993954 airscript-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2023-08-02 04:15:18.000000 airscript-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.961944 airscript-0.0.6/airscript/
+-rw-rw-rw-   0        0        0      138 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.976944 airscript-0.0.6/airscript/action/
+-rw-rw-rw-   0        0        0      798 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/action/__init__.py
+-rw-rw-rw-   0        0        0      258 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/action/gesture.py
+-rw-rw-rw-   0        0        0     1376 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/action/key.py
+-rw-rw-rw-   0        0        0     1272 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/action/path.py
+-rw-rw-rw-   0        0        0      165 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/action/touch.py
+-rw-rw-rw-   0        0        0      195 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/data.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.978953 airscript-0.0.6/airscript/graphics/
+-rw-rw-rw-   0        0        0       85 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/graphics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.980946 airscript-0.0.6/airscript/intent/
+-rw-rw-rw-   0        0        0      111 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/intent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.982944 airscript-0.0.6/airscript/node/
+-rw-rw-rw-   0        0        0     4575 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/node/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.983944 airscript-0.0.6/airscript/screen/
+-rw-rw-rw-   0        0        0     3960 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/screen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.984947 airscript-0.0.6/airscript/system/
+-rw-rw-rw-   0        0        0      716 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.989953 airscript-0.0.6/airscript/ui/
+-rw-rw-rw-   0        0        0      631 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/ui/__init__.py
+-rw-rw-rw-   0        0        0      961 2023-08-02 04:15:18.000000 airscript-0.0.6/airscript/ui/dialog.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:26:43.968945 airscript-0.0.6/airscript.egg-info/
+-rw-rw-rw-   0        0        0      493 2023-08-02 04:26:43.000000 airscript-0.0.6/airscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-08-02 04:26:43.000000 airscript-0.0.6/airscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 04:26:43.000000 airscript-0.0.6/airscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-02 04:26:43.000000 airscript-0.0.6/airscript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 04:26:43.995959 airscript-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      690 2023-08-02 04:25:19.000000 airscript-0.0.6/setup.py
```

### Comparing `airscript-0.0.5/airscript/action/key.py` & `airscript-0.0.6/airscript/action/key.py`

 * *Files identical despite different names*

### Comparing `airscript-0.0.5/airscript/action/path.py` & `airscript-0.0.6/airscript/action/path.py`

 * *Files identical despite different names*

### Comparing `airscript-0.0.5/airscript/screen/__init__.py` & `airscript-0.0.6/airscript/screen/__init__.py`

 * *Files identical despite different names*

### Comparing `airscript-0.0.5/airscript/system/__init__.py` & `airscript-0.0.6/airscript/system/__init__.py`

 * *Files identical despite different names*

### Comparing `airscript-0.0.5/airscript/ui/__init__.py` & `airscript-0.0.6/airscript/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `airscript-0.0.5/airscript/ui/dialog.py` & `airscript-0.0.6/airscript/ui/dialog.py`

 * *Files identical despite different names*

### Comparing `airscript-0.0.5/setup.py` & `airscript-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
-DESCRIPTION = 'airscript Type derivation package'
+VERSION = '0.0.6'
+DESCRIPTION = 'airscript 类型提示语言包'
 
 setup(
     name="airscript",
     version=VERSION,
     author="ITisl",
-    author_email="1831207432@qq.com",
+    author_email="aojoy@163.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding="UTF8").read(),
     packages=find_packages(),
     keywords=['python', "airscript"],
     license="MIT",
-classifiers=[
+    classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     url="https://github.com/itisl2220/airscript",
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

