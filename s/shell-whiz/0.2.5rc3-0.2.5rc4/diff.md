# Comparing `tmp/shell_whiz-0.2.5rc3.tar.gz` & `tmp/shell_whiz-0.2.5rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whiz-0.2.5rc3.tar", max compression
+gzip compressed data, was "shell_whiz-0.2.5rc4.tar", max compression
```

## Comparing `shell_whiz-0.2.5rc3.tar` & `shell_whiz-0.2.5rc4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-08-01 19:31:55.693470 shell_whiz-0.2.5rc3/LICENSE
--rw-r--r--   0        0        0     3141 2023-08-01 19:31:55.693470 shell_whiz-0.2.5rc3/README.md
--rw-r--r--   0        0        0      542 2023-08-01 19:31:55.697470 shell_whiz-0.2.5rc3/pyproject.toml
--rw-r--r--   0        0        0      510 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/argparse.py
--rw-r--r--   0        0        0     6780 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/cli.py
--rw-r--r--   0        0        0     1686 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/config.py
--rw-r--r--   0        0        0       54 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/console.py
--rw-r--r--   0        0        0      207 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/constants.py
--rw-r--r--   0        0        0      152 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/exceptions.py
--rw-r--r--   0        0        0    10011 2023-08-01 19:31:55.701470 shell_whiz-0.2.5rc3/shell_whiz/openai.py
--rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 shell_whiz-0.2.5rc3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-02 08:02:38.893533 shell_whiz-0.2.5rc4/LICENSE
+-rw-r--r--   0        0        0     3141 2023-08-02 08:02:38.893533 shell_whiz-0.2.5rc4/README.md
+-rw-r--r--   0        0        0      542 2023-08-02 08:02:38.901533 shell_whiz-0.2.5rc4/pyproject.toml
+-rw-r--r--   0        0        0      510 2023-08-02 08:02:38.901533 shell_whiz-0.2.5rc4/shell_whiz/argparse.py
+-rw-r--r--   0        0        0     6780 2023-08-02 08:02:38.901533 shell_whiz-0.2.5rc4/shell_whiz/cli.py
+-rw-r--r--   0        0        0     1686 2023-08-02 08:02:38.901533 shell_whiz-0.2.5rc4/shell_whiz/config.py
+-rw-r--r--   0        0        0       54 2023-08-02 08:02:38.901533 shell_whiz-0.2.5rc4/shell_whiz/console.py
+-rw-r--r--   0        0        0      207 2023-08-02 08:02:38.901533 shell_whiz-0.2.5rc4/shell_whiz/constants.py
+-rw-r--r--   0        0        0      152 2023-08-02 08:02:38.901533 shell_whiz-0.2.5rc4/shell_whiz/exceptions.py
+-rw-r--r--   0        0        0    10011 2023-08-02 08:02:38.901533 shell_whiz-0.2.5rc4/shell_whiz/openai.py
+-rw-r--r--   0        0        0     3892 1970-01-01 00:00:00.000000 shell_whiz-0.2.5rc4/PKG-INFO
```

### Comparing `shell_whiz-0.2.5rc3/LICENSE` & `shell_whiz-0.2.5rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc3/README.md` & `shell_whiz-0.2.5rc4/README.md`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc3/pyproject.toml` & `shell_whiz-0.2.5rc4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "shell-whiz"
-version = "0.2.5rc3"
+version = "0.2.5rc4"
 description = "Shell Whiz: AI assistant right in your terminal"
 license = "GPL-3.0-only"
 authors = ["Tamerlan Bimzhanov <bimzhanovt.net@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_whiz"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8 <4"
+python = ">=3.9 <4"
 openai = "^0.27.8"
 inquirer = "^3.1.3"
 yaspin = "^2.3.0"
 jsonschema = "^4.18.4"
-rich = "^13.4.2"
+rich = "^13.5.2"
 
 [tool.poetry.scripts]
 sw = "shell_whiz.cli:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shell_whiz-0.2.5rc3/shell_whiz/cli.py` & `shell_whiz-0.2.5rc4/shell_whiz/cli.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc3/shell_whiz/config.py` & `shell_whiz-0.2.5rc4/shell_whiz/config.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc3/shell_whiz/openai.py` & `shell_whiz-0.2.5rc4/shell_whiz/openai.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc3/PKG-INFO` & `shell_whiz-0.2.5rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: shell-whiz
-Version: 0.2.5rc3
+Version: 0.2.5rc4
 Summary: Shell Whiz: AI assistant right in your terminal
 License: GPL-3.0-only
 Author: Tamerlan Bimzhanov
 Author-email: bimzhanovt.net@gmail.com
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: jsonschema (>=4.18.4,<5.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: rich (>=13.5.2,<14.0.0)
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://github.com/beimzhan/shell-whiz/raw/main/images/shell-whiz.png" />
 </p>
```

