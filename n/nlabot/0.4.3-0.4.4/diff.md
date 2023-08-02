# Comparing `tmp/nlabot-0.4.3-py3-none-any.whl.zip` & `tmp/nlabot-0.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10789 bytes, number of entries: 8
--rwxrwxrwx  2.0 unx    45146 b- defN 23-Aug-02 10:01 nlaftn/__init__.py
--rwxrwxrwx  2.0 unx       10 b- defN 23-Aug-02 10:01 nlabot-0.4.3.dist-info/DESCRIPTION.rst
--rwxrwxrwx  2.0 unx       47 b- defN 23-Aug-02 10:01 nlabot-0.4.3.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx      619 b- defN 23-Aug-02 10:01 nlabot-0.4.3.dist-info/metadata.json
--rwxrwxrwx  2.0 unx        7 b- defN 23-Aug-02 10:01 nlabot-0.4.3.dist-info/top_level.txt
--rwxrwxrwx  2.0 unx       92 b- defN 23-Aug-02 10:01 nlabot-0.4.3.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      531 b- defN 23-Aug-02 10:01 nlabot-0.4.3.dist-info/METADATA
--rwxrwxrwx  2.0 unx      659 b- defN 23-Aug-02 10:01 nlabot-0.4.3.dist-info/RECORD
-8 files, 47111 bytes uncompressed, 9641 bytes compressed:  79.5%
+Zip file size: 10788 bytes, number of entries: 8
+-rwxrwxrwx  2.0 unx    45146 b- defN 23-Aug-02 10:04 nlaftn/__init__.py
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/DESCRIPTION.rst
+-rwxrwxrwx  2.0 unx       47 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      619 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/metadata.json
+-rwxrwxrwx  2.0 unx        7 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/top_level.txt
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      531 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      659 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/RECORD
+8 files, 47111 bytes uncompressed, 9640 bytes compressed:  79.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: nlaftn/__init__.py
 Comment: 
 
-Filename: nlabot-0.4.3.dist-info/DESCRIPTION.rst
+Filename: nlabot-0.4.4.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: nlabot-0.4.3.dist-info/dependency_links.txt
+Filename: nlabot-0.4.4.dist-info/dependency_links.txt
 Comment: 
 
-Filename: nlabot-0.4.3.dist-info/metadata.json
+Filename: nlabot-0.4.4.dist-info/metadata.json
 Comment: 
 
-Filename: nlabot-0.4.3.dist-info/top_level.txt
+Filename: nlabot-0.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: nlabot-0.4.3.dist-info/WHEEL
+Filename: nlabot-0.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: nlabot-0.4.3.dist-info/METADATA
+Filename: nlabot-0.4.4.dist-info/METADATA
 Comment: 
 
-Filename: nlabot-0.4.3.dist-info/RECORD
+Filename: nlabot-0.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nlaftn/__init__.py

```diff
@@ -153,15 +153,15 @@
             "display_name": name
         }
     )
 
 
 class PartyBot(commands.Bot):
     def __init__(self, device_id: str, account_id: str, secret: str, loop=asyncio.get_event_loop(), **kwargs) -> None:
-        self.status = '👽 {party_size}/16 USE CODE HUB 👽'
+        self.status = '👽 {party_size}/16 USE CODE 667 👽'
         self.kairos = 'cid_028_ff2b06cf446376144ba408d3482f5c982bf2584cf0f508ee3e4ba4a0fd461a38'
 
         super().__init__(
             command_prefix=prefix,
             case_insensitive=True,
             auth=fortnitepy.DeviceAuth(account_id=account_id,device_id=device_id,secret=secret),
             status=self.status,
@@ -175,19 +175,19 @@
         self.default_backpack = "BID_138_Celestial"
         self.default_pickaxe = "Pickaxe_Lockjaw"
         self.banner = "otherbanner51"
         self.banner_colour = "defaultcolor22"
         self.default_level = 68
         self.default_bp_tier = 68
         self.invitecc = ''
-        self.invite_message = "JOIN ME \n USE CODE HUB"
+        self.invite_message = "JOIN ME \n USE CODE 667"
 
         self.sanic_app = sanic_app
         self.server = server
-        self.welcome_message =  " Use Code HUB in the Item Shop (#EpicPartner)\nCreate own your bot : https://schbots.com \n free battle pass code here : 8455-3482-1956 \n"
+        self.welcome_message =  " Use Code 667 in the Item Shop (#EpicPartner)\nCreate own your bot : https://schbots.com \n free battle pass code here : 8455-3482-1956 \n"
 
     async def set_and_update_party_prop(self, schema_key: str, new_value: Any) -> None:
         prop = {schema_key: self.party.me.meta.set_prop(schema_key, new_value)}
 
         await self.party.patch(updated=prop)
 
     async def add_list(self) -> None:
```

## Comparing `nlabot-0.4.3.dist-info/metadata.json` & `nlabot-0.4.4.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.4.4'"}*

```diff
@@ -34,9 +34,9 @@
                 "crayons",
                 "fortnitepy (==3.6.7)",
                 "sanic (==21.6.2)"
             ]
         }
     ],
     "summary": "Lobby bot.",
-    "version": "0.4.3"
+    "version": "0.4.4"
 }
```

## Comparing `nlabot-0.4.3.dist-info/METADATA` & `nlabot-0.4.4.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: nlabot
-Version: 0.4.3
+Version: 0.4.4
 Summary: Lobby bot.
 Home-page: https://www.youtube.com/
 Author: Aeroz
 Author-email: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `nlabot-0.4.3.dist-info/RECORD` & `nlabot-0.4.4.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-nlabot-0.4.3.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
-nlabot-0.4.3.dist-info/METADATA,sha256=DrOwpa15Jf3t0H190ItAu3n5yG6tBMONmsQNKgcteqw,531
-nlabot-0.4.3.dist-info/RECORD,,
-nlabot-0.4.3.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-nlabot-0.4.3.dist-info/dependency_links.txt,sha256=w-iWPDMAaFhNNlD27qG0wZlgCL7bmLrdykt1CAjMpg4,47
-nlabot-0.4.3.dist-info/metadata.json,sha256=IHYsHbHzK7hakizrRBYLHMkvarqC0ONUHYHhgh3_u4M,619
-nlabot-0.4.3.dist-info/top_level.txt,sha256=Hf6V-zsLXka13-6RurPoKaSDrHpVgxjB9QZCqY0kBo0,7
-nlaftn/__init__.py,sha256=odkJ4uL-hG1BzbcWdXQYEjl9spzNZ1KPVVvbCUfzTCw,45146
+nlabot-0.4.4.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
+nlabot-0.4.4.dist-info/METADATA,sha256=r2Ki1eYrM3MZ7n9rDYVsXlKzGXHJl84cSDwSlFQCPMg,531
+nlabot-0.4.4.dist-info/RECORD,,
+nlabot-0.4.4.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+nlabot-0.4.4.dist-info/dependency_links.txt,sha256=w-iWPDMAaFhNNlD27qG0wZlgCL7bmLrdykt1CAjMpg4,47
+nlabot-0.4.4.dist-info/metadata.json,sha256=qi73f4XnylEDUV2Z7NQLkLKk9Xkku157Ii7fxCKMsE0,619
+nlabot-0.4.4.dist-info/top_level.txt,sha256=Hf6V-zsLXka13-6RurPoKaSDrHpVgxjB9QZCqY0kBo0,7
+nlaftn/__init__.py,sha256=mzHLLPJD1D0w7v3A0XKPKEuVstCLBeYAXrX6w-rXMtg,45146
```

