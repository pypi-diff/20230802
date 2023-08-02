# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.8.7.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.8.7.tar", last modified: Mon Jul 31 09:04:58 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.8.8.tar", last modified: Wed Aug  2 11:03:03 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7.tar` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    28237 2023-07-31 09:00:33.044393 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6144 2023-07-30 13:05:57.372381 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    16374 2023-07-31 08:44:43.225031 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     7558 2023-07-31 08:51:57.113235 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    19733 2023-07-30 13:05:43.463072 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0    10785 2023-07-25 03:34:42.018245 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    46184 2023-07-31 08:52:09.570345 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     6353 2023-07-24 18:32:11.211285 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4677 2023-07-22 03:29:42.199501 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2066 2023-07-30 13:00:25.198724 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      724 2023-07-31 04:15:37.158867 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      730 2023-07-31 09:04:58.796581 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    28556 2023-08-02 11:02:48.070997 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6144 2023-07-30 13:05:57.372381 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    16512 2023-08-02 09:53:22.132707 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     7604 2023-08-02 03:51:33.221327 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    20867 2023-08-02 06:41:43.576286 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0    10785 2023-07-25 03:34:42.018245 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    47854 2023-08-02 11:02:49.349205 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     6353 2023-07-24 18:32:11.211285 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4677 2023-07-22 03:29:42.199501 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2066 2023-07-30 13:00:25.198724 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      724 2023-07-31 04:15:37.158867 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      730 2023-08-02 11:03:03.553261 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/pyproject.toml
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,22 @@
                            action="store_true", help="关闭自动匹配", dest="match")
 aidraw_parser.add_argument("-sr_on", "-sr-on", "-sr",
                            action="store_true", help="图片生产后再次超分", dest="sr")
 aidraw_parser.add_argument("-td", "--tiled-diffusion",
                            action="store_true", help="使用tiled-diffusion来生成图片", dest="td")
 # aidraw_parser.add_argument("-hr_e",
 #                            action=float, help="重绘幅度", dest="hr_strength")
+# aidraw_parser.add_argument("-acs", "--activate_custom_scripts",
+#                            action=int, help="启动自定义脚本生图", dest="custom_scripts")
+# aidraw_parser.add_argument("-xyz",
+#                            action=str, help="xyz生图", dest="xyz_plot")
+# aidraw_parser.add_argument("-sc", "--script", "--scripts",
+#                            action=int, help="脚本生图", dest="scripts")
+# aidraw_parser.add_argument("-ef", "--eye_fix",
+#                            action="store_true", help="使用ad插件修复脸部", dest="eye_fix")
 
 
 async def get_message_at(data: str) -> int:
     '''
     获取at列表
     :param data: event.json()
     '''
@@ -112,14 +120,15 @@
     parser=aidraw_parser,
     priority=5
 )
 
 
 @aidraw.handle()
 async def aidraw_get(bot: Bot, event: MessageEvent, args: Namespace = ShellCommandArgs()):
+    logger.debug(args.tags)
     tags_list = []
     model_info_ = ""
     random_tags = ""
     info_style = ""
     style_tag, style_ntag = "", ""
     user_id = str(event.user_id)
     if isinstance(event, PrivateMessageEvent):
@@ -165,15 +174,15 @@
                 message_id = message_data["message_id"]
                 loop = get_running_loop()
                 loop.call_later(
                     random.randint(30, 60),
                     lambda: loop.create_task(
                         bot.delete_msg(message_id=message_id)),
                 )
-        tags_list = tags_to_list(args.tags[0])
+        tags_list = await prepocess_tags(args.tags)
         if redis_client:
             if config.auto_match and args.match is False:
                 r = redis_client[1]
                 if r.exists("style"):
                     info_style = ""
                     style_list: list[bytes] = r.lrange("style", 0, -1)
                     style_list_: list[bytes] = r.lrange("user_style", 0, -1)
@@ -188,25 +197,16 @@
                                 if style["name"] in tag:
                                     style_ = style["name"]
                                     info_style += f"自动找到的预设: {style_}\n"
                                     style_tag += style["prompt"]  + ","
                                     style_ntag += style["negative_prompt"] + ","
                                     tags_list.pop(org_tag_list.index(tag))
                                     logger.info(info_style)
-                                    break
-                                 
-        org_str = []
-        convert_list = []
-        for tag in tags_list:
-            if "_" in tag:
-                org_str.append(tag)
-            else:
-                convert_list.append(tag)
-        args.tags = convert_list + org_str
-        args.tags = await prepocess_tags(args.tags, False)
+                                    break                       
+        args.tags = tags_list
         fifo = AIDRAW(**vars(args), event=event)
         fifo.extra_info += info_style
         
         if fifo.backend_index is not None and isinstance(fifo.backend_index, int):
             fifo.backend_name = config.backend_name_list[fifo.backend_index]
         else:
             await fifo.load_balance_init()
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,17 @@
         sampler: None or str = None,
         backend_index: str = None,
         disable_hr: bool = False if config.novelai_hr else True,
         hiresfix_scale: float = None,
         event: MessageEvent = None,
         sr: bool = False,
         model_index: str = None,
-        td: bool = False,
+        custom_scripts: int = None,
+        scripts: int = None,
+        td = None,
         **kwargs,
     ):
         """
         AI绘画的核心部分,将与服务器通信的过程包装起来,并方便扩展服务器类型
 
         :user_id: 用户id,必须
         :group_id: 群聊id,如果是私聊则应置为0,必须
@@ -132,14 +134,16 @@
         self.task_type: str = None
         self.img_hash = None
         self.extra_info = ""
         self.audit_info = ""
         self.sr = sr or config.novelai_SuperRes_generate
         self.model_index = model_index
         self.is_random_model = False
+        self.custom_scripts = custom_scripts
+        self.scripts = scripts
         self.td = td
         
         # 数值合法检查
         if self.steps <= 0 or self.steps > (36 if config.novelai_paid else 28):
             self.steps = 28
         if self.strength < 0 or self.strength > 1:
             self.strength = 0.7
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,16 @@
             "seed": self.seed,
             "steps": self.steps,
             "cfg_scale": self.scale,
             "width": self.width,
             "height": self.height,
             "negative_prompt": self.ntags,
             "sampler_name": self.sampler,
-            "denoising_strength": self.strength
+            "denoising_strength": self.strength,
+            "save_images": config.save_img
         }
         
         if self.model_index:
             from ..extension.sd_extra_api_func import sd
             model_dict = await sd(self.backend_index or config.backend_site_list.index(self.backend_site), True)
             self.model_index = self.model_index if self.model_index.isdigit() else await self.get_model_index(self.model_index, model_dict)
             if self.is_random_model:
@@ -94,15 +95,15 @@
         if self.img2img:
             if self.control_net["control_net"] and config.novelai_hr:
                 parameters.update(self.novelai_hr_payload)
             parameters.update({
                 "init_images": ["data:image/jpeg;base64,"+self.image],
                 "denoising_strength": self.strength,
             }
-            )
+            ) 
         else:
             if config.novelai_hr and self.disable_hr is False:
                 parameters.update(self.novelai_hr_payload)
             else:
                 self.hiresfix = False
         if self.td or config.tiled_diffusion:
             parameters.update({"alwayson_scripts": config.custom_scripts})
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,16 +92,52 @@
         novelai_size: int = novelai_size_org * novelai_hr_payload["hr_scale"]
     custom_scripts = {  # 自定义脚本此功能就可以使用webui上才能调用的插件, 需要自己去抓包
     "Tiled Diffusion": {
         "args": [True, "MultiDiffusion", False, True, 1024, 1024, 96, 96, 48, 1, "None", 2, False, 10, 1, []]
     },
     "Tiled VAE": {
         "args": [True, 1536, 96, False, True, True]
+    },
+    "ADetailer": {
+        "args": [
+        True, 
+        {
+    "ad_model": "mediapipe_face_mesh_eyes_only",
+    "ad_prompt": "",
+    "ad_negative_prompt": "",
+    "ad_confidence": 0.1,
+    "ad_mask_min_ratio": 0,
+    "ad_mask_max_ratio": 1,
+    "ad_x_offset": 0,
+    "ad_y_offset": 0,
+    "ad_dilate_erode": 4,
+    "ad_mask_merge_invert": "None",
+    "ad_mask_blur": 4,
+    "ad_denoising_strength": 0.4,
+    "ad_inpaint_only_masked": True,
+    "ad_inpaint_only_masked_padding": 32,
+    "ad_use_inpaint_width_height": False,
+    "ad_inpaint_width": 512,
+    "ad_inpaint_height": 512,
+    "ad_use_steps": False,
+    "ad_steps": 28,
+    "ad_use_cfg_scale": False,
+    "ad_cfg_scale": 7,
+    "ad_use_sampler": False,
+    "ad_sampler": "Euler a",
+    "ad_use_noise_multiplier": False,
+    "ad_noise_multiplier": 1,
+    "ad_use_clip_skip": False,
+    "ad_clip_skip": 1,
+    "ad_restore_face": False
+                }
+            ]
+        }
     }
-    }
+    scripts = [{"name": "x/y/z plot", "args": [9, "", ["DDIM", "Euler a", "Euler"], 0, "", "", 0, "", ""]}]
     novelai_ControlNet_payload: list = [
         {
             "alwayson_scripts": {
             "controlnet": {
             "args": [
                 {
                 "input_image": "",
@@ -154,14 +190,15 @@
     auto_match = True  # 是否自动匹配
     hr_off_when_cn = True  # 使用controlnet功能的时候关闭高清修复
     backend_name_list = []
     backend_site_list = []
     only_super_user = True  # 只有超级用户才能永久更换模型, 雕雕没有小号来测试了, 悲
     tiled_diffusion = False  # 使用tiled-diffusion来生成图片
     enable_scripts = False  # 是否启动custom_scripts中设置的自定义脚本
+    save_img = True  # 是否保存图片(API侧)
     # 允许单群设置的设置
     def keys(cls):
         return ("novelai_cd", "novelai_tags", "novelai_on", "novelai_ntags", "novelai_revoke", "novelai_h", "novelai_htype", "novelai_picaudit", "novelai_pure", "novelai_site")
 
     def __getitem__(cls, item):
         return getattr(cls, item)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 reload_ = on_command("卸载模型", aliases={"释放显存"})
 style_ = on_command("预设")
 rembg = on_command("去背景", aliases={"rembg", "抠图"})
 read_png_info = on_command("读图", aliases={"读png", "读PNG"})
 random_pic = on_command("随机出图", aliases={"随机模型", "随机画图"})
 refresh_models = on_command("刷新模型")
 stop_all_mission = on_command("终止生成")
+get_scripts = on_command("获取脚本")
 
 more_func_parser, style_parser = ArgumentParser(), ArgumentParser()
 more_func_parser.add_argument("-i", "--index", type=int, help="设置索引", dest="index")
 more_func_parser.add_argument("-v", "--value", type=str, help="设置值", dest="value")
 more_func_parser.add_argument("-s", "--search", type=str, help="搜索设置名", dest="search")
 style_parser.add_argument("tags", type=str, nargs="*", help="正面提示词")
 style_parser.add_argument("-f", "--find", type=str, help="寻找预设", dest="find_style_name")
@@ -111,14 +112,29 @@
 style_ = on_shell_command(
     "预设",
     parser=style_parser,
     priority=5
 )
 
 
+class GET_API():
+    
+    def __init__(self, 
+                site: str = None,
+                end_point: str = None
+    ) -> None:
+        self.site = site
+        self.end_point = end_point
+        self.task_list = []
+    
+    async def get_all_resp(self):
+        pass
+    
+
+
 async def get_random_tags(sample_num=12):
     try:
         if redis_client:
             r = redis_client[0]
             all_tags_list = []
             all_tags_list_str = [] 
             byte_tags_list = r.lrange("prompts", 0, -1)
@@ -1125,8 +1141,40 @@
             await stop_all_mission.finish("笨蛋!后端编号是数字啦!!")
     else:
         extra_msg = "所有"
         for backend in config.backend_site_list:
             backend_url = f"http://{backend}/sdapi/v1/interrupt" 
             task_list.append(aiohttp_func("post", backend_url))
     _ = await asyncio.gather(*task_list, return_exceptions=False)
-    await stop_all_mission.finish(f"终止{extra_msg}任务成功")
+    await stop_all_mission.finish(f"终止{extra_msg}任务成功")
+    
+    
+@get_scripts.handle()
+async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
+    script_index = None
+    select_script_args = None
+    script_name = []
+    
+    if msg is not None:
+        text_msg = msg.extract_plain_text()
+        if "_" in text_msg:
+            backend = config.backend_site_list[int(text_msg.split("_")[0])]
+            script_index = int(text_msg.split("_")[1])
+        else:
+            if text_msg.isdigit():
+                backend = config.backend_site_list[int(text_msg)]
+            else:
+                await get_scripts.finish("笨蛋!后端编号是数字啦!!")
+                
+        backend_url = f"http://{backend}/sdapi/v1/script-info"
+        resp = await aiohttp_func("get", backend_url)
+        for script in resp[0]:
+            name = script["name"]
+            script_name.append(f"{name}\n")
+        if script_index:
+            select_script_args = resp[0][script_index]["args"]
+            print(select_script_args)
+            await risk_control(bot, event, str(select_script_args), True)
+        await risk_control(bot, event, script_name, True)
+        
+    else:
+        await get_scripts.finish("请按照以下格式获取脚本信息\n例如 获取脚本0 再使用 获取脚本0_2 查看具体脚本所需的参数")
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.8.7/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.3.9.8.7"
+version = "0.3.9.8.8"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

