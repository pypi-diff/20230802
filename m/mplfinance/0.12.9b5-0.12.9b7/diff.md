# Comparing `tmp/mplfinance-0.12.9b5.tar.gz` & `tmp/mplfinance-0.12.9b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mplfinance-0.12.9b5.tar", last modified: Wed Nov  2 01:41:48 2022, max compression
+gzip compressed data, was "mplfinance-0.12.9b7.tar", last modified: Thu Dec  8 21:13:00 2022, max compression
```

## Comparing `mplfinance-0.12.9b5.tar` & `mplfinance-0.12.9b7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 01:41:48.957405 mplfinance-0.12.9b5/
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    18966 2022-11-02 01:41:48.957405 mplfinance-0.12.9b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17606 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-02 01:41:48.957405 mplfinance-0.12.9b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 01:41:48.953405 mplfinance-0.12.9b5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 01:41:48.957405 mplfinance-0.12.9b5/src/mplfinance/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18987 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_arg_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4090 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5596 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_kwarg_help.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_mpf_warnings.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2276 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_mplrcputils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4157 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_mplwraps.py
--rw-r--r--   0 runner    (1001) docker     (121)     9033 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_panels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 01:41:48.957405 mplfinance-0.12.9b5/src/mplfinance/_styledata/
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/binance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/blueskies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/brasil.py
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/charles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/checkers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/classic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/default.py
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/ibd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/kenan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2105 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/mike.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/nightclouds.py
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/sas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/starsandstripes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styledata/yahoo.py
--rw-r--r--   0 runner    (1001) docker     (121)    16399 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_styles.py
--rw-r--r--   0 runner    (1001) docker     (121)    62404 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     8563 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/_widths.py
--rw-r--r--   0 runner    (1001) docker     (121)    27280 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/original_flavor.py
--rw-r--r--   0 runner    (1001) docker     (121)    70249 2022-11-02 01:41:41.000000 mplfinance-0.12.9b5/src/mplfinance/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 01:41:48.957405 mplfinance-0.12.9b5/src/mplfinance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18966 2022-11-02 01:41:48.000000 mplfinance-0.12.9b5/src/mplfinance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-11-02 01:41:48.000000 mplfinance-0.12.9b5/src/mplfinance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 01:41:48.000000 mplfinance-0.12.9b5/src/mplfinance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-02 01:41:48.000000 mplfinance-0.12.9b5/src/mplfinance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-02 01:41:48.000000 mplfinance-0.12.9b5/src/mplfinance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 21:13:00.130370 mplfinance-0.12.9b7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2022-12-08 21:12:51.000000 mplfinance-0.12.9b7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-08 21:12:51.000000 mplfinance-0.12.9b7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18966 2022-12-08 21:13:00.130370 mplfinance-0.12.9b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17606 2022-12-08 21:12:51.000000 mplfinance-0.12.9b7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 21:13:00.130370 mplfinance-0.12.9b7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 21:13:00.122370 mplfinance-0.12.9b7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 21:13:00.126370 mplfinance-0.12.9b7/src/mplfinance/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18987 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_arg_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_kwarg_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_mpf_warnings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2276 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_mplrcputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_mplwraps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 21:13:00.130370 mplfinance-0.12.9b7/src/mplfinance/_styledata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/blueskies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/brasil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/charles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/ibd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/kenan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/mike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/nightclouds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/sas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/starsandstripes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styledata/yahoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64528 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/_widths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27280 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/original_flavor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71668 2022-12-08 21:12:52.000000 mplfinance-0.12.9b7/src/mplfinance/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 21:13:00.130370 mplfinance-0.12.9b7/src/mplfinance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18966 2022-12-08 21:13:00.000000 mplfinance-0.12.9b7/src/mplfinance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2022-12-08 21:13:00.000000 mplfinance-0.12.9b7/src/mplfinance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 21:13:00.000000 mplfinance-0.12.9b7/src/mplfinance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-08 21:13:00.000000 mplfinance-0.12.9b7/src/mplfinance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-08 21:13:00.000000 mplfinance-0.12.9b7/src/mplfinance.egg-info/top_level.txt
```

### Comparing `mplfinance-0.12.9b5/LICENSE` & `mplfinance-0.12.9b7/LICENSE`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/PKG-INFO` & `mplfinance-0.12.9b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplfinance
-Version: 0.12.9b5
+Version: 0.12.9b7
 Summary: Utilities for the visualization, and visual analysis, of financial data
 Home-page: http://github.com/matplotlib/mplfinance
 Author: MPL Developers
 Author-email: matplotlib-users@python.org
 Maintainer-email: dgoldfarb.github@gmail.com
 License: BSD-style
 Keywords: finance,candlestick,ohlc,market,investing,technical analysis
```

### Comparing `mplfinance-0.12.9b5/README.md` & `mplfinance-0.12.9b7/README.md`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/setup.py` & `mplfinance-0.12.9b7/setup.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_arg_validators.py` & `mplfinance-0.12.9b7/src/mplfinance/_arg_validators.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_helpers.py` & `mplfinance-0.12.9b7/src/mplfinance/_helpers.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_kwarg_help.py` & `mplfinance-0.12.9b7/src/mplfinance/_kwarg_help.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     dividers = []
     for col in df.columns:
         dividers.append('-'*int(df[col].str.len().max()))
     dfd = pd.DataFrame(dividers).T
     dfd.columns = df.columns
     dfd.index = pd.Index(['---'])
 
-    df = dfd.append(df)
+    df = pd.concat([dfd,df])
 
     formatters = { 'Kwarg'       : make_left_formatter( klen ),
                    'Default'     : make_left_formatter( dlen ),
                    'Description' : make_left_formatter( wraplen ),
                  }
     
     print('\n ','-'*78)
```

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_mpf_warnings.py` & `mplfinance-0.12.9b7/src/mplfinance/_mpf_warnings.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_mplrcputils.py` & `mplfinance-0.12.9b7/src/mplfinance/_mplrcputils.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_mplwraps.py` & `mplfinance-0.12.9b7/src/mplfinance/_mplwraps.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_panels.py` & `mplfinance-0.12.9b7/src/mplfinance/_panels.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/__init__.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/__init__.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/binance.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/binance.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/blueskies.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/blueskies.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/brasil.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/brasil.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/charles.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/charles.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/checkers.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/checkers.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/classic.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/classic.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/default.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/default.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/ibd.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/ibd.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/kenan.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/kenan.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/mike.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/mike.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/nightclouds.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/nightclouds.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/starsandstripes.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/starsandstripes.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styledata/yahoo.py` & `mplfinance-0.12.9b7/src/mplfinance/_styledata/yahoo.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_styles.py` & `mplfinance-0.12.9b7/src/mplfinance/_styles.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,22 @@
     '''
     return copy.deepcopy(_styles[style])
 
 def _apply_mpfstyle(style):
 
     plt.style.use('default')
 
-    if style['base_mpl_style'] is not None:
+    if style['base_mpl_style'] == 'seaborn-darkgrid':
+        # deal with deprecation of old seaborn-darkgrid:
+        try:
+            plt.style.use('seaborn-v0_8-darkgrid')
+            style['base_mpl_style'] = 'seaborn-v0_8-darkgrid'
+        except:
+            plt.style.use(style['base_mpl_style']) 
+    elif style['base_mpl_style'] is not None:
         plt.style.use(style['base_mpl_style']) 
 
     if style['rc'] is not None:
         plt.rcParams.update(style['rc'])
 
     if style['facecolor'] is not None:
         plt.rcParams.update({'axes.facecolor' : style['facecolor'] })
```

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_utils.py` & `mplfinance-0.12.9b7/src/mplfinance/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,16 +101,16 @@
         collections = _construct_ohlc_collections(xdates, opens, highs, lows, closes,
                                                   marketcolors=style['marketcolors'],config=config )
     elif ptype == 'renko':
         collections = _construct_renko_collections(
             dates, highs, lows, volumes, config['renko_params'], closes, marketcolors=style['marketcolors'])
 
     elif ptype == 'pnf':
-        collections = _construct_pointnfig_collections(
-            dates, highs, lows, volumes, config['pnf_params'], closes, marketcolors=style['marketcolors'])
+        raise ValueError('Plot type="pnf" should no longer come this way!')
+
     else:
         raise TypeError('Unknown ptype="',str(ptype),'"')
 
     return collections
 
 
 def _calculate_atr(atr_length, highs, lows, closes):
@@ -411,29 +411,59 @@
         "Default"      - The default value for the kwarg if none is specified.
         "Description"  - The description for the kwarg.
         "Validator"    - A function that takes the caller specified value for the kwarg,
                          and validates that it is the correct type, and (for kwargs with
                          a limited set of allowed values) may also validate that the
                          kwarg value is one of the allowed values.
     '''
+    def _box_size_validator(v):
+        if isinstance(v,(float,int)): return True
+        if v == 'atr': return True
+        if ( isinstance(v,str) and
+             v[-1:] == '%'     and
+             v[:-1].replace('.','',1).isdigit()
+           ) : return True
+        return False
+
     vkwargs = {
-        'box_size'    : { 'Default'     : 'atr',
-                          'Description' : 'size of each box on y-axis (typically price).'+
-                                          ' specify a number, or specify "atr" for average true range.',
-                          'Validator'   : lambda value: isinstance(value,(float,int))
-                                                        or value == 'atr' },
-        'atr_length'  : { 'Default'     : 14,
-                          'Description' : 'number of periods for atr calculation (if box size is "atr")',
-                          'Validator'   : lambda value: isinstance(value,int)
+        'box_size'     : { 'Default'     : 'atr',
+                           'Description' : 'size of each box on y-axis (typically price).'+
+                                           ' specify a number, or "atr" for average true range'+
+                                           ' or a string containing a number and "%" for'+
+                                           ' percent of the most recent close price.',
+                           'Validator'   : lambda value: _box_size_validator(value) },
+        'atr_length'   : { 'Default'     : 'total',
+                           'Description' : 'number of periods for atr calculation (if box size is "atr")',
+                           'Validator'   : lambda value: isinstance(value,int)
                                                         or value == 'total' },
 
-        'reversal'    : { 'Default'     : 1,
-                          'Description' : 'number of boxes, in opposite direction, needed to reverse'+
-                                          ' a trend (i.e. to start a new column).',
-                          'Validator'   : lambda value: isinstance(value,int) },
+        'reversal'     : { 'Default'     : 3,
+                           'Description' : 'number of boxes, in opposite direction, needed to reverse'+
+                                           ' a trend (i.e. to start a new column).',
+                           'Validator'   : lambda value: isinstance(value,int) },
+
+        'method'       : { 'Default'     : 'hilo',
+                           'Description' : 'pricing method:'+
+                                           ' specify "hilo" to use High for X and Low for O'+
+                                           ' or specify "open" or "close" to use only Open or only Close price.',
+                           'Validator'   : lambda value: value in ['hilo','open','close']},
+
+        'use_candle_colors': { 'Default' : False,
+                           'Description' : 'use same colors as candles for given style'+
+                                           ' (instead of PNF colors derived from candle colors).',
+                           'Validator'   : lambda value: isinstance(value,bool) },
+
+        'scale_markers': { 'Default'     : 1.0,
+                           'Description' : 'Scale PNF markers larger ( > 1.0) or smaller ( < 1.0)',
+                           'Validator'   : lambda value: isinstance(value,(int,float)) },
+
+        'scale_right_padding': {'Default': 1.0,
+                           'Description' : 'Scale the amount of padding on the right side'+
+                                           ' of the plot. (Padding helps the PnF remain square',
+                           'Validator'   : lambda value: isinstance(value,(int,float)) },
     }
 
     _validate_vkwargs_dict(vkwargs)
 
     return vkwargs
 
 
@@ -827,15 +857,14 @@
     renko_params = _process_kwargs(config_renko_params, _valid_renko_kwargs())
     if marketcolors is None:
         marketcolors = _get_mpfstyle('classic')['marketcolors']
 
     brick_size = renko_params['brick_size']
     atr_length = renko_params['atr_length']
 
-
     if brick_size == 'atr':
         if atr_length == 'total':
             brick_size = _calculate_atr(len(closes)-1, highs, lows, closes)
         else:
             brick_size = _calculate_atr(atr_length, highs, lows, closes)
     else: # is an integer or float
         upper_limit = (max(closes) - min(closes)) / 2
@@ -930,257 +959,14 @@
                                     edgecolors=edge_colors,
                                     linewidths=lw
                                     )
     calculated_values = dict(dates=new_dates,volumes=new_volumes,
                              values=brick_values,size=brick_size)
     return [rectCollection,], calculated_values
 
-
-def _construct_pointnfig_collections(dates, highs, lows, volumes, config_pointnfig_params, closes, marketcolors=None):
-    """Represent the price change with Xs and Os
-
-    NOTE: this code assumes if any value open, low, high, close is
-    missing they all are missing
-
-    Algorithm Explanation
-    ---------------------
-    In the first part of the algorithm, we populate the boxes array
-    along with adjusting the dates and volumes arrays into the new_dates and
-    new_volumes arrays. A single date includes a range from no boxes to many
-    boxes, if a date has no boxes it shall not be included in new_dates,
-    and if it has n boxes then it will be included n times. Volumes use a
-    volume cache to save volume amounts for dates that do not have any boxes
-    before adding the cache to the next date that has at least one box.
-    We populate the boxes array with each close values difference from the
-    previously created brick divided by the box size.
-
-    The second part of the algorithm has a series of step. First we combine the
-    adjacent like signed values in the boxes array (ex. [-1, -2, 3, -4] -> [-3, 3, -4]).
-    Next we subtract 1 from the absolute value of each element in boxes except the
-    first to ensure every time there is a trend change (ex. previous box is
-    an X, current brick is a O) we draw one less box to account for the price
-    having to move the previous box's amount before creating a box in the
-    opposite direction. During this same step we also combine like signed elements
-    and associated volume/date data ignoring any zero values that are created by
-    subtracting 1 from the box value. Next we recreate the box array utilizing a
-    rolling_change and volume_cache to store and sum the changes that don't break
-    the reversal threshold.
-
-    Lastly, we enumerate through the boxes to populate the line_seg and circle_patches
-    arrays. line_seg holds the / and \ line segments that make up an X and
-    circle_patches holds matplotlib.patches Ellipse objects for each O. We start
-    by filling an x and y array each iteration which contain the x and y
-    coordinates for each box in the column. Then for each coordinate pair in
-    x, y we add to either the line_seg array or the circle_patches array
-    depending on the value of sign for the current column (1 indicates
-    line_seg, -1 indicates circle_patches). The height of the boxes take
-    into account padding which separates each box by a small margin in
-    order to increase readability.
-
-    Useful sources:
-    https://stackoverflow.com/questions/8750648/point-and-figure-chart-with-matplotlib
-    https://www.investopedia.com/articles/technical/03/081303.asp
-
-    Parameters
-    ----------
-    dates : sequence
-        sequence of dates
-    highs : sequence
-        sequence of high values
-    lows : sequence
-        sequence of low values
-    config_pointnfig_params : kwargs table (dictionary)
-        box_size : size of each box
-        atr_length : length of time used for calculating atr
-    closes : sequence
-        sequence of closing values
-    marketcolors : dict of colors: up, down, edge, wick, alpha
-
-    Returns
-    -------
-    ret : tuple
-        rectCollection
-    """
-    pointnfig_params = _process_kwargs(config_pointnfig_params, _valid_pnf_kwargs())
-    if marketcolors is None:
-        marketcolors = _get_mpfstyle('classic')['marketcolors']
-
-    box_size = pointnfig_params['box_size']
-    atr_length = pointnfig_params['atr_length']
-    reversal = pointnfig_params['reversal']
-
-    if box_size == 'atr':
-        if atr_length == 'total':
-            box_size = _calculate_atr(len(closes)-1, highs, lows, closes)
-        else:
-            box_size = _calculate_atr(atr_length, highs, lows, closes)
-    else: # is an integer or float
-        upper_limit = (max(closes) - min(closes)) / 2
-        lower_limit = 0.01 * _calculate_atr(len(closes)-1, highs, lows, closes)
-        if box_size > upper_limit:
-            raise ValueError("Specified box_size may not be larger than (50% of the close price range of the dataset) which has value: "+ str(upper_limit))
-        elif box_size < lower_limit:
-            raise ValueError("Specified box_size may not be smaller than (0.01* the Average True Value of the dataset) which has value: "+ str(lower_limit))
-
-    if reversal < 1 or reversal > 9:
-        raise ValueError("Specified reversal must be an integer in the range [1,9]")
-
-    alpha  = marketcolors['alpha']
-
-    uc     = mcolors.to_rgba(marketcolors['ohlc'][ 'up' ], alpha)
-    dc     = mcolors.to_rgba(marketcolors['ohlc']['down'], alpha)
-    tfc    = mcolors.to_rgba(marketcolors['edge']['down'], 0) # transparent face color
-
-    boxes = [] # each element in an integer representing the number of boxes to be drawn on that indexes column (negative numbers -> Os, positive numbers -> Xs)
-    prev_close_box = closes[0] # represents the value of the last box in the previous column
-    volume_cache = 0 # holds the volumes for the dates that were skipped
-    temp_volumes, temp_dates = [], [] # holds the temp adjusted volumes and dates respectively
-
-    for i in range(len(closes)-1):
-        box_diff = int((closes[i+1] - prev_close_box) / box_size)
-        if box_diff == 0:
-            if volumes is not None:
-                volume_cache += volumes[i]
-            continue
-
-        boxes.append(box_diff)
-        if volumes is not None:
-            temp_volumes.append(volumes[i] + volume_cache)
-            volume_cache = 0
-        temp_dates.append(dates[i])
-        prev_close_box += box_diff *box_size
-
-    # combine adjacent similarly signed differences
-    boxes, indexes = combine_adjacent(boxes)
-    new_volumes, new_dates = coalesce_volume_dates(temp_volumes, temp_dates, indexes)
-
-    adjusted_boxes = [boxes[0]]
-    temp_volumes, temp_dates = [new_volumes[0]], [new_dates[0]]
-    volume_cache = 0
-
-    # Clean data to subtract 1 from all box # not including the first boxes element and combine like signed adjacent values (after ignoring zeros)
-    for i in range(1, len(boxes)):
-        adjusted_value = boxes[i]- int((boxes[i]/abs(boxes[i])))
-
-        # not equal to 0 and different signs
-        if adjusted_value != 0 and adjusted_boxes[-1]*adjusted_value < 0:
-
-            # Append adjusted_value, volumes, and date to associated lists
-            adjusted_boxes.append(adjusted_value)
-            temp_volumes.append(new_volumes[i] + volume_cache)
-            temp_dates.append(new_dates[i])
-
-            # reset volume_cache once we use it
-            volume_cache = 0
-
-        # not equal to 0 and same signs
-        elif adjusted_value != 0 and adjusted_boxes[-1]*adjusted_value > 0:
-
-            # Add adjusted_value and volume values to last added elements
-            adjusted_boxes[-1] += adjusted_value
-            temp_volumes[-1] += new_volumes[i] + volume_cache
-
-            # reset volume_cache once we use it
-            volume_cache = 0
-
-        else: # adjusted_value == 0
-            volume_cache += new_volumes[i]
-
-    boxes = [adjusted_boxes[0]]
-    new_volumes = [temp_volumes[0]]
-    new_dates = [temp_dates[0]]
-
-    rolling_change = 0
-    volume_cache = 0
-    biggest_difference = 0 # only used for the last column
-
-    #Clean data to account for reversal size (added to allow overriding the default reversal of 1)
-    for i in range(1, len(adjusted_boxes)):
-
-        # Add to rolling_change and volume_cache which stores the box and volume values
-        rolling_change += adjusted_boxes[i]
-        volume_cache += temp_volumes[i]
-
-        # if rolling_change is the same sign as the previous box and the abs value is bigger than the
-        # abs value of biggest_difference then we should replace biggest_difference with rolling_change
-        if rolling_change*boxes[-1] > 0 and abs(rolling_change) > abs(biggest_difference):
-            biggest_difference = rolling_change
-
-        # Add to new list if the rolling change is >= the reversal
-        if abs(rolling_change) >= reversal:
-
-            # if rolling_change is the same sign as the previous # of boxes then combine
-            if rolling_change*boxes[-1] > 0:
-                boxes[-1] += rolling_change
-                new_volumes[-1] += volume_cache
-
-            # otherwise add new box
-            else: # < 0 (== 0 can't happen since neither rolling_change or boxes[-1] can be 0)
-                boxes.append(rolling_change)
-                new_volumes.append(volume_cache)
-                new_dates.append(temp_dates[i])
-
-            # reset rolling_change and volume_cache once we've used them
-            rolling_change = 0
-            volume_cache = 0
-
-            # reset biggest_difference as we start from the beginning every time there is a reversal
-            biggest_difference = 0
-
-    # Adjust the last box column if the left over rolling_change is the same sign as the column
-    boxes[-1] += biggest_difference
-    new_volumes[-1] += volume_cache
-
-    curr_price = closes[0]
-    box_values = [] # y values for the boxes
-    circle_patches = [] # list of circle patches to be used to create the cirCollection
-    line_seg = [] # line segments that make up the Xs
-
-    for index, difference in enumerate(boxes):
-        diff = abs(difference)
-
-        sign = (difference / abs(difference)) # -1 or 1
-        start_iteration = 0 if sign > 0 else 1
-
-        x = [index] * (diff)
-        y = [curr_price + (i * box_size * sign) for i in range(start_iteration, diff+start_iteration)]
-
-        curr_price += (box_size * sign * (diff))
-        box_values.append( y )
-
-        for i in range(len(x)): # x and y have the same length
-            height = box_size * 0.85
-            width = 0.6
-            if height < 0.5:
-                width = height
-
-            padding = (box_size * 0.075)
-            if sign == 1: # X
-                line_seg.append([(x[i]-width/2, y[i] + padding), (x[i]+width/2, y[i]+height + padding)]) # create / part of the X
-                line_seg.append([(x[i]-width/2, y[i]+height+padding), (x[i]+width/2, y[i]+padding)]) # create \ part of the X
-            else: # O
-                circle_patches.append(Ellipse((x[i], y[i]-(height/2) - padding), width, height))
-
-    useAA = 0,    # use tuple here
-    lw = 0.5
-
-    cirCollection = PatchCollection(circle_patches)
-    cirCollection.set_facecolor([tfc] * len(circle_patches))
-    cirCollection.set_edgecolor([dc] * len(circle_patches))
-
-    xCollection = LineCollection(line_seg,
-                                 colors=[uc] * len(line_seg),
-                                 linewidths=lw,
-                                 antialiaseds=useAA
-                                 )
-    calculated_values = dict(dates=new_dates,counts=boxes,values=box_values,
-                             volumes=new_volumes,size=box_size)
-    return [cirCollection, xCollection], calculated_values
-
-
 def _construct_aline_collections(alines, dtix=None):
     """construct arbitrary line collections
 
     Parameters
     ----------
     alines : sequence
         sequences of segments, which are sequences of lines,
@@ -1509,7 +1295,296 @@
             else:
                 marker_obj = mmarkers.MarkerStyle(marker)
             path = marker_obj.get_path().transformed(
                         marker_obj.get_transform())
             paths.append(path)
         sc.set_paths(paths)
     return sc
+
+
+def _pnf_calculator(indf,boxsize,reverse=3,method='hilo'):
+    '''Calculate Point and Figure Numbers
+
+    TODO: Support arbitrary column names of OHLC
+    '''
+    
+    def round_to(n, precision):
+        correction = 0.5 if n >= 0 else -0.5
+        return int( (n/precision)+correction ) * precision
+
+    # indf = df.copy()[df.columns.values]
+    
+    # suppliment data with the "box" that each row of data falls into:
+
+    if method == 'hilo':
+        Xprices = indf.High
+        Oprices = indf.Low
+    elif method == 'open':
+        Xprices = indf.Open
+        Oprices = indf.Open
+    elif method == 'close':
+        Xprices = indf.Close
+        Oprices = indf.Close
+    else:
+        raise ValueError('Bad value for method="'+str(method)+'"')
+    
+    # X Boxes: Round down, i.e. truncate, to boxsize:
+    indf.loc[:,'XBox'] = [(int(x/boxsize))*boxsize for x in Xprices]
+
+    # O Boxes: Round up to boxsize:
+    indf.loc[:,'OBox'] = [(int(round_to((x+(0.5*boxsize)),boxsize)/boxsize))*boxsize for x in Oprices]
+
+    # Initialize First Column:
+
+    # There are a number of ways to decide whether the first column is up (X) or down (O).
+    # Initially I tried something that I saw described online: 
+    # If the first day (period) is an up day (close>open) then make the first column up (X).
+    # The problem with this was sometimes the trend was really the opposite of what the first
+    # day (period) just happened to be.  Next I tried comparing the close of the first two
+    # days.  That had a better shot a being right but still often did not match what I saw
+    # with PnF charts on Bloomberg or Schwab.  Next I tried a "vote" among the first three
+    # days, seeing whether each day was an up day (Close>Open) or down day (Open>Close).
+    # Being an odd number of days the "vote" could never be a tie.  This worked quite well
+    # but sometimes did not match Bloomberg.  Finally, after close inspection of the cases
+    # that did not match, I decided to compare the Close of the 3rd day with the Open on the
+    # 1st day.  This technique matched Bloomberg perfectly for all of the approximately ten
+    # cases that I tested:
+
+    v = indf.iloc[2].Close - indf.iloc[0].Open
+    xo = 'X' if v > 0 else 'O' 
+
+    d0 = indf.index[0]
+    if xo == 'X':
+        column = [indf.OBox[d0]-boxsize]
+    else:
+        column = [indf.XBox[d0]+boxsize]
+    xo
+    pnf = {}
+    pnf[d0] = column
+    
+    # HERE STARTS THE MAIN LOOP:
+    
+    column_count   = 1
+    current_column = pnf[d0]
+    for d in indf.index[1:]:
+        current_level = current_column[-1]
+        new_column    = []
+        if xo == 'X':
+            box = indf.XBox[d]
+            reverse = current_level - 3*boxsize        
+            if box > current_level:
+               #print(xo,d,'curlev=',current_level,'box=',box,'num=',num)
+               #print(xo,d,'current_column.1=',current_column)
+                num = int(round((box-current_level)/boxsize))
+                for jj in range(1,num+1):
+                    current_column.append(current_level+(jj*boxsize))
+               #print(xo,d,'current_column.2=',current_column)
+            elif indf.OBox[d] <= reverse:
+                top = current_level - boxsize
+                box = indf.OBox[d]
+                num = int(round((top-box)/boxsize))
+                new_column = [top]
+                for jj in range(1,num+1):
+                    new_column.append(top-(jj*boxsize))
+                pnf[d] = new_column
+                xo = 'O'
+                current_column = new_column
+                column_count += 1
+        else: # xo = 'O'
+            box = indf.OBox[d]
+            #print('d=',d,'box=',box,'current_level=',current_level)
+            reverse = current_level + 3*boxsize
+            if round_to(box,1.0*boxsize) < current_level:
+               #print(xo,d,'curlev=',current_level,'box=',box,'num=',num)
+               #print(xo,d,'current_column.1=',current_column)
+                num = int(round((current_level-box)/boxsize))
+                for jj in range(1,num+1):
+                    current_column.append(current_level-(jj*boxsize))
+               #print(xo,d,'current_column.2=',current_column)
+            elif indf.XBox[d] >= reverse:
+                bot = current_level + boxsize
+                box = indf.XBox[d]
+                num = int(round((box-bot)/boxsize))
+                new_column = [bot]
+                for jj in range(1,num+1):
+                    new_column.append(bot+(jj*boxsize))
+                pnf[d] = new_column
+                xo = 'X'
+                current_column = new_column
+                column_count += 1
+        #print('d=',d,'reverse=',reverse)
+        #if column_count > 4:
+        #    break
+    return pnf
+
+def _construct_pnf_scatter(ax,ptype,dates,xdates,opens,highs,lows,closes,volumes,config,style):
+    """Represent the price change with Xs and Os
+
+    NOTE: this code assumes if any value open, low, high, close is
+    missing they all are missing
+
+    Algorithm Explanation
+    ---------------------
+    In the first part of the algorithm ...
+
+    Useful sources:
+    https://...
+    https://...
+
+    Parameters
+    ----------
+    dates : sequence
+        sequence of dates
+    highs : sequence
+        sequence of high values
+    lows : sequence
+        sequence of low values
+    config_pointnfig_params : kwargs table (dictionary)
+        box_size : size of each box
+        atr_length : length of time used for calculating atr
+    closes : sequence
+        sequence of closing values
+    marketcolors : dict of colors: up, down, edge, wick, alpha
+
+    Returns
+    -------
+    calculate_values : dict of assorted point-and-figure box calculation results
+    """
+
+    # Put the data into a dataframe so easier to work with.
+    # Someday we may change mplfinance in general to keep the input data in a dataframe.
+    df = pd.DataFrame(dict(Open=opens,High=highs,Low=lows,Close=closes,Volume=volumes))
+    if config['tz_localize']:
+        df.index = pd.DatetimeIndex(mdates.num2date(dates)).tz_localize(None)
+    else:
+        df.index = pd.DatetimeIndex(mdates.num2date(dates))
+    df.index.name = 'Date'
+
+    marketcolors=style['marketcolors']
+    if marketcolors is None:
+        marketcolors = _get_mpfstyle('classic')['marketcolors']
+
+    pointnfig_params = _process_kwargs(config['pnf_params'], _valid_pnf_kwargs())
+
+    box_size   = pointnfig_params['box_size']
+    atr_length = pointnfig_params['atr_length']
+    reversal   = pointnfig_params['reversal']
+    method     = pointnfig_params['method']
+
+    if box_size == 'atr':
+        if atr_length == 'total':
+            box_size = _calculate_atr(len(closes)-1, df.High, df.Low, df.Close)
+        else:
+            box_size = _calculate_atr(atr_length, df.High, df.Low, df.Close)
+    elif isinstance(box_size,str) and box_size[-1] == '%':
+        percent  = float(box_size[:-1])
+        if not (percent > 0 and percent < 50) :
+            raise ValueError("Specified percent (for box_size) must be > 0. and < 50.")
+        box_size = (percent/100.) * df.Close.iloc[-1] # percent of last close
+    else: # is an integer or float
+        upper_limit = (max(df.Close) - min(df.Close)) / 2
+        lower_limit = 0.01 * _calculate_atr(len(df.Close)-1, df.High, df.Low, df.Close)
+        if box_size > upper_limit:
+            raise ValueError("Specified box_size may not be larger than [50% of the close"+
+                             " price range of the dataset] which has value: "+ str(upper_limit))
+        elif box_size < lower_limit:
+            raise ValueError("Specified box_size may not be smaller than [0.01* the Average"+
+                             " True Value of the dataset) which has value: "+ str(lower_limit))
+
+    if reversal < 1 or reversal > 9:
+        raise ValueError("Specified reversal must be an integer in the range [1,9]")
+
+
+    pnfd = _pnf_calculator(df,boxsize=box_size,reverse=reversal,method=method)
+
+    yvals = [y for key in pnfd.keys() for y in pnfd[key] ]
+
+    # yval is the bottom of the box:
+    ylim_top = max(yvals) + 0.5*box_size
+    ylim_bot = min(yvals) - 0.5*box_size
+
+    # Attempt to calculate the ideal marker size:
+    dpi = ax.figure.get_dpi()
+    wxt = ax.get_window_extent()
+
+    axis_height_inches = wxt.height / dpi
+    max_vertical_boxes = (ylim_top - ylim_bot) / box_size
+    inches_per_box     = axis_height_inches / max_vertical_boxes
+    ideal_marker_size  = (inches_per_box*72) ** 2  # 72 points per inch, square for area.
+    ideal_marker_size  *= 0.6 # kludgey adjustment (should have worked without??)
+    marker_size        = ideal_marker_size * pointnfig_params['scale_markers']
+
+    alpha  = marketcolors['alpha']
+
+    if pointnfig_params['use_candle_colors']:
+        uc = mcolors.to_rgba(marketcolors['candle'][ 'up' ], alpha)
+        ue = mcolors.to_rgba(marketcolors['edge']['up'])#, alpha) 
+        uw = 0.5
+        dc = mcolors.to_rgba(marketcolors['candle']['down'], alpha)
+        de = mcolors.to_rgba(marketcolors['edge']['up'])#, alpha)
+        dw = 0.5
+    else:
+        uc = mcolors.to_rgba(marketcolors['edge']['up'], alpha)
+        ue = mcolors.to_rgba(marketcolors['edge']['up'], alpha)
+        uw = 0.5
+        dc = mcolors.to_rgba(marketcolors['candle']['down'], 0.0)
+        de = mcolors.to_rgba(marketcolors['candle']['down'], alpha)
+        dw = 0.18*(marker_size**0.5) # empirical "guess"
+        #print('dw=',dw)
+
+    xvals = []
+    yvals = []
+    mvals = []
+    cvals = []
+    evals = []
+    lwids = []
+    jj = 0
+    for key in pnfd.keys():
+
+        m = 'X' if pnfd[key][0] < pnfd[key][-1] else 'o'  # marker
+        c = uc  if pnfd[key][0] < pnfd[key][-1] else dc   # color
+        e = ue  if pnfd[key][0] < pnfd[key][-1] else de   # edge color
+        w = uw  if pnfd[key][0] < pnfd[key][-1] else dw   # edge width
+
+        for v in pnfd[key]:
+            yvals.append(v)
+            xvals.append(jj)
+            mvals.append(m)
+            evals.append(e)
+            cvals.append(c)
+            lwids.append(w)
+        jj += 1
+
+    plot_yvals = [y+(0.5*box_size) for y in yvals] # adjust so marker is _in_ the box.
+
+    _ = _mscatter(xvals,plot_yvals,ax,mvals,s=marker_size,c=cvals,linewidths=lwids,edgecolors=evals)
+
+    if config['volume'] is not None:
+        pnf_volumes = []
+        d1list = [d for d in pnfd.keys()]
+        d2list = d1list[1:] + [df.index[-1],]
+        for d1,d2 in zip(d1list,d2list):
+            pnf_volumes.append(df.Volume.loc[d1:d2].sum())
+    else:
+        pnf_volumes = [0]*len(xvals)
+
+    # make the length of the x-axis approximately equal to the total 
+    # number of vertical boxes, so the boxes are approximately square:
+    hi   = max(yvals)
+    lo   = min(yvals)
+    xlen = int(round((hi-lo)/box_size,0)+2) # +2 empirical kludge
+    pad  = (xlen-xvals[-1]) * pointnfig_params['scale_right_padding']
+    pad  = max(0,pad) # less than zero not allowed
+    #print('hi,lo,xlen,xvals[-1],pad=',hi,lo,xlen,xvals[-1],pad)
+    #print('ylim_top,ylim_bot=',ylim_top,ylim_bot)
+
+    xdates = np.arange(len(pnfd)+int(pad))
+    pnf_volumes = pnf_volumes + [float('nan')]*int(pad)
+
+    pnf_results = dict(pnf_volumes=pnf_volumes,
+                       pnf_ylimits=(ylim_bot,ylim_top),
+                       pnf_values=pnfd,
+                       pnf_df=df,
+                       pnf_boxsize=box_size,
+                       pnf_xdates=xdates)
+
+    return pnf_results
```

### Comparing `mplfinance-0.12.9b5/src/mplfinance/_widths.py` & `mplfinance-0.12.9b7/src/mplfinance/_widths.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/original_flavor.py` & `mplfinance-0.12.9b7/src/mplfinance/original_flavor.py`

 * *Files identical despite different names*

### Comparing `mplfinance-0.12.9b5/src/mplfinance/plotting.py` & `mplfinance-0.12.9b7/src/mplfinance/plotting.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #register_matplotlib_converters()
 
 from mplfinance._utils import _construct_aline_collections
 from mplfinance._utils import _construct_hline_collections
 from mplfinance._utils import _construct_vline_collections
 from mplfinance._utils import _construct_tline_collections
 from mplfinance._utils import _construct_mpf_collections
+from mplfinance._utils import _construct_pnf_scatter
 
 from mplfinance._widths import _determine_width_config
 
 from mplfinance._utils import _updown_colors
 from mplfinance._utils import IntegerIndexDateTimeFormatter
 from mplfinance._utils import _mscatter
 from mplfinance._utils import _check_and_convert_xlim_configuration
@@ -522,62 +523,78 @@
     if isinstance(rwc,dict) and len(rwc)==0:
         config['return_width_config'].update(config['_width_config'])
 
     collections = None
     if ptype == 'line':
         lw = config['_width_config']['line_width']
         axA1.plot(xdates, closes, color=config['linecolor'], linewidth=lw)
+    elif ptype == 'pnf':
+        pnf_results = _construct_pnf_scatter(axA1,ptype,dates,xdates,opens,highs,lows,closes,volumes,config,style)
     else:
         collections =_construct_mpf_collections(ptype,dates,xdates,opens,highs,lows,closes,volumes,config,style)
 
-    if ptype in VALID_PMOVE_TYPES:
-        collections, calculated_values = collections
-        volumes       = calculated_values['volumes']
-        pmove_dates   = calculated_values['dates']
-        pmove_values  = calculated_values['values']
-        if all([isinstance(v,(list,tuple)) for v in pmove_values]):
-            pmove_avgvals = [sum(v)/len(v) for v in pmove_values]
-        else:
-            pmove_avgvals = pmove_values
-        pmove_size    = calculated_values['size']
-        pmove_counts  = calculated_values['counts'] if 'counts' in calculated_values else None
-        formatter = IntegerIndexDateTimeFormatter(pmove_dates, fmtstring)
-        xdates = np.arange(len(pmove_dates))
+    if ptype == 'pnf':
+        volumes    = pnf_results['pnf_volumes']
+        pnf_values = pnf_results['pnf_values']
+        pnf_mdates = mdates.date2num(list(pnf_values.keys()))
+        formatter  = IntegerIndexDateTimeFormatter(pnf_mdates,fmtstring)
+        xdates     = pnf_results['pnf_xdates']
+    elif ptype == 'renko':
+        collections, renko_results = collections
+        volumes       = renko_results['volumes']
+        renko_dates   = renko_results['dates']
+        renko_values  = renko_results['values']
+        formatter = IntegerIndexDateTimeFormatter(renko_dates, fmtstring)
+        renko_avgvals = renko_values
+        renko_size    = renko_results['size']
+        xdates = np.arange(len(renko_dates))
 
     if collections is not None:
         for collection in collections:
             axA1.add_collection(collection)
 
-    if ptype in VALID_PMOVE_TYPES:
-        mavprices = _plot_mav(axA1,config,xdates,pmove_avgvals)
-        emaprices = _plot_ema(axA1, config, xdates, pmove_avgvals)
+    #formatter = IntegerIndexDateTimeFormatter(xdates, fmtstring)
+
+    if (ptype == 'pnf' and 
+        (config['mav'] is not None or config['ema'] is not None)):
+        warnings.warn('\n\n ================================================================ '+
+                      '\n\n   MOVING Averages IGNORED for POINT and FIGURE PLOTS!'+
+                      '\n\n ================================================================ ',
+                      category=UserWarning)
+    elif ptype == 'renko':
+        mavprices = _plot_mav(axA1,config,xdates,renko_avgvals)
+        emaprices = _plot_ema(axA1,config,xdates,renko_avgvals)
     else:
         mavprices = _plot_mav(axA1,config,xdates,closes)
-        emaprices = _plot_ema(axA1, config, xdates, closes)
+        emaprices = _plot_ema(axA1,config,xdates,closes)
 
     avg_dist_between_points = (xdates[-1] - xdates[0]) / float(len(xdates))
     if not config['tight_layout']:
         minx = xdates[0]  - avg_dist_between_points
         maxx = xdates[-1] + avg_dist_between_points
     else:
         minx = xdates[0]  - (0.45 * avg_dist_between_points)
         maxx = xdates[-1] + (0.45 * avg_dist_between_points)
 
     if len(xdates) == 1:  # kludge special case
         minx = minx - 0.75
         maxx = maxx + 0.75
-    if ptype not in VALID_PMOVE_TYPES:
+
+    if ptype == 'renko':
+        _lows  = renko_avgvals 
+        _highs = [value+renko_size for value in renko_avgvals]
+    else:
         _lows  = lows
         _highs = highs
-    else:
-        _lows  = pmove_avgvals
-        _highs = [value+pmove_size for value in pmove_avgvals]
 
-    miny = np.nanmin(_lows)
-    maxy = np.nanmax(_highs)
+    if ptype == 'pnf':
+       miny, maxy = pnf_results['pnf_ylimits']
+    else:
+        miny = np.nanmin(_lows)
+        maxy = np.nanmax(_highs)
 
     if config['ylim'] is not None:
         axA1.set_ylim(config['ylim'][0], config['ylim'][1])
     elif config['tight_layout']:
         ydelta = 0.01 * (maxy-miny)
         if miny > 0.0:
             # don't let it go negative:
@@ -596,47 +613,46 @@
         not config['tight_layout']):
         corners = (minx, miny), (maxx, maxy)
         axA1.update_datalim(corners)
 
     if config['return_calculated_values'] is not None:
         retdict = config['return_calculated_values']
         if ptype == 'renko':
-            retdict['renko_bricks' ] = pmove_values
-            retdict['renko_dates'  ] = mdates.num2date(pmove_dates)
-            retdict['renko_size'   ] = pmove_size
+            retdict['renko_bricks' ] = renko_values
+            retdict['renko_dates'  ] = mdates.num2date(renko_dates)
+            retdict['renko_size'   ] = renko_size
             retdict['renko_volumes'] = volumes if config['volume'] else None
         elif ptype == 'pnf':
-            retdict['pnf_dates'    ] = mdates.num2date(pmove_dates)
-            retdict['pnf_counts'   ] = pmove_counts
-            retdict['pnf_values'   ] = pmove_values
-            retdict['pnf_avgvals'  ] = pmove_avgvals
-            retdict['pnf_size'     ] = pmove_size
-            retdict['pnf_volumes'  ] = volumes if config['volume'] else None
-        if config['mav'] is not None:
+            retdict['pnf_dates'    ] = mdates.num2date(pnf_mdates)
+            retdict['pnf_values'   ] = pnf_values
+            retdict['pnf_size'     ] = pnf_results['pnf_boxsize']
+            retdict['pnf_volumes'  ] = volumes[:len(pnf_values)] if config['volume'] else None
+        if config['mav'] is not None and ptype != 'pnf':
             mav = config['mav']
             if len(mav) != len(mavprices):
                 warnings.warn('len(mav)='+str(len(mav))+' BUT len(mavprices)='+str(len(mavprices)))
             else:
                 for jj in range(0,len(mav)):     
                     retdict['mav' + str(mav[jj])] = mavprices[jj]
-        if config['ema'] is not None:
+        if config['ema'] is not None and ptype != 'pnf':
             ema = config['ema']
             if len(ema) != len(emaprices):
                 warnings.warn('len(ema)='+str(len(ema))+' BUT len(emaprices)='+str(len(emaprices)))
             else:
                 for jj in range(0, len(ema)):
                     retdict['ema' + str(ema[jj])] = emaprices[jj]
         retdict['minx'] = minx
         retdict['maxx'] = maxx
         retdict['miny'] = miny
         retdict['maxy'] = maxy
 
     # Note: these are NOT mutually exclusive, so the order of this
     #       if/elif is important: VALID_PMOVE_TYPES must be first.
     if ptype in VALID_PMOVE_TYPES:
+        pmove_dates = pnf_mdates if ptype == 'pnf' else renko_dates
         dtix = pd.DatetimeIndex([dt for dt in mdates.num2date(pmove_dates)])
     elif not config['show_nontrading']:
         dtix = data.index
     else:
         dtix = None
 
     line_collections = []
@@ -682,14 +698,26 @@
         _set_ticks_on_bottom_panel_only(panels,formatter,rotation=xrotation,
                                         xlabel=config['xlabel'])
     else:
         axA1.tick_params(axis='x',rotation=xrotation)
         axA1.xaxis.set_major_formatter(formatter)
         axA1.set_xlabel(config['xlabel'])
 
+    if config['type'] == 'pnf':
+        pnf_xs = list(pnf_results['pnf_df'].XBox.values)
+        pnf_os = list(pnf_results['pnf_df'].OBox.values)
+        tick_vals = sorted( set(pnf_xs + pnf_os) )
+        axA1.set_yticks(tick_vals)
+        skip = int( round(len(xdates)/10.0, 0) )
+        skip = max(1,skip) # must be at least 1
+        tick_vals = [t for t in range(0-skip,len(xdates)+1,skip)]
+        #print('len(xdates)=',len(xdates),'len(pnf_mdates)=',len(pnf_mdates))
+        #print('skip=',skip,'\nxdates=',xdates,'\npnf_dates=',[str(d.date()) for d in mdates.num2date(pnf_mdates)])
+        axA1.set_xticks(tick_vals)
+
     ysd = config['yscale']
     if isinstance(ysd,dict):
         yscale = ysd['yscale']
         del      ysd['yscale']
         axA1.set_yscale(yscale,**ysd)
     elif isinstance(ysd,str):
         axA1.set_yscale(ysd)
```

### Comparing `mplfinance-0.12.9b5/src/mplfinance.egg-info/PKG-INFO` & `mplfinance-0.12.9b7/src/mplfinance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplfinance
-Version: 0.12.9b5
+Version: 0.12.9b7
 Summary: Utilities for the visualization, and visual analysis, of financial data
 Home-page: http://github.com/matplotlib/mplfinance
 Author: MPL Developers
 Author-email: matplotlib-users@python.org
 Maintainer-email: dgoldfarb.github@gmail.com
 License: BSD-style
 Keywords: finance,candlestick,ohlc,market,investing,technical analysis
```

### Comparing `mplfinance-0.12.9b5/src/mplfinance.egg-info/SOURCES.txt` & `mplfinance-0.12.9b7/src/mplfinance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

