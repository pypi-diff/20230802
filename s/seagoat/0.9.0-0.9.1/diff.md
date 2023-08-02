# Comparing `tmp/seagoat-0.9.0.tar.gz` & `tmp/seagoat-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagoat-0.9.0.tar", max compression
+gzip compressed data, was "seagoat-0.9.1.tar", max compression
```

## Comparing `seagoat-0.9.0.tar` & `seagoat-0.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-08-02 15:12:35.088119 seagoat-0.9.0/LICENSE
--rw-r--r--   0        0        0     1849 2023-08-02 15:12:35.088119 seagoat-0.9.0/README.md
--rw-r--r--   0        0        0     3061 2023-08-02 15:12:35.892112 seagoat-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-08-02 15:12:35.892112 seagoat-0.9.0/seagoat/__init__.py
--rw-r--r--   0        0        0     1601 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/cache.py
--rw-r--r--   0        0        0     3209 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/cli.py
--rw-r--r--   0        0        0      196 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/common.py
--rw-r--r--   0        0        0     4424 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/engine.py
--rw-r--r--   0        0        0     3492 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/file.py
--rw-r--r--   0        0        0     2689 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/repository.py
--rw-r--r--   0        0        0     2021 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/result.py
--rw-r--r--   0        0        0     5766 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/server.py
--rw-r--r--   0        0        0     1692 2023-08-02 15:12:35.096119 seagoat-0.9.0/seagoat/sources/chroma.py
--rw-r--r--   0        0        0     1105 2023-08-02 15:12:35.096119 seagoat-0.9.0/seagoat/sources/ripgrep.py
--rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 seagoat-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-02 18:16:36.246643 seagoat-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1849 2023-08-02 18:16:36.246643 seagoat-0.9.1/README.md
+-rw-r--r--   0        0        0     3120 2023-08-02 18:16:37.398646 seagoat-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-08-02 18:16:37.398646 seagoat-0.9.1/seagoat/__init__.py
+-rw-r--r--   0        0        0     1601 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/cache.py
+-rw-r--r--   0        0        0     3209 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/cli.py
+-rw-r--r--   0        0        0      196 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/common.py
+-rw-r--r--   0        0        0     4424 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/engine.py
+-rw-r--r--   0        0        0     3482 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/file.py
+-rw-r--r--   0        0        0     2689 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/repository.py
+-rw-r--r--   0        0        0     2021 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/result.py
+-rw-r--r--   0        0        0     5766 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/server.py
+-rw-r--r--   0        0        0     1678 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/sources/chroma.py
+-rw-r--r--   0        0        0     1105 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/sources/ripgrep.py
+-rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 seagoat-0.9.1/PKG-INFO
```

### Comparing `seagoat-0.9.0/LICENSE` & `seagoat-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.0/README.md` & `seagoat-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.0/pyproject.toml` & `seagoat-0.9.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seagoat"
-version = "0.9.0"
+version = "0.9.1"
 description = "A semantic-code search engine"
 authors = ["Daniel Kantor <git@daniel-kantor.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
 gt = "seagoat.cli:seagoat"
@@ -47,14 +47,16 @@
 exceptiongroup = "^1.1.2"
 pytest-mock = "^3.11.1"
 pytest-fast-first = "^1.0.5"
 pytest-testmon = "^2.0.12"
 pytest-leaks = "^0.3.1"
 mkdocs-material = "^9.1.19"
 markdown-include = "^0.8.1"
+python-semantic-release = "^8.0.4"
+pytest-sugar = "^0.9.7"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 venvPath = "."
```

### Comparing `seagoat-0.9.0/seagoat/cache.py` & `seagoat-0.9.1/seagoat/cache.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.0/seagoat/cli.py` & `seagoat-0.9.1/seagoat/cli.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.0/seagoat/engine.py` & `seagoat-0.9.1/seagoat/engine.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.0/seagoat/file.py` & `seagoat-0.9.1/seagoat/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import hashlib
 import time
+from typing import Dict
 from typing import List
 from typing import Literal
 
-from chromadb.errors import Dict
-
 
 class File:
     def __init__(self, path: str, absolute_path: str):
         self.path = path
         self.absolute_path = absolute_path
         self._commit_times = set()
         self.commit_messages = set()
```

### Comparing `seagoat-0.9.0/seagoat/repository.py` & `seagoat-0.9.1/seagoat/repository.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.0/seagoat/result.py` & `seagoat-0.9.1/seagoat/result.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.0/seagoat/server.py` & `seagoat-0.9.1/seagoat/server.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.0/seagoat/sources/chroma.py` & `seagoat-0.9.1/seagoat/sources/chroma.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from chromadb import chromadb
+import chromadb
 from chromadb.errors import IDAlreadyExistsError
 
 from seagoat.cache import Cache
 from seagoat.repository import Repository
 from seagoat.result import Result
```

### Comparing `seagoat-0.9.0/seagoat/sources/ripgrep.py` & `seagoat-0.9.1/seagoat/sources/ripgrep.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.0/PKG-INFO` & `seagoat-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagoat
-Version: 0.9.0
+Version: 0.9.1
 Summary: A semantic-code search engine
 License: MIT
 Author: Daniel Kantor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

