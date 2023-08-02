# Comparing `tmp/yyszh-0.1.1.tar.gz` & `tmp/yyszh-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yyszh-0.1.1.tar", last modified: Wed Aug  2 03:22:22 2023, max compression
+gzip compressed data, was "dist\yyszh-0.1.2.tar", last modified: Wed Aug  2 03:25:50 2023, max compression
```

## Comparing `yyszh-0.1.1.tar` & `yyszh-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 03:22:22.000000 yyszh-0.1.1/
--rw-rw-rw-   0        0        0      157 2023-08-02 03:22:22.000000 yyszh-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        5 2023-07-04 11:22:41.000000 yyszh-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-02 03:22:22.000000 yyszh-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-08-02 03:13:49.000000 yyszh-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh/
--rw-rw-rw-   0        0        0     1888 2023-08-02 03:21:55.000000 yyszh-0.1.1/yyszh/__init__.py
--rw-rw-rw-   0        0        0    23737 2023-08-02 02:39:32.000000 yyszh-0.1.1/yyszh/utils.py
--rw-rw-rw-   0        0        0     1471 2023-08-02 03:21:55.000000 yyszh-0.1.1/yyszh/word_cloud_diagram.py
-drwxrwxrwx   0        0        0        0 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh.egg-info/
--rw-rw-rw-   0        0        0      157 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 03:25:50.000000 yyszh-0.1.2/
+-rw-rw-rw-   0        0        0      157 2023-08-02 03:25:50.000000 yyszh-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2023-07-04 11:22:41.000000 yyszh-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-02 03:25:50.000000 yyszh-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-08-02 03:25:30.000000 yyszh-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 03:25:50.000000 yyszh-0.1.2/yyszh/
+-rw-rw-rw-   0        0        0     1888 2023-08-02 03:21:55.000000 yyszh-0.1.2/yyszh/__init__.py
+-rw-rw-rw-   0        0        0    23737 2023-08-02 02:39:32.000000 yyszh-0.1.2/yyszh/utils.py
+-rw-rw-rw-   0        0        0     1480 2023-08-02 03:24:57.000000 yyszh-0.1.2/yyszh/word_cloud_diagram.py
+drwxrwxrwx   0        0        0        0 2023-08-02 03:25:50.000000 yyszh-0.1.2/yyszh.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-08-02 03:25:49.000000 yyszh-0.1.2/yyszh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-08-02 03:25:50.000000 yyszh-0.1.2/yyszh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 03:25:49.000000 yyszh-0.1.2/yyszh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-08-02 03:25:49.000000 yyszh-0.1.2/yyszh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-02 03:25:49.000000 yyszh-0.1.2/yyszh.egg-info/top_level.txt
```

### Comparing `yyszh-0.1.1/setup.py` & `yyszh-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='yyszh',
-    version='0.1.1',
+    version='0.1.2',
     description=(
         'utils for yyszhyyy'
     ),
     author='yyszh',
     author_email='yyszhyyy@163.com',
     license='Apache License 2.0',
     include_package_data=True,
```

### Comparing `yyszh-0.1.1/yyszh/__init__.py` & `yyszh-0.1.2/yyszh/__init__.py`

 * *Files identical despite different names*

### Comparing `yyszh-0.1.1/yyszh/utils.py` & `yyszh-0.1.2/yyszh/utils.py`

 * *Files identical despite different names*

### Comparing `yyszh-0.1.1/yyszh/word_cloud_diagram.py` & `yyszh-0.1.2/yyszh/word_cloud_diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import jieba
 import matplotlib.pyplot as plt
 from wordcloud import WordCloud
-import yyszh.utils
+import yyszh.utils as utils
 
 def word_cloud_diagram(txt_path, diagram_path, stop_words=None):
     """
     生成词云图的函数，将txt中的内容根据关键词生成词云图
     如：
         word_cloud_diagram('test.txt', 'ciyun.png', stop_words=['吃饭', '睡觉', '上班'])
         将本地的test.txt文件生成词云图，并保存到ciyun.png，自己添加了 吃饭、睡觉、上班三个停用词
```

