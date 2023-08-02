# Comparing `tmp/moligeek-1.0.0.tar.gz` & `tmp/moligeek-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moligeek-1.0.0.tar", last modified: Wed Aug  2 10:25:44 2023, max compression
+gzip compressed data, was "moligeek-1.0.1.tar", last modified: Wed Aug  2 12:08:34 2023, max compression
```

## Comparing `moligeek-1.0.0.tar` & `moligeek-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 10:25:44.332847 moligeek-1.0.0/
--rw-rw-rw-   0        0        0    11558 2023-06-23 14:02:51.000000 moligeek-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      129 2023-08-02 09:01:41.000000 moligeek-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6332 2023-08-02 10:25:44.331850 moligeek-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5492 2023-08-02 05:54:20.000000 moligeek-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 10:25:44.311277 moligeek-1.0.0/moligeek/
--rw-rw-rw-   0        0        0     1430 2023-08-01 06:48:22.000000 moligeek-1.0.0/moligeek/__init__.py
--rw-rw-rw-   0        0        0      340 2023-08-02 08:24:54.000000 moligeek-1.0.0/moligeek/__version__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:25:44.318261 moligeek-1.0.0/moligeek/core/
-drwxrwxrwx   0        0        0        0 2023-08-02 10:25:44.319766 moligeek-1.0.0/moligeek/core/LAN/
--rw-rw-rw-   0        0        0       43 2023-06-23 14:02:51.000000 moligeek-1.0.0/moligeek/core/LAN/__init__.py
--rw-rw-rw-   0        0        0     1206 2023-08-02 08:24:54.000000 moligeek-1.0.0/moligeek/core/LAN/scan.py
--rw-rw-rw-   0        0        0      709 2023-08-02 08:24:54.000000 moligeek-1.0.0/moligeek/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:25:44.321779 moligeek-1.0.0/moligeek/core/encode/
--rw-rw-rw-   0        0        0       42 2023-06-23 14:02:51.000000 moligeek-1.0.0/moligeek/core/encode/__init__.py
--rw-rw-rw-   0        0        0     1097 2023-08-02 05:54:20.000000 moligeek-1.0.0/moligeek/core/encode/decode.py
--rw-rw-rw-   0        0        0     1183 2023-06-23 14:02:51.000000 moligeek-1.0.0/moligeek/core/encode/fence.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:25:44.323767 moligeek-1.0.0/moligeek/core/network/
--rw-rw-rw-   0        0        0     2053 2023-08-02 08:24:54.000000 moligeek-1.0.0/moligeek/core/network/__init__.py
--rw-rw-rw-   0        0        0     1566 2023-08-02 08:24:54.000000 moligeek-1.0.0/moligeek/core/network/hostinfo.py
--rw-rw-rw-   0        0        0     1418 2023-08-02 08:24:54.000000 moligeek-1.0.0/moligeek/core/network/wifi.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:25:44.324763 moligeek-1.0.0/moligeek/core/web/
--rw-rw-rw-   0        0        0     3075 2023-08-02 05:54:20.000000 moligeek-1.0.0/moligeek/core/web/__init__.py
--rw-rw-rw-   0        0        0     6177 2023-06-23 14:02:51.000000 moligeek-1.0.0/moligeek/core/web/imitate.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:25:44.325760 moligeek-1.0.0/moligeek/core/zip/
--rw-rw-rw-   0        0        0     5356 2023-08-02 05:54:20.000000 moligeek-1.0.0/moligeek/core/zip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:25:44.326757 moligeek-1.0.0/moligeek/database/
--rw-rw-rw-   0        0        0   155593 2023-06-23 14:02:51.000000 moligeek-1.0.0/moligeek/database/YiYan.dat
-drwxrwxrwx   0        0        0        0 2023-08-02 10:25:44.331850 moligeek-1.0.0/moligeek/path_dict/
--rw-rw-rw-   0        0        0    40710 2023-06-23 14:02:51.000000 moligeek-1.0.0/moligeek/path_dict/ASP.txt
--rw-rw-rw-   0        0        0    18013 2023-06-23 14:02:51.000000 moligeek-1.0.0/moligeek/path_dict/ASPX.txt
--rw-rw-rw-   0        0        0    23958 2023-06-23 14:02:51.000000 moligeek-1.0.0/moligeek/path_dict/DIR.txt
--rw-rw-rw-   0        0        0    13824 2023-06-23 14:02:51.000000 moligeek-1.0.0/moligeek/path_dict/JSP.txt
--rw-rw-rw-   0        0        0    10198 2023-06-23 14:02:51.000000 moligeek-1.0.0/moligeek/path_dict/MDB.txt
--rw-rw-rw-   0        0        0    21362 2023-06-23 14:02:51.000000 moligeek-1.0.0/moligeek/path_dict/PHP.txt
--rw-rw-rw-   0        0        0      303 2023-06-23 14:02:51.000000 moligeek-1.0.0/moligeek/path_dict/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:25:44.318261 moligeek-1.0.0/moligeek.egg-info/
--rw-rw-rw-   0        0        0     6332 2023-08-02 10:25:44.000000 moligeek-1.0.0/moligeek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      875 2023-08-02 10:25:44.000000 moligeek-1.0.0/moligeek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 10:25:44.000000 moligeek-1.0.0/moligeek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 09:02:13.000000 moligeek-1.0.0/moligeek.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2023-08-02 10:25:44.000000 moligeek-1.0.0/moligeek.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-02 10:25:44.000000 moligeek-1.0.0/moligeek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-08-01 06:48:22.000000 moligeek-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 10:25:44.332847 moligeek-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1661 2023-08-02 08:59:51.000000 moligeek-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.253470 moligeek-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-06-23 14:02:51.000000 moligeek-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-08-02 09:01:41.000000 moligeek-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6332 2023-08-02 12:08:34.253470 moligeek-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5492 2023-08-02 05:54:20.000000 moligeek-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.198316 moligeek-1.0.1/moligeek/
+-rw-rw-rw-   0        0        0     1605 2023-08-02 12:08:03.000000 moligeek-1.0.1/moligeek/__init__.py
+-rw-rw-rw-   0        0        0      340 2023-08-02 12:08:03.000000 moligeek-1.0.1/moligeek/__version__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.238183 moligeek-1.0.1/moligeek/core/
+drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.239178 moligeek-1.0.1/moligeek/core/LAN/
+-rw-rw-rw-   0        0        0       43 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/core/LAN/__init__.py
+-rw-rw-rw-   0        0        0     1206 2023-08-02 08:24:54.000000 moligeek-1.0.1/moligeek/core/LAN/scan.py
+-rw-rw-rw-   0        0        0      709 2023-08-02 08:24:54.000000 moligeek-1.0.1/moligeek/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.241172 moligeek-1.0.1/moligeek/core/encode/
+-rw-rw-rw-   0        0        0       42 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/core/encode/__init__.py
+-rw-rw-rw-   0        0        0     1097 2023-08-02 05:54:20.000000 moligeek-1.0.1/moligeek/core/encode/decode.py
+-rw-rw-rw-   0        0        0     1183 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/core/encode/fence.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.243166 moligeek-1.0.1/moligeek/core/network/
+-rw-rw-rw-   0        0        0     2053 2023-08-02 08:24:54.000000 moligeek-1.0.1/moligeek/core/network/__init__.py
+-rw-rw-rw-   0        0        0     1566 2023-08-02 08:24:54.000000 moligeek-1.0.1/moligeek/core/network/hostinfo.py
+-rw-rw-rw-   0        0        0     1418 2023-08-02 08:24:54.000000 moligeek-1.0.1/moligeek/core/network/wifi.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.245206 moligeek-1.0.1/moligeek/core/web/
+-rw-rw-rw-   0        0        0     3075 2023-08-02 05:54:20.000000 moligeek-1.0.1/moligeek/core/web/__init__.py
+-rw-rw-rw-   0        0        0     6177 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/core/web/imitate.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.246156 moligeek-1.0.1/moligeek/core/zip/
+-rw-rw-rw-   0        0        0     5356 2023-08-02 05:54:20.000000 moligeek-1.0.1/moligeek/core/zip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.246156 moligeek-1.0.1/moligeek/database/
+-rw-rw-rw-   0        0        0   155593 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/database/YiYan.dat
+drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.252044 moligeek-1.0.1/moligeek/path_dict/
+-rw-rw-rw-   0        0        0    40710 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/ASP.txt
+-rw-rw-rw-   0        0        0    18013 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/ASPX.txt
+-rw-rw-rw-   0        0        0    23958 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/DIR.txt
+-rw-rw-rw-   0        0        0    13824 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/JSP.txt
+-rw-rw-rw-   0        0        0    10198 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/MDB.txt
+-rw-rw-rw-   0        0        0    21362 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/PHP.txt
+-rw-rw-rw-   0        0        0      303 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.237186 moligeek-1.0.1/moligeek.egg-info/
+-rw-rw-rw-   0        0        0     6332 2023-08-02 12:08:33.000000 moligeek-1.0.1/moligeek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      875 2023-08-02 12:08:34.000000 moligeek-1.0.1/moligeek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 12:08:33.000000 moligeek-1.0.1/moligeek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 09:02:13.000000 moligeek-1.0.1/moligeek.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2023-08-02 12:08:33.000000 moligeek-1.0.1/moligeek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 12:08:33.000000 moligeek-1.0.1/moligeek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2023-08-01 06:48:22.000000 moligeek-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 12:08:34.253470 moligeek-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1661 2023-08-02 08:59:51.000000 moligeek-1.0.1/setup.py
```

### Comparing `moligeek-1.0.0/LICENSE` & `moligeek-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/PKG-INFO` & `moligeek-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moligeek
-Version: 1.0.0
+Version: 1.0.1
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
-Metadata-Version: 2.1 Name: moligeek Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: moligeek Version: 1.0.1 Summary:
 ä¸æ¬¾éæ¸å®åçpythonéæå·¥å·,åªåä¸ºå¼åèæä¾æå¤§çä¾¿å©
 Home-page: https://github.com/yourmoln/moligeek Author: yourmoln Author-email:
 yourmoln@outlook.com License: Apache 2.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `moligeek-1.0.0/README.md` & `moligeek-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/__init__.py` & `moligeek-1.0.1/moligeek/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 # -*- coding: utf-8 -*-
 # by yourmoln
-
 import sys
 import os
 script_path = os.path.split(os.path.realpath(__file__))[0]
 sys.path.append(script_path)
 import core
 import random
 import pickle
-print(core.__docs__)
-requirements_path = os.path.join(script_path, "../requirements.txt")
-for _ in range(3):
-    try:
-        import requests
-        import meo
-        import bs4
-        import pywifi
-        import tqdm
-        import asyncio
-        break
-    except:
-        source_list = [
-            "https://pypi.douban.com/simple",
-            "https://pypi.org/simple"
-        ]
-        print("有缺失的包，请选择一种下载方式: ")
-        print("\n".join([
-            f"[{i + 1}] {source}"
-            for i, source in enumerate(source_list)
-        ]))
-        idx = int(input("请输入序号(推荐使用1): ")) - 1
-        #requirements_path = os.path.join(script_path, "../requirements.txt")
-        os.system(
-            f"python -m pip install -r {requirements_path} -i {source_list[idx]}"
-        )
-        print("\a安装完成，开始运行")
+def start():
+    print(core.__docs__)
+    requirements_path = os.path.join(script_path, "../requirements.txt")
+    for _ in range(3):
+        try:
+            import requests
+            import meo
+            import bs4
+            import pywifi
+            import tqdm
+            import asyncio
+            break
+        except:
+            source_list = [
+                "https://pypi.douban.com/simple",
+                "https://pypi.org/simple"
+            ]
+            print("有缺失的包，请选择一种下载方式: ")
+            print("\n".join([
+                f"[{i + 1}] {source}"
+                for i, source in enumerate(source_list)
+            ]))
+            idx = int(input("请输入序号(推荐使用1): ")) - 1
+            #requirements_path = os.path.join(script_path, "../requirements.txt")
+            os.system(
+                f"python -m pip install -r {requirements_path} -i {source_list[idx]}"
+            )
+            print("\a安装完成，开始运行")
+    def yiyan():
+        with open(os.path.join(script_path, "./database/YiYan.dat"), "rb") as f:
+            YiYans = pickle.loads(f.read())
+        meo.screen.blue_font('一言:'+YiYans[str(random.randint(1, len(YiYans)))])
+    yiyan()
+
 
 import core.network as network
 import core.web as web
 import core.zip as zip
 import core.encode as encode
 import core.LAN as LAN
-
-with open(os.path.join(script_path, "./database/YiYan.dat"), "rb") as f:
-    YiYans = pickle.loads(f.read())
-meo.screen.blue_font('一言:'+YiYans[str(random.randint(1, len(YiYans)))])
```

### Comparing `moligeek-1.0.0/moligeek/core/LAN/scan.py` & `moligeek-1.0.1/moligeek/core/LAN/scan.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/core/__init__.py` & `moligeek-1.0.1/moligeek/core/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/core/encode/decode.py` & `moligeek-1.0.1/moligeek/core/encode/decode.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/core/encode/fence.py` & `moligeek-1.0.1/moligeek/core/encode/fence.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/core/network/__init__.py` & `moligeek-1.0.1/moligeek/core/network/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/core/network/hostinfo.py` & `moligeek-1.0.1/moligeek/core/network/hostinfo.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/core/network/wifi.py` & `moligeek-1.0.1/moligeek/core/network/wifi.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/core/web/__init__.py` & `moligeek-1.0.1/moligeek/core/web/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/core/web/imitate.py` & `moligeek-1.0.1/moligeek/core/web/imitate.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/core/zip/__init__.py` & `moligeek-1.0.1/moligeek/core/zip/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/database/YiYan.dat` & `moligeek-1.0.1/moligeek/database/YiYan.dat`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/path_dict/ASP.txt` & `moligeek-1.0.1/moligeek/path_dict/ASP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/path_dict/ASPX.txt` & `moligeek-1.0.1/moligeek/path_dict/ASPX.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/path_dict/DIR.txt` & `moligeek-1.0.1/moligeek/path_dict/DIR.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/path_dict/JSP.txt` & `moligeek-1.0.1/moligeek/path_dict/JSP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/path_dict/MDB.txt` & `moligeek-1.0.1/moligeek/path_dict/MDB.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek/path_dict/PHP.txt` & `moligeek-1.0.1/moligeek/path_dict/PHP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/moligeek.egg-info/PKG-INFO` & `moligeek-1.0.1/moligeek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moligeek
-Version: 1.0.0
+Version: 1.0.1
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
-Metadata-Version: 2.1 Name: moligeek Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: moligeek Version: 1.0.1 Summary:
 ä¸æ¬¾éæ¸å®åçpythonéæå·¥å·,åªåä¸ºå¼åèæä¾æå¤§çä¾¿å©
 Home-page: https://github.com/yourmoln/moligeek Author: yourmoln Author-email:
 yourmoln@outlook.com License: Apache 2.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `moligeek-1.0.0/moligeek.egg-info/SOURCES.txt` & `moligeek-1.0.1/moligeek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.0/setup.py` & `moligeek-1.0.1/setup.py`

 * *Files identical despite different names*

