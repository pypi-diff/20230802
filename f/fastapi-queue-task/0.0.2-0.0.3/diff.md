# Comparing `tmp/fastapi_queue_task-0.0.2.tar.gz` & `tmp/fastapi_queue_task-0.0.3.tar.gz`

## Comparing `fastapi_queue_task-0.0.2.tar` & `fastapi_queue_task-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/build_and_publish.sh
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/build_and_test.sh
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/requirements.txt
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/tox.ini
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/src/fastapi_queue_task/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/src/fastapi_queue_task/constants/queue_constant.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/src/fastapi_queue_task/loggers/format.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/src/fastapi_queue_task/loggers/logger.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/src/fastapi_queue_task/services/queue_service.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/src/fastapi_queue_task/tasks/base.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/src/fastapi_queue_task/tasks/decorator.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/src/fastapi_queue_task/tasks/storage.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/src/fastapi_queue_task/type_dicts/queue_option_type.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/LICENSE
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/README.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/build_and_publish.sh
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/build_and_test.sh
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/tox.ini
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/src/fastapi_queue_task/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/src/fastapi_queue_task/constants/queue_constant.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/src/fastapi_queue_task/loggers/format.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/src/fastapi_queue_task/loggers/logger.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/src/fastapi_queue_task/services/queue_service.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/src/fastapi_queue_task/tasks/base.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/src/fastapi_queue_task/tasks/decorator.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/src/fastapi_queue_task/tasks/storage.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/src/fastapi_queue_task/type_dicts/queue_option_type.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/LICENSE
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/README.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 fastapi_queue_task-0.0.3/PKG-INFO
```

### Comparing `fastapi_queue_task-0.0.2/src/fastapi_queue_task/loggers/format.py` & `fastapi_queue_task-0.0.3/src/fastapi_queue_task/loggers/format.py`

 * *Files identical despite different names*

### Comparing `fastapi_queue_task-0.0.2/src/fastapi_queue_task/services/queue_service.py` & `fastapi_queue_task-0.0.3/src/fastapi_queue_task/services/queue_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,24 +14,27 @@
     running_tasks = set()
 
     def __init__(self, redis: Any, options: QueueOption):
         self.redis = redis
         self.concurrency = options.get('concurrency') or 10
         self.max_attempt = options.get('max_attempt') or 3
 
-    async def run(self):
+    async def __get_queue(self):
         if len(self.running_tasks) <= self.concurrency:
             detail = await self.redis.rpop(QUEUE_NAME)
             if detail:
                 task = asyncio.create_task(self.__process_queue(detail))
                 self.running_tasks.add(task)
                 task.add_done_callback(lambda t: self.running_tasks.discard(t))
 
         await asyncio.sleep(2)
-        asyncio.create_task(self.run())
+        asyncio.create_task(self.__get_queue())
+
+    def run(self):
+        asyncio.create_task(self.__get_queue())
 
     def __find_task_handler(self, name: str):
         task = pydash.find(list_tasks, lambda t: t["name"] == name)
         if task:
             return task
 
         logger.info(f"Dont have any handler for task: {task}")
```

### Comparing `fastapi_queue_task-0.0.2/src/fastapi_queue_task/tasks/base.py` & `fastapi_queue_task-0.0.3/src/fastapi_queue_task/tasks/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_queue_task-0.0.2/src/fastapi_queue_task/tasks/decorator.py` & `fastapi_queue_task-0.0.3/src/fastapi_queue_task/tasks/decorator.py`

 * *Files identical despite different names*

### Comparing `fastapi_queue_task-0.0.2/.gitignore` & `fastapi_queue_task-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_queue_task-0.0.2/LICENSE` & `fastapi_queue_task-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_queue_task-0.0.2/README.md` & `fastapi_queue_task-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 redis = from_url(
     f"redis://#REDIS_HOST:#REDIS_PORT/#REDIS_DATABASE_NAME",
     encoding="utf-8",
     decode_responses=True,
 )
 queue = Queue(redis, {'concurrency': 10, 'max_attempt': 3})
+queue.run()
 ```
 
 2. The `Queue` class expose 2 methods that we can use:
 
 ```python
 # mail_service.py
 from queue_config.py import queue
```

### Comparing `fastapi_queue_task-0.0.2/pyproject.toml` & `fastapi_queue_task-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_queue_task"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Dzung Nguyen", email="dung@megatron-solutions.com" },
 ]
 description = "FastAPI Queue"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `fastapi_queue_task-0.0.2/PKG-INFO` & `fastapi_queue_task-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_queue_task
-Version: 0.0.2
+Version: 0.0.3
 Summary: FastAPI Queue
 Project-URL: Homepage, https://github.com/megatron-global/fastapi-queue
 Project-URL: Bug Tracker, https://github.com/megatron-global/fastapi-queue/issues
 Author-email: Dzung Nguyen <dung@megatron-solutions.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,14 +26,15 @@
 
 redis = from_url(
     f"redis://#REDIS_HOST:#REDIS_PORT/#REDIS_DATABASE_NAME",
     encoding="utf-8",
     decode_responses=True,
 )
 queue = Queue(redis, {'concurrency': 10, 'max_attempt': 3})
+queue.run()
 ```
 
 2. The `Queue` class expose 2 methods that we can use:
 
 ```python
 # mail_service.py
 from queue_config.py import queue
```

