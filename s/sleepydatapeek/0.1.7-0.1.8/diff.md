# Comparing `tmp/sleepydatapeek-0.1.7.tar.gz` & `tmp/sleepydatapeek-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepydatapeek-0.1.7.tar", max compression
+gzip compressed data, was "sleepydatapeek-0.1.8.tar", max compression
```

## Comparing `sleepydatapeek-0.1.7.tar` & `sleepydatapeek-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    35149 2022-12-25 23:19:50.986710 sleepydatapeek-0.1.7/LICENSE
--rw-r--r--   0        0        0     2157 2022-12-26 00:09:54.247932 sleepydatapeek-0.1.7/README.md
--rw-r--r--   0        0        0      577 2022-12-26 00:10:33.076113 sleepydatapeek-0.1.7/pyproject.toml
--rwxr-xr-x   0        0        0     3751 2022-12-25 23:19:50.995313 sleepydatapeek-0.1.7/sleepydatapeek.py
--rw-r--r--   0        0        0     1366 2022-12-25 23:19:50.997586 sleepydatapeek-0.1.7/toolchain/df_utils.py
--rw-r--r--   0        0        0     2602 2022-12-25 23:19:50.998205 sleepydatapeek-0.1.7/toolchain/option_utils.py
--rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 sleepydatapeek-0.1.7/setup.py
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 sleepydatapeek-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-30 21:27:14.923251 sleepydatapeek-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2157 2023-07-30 21:27:14.923444 sleepydatapeek-0.1.8/README.md
+-rw-r--r--   0        0        0      570 2023-08-01 22:07:00.488256 sleepydatapeek-0.1.8/pyproject.toml
+-rwxr-xr-x   0        0        0     1307 2023-08-01 08:21:08.446964 sleepydatapeek-0.1.8/sleepydatapeek.py
+-rw-r--r--   0        0        0     2016 2023-08-01 08:24:07.460864 sleepydatapeek-0.1.8/toolchain/commands.py
+-rw-r--r--   0        0        0      421 2023-08-01 06:36:50.154356 sleepydatapeek-0.1.8/toolchain/utils.py
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 sleepydatapeek-0.1.8/PKG-INFO
```

### Comparing `sleepydatapeek-0.1.7/LICENSE` & `sleepydatapeek-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.1.7/README.md` & `sleepydatapeek-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.1.7/pyproject.toml` & `sleepydatapeek-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "sleepydatapeek"
-version = "0.1.7"
+version = "0.1.8"
 description = "Peek at local datafiles fast!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 repository = "https://github.com/anthonybench/datapeek"
 keywords = ["pandas", "data"]
 packages = [
     { include = "sleepydatapeek.py" },
-    { include = "toolchain/option_utils.py" },
-    { include = "toolchain/df_utils.py" },
+    { include = "toolchain/commands.py" },
+    { include = "toolchain/utils.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^1.5.1"
 
 [build-system]
```

### Comparing `sleepydatapeek-0.1.7/PKG-INFO` & `sleepydatapeek-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepydatapeek
-Version: 0.1.7
+Version: 0.1.8
 Summary: Peek at local datafiles fast!
 Home-page: https://github.com/anthonybench/datapeek
 License: GNU GPL
 Keywords: pandas,data
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
```

