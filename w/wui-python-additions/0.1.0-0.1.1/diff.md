# Comparing `tmp/wui_python_additions-0.1.0.tar.gz` & `tmp/wui_python_additions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wui_python_additions-0.1.0.tar", last modified: Wed Aug  2 16:25:31 2023, max compression
+gzip compressed data, was "wui_python_additions-0.1.1.tar", last modified: Wed Aug  2 21:18:41 2023, max compression
```

## Comparing `wui_python_additions-0.1.0.tar` & `wui_python_additions-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-08-02 16:25:31.008380 wui_python_additions-0.1.0/
--rw-rw-r--   0 igor      (1001) igor      (1001)      350 2023-08-02 16:25:31.008380 wui_python_additions-0.1.0/PKG-INFO
--rw-rw-r--   0 igor      (1001) igor      (1001)        0 2023-08-02 16:10:04.000000 wui_python_additions-0.1.0/README.md
--rw-rw-r--   0 igor      (1001) igor      (1001)      572 2023-08-02 16:24:22.000000 wui_python_additions-0.1.0/pyproject.toml
--rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-08-02 16:25:31.008380 wui_python_additions-0.1.0/setup.cfg
--rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-08-02 16:10:04.000000 wui_python_additions-0.1.0/setup.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-08-02 16:25:31.004380 wui_python_additions-0.1.0/wui_python_additions/
--rw-rw-r--   0 igor      (1001) igor      (1001)       59 2023-08-02 16:20:19.000000 wui_python_additions-0.1.0/wui_python_additions/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     6239 2023-08-02 16:15:58.000000 wui_python_additions-0.1.0/wui_python_additions/configuration.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     3345 2023-08-02 16:23:06.000000 wui_python_additions-0.1.0/wui_python_additions/process_watcher.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-08-02 16:25:31.008380 wui_python_additions-0.1.0/wui_python_additions.egg-info/
--rw-rw-r--   0 igor      (1001) igor      (1001)      350 2023-08-02 16:25:30.000000 wui_python_additions-0.1.0/wui_python_additions.egg-info/PKG-INFO
--rw-rw-r--   0 igor      (1001) igor      (1001)      320 2023-08-02 16:25:30.000000 wui_python_additions-0.1.0/wui_python_additions.egg-info/SOURCES.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-08-02 16:25:30.000000 wui_python_additions-0.1.0/wui_python_additions.egg-info/dependency_links.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)       21 2023-08-02 16:25:30.000000 wui_python_additions-0.1.0/wui_python_additions.egg-info/top_level.txt
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-08-02 21:18:41.908540 wui_python_additions-0.1.1/
+-rw-r--r--   0 igor      (1001) igor      (1001)      491 2023-08-02 16:10:04.000000 wui_python_additions-0.1.1/.gitignore
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1056 2023-08-02 16:23:17.000000 wui_python_additions-0.1.1/Makefile
+-rw-rw-r--   0 igor      (1001) igor      (1001)      350 2023-08-02 21:18:41.908540 wui_python_additions-0.1.1/PKG-INFO
+-rw-rw-r--   0 igor      (1001) igor      (1001)        0 2023-08-02 16:10:04.000000 wui_python_additions-0.1.1/README.md
+-rw-rw-r--   0 igor      (1001) igor      (1001)      593 2023-08-02 21:16:07.000000 wui_python_additions-0.1.1/pyproject.toml
+-rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-08-02 21:18:41.908540 wui_python_additions-0.1.1/setup.cfg
+-rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-08-02 16:10:04.000000 wui_python_additions-0.1.1/setup.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-08-02 21:18:41.904540 wui_python_additions-0.1.1/wui_python_additions/
+-rw-rw-r--   0 igor      (1001) igor      (1001)       59 2023-08-02 16:20:19.000000 wui_python_additions-0.1.1/wui_python_additions/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     8631 2023-08-02 21:17:21.000000 wui_python_additions-0.1.1/wui_python_additions/configuration.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     4530 2023-08-02 20:17:22.000000 wui_python_additions-0.1.1/wui_python_additions/process_watcher.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-08-02 21:18:41.908540 wui_python_additions-0.1.1/wui_python_additions.egg-info/
+-rw-rw-r--   0 igor      (1001) igor      (1001)      350 2023-08-02 21:18:41.000000 wui_python_additions-0.1.1/wui_python_additions.egg-info/PKG-INFO
+-rw-rw-r--   0 igor      (1001) igor      (1001)      383 2023-08-02 21:18:41.000000 wui_python_additions-0.1.1/wui_python_additions.egg-info/SOURCES.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-08-02 21:18:41.000000 wui_python_additions-0.1.1/wui_python_additions.egg-info/dependency_links.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)       16 2023-08-02 21:18:41.000000 wui_python_additions-0.1.1/wui_python_additions.egg-info/requires.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)       21 2023-08-02 21:18:41.000000 wui_python_additions-0.1.1/wui_python_additions.egg-info/top_level.txt
```

### Comparing `wui_python_additions-0.1.0/pyproject.toml` & `wui_python_additions-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wui_python_additions"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Igor Toropov", email="it.cups.54@gmail.com" },
 ]
 description = "TODO"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+  "autopep8==2.0.2",
 ]
 
 [tool.autopep8]
 max_line_length = 120
 ignore = []
 recursive = true
 aggressive = 5
```

### Comparing `wui_python_additions-0.1.0/wui_python_additions/process_watcher.py` & `wui_python_additions-0.1.1/wui_python_additions/process_watcher.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,48 +15,79 @@
     """Data struct to hold process information"""
     id: uuid.UUID
     start_function : typing.Callable
     args : typing.Iterable
     process: Process
 
 class ProcessWatcher():
+    """A monitoring class that starts and monitors state of launched multiprocessing processes.
+    Run processes with add_process() and then run monitor() to start monitoring all added processes.
+    """
     def __init__(self) -> None:
         self._processes : typing.Dict[uuid.UUID, ProcessData] = {}
 
-    def add_process(self, func: typing.Callable, args: typing.Iterable = []):
+    def add_process(self, func: typing.Callable, args: typing.Iterable = []) -> uuid.UUID:
+        """Runs 'func' callable with 'args' in another process and adds it appends it to monitoring list.
+
+        Args:
+            func (typing.Callable): A callable to start as process
+            args (typing.Iterable, optional): Args to callable. Defaults to [].
+
+        Returns:
+            uuid.UUID: uuid of added process
+        """
         id = uuid.uuid4()
         process = Process(target=func, args=args)
         self._processes[id] = ProcessData(id, func, args, process)
         process.start()
         return id
 
     async def terminate_process(self, id: uuid.UUID, timeout: float = 10):
+        """Terminates process
+
+        Args:
+            id (uuid.UUID): uuid of the process, acquired by add_process()
+            timeout (float, optional): timeout, if exceeded segkills process. Defaults to 10.
+        """
         p_data = self._processes[id]
         process = p_data.process
         process.terminate()
         epoch_start = time.time()
         while time.time() - epoch_start < timeout:
             if not process.is_alive():
                 break
             await asyncio.sleep(5)
         if process.is_alive():
             logger.warning(f"Process with uuid [{id}] was not terminated before timeout, SEGKILL'ing it...")
             process.kill()
         self._processes.pop(id)
     
     async def terminate_processes(self, ids: typing.List[uuid.UUID], timeout: float = 10):
+        """Terminates multiple processes
+
+        Args:
+            ids (typing.List[uuid.UUID]): list of uuid
+            timeout (float, optional): timeout for segkill. Defaults to 10.
+        """
         terminations = []
         for id in ids:
             terminations.append(asyncio.create_task(self.terminate_process(id, timeout)))
         await asyncio.gather(*terminations)
         
     async def terminate_all_processes(self, timeout: float = 10):
+        """Terminate all processes
+
+        Args:
+            timeout (float, optional): timeout for segkill. Defaults to 10.
+        """
         await self.terminate_processes(list(self._processes.keys()), timeout)
     
     async def monitor(self):
+        """Main loop in which monitoring occures
+        """
         # while not self._force_stop_flag and len(self._processes) > 0:
         while len(self._processes) > 0:
             for id in list(self._processes.keys()):
                 p_data = self._processes[id]
                 process = p_data.process
                 if process.exitcode is None and not process.is_alive(): # Not finished and not running
                     # Do your error handling and restarting here assigning the new process to processes[n]
```

