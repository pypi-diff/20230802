# Comparing `tmp/nonebot_plugin_blocker-0.3.7.tar.gz` & `tmp/nonebot_plugin_blocker-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blocker-0.3.7.tar", last modified: Mon Jul 31 20:46:37 2023, max compression
+gzip compressed data, was "nonebot_plugin_blocker-0.3.8.tar", last modified: Wed Aug  2 20:11:07 2023, max compression
```

## Comparing `nonebot_plugin_blocker-0.3.7.tar` & `nonebot_plugin_blocker-0.3.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-07-31 20:46:16.550772 nonebot_plugin_blocker-0.3.7/LICENSE
--rw-r--r--   0        0        0     2950 2023-07-31 20:46:16.550772 nonebot_plugin_blocker-0.3.7/README.md
--rw-r--r--   0        0        0      381 2023-07-31 20:46:16.550772 nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0        0        0     3231 2023-07-31 20:46:16.550772 nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0        0        0     3684 2023-07-31 20:46:16.550772 nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/config.py
--rw-r--r--   0        0        0     2709 2023-07-31 20:46:16.550772 nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/web/__init__.py
--rw-r--r--   0        0        0     3208 2023-07-31 20:46:16.554772 nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/web/webpage/main.html
--rw-r--r--   0        0        0     6180 2023-07-31 20:46:16.554772 nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/web/webpage/main.js
--rw-r--r--   0        0        0     2292 2023-07-31 20:46:16.554772 nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/web/webpage/style.css
--rw-r--r--   0        0        0      640 2023-07-31 20:46:37.519620 nonebot_plugin_blocker-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     4560 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-02 20:10:51.280478 nonebot_plugin_blocker-0.3.8/LICENSE
+-rw-r--r--   0        0        0     2950 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/README.md
+-rw-r--r--   0        0        0      381 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0        0        0     3242 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0        0        0     3928 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/config.py
+-rw-r--r--   0        0        0     2709 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/__init__.py
+-rw-r--r--   0        0        0     3208 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/webpage/main.html
+-rw-r--r--   0        0        0     6180 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/webpage/main.js
+-rw-r--r--   0        0        0     2292 2023-08-02 20:10:51.284478 nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/webpage/style.css
+-rw-r--r--   0        0        0      640 2023-08-02 20:11:07.584829 nonebot_plugin_blocker-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     4560 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.8/PKG-INFO
```

### Comparing `nonebot_plugin_blocker-0.3.7/LICENSE` & `nonebot_plugin_blocker-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.7/README.md` & `nonebot_plugin_blocker-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/__main__.py` & `nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from nonebot.exception import IgnoredException
 
 import re
 from .config import BlockerList, get_reply_config, reply_config_raw
 from . import web
 
 blockerlist: BlockerList
-    
+
 driver.server_app.mount("/blocker-webui", web.app, name="blocker-webui")
 
 @driver.on_startup
 async def load_blocker_on_start():
     global blockerlist
     blockerlist = BlockerList()
     logger.info("[Blocker]WebUI is now listening on "
@@ -31,40 +31,41 @@
     global blockerlist
     del blockerlist
     
 async def msg_checker_rule(event: GroupMessageEvent, state: T_State) -> bool:
     if (re.search("[at:qq=\d+]", event.get_plaintext()) and not event.is_tome()) or event.user_id == event.self_id:
         return False # 如果是骰子自己发的或者当发现at了任何人但不是骰子的时候不执行
     try:
-        reply_config: dict = get_reply_config().get(str(event.self_id))
+        reply_config = get_reply_config().get(str(event.self_id))
         for arg in ["on","off"]:
             if re.match(reply_config.get("command_"+arg)+"$", event.get_plaintext()):
                 state["blocker_state"] = "reply_"+arg
                 state["this_reply"] = reply_config.get(state["blocker_state"])
     except (AttributeError,KeyError,TypeError):
-        if match := re.match("[.。]bot (on|off)\s?(|\[at:qq=\d+\])", event.get_plaintext()):
+        if match := re.match("[.。]bot (on|off)\s?(|[at:qq=\d+])", event.get_plaintext()):
             state["blocker_state"] = "reply_"+match.group(1)
             state["this_reply"] = reply_config_raw.get(state["blocker_state"])
     state["blocker_type"] = blockerlist.blocker_type.get(str(event.self_id), False)
     return True if "blocker_state" in state else False  
     
 blocker = on_message(rule=msg_checker_rule, permission=GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=1, block=True)
 
 @run_preprocessor
 async def blocker_hook(matcher: Matcher, event: GroupMessageEvent):
-    if blockerlist.check_blocker(event.group_id, str(event.self_id), matcher.plugin_name):
+    if blockerlist(event.group_id, str(event.self_id), matcher.plugin_name):
         logger.info("[Blocker]Your Message is Blocked By Blocker.")
         raise IgnoredException("[Blocker]Matcher Blocked By Blocker")
         
 @blocker.handle()
 async def blocker_msg_handle(matcher: Matcher, event: GroupMessageEvent, state: T_State):
     assert state["this_reply"] and state["blocker_state"]
     msg_type = state["this_reply"].get("type")
     msg_data = state["this_reply"].get("data")
     if (state["blocker_state"] == "reply_on") ^ state["blocker_type"]:
         blockerlist.del_blocker(event.group_id, str(event.self_id))
     else:
         blockerlist.add_blocker(event.group_id, str(event.self_id))
+    await blockerlist.save_blocker()
     if msg_type == "text":
         await matcher.finish(msg_data)
     else:
         await matcher.finish(MessageSegment(type=msg_type, data={"file":msg_data}))
```

### Comparing `nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/config.py` & `nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pydantic import BaseModel, Field
 from pathlib import Path
 from typing import Dict, Optional
 from nonebot import get_driver, logger
+import asyncio
 import json
 
 DATA_PATH = Path.cwd() / "data" / "blocker"
 if not DATA_PATH.exists():
     DATA_PATH.mkdir(parents=True)
 
 BLOCKLIST_JSON_PATH = DATA_PATH / "blocklist.json"
@@ -18,14 +19,23 @@
 
 REPLY_JSON_PATH = DATA_PATH / "config.json"
 if not REPLY_JSON_PATH.exists():
     REPLY_JSON_PATH.write_text("{}",encoding="u8")
     
 reply_config_raw = {"reply_on": {"type": "text", "data": "在本群开启"}, "reply_off": {"type": "text", "data": "在本群关闭"}}
 
+class JsonEncoder(json.JSONEncoder):
+    sort_keys = True
+    indent = 4
+    ensure_ascii = False
+    def default(self, obj):
+        if isinstance(obj, set):
+            return list(obj)
+        return json.JSONEncoder.default(self, obj)
+
 class PluginConfigModel(BaseModel):
     WEBUI_USERNAME: Optional[str] = Field(None, alias="blocker_webui_username")
     WEBUI_PASSWORD: Optional[str] = Field(None, alias="blocker_webui_password")
     
 class ReplyModel(BaseModel):
     type: str
     data: Optional[str]
@@ -43,64 +53,60 @@
 def get_reply_config() -> dict:
     config = json.load(REPLY_JSON_PATH.open("r", encoding="u8"))
     if not isinstance(config, dict):
         config = {}
     return config
 
 def save_reply_config(config_list: ConfigModel):
-    REPLY_JSON_PATH.write_text(config_list.json(),encoding="u8")
+    REPLY_JSON_PATH.write_text(config_list.json(sort_keys=True, indent=4), encoding="u8")
         
 class BlockerList:
-    blocklist: dict[str, list[int]] = {}
+    blocklist: dict[str, set[int]] = {}
     blocker_type: dict[str, bool] = {}
     
     def __init__(self):
-        self.blocklist = json.load(BLOCKLIST_JSON_PATH.open("r",encoding="u8"))
+        raw_list = json.load(BLOCKLIST_JSON_PATH.open("r",encoding="u8"))
         config = get_reply_config()
-        if not isinstance(self.blocklist, dict):
-            self.blocklist = {}
-        for uin in self.blocklist.keys():
-            this_blocker_type = config.get(uin, {}).get("blocker_type", False)
-            self.blocker_type.setdefault(uin, this_blocker_type)
+        if not isinstance(raw_list, dict):
+            raw_list = {}
+        self.blocklist = {uin: set(val) for uin, val in raw_list.items()}
+        self.blocker_type = {uin: val.get("blocker_type", False) for uin, val in config.items()}
         
     def add_blocker(self,gid: int, uin: str):
         try:
-            self.blocklist.get(uin).index(gid)
-        except ValueError:
-            self.blocklist.get(uin).append(gid)
+            self.blocklist.get(uin).add(gid)
+            logger.info("[Blocker]Add Blocker Successful.")
         except AttributeError:
-            self.blocklist.setdefault(uin,[gid])
+            self.blocklist.setdefault(uin,set([gid]))
+            logger.info("[Blocker]Add Blocker Successful.")
         except:
             logger.info("[Blocker]Add Blocker Failed.")
-            return
-        logger.info("[Blocker]Add Blocker Successful.")
-        
-        
+
     def del_blocker(self,gid: int, uin: str):
         try:
             self.blocklist.get(uin).remove(gid)
             logger.info("[Blocker]Delete Blocker Successful.")
-        except ValueError:
+        except (AttributeError,ValueError):
             logger.info("[Blocker]Delete Blocker Failed.")
     
     def change_blocker_type(self,uin: str, val: bool = False):
         try:
             self.blocker_type[uin] = val
         except KeyError:
             self.blocker_type.setdefault(uin, val)
-        
-    def check_blocker(self,gid: int, uin: str, module_name: str) -> bool:
-        try: 
-            module_name.index("nonebot_plugin_blocker")
+    
+    def __call__(self,gid: int, uin: str, module_name: str) -> bool:
+        if "nonebot_plugin_blocker" in module_name:
             return False
-        except ValueError:
-            try:
-                self.blocklist.get(uin).index(gid)
-                return not self.blocker_type.get(uin, False)
-            except ValueError:
-                return self.blocker_type.get(uin, False)
+        return (gid in self.blocklist.get(uin)) ^ self.blocker_type.get(uin, False)
 
+    async def save_blocker(self):
+        try:
+            BLOCKLIST_JSON_PATH.write_text(JsonEncoder().encode(self.blocklist))
+            logger.info("[Blocker]Save Blocker Successful.")
+        except:
+            logger.info("[Blocker]Save Blocker Failed.")
+        
     def __del__(self):
-        json.dump(self.blocklist,BLOCKLIST_JSON_PATH.open("w",encoding="u8"),ensure_ascii=False)
+        asyncio.get_running_loop().create_task(self.save_blocker())
         
-driver_config = get_driver().config
-config = PluginConfigModel.parse_obj(driver_config.dict())
+config = PluginConfigModel.parse_obj(get_driver().config.dict())
```

### Comparing `nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/web/__init__.py` & `nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/web/webpage/main.html` & `nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/webpage/main.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/web/webpage/main.js` & `nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/webpage/main.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.7/nonebot_plugin_blocker/web/webpage/style.css` & `nonebot_plugin_blocker-0.3.8/nonebot_plugin_blocker/web/webpage/style.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.7/pyproject.toml` & `nonebot_plugin_blocker-0.3.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-blocker"
-version = "0.3.7"
+version = "0.3.8"
 description = "Message Blocker"
 authors = [
     { name = "MerCuJerry", email = "mercujerry@gmail.com" },
 ]
 keywords = [
     "nonebot",
     "nonebot2",
```

### Comparing `nonebot_plugin_blocker-0.3.7/PKG-INFO` & `nonebot_plugin_blocker-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.3.7
+Version: 0.3.8
 Summary: Message Blocker
 Keywords: nonebot nonebot2 qqbot bot
 Home-page: https://github.com/MerCuJerry/nonebot-plugin-blocker
 Author-Email: MerCuJerry <mercujerry@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 MerCuJerry
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.8 Summary:
 Message Blocker Keywords: nonebot nonebot2 qqbot bot Home-page: https://
 github.com/MerCuJerry/nonebot-plugin-blocker Author-Email: MerCuJerry
 gmail.com> License: MIT License Copyright (c) 2023 MerCuJerry Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

