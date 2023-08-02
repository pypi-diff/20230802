# Comparing `tmp/discord-serverless-2023.1001a0.tar.gz` & `tmp/discord-serverless-2023.1004a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-serverless-2023.1001a0.tar", last modified: Wed Aug  2 11:24:03 2023, max compression
+gzip compressed data, was "discord-serverless-2023.1004a0.tar", last modified: Wed Aug  2 11:47:36 2023, max compression
```

## Comparing `discord-serverless-2023.1001a0.tar` & `discord-serverless-2023.1004a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-02 11:24:03.658786 discord-serverless-2023.1001a0/
--rw-r--r--   0 rosco      (501) staff       (20)     1074 2023-08-01 19:56:27.000000 discord-serverless-2023.1001a0/LICENSE.md
--rw-r--r--   0 rosco      (501) staff       (20)     5732 2023-08-02 11:24:03.658514 discord-serverless-2023.1001a0/PKG-INFO
--rw-r--r--   0 rosco      (501) staff       (20)     4073 2023-08-02 11:22:19.000000 discord-serverless-2023.1001a0/README.md
--rw-r--r--   0 rosco      (501) staff       (20)     1275 2023-08-02 11:22:59.000000 discord-serverless-2023.1001a0/pyproject.toml
--rw-r--r--   0 rosco      (501) staff       (20)       38 2023-08-02 11:24:03.658879 discord-serverless-2023.1001a0/setup.cfg
-drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-02 11:24:03.656463 discord-serverless-2023.1001a0/src/
-drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-02 11:24:03.658083 discord-serverless-2023.1001a0/src/discord_serverless.egg-info/
--rw-r--r--   0 rosco      (501) staff       (20)     5732 2023-08-02 11:24:03.000000 discord-serverless-2023.1001a0/src/discord_serverless.egg-info/PKG-INFO
--rw-r--r--   0 rosco      (501) staff       (20)      290 2023-08-02 11:24:03.000000 discord-serverless-2023.1001a0/src/discord_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 rosco      (501) staff       (20)        1 2023-08-02 11:24:03.000000 discord-serverless-2023.1001a0/src/discord_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 rosco      (501) staff       (20)       69 2023-08-02 11:24:03.000000 discord-serverless-2023.1001a0/src/discord_serverless.egg-info/requires.txt
--rw-r--r--   0 rosco      (501) staff       (20)       19 2023-08-02 11:24:03.000000 discord-serverless-2023.1001a0/src/discord_serverless.egg-info/top_level.txt
--rw-r--r--   0 rosco      (501) staff       (20)     5786 2023-08-01 22:16:12.000000 discord-serverless-2023.1001a0/src/discord_serverless.py
+drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-02 11:47:36.530641 discord-serverless-2023.1004a0/
+-rw-r--r--   0 rosco      (501) staff       (20)     1074 2023-08-01 19:56:27.000000 discord-serverless-2023.1004a0/LICENSE.md
+-rw-r--r--   0 rosco      (501) staff       (20)     5791 2023-08-02 11:47:36.530383 discord-serverless-2023.1004a0/PKG-INFO
+-rw-r--r--   0 rosco      (501) staff       (20)     4132 2023-08-02 11:46:32.000000 discord-serverless-2023.1004a0/README.md
+-rw-r--r--   0 rosco      (501) staff       (20)     1267 2023-08-02 11:47:19.000000 discord-serverless-2023.1004a0/pyproject.toml
+-rw-r--r--   0 rosco      (501) staff       (20)       38 2023-08-02 11:47:36.530729 discord-serverless-2023.1004a0/setup.cfg
+drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-02 11:47:36.520494 discord-serverless-2023.1004a0/src/
+drwxr-xr-x   0 rosco      (501) staff       (20)        0 2023-08-02 11:47:36.530012 discord-serverless-2023.1004a0/src/discord_serverless.egg-info/
+-rw-r--r--   0 rosco      (501) staff       (20)     5791 2023-08-02 11:47:36.000000 discord-serverless-2023.1004a0/src/discord_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 rosco      (501) staff       (20)      290 2023-08-02 11:47:36.000000 discord-serverless-2023.1004a0/src/discord_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 rosco      (501) staff       (20)        1 2023-08-02 11:47:36.000000 discord-serverless-2023.1004a0/src/discord_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 rosco      (501) staff       (20)       69 2023-08-02 11:47:36.000000 discord-serverless-2023.1004a0/src/discord_serverless.egg-info/requires.txt
+-rw-r--r--   0 rosco      (501) staff       (20)       19 2023-08-02 11:47:36.000000 discord-serverless-2023.1004a0/src/discord_serverless.egg-info/top_level.txt
+-rw-r--r--   0 rosco      (501) staff       (20)     5786 2023-08-01 22:16:12.000000 discord-serverless-2023.1004a0/src/discord_serverless.py
```

### Comparing `discord-serverless-2023.1001a0/LICENSE.md` & `discord-serverless-2023.1004a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `discord-serverless-2023.1001a0/PKG-INFO` & `discord-serverless-2023.1004a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-serverless
-Version: 2023.1001a0
+Version: 2023.1004a0
 Summary: Simplified serverless Discord bot interactions
 Author-email: Ross Bamford <roscopeco@gmail.com>
 License: Copyright 2023 Ross Bamford & Contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -18,14 +18,16 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 ## Utility library for serverless Discord apps
 
+![PyPI](https://img.shields.io/pypi/v/discord-serverless)
+
 This is a (currently very simple) library that eases development of serverless Discord
 app and bots.
 
 Currently, it targets AWS Lambda only, and provides a decorator and some utility
 functions that make discord signature verification and ping handling automatic.
 
 I will grow it with things I end up needing in my work, but if you have different
```

### Comparing `discord-serverless-2023.1001a0/README.md` & `discord-serverless-2023.1004a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 ## Utility library for serverless Discord apps
 
+![PyPI](https://img.shields.io/pypi/v/discord-serverless)
+
 This is a (currently very simple) library that eases development of serverless Discord
 app and bots.
 
 Currently, it targets AWS Lambda only, and provides a decorator and some utility
 functions that make discord signature verification and ping handling automatic.
 
 I will grow it with things I end up needing in my work, but if you have different
```

### Comparing `discord-serverless-2023.1001a0/pyproject.toml` & `discord-serverless-2023.1004a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "discord-serverless"
-version = "2023.1001-alpha"
+version = "2023.1004-alpha"
 description = "Simplified serverless Discord bot interactions"
 readme = "README.md"
 authors = [{ name = "Ross Bamford", email = "roscopeco@gmail.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -23,26 +23,26 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pre-commit", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/roscopeco/discord-serverless"
 
 [tool.bumpver]
-current_version = "2023.1002-alpha"
+current_version = "2023.1004-alpha"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
-    'current_version = "{version}"',
+    'version = "{version}"',
 ]
 
 [tool.black]
 py36 = true
 include = '\.pyi?$'
 exclude = '''
     /(
```

### Comparing `discord-serverless-2023.1001a0/src/discord_serverless.egg-info/PKG-INFO` & `discord-serverless-2023.1004a0/src/discord_serverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-serverless
-Version: 2023.1001a0
+Version: 2023.1004a0
 Summary: Simplified serverless Discord bot interactions
 Author-email: Ross Bamford <roscopeco@gmail.com>
 License: Copyright 2023 Ross Bamford & Contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -18,14 +18,16 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 ## Utility library for serverless Discord apps
 
+![PyPI](https://img.shields.io/pypi/v/discord-serverless)
+
 This is a (currently very simple) library that eases development of serverless Discord
 app and bots.
 
 Currently, it targets AWS Lambda only, and provides a decorator and some utility
 functions that make discord signature verification and ping handling automatic.
 
 I will grow it with things I end up needing in my work, but if you have different
```

### Comparing `discord-serverless-2023.1001a0/src/discord_serverless.py` & `discord-serverless-2023.1004a0/src/discord_serverless.py`

 * *Files identical despite different names*

