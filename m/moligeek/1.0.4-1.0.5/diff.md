# Comparing `tmp/moligeek-1.0.4.tar.gz` & `tmp/moligeek-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moligeek-1.0.4.tar", last modified: Wed Aug  2 15:39:50 2023, max compression
+gzip compressed data, was "moligeek-1.0.5.tar", last modified: Wed Aug  2 15:42:41 2023, max compression
```

## Comparing `moligeek-1.0.4.tar` & `moligeek-1.0.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 15:39:50.178116 moligeek-1.0.4/
--rw-rw-rw-   0        0        0    11558 2023-06-23 14:02:51.000000 moligeek-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      137 2023-08-02 14:35:19.000000 moligeek-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6553 2023-08-02 15:39:50.178116 moligeek-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5713 2023-08-02 15:20:31.000000 moligeek-1.0.4/README.md
--rw-rw-rw-   0        0        0       64 2023-08-02 14:35:19.000000 moligeek-1.0.4/main.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:39:50.141457 moligeek-1.0.4/moligeek/
--rw-rw-rw-   0        0        0     7457 2023-08-02 14:35:19.000000 moligeek-1.0.4/moligeek/__init__.py
--rw-rw-rw-   0        0        0      340 2023-08-02 15:39:11.000000 moligeek-1.0.4/moligeek/__version__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:39:50.162617 moligeek-1.0.4/moligeek/core/
-drwxrwxrwx   0        0        0        0 2023-08-02 15:39:50.163613 moligeek-1.0.4/moligeek/core/LAN/
--rw-rw-rw-   0        0        0       43 2023-06-23 14:02:51.000000 moligeek-1.0.4/moligeek/core/LAN/__init__.py
--rw-rw-rw-   0        0        0     1206 2023-08-02 08:24:54.000000 moligeek-1.0.4/moligeek/core/LAN/scan.py
--rw-rw-rw-   0        0        0      709 2023-08-02 08:24:54.000000 moligeek-1.0.4/moligeek/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:39:50.166602 moligeek-1.0.4/moligeek/core/encode/
--rw-rw-rw-   0        0        0       42 2023-06-23 14:02:51.000000 moligeek-1.0.4/moligeek/core/encode/__init__.py
--rw-rw-rw-   0        0        0     1097 2023-08-02 05:54:20.000000 moligeek-1.0.4/moligeek/core/encode/decode.py
--rw-rw-rw-   0        0        0     1183 2023-06-23 14:02:51.000000 moligeek-1.0.4/moligeek/core/encode/fence.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:39:50.168592 moligeek-1.0.4/moligeek/core/network/
--rw-rw-rw-   0        0        0     2047 2023-08-02 15:22:21.000000 moligeek-1.0.4/moligeek/core/network/__init__.py
--rw-rw-rw-   0        0        0     1566 2023-08-02 08:24:54.000000 moligeek-1.0.4/moligeek/core/network/hostinfo.py
--rw-rw-rw-   0        0        0     1418 2023-08-02 08:24:54.000000 moligeek-1.0.4/moligeek/core/network/wifi.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:39:50.169592 moligeek-1.0.4/moligeek/core/web/
--rw-rw-rw-   0        0        0     3075 2023-08-02 15:39:17.000000 moligeek-1.0.4/moligeek/core/web/__init__.py
--rw-rw-rw-   0        0        0     6177 2023-06-23 14:02:51.000000 moligeek-1.0.4/moligeek/core/web/imitate.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:39:50.170585 moligeek-1.0.4/moligeek/core/zip/
--rw-rw-rw-   0        0        0     5356 2023-08-02 05:54:20.000000 moligeek-1.0.4/moligeek/core/zip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:39:50.171584 moligeek-1.0.4/moligeek/database/
--rw-rw-rw-   0        0        0   155593 2023-06-23 14:02:51.000000 moligeek-1.0.4/moligeek/database/YiYan.dat
-drwxrwxrwx   0        0        0        0 2023-08-02 15:39:50.177114 moligeek-1.0.4/moligeek/path_dict/
--rw-rw-rw-   0        0        0    40710 2023-06-23 14:02:51.000000 moligeek-1.0.4/moligeek/path_dict/ASP.txt
--rw-rw-rw-   0        0        0    18013 2023-06-23 14:02:51.000000 moligeek-1.0.4/moligeek/path_dict/ASPX.txt
--rw-rw-rw-   0        0        0    23958 2023-06-23 14:02:51.000000 moligeek-1.0.4/moligeek/path_dict/DIR.txt
--rw-rw-rw-   0        0        0    13824 2023-06-23 14:02:51.000000 moligeek-1.0.4/moligeek/path_dict/JSP.txt
--rw-rw-rw-   0        0        0    10198 2023-06-23 14:02:51.000000 moligeek-1.0.4/moligeek/path_dict/MDB.txt
--rw-rw-rw-   0        0        0    21362 2023-06-23 14:02:51.000000 moligeek-1.0.4/moligeek/path_dict/PHP.txt
--rw-rw-rw-   0        0        0      303 2023-06-23 14:02:51.000000 moligeek-1.0.4/moligeek/path_dict/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:39:50.161618 moligeek-1.0.4/moligeek.egg-info/
--rw-rw-rw-   0        0        0     6553 2023-08-02 15:39:49.000000 moligeek-1.0.4/moligeek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-08-02 15:39:50.000000 moligeek-1.0.4/moligeek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 15:39:49.000000 moligeek-1.0.4/moligeek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 15:39:49.000000 moligeek-1.0.4/moligeek.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 09:02:13.000000 moligeek-1.0.4/moligeek.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2023-08-02 15:39:49.000000 moligeek-1.0.4/moligeek.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-02 15:39:49.000000 moligeek-1.0.4/moligeek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-08-01 06:48:22.000000 moligeek-1.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 15:39:50.179109 moligeek-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1768 2023-08-02 14:35:19.000000 moligeek-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.128351 moligeek-1.0.5/
+-rw-rw-rw-   0        0        0    11558 2023-06-23 14:02:51.000000 moligeek-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      137 2023-08-02 14:35:19.000000 moligeek-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6553 2023-08-02 15:42:41.127357 moligeek-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5713 2023-08-02 15:20:31.000000 moligeek-1.0.5/README.md
+-rw-rw-rw-   0        0        0       64 2023-08-02 14:35:19.000000 moligeek-1.0.5/main.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.099017 moligeek-1.0.5/moligeek/
+-rw-rw-rw-   0        0        0     7457 2023-08-02 14:35:19.000000 moligeek-1.0.5/moligeek/__init__.py
+-rw-rw-rw-   0        0        0      340 2023-08-02 15:42:13.000000 moligeek-1.0.5/moligeek/__version__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.112063 moligeek-1.0.5/moligeek/core/
+drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.114051 moligeek-1.0.5/moligeek/core/LAN/
+-rw-rw-rw-   0        0        0       43 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/core/LAN/__init__.py
+-rw-rw-rw-   0        0        0     1206 2023-08-02 08:24:54.000000 moligeek-1.0.5/moligeek/core/LAN/scan.py
+-rw-rw-rw-   0        0        0      709 2023-08-02 08:24:54.000000 moligeek-1.0.5/moligeek/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.116043 moligeek-1.0.5/moligeek/core/encode/
+-rw-rw-rw-   0        0        0       42 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/core/encode/__init__.py
+-rw-rw-rw-   0        0        0     1097 2023-08-02 05:54:20.000000 moligeek-1.0.5/moligeek/core/encode/decode.py
+-rw-rw-rw-   0        0        0     1183 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/core/encode/fence.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.118045 moligeek-1.0.5/moligeek/core/network/
+-rw-rw-rw-   0        0        0     2047 2023-08-02 15:22:21.000000 moligeek-1.0.5/moligeek/core/network/__init__.py
+-rw-rw-rw-   0        0        0     1566 2023-08-02 08:24:54.000000 moligeek-1.0.5/moligeek/core/network/hostinfo.py
+-rw-rw-rw-   0        0        0     1418 2023-08-02 08:24:54.000000 moligeek-1.0.5/moligeek/core/network/wifi.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.119034 moligeek-1.0.5/moligeek/core/web/
+-rw-rw-rw-   0        0        0     3069 2023-08-02 15:40:40.000000 moligeek-1.0.5/moligeek/core/web/__init__.py
+-rw-rw-rw-   0        0        0     6177 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/core/web/imitate.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.119952 moligeek-1.0.5/moligeek/core/zip/
+-rw-rw-rw-   0        0        0     5356 2023-08-02 05:54:20.000000 moligeek-1.0.5/moligeek/core/zip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.121025 moligeek-1.0.5/moligeek/database/
+-rw-rw-rw-   0        0        0   155593 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/database/YiYan.dat
+drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.126302 moligeek-1.0.5/moligeek/path_dict/
+-rw-rw-rw-   0        0        0    40710 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/ASP.txt
+-rw-rw-rw-   0        0        0    18013 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/ASPX.txt
+-rw-rw-rw-   0        0        0    23958 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/DIR.txt
+-rw-rw-rw-   0        0        0    13824 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/JSP.txt
+-rw-rw-rw-   0        0        0    10198 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/MDB.txt
+-rw-rw-rw-   0        0        0    21362 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/PHP.txt
+-rw-rw-rw-   0        0        0      303 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.111063 moligeek-1.0.5/moligeek.egg-info/
+-rw-rw-rw-   0        0        0     6553 2023-08-02 15:42:40.000000 moligeek-1.0.5/moligeek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-08-02 15:42:41.000000 moligeek-1.0.5/moligeek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 15:42:40.000000 moligeek-1.0.5/moligeek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 15:42:40.000000 moligeek-1.0.5/moligeek.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 09:02:13.000000 moligeek-1.0.5/moligeek.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2023-08-02 15:42:40.000000 moligeek-1.0.5/moligeek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 15:42:40.000000 moligeek-1.0.5/moligeek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2023-08-01 06:48:22.000000 moligeek-1.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 15:42:41.128351 moligeek-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1768 2023-08-02 14:35:19.000000 moligeek-1.0.5/setup.py
```

### Comparing `moligeek-1.0.4/LICENSE` & `moligeek-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/PKG-INFO` & `moligeek-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moligeek
-Version: 1.0.4
+Version: 1.0.5
 Summary: 一款逐渐完善的python集成工具,努力为开发者提供最大的便利
 Home-page: https://github.com/yourmoln/moligeek
 Author: yourmoln
 Author-email: yourmoln@outlook.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moligeek Version: 1.0.4 Summary:
+Metadata-Version: 2.1 Name: moligeek Version: 1.0.5 Summary:
 ä¸æ¬¾éæ¸å®åçpythonéæå·¥å·,åªåä¸ºå¼åèæä¾æå¤§çä¾¿å©
 Home-page: https://github.com/yourmoln/moligeek Author: yourmoln Author-email:
 yourmoln@outlook.com License: Apache 2.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `moligeek-1.0.4/README.md` & `moligeek-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/__init__.py` & `moligeek-1.0.5/moligeek/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/core/LAN/scan.py` & `moligeek-1.0.5/moligeek/core/LAN/scan.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/core/__init__.py` & `moligeek-1.0.5/moligeek/core/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/core/encode/decode.py` & `moligeek-1.0.5/moligeek/core/encode/decode.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/core/encode/fence.py` & `moligeek-1.0.5/moligeek/core/encode/fence.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/core/network/__init__.py` & `moligeek-1.0.5/moligeek/core/network/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/core/network/hostinfo.py` & `moligeek-1.0.5/moligeek/core/network/hostinfo.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/core/network/wifi.py` & `moligeek-1.0.5/moligeek/core/network/wifi.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/core/web/__init__.py` & `moligeek-1.0.5/moligeek/core/web/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import path_dict
 
 #仿站
 from .imitate import Imitate
 
 HOST_PATTERN = r".+://(.+)"
 headers = {
-    "User-Agent": meo.net.UserAgent.FIREFOX.value
+    "User-Agent": meo.net.UserAgent.FIREFOX
 }
 
 
 def getsrc(url, output=None, headers=headers):
     host_match = re.match(HOST_PATTERN, url)
     host = host_match.group(1)
     try:
```

### Comparing `moligeek-1.0.4/moligeek/core/web/imitate.py` & `moligeek-1.0.5/moligeek/core/web/imitate.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/core/zip/__init__.py` & `moligeek-1.0.5/moligeek/core/zip/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/database/YiYan.dat` & `moligeek-1.0.5/moligeek/database/YiYan.dat`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/path_dict/ASP.txt` & `moligeek-1.0.5/moligeek/path_dict/ASP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/path_dict/ASPX.txt` & `moligeek-1.0.5/moligeek/path_dict/ASPX.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/path_dict/DIR.txt` & `moligeek-1.0.5/moligeek/path_dict/DIR.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/path_dict/JSP.txt` & `moligeek-1.0.5/moligeek/path_dict/JSP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/path_dict/MDB.txt` & `moligeek-1.0.5/moligeek/path_dict/MDB.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek/path_dict/PHP.txt` & `moligeek-1.0.5/moligeek/path_dict/PHP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/moligeek.egg-info/PKG-INFO` & `moligeek-1.0.5/moligeek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moligeek
-Version: 1.0.4
+Version: 1.0.5
 Summary: 一款逐渐完善的python集成工具,努力为开发者提供最大的便利
 Home-page: https://github.com/yourmoln/moligeek
 Author: yourmoln
 Author-email: yourmoln@outlook.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moligeek Version: 1.0.4 Summary:
+Metadata-Version: 2.1 Name: moligeek Version: 1.0.5 Summary:
 ä¸æ¬¾éæ¸å®åçpythonéæå·¥å·,åªåä¸ºå¼åèæä¾æå¤§çä¾¿å©
 Home-page: https://github.com/yourmoln/moligeek Author: yourmoln Author-email:
 yourmoln@outlook.com License: Apache 2.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `moligeek-1.0.4/moligeek.egg-info/SOURCES.txt` & `moligeek-1.0.5/moligeek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.4/setup.py` & `moligeek-1.0.5/setup.py`

 * *Files identical despite different names*

