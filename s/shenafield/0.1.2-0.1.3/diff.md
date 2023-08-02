# Comparing `tmp/shenafield-0.1.2.tar.gz` & `tmp/shenafield-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shenafield-0.1.2.tar", max compression
+gzip compressed data, was "shenafield-0.1.3.tar", max compression
```

## Comparing `shenafield-0.1.2.tar` & `shenafield-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1115 2023-08-02 19:24:40.289219 shenafield-0.1.2/README.md
--rw-r--r--   0        0        0      457 2023-08-02 19:24:53.257187 shenafield-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      114 2023-08-02 18:46:02.270388 shenafield-0.1.2/shenafield/__init__.py
--rw-r--r--   0        0        0     2253 2023-08-02 19:06:53.142981 shenafield-0.1.2/shenafield/cli.py
--rw-r--r--   0        0        0     1588 2023-08-02 19:02:57.734223 shenafield-0.1.2/shenafield/shenafield.py
--rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 shenafield-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-02 19:26:47.227186 shenafield-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1224 2023-08-02 19:28:34.070575 shenafield-0.1.3/README.md
+-rw-r--r--   0        0        0      544 2023-08-02 19:27:55.643396 shenafield-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-08-02 18:46:02.270388 shenafield-0.1.3/shenafield/__init__.py
+-rw-r--r--   0        0        0     2253 2023-08-02 19:06:53.142981 shenafield-0.1.3/shenafield/cli.py
+-rw-r--r--   0        0        0     1588 2023-08-02 19:02:57.734223 shenafield-0.1.3/shenafield/shenafield.py
+-rw-r--r--   0        0        0     1840 1970-01-01 00:00:00.000000 shenafield-0.1.3/PKG-INFO
```

### Comparing `shenafield-0.1.2/README.md` & `shenafield-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # shenafield
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 shenafield is a Python library that replicates the unique typing style of shenafield. This library allows users to transform their text into the distinctive style in which shenafield talks.
 
 ## Installation
 
 To install shenafield, you can use `pipx` by running the following command:
 
 ```bash
```

### Comparing `shenafield-0.1.2/shenafield/cli.py` & `shenafield-0.1.3/shenafield/cli.py`

 * *Files identical despite different names*

### Comparing `shenafield-0.1.2/shenafield/shenafield.py` & `shenafield-0.1.3/shenafield/shenafield.py`

 * *Files identical despite different names*

### Comparing `shenafield-0.1.2/PKG-INFO` & `shenafield-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: shenafield
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library that replicates how shenafield talks
+Home-page: https://github.com/shenafield/shenafield-style-replicator
+License: MIT
 Author: shenafield
 Author-email: 99119344+shenafield@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # shenafield
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 shenafield is a Python library that replicates the unique typing style of shenafield. This library allows users to transform their text into the distinctive style in which shenafield talks.
 
 ## Installation
 
 To install shenafield, you can use `pipx` by running the following command:
 
 ```bash
```

