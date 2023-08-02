# Comparing `tmp/yyszh-0.1.3.tar.gz` & `tmp/yyszh-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yyszh-0.1.3.tar", last modified: Wed Aug  2 05:40:08 2023, max compression
+gzip compressed data, was "dist\yyszh-0.1.4.tar", last modified: Wed Aug  2 05:45:12 2023, max compression
```

## Comparing `yyszh-0.1.3.tar` & `yyszh-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 05:40:08.000000 yyszh-0.1.3/
--rw-rw-rw-   0        0        0      157 2023-08-02 05:40:08.000000 yyszh-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0        5 2023-07-04 11:22:41.000000 yyszh-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-08-02 05:40:08.000000 yyszh-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-08-02 05:39:59.000000 yyszh-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 05:40:08.000000 yyszh-0.1.3/yyszh/
--rw-rw-rw-   0        0        0     1888 2023-08-02 03:21:55.000000 yyszh-0.1.3/yyszh/__init__.py
--rw-rw-rw-   0        0        0    23737 2023-08-02 02:39:32.000000 yyszh-0.1.3/yyszh/utils.py
--rw-rw-rw-   0        0        0     1486 2023-08-02 05:39:50.000000 yyszh-0.1.3/yyszh/word_cloud_diagram.py
-drwxrwxrwx   0        0        0        0 2023-08-02 05:40:08.000000 yyszh-0.1.3/yyszh.egg-info/
--rw-rw-rw-   0        0        0      157 2023-08-02 05:40:08.000000 yyszh-0.1.3/yyszh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-08-02 05:40:08.000000 yyszh-0.1.3/yyszh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 05:40:08.000000 yyszh-0.1.3/yyszh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-08-02 05:40:08.000000 yyszh-0.1.3/yyszh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-02 05:40:08.000000 yyszh-0.1.3/yyszh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 05:45:12.000000 yyszh-0.1.4/
+-rw-rw-rw-   0        0        0      157 2023-08-02 05:45:12.000000 yyszh-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2023-07-04 11:22:41.000000 yyszh-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-02 05:45:12.000000 yyszh-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-08-02 05:45:06.000000 yyszh-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:45:12.000000 yyszh-0.1.4/yyszh/
+-rw-rw-rw-   0        0        0     1888 2023-08-02 03:21:55.000000 yyszh-0.1.4/yyszh/__init__.py
+-rw-rw-rw-   0        0        0    11425 2023-08-02 05:42:51.000000 yyszh-0.1.4/yyszh/hit_stopwords.py
+-rw-rw-rw-   0        0        0    23737 2023-08-02 02:39:32.000000 yyszh-0.1.4/yyszh/utils.py
+-rw-rw-rw-   0        0        0     1484 2023-08-02 05:45:06.000000 yyszh-0.1.4/yyszh/word_cloud_diagram.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:45:12.000000 yyszh-0.1.4/yyszh.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-08-02 05:45:12.000000 yyszh-0.1.4/yyszh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-08-02 05:45:12.000000 yyszh-0.1.4/yyszh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 05:45:12.000000 yyszh-0.1.4/yyszh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-08-02 05:45:12.000000 yyszh-0.1.4/yyszh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-02 05:45:12.000000 yyszh-0.1.4/yyszh.egg-info/top_level.txt
```

### Comparing `yyszh-0.1.3/setup.py` & `yyszh-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='yyszh',
-    version='0.1.3',
+    version='0.1.4',
     description=(
         'utils for yyszhyyy'
     ),
     author='yyszh',
     author_email='yyszhyyy@163.com',
     license='Apache License 2.0',
     include_package_data=True,
```

### Comparing `yyszh-0.1.3/yyszh/__init__.py` & `yyszh-0.1.4/yyszh/__init__.py`

 * *Files identical despite different names*

### Comparing `yyszh-0.1.3/yyszh/utils.py` & `yyszh-0.1.4/yyszh/utils.py`

 * *Files identical despite different names*

### Comparing `yyszh-0.1.3/yyszh/word_cloud_diagram.py` & `yyszh-0.1.4/yyszh/word_cloud_diagram.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import jieba
 import matplotlib.pyplot as plt
 from wordcloud import WordCloud
 import yyszh.utils as utils
+from yyszh.hit_stopwords import stopwords
 
 def word_cloud_diagram(txt_path, diagram_path, stop_words=None):
     """
     生成词云图的函数，将txt中的内容根据关键词生成词云图
     如：
         word_cloud_diagram('test.txt', 'ciyun.png', stop_words=['吃饭', '睡觉', '上班'])
         将本地的test.txt文件生成词云图，并保存到ciyun.png，自己添加了 吃饭、睡觉、上班三个停用词
     :param txt_path: txt文本路径
     :param diagram_path: 词云图保存路径
     :param stop_words: list，自定义停用词，默认已经使用哈工大停用词
     """
-    stops = utils.read_json('yyszh/hit_stopwords.json')
     if isinstance(stop_words, list):
         for s in stop_words:
-            if s not in stops:
-                stops.append(s)
+            if s not in stopwords:
+                stopwords.append(s)
 
     text = open(txt_path, encoding="utf-8").read()  # 标明文本路径，打开
     data_cut = jieba.lcut(text, cut_all=False)
 
     data_result = []
     for i in data_cut:
-        if i not in stops:
+        if i not in stopwords:
             data_result.append(i)
     text = " ".join(data_result).replace("\n", " ")
 
     # 生成对象
     wc = WordCloud(font_path = "data/msyh.ttc",width=1500, height=1200, mode="RGBA", background_color=None).generate(text)
 
     # 保存词云图
```

