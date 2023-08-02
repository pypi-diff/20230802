# Comparing `tmp/schbot-0.6.2-py3-none-any.whl.zip` & `tmp/schbot-0.6.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10746 bytes, number of entries: 8
--rwxrwxrwx  2.0 unx    45096 b- defN 23-Apr-14 19:51 schbot/__init__.py
--rwxrwxrwx  2.0 unx       10 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/DESCRIPTION.rst
--rwxrwxrwx  2.0 unx       47 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx      619 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/metadata.json
--rwxrwxrwx  2.0 unx        7 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/top_level.txt
--rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      531 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/METADATA
--rwxrwxrwx  2.0 unx      659 b- defN 23-Apr-14 20:24 schbot-0.6.2.dist-info/RECORD
-8 files, 47061 bytes uncompressed, 9598 bytes compressed:  79.6%
+Zip file size: 10752 bytes, number of entries: 8
+-rwxrwxrwx  2.0 unx    45097 b- defN 23-Aug-02 10:03 schbot/__init__.py
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Aug-02 10:03 schbot-0.6.3.dist-info/DESCRIPTION.rst
+-rwxrwxrwx  2.0 unx       47 b- defN 23-Aug-02 10:03 schbot-0.6.3.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      619 b- defN 23-Aug-02 10:03 schbot-0.6.3.dist-info/metadata.json
+-rwxrwxrwx  2.0 unx        7 b- defN 23-Aug-02 10:03 schbot-0.6.3.dist-info/top_level.txt
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Aug-02 10:03 schbot-0.6.3.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      531 b- defN 23-Aug-02 10:03 schbot-0.6.3.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      659 b- defN 23-Aug-02 10:03 schbot-0.6.3.dist-info/RECORD
+8 files, 47062 bytes uncompressed, 9604 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: schbot/__init__.py
 Comment: 
 
-Filename: schbot-0.6.2.dist-info/DESCRIPTION.rst
+Filename: schbot-0.6.3.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: schbot-0.6.2.dist-info/dependency_links.txt
+Filename: schbot-0.6.3.dist-info/dependency_links.txt
 Comment: 
 
-Filename: schbot-0.6.2.dist-info/metadata.json
+Filename: schbot-0.6.3.dist-info/metadata.json
 Comment: 
 
-Filename: schbot-0.6.2.dist-info/top_level.txt
+Filename: schbot-0.6.3.dist-info/top_level.txt
 Comment: 
 
-Filename: schbot-0.6.2.dist-info/WHEEL
+Filename: schbot-0.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: schbot-0.6.2.dist-info/METADATA
+Filename: schbot-0.6.3.dist-info/METADATA
 Comment: 
 
-Filename: schbot-0.6.2.dist-info/RECORD
+Filename: schbot-0.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## schbot/__init__.py

```diff
@@ -153,15 +153,15 @@
             "display_name": name
         }
     )
 
 
 class PartyBot(commands.Bot):
     def __init__(self, device_id: str, account_id: str, secret: str, loop=asyncio.get_event_loop(), **kwargs) -> None:
-        self.status = ' 💥 {party_size}/16 Use Code SCH 💥'
+        self.status = ' 💥 {party_size}/16 Use Code 667 💥'
         self.kairos = 'cid_028_ff2b06cf446376144ba408d3482f5c982bf2584cf0f508ee3e4ba4a0fd461a38'
 
         super().__init__(
             command_prefix=prefix,
             case_insensitive=True,
             auth=fortnitepy.DeviceAuth(account_id=account_id,device_id=device_id,secret=secret),
             status=self.status,
@@ -178,35 +178,34 @@
         self.banner_colour = "defaultcolor22"
         self.default_level = 69
         self.default_bp_tier = 69
         self.invitecc = ''
 
         self.sanic_app = sanic_app
         self.server = server
-        self.welcome_message =  " Use Code SCH in the Item Shop (#EpicPartner)\n Create own your bot : https://schbots.com \n free battle pass code here : 8455-3482-1956 \n"
+        self.welcome_message =  " Use Code 667 in the Item Shop (#EpicPartner)\n Create own your bot : https://schbots.com \n free battle pass code here : 8455-3482-1956 \n"
 
     async def set_and_update_party_prop(self, schema_key: str, new_value: Any) -> None:
         prop = {schema_key: self.party.me.meta.set_prop(schema_key, new_value)}
 
         await self.party.patch(updated=prop)
 
     async def add_list(self) -> None:
         try:
             await self.add_friend('4b713a5896744d8a9d3b9ff32266682a')
         except: pass
 
     async def status_change(self) -> None:
         await asyncio.sleep(3600)
-        await self.set_presence("💥 {party_size}/16 Use Code SCH 💥")
+        await self.set_presence("💥 {party_size}/16 Use Code 667 💥")
         await asyncio.sleep(10)
         await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
         await asyncio.sleep(3600)
-        await self.set_presence("💥 {party_size}/16 Use Code SCH 💥")
-        await asyncio.sleep(10)
-        await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+        await self.set_presence("💥 {party_size}/16 Use Code 667 💥")
+        await asyncio.sleep(10667        await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
         self.loop.create_task(self.status_changer())
 
     async def event_device_auth_generate(self, details: dict, email: str) -> None:
         print(self.user.display_name)
 
     async def event_ready(self) -> None:
         global name
@@ -247,15 +246,15 @@
         if not self.is_ready():
             await self.wait_until_ready()
         if self.invitecc == 'True':
             if old_presence is None:
                 friend = presence.friend
                 if friend.display_name != 'AerozOff': #blacklisted pour pas recevoir
                     try:
-                        await friend.send('Join me \n Use Code : SCH')
+                        await friend.send('Join me \n Use Code : 667')
                     except:
                         pass
                     else:
                         if not self.party.member_count >= 16:
                             await friend.invite()
 
     async def update_settings(self) -> None:
```

## Comparing `schbot-0.6.2.dist-info/metadata.json` & `schbot-0.6.3.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.6.3'"}*

```diff
@@ -34,9 +34,9 @@
                 "crayons",
                 "fortnitepy (==3.6.7)",
                 "sanic (==21.6.2)"
             ]
         }
     ],
     "summary": "Lobby bot.",
-    "version": "0.6.2"
+    "version": "0.6.3"
 }
```

## Comparing `schbot-0.6.2.dist-info/METADATA` & `schbot-0.6.3.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: schbot
-Version: 0.6.2
+Version: 0.6.3
 Summary: Lobby bot.
 Home-page: https://www.youtube.com/
 Author: Aeroz
 Author-email: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

