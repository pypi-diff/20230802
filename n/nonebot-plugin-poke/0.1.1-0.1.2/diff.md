# Comparing `tmp/nonebot_plugin_poke-0.1.1.tar.gz` & `tmp/nonebot_plugin_poke-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_poke-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_poke-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_poke-0.1.1.tar` & `nonebot_plugin_poke-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-30 15:54:55.968021 nonebot_plugin_poke-0.1.1/LICENSE
--rw-r--r--   0        0        0     3045 2023-07-30 15:54:55.968021 nonebot_plugin_poke-0.1.1/README.md
--rw-r--r--   0        0        0     5209 2023-07-30 15:54:55.968021 nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/__init__.py
--rw-r--r--   0        0        0      727 2023-07-30 15:54:55.968021 nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/config.py
--rw-r--r--   0        0        0     1280 2023-07-30 15:54:55.972021 nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/matcher.py
--rw-r--r--   0        0        0     5115 2023-07-30 15:54:55.972021 nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/utils.py
--rw-r--r--   0        0        0     1682 2023-07-30 15:54:55.972021 nonebot_plugin_poke-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-02 08:32:07.992534 nonebot_plugin_poke-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3134 2023-08-02 08:32:07.992534 nonebot_plugin_poke-0.1.2/README.md
+-rw-r--r--   0        0        0     2785 2023-08-02 08:32:07.992534 nonebot_plugin_poke-0.1.2/nonebot_plugin_poke/__init__.py
+-rw-r--r--   0        0        0      727 2023-08-02 08:32:07.992534 nonebot_plugin_poke-0.1.2/nonebot_plugin_poke/config.py
+-rw-r--r--   0        0        0     1280 2023-08-02 08:32:07.992534 nonebot_plugin_poke-0.1.2/nonebot_plugin_poke/matcher.py
+-rw-r--r--   0        0        0     5115 2023-08-02 08:32:07.992534 nonebot_plugin_poke-0.1.2/nonebot_plugin_poke/utils.py
+-rw-r--r--   0        0        0     1682 2023-08-02 08:32:07.992534 nonebot_plugin_poke-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4117 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_poke-0.1.1/LICENSE` & `nonebot_plugin_poke-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.1.1/README.md` & `nonebot_plugin_poke-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+<!-- markdownlint-disable MD026 MD031 MD033 MD036 MD041 MD046 -->
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
@@ -32,14 +33,15 @@
 方法一：
 
         nb plugin install nonebot_plugin_poke
 
 方法二：
 
         pip install nonebot_plugin_poke
+        poetry add nonebot-plugin-pjsk
 
 再手动添加`nonebot_plugin_poke`到bot文件下`pyproject.toml`文件中
 
 ## env配置项:
 
     # 在完全不写的情况下，效果是戳戳后反戳戳
     # 机器人名称
@@ -70,15 +72,14 @@
 
 ## 指令
 
 群里双击bot头像，会依次按照配置文件，逐步检查回复
 
 ## 数据结构
 
-
 ```txt
 举例：
 └── data
     └── poke
         ├── poke.txt        # 回复文字
         ├── pic             # 回复图片
             ├── 1.png
@@ -95,8 +96,8 @@
 ## 其他
 
 - 如果发不出语音，请手动安装ffmpeg
 - 当语音，与图或文都为True的时候，则随机发送一种，防止刷屏刷到风控
 
 ## 参考
 
-- [智障回复](https://github.com/Special-Week/nonebot_plugin_smart_reply) - 配置写法
+- [智障回复](https://github.com/Special-Week/nonebot_plugin_smart_reply)
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_poke _â¨Nonebot & èªå®ä¹æ³æ³ç¾¤èäºä»¶â¨_ [GitHub
        stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## å®è£ æ¹æ³ä¸ï¼ nb plugin install nonebot_plugin_poke æ¹æ³äºï¼ pip
-install nonebot_plugin_poke
+install nonebot_plugin_poke poetry add nonebot-plugin-pjsk
 åæå¨æ·»å `nonebot_plugin_poke`å°botæä»¶ä¸`pyproject.toml`æä»¶ä¸­ ##
 envéç½®é¡¹: # å¨å®å¨ä¸åçæåµä¸ï¼æææ¯æ³æ³ååæ³æ³ #
 æºå¨äººåç§° bot_nickname: str = 'å®å®' # æ¯å¦åå¤å¾ç
 poke_send_pic: bool = False # æ¯å¦åå¤æ³æ³ poke_send_poke: bool = True #
 æ¯å¦åå¤æå­ poke_send_text: bool = False # æ¯å¦åå¤é³é¢
 poke_send_acc: bool = False
 å¦æä¸ç¥éä»¥ä¸éç½®ï¼é»è®¤å°±å¯ä»¥ï¼åªä¿®æ¹ä¸é¢é¨å #
@@ -20,8 +20,8 @@
 æ°æ®ç»æ ```txt ä¸¾ä¾ï¼ âââ data âââ poke âââ poke.txt
 # åå¤æå­ âââ pic # åå¤å¾ç âââ 1.png âââ 2.jpg
 âââ 3.jpeg âââ ... âââ acc # åå¤é³é¢ âââ 1.acc
 âââ 2.mp3 âââ ... ... ``` ## å¶ä» -
 å¦æåä¸åºè¯­é³ï¼è¯·æå¨å®è£ffmpeg -
 å½è¯­é³ï¼ä¸å¾ææé½ä¸ºTrueçæ¶åï¼åéæºåéä¸ç§ï¼é²æ­¢å·å±å·å°é£æ§
 ## åè - [æºéåå¤](https://github.com/Special-Week/
-nonebot_plugin_smart_reply) - éç½®åæ³
+nonebot_plugin_smart_reply)
```

### Comparing `nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/config.py` & `nonebot_plugin_poke-0.1.2/nonebot_plugin_poke/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/matcher.py` & `nonebot_plugin_poke-0.1.2/nonebot_plugin_poke/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/utils.py` & `nonebot_plugin_poke-0.1.2/nonebot_plugin_poke/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                 "有事恁叫我，别天天一个劲戳戳戳！",
                 "欸很烦欸！你戳🔨呢",
                 "再戳一下试试？",
                 "正在关闭对您的所有服务...关闭成功",
                 "啊呜，太舒服刚刚竟然睡着了。什么事？",
                 "正在定位您的真实地址...定位成功。轰炸机已起飞",
             ]
-            await f.write("/n".join(text_file_list))
+            await f.write("\n".join(text_file_list))
             send_text = random.choice(text_file_list)
     send_text.replace("我", config.bot_nickname)
     return send_text
 
 
 async def pic_or_text(
     send_pic: Optional[Path],
```

### Comparing `nonebot_plugin_poke-0.1.1/pyproject.toml` & `nonebot_plugin_poke-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_poke"
-version = "0.1.1"
+version = "0.1.2"
 description = "自定义群聊戳戳事件 plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_poke"
 repository = "https://github.com/Agnes4m/nonebot_plugin_poke"
 keywords = ["nonebot2", "plugin","event"]
```

### Comparing `nonebot_plugin_poke-0.1.1/PKG-INFO` & `nonebot_plugin_poke-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-poke
-Version: 0.1.1
+Version: 0.1.2
 Summary: 自定义群聊戳戳事件 plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_poke
 License: MIT
 Keywords: nonebot2,plugin,event
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.8,<4.0
@@ -19,14 +19,15 @@
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_poke
 Description-Content-Type: text/markdown
 
+<!-- markdownlint-disable MD026 MD031 MD033 MD036 MD041 MD046 -->
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
@@ -57,14 +58,15 @@
 方法一：
 
         nb plugin install nonebot_plugin_poke
 
 方法二：
 
         pip install nonebot_plugin_poke
+        poetry add nonebot-plugin-pjsk
 
 再手动添加`nonebot_plugin_poke`到bot文件下`pyproject.toml`文件中
 
 ## env配置项:
 
     # 在完全不写的情况下，效果是戳戳后反戳戳
     # 机器人名称
@@ -95,15 +97,14 @@
 
 ## 指令
 
 群里双击bot头像，会依次按照配置文件，逐步检查回复
 
 ## 数据结构
 
-
 ```txt
 举例：
 └── data
     └── poke
         ├── poke.txt        # 回复文字
         ├── pic             # 回复图片
             ├── 1.png
@@ -120,9 +121,9 @@
 ## 其他
 
 - 如果发不出语音，请手动安装ffmpeg
 - 当语音，与图或文都为True的时候，则随机发送一种，防止刷屏刷到风控
 
 ## 参考
 
-- [智障回复](https://github.com/Special-Week/nonebot_plugin_smart_reply) - 配置写法
+- [智障回复](https://github.com/Special-Week/nonebot_plugin_smart_reply)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.1.2 Summary:
 èªå®ä¹ç¾¤èæ³æ³äºä»¶ plugin for NoneBot2 Home-page: https://github.com/
 Agnes4m/nonebot_plugin_poke License: MIT Keywords: nonebot2,plugin,event
 Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,15 @@
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Project-URL: Repository, https://
 github.com/Agnes4m/nonebot_plugin_poke Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_poke _â¨Nonebot & èªå®ä¹æ³æ³ç¾¤èäºä»¶â¨_ [GitHub
        stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## å®è£ æ¹æ³ä¸ï¼ nb plugin install nonebot_plugin_poke æ¹æ³äºï¼ pip
-install nonebot_plugin_poke
+install nonebot_plugin_poke poetry add nonebot-plugin-pjsk
 åæå¨æ·»å `nonebot_plugin_poke`å°botæä»¶ä¸`pyproject.toml`æä»¶ä¸­ ##
 envéç½®é¡¹: # å¨å®å¨ä¸åçæåµä¸ï¼æææ¯æ³æ³ååæ³æ³ #
 æºå¨äººåç§° bot_nickname: str = 'å®å®' # æ¯å¦åå¤å¾ç
 poke_send_pic: bool = False # æ¯å¦åå¤æ³æ³ poke_send_poke: bool = True #
 æ¯å¦åå¤æå­ poke_send_text: bool = False # æ¯å¦åå¤é³é¢
 poke_send_acc: bool = False
 å¦æä¸ç¥éä»¥ä¸éç½®ï¼é»è®¤å°±å¯ä»¥ï¼åªä¿®æ¹ä¸é¢é¨å #
@@ -33,8 +33,8 @@
 æ°æ®ç»æ ```txt ä¸¾ä¾ï¼ âââ data âââ poke âââ poke.txt
 # åå¤æå­ âââ pic # åå¤å¾ç âââ 1.png âââ 2.jpg
 âââ 3.jpeg âââ ... âââ acc # åå¤é³é¢ âââ 1.acc
 âââ 2.mp3 âââ ... ... ``` ## å¶ä» -
 å¦æåä¸åºè¯­é³ï¼è¯·æå¨å®è£ffmpeg -
 å½è¯­é³ï¼ä¸å¾ææé½ä¸ºTrueçæ¶åï¼åéæºåéä¸ç§ï¼é²æ­¢å·å±å·å°é£æ§
 ## åè - [æºéåå¤](https://github.com/Special-Week/
-nonebot_plugin_smart_reply) - éç½®åæ³
+nonebot_plugin_smart_reply)
```

