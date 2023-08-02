# Comparing `tmp/seagoat-0.8.9.tar.gz` & `tmp/seagoat-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagoat-0.8.9.tar", max compression
+gzip compressed data, was "seagoat-0.9.0.tar", max compression
```

## Comparing `seagoat-0.8.9.tar` & `seagoat-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-07-31 08:42:03.852176 seagoat-0.8.9/LICENSE
--rw-r--r--   0        0        0     1847 2023-07-31 08:42:03.852176 seagoat-0.8.9/README.md
--rw-r--r--   0        0        0     3085 2023-07-31 08:42:04.672192 seagoat-0.8.9/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-31 08:42:04.672192 seagoat-0.8.9/seagoat/__init__.py
--rw-r--r--   0        0        0     1601 2023-07-31 08:42:03.860176 seagoat-0.8.9/seagoat/cache.py
--rw-r--r--   0        0        0     2901 2023-07-31 08:42:03.860176 seagoat-0.8.9/seagoat/cli.py
--rw-r--r--   0        0        0      196 2023-07-31 08:42:03.860176 seagoat-0.8.9/seagoat/common.py
--rw-r--r--   0        0        0     4424 2023-07-31 08:42:03.860176 seagoat-0.8.9/seagoat/engine.py
--rw-r--r--   0        0        0     3492 2023-07-31 08:42:03.860176 seagoat-0.8.9/seagoat/file.py
--rw-r--r--   0        0        0     2689 2023-07-31 08:42:03.860176 seagoat-0.8.9/seagoat/repository.py
--rw-r--r--   0        0        0     2021 2023-07-31 08:42:03.860176 seagoat-0.8.9/seagoat/result.py
--rw-r--r--   0        0        0     5766 2023-07-31 08:42:03.860176 seagoat-0.8.9/seagoat/server.py
--rw-r--r--   0        0        0     1692 2023-07-31 08:42:03.860176 seagoat-0.8.9/seagoat/sources/chroma.py
--rw-r--r--   0        0        0     1105 2023-07-31 08:42:03.860176 seagoat-0.8.9/seagoat/sources/ripgrep.py
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 seagoat-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-02 15:12:35.088119 seagoat-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1849 2023-08-02 15:12:35.088119 seagoat-0.9.0/README.md
+-rw-r--r--   0        0        0     3061 2023-08-02 15:12:35.892112 seagoat-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-08-02 15:12:35.892112 seagoat-0.9.0/seagoat/__init__.py
+-rw-r--r--   0        0        0     1601 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/cache.py
+-rw-r--r--   0        0        0     3209 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/cli.py
+-rw-r--r--   0        0        0      196 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/common.py
+-rw-r--r--   0        0        0     4424 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/engine.py
+-rw-r--r--   0        0        0     3492 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/file.py
+-rw-r--r--   0        0        0     2689 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/repository.py
+-rw-r--r--   0        0        0     2021 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/result.py
+-rw-r--r--   0        0        0     5766 2023-08-02 15:12:35.092119 seagoat-0.9.0/seagoat/server.py
+-rw-r--r--   0        0        0     1692 2023-08-02 15:12:35.096119 seagoat-0.9.0/seagoat/sources/chroma.py
+-rw-r--r--   0        0        0     1105 2023-08-02 15:12:35.096119 seagoat-0.9.0/seagoat/sources/ripgrep.py
+-rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 seagoat-0.9.0/PKG-INFO
```

### Comparing `seagoat-0.8.9/LICENSE` & `seagoat-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.9/README.md` & `seagoat-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 In order to install SeaGOAT, you need to have the following
 dependencies already installed on your computer:
 
 - Python 3.11 or newer
 - ripgrep
 
-To install SeaGOAT using `pip`, use the following command:
+To install SeaGOAT using `pipx`, use the following command:
 
 ```bash
-pip install seagoat
+pipx install seagoat
 ```
 
 ### Start SeaGOAT server
 
 In order to use SeaGOAT in your project, you have to start the SeaGOAT server
 using the following command:
```

### Comparing `seagoat-0.8.9/pyproject.toml` & `seagoat-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seagoat"
-version = "0.8.9"
+version = "0.9.0"
 description = "A semantic-code search engine"
 authors = ["Daniel Kantor <git@daniel-kantor.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
 gt = "seagoat.cli:seagoat"
@@ -43,15 +43,14 @@
 syrupy = "^4.0.4"
 pytest-asyncio = "^0.21.0"
 ipython = "^8.14.0"
 pytest-flask = "^1.2.0"
 exceptiongroup = "^1.1.2"
 pytest-mock = "^3.11.1"
 pytest-fast-first = "^1.0.5"
-pytest-sugar = "^0.9.7"
 pytest-testmon = "^2.0.12"
 pytest-leaks = "^0.3.1"
 mkdocs-material = "^9.1.19"
 markdown-include = "^0.8.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `seagoat-0.8.9/seagoat/cache.py` & `seagoat-0.9.0/seagoat/cache.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.9/seagoat/cli.py` & `seagoat-0.9.0/seagoat/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import sys
 from functools import cache
+from itertools import islice
 
 import click
 import requests
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
 from pygments.lexers import get_lexer_for_filename
 from pygments.lexers.javascript import JavascriptLexer
@@ -64,30 +65,43 @@
     else:
         for line_content in result["lines"]:
             if line_content["line"] == line:
                 print(f"{result['path']}:{line}:{line_content['line_text']}")
                 break
 
 
+def iterate_result_lines(results):
+    for result in results:
+        for line in result.get("lines", []):
+            yield result, line
+
+
 @click.command()
 @click.argument("query")
 @click.argument("repo_path", required=False, default=os.getcwd())
 @click.option(
     "--no-color",
     is_flag=True,
     help="Disable formatting. Automatically enabled when part of a bash pipeline.",
 )
+@click.option(
+    "-l",
+    "--max-results",
+    type=int,
+    default=None,
+    help="Limit the number of result lines",
+)
 @click.version_option(version=__version__, prog_name="seagoat")
-def seagoat(query, repo_path, no_color):
+def seagoat(query, repo_path, no_color, max_results):
     server_info_file = get_server_info_file(repo_path)
     _, __, ___, server_address = load_server_info(server_info_file)
     results = query_server(query, server_address, repo_path)
 
     color_enabled = os.isatty(0) and not no_color
-    for result in results:
-        for result_line in result.get("lines", []):
-            print_result_line(result, result_line["line"], color_enabled)
+
+    for result, result_line in islice(iterate_result_lines(results), max_results):
+        print_result_line(result, result_line["line"], color_enabled)
 
 
 if __name__ == "__main__":
     # pylint: disable-next=no-value-for-parameter
     seagoat()
```

### Comparing `seagoat-0.8.9/seagoat/engine.py` & `seagoat-0.9.0/seagoat/engine.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.9/seagoat/file.py` & `seagoat-0.9.0/seagoat/file.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.9/seagoat/repository.py` & `seagoat-0.9.0/seagoat/repository.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.9/seagoat/result.py` & `seagoat-0.9.0/seagoat/result.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.9/seagoat/server.py` & `seagoat-0.9.0/seagoat/server.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.9/seagoat/sources/chroma.py` & `seagoat-0.9.0/seagoat/sources/chroma.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.9/seagoat/sources/ripgrep.py` & `seagoat-0.9.0/seagoat/sources/ripgrep.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.8.9/PKG-INFO` & `seagoat-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagoat
-Version: 0.8.9
+Version: 0.9.0
 Summary: A semantic-code search engine
 License: MIT
 Author: Daniel Kantor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -44,18 +44,18 @@
 
 In order to install SeaGOAT, you need to have the following
 dependencies already installed on your computer:
 
 - Python 3.11 or newer
 - ripgrep
 
-To install SeaGOAT using `pip`, use the following command:
+To install SeaGOAT using `pipx`, use the following command:
 
 ```bash
-pip install seagoat
+pipx install seagoat
 ```
 
 ### Start SeaGOAT server
 
 In order to use SeaGOAT in your project, you have to start the SeaGOAT server
 using the following command:
```

