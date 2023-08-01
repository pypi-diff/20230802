# Comparing `tmp/gymnasium-trading-0.0.1.tar.gz` & `tmp/gymnasium_trading-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium-trading-0.0.1.tar", last modified: Tue Aug  1 21:32:37 2023, max compression
+gzip compressed data, was "gymnasium_trading-0.0.2.tar", last modified: Tue Aug  1 22:01:28 2023, max compression
```

## Comparing `gymnasium-trading-0.0.1.tar` & `gymnasium_trading-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 21:32:37.248402 gymnasium-trading-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-08-01 20:41:48.000000 gymnasium-trading-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       87 2023-08-01 21:32:37.248402 gymnasium-trading-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       72 2023-08-01 20:41:48.000000 gymnasium-trading-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 21:32:37.215441 gymnasium-trading-0.0.1/gymnasium_trading/
--rw-rw-rw-   0        0        0      188 2023-08-01 21:25:19.000000 gymnasium-trading-0.0.1/gymnasium_trading/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:32:37.247375 gymnasium-trading-0.0.1/gymnasium_trading/envs/
--rw-rw-rw-   0        0        0       74 2023-08-01 21:26:27.000000 gymnasium-trading-0.0.1/gymnasium_trading/envs/__init__.py
--rw-rw-rw-   0        0        0     6362 2023-08-01 21:24:08.000000 gymnasium-trading-0.0.1/gymnasium_trading/envs/gymnasium_trading.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:32:37.244404 gymnasium-trading-0.0.1/gymnasium_trading.egg-info/
--rw-rw-rw-   0        0        0       87 2023-08-01 21:32:37.000000 gymnasium-trading-0.0.1/gymnasium_trading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-08-01 21:32:37.000000 gymnasium-trading-0.0.1/gymnasium_trading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 21:32:37.000000 gymnasium-trading-0.0.1/gymnasium_trading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-08-01 21:32:37.000000 gymnasium-trading-0.0.1/gymnasium_trading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-08-01 21:32:37.000000 gymnasium-trading-0.0.1/gymnasium_trading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-01 21:32:37.254549 gymnasium-trading-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      158 2023-08-01 21:15:00.000000 gymnasium-trading-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:01:28.077174 gymnasium_trading-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      386 2023-08-01 22:01:28.077174 gymnasium_trading-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2023-08-01 20:41:48.000000 gymnasium_trading-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 22:01:28.058565 gymnasium_trading-0.0.2/gymnasium_trading/
+-rw-rw-rw-   0        0        0      188 2023-08-01 21:25:19.000000 gymnasium_trading-0.0.2/gymnasium_trading/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:01:28.076181 gymnasium_trading-0.0.2/gymnasium_trading/envs/
+-rw-rw-rw-   0        0        0       74 2023-08-01 21:26:27.000000 gymnasium_trading-0.0.2/gymnasium_trading/envs/__init__.py
+-rw-rw-rw-   0        0        0     6362 2023-08-01 21:24:08.000000 gymnasium_trading-0.0.2/gymnasium_trading/envs/gymnasium_trading.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:01:28.073187 gymnasium_trading-0.0.2/gymnasium_trading.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-08-01 22:01:27.000000 gymnasium_trading-0.0.2/gymnasium_trading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-08-01 22:01:27.000000 gymnasium_trading-0.0.2/gymnasium_trading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 22:01:27.000000 gymnasium_trading-0.0.2/gymnasium_trading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-01 22:01:27.000000 gymnasium_trading-0.0.2/gymnasium_trading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-01 22:01:27.000000 gymnasium_trading-0.0.2/gymnasium_trading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-01 22:01:28.078184 gymnasium_trading-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-08-01 22:01:20.000000 gymnasium_trading-0.0.2/setup.py
```

### Comparing `gymnasium-trading-0.0.1/LICENSE` & `gymnasium_trading-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium-trading-0.0.1/gymnasium_trading/envs/gymnasium_trading.py` & `gymnasium_trading-0.0.2/gymnasium_trading/envs/gymnasium_trading.py`

 * *Files identical despite different names*

