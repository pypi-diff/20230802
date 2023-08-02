# Comparing `tmp/gymnasium_trading-0.0.4.tar.gz` & `tmp/gymnasium_trading-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_trading-0.0.4.tar", last modified: Wed Aug  2 16:19:54 2023, max compression
+gzip compressed data, was "gymnasium_trading-0.0.5.tar", last modified: Wed Aug  2 16:25:19 2023, max compression
```

## Comparing `gymnasium_trading-0.0.4.tar` & `gymnasium_trading-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 16:19:54.945781 gymnasium_trading-0.0.4/
--rw-rw-rw-   0        0        0    35823 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      386 2023-08-02 16:19:54.945781 gymnasium_trading-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       72 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 16:19:54.913455 gymnasium_trading-0.0.4/gymnasium_trading/
--rw-rw-rw-   0        0        0      186 2023-08-02 16:15:29.000000 gymnasium_trading-0.0.4/gymnasium_trading/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:19:54.944788 gymnasium_trading-0.0.4/gymnasium_trading/envs/
--rw-rw-rw-   0        0        0       68 2023-08-02 16:03:22.000000 gymnasium_trading-0.0.4/gymnasium_trading/envs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:19:54.942791 gymnasium_trading-0.0.4/gymnasium_trading.egg-info/
--rw-rw-rw-   0        0        0      386 2023-08-02 16:19:54.000000 gymnasium_trading-0.0.4/gymnasium_trading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-08-02 16:19:54.000000 gymnasium_trading-0.0.4/gymnasium_trading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 16:19:54.000000 gymnasium_trading-0.0.4/gymnasium_trading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-08-02 16:19:54.000000 gymnasium_trading-0.0.4/gymnasium_trading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-08-02 16:19:54.000000 gymnasium_trading-0.0.4/gymnasium_trading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-02 16:19:54.948284 gymnasium_trading-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-08-02 16:18:33.000000 gymnasium_trading-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:25:19.904207 gymnasium_trading-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      386 2023-08-02 16:25:19.904207 gymnasium_trading-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 16:25:19.880322 gymnasium_trading-0.0.5/gymnasium_trading/
+-rw-rw-rw-   0        0        0      198 2023-08-02 16:24:29.000000 gymnasium_trading-0.0.5/gymnasium_trading/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:25:19.903044 gymnasium_trading-0.0.5/gymnasium_trading/envs/
+-rw-rw-rw-   0        0        0       68 2023-08-02 16:03:22.000000 gymnasium_trading-0.0.5/gymnasium_trading/envs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:25:19.901565 gymnasium_trading-0.0.5/gymnasium_trading.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-08-02 16:25:19.000000 gymnasium_trading-0.0.5/gymnasium_trading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-08-02 16:25:19.000000 gymnasium_trading-0.0.5/gymnasium_trading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 16:25:19.000000 gymnasium_trading-0.0.5/gymnasium_trading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-02 16:25:19.000000 gymnasium_trading-0.0.5/gymnasium_trading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-02 16:25:19.000000 gymnasium_trading-0.0.5/gymnasium_trading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-02 16:25:19.906568 gymnasium_trading-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-08-02 16:24:54.000000 gymnasium_trading-0.0.5/setup.py
```

### Comparing `gymnasium_trading-0.0.4/LICENSE` & `gymnasium_trading-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_trading-0.0.4/setup.py` & `gymnasium_trading-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="gymnasium_trading",
-    version="0.0.4",
+    version="0.0.5",
     install_requires=["gymnasium==0.28.1", "pygame==2.5.0"],
     author='Alejandro Rioja Chocrón',
     author_email='archocron@gmail.com',
     url='https://github.com/archocron/gymnasium-trading',
     packages=['gymnasium_trading'],
     license='gpl-3.0',
     description='Gimnasium environment focus on trading strategies',
```

