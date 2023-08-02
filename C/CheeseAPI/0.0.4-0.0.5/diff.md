# Comparing `tmp/CheeseAPI-0.0.4.tar.gz` & `tmp/CheeseAPI-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheeseAPI-0.0.4.tar", last modified: Wed Aug  2 04:03:40 2023, max compression
+gzip compressed data, was "CheeseAPI-0.0.5.tar", last modified: Wed Aug  2 15:37:54 2023, max compression
```

## Comparing `CheeseAPI-0.0.4.tar` & `CheeseAPI-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 04:03:40.887442 CheeseAPI-0.0.4/
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 04:03:40.886371 CheeseAPI-0.0.4/CheeseAPI/
--rw-r--r--   0 cheese     (501) staff       (20)      255 2023-08-01 09:51:10.000000 CheeseAPI-0.0.4/CheeseAPI/__init__.py
--rw-r--r--   0 cheese     (501) staff       (20)    16971 2023-08-02 04:02:53.000000 CheeseAPI-0.0.4/CheeseAPI/app.py
--rw-r--r--   0 cheese     (501) staff       (20)     1636 2023-08-01 09:45:24.000000 CheeseAPI-0.0.4/CheeseAPI/cSignal.py
--rw-r--r--   0 cheese     (501) staff       (20)     6984 2023-08-02 04:02:27.000000 CheeseAPI-0.0.4/CheeseAPI/command.py
--rw-r--r--   0 cheese     (501) staff       (20)      492 2023-07-31 08:17:28.000000 CheeseAPI-0.0.4/CheeseAPI/exception.py
--rw-r--r--   0 cheese     (501) staff       (20)     2434 2023-08-01 05:36:54.000000 CheeseAPI-0.0.4/CheeseAPI/file.py
--rw-r--r--   0 cheese     (501) staff       (20)     2287 2023-08-01 09:12:11.000000 CheeseAPI-0.0.4/CheeseAPI/module.py
--rw-r--r--   0 cheese     (501) staff       (20)     3675 2023-08-01 08:04:57.000000 CheeseAPI-0.0.4/CheeseAPI/request.py
--rw-r--r--   0 cheese     (501) staff       (20)    12440 2023-08-01 08:05:03.000000 CheeseAPI-0.0.4/CheeseAPI/response.py
--rw-r--r--   0 cheese     (501) staff       (20)     4317 2023-08-01 06:17:09.000000 CheeseAPI-0.0.4/CheeseAPI/route.py
--rw-r--r--   0 cheese     (501) staff       (20)     3526 2023-08-01 08:05:19.000000 CheeseAPI-0.0.4/CheeseAPI/server.py
--rw-r--r--   0 cheese     (501) staff       (20)      676 2023-07-31 08:11:41.000000 CheeseAPI-0.0.4/CheeseAPI/system.py
--rw-r--r--   0 cheese     (501) staff       (20)     1345 2023-08-01 07:01:25.000000 CheeseAPI-0.0.4/CheeseAPI/websocket.py
--rw-r--r--   0 cheese     (501) staff       (20)      295 2023-07-31 08:11:30.000000 CheeseAPI-0.0.4/CheeseAPI/workspace.py
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 04:03:40.887130 CheeseAPI-0.0.4/CheeseAPI.egg-info/
--rw-r--r--   0 cheese     (501) staff       (20)     7909 2023-08-02 04:03:40.000000 CheeseAPI-0.0.4/CheeseAPI.egg-info/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)      516 2023-08-02 04:03:40.000000 CheeseAPI-0.0.4/CheeseAPI.egg-info/SOURCES.txt
--rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-02 04:03:40.000000 CheeseAPI-0.0.4/CheeseAPI.egg-info/dependency_links.txt
--rw-r--r--   0 cheese     (501) staff       (20)       56 2023-08-02 04:03:40.000000 CheeseAPI-0.0.4/CheeseAPI.egg-info/entry_points.txt
--rw-r--r--   0 cheese     (501) staff       (20)       57 2023-08-02 04:03:40.000000 CheeseAPI-0.0.4/CheeseAPI.egg-info/requires.txt
--rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-02 04:03:40.000000 CheeseAPI-0.0.4/CheeseAPI.egg-info/top_level.txt
--rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 13:50:19.000000 CheeseAPI-0.0.4/LICENSE
--rw-r--r--   0 cheese     (501) staff       (20)     7909 2023-08-02 04:03:40.887317 CheeseAPI-0.0.4/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)     7458 2023-08-02 01:58:40.000000 CheeseAPI-0.0.4/README.md
--rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-02 04:03:40.887487 CheeseAPI-0.0.4/setup.cfg
--rw-r--r--   0 cheese     (501) staff       (20)      984 2023-08-02 04:03:24.000000 CheeseAPI-0.0.4/setup.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 15:37:54.390228 CheeseAPI-0.0.5/
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 15:37:54.387680 CheeseAPI-0.0.5/CheeseAPI/
+-rw-r--r--   0 cheese     (501) staff       (20)      255 2023-08-01 09:51:10.000000 CheeseAPI-0.0.5/CheeseAPI/__init__.py
+-rw-r--r--   0 cheese     (501) staff       (20)    16971 2023-08-02 15:14:07.000000 CheeseAPI-0.0.5/CheeseAPI/app.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1636 2023-08-01 09:45:24.000000 CheeseAPI-0.0.5/CheeseAPI/cSignal.py
+-rw-r--r--   0 cheese     (501) staff       (20)     8370 2023-08-02 15:37:10.000000 CheeseAPI-0.0.5/CheeseAPI/command.py
+-rw-r--r--   0 cheese     (501) staff       (20)      492 2023-07-31 08:17:28.000000 CheeseAPI-0.0.5/CheeseAPI/exception.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2434 2023-08-01 05:36:54.000000 CheeseAPI-0.0.5/CheeseAPI/file.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2287 2023-08-01 09:12:11.000000 CheeseAPI-0.0.5/CheeseAPI/module.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3675 2023-08-01 08:04:57.000000 CheeseAPI-0.0.5/CheeseAPI/request.py
+-rw-r--r--   0 cheese     (501) staff       (20)    12440 2023-08-01 08:05:03.000000 CheeseAPI-0.0.5/CheeseAPI/response.py
+-rw-r--r--   0 cheese     (501) staff       (20)     4317 2023-08-01 06:17:09.000000 CheeseAPI-0.0.5/CheeseAPI/route.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3709 2023-08-02 09:26:09.000000 CheeseAPI-0.0.5/CheeseAPI/server.py
+-rw-r--r--   0 cheese     (501) staff       (20)      676 2023-07-31 08:11:41.000000 CheeseAPI-0.0.5/CheeseAPI/system.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1345 2023-08-01 07:01:25.000000 CheeseAPI-0.0.5/CheeseAPI/websocket.py
+-rw-r--r--   0 cheese     (501) staff       (20)      295 2023-07-31 08:11:30.000000 CheeseAPI-0.0.5/CheeseAPI/workspace.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 15:37:54.389349 CheeseAPI-0.0.5/CheeseAPI.egg-info/
+-rw-r--r--   0 cheese     (501) staff       (20)     7909 2023-08-02 15:37:54.000000 CheeseAPI-0.0.5/CheeseAPI.egg-info/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)      516 2023-08-02 15:37:54.000000 CheeseAPI-0.0.5/CheeseAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-02 15:37:54.000000 CheeseAPI-0.0.5/CheeseAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       56 2023-08-02 15:37:54.000000 CheeseAPI-0.0.5/CheeseAPI.egg-info/entry_points.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       57 2023-08-02 15:37:54.000000 CheeseAPI-0.0.5/CheeseAPI.egg-info/requires.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-02 15:37:54.000000 CheeseAPI-0.0.5/CheeseAPI.egg-info/top_level.txt
+-rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 13:50:19.000000 CheeseAPI-0.0.5/LICENSE
+-rw-r--r--   0 cheese     (501) staff       (20)     7909 2023-08-02 15:37:54.389937 CheeseAPI-0.0.5/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)     7458 2023-08-02 01:58:40.000000 CheeseAPI-0.0.5/README.md
+-rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-02 15:37:54.390357 CheeseAPI-0.0.5/setup.cfg
+-rw-r--r--   0 cheese     (501) staff       (20)      984 2023-08-02 15:37:32.000000 CheeseAPI-0.0.5/setup.py
```

### Comparing `CheeseAPI-0.0.4/CheeseAPI/app.py` & `CheeseAPI-0.0.5/CheeseAPI/app.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.4/CheeseAPI/cSignal.py` & `CheeseAPI-0.0.5/CheeseAPI/cSignal.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.4/CheeseAPI/command.py` & `CheeseAPI-0.0.5/CheeseAPI/command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-import argparse, time, os, traceback, json, shutil
+import argparse, time, os, traceback, json, shutil, importlib, importlib.util
 
 import CheeseLog, uvicorn, CheeseType, CheeseType.network, uvicorn.importer
 
+from .module import Module, LocalModule
+
 def command():
     from .app import app
     from .cSignal import signal
 
     parser = argparse.ArgumentParser()
     parser.add_argument('--app', nargs = '?', default = 'app:app', help = '服务器本服务【默认值：app:app】')
     parser.add_argument('--host', nargs = '?', default = '127.0.0.1', help = '服务器地址【默认值：127.0.0.1】')
-    parser.add_argument('--port', nargs = '?', default = 5214, help = '端口号【默认值：5214】')
-    parser.add_argument('--reload', nargs = '?', default = False, help = '热更新。与workers冲突【默认值：False】')
-    parser.add_argument('--workers', nargs = '?', default = 1, help = 'workers为0时会自动设置为cpu核数*2。与reload冲突【默认值：1】')
+    parser.add_argument('--port', type = int, nargs = '?', default = 5214, help = '端口号【默认值：5214】')
+    parser.add_argument('--reload', action='store_true', help = '热更新。与workers冲突【默认值：False】')
+    parser.add_argument('--workers', type = int, nargs = '?', default = 1, help = 'workers为0时会自动设置为cpu核数*2。与reload冲突【默认值：1】')
     parser.add_argument('--log_path', nargs = '?', default = '/logs/', help = '日志文件夹的相对路径【默认值：/logs/】')
     parser.add_argument('--log_filename', nargs = '?', default = False, help = '日志文件名。当值为True时，自动设置为%%Y_%%m_%%d-%%H_%%M_%%S.log；当值为False，关闭日志文件记录；自定义文件名也是允许的【默认值：True】')
     args = parser.parse_args()
 
     startTimer: float = time.time()
 
     _app = args.app
@@ -25,14 +27,17 @@
     workers = CheeseType.NonNegativeInt(args.workers)
     log_path = args.log_path
     try:
         log_filename = CheeseType.Bool(args.log_filename)
     except:
         ...
 
+    if reload:
+        workers = 1
+
     app.workspace.LOG_PATH = log_path
     app.server.LOG_FILENAME = log_filename
     app.server.HOST = host
     app.server.PORT = port
     app.server.IS_RELOAD = reload
     app.server.WORKERS = workers
 
@@ -97,14 +102,42 @@
 is debug: \033[34m{app.server.IS_DEBUG}\033[0m
 is request logged: \033[34m{app.server.IS_REQUEST_LOGGED}\033[0m''' + (f'''
 static path: \033[34m{app.server.STATIC_PATH}\033[0m''' if app.server.STATIC_PATH is not False else '') + (f'''
 current log file path: \033[4;36m.{app.logger.filePath[len(app.workspace.BASE_PATH):]}\033[0m''' if app.server.LOG_FILENAME is not False else ''))
 
     CheeseLog.starting(f'The server running on http://{app.server.HOST}:{app.server.PORT}', f'The server running on \033[4;36mhttp://{app.server.HOST}:{app.server.PORT}\033[0m')
 
+    import sys
+    sys.path.append(os.getcwd())
+    app = __import__(_app.split(':')[0]).app
+
+    _modules = set()
+    if len(app.modules):
+        CheeseLog.starting(f'Modules:\n{" | ".join(app.modules)}')
+    for module in app.modules:
+        _modules.add(Module(_modules, module))
+    app.modules = _modules
+
+    if app.localModules is True:
+        app.localModules = set()
+        for folderName in os.listdir(app.workspace.BASE_PATH):
+            if folderName[0] == '.':
+                continue
+            if folderName in app.exclude_localModules:
+                continue
+            folderPath = os.path.join(app.workspace.BASE_PATH, folderName)
+            if os.path.isdir(folderPath) and folderPath not in [ app.workspace.BASE_PATH + app.workspace.STATIC_PATH[:-1], app.workspace.BASE_PATH + app.workspace.MEDIA_PATH[:-1], app.workspace.BASE_PATH + app.workspace.LOG_PATH[:-1], app.workspace.BASE_PATH + '/__pycache__' ]:
+                app.localModules.add(folderName)
+    if len(app.localModules):
+        CheeseLog.starting(f'Local modules:\n{" | ".join(app.localModules)}')
+    _localModules = set()
+    for module in app.localModules:
+        _localModules.add(LocalModule(app.workspace.BASE_PATH, module))
+    app.localModules = _localModules
+
     if signal.receiver('server_startingHandle'):
         signal.send('server_startingHandle')
     for server_startingHandle in app.server_startingHandles:
         server_startingHandle()
 
     try:
         uvicorn.run(
```

### Comparing `CheeseAPI-0.0.4/CheeseAPI/file.py` & `CheeseAPI-0.0.5/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.4/CheeseAPI/module.py` & `CheeseAPI-0.0.5/CheeseAPI/module.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.4/CheeseAPI/request.py` & `CheeseAPI-0.0.5/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.4/CheeseAPI/response.py` & `CheeseAPI-0.0.5/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.4/CheeseAPI/route.py` & `CheeseAPI-0.0.5/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.4/CheeseAPI/server.py` & `CheeseAPI-0.0.5/CheeseAPI/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,30 +37,33 @@
     @IS_DEBUG.setter
     def IS_DEBUG(self, value):
         self._IS_DEBUG = CheeseType.Bool(value)
         if isinstance(self._app.logger.filter, set):
             if not self._IS_DEBUG:
                 self._app.logger.filter.add('DEBUG')
             elif self._IS_DEBUG:
-                self._app.logger.filter.remove('DEBUG')
+                if 'DEBUG' in self._app.logger.filter:
+                    self._app.logger.filter.remove('DEBUG')
 
     @property
     def IS_REQUEST_LOGGED(self) -> bool:
         return self._IS_REQUEST_LOGGED
 
     @IS_REQUEST_LOGGED.setter
     def IS_REQUEST_LOGGED(self, value):
         self._IS_REQUEST_LOGGED = CheeseType.Bool(value)
         if isinstance(self._app.logger.filter, set):
             if not self._IS_REQUEST_LOGGED:
                 self._app.logger.filter.add('HTTP')
                 self._app.logger.filter.add('WEBSOCKET')
             elif self._IS_REQUEST_LOGGED:
-                self._app.logger.filter.remove('HTTP')
-                self._app.logger.filter.add('WEBSOCKET')
+                if 'HTTP' in self._app.logger.filter:
+                    self._app.logger.filter.remove('HTTP')
+                if 'WEBSOCKET' in self._app.logger.filter:
+                    self._app.logger.filter.remove('WEBSOCKET')
 
     @property
     def LOG_FILENAME(self) -> str | bool:
         return self._LOG_FILENAME
 
     @LOG_FILENAME.setter
     def LOG_FILENAME(self, value):
```

### Comparing `CheeseAPI-0.0.4/CheeseAPI/system.py` & `CheeseAPI-0.0.5/CheeseAPI/system.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.4/CheeseAPI/websocket.py` & `CheeseAPI-0.0.5/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.4/CheeseAPI.egg-info/PKG-INFO` & `CheeseAPI-0.0.5/CheeseAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheeseAPI
-Version: 0.0.4
+Version: 0.0.5
 Summary: 一款基于uvicorn的web协程框架
 Home-page: https://github.com/CheeseUnknown/CheeseAPI
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: api framework backend asyncio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CheeseAPI-0.0.4/CheeseAPI.egg-info/SOURCES.txt` & `CheeseAPI-0.0.5/CheeseAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.4/LICENSE` & `CheeseAPI-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.4/PKG-INFO` & `CheeseAPI-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheeseAPI
-Version: 0.0.4
+Version: 0.0.5
 Summary: 一款基于uvicorn的web协程框架
 Home-page: https://github.com/CheeseUnknown/CheeseAPI
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: api framework backend asyncio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CheeseAPI-0.0.4/README.md` & `CheeseAPI-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.4/setup.py` & `CheeseAPI-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('./README.md', 'r', encoding = 'utf-8') as f:
     longDescription = f.read()
 
 setuptools.setup(
     name = 'CheeseAPI',
-    version = '0.0.4',
+    version = '0.0.5',
     author = 'Cheese Unknown',
     author_email = 'cheese@cheese.ren',
     description = '一款基于uvicorn的web协程框架',
     long_description = longDescription,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/CheeseUnknown/CheeseAPI',
     license = 'MIT',
```

