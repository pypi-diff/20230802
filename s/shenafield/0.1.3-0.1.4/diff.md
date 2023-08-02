# Comparing `tmp/shenafield-0.1.3.tar.gz` & `tmp/shenafield-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shenafield-0.1.3.tar", max compression
+gzip compressed data, was "shenafield-0.1.4.tar", max compression
```

## Comparing `shenafield-0.1.3.tar` & `shenafield-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-08-02 19:26:47.227186 shenafield-0.1.3/LICENSE
--rw-r--r--   0        0        0     1224 2023-08-02 19:28:34.070575 shenafield-0.1.3/README.md
--rw-r--r--   0        0        0      544 2023-08-02 19:27:55.643396 shenafield-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      114 2023-08-02 18:46:02.270388 shenafield-0.1.3/shenafield/__init__.py
--rw-r--r--   0        0        0     2253 2023-08-02 19:06:53.142981 shenafield-0.1.3/shenafield/cli.py
--rw-r--r--   0        0        0     1588 2023-08-02 19:02:57.734223 shenafield-0.1.3/shenafield/shenafield.py
--rw-r--r--   0        0        0     1840 1970-01-01 00:00:00.000000 shenafield-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-02 19:26:47.227186 shenafield-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1320 2023-08-02 19:30:19.100256 shenafield-0.1.4/README.md
+-rw-r--r--   0        0        0      544 2023-08-02 19:30:25.798308 shenafield-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-08-02 18:46:02.270388 shenafield-0.1.4/shenafield/__init__.py
+-rw-r--r--   0        0        0     2253 2023-08-02 19:06:53.142981 shenafield-0.1.4/shenafield/cli.py
+-rw-r--r--   0        0        0     1588 2023-08-02 19:02:57.734223 shenafield-0.1.4/shenafield/shenafield.py
+-rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 shenafield-0.1.4/PKG-INFO
```

### Comparing `shenafield-0.1.3/LICENSE` & `shenafield-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shenafield-0.1.3/README.md` & `shenafield-0.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # shenafield
 
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/shenafield.svg)](https://badge.fury.io/py/shenafield)
 
 shenafield is a Python library that replicates the unique typing style of shenafield. This library allows users to transform their text into the distinctive style in which shenafield talks.
 
 ## Installation
 
 To install shenafield, you can use `pipx` by running the following command:
```

### Comparing `shenafield-0.1.3/pyproject.toml` & `shenafield-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shenafield"
-version = "0.1.3"
+version = "0.1.4"
 description = "A library that replicates how shenafield talks"
 authors = ["shenafield <99119344+shenafield@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/shenafield/shenafield-style-replicator"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `shenafield-0.1.3/shenafield/cli.py` & `shenafield-0.1.4/shenafield/cli.py`

 * *Files identical despite different names*

### Comparing `shenafield-0.1.3/shenafield/shenafield.py` & `shenafield-0.1.4/shenafield/shenafield.py`

 * *Files identical despite different names*

### Comparing `shenafield-0.1.3/PKG-INFO` & `shenafield-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shenafield
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library that replicates how shenafield talks
 Home-page: https://github.com/shenafield/shenafield-style-replicator
 License: MIT
 Author: shenafield
 Author-email: 99119344+shenafield@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # shenafield
 
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/shenafield.svg)](https://badge.fury.io/py/shenafield)
 
 shenafield is a Python library that replicates the unique typing style of shenafield. This library allows users to transform their text into the distinctive style in which shenafield talks.
 
 ## Installation
 
 To install shenafield, you can use `pipx` by running the following command:
```

