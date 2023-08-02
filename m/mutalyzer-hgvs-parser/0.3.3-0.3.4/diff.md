# Comparing `tmp/mutalyzer_hgvs_parser-0.3.3.tar.gz` & `tmp/mutalyzer_hgvs_parser-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mihai/projects/lumc/mutalyzer/hgvs-parser/dist/tmp9bdqhphx/mutalyzer_hgvs_parser-0.3.3.tar", last modified: Mon May  2 16:00:24 2022, max compression
+gzip compressed data, was "mutalyzer_hgvs_parser-0.3.4.tar", last modified: Wed Aug  2 19:22:00 2023, max compression
```

## Comparing `mutalyzer_hgvs_parser-0.3.3.tar` & `mutalyzer_hgvs_parser-0.3.4.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-05-02 16:00:24.177320 mutalyzer_hgvs_parser-0.3.3/
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1089 2020-07-06 17:51:44.000000 mutalyzer_hgvs_parser-0.3.3/LICENSE
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      321 2021-08-18 08:29:22.000000 mutalyzer_hgvs_parser-0.3.3/MANIFEST.in
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3228 2022-05-02 16:00:24.177320 mutalyzer_hgvs_parser-0.3.3/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2590 2021-04-16 07:02:31.000000 mutalyzer_hgvs_parser-0.3.3/README.rst
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-05-02 16:00:24.173320 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      774 2021-08-18 08:29:22.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2531 2022-01-11 12:27:28.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/cli.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    10137 2022-04-11 07:56:25.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/convert.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-05-02 16:00:24.173320 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/ebnf/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      131 2021-08-18 08:29:22.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/ebnf/common.g
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       50 2021-08-18 08:29:22.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/ebnf/description.g
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2029 2022-04-11 08:50:35.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/ebnf/dna.g
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1813 2021-06-10 09:28:15.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/ebnf/hgvs_mutalyzer_3.g
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2018 2021-08-18 08:29:22.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/ebnf/protein.g
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      107 2021-08-18 08:29:22.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/ebnf/reference.g
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       51 2021-08-18 08:29:22.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/ebnf/top.g
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4741 2022-05-02 13:12:55.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/exceptions.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    18285 2022-05-02 15:48:53.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/hgvs_parser.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1224 2021-08-18 08:29:22.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/util.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-05-02 16:00:24.173320 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)     3228 2022-05-02 16:00:23.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser.egg-info/PKG-INFO
--rw-r--r--   0 mihai     (1000) mihai     (1000)      976 2022-05-02 16:00:24.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser.egg-info/SOURCES.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2022-05-02 16:00:23.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser.egg-info/dependency_links.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       73 2022-05-02 16:00:23.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser.egg-info/entry_points.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)        1 2020-07-06 18:09:00.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser.egg-info/not-zip-safe
--rw-r--r--   0 mihai     (1000) mihai     (1000)       27 2022-05-02 16:00:24.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser.egg-info/requires.txt
--rw-r--r--   0 mihai     (1000) mihai     (1000)       28 2022-05-02 16:00:24.000000 mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1264 2022-05-02 16:00:24.177320 mutalyzer_hgvs_parser-0.3.3/setup.cfg
--rw-r--r--   0 mihai     (1000) mihai     (1000)       39 2020-07-06 17:51:44.000000 mutalyzer_hgvs_parser-0.3.3/setup.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-05-02 16:00:24.177320 mutalyzer_hgvs_parser-0.3.3/tests/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2018-07-12 11:18:43.000000 mutalyzer_hgvs_parser-0.3.3/tests/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3181 2022-01-11 13:21:58.000000 mutalyzer_hgvs_parser-0.3.3/tests/test_ambig.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       65 2021-07-08 14:28:54.000000 mutalyzer_hgvs_parser-0.3.3/tests/test_cli.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    30705 2022-05-02 08:05:53.000000 mutalyzer_hgvs_parser-0.3.3/tests/test_convert.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4027 2021-08-18 08:29:22.000000 mutalyzer_hgvs_parser-0.3.3/tests/test_hgvs_parser.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    31937 2021-08-18 08:29:22.000000 mutalyzer_hgvs_parser-0.3.3/tests/test_protein.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    10189 2022-05-02 15:49:09.000000 mutalyzer_hgvs_parser-0.3.3/tests/test_syntax.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-02 19:22:00.592708 mutalyzer_hgvs_parser-0.3.4/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1089 2021-07-09 11:25:18.000000 mutalyzer_hgvs_parser-0.3.4/LICENSE
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      321 2021-07-22 13:16:08.000000 mutalyzer_hgvs_parser-0.3.4/MANIFEST.in
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3208 2023-08-02 19:22:00.592708 mutalyzer_hgvs_parser-0.3.4/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2590 2021-07-09 11:25:18.000000 mutalyzer_hgvs_parser-0.3.4/README.rst
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-02 19:22:00.592708 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      774 2021-07-22 13:16:08.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2531 2023-08-01 09:07:50.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/cli.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    10137 2023-08-01 09:07:50.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/convert.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-02 19:22:00.592708 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/ebnf/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      131 2021-07-22 13:16:08.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/ebnf/common.g
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       50 2021-07-22 13:16:08.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/ebnf/description.g
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2029 2023-08-01 09:07:50.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/ebnf/dna.g
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1813 2021-07-09 11:25:18.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/ebnf/hgvs_mutalyzer_3.g
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2018 2021-07-22 13:16:08.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/ebnf/protein.g
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      107 2021-07-22 13:16:08.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/ebnf/reference.g
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       51 2021-07-22 13:16:08.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/ebnf/top.g
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4741 2023-08-01 09:07:50.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/exceptions.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    28013 2023-08-02 13:11:19.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/hgvs_parser.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1224 2021-07-22 13:16:08.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/util.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-02 19:22:00.592708 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser.egg-info/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3208 2023-08-02 19:22:00.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      958 2023-08-02 19:22:00.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2023-08-02 19:22:00.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       73 2023-08-02 19:22:00.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser.egg-info/entry_points.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2021-07-09 11:26:16.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser.egg-info/not-zip-safe
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       27 2023-08-02 19:22:00.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       28 2023-08-02 19:22:00.000000 mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1264 2023-08-02 19:22:00.592708 mutalyzer_hgvs_parser-0.3.4/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       39 2021-07-09 11:25:18.000000 mutalyzer_hgvs_parser-0.3.4/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-02 19:22:00.592708 mutalyzer_hgvs_parser-0.3.4/tests/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2021-07-09 11:25:18.000000 mutalyzer_hgvs_parser-0.3.4/tests/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3181 2023-08-01 09:07:50.000000 mutalyzer_hgvs_parser-0.3.4/tests/test_ambig.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    33563 2023-08-02 12:57:01.000000 mutalyzer_hgvs_parser-0.3.4/tests/test_convert.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4027 2021-07-22 13:16:08.000000 mutalyzer_hgvs_parser-0.3.4/tests/test_hgvs_parser.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    31937 2021-07-22 13:16:08.000000 mutalyzer_hgvs_parser-0.3.4/tests/test_protein.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    10189 2023-08-01 09:07:50.000000 mutalyzer_hgvs_parser-0.3.4/tests/test_syntax.py
```

### Comparing `mutalyzer_hgvs_parser-0.3.3/LICENSE` & `mutalyzer_hgvs_parser-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/PKG-INFO` & `mutalyzer_hgvs_parser-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mutalyzer_hgvs_parser
-Version: 0.3.3
+Version: 0.3.4
 Summary: Mutalyzer HGVS variant description parser.
 Home-page: https://github.com/mutalyzer/hgvs-parser
 Author: Mihai Lefter
 Author-email: M.Lefter@lumc.nl
 License: MIT
 Keywords: Mutalyzer,HGVS,description,parser,genomic
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: test
@@ -88,9 +87,7 @@
     >>> model['reference']
     {'id': 'NG_012337.1'}
 
 
 Please see ReadTheDocs_ for the latest documentation.
 
 .. _ReadTheDocs: https://mutalyzer-hgvs-parser.readthedocs.io/en/latest/
-
-
```

### Comparing `mutalyzer_hgvs_parser-0.3.3/README.rst` & `mutalyzer_hgvs_parser-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/__init__.py` & `mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/cli.py` & `mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/cli.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/convert.py` & `mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/convert.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/ebnf/dna.g` & `mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/ebnf/dna.g`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/ebnf/hgvs_mutalyzer_3.g` & `mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/ebnf/hgvs_mutalyzer_3.g`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/ebnf/protein.g` & `mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/ebnf/protein.g`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/exceptions.py` & `mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser/util.py` & `mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser/util.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser.egg-info/PKG-INFO` & `mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mutalyzer-hgvs-parser
-Version: 0.3.3
+Version: 0.3.4
 Summary: Mutalyzer HGVS variant description parser.
 Home-page: https://github.com/mutalyzer/hgvs-parser
 Author: Mihai Lefter
 Author-email: M.Lefter@lumc.nl
 License: MIT
 Keywords: Mutalyzer,HGVS,description,parser,genomic
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: test
@@ -88,9 +87,7 @@
     >>> model['reference']
     {'id': 'NG_012337.1'}
 
 
 Please see ReadTheDocs_ for the latest documentation.
 
 .. _ReadTheDocs: https://mutalyzer-hgvs-parser.readthedocs.io/en/latest/
-
-
```

### Comparing `mutalyzer_hgvs_parser-0.3.3/mutalyzer_hgvs_parser.egg-info/SOURCES.txt` & `mutalyzer_hgvs_parser-0.3.4/mutalyzer_hgvs_parser.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,12 +21,11 @@
 mutalyzer_hgvs_parser/ebnf/dna.g
 mutalyzer_hgvs_parser/ebnf/hgvs_mutalyzer_3.g
 mutalyzer_hgvs_parser/ebnf/protein.g
 mutalyzer_hgvs_parser/ebnf/reference.g
 mutalyzer_hgvs_parser/ebnf/top.g
 tests/__init__.py
 tests/test_ambig.py
-tests/test_cli.py
 tests/test_convert.py
 tests/test_hgvs_parser.py
 tests/test_protein.py
 tests/test_syntax.py
```

### Comparing `mutalyzer_hgvs_parser-0.3.3/setup.cfg` & `mutalyzer_hgvs_parser-0.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mutalyzer_hgvs_parser
-version = 0.3.3
+version = 0.3.4
 description = Mutalyzer HGVS variant description parser.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Mihai Lefter
 author_email = M.Lefter@lumc.nl
 url = https://github.com/mutalyzer/hgvs-parser
 keywords = Mutalyzer, HGVS, description, parser, genomic
```

### Comparing `mutalyzer_hgvs_parser-0.3.3/tests/test_ambig.py` & `mutalyzer_hgvs_parser-0.3.4/tests/test_ambig.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/tests/test_convert.py` & `mutalyzer_hgvs_parser-0.3.4/tests/test_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,27 @@
     },
     "*10-20": {
         "type": "point",
         "position": 10,
         "outside_cds": "downstream",
         "offset": {"value": -20},
     },
+    "10-5_10-2": {
+        "type": "range",
+        "start": {
+            "type": "point",
+            "position": 10,
+            "offset": {"value": -5},
+        },
+        "end": {
+            "type": "point",
+            "position": 10,
+            "offset": {"value": -2},
+        },
+    },
     "10_15": {
         "type": "range",
         "start": {"type": "point", "position": 10},
         "end": {"type": "point", "position": 15},
     },
     "(10_15)": {
         "type": "range",
@@ -371,14 +384,15 @@
 
 VARIANTS = {
     "1": {"location": LOCATIONS["1"]},
     "??": {"location": LOCATIONS["??"]},
     "100?": {"location": LOCATIONS["100?"]},
     "10_15": {"location": LOCATIONS["10_15"]},
     "(10_15)": {"location": LOCATIONS["(10_15)"]},
+    "10-5_10-2": {"location": LOCATIONS["10-5_10-2"]},
     # Substitutions
     "10C>A": {
         "type": "substitution",
         "source": "reference",
         "location": LOCATIONS["10"],
         "deleted": [{"sequence": "C", "source": "description"}],
         "inserted": [{"sequence": "A", "source": "description"}],
@@ -566,14 +580,19 @@
         "location": LOCATIONS["-10+20"],
     },
     "-10-20inv": {
         "type": "inversion",
         "source": "reference",
         "location": LOCATIONS["-10-20"],
     },
+    "10-5_10-2inv": {
+        "type": "inversion",
+        "source": "reference",
+        "location": LOCATIONS["10-5_10-2"]
+    },
     # Conversions
     "10_20con40_50": {
         "type": "conversion",
         "source": "reference",
         "location": LOCATIONS["10_20"],
         "inserted": [{"source": "reference", "location": LOCATIONS["40_50"]}],
     },
@@ -910,14 +929,87 @@
     },
     "R1:g.[10_20conR2:40_50;(10_11insA)]": {
         "reference": REFERENCES["R1"],
         "type": "description_dna",
         "coordinate_system": "g",
         "variants": [VARIANTS["10_20conR2:40_50"], VARIANTS["(10_11insA)"]],
     },
+    "R1:c.10-5_10-2": {
+        "reference": REFERENCES["R1"],
+        "type": "description_dna",
+        "coordinate_system": "c",
+        "variants": [VARIANTS["10-5_10-2"]],
+    },
+    "R1:c.10-5_10-2dupR2:10": {
+        "reference": REFERENCES["R1"],
+        "type": "description_dna",
+        "coordinate_system": "c",
+        "variants": [{
+            "location": LOCATIONS["10-5_10-2"],
+            "type": "duplication",
+            "source": "reference",
+            "inserted": [
+                {
+                    "type": "description_dna",
+                    "source": {"id": "R2"},
+                    "location": {
+                        "type": "point",
+                        "position": 10
+                    }
+                }
+            ]
+        }],
+    },
+    "R1:c.10-5_10-2delinsTCTR2.2:c.10": {
+        "reference": REFERENCES["R1"],
+        "type": "description_dna",
+        "coordinate_system": "c",
+        "variants": [{
+            "location": LOCATIONS["10-5_10-2"],
+            "type": "deletion_insertion",
+            "source": "reference",
+            "inserted": [
+                {
+                    "type": "description_dna",
+                    "source": {"id": "TCTR2.2"},
+                    "coordinate_system": "c",
+                    "location": {
+                        "type": "point",
+                        "position": 10
+                    }
+                }
+            ]
+        }],
+    },
+    # TODO: revisit this in the repeats context.
+    "R1:c.10-20[5]": {
+        "reference": REFERENCES["R1"],
+        "type": "description_dna",
+        "coordinate_system": "c",
+        "variants": [{
+            "location": LOCATIONS["10-20"],
+            "type": "repeat",
+            "source": "reference",
+            "inserted": [{"length": LENGTHS["5"]}
+            ]
+        }],
+    },
+    "R1:c.10-5_10-2[5]": {
+        "reference": REFERENCES["R1"],
+        "type": "description_dna",
+        "coordinate_system": "c",
+        "variants": [{
+            "location": LOCATIONS["10-5_10-2"],
+            "type": "repeat",
+            "source": "reference",
+            "inserted": [{"length": LENGTHS["5"]}
+                         ]
+        }],
+    },
+
 }
 
 
 @pytest.mark.parametrize("description, model", _get_tests(DESCRIPTIONS))
 def test_convert(description, model):
     assert to_model(description) == model
 
@@ -963,12 +1055,19 @@
 @pytest.mark.parametrize("description, model", _get_tests(_get_mix()))
 def test_mix(description, model):
     assert to_model(description) == model
 
 
 @pytest.mark.parametrize(
     "description",
-    ["R1:1delinsR2:2del", "R1:1del[R2:2del]", "R1:[1del;10_11insR2:2del]"],
+    [
+        "R1:1delinsR2:2del",
+        "R1:1del[R2:2del]",
+        "R1:[1del;10_11insR2:2del]",
+        "R1:c.10-5_10-2delR2:10del",
+        "R1:c.10-5_10-2dupR2:10del",
+        "R1:c.10-5_10-2delinsTCTR2.2:c.10insT",
+    ],
 )
 def test_nested_descriptions(description):
     with pytest.raises(NestedDescriptions):
         to_model(description)
```

### Comparing `mutalyzer_hgvs_parser-0.3.3/tests/test_hgvs_parser.py` & `mutalyzer_hgvs_parser-0.3.4/tests/test_hgvs_parser.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/tests/test_protein.py` & `mutalyzer_hgvs_parser-0.3.4/tests/test_protein.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_hgvs_parser-0.3.3/tests/test_syntax.py` & `mutalyzer_hgvs_parser-0.3.4/tests/test_syntax.py`

 * *Files identical despite different names*

