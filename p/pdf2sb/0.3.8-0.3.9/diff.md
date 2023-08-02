# Comparing `tmp/pdf2sb-0.3.8.tar.gz` & `tmp/pdf2sb-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf2sb-0.3.8.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pdf2sb-0.3.8.tar` & `pdf2sb-0.3.9.tar`

### file list

```diff
@@ -1,6 +1,15 @@
--rw-r--r--   0        0        0     1070 2022-11-30 17:53:57.382306 pdf2sb-0.3.8/LICENSE
--rw-r--r--   0        0        0     1397 2022-11-30 17:53:57.382306 pdf2sb-0.3.8/README.md
--rw-r--r--   0        0        0     5461 2022-11-30 17:53:57.382306 pdf2sb-0.3.8/pdf2sb/__init__.py
--rw-r--r--   0        0        0      779 2022-11-30 17:53:57.382306 pdf2sb-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     2309 1970-01-01 00:00:00.000000 pdf2sb-0.3.8/setup.py
--rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 pdf2sb-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/.dockerignore
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/Dockerfile
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/requirements-dev.lock
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/requirements.lock
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/.github/workflows/package.yaml
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/src/pdf2sb/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/tests/__init__.py
+-rw-r--r--   0        0        0   623354 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/tests/slides.pdf
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/tests/test_pdf2sb.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/README.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 pdf2sb-0.3.9/PKG-INFO
```

### Comparing `pdf2sb-0.3.8/LICENSE` & `pdf2sb-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf2sb-0.3.8/README.md` & `pdf2sb-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pdf2sb-0.3.8/pdf2sb/__init__.py` & `pdf2sb-0.3.9/src/pdf2sb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from itertools import chain
 from pathlib import Path
 from typing import Iterable, Iterator, List, Optional, Tuple
 from urllib.request import urlopen
 
 import click
 import gyazo
-import PyPDF2
+import PyPDF2  # type: ignore[import]
 from pdf2image import convert_from_path
 from PIL.Image import Image
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 
 
 def parse_range(expr: str) -> Iterator[Tuple[int, int]]:
     """Yield start and end integer pairs from a range string like "1-9,12, 15-20,23".
 
     >>> list(parse_range("1-9,12, 15-20,23"))
     [(1, 9), (12, 12), (15, 20), (23, 23)]
```

### Comparing `pdf2sb-0.3.8/PKG-INFO` & `pdf2sb-0.3.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 Metadata-Version: 2.1
 Name: pdf2sb
-Version: 0.3.8
+Version: 0.3.9
 Summary: Upload PDF file to Gyazo as images then convert Scrapbox format
-Home-page: https://github.com/reiyw/pdf2sb
-License: MIT
-Author: reiyw
-Author-email: reiyw.setuve@gmail.com
-Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pillow (>=8.4.0,<9.0.0)
-Requires-Dist: click (>=8.0,<9.0)
-Requires-Dist: pdf2image (>=1.4,<2.0)
-Requires-Dist: pypdf2 (>=1.26,<2.0)
-Requires-Dist: python-gyazo (>=1.1,<2.0)
-Project-URL: Repository, https://github.com/reiyw/pdf2sb
+Project-URL: repository, https://github.com/reiyw/pdf2sb
+Author-email: Ryo Takahashi <reiyw.setuve@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
+Requires-Python: >=3.8
+Requires-Dist: click~=8.0
+Requires-Dist: pdf2image~=1.4
+Requires-Dist: pillow~=8.4.0
+Requires-Dist: pypdf2~=1.26
+Requires-Dist: python-gyazo~=1.1
 Description-Content-Type: text/markdown
 
 # pdf2sb
 
 ![PyPI](https://img.shields.io/pypi/v/pdf2sb.svg) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pdf2sb.svg) ![PyPI - License](https://img.shields.io/pypi/l/pdf2sb.svg)
 
 Upload PDF file to Gyazo as images then convert Scrapbox format.
@@ -68,8 +60,7 @@
 You can run pdf2sb also via Docker:
 
 ```sh
 FILE=<your pdf file>; docker run --env GYAZO_ACCESS_TOKEN=$GYAZO_ACCESS_TOKEN -v $(readlink -f $FILE):/app/${FILE##*/} ghcr.io/reiyw/pdf2sb ${FILE##*/}
 # or
 docker run --env GYAZO_ACCESS_TOKEN=$GYAZO_ACCESS_TOKEN ghcr.io/reiyw/pdf2sb <URL>
 ```
-
```

