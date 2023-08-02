# Comparing `tmp/scPANTHEON-0.3.8.tar.gz` & `tmp/scPANTHEON-0.3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.3.8.tar", last modified: Thu Jul 20 07:42:01 2023, max compression
+gzip compressed data, was "scPANTHEON-0.3.9.1.tar", last modified: Wed Aug  2 08:25:03 2023, max compression
```

## Comparing `scPANTHEON-0.3.8.tar` & `scPANTHEON-0.3.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 07:42:01.762666 scPANTHEON-0.3.8/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0      288 2023-07-20 07:42:01.761666 scPANTHEON-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 07:42:01.735655 scPANTHEON-0.3.8/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      288 2023-07-20 07:42:01.000000 scPANTHEON-0.3.8/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-07-20 07:42:01.000000 scPANTHEON-0.3.8/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 07:42:01.000000 scPANTHEON-0.3.8/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-20 07:42:01.000000 scPANTHEON-0.3.8/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      175 2023-07-20 07:42:01.000000 scPANTHEON-0.3.8/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-20 07:42:01.000000 scPANTHEON-0.3.8/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 07:42:01.743866 scPANTHEON-0.3.8/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.8/scpantheon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 07:42:01.750471 scPANTHEON-0.3.8/scpantheon/app/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.8/scpantheon/app/__init__.py
--rw-rw-rw-   0        0        0     2607 2023-07-05 15:50:04.000000 scPANTHEON-0.3.8/scpantheon/app/bokeh_qt.py
-drwxrwxrwx   0        0        0        0 2023-07-20 07:42:01.758639 scPANTHEON-0.3.8/scpantheon/front_end/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.8/scpantheon/front_end/__init__.py
--rw-rw-rw-   0        0        0     5711 2023-07-13 13:24:16.000000 scPANTHEON-0.3.8/scpantheon/front_end/data_qt.py
--rw-rw-rw-   0        0        0     3683 2023-07-10 13:33:19.000000 scPANTHEON-0.3.8/scpantheon/front_end/save_qt.py
--rw-rw-rw-   0        0        0     1363 2023-07-20 07:37:16.000000 scPANTHEON-0.3.8/scpantheon/main.py
--rw-rw-rw-   0        0        0    66241 2023-07-20 07:40:37.000000 scPANTHEON-0.3.8/scpantheon/source.py
--rw-rw-rw-   0        0        0       42 2023-07-20 07:42:01.762666 scPANTHEON-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1206 2023-07-20 07:41:24.000000 scPANTHEON-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:25:03.377318 scPANTHEON-0.3.9.1/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      290 2023-08-02 08:25:03.377318 scPANTHEON-0.3.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 08:25:03.362903 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      290 2023-08-02 08:25:03.000000 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-08-02 08:25:03.000000 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:25:03.000000 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-08-02 08:25:03.000000 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      109 2023-08-02 08:25:03.000000 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-02 08:25:03.000000 scPANTHEON-0.3.9.1/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 08:25:03.366924 scPANTHEON-0.3.9.1/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.1/scpantheon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:25:03.369526 scPANTHEON-0.3.9.1/scpantheon/app/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.1/scpantheon/app/__init__.py
+-rw-rw-rw-   0        0        0     2607 2023-07-05 15:50:04.000000 scPANTHEON-0.3.9.1/scpantheon/app/bokeh_qt.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:25:03.374386 scPANTHEON-0.3.9.1/scpantheon/front_end/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.9.1/scpantheon/front_end/__init__.py
+-rw-rw-rw-   0        0        0     5711 2023-07-13 13:24:16.000000 scPANTHEON-0.3.9.1/scpantheon/front_end/data_qt.py
+-rw-rw-rw-   0        0        0     3683 2023-07-10 13:33:19.000000 scPANTHEON-0.3.9.1/scpantheon/front_end/save_qt.py
+-rw-rw-rw-   0        0        0     1363 2023-07-20 07:37:16.000000 scPANTHEON-0.3.9.1/scpantheon/main.py
+-rw-rw-rw-   0        0        0    66241 2023-07-20 07:40:37.000000 scPANTHEON-0.3.9.1/scpantheon/source.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 08:25:03.377318 scPANTHEON-0.3.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-08-02 08:24:06.000000 scPANTHEON-0.3.9.1/setup.py
```

### Comparing `scPANTHEON-0.3.8/scpantheon/app/bokeh_qt.py` & `scPANTHEON-0.3.9.1/scpantheon/app/bokeh_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.8/scpantheon/front_end/data_qt.py` & `scPANTHEON-0.3.9.1/scpantheon/front_end/data_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.8/scpantheon/front_end/save_qt.py` & `scPANTHEON-0.3.9.1/scpantheon/front_end/save_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.8/scpantheon/main.py` & `scPANTHEON-0.3.9.1/scpantheon/main.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.8/scpantheon/source.py` & `scPANTHEON-0.3.9.1/scpantheon/source.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.8/setup.py` & `scPANTHEON-0.3.9.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.3.8',#版本
+    version='0.3.9.1',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon', 'scpantheon.app', 'scpantheon.front_end'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
-    install_requires=['bokeh==2.4.3','pandas==1.4.4','anndata==0.8.0','colorcet==3.0.0','scanpy==1.9.1','numpy==1.21.5','PyQt5==5.15.9','PyQtWebEngine==5.15.6',
-                        'appdirs==1.4.4',], # 依赖包,如果没有,可以不要
+    install_requires=['bokeh','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
+                        'appdirs',], # 依赖包,如果没有,可以不要
     extras_require={
         'tomas': ['tomas'], 'leidenalg': ['leidenalg']
     }, # 依赖包,深度使用需手动安装
     entry_points={
         'console_scripts': [
             'sc-pantheon = scpantheon.main:main' # scripts -> multiprocessing
         ]
```

