# Comparing `tmp/CheeseAPI-0.0.3.tar.gz` & `tmp/CheeseAPI-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheeseAPI-0.0.3.tar", last modified: Wed Aug  2 02:05:39 2023, max compression
+gzip compressed data, was "CheeseAPI-0.0.4.tar", last modified: Wed Aug  2 04:03:40 2023, max compression
```

## Comparing `CheeseAPI-0.0.3.tar` & `CheeseAPI-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 02:05:39.424415 CheeseAPI-0.0.3/
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 02:05:39.423156 CheeseAPI-0.0.3/CheeseAPI/
--rw-r--r--   0 cheese     (501) staff       (20)      255 2023-08-01 09:51:10.000000 CheeseAPI-0.0.3/CheeseAPI/__init__.py
--rw-r--r--   0 cheese     (501) staff       (20)    16039 2023-08-02 01:49:39.000000 CheeseAPI-0.0.3/CheeseAPI/app.py
--rw-r--r--   0 cheese     (501) staff       (20)     1636 2023-08-01 09:45:24.000000 CheeseAPI-0.0.3/CheeseAPI/cSignal.py
--rw-r--r--   0 cheese     (501) staff       (20)     5440 2023-08-02 02:04:56.000000 CheeseAPI-0.0.3/CheeseAPI/command.py
--rw-r--r--   0 cheese     (501) staff       (20)      492 2023-07-31 08:17:28.000000 CheeseAPI-0.0.3/CheeseAPI/exception.py
--rw-r--r--   0 cheese     (501) staff       (20)     2434 2023-08-01 05:36:54.000000 CheeseAPI-0.0.3/CheeseAPI/file.py
--rw-r--r--   0 cheese     (501) staff       (20)     2287 2023-08-01 09:12:11.000000 CheeseAPI-0.0.3/CheeseAPI/module.py
--rw-r--r--   0 cheese     (501) staff       (20)     3675 2023-08-01 08:04:57.000000 CheeseAPI-0.0.3/CheeseAPI/request.py
--rw-r--r--   0 cheese     (501) staff       (20)    12440 2023-08-01 08:05:03.000000 CheeseAPI-0.0.3/CheeseAPI/response.py
--rw-r--r--   0 cheese     (501) staff       (20)     4317 2023-08-01 06:17:09.000000 CheeseAPI-0.0.3/CheeseAPI/route.py
--rw-r--r--   0 cheese     (501) staff       (20)     3526 2023-08-01 08:05:19.000000 CheeseAPI-0.0.3/CheeseAPI/server.py
--rw-r--r--   0 cheese     (501) staff       (20)      676 2023-07-31 08:11:41.000000 CheeseAPI-0.0.3/CheeseAPI/system.py
--rw-r--r--   0 cheese     (501) staff       (20)     1345 2023-08-01 07:01:25.000000 CheeseAPI-0.0.3/CheeseAPI/websocket.py
--rw-r--r--   0 cheese     (501) staff       (20)      295 2023-07-31 08:11:30.000000 CheeseAPI-0.0.3/CheeseAPI/workspace.py
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 02:05:39.424079 CheeseAPI-0.0.3/CheeseAPI.egg-info/
--rw-r--r--   0 cheese     (501) staff       (20)     7909 2023-08-02 02:05:39.000000 CheeseAPI-0.0.3/CheeseAPI.egg-info/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)      516 2023-08-02 02:05:39.000000 CheeseAPI-0.0.3/CheeseAPI.egg-info/SOURCES.txt
--rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-02 02:05:39.000000 CheeseAPI-0.0.3/CheeseAPI.egg-info/dependency_links.txt
--rw-r--r--   0 cheese     (501) staff       (20)       56 2023-08-02 02:05:39.000000 CheeseAPI-0.0.3/CheeseAPI.egg-info/entry_points.txt
--rw-r--r--   0 cheese     (501) staff       (20)       57 2023-08-02 02:05:39.000000 CheeseAPI-0.0.3/CheeseAPI.egg-info/requires.txt
--rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-02 02:05:39.000000 CheeseAPI-0.0.3/CheeseAPI.egg-info/top_level.txt
--rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 13:50:19.000000 CheeseAPI-0.0.3/LICENSE
--rw-r--r--   0 cheese     (501) staff       (20)     7909 2023-08-02 02:05:39.424286 CheeseAPI-0.0.3/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)     7458 2023-08-02 01:58:40.000000 CheeseAPI-0.0.3/README.md
--rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-02 02:05:39.424460 CheeseAPI-0.0.3/setup.cfg
--rw-r--r--   0 cheese     (501) staff       (20)      984 2023-08-02 01:57:12.000000 CheeseAPI-0.0.3/setup.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 04:03:40.887442 CheeseAPI-0.0.4/
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 04:03:40.886371 CheeseAPI-0.0.4/CheeseAPI/
+-rw-r--r--   0 cheese     (501) staff       (20)      255 2023-08-01 09:51:10.000000 CheeseAPI-0.0.4/CheeseAPI/__init__.py
+-rw-r--r--   0 cheese     (501) staff       (20)    16971 2023-08-02 04:02:53.000000 CheeseAPI-0.0.4/CheeseAPI/app.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1636 2023-08-01 09:45:24.000000 CheeseAPI-0.0.4/CheeseAPI/cSignal.py
+-rw-r--r--   0 cheese     (501) staff       (20)     6984 2023-08-02 04:02:27.000000 CheeseAPI-0.0.4/CheeseAPI/command.py
+-rw-r--r--   0 cheese     (501) staff       (20)      492 2023-07-31 08:17:28.000000 CheeseAPI-0.0.4/CheeseAPI/exception.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2434 2023-08-01 05:36:54.000000 CheeseAPI-0.0.4/CheeseAPI/file.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2287 2023-08-01 09:12:11.000000 CheeseAPI-0.0.4/CheeseAPI/module.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3675 2023-08-01 08:04:57.000000 CheeseAPI-0.0.4/CheeseAPI/request.py
+-rw-r--r--   0 cheese     (501) staff       (20)    12440 2023-08-01 08:05:03.000000 CheeseAPI-0.0.4/CheeseAPI/response.py
+-rw-r--r--   0 cheese     (501) staff       (20)     4317 2023-08-01 06:17:09.000000 CheeseAPI-0.0.4/CheeseAPI/route.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3526 2023-08-01 08:05:19.000000 CheeseAPI-0.0.4/CheeseAPI/server.py
+-rw-r--r--   0 cheese     (501) staff       (20)      676 2023-07-31 08:11:41.000000 CheeseAPI-0.0.4/CheeseAPI/system.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1345 2023-08-01 07:01:25.000000 CheeseAPI-0.0.4/CheeseAPI/websocket.py
+-rw-r--r--   0 cheese     (501) staff       (20)      295 2023-07-31 08:11:30.000000 CheeseAPI-0.0.4/CheeseAPI/workspace.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 04:03:40.887130 CheeseAPI-0.0.4/CheeseAPI.egg-info/
+-rw-r--r--   0 cheese     (501) staff       (20)     7909 2023-08-02 04:03:40.000000 CheeseAPI-0.0.4/CheeseAPI.egg-info/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)      516 2023-08-02 04:03:40.000000 CheeseAPI-0.0.4/CheeseAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-02 04:03:40.000000 CheeseAPI-0.0.4/CheeseAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       56 2023-08-02 04:03:40.000000 CheeseAPI-0.0.4/CheeseAPI.egg-info/entry_points.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       57 2023-08-02 04:03:40.000000 CheeseAPI-0.0.4/CheeseAPI.egg-info/requires.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-02 04:03:40.000000 CheeseAPI-0.0.4/CheeseAPI.egg-info/top_level.txt
+-rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 13:50:19.000000 CheeseAPI-0.0.4/LICENSE
+-rw-r--r--   0 cheese     (501) staff       (20)     7909 2023-08-02 04:03:40.887317 CheeseAPI-0.0.4/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)     7458 2023-08-02 01:58:40.000000 CheeseAPI-0.0.4/README.md
+-rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-02 04:03:40.887487 CheeseAPI-0.0.4/setup.cfg
+-rw-r--r--   0 cheese     (501) staff       (20)      984 2023-08-02 04:03:24.000000 CheeseAPI-0.0.4/setup.py
```

### Comparing `CheeseAPI-0.0.3/CheeseAPI/app.py` & `CheeseAPI-0.0.4/CheeseAPI/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, time, inspect, traceback, multiprocessing
+import os, time, inspect, traceback, multiprocessing, json, shutil
 from typing import Callable, AsyncIterator, Dict, List, Any, Set
 from multiprocessing.process import BaseProcess
 
 import CheeseLog, asyncio
 from CheeseLog import logger, Logger
 
 from . import exception
@@ -44,14 +44,30 @@
         self.http_afterResponseHandles: List[Callable] = []
         # websocket
         self.websocket_beforeConnectionHandles: List[Callable] = []
         self.websocket_afterDisconnectHandles: List[Callable] = []
         self.websocket_errorHandles: List[Callable] = []
         self.websocket_notFoundHandles: List[Callable] = []
 
+        if os.path.exists(self.workspace.BASE_PATH + '/.cache/config.json'):
+            with open(self.workspace.BASE_PATH + '/.cache/config.json', 'r') as f:
+                data = json.load(f)
+            self.workspace.LOG_PATH = data['workspace']['LOG_PATH']
+            self.server.HOST = data['server']['HOST']
+            self.server.PORT = data['server']['PORT']
+            self.server.IS_RELOAD = data['server']['IS_RELOAD']
+            self.server.WORKERS = data['server']['WORKERS']
+            self.server.LOG_FILENAME = data['server']['LOG_FILENAME']
+            with open(self.workspace.BASE_PATH + '/.cache/workers', 'a+') as f:
+                f.write('1')
+                f.seek(0)
+                workers = len(f.readline())
+            if workers == self.server.WORKERS and os.path.exists(self.workspace.BASE_PATH + '/.cache'):
+                shutil.rmtree(self.workspace.BASE_PATH + '/.cache')
+
     async def __call__(self, scope, receive, send):
         ''' Server started '''
         if scope['type'] == 'lifespan':
             message = await receive()
             if message['type'] == 'lifespan.startup':
                 _modules = set()
                 if self.process.name == 'MainProcess' and len(self.modules):
```

### Comparing `CheeseAPI-0.0.3/CheeseAPI/cSignal.py` & `CheeseAPI-0.0.4/CheeseAPI/cSignal.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.3/CheeseAPI/command.py` & `CheeseAPI-0.0.4/CheeseAPI/command.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,65 @@
-import argparse, time, os, traceback
+import argparse, time, os, traceback, json, shutil
 
 import CheeseLog, uvicorn, CheeseType, CheeseType.network, uvicorn.importer
 
-from .app import app
-from .cSignal import signal
-
 def command():
+    from .app import app
+    from .cSignal import signal
+
     parser = argparse.ArgumentParser()
-    parser.add_argument('--app', nargs = '?', default = 'app:app', help = '【默认值：app:app】')
-    parser.add_argument('--host', nargs = '?', default = '127.0.0.1', help = '【默认值：127.0.0.1】')
-    parser.add_argument('--port', nargs = '?', default = 5214, help = '【默认值：5214】')
-    parser.add_argument('--reload', nargs = '?', default = False, help = '【默认值：False】')
-    parser.add_argument('--workers', nargs = '?', default = 1, help = 'workers为0时会自动设置为cpu核数*2【默认值：1】')
+    parser.add_argument('--app', nargs = '?', default = 'app:app', help = '服务器本服务【默认值：app:app】')
+    parser.add_argument('--host', nargs = '?', default = '127.0.0.1', help = '服务器地址【默认值：127.0.0.1】')
+    parser.add_argument('--port', nargs = '?', default = 5214, help = '端口号【默认值：5214】')
+    parser.add_argument('--reload', nargs = '?', default = False, help = '热更新。与workers冲突【默认值：False】')
+    parser.add_argument('--workers', nargs = '?', default = 1, help = 'workers为0时会自动设置为cpu核数*2。与reload冲突【默认值：1】')
+    parser.add_argument('--log_path', nargs = '?', default = '/logs/', help = '日志文件夹的相对路径【默认值：/logs/】')
+    parser.add_argument('--log_filename', nargs = '?', default = False, help = '日志文件名。当值为True时，自动设置为%%Y_%%m_%%d-%%H_%%M_%%S.log；当值为False，关闭日志文件记录；自定义文件名也是允许的【默认值：True】')
     args = parser.parse_args()
 
     startTimer: float = time.time()
 
+    _app = args.app
+    host = CheeseType.network.IPv4(args.host)
+    port = CheeseType.network.Port(args.port)
+    reload = CheeseType.Bool(args.reload)
+    workers = CheeseType.NonNegativeInt(args.workers)
+    log_path = args.log_path
+    try:
+        log_filename = CheeseType.Bool(args.log_filename)
+    except:
+        ...
+
+    app.workspace.LOG_PATH = log_path
+    app.server.LOG_FILENAME = log_filename
+    app.server.HOST = host
+    app.server.PORT = port
+    app.server.IS_RELOAD = reload
+    app.server.WORKERS = workers
+
+    if os.path.exists(app.workspace.BASE_PATH + '/.cache'):
+        shutil.rmtree(app.workspace.BASE_PATH + '/.cache')
+    if workers != 1:
+        os.makedirs(app.workspace.BASE_PATH + '/.cache', exist_ok = True)
+        with open(app.workspace.BASE_PATH + '/.cache/config.json', "w") as f:
+            json.dump({
+                'workers': 0,
+                'app': _app,
+                'workspace': {
+                    'LOG_PATH': log_path
+                },
+                'server': {
+                    'HOST': host,
+                    'PORT': port,
+                    'IS_RELOAD': reload,
+                    'WORKERS': workers,
+                    'LOG_FILENAME': log_filename
+                }
+            }, f)
+
     CheeseLog.starting(f'Started CheeseAPI master process {os.getpid()}', f'Started CheeseAPI master process \033[34m{os.getpid()}\033[0m')
     CheeseLog.starting('The application starts loading...')
 
     CheeseLog.starting('''System information:
 system: ''' + {
 'WINDOWS': 'Windows',
 'LINUX': 'Linux',
@@ -62,27 +102,23 @@
     CheeseLog.starting(f'The server running on http://{app.server.HOST}:{app.server.PORT}', f'The server running on \033[4;36mhttp://{app.server.HOST}:{app.server.PORT}\033[0m')
 
     if signal.receiver('server_startingHandle'):
         signal.send('server_startingHandle')
     for server_startingHandle in app.server_startingHandles:
         server_startingHandle()
 
-    app.server.HOST = CheeseType.network.IPv4(args.host)
-    app.server.PORT = CheeseType.network.Port(args.port)
-    app.server.IS_RELOAD = CheeseType.Bool(args.reload)
-    app.server.WORKERS = CheeseType.NonNegativeInt(args.workers)
     try:
         uvicorn.run(
-            args.app,
+            _app,
             host = app.server.HOST,
             port = app.server.PORT,
             reload = app.server.IS_RELOAD,
             workers = app.server.WORKERS,
             log_level = 'critical',
-            app_dir = os.getcwd()
+            app_dir = app.workspace.BASE_PATH
         )
     except:
         CheeseLog.error(f'server startup failed\n{traceback.format_exc()}'[:-1])
 
     if signal.receiver('server_endingHandle'):
         signal.send('server_endingHandle')
     for server_endingHandle in app.server_endingHandles:
```

### Comparing `CheeseAPI-0.0.3/CheeseAPI/file.py` & `CheeseAPI-0.0.4/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.3/CheeseAPI/module.py` & `CheeseAPI-0.0.4/CheeseAPI/module.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.3/CheeseAPI/request.py` & `CheeseAPI-0.0.4/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.3/CheeseAPI/response.py` & `CheeseAPI-0.0.4/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.3/CheeseAPI/route.py` & `CheeseAPI-0.0.4/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.3/CheeseAPI/server.py` & `CheeseAPI-0.0.4/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.3/CheeseAPI/system.py` & `CheeseAPI-0.0.4/CheeseAPI/system.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.3/CheeseAPI/websocket.py` & `CheeseAPI-0.0.4/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.3/CheeseAPI.egg-info/PKG-INFO` & `CheeseAPI-0.0.4/CheeseAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheeseAPI
-Version: 0.0.3
+Version: 0.0.4
 Summary: 一款基于uvicorn的web协程框架
 Home-page: https://github.com/CheeseUnknown/CheeseAPI
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: api framework backend asyncio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CheeseAPI-0.0.3/CheeseAPI.egg-info/SOURCES.txt` & `CheeseAPI-0.0.4/CheeseAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.3/LICENSE` & `CheeseAPI-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.3/PKG-INFO` & `CheeseAPI-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheeseAPI
-Version: 0.0.3
+Version: 0.0.4
 Summary: 一款基于uvicorn的web协程框架
 Home-page: https://github.com/CheeseUnknown/CheeseAPI
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: api framework backend asyncio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CheeseAPI-0.0.3/README.md` & `CheeseAPI-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.3/setup.py` & `CheeseAPI-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('./README.md', 'r', encoding = 'utf-8') as f:
     longDescription = f.read()
 
 setuptools.setup(
     name = 'CheeseAPI',
-    version = '0.0.3',
+    version = '0.0.4',
     author = 'Cheese Unknown',
     author_email = 'cheese@cheese.ren',
     description = '一款基于uvicorn的web协程框架',
     long_description = longDescription,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/CheeseUnknown/CheeseAPI',
     license = 'MIT',
```

