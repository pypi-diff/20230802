# Comparing `tmp/nonebot_plugin_savepic-0.1.2.tar.gz` & `tmp/nonebot_plugin_savepic-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_savepic-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_savepic-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_savepic-0.1.2.tar` & `nonebot_plugin_savepic-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1060 2023-08-01 22:07:58.926782 nonebot_plugin_savepic-0.1.2/LICENSE
--rw-r--r--   0        0        0     1984 2023-08-01 22:07:58.926782 nonebot_plugin_savepic-0.1.2/README.md
--rw-r--r--   0        0        0     5631 2023-08-01 22:07:58.926782 nonebot_plugin_savepic-0.1.2/nonebot_plugin_savepic/__init__.py
--rw-r--r--   0        0        0      181 2023-08-01 22:07:58.926782 nonebot_plugin_savepic-0.1.2/nonebot_plugin_savepic/config.py
--rw-r--r--   0        0        0      846 2023-08-01 22:07:58.926782 nonebot_plugin_savepic-0.1.2/nonebot_plugin_savepic/migrations/1a654e02179b_.py
--rw-r--r--   0        0        0      581 2023-08-01 22:07:58.926782 nonebot_plugin_savepic-0.1.2/nonebot_plugin_savepic/model.py
--rw-r--r--   0        0        0     4948 2023-08-01 22:07:58.926782 nonebot_plugin_savepic-0.1.2/nonebot_plugin_savepic/pic_sql.py
--rw-r--r--   0        0        0      971 2023-08-01 22:07:58.926782 nonebot_plugin_savepic-0.1.2/nonebot_plugin_savepic/rule.py
--rw-r--r--   0        0        0      553 2023-08-01 22:07:58.926782 nonebot_plugin_savepic-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2688 1970-01-01 00:00:00.000000 nonebot_plugin_savepic-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1984 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/README.md
+-rw-r--r--   0        0        0     5684 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/__init__.py
+-rw-r--r--   0        0        0      181 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/config.py
+-rw-r--r--   0        0        0      846 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/migrations/1a654e02179b_.py
+-rw-r--r--   0        0        0      581 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/model.py
+-rw-r--r--   0        0        0     4948 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/pic_sql.py
+-rw-r--r--   0        0        0      971 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/rule.py
+-rw-r--r--   0        0        0      553 2023-08-01 22:20:09.069478 nonebot_plugin_savepic-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2688 1970-01-01 00:00:00.000000 nonebot_plugin_savepic-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_savepic-0.1.2/LICENSE` & `nonebot_plugin_savepic-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.2/README.md` & `nonebot_plugin_savepic-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.2/nonebot_plugin_savepic/__init__.py` & `nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 /savepic -d <文件名> 删除图图片
 /savepic -m <原文件名> <新文件名> 重命名图片
 /randpic <关键词> 随机图片
 <文件名> 发送图片""",
     config=Config,
     homepage="https://github.com/Yan-Zero/nonebot-plugin-savepic",
     type="application",
+    supported_adapters=[
+        '~onebot.v11'
+    ]
 )
 
 INVALID_FILENAME_CHARACTERS = r'\/:*?"<>|'
 
 global_config = get_driver().config
 p_config = Config.parse_obj(global_config)
```

### Comparing `nonebot_plugin_savepic-0.1.2/nonebot_plugin_savepic/migrations/1a654e02179b_.py` & `nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/migrations/1a654e02179b_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.2/nonebot_plugin_savepic/model.py` & `nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.2/nonebot_plugin_savepic/pic_sql.py` & `nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/pic_sql.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.2/nonebot_plugin_savepic/rule.py` & `nonebot_plugin_savepic-0.1.3/nonebot_plugin_savepic/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_savepic-0.1.2/pyproject.toml` & `nonebot_plugin_savepic-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-savepic"
-version = "0.1.2"
+version = "0.1.3"
 description = "保存表情包（语录）与随机出图"
 authors = ["Yan <1964649083@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_savepic"}]
 homepage = "https://github.com/Yan-Zero/nonebot-plugin-savepic"
```

### Comparing `nonebot_plugin_savepic-0.1.2/PKG-INFO` & `nonebot_plugin_savepic-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-savepic
-Version: 0.1.2
+Version: 0.1.3
 Summary: 保存表情包（语录）与随机出图
 Home-page: https://github.com/Yan-Zero/nonebot-plugin-savepic
 License: MIT
 Author: Yan
 Author-email: 1964649083@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-savepic Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-savepic Version: 0.1.3 Summary:
 ä¿å­è¡¨æåï¼è¯­å½ï¼ä¸éæºåºå¾ Home-page: https://github.com/Yan-
 Zero/nonebot-plugin-savepic License: MIT Author: Yan Author-email:
 1964649083@qq.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: asyncpg (>=0.28.0,<0.29.0) Requires-
 Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-
```

