# Comparing `tmp/fps_kernels-0.2.0.tar.gz` & `tmp/fps_kernels-0.2.1.tar.gz`

## Comparing `fps_kernels-0.2.0.tar` & `fps_kernels-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/fps_kernels/main.py
--rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/COPYING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fps_kernels-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/fps_kernels/main.py
+-rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/COPYING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fps_kernels-0.2.1/PKG-INFO
```

### Comparing `fps_kernels-0.2.0/fps_kernels/main.py` & `fps_kernels-0.2.1/fps_kernels/main.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.2.0/fps_kernels/routes.py` & `fps_kernels-0.2.1/fps_kernels/routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,17 +131,18 @@
 
     async def get_sessions(
         self,
         user: User,
     ):
         for session in self.sessions.values():
             kernel_id = session.kernel.id
-            kernel_server = kernels[kernel_id]["server"]
-            session.kernel.last_activity = kernel_server.last_activity["date"]
-            session.kernel.execution_state = kernel_server.last_activity["execution_state"]
+            if kernel_id in kernels:
+                kernel_server = kernels[kernel_id]["server"]
+                session.kernel.last_activity = kernel_server.last_activity["date"]
+                session.kernel.execution_state = kernel_server.last_activity["execution_state"]
         return list(self.sessions.values())
 
     async def create_session(
         self,
         request: Request,
         user: User,
     ):
@@ -303,15 +304,15 @@
         accepted_websocket = AcceptedWebSocket(websocket, subprotocol)
         if kernel_id in kernels:
             kernel_server = kernels[kernel_id]["server"]
             if kernel_server is None:
                 # this is an external kernel
                 # kernel is already launched, just start a kernel server
                 kernel_server = KernelServer(
-                    connection_file=kernel_id,
+                    connection_file=self.kernel_id_to_connection_file[kernel_id],
                     write_connection_file=False,
                 )
                 await kernel_server.start(launch_kernel=False)
                 kernels[kernel_id]["server"] = kernel_server
             await kernel_server.serve(accepted_websocket, session_id, permissions)
 
     async def watch_connection_files(self, path: Path) -> None:
@@ -339,23 +340,24 @@
                     to_delete.append(p)
         for p in to_delete:
             del file_changes[p]
         # process file changes
         for path, cs in file_changes.items():
             for change in cs:
                 if change == Change.deleted:
-                    if path in kernels:
+                    if path in self.kernel_id_to_connection_file.values():
                         kernel_id = list(self.kernel_id_to_connection_file.keys())[
                             list(self.kernel_id_to_connection_file.values()).index(path)
                         ]
+                        del self.kernel_id_to_connection_file[kernel_id]
                         del kernels[kernel_id]
                 elif change == Change.added:
                     try:
                         data = json.loads(Path(path).read_text())
-                    except BaseException:
+                    except Exception:
                         continue
                     if "kernel_name" not in data or "key" not in data:
                         continue
                     # looks like a kernel connection file
                     kernel_id = str(uuid.uuid4())
                     self.kernel_id_to_connection_file[kernel_id] = path
                     kernels[kernel_id] = {
```

### Comparing `fps_kernels-0.2.0/fps_kernels/kernel_driver/connect.py` & `fps_kernels-0.2.1/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.2.0/fps_kernels/kernel_driver/driver.py` & `fps_kernels-0.2.1/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.2.0/fps_kernels/kernel_driver/kernelspec.py` & `fps_kernels-0.2.1/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.2.0/fps_kernels/kernel_driver/message.py` & `fps_kernels-0.2.1/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.2.0/fps_kernels/kernel_driver/paths.py` & `fps_kernels-0.2.1/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.2.0/fps_kernels/kernel_server/message.py` & `fps_kernels-0.2.1/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.2.0/fps_kernels/kernel_server/server.py` & `fps_kernels-0.2.1/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.2.0/.gitignore` & `fps_kernels-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.2.0/COPYING.md` & `fps_kernels-0.2.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.2.0/pyproject.toml` & `fps_kernels-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.2.0/PKG-INFO` & `fps_kernels-0.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_kernels
-Version: 0.2.0
+Version: 0.2.1
 Summary: An FPS plugin for the kernels API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

