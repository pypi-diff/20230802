# Comparing `tmp/gymnasium_trading-0.0.2.tar.gz` & `tmp/gymnasium_trading-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_trading-0.0.2.tar", last modified: Tue Aug  1 22:01:28 2023, max compression
+gzip compressed data, was "gymnasium_trading-0.0.3.tar", last modified: Tue Aug  1 22:38:19 2023, max compression
```

## Comparing `gymnasium_trading-0.0.2.tar` & `gymnasium_trading-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 22:01:28.077174 gymnasium_trading-0.0.2/
--rw-rw-rw-   0        0        0    35823 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      386 2023-08-01 22:01:28.077174 gymnasium_trading-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       72 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 22:01:28.058565 gymnasium_trading-0.0.2/gymnasium_trading/
--rw-rw-rw-   0        0        0      188 2023-08-01 21:25:19.000000 gymnasium_trading-0.0.2/gymnasium_trading/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 22:01:28.076181 gymnasium_trading-0.0.2/gymnasium_trading/envs/
--rw-rw-rw-   0        0        0       74 2023-08-01 21:26:27.000000 gymnasium_trading-0.0.2/gymnasium_trading/envs/__init__.py
--rw-rw-rw-   0        0        0     6362 2023-08-01 21:24:08.000000 gymnasium_trading-0.0.2/gymnasium_trading/envs/gymnasium_trading.py
-drwxrwxrwx   0        0        0        0 2023-08-01 22:01:28.073187 gymnasium_trading-0.0.2/gymnasium_trading.egg-info/
--rw-rw-rw-   0        0        0      386 2023-08-01 22:01:27.000000 gymnasium_trading-0.0.2/gymnasium_trading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-08-01 22:01:27.000000 gymnasium_trading-0.0.2/gymnasium_trading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 22:01:27.000000 gymnasium_trading-0.0.2/gymnasium_trading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-08-01 22:01:27.000000 gymnasium_trading-0.0.2/gymnasium_trading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-08-01 22:01:27.000000 gymnasium_trading-0.0.2/gymnasium_trading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-01 22:01:28.078184 gymnasium_trading-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-08-01 22:01:20.000000 gymnasium_trading-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:38:19.872533 gymnasium_trading-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      386 2023-08-01 22:38:19.874040 gymnasium_trading-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 22:38:19.833963 gymnasium_trading-0.0.3/gymnasium_trading/
+-rw-rw-rw-   0        0        0      188 2023-08-01 21:25:19.000000 gymnasium_trading-0.0.3/gymnasium_trading/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:38:19.872533 gymnasium_trading-0.0.3/gymnasium_trading/envs/
+-rw-rw-rw-   0        0        0       74 2023-08-01 21:26:27.000000 gymnasium_trading-0.0.3/gymnasium_trading/envs/__init__.py
+-rw-rw-rw-   0        0        0     6362 2023-08-01 21:24:08.000000 gymnasium_trading-0.0.3/gymnasium_trading/envs/gymnasium_trading.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:38:19.868518 gymnasium_trading-0.0.3/gymnasium_trading.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-08-01 22:38:19.000000 gymnasium_trading-0.0.3/gymnasium_trading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-08-01 22:38:19.000000 gymnasium_trading-0.0.3/gymnasium_trading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 22:38:19.000000 gymnasium_trading-0.0.3/gymnasium_trading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-01 22:38:19.000000 gymnasium_trading-0.0.3/gymnasium_trading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-01 22:38:19.000000 gymnasium_trading-0.0.3/gymnasium_trading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-01 22:38:19.875478 gymnasium_trading-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-08-01 22:37:49.000000 gymnasium_trading-0.0.3/setup.py
```

### Comparing `gymnasium_trading-0.0.2/LICENSE` & `gymnasium_trading-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_trading-0.0.2/gymnasium_trading/envs/gymnasium_trading.py` & `gymnasium_trading-0.0.3/gymnasium_trading/envs/gymnasium_trading.py`

 * *Files identical despite different names*

### Comparing `gymnasium_trading-0.0.2/setup.py` & `gymnasium_trading-0.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     name="gymnasium_trading",
-    version="0.0.2",
-    install_requires=["gymnasium==0.29.0", "pygame==2.5.0"],
+    version="0.0.3",
+    install_requires=["gymnasium==0.28.1", "pygame==2.5.0"],
     author='Alejandro Rioja Chocrón',
     author_email='archocron@gmail.com',
     url='https://github.com/archocron/gymnasium-trading',
     packages=['gymnasium_trading'],
     license='gpl-3.0',
     description='Gimnasium environment focus on trading strategies',
     # I explain this later on
-    download_url='https://github.com/archocron/gymnasium-trading/archive/refs/tags/0.0.2.tar.gz',
+    download_url='https://github.com/archocron/gymnasium-trading/archive/refs/tags/0.0.3.tar.gz',
 
 )
```

