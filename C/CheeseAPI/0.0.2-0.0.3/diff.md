# Comparing `tmp/CheeseAPI-0.0.2.tar.gz` & `tmp/CheeseAPI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheeseAPI-0.0.2.tar", last modified: Tue Aug  1 08:13:05 2023, max compression
+gzip compressed data, was "CheeseAPI-0.0.3.tar", last modified: Wed Aug  2 02:05:39 2023, max compression
```

## Comparing `CheeseAPI-0.0.2.tar` & `CheeseAPI-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 08:13:05.388426 CheeseAPI-0.0.2/
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 08:13:05.387276 CheeseAPI-0.0.2/CheeseAPI/
--rw-r--r--   0 cheese     (501) staff       (20)      255 2023-08-01 08:05:36.000000 CheeseAPI-0.0.2/CheeseAPI/__init__.py
--rw-r--r--   0 cheese     (501) staff       (20)    21070 2023-08-01 08:10:18.000000 CheeseAPI-0.0.2/CheeseAPI/app.py
--rw-r--r--   0 cheese     (501) staff       (20)     1153 2023-08-01 07:06:19.000000 CheeseAPI-0.0.2/CheeseAPI/cSignal.py
--rw-r--r--   0 cheese     (501) staff       (20)      492 2023-07-31 08:17:28.000000 CheeseAPI-0.0.2/CheeseAPI/exception.py
--rw-r--r--   0 cheese     (501) staff       (20)     2434 2023-08-01 05:36:54.000000 CheeseAPI-0.0.2/CheeseAPI/file.py
--rw-r--r--   0 cheese     (501) staff       (20)     2287 2023-07-31 16:29:49.000000 CheeseAPI-0.0.2/CheeseAPI/module.py
--rw-r--r--   0 cheese     (501) staff       (20)     3675 2023-08-01 08:04:57.000000 CheeseAPI-0.0.2/CheeseAPI/request.py
--rw-r--r--   0 cheese     (501) staff       (20)    12440 2023-08-01 08:05:03.000000 CheeseAPI-0.0.2/CheeseAPI/response.py
--rw-r--r--   0 cheese     (501) staff       (20)     4317 2023-08-01 06:17:09.000000 CheeseAPI-0.0.2/CheeseAPI/route.py
--rw-r--r--   0 cheese     (501) staff       (20)     3526 2023-08-01 08:05:19.000000 CheeseAPI-0.0.2/CheeseAPI/server.py
--rw-r--r--   0 cheese     (501) staff       (20)      676 2023-07-31 08:11:41.000000 CheeseAPI-0.0.2/CheeseAPI/system.py
--rw-r--r--   0 cheese     (501) staff       (20)     1345 2023-08-01 07:01:25.000000 CheeseAPI-0.0.2/CheeseAPI/websocket.py
--rw-r--r--   0 cheese     (501) staff       (20)      295 2023-07-31 08:11:30.000000 CheeseAPI-0.0.2/CheeseAPI/workspace.py
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 08:13:05.387931 CheeseAPI-0.0.2/CheeseAPI.egg-info/
--rw-r--r--   0 cheese     (501) staff       (20)     7852 2023-08-01 08:13:05.000000 CheeseAPI-0.0.2/CheeseAPI.egg-info/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)      459 2023-08-01 08:13:05.000000 CheeseAPI-0.0.2/CheeseAPI.egg-info/SOURCES.txt
--rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-01 08:13:05.000000 CheeseAPI-0.0.2/CheeseAPI.egg-info/dependency_links.txt
--rw-r--r--   0 cheese     (501) staff       (20)       57 2023-08-01 08:13:05.000000 CheeseAPI-0.0.2/CheeseAPI.egg-info/requires.txt
--rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-01 08:13:05.000000 CheeseAPI-0.0.2/CheeseAPI.egg-info/top_level.txt
--rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 13:50:19.000000 CheeseAPI-0.0.2/LICENSE
--rw-r--r--   0 cheese     (501) staff       (20)     7852 2023-08-01 08:13:05.388221 CheeseAPI-0.0.2/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)     7401 2023-08-01 07:41:22.000000 CheeseAPI-0.0.2/README.md
--rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-01 08:13:05.388475 CheeseAPI-0.0.2/setup.cfg
--rw-r--r--   0 cheese     (501) staff       (20)      865 2023-08-01 08:12:41.000000 CheeseAPI-0.0.2/setup.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 02:05:39.424415 CheeseAPI-0.0.3/
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 02:05:39.423156 CheeseAPI-0.0.3/CheeseAPI/
+-rw-r--r--   0 cheese     (501) staff       (20)      255 2023-08-01 09:51:10.000000 CheeseAPI-0.0.3/CheeseAPI/__init__.py
+-rw-r--r--   0 cheese     (501) staff       (20)    16039 2023-08-02 01:49:39.000000 CheeseAPI-0.0.3/CheeseAPI/app.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1636 2023-08-01 09:45:24.000000 CheeseAPI-0.0.3/CheeseAPI/cSignal.py
+-rw-r--r--   0 cheese     (501) staff       (20)     5440 2023-08-02 02:04:56.000000 CheeseAPI-0.0.3/CheeseAPI/command.py
+-rw-r--r--   0 cheese     (501) staff       (20)      492 2023-07-31 08:17:28.000000 CheeseAPI-0.0.3/CheeseAPI/exception.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2434 2023-08-01 05:36:54.000000 CheeseAPI-0.0.3/CheeseAPI/file.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2287 2023-08-01 09:12:11.000000 CheeseAPI-0.0.3/CheeseAPI/module.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3675 2023-08-01 08:04:57.000000 CheeseAPI-0.0.3/CheeseAPI/request.py
+-rw-r--r--   0 cheese     (501) staff       (20)    12440 2023-08-01 08:05:03.000000 CheeseAPI-0.0.3/CheeseAPI/response.py
+-rw-r--r--   0 cheese     (501) staff       (20)     4317 2023-08-01 06:17:09.000000 CheeseAPI-0.0.3/CheeseAPI/route.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3526 2023-08-01 08:05:19.000000 CheeseAPI-0.0.3/CheeseAPI/server.py
+-rw-r--r--   0 cheese     (501) staff       (20)      676 2023-07-31 08:11:41.000000 CheeseAPI-0.0.3/CheeseAPI/system.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1345 2023-08-01 07:01:25.000000 CheeseAPI-0.0.3/CheeseAPI/websocket.py
+-rw-r--r--   0 cheese     (501) staff       (20)      295 2023-07-31 08:11:30.000000 CheeseAPI-0.0.3/CheeseAPI/workspace.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 02:05:39.424079 CheeseAPI-0.0.3/CheeseAPI.egg-info/
+-rw-r--r--   0 cheese     (501) staff       (20)     7909 2023-08-02 02:05:39.000000 CheeseAPI-0.0.3/CheeseAPI.egg-info/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)      516 2023-08-02 02:05:39.000000 CheeseAPI-0.0.3/CheeseAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-02 02:05:39.000000 CheeseAPI-0.0.3/CheeseAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       56 2023-08-02 02:05:39.000000 CheeseAPI-0.0.3/CheeseAPI.egg-info/entry_points.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       57 2023-08-02 02:05:39.000000 CheeseAPI-0.0.3/CheeseAPI.egg-info/requires.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-02 02:05:39.000000 CheeseAPI-0.0.3/CheeseAPI.egg-info/top_level.txt
+-rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 13:50:19.000000 CheeseAPI-0.0.3/LICENSE
+-rw-r--r--   0 cheese     (501) staff       (20)     7909 2023-08-02 02:05:39.424286 CheeseAPI-0.0.3/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)     7458 2023-08-02 01:58:40.000000 CheeseAPI-0.0.3/README.md
+-rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-02 02:05:39.424460 CheeseAPI-0.0.3/setup.cfg
+-rw-r--r--   0 cheese     (501) staff       (20)      984 2023-08-02 01:57:12.000000 CheeseAPI-0.0.3/setup.py
```

### Comparing `CheeseAPI-0.0.2/CheeseAPI/file.py` & `CheeseAPI-0.0.3/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.2/CheeseAPI/module.py` & `CheeseAPI-0.0.3/CheeseAPI/module.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.2/CheeseAPI/request.py` & `CheeseAPI-0.0.3/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.2/CheeseAPI/response.py` & `CheeseAPI-0.0.3/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.2/CheeseAPI/route.py` & `CheeseAPI-0.0.3/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.2/CheeseAPI/server.py` & `CheeseAPI-0.0.3/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.2/CheeseAPI/system.py` & `CheeseAPI-0.0.3/CheeseAPI/system.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.2/CheeseAPI/websocket.py` & `CheeseAPI-0.0.3/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.2/CheeseAPI.egg-info/PKG-INFO` & `CheeseAPI-0.0.3/CheeseAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheeseAPI
-Version: 0.0.2
+Version: 0.0.3
 Summary: 一款基于uvicorn的web协程框架
 Home-page: https://github.com/CheeseUnknown/CheeseAPI
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: api framework backend asyncio
 Classifier: License :: OSI Approved :: MIT License
@@ -46,30 +46,25 @@
 ### **简单的示例**
 
 创建一个入口文件：
 
 ```python
 # File path: /app.py
 
-from CheeseAPI import App, Request, Response
-
-app = App()
+from CheeseAPI import app, Request, Response
 
 @app.route('/', [ 'GET' ])
 async def index(request: Request):
     return Response('你好，这里是CheeseAPI！')
-
-if __name__ == '__main__':
-    app.run()
 ```
 
 使用命令行启动服务器，你可以看到相应的信息打印在控制台上（默认为彩色打印）:
 
 ```bash
-$ python app.py
+$ CheeseAPI --app app:app
 (STARTING) 2023-08-01 00:44:11.143085 > Started CheeseAPI master process 92102
 (STARTING) 2023-08-01 00:44:11.143122 > The application starts loading...
 (STARTING) 2023-08-01 00:44:11.143133 > System information:
     system: MacOS
     python version: 3.11.4
     CheeseAPI version: 0.0.1
 (STARTING) 2023-08-01 00:44:11.143142 > Workspace information:
@@ -178,15 +173,15 @@
 # 获取用户
 def get_user(id: uuid.UUID) -> User | None:
     if id in users:
         return users[id]
     return None
 
 # 修改用户信息
-def set_user(id: uuid:UUID, nickname: str | None, password: str | None, gender: Gender | None) -> User | None:
+def set_user(id: uuid.UUID, nickname: str | None, password: str | None, gender: Gender | None) -> User | None:
     if id in users:
         user = users[id]
         if nickname:
             user.nickname = nickname
         if password:
             user.password = password
         if gender:
@@ -244,47 +239,49 @@
 def get_user(id: uuid.UUID):
     user = service.get_user(id)
     if user:
         return JsonResponse(user.__dict__)
     return Response('查找失败！', 404)
 
 @route.put('/<id:uuid>')
-def set_user(id: uuid:UUID):
+def set_user(id: uuid.UUID):
     nickname = request.form.get('nickname')
     password = request.form.get('password')
     gender = request.form.get('gender')
     if gender:
         gender = Gender(gender)
     user = service.set_user(id, nickname, password, gender)
     if user:
         return JsonResponse(user.__dict__)
     return Response('修改信息失败！', 404)
 
 @route.delete('/<id:uuid>')
-def delete_user(id: uuid:UUID):
+def delete_user(id: uuid.UUID):
     flag = service.delete_user(id)
     if flag:
         return Response('删除用户成功！')
     return Response('删除用户失败！', 404)
 ```
 
 这样，一个简陋的用户系统就搭建完成了，其中有很多纰漏例如会把密码返回出去 :(
 
 ## **更多...**
 
-### 1. **[详细配置](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/detail.md)**
+### 1. **[命令行](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/command.md)**
+
+### 2. **[详细配置](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/detail.md)**
 
-### 2. **[模块](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/module.md)**
+### 3. **[模块](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/module.md)**
 
-### 3. **[路由](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/route.md)**
+### 4. **[路由](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/route.md)**
 
-### 4. **[请求](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/request.md)**
+### 5. **[请求](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/request.md)**
 
-### 5. **[响应](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/response.md)**
+### 6. **[响应](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/response.md)**
 
-### 6. **[装饰器](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/decorator.md)**
+### 7. **[装饰器](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/decorator.md)**
 
-### 7. **[websocket](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/websocket.md)**
+### 8. **[websocket](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/websocket.md)**
 
-### 8. **[信号](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/signal.md)**
+### 9. **[信号](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/signal.md)**
 
-### 9. **[文件](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/file.md)**
+### 10. **[文件](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/file.md)**
```

### Comparing `CheeseAPI-0.0.2/LICENSE` & `CheeseAPI-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.2/PKG-INFO` & `CheeseAPI-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheeseAPI
-Version: 0.0.2
+Version: 0.0.3
 Summary: 一款基于uvicorn的web协程框架
 Home-page: https://github.com/CheeseUnknown/CheeseAPI
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: api framework backend asyncio
 Classifier: License :: OSI Approved :: MIT License
@@ -46,30 +46,25 @@
 ### **简单的示例**
 
 创建一个入口文件：
 
 ```python
 # File path: /app.py
 
-from CheeseAPI import App, Request, Response
-
-app = App()
+from CheeseAPI import app, Request, Response
 
 @app.route('/', [ 'GET' ])
 async def index(request: Request):
     return Response('你好，这里是CheeseAPI！')
-
-if __name__ == '__main__':
-    app.run()
 ```
 
 使用命令行启动服务器，你可以看到相应的信息打印在控制台上（默认为彩色打印）:
 
 ```bash
-$ python app.py
+$ CheeseAPI --app app:app
 (STARTING) 2023-08-01 00:44:11.143085 > Started CheeseAPI master process 92102
 (STARTING) 2023-08-01 00:44:11.143122 > The application starts loading...
 (STARTING) 2023-08-01 00:44:11.143133 > System information:
     system: MacOS
     python version: 3.11.4
     CheeseAPI version: 0.0.1
 (STARTING) 2023-08-01 00:44:11.143142 > Workspace information:
@@ -178,15 +173,15 @@
 # 获取用户
 def get_user(id: uuid.UUID) -> User | None:
     if id in users:
         return users[id]
     return None
 
 # 修改用户信息
-def set_user(id: uuid:UUID, nickname: str | None, password: str | None, gender: Gender | None) -> User | None:
+def set_user(id: uuid.UUID, nickname: str | None, password: str | None, gender: Gender | None) -> User | None:
     if id in users:
         user = users[id]
         if nickname:
             user.nickname = nickname
         if password:
             user.password = password
         if gender:
@@ -244,47 +239,49 @@
 def get_user(id: uuid.UUID):
     user = service.get_user(id)
     if user:
         return JsonResponse(user.__dict__)
     return Response('查找失败！', 404)
 
 @route.put('/<id:uuid>')
-def set_user(id: uuid:UUID):
+def set_user(id: uuid.UUID):
     nickname = request.form.get('nickname')
     password = request.form.get('password')
     gender = request.form.get('gender')
     if gender:
         gender = Gender(gender)
     user = service.set_user(id, nickname, password, gender)
     if user:
         return JsonResponse(user.__dict__)
     return Response('修改信息失败！', 404)
 
 @route.delete('/<id:uuid>')
-def delete_user(id: uuid:UUID):
+def delete_user(id: uuid.UUID):
     flag = service.delete_user(id)
     if flag:
         return Response('删除用户成功！')
     return Response('删除用户失败！', 404)
 ```
 
 这样，一个简陋的用户系统就搭建完成了，其中有很多纰漏例如会把密码返回出去 :(
 
 ## **更多...**
 
-### 1. **[详细配置](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/detail.md)**
+### 1. **[命令行](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/command.md)**
+
+### 2. **[详细配置](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/detail.md)**
 
-### 2. **[模块](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/module.md)**
+### 3. **[模块](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/module.md)**
 
-### 3. **[路由](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/route.md)**
+### 4. **[路由](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/route.md)**
 
-### 4. **[请求](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/request.md)**
+### 5. **[请求](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/request.md)**
 
-### 5. **[响应](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/response.md)**
+### 6. **[响应](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/response.md)**
 
-### 6. **[装饰器](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/decorator.md)**
+### 7. **[装饰器](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/decorator.md)**
 
-### 7. **[websocket](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/websocket.md)**
+### 8. **[websocket](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/websocket.md)**
 
-### 8. **[信号](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/signal.md)**
+### 9. **[信号](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/signal.md)**
 
-### 9. **[文件](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/file.md)**
+### 10. **[文件](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/file.md)**
```

### Comparing `CheeseAPI-0.0.2/README.md` & `CheeseAPI-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,30 +31,25 @@
 ### **简单的示例**
 
 创建一个入口文件：
 
 ```python
 # File path: /app.py
 
-from CheeseAPI import App, Request, Response
-
-app = App()
+from CheeseAPI import app, Request, Response
 
 @app.route('/', [ 'GET' ])
 async def index(request: Request):
     return Response('你好，这里是CheeseAPI！')
-
-if __name__ == '__main__':
-    app.run()
 ```
 
 使用命令行启动服务器，你可以看到相应的信息打印在控制台上（默认为彩色打印）:
 
 ```bash
-$ python app.py
+$ CheeseAPI --app app:app
 (STARTING) 2023-08-01 00:44:11.143085 > Started CheeseAPI master process 92102
 (STARTING) 2023-08-01 00:44:11.143122 > The application starts loading...
 (STARTING) 2023-08-01 00:44:11.143133 > System information:
     system: MacOS
     python version: 3.11.4
     CheeseAPI version: 0.0.1
 (STARTING) 2023-08-01 00:44:11.143142 > Workspace information:
@@ -163,15 +158,15 @@
 # 获取用户
 def get_user(id: uuid.UUID) -> User | None:
     if id in users:
         return users[id]
     return None
 
 # 修改用户信息
-def set_user(id: uuid:UUID, nickname: str | None, password: str | None, gender: Gender | None) -> User | None:
+def set_user(id: uuid.UUID, nickname: str | None, password: str | None, gender: Gender | None) -> User | None:
     if id in users:
         user = users[id]
         if nickname:
             user.nickname = nickname
         if password:
             user.password = password
         if gender:
@@ -229,47 +224,49 @@
 def get_user(id: uuid.UUID):
     user = service.get_user(id)
     if user:
         return JsonResponse(user.__dict__)
     return Response('查找失败！', 404)
 
 @route.put('/<id:uuid>')
-def set_user(id: uuid:UUID):
+def set_user(id: uuid.UUID):
     nickname = request.form.get('nickname')
     password = request.form.get('password')
     gender = request.form.get('gender')
     if gender:
         gender = Gender(gender)
     user = service.set_user(id, nickname, password, gender)
     if user:
         return JsonResponse(user.__dict__)
     return Response('修改信息失败！', 404)
 
 @route.delete('/<id:uuid>')
-def delete_user(id: uuid:UUID):
+def delete_user(id: uuid.UUID):
     flag = service.delete_user(id)
     if flag:
         return Response('删除用户成功！')
     return Response('删除用户失败！', 404)
 ```
 
 这样，一个简陋的用户系统就搭建完成了，其中有很多纰漏例如会把密码返回出去 :(
 
 ## **更多...**
 
-### 1. **[详细配置](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/detail.md)**
+### 1. **[命令行](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/command.md)**
+
+### 2. **[详细配置](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/detail.md)**
 
-### 2. **[模块](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/module.md)**
+### 3. **[模块](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/module.md)**
 
-### 3. **[路由](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/route.md)**
+### 4. **[路由](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/route.md)**
 
-### 4. **[请求](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/request.md)**
+### 5. **[请求](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/request.md)**
 
-### 5. **[响应](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/response.md)**
+### 6. **[响应](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/response.md)**
 
-### 6. **[装饰器](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/decorator.md)**
+### 7. **[装饰器](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/decorator.md)**
 
-### 7. **[websocket](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/websocket.md)**
+### 8. **[websocket](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/websocket.md)**
 
-### 8. **[信号](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/signal.md)**
+### 9. **[信号](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/signal.md)**
 
-### 9. **[文件](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/file.md)**
+### 10. **[文件](https://github.com/CheeseUnknown/CheeseAPI/tree/master/documents/file.md)**
```

### Comparing `CheeseAPI-0.0.2/setup.py` & `CheeseAPI-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import setuptools
 
 with open('./README.md', 'r', encoding = 'utf-8') as f:
     longDescription = f.read()
 
 setuptools.setup(
     name = 'CheeseAPI',
-    version = '0.0.2',
+    version = '0.0.3',
     author = 'Cheese Unknown',
     author_email = 'cheese@cheese.ren',
     description = '一款基于uvicorn的web协程框架',
     long_description = longDescription,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/CheeseUnknown/CheeseAPI',
     license = 'MIT',
     classifiers = [
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.11'
     ],
     keywords = 'api framework backend asyncio',
     python_requires = '>=3.11',
+    entry_points = {
+        'console_scripts': [
+            'CheeseAPI = CheeseAPI.command:command'
+        ]
+    },
     install_requires = [
         'uvicorn[standard]',
         'CheeseType',
         'CheeseLog',
         'xmltodict',
         'blinker'
     ],
```

