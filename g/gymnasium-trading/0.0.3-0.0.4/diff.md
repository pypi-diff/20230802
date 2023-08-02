# Comparing `tmp/gymnasium_trading-0.0.3.tar.gz` & `tmp/gymnasium_trading-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_trading-0.0.3.tar", last modified: Tue Aug  1 22:38:19 2023, max compression
+gzip compressed data, was "gymnasium_trading-0.0.4.tar", last modified: Wed Aug  2 16:19:54 2023, max compression
```

## Comparing `gymnasium_trading-0.0.3.tar` & `gymnasium_trading-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 22:38:19.872533 gymnasium_trading-0.0.3/
--rw-rw-rw-   0        0        0    35823 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      386 2023-08-01 22:38:19.874040 gymnasium_trading-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       72 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 22:38:19.833963 gymnasium_trading-0.0.3/gymnasium_trading/
--rw-rw-rw-   0        0        0      188 2023-08-01 21:25:19.000000 gymnasium_trading-0.0.3/gymnasium_trading/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 22:38:19.872533 gymnasium_trading-0.0.3/gymnasium_trading/envs/
--rw-rw-rw-   0        0        0       74 2023-08-01 21:26:27.000000 gymnasium_trading-0.0.3/gymnasium_trading/envs/__init__.py
--rw-rw-rw-   0        0        0     6362 2023-08-01 21:24:08.000000 gymnasium_trading-0.0.3/gymnasium_trading/envs/gymnasium_trading.py
-drwxrwxrwx   0        0        0        0 2023-08-01 22:38:19.868518 gymnasium_trading-0.0.3/gymnasium_trading.egg-info/
--rw-rw-rw-   0        0        0      386 2023-08-01 22:38:19.000000 gymnasium_trading-0.0.3/gymnasium_trading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-08-01 22:38:19.000000 gymnasium_trading-0.0.3/gymnasium_trading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 22:38:19.000000 gymnasium_trading-0.0.3/gymnasium_trading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-08-01 22:38:19.000000 gymnasium_trading-0.0.3/gymnasium_trading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-08-01 22:38:19.000000 gymnasium_trading-0.0.3/gymnasium_trading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-01 22:38:19.875478 gymnasium_trading-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-08-01 22:37:49.000000 gymnasium_trading-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:19:54.945781 gymnasium_trading-0.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      386 2023-08-02 16:19:54.945781 gymnasium_trading-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 16:19:54.913455 gymnasium_trading-0.0.4/gymnasium_trading/
+-rw-rw-rw-   0        0        0      186 2023-08-02 16:15:29.000000 gymnasium_trading-0.0.4/gymnasium_trading/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:19:54.944788 gymnasium_trading-0.0.4/gymnasium_trading/envs/
+-rw-rw-rw-   0        0        0       68 2023-08-02 16:03:22.000000 gymnasium_trading-0.0.4/gymnasium_trading/envs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:19:54.942791 gymnasium_trading-0.0.4/gymnasium_trading.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-08-02 16:19:54.000000 gymnasium_trading-0.0.4/gymnasium_trading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-08-02 16:19:54.000000 gymnasium_trading-0.0.4/gymnasium_trading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 16:19:54.000000 gymnasium_trading-0.0.4/gymnasium_trading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-02 16:19:54.000000 gymnasium_trading-0.0.4/gymnasium_trading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-02 16:19:54.000000 gymnasium_trading-0.0.4/gymnasium_trading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-02 16:19:54.948284 gymnasium_trading-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-08-02 16:18:33.000000 gymnasium_trading-0.0.4/setup.py
```

### Comparing `gymnasium_trading-0.0.3/LICENSE` & `gymnasium_trading-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_trading-0.0.3/setup.py` & `gymnasium_trading-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="gymnasium_trading",
-    version="0.0.3",
+    version="0.0.4",
     install_requires=["gymnasium==0.28.1", "pygame==2.5.0"],
     author='Alejandro Rioja Chocrón',
     author_email='archocron@gmail.com',
     url='https://github.com/archocron/gymnasium-trading',
     packages=['gymnasium_trading'],
     license='gpl-3.0',
     description='Gimnasium environment focus on trading strategies',
```

