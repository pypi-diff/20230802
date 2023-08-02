# Comparing `tmp/python3-libraccoon-3.0.0.tar.gz` & `tmp/python3-libraccoon-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-libraccoon-3.0.0.tar", last modified: Wed Feb 15 06:40:30 2023, max compression
+gzip compressed data, was "python3-libraccoon-3.0.2.tar", last modified: Wed Aug  2 16:02:35 2023, max compression
```

## Comparing `python3-libraccoon-3.0.0.tar` & `python3-libraccoon-3.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 latest-release  (1000) latest-release  (1000)        0 2023-02-15 06:40:30.698835 python3-libraccoon-3.0.0/
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)    35149 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/LICENSE
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     4879 2023-02-15 06:40:30.698835 python3-libraccoon-3.0.0/PKG-INFO
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     4062 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/README.md
-drwxrwxr-x   0 latest-release  (1000) latest-release  (1000)        0 2023-02-15 06:40:30.694835 python3-libraccoon-3.0.0/libraccoon/
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)        0 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/__init__.py
-drwxrwxr-x   0 latest-release  (1000) latest-release  (1000)        0 2023-02-15 06:40:30.698835 python3-libraccoon-3.0.0/libraccoon/libs/
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)        0 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/libs/__init__.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     4128 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/libs/bingip2host.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)    11956 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/libs/corscanner.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     2651 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/libs/dns_handler.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     8144 2022-07-19 12:07:20.000000 python3-libraccoon-3.0.0/libraccoon/libs/fierce.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     5743 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/libs/fuzzer.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     4276 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/libs/host.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)    12092 2023-02-15 06:37:32.000000 python3-libraccoon-3.0.0/libraccoon/libs/knockpy.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     6953 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/libs/storage_explorer.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     4060 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/libs/sub_domain.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     5401 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/libs/waf.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     9256 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/libs/web_app.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     6414 2022-10-13 09:43:24.000000 python3-libraccoon-3.0.0/libraccoon/libs/whatwebapi.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)        0 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/main.py
-drwxrwxr-x   0 latest-release  (1000) latest-release  (1000)        0 2023-02-15 06:40:30.698835 python3-libraccoon-3.0.0/libraccoon/utils/
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)        0 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/utils/__init__.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     1761 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/utils/exceptions.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     6603 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/utils/help_utils.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     4991 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/utils/request_handler.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)      294 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/utils/singleton.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     1285 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/utils/utils.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)      900 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/utils/web_server_validator.py
-drwxrwxr-x   0 latest-release  (1000) latest-release  (1000)        0 2023-02-15 06:40:30.698835 python3-libraccoon-3.0.0/libraccoon/wordlists/
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)        1 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/wordlists/__init__.py
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)      199 2022-07-19 05:51:29.000000 python3-libraccoon-3.0.0/libraccoon/wordlists/wordlist_helper.py
-drwxrwxr-x   0 latest-release  (1000) latest-release  (1000)        0 2023-02-15 06:40:30.698835 python3-libraccoon-3.0.0/python3_libraccoon.egg-info/
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     4879 2023-02-15 06:40:30.000000 python3-libraccoon-3.0.0/python3_libraccoon.egg-info/PKG-INFO
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)      943 2023-02-15 06:40:30.000000 python3-libraccoon-3.0.0/python3_libraccoon.egg-info/SOURCES.txt
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)        1 2023-02-15 06:40:30.000000 python3-libraccoon-3.0.0/python3_libraccoon.egg-info/dependency_links.txt
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)       88 2023-02-15 06:40:30.000000 python3-libraccoon-3.0.0/python3_libraccoon.egg-info/requires.txt
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)       11 2023-02-15 06:40:30.000000 python3-libraccoon-3.0.0/python3_libraccoon.egg-info/top_level.txt
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)       38 2023-02-15 06:40:30.698835 python3-libraccoon-3.0.0/setup.cfg
--rw-rw-r--   0 latest-release  (1000) latest-release  (1000)     1270 2023-02-15 06:40:18.000000 python3-libraccoon-3.0.0/setup.py
+drwxrwxr-x   0 nmmapper  (1000) nmmapper  (1000)        0 2023-08-02 16:02:35.161780 python3-libraccoon-3.0.2/
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)    35149 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/LICENSE
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     4879 2023-08-02 16:02:35.161780 python3-libraccoon-3.0.2/PKG-INFO
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     4062 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/README.md
+drwxrwxr-x   0 nmmapper  (1000) nmmapper  (1000)        0 2023-08-02 16:02:35.157778 python3-libraccoon-3.0.2/libraccoon/
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)        0 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/__init__.py
+drwxrwxr-x   0 nmmapper  (1000) nmmapper  (1000)        0 2023-08-02 16:02:35.161780 python3-libraccoon-3.0.2/libraccoon/libs/
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)        0 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/libs/__init__.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     4128 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/libs/bingip2host.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)    11956 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/libs/corscanner.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     2651 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/libs/dns_handler.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     8144 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/libs/fierce.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     5743 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/libs/fuzzer.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     4276 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/libs/host.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)    22910 2023-07-26 16:19:41.000000 python3-libraccoon-3.0.2/libraccoon/libs/knockpy.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     6953 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/libs/storage_explorer.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     4060 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/libs/sub_domain.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     5401 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/libs/waf.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     9256 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/libs/web_app.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     6414 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/libs/whatwebapi.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)        0 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/main.py
+drwxrwxr-x   0 nmmapper  (1000) nmmapper  (1000)        0 2023-08-02 16:02:35.161780 python3-libraccoon-3.0.2/libraccoon/utils/
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)        0 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/utils/__init__.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     1761 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/utils/exceptions.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     6603 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/utils/help_utils.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     4991 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/utils/request_handler.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)      294 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/utils/singleton.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     1285 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/utils/utils.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)      900 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/utils/web_server_validator.py
+drwxrwxr-x   0 nmmapper  (1000) nmmapper  (1000)        0 2023-08-02 16:02:35.161780 python3-libraccoon-3.0.2/libraccoon/wordlists/
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)        1 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/wordlists/__init__.py
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)      199 2023-07-26 16:08:02.000000 python3-libraccoon-3.0.2/libraccoon/wordlists/wordlist_helper.py
+drwxrwxr-x   0 nmmapper  (1000) nmmapper  (1000)        0 2023-08-02 16:02:35.161780 python3-libraccoon-3.0.2/python3_libraccoon.egg-info/
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     4879 2023-08-02 16:02:35.000000 python3-libraccoon-3.0.2/python3_libraccoon.egg-info/PKG-INFO
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)      943 2023-08-02 16:02:35.000000 python3-libraccoon-3.0.2/python3_libraccoon.egg-info/SOURCES.txt
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)        1 2023-08-02 16:02:35.000000 python3-libraccoon-3.0.2/python3_libraccoon.egg-info/dependency_links.txt
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)       88 2023-08-02 16:02:35.000000 python3-libraccoon-3.0.2/python3_libraccoon.egg-info/requires.txt
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)       11 2023-08-02 16:02:35.000000 python3-libraccoon-3.0.2/python3_libraccoon.egg-info/top_level.txt
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)       38 2023-08-02 16:02:35.161780 python3-libraccoon-3.0.2/setup.cfg
+-rw-rw-r--   0 nmmapper  (1000) nmmapper  (1000)     1270 2023-08-02 16:02:07.000000 python3-libraccoon-3.0.2/setup.py
```

### Comparing `python3-libraccoon-3.0.0/LICENSE` & `python3-libraccoon-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/PKG-INFO` & `python3-libraccoon-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-libraccoon
-Version: 3.0.0
+Version: 3.0.2
 Summary: libraccon a library for high performance offensive security tool for reconnaissance based on raccoon scanner. This include performing DNS reconnaissance 
 Home-page: https://github.com/nmmapper/python3-libraccoon
 Author: nmmapper
 Author-email: inquiry@nmmapper.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/nmmapper/python3-libraccoon
 Project-URL: Homepage, https://github.com/nmmapper/python3-libraccoon
```

### Comparing `python3-libraccoon-3.0.0/README.md` & `python3-libraccoon-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/libs/bingip2host.py` & `python3-libraccoon-3.0.2/libraccoon/libs/bingip2host.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/libs/corscanner.py` & `python3-libraccoon-3.0.2/libraccoon/libs/corscanner.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/libs/dns_handler.py` & `python3-libraccoon-3.0.2/libraccoon/libs/dns_handler.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/libs/fierce.py` & `python3-libraccoon-3.0.2/libraccoon/libs/fierce.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/libs/fuzzer.py` & `python3-libraccoon-3.0.2/libraccoon/libs/fuzzer.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/libs/host.py` & `python3-libraccoon-3.0.2/libraccoon/libs/host.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/libs/storage_explorer.py` & `python3-libraccoon-3.0.2/libraccoon/libs/storage_explorer.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/libs/sub_domain.py` & `python3-libraccoon-3.0.2/libraccoon/libs/sub_domain.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/libs/waf.py` & `python3-libraccoon-3.0.2/libraccoon/libs/waf.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/libs/web_app.py` & `python3-libraccoon-3.0.2/libraccoon/libs/web_app.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/libs/whatwebapi.py` & `python3-libraccoon-3.0.2/libraccoon/libs/whatwebapi.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/utils/exceptions.py` & `python3-libraccoon-3.0.2/libraccoon/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/utils/help_utils.py` & `python3-libraccoon-3.0.2/libraccoon/utils/help_utils.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/utils/request_handler.py` & `python3-libraccoon-3.0.2/libraccoon/utils/request_handler.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/utils/utils.py` & `python3-libraccoon-3.0.2/libraccoon/utils/utils.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/libraccoon/utils/web_server_validator.py` & `python3-libraccoon-3.0.2/libraccoon/utils/web_server_validator.py`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/python3_libraccoon.egg-info/PKG-INFO` & `python3-libraccoon-3.0.2/python3_libraccoon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-libraccoon
-Version: 3.0.0
+Version: 3.0.2
 Summary: libraccon a library for high performance offensive security tool for reconnaissance based on raccoon scanner. This include performing DNS reconnaissance 
 Home-page: https://github.com/nmmapper/python3-libraccoon
 Author: nmmapper
 Author-email: inquiry@nmmapper.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/nmmapper/python3-libraccoon
 Project-URL: Homepage, https://github.com/nmmapper/python3-libraccoon
```

### Comparing `python3-libraccoon-3.0.0/python3_libraccoon.egg-info/SOURCES.txt` & `python3-libraccoon-3.0.2/python3_libraccoon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3-libraccoon-3.0.0/setup.py` & `python3-libraccoon-3.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="python3-libraccoon", 
-    version="3.0.0",
+    version="3.0.2",
     author="nmmapper",
     author_email="inquiry@nmmapper.com",
     description="libraccon a library for high performance offensive security tool for reconnaissance based on raccoon scanner. This include performing DNS reconnaissance ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nmmapper/python3-libraccoon",
     project_urls={
```

