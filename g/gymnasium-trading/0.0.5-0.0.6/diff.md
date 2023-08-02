# Comparing `tmp/gymnasium_trading-0.0.5.tar.gz` & `tmp/gymnasium_trading-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_trading-0.0.5.tar", last modified: Wed Aug  2 16:25:19 2023, max compression
+gzip compressed data, was "gymnasium_trading-0.0.6.tar", last modified: Wed Aug  2 16:36:00 2023, max compression
```

## Comparing `gymnasium_trading-0.0.5.tar` & `gymnasium_trading-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 16:25:19.904207 gymnasium_trading-0.0.5/
--rw-rw-rw-   0        0        0    35823 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      386 2023-08-02 16:25:19.904207 gymnasium_trading-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       72 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 16:25:19.880322 gymnasium_trading-0.0.5/gymnasium_trading/
--rw-rw-rw-   0        0        0      198 2023-08-02 16:24:29.000000 gymnasium_trading-0.0.5/gymnasium_trading/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:25:19.903044 gymnasium_trading-0.0.5/gymnasium_trading/envs/
--rw-rw-rw-   0        0        0       68 2023-08-02 16:03:22.000000 gymnasium_trading-0.0.5/gymnasium_trading/envs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:25:19.901565 gymnasium_trading-0.0.5/gymnasium_trading.egg-info/
--rw-rw-rw-   0        0        0      386 2023-08-02 16:25:19.000000 gymnasium_trading-0.0.5/gymnasium_trading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-08-02 16:25:19.000000 gymnasium_trading-0.0.5/gymnasium_trading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 16:25:19.000000 gymnasium_trading-0.0.5/gymnasium_trading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-08-02 16:25:19.000000 gymnasium_trading-0.0.5/gymnasium_trading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-08-02 16:25:19.000000 gymnasium_trading-0.0.5/gymnasium_trading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-02 16:25:19.906568 gymnasium_trading-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-08-02 16:24:54.000000 gymnasium_trading-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:36:00.165772 gymnasium_trading-0.0.6/
+-rw-rw-rw-   0        0        0    35823 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      386 2023-08-02 16:36:00.165772 gymnasium_trading-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 16:36:00.145533 gymnasium_trading-0.0.6/gymnasium_trading/
+-rw-rw-rw-   0        0        0      193 2023-08-02 16:35:28.000000 gymnasium_trading-0.0.6/gymnasium_trading/__init__.py
+-rw-rw-rw-   0        0        0     6362 2023-08-01 21:24:08.000000 gymnasium_trading-0.0.6/gymnasium_trading/gym_trading.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:36:00.164730 gymnasium_trading-0.0.6/gymnasium_trading.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-08-02 16:35:59.000000 gymnasium_trading-0.0.6/gymnasium_trading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-08-02 16:36:00.000000 gymnasium_trading-0.0.6/gymnasium_trading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 16:35:59.000000 gymnasium_trading-0.0.6/gymnasium_trading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-02 16:35:59.000000 gymnasium_trading-0.0.6/gymnasium_trading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-02 16:35:59.000000 gymnasium_trading-0.0.6/gymnasium_trading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-02 16:36:00.167800 gymnasium_trading-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-08-02 16:35:56.000000 gymnasium_trading-0.0.6/setup.py
```

### Comparing `gymnasium_trading-0.0.5/LICENSE` & `gymnasium_trading-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_trading-0.0.5/setup.py` & `gymnasium_trading-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="gymnasium_trading",
-    version="0.0.5",
+    version="0.0.6",
     install_requires=["gymnasium==0.28.1", "pygame==2.5.0"],
     author='Alejandro Rioja Chocrón',
     author_email='archocron@gmail.com',
     url='https://github.com/archocron/gymnasium-trading',
     packages=['gymnasium_trading'],
     license='gpl-3.0',
     description='Gimnasium environment focus on trading strategies',
```

