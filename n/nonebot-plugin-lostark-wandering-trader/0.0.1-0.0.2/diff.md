# Comparing `tmp/nonebot_plugin_lostark_wandering_trader-0.0.1.tar.gz` & `tmp/nonebot_plugin_lostark_wandering_trader-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nonebot_plugin_lostark_wandering_trader-0.0.1.tar", last modified: Wed Aug  2 06:04:36 2023, max compression
+gzip compressed data, was "dist/nonebot_plugin_lostark_wandering_trader-0.0.2.tar", last modified: Wed Aug  2 06:24:16 2023, max compression
```

## Comparing `nonebot_plugin_lostark_wandering_trader-0.0.1.tar` & `nonebot_plugin_lostark_wandering_trader-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-02 06:04:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/
--rw-r--r--   0 gongmin    (501) staff       (20)     4422 2023-08-02 06:04:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/PKG-INFO
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-02 06:04:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/nonebot_plugin_lostark_wandering_trader/
--rw-r--r--   0 gongmin    (501) staff       (20)      216 2023-08-02 03:29:55.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/nonebot_plugin_lostark_wandering_trader/config.py
--rw-r--r--   0 gongmin    (501) staff       (20)     7749 2023-08-02 05:58:14.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/nonebot_plugin_lostark_wandering_trader/__init__.py
--rw-r--r--   0 gongmin    (501) staff       (20)     2982 2023-08-02 06:00:15.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/README.md
--rw-r--r--   0 gongmin    (501) staff       (20)     1285 2023-08-02 06:03:50.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/setup.py
--rw-r--r--   0 gongmin    (501) staff       (20)       38 2023-08-02 06:04:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/setup.cfg
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-02 06:04:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/nonebot_plugin_lostark_wandering_trader.egg-info/
--rw-r--r--   0 gongmin    (501) staff       (20)     4422 2023-08-02 06:04:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO
--rw-r--r--   0 gongmin    (501) staff       (20)      434 2023-08-02 06:04:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/nonebot_plugin_lostark_wandering_trader.egg-info/SOURCES.txt
--rw-r--r--   0 gongmin    (501) staff       (20)      126 2023-08-02 06:04:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/nonebot_plugin_lostark_wandering_trader.egg-info/requires.txt
--rw-r--r--   0 gongmin    (501) staff       (20)       40 2023-08-02 06:04:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/nonebot_plugin_lostark_wandering_trader.egg-info/top_level.txt
--rw-r--r--   0 gongmin    (501) staff       (20)        1 2023-08-02 06:04:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.1/nonebot_plugin_lostark_wandering_trader.egg-info/dependency_links.txt
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-02 06:24:16.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/
+-rw-r--r--   0 gongmin    (501) staff       (20)     4418 2023-08-02 06:24:16.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/PKG-INFO
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-02 06:24:16.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/nonebot_plugin_lostark_wandering_trader/
+-rw-r--r--   0 gongmin    (501) staff       (20)      216 2023-08-02 03:29:55.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/nonebot_plugin_lostark_wandering_trader/config.py
+-rw-r--r--   0 gongmin    (501) staff       (20)     7748 2023-08-02 06:23:04.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/nonebot_plugin_lostark_wandering_trader/__init__.py
+-rw-r--r--   0 gongmin    (501) staff       (20)     2978 2023-08-02 06:23:00.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/README.md
+-rw-r--r--   0 gongmin    (501) staff       (20)     1285 2023-08-02 06:23:59.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/setup.py
+-rw-r--r--   0 gongmin    (501) staff       (20)       38 2023-08-02 06:24:16.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/setup.cfg
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-02 06:24:16.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/nonebot_plugin_lostark_wandering_trader.egg-info/
+-rw-r--r--   0 gongmin    (501) staff       (20)     4418 2023-08-02 06:24:16.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO
+-rw-r--r--   0 gongmin    (501) staff       (20)      434 2023-08-02 06:24:16.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/nonebot_plugin_lostark_wandering_trader.egg-info/SOURCES.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)      126 2023-08-02 06:24:16.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/nonebot_plugin_lostark_wandering_trader.egg-info/requires.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)       40 2023-08-02 06:24:16.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/nonebot_plugin_lostark_wandering_trader.egg-info/top_level.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)        1 2023-08-02 06:24:16.000000 nonebot_plugin_lostark_wandering_trader-0.0.2/nonebot_plugin_lostark_wandering_trader.egg-info/dependency_links.txt
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.1/PKG-INFO` & `nonebot_plugin_lostark_wandering_trader-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_lostark_wandering_trader
-Version: 0.0.1
+Version: 0.0.2
 Summary: NoneBot lostark cn wandering trader plugin
 Home-page: https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader
 Author: EmiyaGm
 Author-email: 464723943@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader/issues
 Description: 
@@ -24,19 +24,19 @@
         # nonebot-plugin-lostark-wandering-trader
         
         _✨ NoneBot 命运方舟国服流浪商人刷新时间查看 自动播报稀有及其以上卡牌刷新 插件 ✨_
         
         </div>
         
         <p align="center">
-          <a href="https://raw.githubusercontent.com/emiyagm/nonebot-plugin-loastark-wandering-trader/main/LICENSE">
-            <img src="https://img.shields.io/github/license/emiyagm/nonebot-plugin-loastark-wandering-trader.svg" alt="license">
+          <a href="https://raw.githubusercontent.com/emiyagm/nonebot-plugin-lostark-wandering-trader/main/LICENSE">
+            <img src="https://img.shields.io/github/license/emiyagm/nonebot-plugin-lostark-wandering-trader.svg" alt="license">
           </a>
-          <a href="https://pypi.python.org/pypi/nonebot-plugin-loastark-wandering-trader">
-            <img src="https://img.shields.io/pypi/v/nonebot-plugin-loastark-wandering-trader.svg" alt="pypi">
+          <a href="https://pypi.python.org/pypi/nonebot-plugin-lostark-wandering-trader">
+            <img src="https://img.shields.io/pypi/v/nonebot-plugin-lostark-wandering-trader.svg" alt="pypi">
           </a>
           <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
         </p>
         
         ## 使用方式
         
         通用:
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: nonebot_plugin_lostark_wandering_trader Version:
-0.0.1 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
+0.0.2 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
 github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader Author: EmiyaGm
 Author-email: 464723943@qq.com License: UNKNOWN Project-URL: Bug Tracker,
 https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader/issues
 Description:
                                    [nonebot]
             # nonebot-plugin-lostark-wandering-trader _â¨ NoneBot
                å½è¿æ¹èå½ææµæµªåäººå·æ°æ¶é´æ¥ç
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.1/nonebot_plugin_lostark_wandering_trader/__init__.py` & `nonebot_plugin_lostark_wandering_trader-0.0.2/nonebot_plugin_lostark_wandering_trader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .config import Config
 
 __plugin_meta__ = PluginMetadata(
     name="命运方舟流浪商人卡牌刷新提示",
     description="国服命运方舟流浪商人稀有史诗传说卡牌刷新提示",
     usage="nb plugin install nonebot_plugin_lostark_wandering_trader",
     type="application",
-    homepage="https://github.com/EmiyaGm/nonebot-plugin-loastark-wandering-trader",
+    homepage="https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader",
     config=Config,
     extra={},
     supported_adapters={"~onebot.v11"},
 )
 
 require("nonebot_plugin_apscheduler")
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.1/README.md` & `nonebot_plugin_lostark_wandering_trader-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # nonebot-plugin-lostark-wandering-trader
 
 _✨ NoneBot 命运方舟国服流浪商人刷新时间查看 自动播报稀有及其以上卡牌刷新 插件 ✨_
 
 </div>
 
 <p align="center">
-  <a href="https://raw.githubusercontent.com/emiyagm/nonebot-plugin-loastark-wandering-trader/main/LICENSE">
-    <img src="https://img.shields.io/github/license/emiyagm/nonebot-plugin-loastark-wandering-trader.svg" alt="license">
+  <a href="https://raw.githubusercontent.com/emiyagm/nonebot-plugin-lostark-wandering-trader/main/LICENSE">
+    <img src="https://img.shields.io/github/license/emiyagm/nonebot-plugin-lostark-wandering-trader.svg" alt="license">
   </a>
-  <a href="https://pypi.python.org/pypi/nonebot-plugin-loastark-wandering-trader">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-loastark-wandering-trader.svg" alt="pypi">
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-lostark-wandering-trader">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-lostark-wandering-trader.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
 </p>
 
 ## 使用方式
 
 通用:
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.1/setup.py` & `nonebot_plugin_lostark_wandering_trader-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = "NoneBot lostark cn wandering trader plugin"
 
 setuptools.setup(
     name="nonebot_plugin_lostark_wandering_trader",
-    version="0.0.1",
+    version="0.0.2",
     author="EmiyaGm",
     author_email="464723943@qq.com",
     description="NoneBot lostark cn wandering trader plugin",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader",
     project_urls={
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.1/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO` & `nonebot_plugin_lostark_wandering_trader-0.0.2/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-lostark-wandering-trader
-Version: 0.0.1
+Version: 0.0.2
 Summary: NoneBot lostark cn wandering trader plugin
 Home-page: https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader
 Author: EmiyaGm
 Author-email: 464723943@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader/issues
 Description: 
@@ -24,19 +24,19 @@
         # nonebot-plugin-lostark-wandering-trader
         
         _✨ NoneBot 命运方舟国服流浪商人刷新时间查看 自动播报稀有及其以上卡牌刷新 插件 ✨_
         
         </div>
         
         <p align="center">
-          <a href="https://raw.githubusercontent.com/emiyagm/nonebot-plugin-loastark-wandering-trader/main/LICENSE">
-            <img src="https://img.shields.io/github/license/emiyagm/nonebot-plugin-loastark-wandering-trader.svg" alt="license">
+          <a href="https://raw.githubusercontent.com/emiyagm/nonebot-plugin-lostark-wandering-trader/main/LICENSE">
+            <img src="https://img.shields.io/github/license/emiyagm/nonebot-plugin-lostark-wandering-trader.svg" alt="license">
           </a>
-          <a href="https://pypi.python.org/pypi/nonebot-plugin-loastark-wandering-trader">
-            <img src="https://img.shields.io/pypi/v/nonebot-plugin-loastark-wandering-trader.svg" alt="pypi">
+          <a href="https://pypi.python.org/pypi/nonebot-plugin-lostark-wandering-trader">
+            <img src="https://img.shields.io/pypi/v/nonebot-plugin-lostark-wandering-trader.svg" alt="pypi">
           </a>
           <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
         </p>
         
         ## 使用方式
         
         通用:
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: nonebot-plugin-lostark-wandering-trader Version:
-0.0.1 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
+0.0.2 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
 github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader Author: EmiyaGm
 Author-email: 464723943@qq.com License: UNKNOWN Project-URL: Bug Tracker,
 https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader/issues
 Description:
                                    [nonebot]
             # nonebot-plugin-lostark-wandering-trader _â¨ NoneBot
                å½è¿æ¹èå½ææµæµªåäººå·æ°æ¶é´æ¥ç
```

