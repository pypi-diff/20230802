# Comparing `tmp/discord-serverless-2023.1004a0.tar.gz` & `tmp/discord-serverless-2023.1005a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-serverless-2023.1004a0.tar", last modified: Wed Aug  2 11:47:36 2023, max compression
+gzip compressed data, was "discord-serverless-2023.1005a0.tar", last modified: Wed Aug  2 18:18:28 2023, max compression
```

## Comparing `discord-serverless-2023.1004a0.tar` & `discord-serverless-2023.1005a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-02 11:47:36.530641 discord-serverless-2023.1004a0/
--rw-r--r--   0 rosco      (501) staff       (20)     1074 2023-08-01 19:56:27.000000 discord-serverless-2023.1004a0/LICENSE.md
--rw-r--r--   0 rosco      (501) staff       (20)     5791 2023-08-02 11:47:36.530383 discord-serverless-2023.1004a0/PKG-INFO
--rw-r--r--   0 rosco      (501) staff       (20)     4132 2023-08-02 11:46:32.000000 discord-serverless-2023.1004a0/README.md
--rw-r--r--   0 rosco      (501) staff       (20)     1267 2023-08-02 11:47:19.000000 discord-serverless-2023.1004a0/pyproject.toml
--rw-r--r--   0 rosco      (501) staff       (20)       38 2023-08-02 11:47:36.530729 discord-serverless-2023.1004a0/setup.cfg
-drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-02 11:47:36.520494 discord-serverless-2023.1004a0/src/
-drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-02 11:47:36.530012 discord-serverless-2023.1004a0/src/discord_serverless.egg-info/
--rw-r--r--   0 rosco      (501) staff       (20)     5791 2023-08-02 11:47:36.000000 discord-serverless-2023.1004a0/src/discord_serverless.egg-info/PKG-INFO
--rw-r--r--   0 rosco      (501) staff       (20)      290 2023-08-02 11:47:36.000000 discord-serverless-2023.1004a0/src/discord_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 rosco      (501) staff       (20)        1 2023-08-02 11:47:36.000000 discord-serverless-2023.1004a0/src/discord_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 rosco      (501) staff       (20)       69 2023-08-02 11:47:36.000000 discord-serverless-2023.1004a0/src/discord_serverless.egg-info/requires.txt
--rw-r--r--   0 rosco      (501) staff       (20)       19 2023-08-02 11:47:36.000000 discord-serverless-2023.1004a0/src/discord_serverless.egg-info/top_level.txt
--rw-r--r--   0 rosco      (501) staff       (20)     5786 2023-08-01 22:16:12.000000 discord-serverless-2023.1004a0/src/discord_serverless.py
+drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-02 18:18:28.099623 discord-serverless-2023.1005a0/
+-rw-r--r--   0 rosco      (501) staff       (20)     1074 2023-08-01 19:56:27.000000 discord-serverless-2023.1005a0/LICENSE.md
+-rw-r--r--   0 rosco      (501) staff       (20)     5791 2023-08-02 18:18:28.099358 discord-serverless-2023.1005a0/PKG-INFO
+-rw-r--r--   0 rosco      (501) staff       (20)     4132 2023-08-02 11:46:32.000000 discord-serverless-2023.1005a0/README.md
+-rw-r--r--   0 rosco      (501) staff       (20)     1290 2023-08-02 18:18:19.000000 discord-serverless-2023.1005a0/pyproject.toml
+-rw-r--r--   0 rosco      (501) staff       (20)       38 2023-08-02 18:18:28.099743 discord-serverless-2023.1005a0/setup.cfg
+drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-02 18:18:28.097279 discord-serverless-2023.1005a0/src/
+drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-02 18:18:28.098987 discord-serverless-2023.1005a0/src/discord_serverless.egg-info/
+-rw-r--r--   0 rosco      (501) staff       (20)     5791 2023-08-02 18:18:28.000000 discord-serverless-2023.1005a0/src/discord_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 rosco      (501) staff       (20)      290 2023-08-02 18:18:28.000000 discord-serverless-2023.1005a0/src/discord_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 rosco      (501) staff       (20)        1 2023-08-02 18:18:28.000000 discord-serverless-2023.1005a0/src/discord_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 rosco      (501) staff       (20)       86 2023-08-02 18:18:28.000000 discord-serverless-2023.1005a0/src/discord_serverless.egg-info/requires.txt
+-rw-r--r--   0 rosco      (501) staff       (20)       19 2023-08-02 18:18:28.000000 discord-serverless-2023.1005a0/src/discord_serverless.egg-info/top_level.txt
+-rw-r--r--   0 rosco      (501) staff       (20)     6296 2023-08-02 18:16:56.000000 discord-serverless-2023.1005a0/src/discord_serverless.py
```

### Comparing `discord-serverless-2023.1004a0/LICENSE.md` & `discord-serverless-2023.1005a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `discord-serverless-2023.1004a0/PKG-INFO` & `discord-serverless-2023.1005a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-serverless
-Version: 2023.1004a0
+Version: 2023.1005a0
 Summary: Simplified serverless Discord bot interactions
 Author-email: Ross Bamford <roscopeco@gmail.com>
 License: Copyright 2023 Ross Bamford & Contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `discord-serverless-2023.1004a0/README.md` & `discord-serverless-2023.1005a0/README.md`

 * *Files identical despite different names*

### Comparing `discord-serverless-2023.1004a0/pyproject.toml` & `discord-serverless-2023.1005a0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "discord-serverless"
-version = "2023.1004-alpha"
+version = "2023.1005-alpha"
 description = "Simplified serverless Discord bot interactions"
 readme = "README.md"
 authors = [{ name = "Ross Bamford", email = "roscopeco@gmail.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["feed", "reader", "tutorial"]
 dependencies = [
     "pynacl >= 1.5.0",
+    "requests>=2.31.0"
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pre-commit", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/roscopeco/discord-serverless"
 
 [tool.bumpver]
-current_version = "2023.1004-alpha"
+current_version = "2023.1005-alpha"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `discord-serverless-2023.1004a0/src/discord_serverless.egg-info/PKG-INFO` & `discord-serverless-2023.1005a0/src/discord_serverless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-serverless
-Version: 2023.1004a0
+Version: 2023.1005a0
 Summary: Simplified serverless Discord bot interactions
 Author-email: Ross Bamford <roscopeco@gmail.com>
 License: Copyright 2023 Ross Bamford & Contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `discord-serverless-2023.1004a0/src/discord_serverless.py` & `discord-serverless-2023.1005a0/src/discord_serverless.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 #
 # Copyright (c)2023 Ross Bamford (and contributors)
 # MIT license
 #
 import json
 from typing import Callable, Any
 
+import requests as requests
+from requests import Response
 from nacl.signing import VerifyKey
 from nacl.exceptions import BadSignatureError
 
 
 def discord_command_lambda(discord_key: str):
     """Decorator for an AWS lambda function handler that processes Discord webhook interactions
 
@@ -129,17 +131,32 @@
 
 
 def discord_unknown_command_response(command: str) -> dict[str, Any]:
     """Generate a generic "unknown command" response for Discord.
 
     :param command: Command to parrot in the response error message
     """
+
     return {"statusCode": 400, "body": json.dumps(f"Unknown command: {command}")}
 
 
+def discord_webhook_reply(content: str, app_id: str, token: str) -> Response:
+    """Post a follow-up reply to a discord webhook interaction
+
+    :param content The message content.
+    :param app_id The app_id (from Discord).
+    :param token The interaction token (provided when your webhook was called).
+    """
+
+    return requests.post(
+        f"https://discord.com/api/v10/webhooks/{app_id}/{token}",
+        json={"content": content},
+    )
+
+
 def discord_verify_signature(
     public_key: str, signature: str, timestamp: str, raw_payload: str
 ) -> bool:
     message = timestamp + raw_payload
     verify_key = VerifyKey(bytes.fromhex(public_key))
 
     try:
```

