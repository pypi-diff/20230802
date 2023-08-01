# Comparing `tmp/sleepydatapeek-0.1.9.tar.gz` & `tmp/sleepydatapeek-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepydatapeek-0.1.9.tar", max compression
+gzip compressed data, was "sleepydatapeek-0.2.0.tar", max compression
```

## Comparing `sleepydatapeek-0.1.9.tar` & `sleepydatapeek-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-07-30 21:27:14.923251 sleepydatapeek-0.1.9/LICENSE
--rw-r--r--   0        0        0     2157 2023-07-30 21:27:14.923444 sleepydatapeek-0.1.9/README.md
--rw-r--r--   0        0        0      570 2023-08-01 22:14:11.380149 sleepydatapeek-0.1.9/pyproject.toml
--rwxr-xr-x   0        0        0     1118 2023-08-01 22:13:44.055991 sleepydatapeek-0.1.9/sleepydatapeek.py
--rw-r--r--   0        0        0     2016 2023-08-01 08:24:07.460864 sleepydatapeek-0.1.9/toolchain/commands.py
--rw-r--r--   0        0        0      421 2023-08-01 06:36:50.154356 sleepydatapeek-0.1.9/toolchain/utils.py
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 sleepydatapeek-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-30 21:27:14.923251 sleepydatapeek-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1817 2023-08-01 22:30:32.920527 sleepydatapeek-0.2.0/README.md
+-rw-r--r--   0        0        0      570 2023-08-01 22:33:33.036721 sleepydatapeek-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1118 2023-08-01 22:13:44.055991 sleepydatapeek-0.2.0/sleepydatapeek.py
+-rw-r--r--   0        0        0     2016 2023-08-01 08:24:07.460864 sleepydatapeek-0.2.0/toolchain/commands.py
+-rw-r--r--   0        0        0      421 2023-08-01 06:36:50.154356 sleepydatapeek-0.2.0/toolchain/utils.py
+-rw-r--r--   0        0        0     2442 1970-01-01 00:00:00.000000 sleepydatapeek-0.2.0/PKG-INFO
```

### Comparing `sleepydatapeek-0.1.9/LICENSE` & `sleepydatapeek-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.1.9/README.md` & `sleepydatapeek-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: sleepydatapeek
+Version: 0.2.0
+Summary: Peek at local datafiles fast!
+Home-page: https://github.com/anthonybench/datapeek
+License: GNU GPL
+Keywords: pandas,data
+Author: anthonybench
+Author-email: anythonybenchyep@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas (>=1.5.1,<2.0.0)
+Project-URL: Repository, https://github.com/anthonybench/datapeek
+Description-Content-Type: text/markdown
+
 # **DataPeek**
 *A quick way to peek at local datafiles.*
 
 <br />
 
 ## **Welcome to sleepydatapeek!**
 In short, it's hand to have something be able to spit out a configurable preview of data from a file, and bonus points if you can just as easily output in markdown. It would also be nice if said tool could read all the formats.\
@@ -20,54 +38,61 @@
   - License/Stats/Author
 
 <br />
 
 ## **Get Started 🚀**
 <hr>
 
-This repo is currently private, so adding this package is all the user needs to care about.
+```sh
+pip install sleepydatapeek
+pip install --upgrade sleepydatapeek
+```
 
 <br />
 
 ## **Usage ⚙**
 <hr>
 
-After setting up the tool, run `./main.py [-h|--help]` to display this message:
-```txt
-This tool takes an input file path and outputs a limited dataframe to either stdout or a markdown file.
-
-
-Limit defaults to 20 rows, and can be overwritten.
-Format value has synonyms 'xlsx' and 'xls'.
---------------
-Usage:
-  ./sleepydatapeek.py --format=[parquet|csv|json|excel] --path=<path> [--output=<path>] [--limit=<row-limit>]
-Examples:
-  ./sleepydatapeek.py --format=csv --path=sample-data/data.csv
-  ./sleepydatapeek.py --format=csv --path=sample-data/data.csv --limit=6
-  ./sleepydatapeek.py --format=csv --path=sample-data/data.csv --output=results.md
-Info:
-  ./sleepydatapeek.py [-h|--help]
---------------
+Fetch dependencies:
+```sh
+pip install -r requirements.txt
+```
+
+Set a function in your shell environment to run a script like:
+```sh
+# pip install sleepydatapeek
+# pip install --upgrade sleepydatapeek
+
+from sleepydatapeek import sleepydatapeek
+from sys import argv, exit
+
+sleepydatapeek(argv[1:])
+exit(0)
+```
+
+Presuming you've named said function `emoji`, print the help message:
+```sh
+sleepydatapeek --help
 ```
 
 <br />
 
 ## **Technologies 🧰**
 <hr>
 
   - [Pandas](https://pandas.pydata.org/docs/)
+  - [Tabulate](https://pypi.org/project/tabulate/)
+  - [Typer](https://typer.tiangolo.com/)
 
 <br />
 
 ## **Contribute 🤝**
 <hr>
 
-As stated in the welcome section, the corresponding GitHub repo is private. \
-However, feel free to [reach out with opinions](https://github.com/anthonybench)!
+If you have opinions, submit a PR 😊.
 
 <br />
 
 ## **Acknowledgements 💙**
 <hr>
 
 Cheers to the chaos of modern life for needing personalized agility in schema assessment.
@@ -80,10 +105,10 @@
 <img align="right" alt="example image tag" src="https://i.imgur.com/jtNwEWu.png" width="200" />
 
 <!-- badge cluster -->
 
 ![PyPI - License](https://img.shields.io/pypi/l/sleepydatapeek?style=plastic)
 
 <!-- / -->
-See [License](TODO) for the full license text.
+See [License](LICENSE) for the full license text.
 
-This package was authored by *Isaac Yep*.
+This package was authored by *Isaac Yep*.
```

### Comparing `sleepydatapeek-0.1.9/pyproject.toml` & `sleepydatapeek-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sleepydatapeek"
-version = "0.1.9"
+version = "0.2.0"
 description = "Peek at local datafiles fast!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 repository = "https://github.com/anthonybench/datapeek"
 keywords = ["pandas", "data"]
 packages = [
```

### Comparing `sleepydatapeek-0.1.9/sleepydatapeek.py` & `sleepydatapeek-0.2.0/sleepydatapeek.py`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.1.9/toolchain/commands.py` & `sleepydatapeek-0.2.0/toolchain/commands.py`

 * *Files identical despite different names*

