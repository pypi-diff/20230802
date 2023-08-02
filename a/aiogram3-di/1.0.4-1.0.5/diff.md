# Comparing `tmp/aiogram3_di-1.0.4.tar.gz` & `tmp/aiogram3_di-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_di-1.0.4.tar", last modified: Mon Jul 31 10:17:37 2023, max compression
+gzip compressed data, was "aiogram3_di-1.0.5.tar", last modified: Wed Aug  2 12:13:30 2023, max compression
```

## Comparing `aiogram3_di-1.0.4.tar` & `aiogram3_di-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-31 10:17:37.301295 aiogram3_di-1.0.4/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1075 2023-01-01 13:29:08.000000 aiogram3_di-1.0.4/LICENSE
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2050 2023-07-31 10:17:37.301295 aiogram3_di-1.0.4/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1420 2023-07-30 18:50:20.000000 aiogram3_di-1.0.4/README.md
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-31 10:17:37.301295 aiogram3_di-1.0.4/aiogram3_di/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      142 2023-07-28 19:36:21.000000 aiogram3_di-1.0.4/aiogram3_di/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-07-31 10:16:49.000000 aiogram3_di-1.0.4/aiogram3_di/_version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      276 2023-07-31 08:28:38.000000 aiogram3_di-1.0.4/aiogram3_di/depends.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1046 2023-07-30 15:37:12.000000 aiogram3_di-1.0.4/aiogram3_di/middleware.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5546 2023-07-31 10:11:43.000000 aiogram3_di-1.0.4/aiogram3_di/utils.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-31 10:17:37.301295 aiogram3_di-1.0.4/aiogram3_di.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2050 2023-07-31 10:17:37.000000 aiogram3_di-1.0.4/aiogram3_di.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      318 2023-07-31 10:17:37.000000 aiogram3_di-1.0.4/aiogram3_di.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-07-31 10:17:37.000000 aiogram3_di-1.0.4/aiogram3_di.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       17 2023-07-31 10:17:37.000000 aiogram3_di-1.0.4/aiogram3_di.egg-info/requires.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       12 2023-07-31 10:17:37.000000 aiogram3_di-1.0.4/aiogram3_di.egg-info/top_level.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-07-31 10:17:37.301295 aiogram3_di-1.0.4/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1044 2023-07-30 19:11:38.000000 aiogram3_di-1.0.4/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-02 12:13:30.469361 aiogram3_di-1.0.5/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1075 2023-01-01 13:29:08.000000 aiogram3_di-1.0.5/LICENSE
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     2037 2023-08-02 12:13:30.469361 aiogram3_di-1.0.5/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1407 2023-08-02 12:12:17.000000 aiogram3_di-1.0.5/README.md
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-02 12:13:30.469361 aiogram3_di-1.0.5/aiogram3_di/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      142 2023-07-28 19:36:21.000000 aiogram3_di-1.0.5/aiogram3_di/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-02 12:11:35.000000 aiogram3_di-1.0.5/aiogram3_di/_version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      276 2023-07-31 08:28:38.000000 aiogram3_di-1.0.5/aiogram3_di/depends.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1067 2023-08-02 12:10:09.000000 aiogram3_di-1.0.5/aiogram3_di/middleware.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5546 2023-07-31 10:11:43.000000 aiogram3_di-1.0.5/aiogram3_di/utils.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-02 12:13:30.469361 aiogram3_di-1.0.5/aiogram3_di.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     2037 2023-08-02 12:13:30.000000 aiogram3_di-1.0.5/aiogram3_di.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      318 2023-08-02 12:13:30.000000 aiogram3_di-1.0.5/aiogram3_di.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-08-02 12:13:30.000000 aiogram3_di-1.0.5/aiogram3_di.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       17 2023-08-02 12:13:30.000000 aiogram3_di-1.0.5/aiogram3_di.egg-info/requires.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       12 2023-08-02 12:13:30.000000 aiogram3_di-1.0.5/aiogram3_di.egg-info/top_level.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-08-02 12:13:30.469361 aiogram3_di-1.0.5/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1044 2023-07-30 19:11:38.000000 aiogram3_di-1.0.5/setup.py
```

### Comparing `aiogram3_di-1.0.4/LICENSE` & `aiogram3_di-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.4/PKG-INFO` & `aiogram3_di-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3_di
-Version: 1.0.4
+Version: 1.0.5
 Summary: Dependency Injection implementation for aiogram 3.
 Home-page: https://github.com/Vladyslav49/aiogram3_di
 Author: Vladyslav49
 Author-email: 
 License: MIT
 Keywords: Aiogram,Telegram,Bots,DI,Dependency Injection
 Classifier: Intended Audience :: Developers
@@ -20,22 +20,22 @@
 
 ```python
 import logging
 from os import getenv
 from typing import Annotated
 
 from aiogram import Router, Bot, Dispatcher
-from aiogram.types import Message, User
+from aiogram.types import Message
 from aiogram3_di import DIMiddleware, Depends
 
 router = Router()
 
 
-def get_user_full_name(event_from_user: User) -> str:
-    return event_from_user.full_name
+def get_user_full_name(event: Message) -> str:
+    return event.from_user.full_name
 
 
 @router.message()
 async def _(message: Message, full_name: Annotated[str, Depends(get_user_full_name)]) -> None:
     await message.answer(f'Hi {full_name}')
```

### Comparing `aiogram3_di-1.0.4/README.md` & `aiogram3_di-1.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 ```python
 import logging
 from os import getenv
 from typing import Annotated
 
 from aiogram import Router, Bot, Dispatcher
-from aiogram.types import Message, User
+from aiogram.types import Message
 from aiogram3_di import DIMiddleware, Depends
 
 router = Router()
 
 
-def get_user_full_name(event_from_user: User) -> str:
-    return event_from_user.full_name
+def get_user_full_name(event: Message) -> str:
+    return event.from_user.full_name
 
 
 @router.message()
 async def _(message: Message, full_name: Annotated[str, Depends(get_user_full_name)]) -> None:
     await message.answer(f'Hi {full_name}')
```

### Comparing `aiogram3_di-1.0.4/aiogram3_di/middleware.py` & `aiogram3_di-1.0.5/aiogram3_di/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,9 +18,9 @@
     ) -> Any:
         dispatcher_dependencies = list(getattr(data['dispatcher'], 'dependencies', []))
         router_dependencies = list(getattr(data['event_router'], 'dependencies', []))
         handler_dependencies = list(get_flag(data, 'dependencies', default=[]))
 
         async with AsyncExitStack() as stack:
             data = await process_dependencies(stack, (dispatcher_dependencies + router_dependencies),
-                                              handler_dependencies, data.copy())
+                                              handler_dependencies, (data.copy() | {'event': event}))
             return await handler(event, data)
```

### Comparing `aiogram3_di-1.0.4/aiogram3_di/utils.py` & `aiogram3_di-1.0.5/aiogram3_di/utils.py`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.4/aiogram3_di.egg-info/PKG-INFO` & `aiogram3_di-1.0.5/aiogram3_di.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-di
-Version: 1.0.4
+Version: 1.0.5
 Summary: Dependency Injection implementation for aiogram 3.
 Home-page: https://github.com/Vladyslav49/aiogram3_di
 Author: Vladyslav49
 Author-email: 
 License: MIT
 Keywords: Aiogram,Telegram,Bots,DI,Dependency Injection
 Classifier: Intended Audience :: Developers
@@ -20,22 +20,22 @@
 
 ```python
 import logging
 from os import getenv
 from typing import Annotated
 
 from aiogram import Router, Bot, Dispatcher
-from aiogram.types import Message, User
+from aiogram.types import Message
 from aiogram3_di import DIMiddleware, Depends
 
 router = Router()
 
 
-def get_user_full_name(event_from_user: User) -> str:
-    return event_from_user.full_name
+def get_user_full_name(event: Message) -> str:
+    return event.from_user.full_name
 
 
 @router.message()
 async def _(message: Message, full_name: Annotated[str, Depends(get_user_full_name)]) -> None:
     await message.answer(f'Hi {full_name}')
```

### Comparing `aiogram3_di-1.0.4/setup.py` & `aiogram3_di-1.0.5/setup.py`

 * *Files identical despite different names*

