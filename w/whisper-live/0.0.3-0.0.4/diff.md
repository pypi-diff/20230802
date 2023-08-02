# Comparing `tmp/whisper-live-0.0.3.tar.gz` & `tmp/whisper-live-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-live-0.0.3.tar", last modified: Wed Aug  2 08:01:08 2023, max compression
+gzip compressed data, was "whisper-live-0.0.4.tar", last modified: Wed Aug  2 08:12:26 2023, max compression
```

## Comparing `whisper-live-0.0.3.tar` & `whisper-live-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 08:01:08.449278 whisper-live-0.0.3/
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     1085 2023-07-10 09:30:36.000000 whisper-live-0.0.3/LICENSE
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     4306 2023-08-02 08:01:08.449278 whisper-live-0.0.3/PKG-INFO
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     3848 2023-08-02 08:00:41.000000 whisper-live-0.0.3/README.md
--rw-rw-r--   0 vineet    (1000) vineet    (1000)       38 2023-08-02 08:01:08.449278 whisper-live-0.0.3/setup.cfg
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     1316 2023-08-02 08:00:56.000000 whisper-live-0.0.3/setup.py
-drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 08:01:08.449278 whisper-live-0.0.3/whisper_live/
--rw-rw-r--   0 vineet    (1000) vineet    (1000)        0 2023-07-31 14:05:43.000000 whisper-live-0.0.3/whisper_live/__init__.py
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     9412 2023-08-01 19:51:31.000000 whisper-live-0.0.3/whisper_live/client.py
--rw-rw-r--   0 vineet    (1000) vineet    (1000)    11926 2023-08-02 08:00:21.000000 whisper-live-0.0.3/whisper_live/server.py
--rw-rw-r--   0 vineet    (1000) vineet    (1000)    32804 2023-07-31 14:00:59.000000 whisper-live-0.0.3/whisper_live/transcriber.py
-drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 08:01:08.449278 whisper-live-0.0.3/whisper_live.egg-info/
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     4306 2023-08-02 08:01:08.000000 whisper-live-0.0.3/whisper_live.egg-info/PKG-INFO
--rw-rw-r--   0 vineet    (1000) vineet    (1000)      304 2023-08-02 08:01:08.000000 whisper-live-0.0.3/whisper_live.egg-info/SOURCES.txt
--rw-rw-r--   0 vineet    (1000) vineet    (1000)        1 2023-08-02 08:01:08.000000 whisper-live-0.0.3/whisper_live.egg-info/dependency_links.txt
--rw-rw-r--   0 vineet    (1000) vineet    (1000)      107 2023-08-02 08:01:08.000000 whisper-live-0.0.3/whisper_live.egg-info/requires.txt
--rw-rw-r--   0 vineet    (1000) vineet    (1000)       13 2023-08-02 08:01:08.000000 whisper-live-0.0.3/whisper_live.egg-info/top_level.txt
+drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 08:12:26.277721 whisper-live-0.0.4/
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     1085 2023-07-10 09:30:36.000000 whisper-live-0.0.4/LICENSE
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     4306 2023-08-02 08:12:26.277721 whisper-live-0.0.4/PKG-INFO
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     3848 2023-08-02 08:00:41.000000 whisper-live-0.0.4/README.md
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)       38 2023-08-02 08:12:26.277721 whisper-live-0.0.4/setup.cfg
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     1316 2023-08-02 08:11:19.000000 whisper-live-0.0.4/setup.py
+drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 08:12:26.277721 whisper-live-0.0.4/whisper_live/
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)        0 2023-07-31 14:05:43.000000 whisper-live-0.0.4/whisper_live/__init__.py
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     9299 2023-08-02 08:11:53.000000 whisper-live-0.0.4/whisper_live/client.py
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)    11926 2023-08-02 08:00:21.000000 whisper-live-0.0.4/whisper_live/server.py
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)    32804 2023-07-31 14:00:59.000000 whisper-live-0.0.4/whisper_live/transcriber.py
+drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 08:12:26.277721 whisper-live-0.0.4/whisper_live.egg-info/
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     4306 2023-08-02 08:12:26.000000 whisper-live-0.0.4/whisper_live.egg-info/PKG-INFO
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)      304 2023-08-02 08:12:26.000000 whisper-live-0.0.4/whisper_live.egg-info/SOURCES.txt
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)        1 2023-08-02 08:12:26.000000 whisper-live-0.0.4/whisper_live.egg-info/dependency_links.txt
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)      107 2023-08-02 08:12:26.000000 whisper-live-0.0.4/whisper_live.egg-info/requires.txt
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)       13 2023-08-02 08:12:26.000000 whisper-live-0.0.4/whisper_live.egg-info/top_level.txt
```

### Comparing `whisper-live-0.0.3/LICENSE` & `whisper-live-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.3/PKG-INFO` & `whisper-live-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-live
-Version: 0.0.3
+Version: 0.0.4
 Summary: A nearly-live implementation of OpenAI's Whisper.
 Home-page: https://github.com/collabora/WhisperLive
 Author: Collabora Ltd
 Author-email: vineet.suryan@collabora.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `whisper-live-0.0.3/README.md` & `whisper-live-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.3/setup.py` & `whisper-live-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(name="whisper-live",
-      version="0.0.3",
+      version="0.0.4",
       description="A nearly-live implementation of OpenAI's Whisper.",
       long_description=README,
       long_description_content_type="text/markdown",
       include_package_data=True,
       url="https://github.com/collabora/WhisperLive",
       author="Collabora Ltd",
       author_email="vineet.suryan@collabora.com",
```

### Comparing `whisper-live-0.0.3/whisper_live/client.py` & `whisper-live-0.0.4/whisper_live/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,15 @@
 
     @staticmethod
     def on_error(ws, error):
         print(error)
 
     @staticmethod
     def on_close(ws, close_status_code, close_msg):
-        print(f"### {ws} websocket connection closed with status: \
-              {close_status_code} and msg: {close_msg} ###")
+        print(f"[INFO]: Websocket connection closed.")
 
     @staticmethod
     def on_open(ws):
         print(Client.multilingual, Client.language, Client.task)
 
         print("[INFO]: Opened connection")
         ws.send(json.dumps({
@@ -176,28 +175,26 @@
 
         except KeyboardInterrupt:
             self.wf.close()
             self.stream.stop_stream()
             self.stream.close()
             self.p.terminate()
             self.close_websocket()
-            print("Keyboard interrupt.")
+            print("[INFO]: Keyboard interrupt.")
 
     def close_websocket(self):
         try:
             self.client_socket.close()  # Close the WebSocket connection
         except Exception as e:
-            print("[Error]: Error closing WebSocket:", e)
+            print("[ERROR]: Error closing WebSocket:", e)
 
         try:
             self.ws_thread.join()  # Wait for the WebSocket thread to finish
         except Exception as e:
-            print("[Error:] Error joining WebSocket thread:", e)
-
-        print("WebSocket and thread closed.")
+            print("[ERROR:] Error joining WebSocket thread:", e)
 
     def get_client_socket(self):
         return self.client_socket
     
     def write_audio_frames_to_file(self, frames, file_name):
         wf = wave.open(file_name, 'wb')
         wf.setnchannels(self.CHANNELS)
```

### Comparing `whisper-live-0.0.3/whisper_live/server.py` & `whisper-live-0.0.4/whisper_live/server.py`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.3/whisper_live/transcriber.py` & `whisper-live-0.0.4/whisper_live/transcriber.py`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.3/whisper_live.egg-info/PKG-INFO` & `whisper-live-0.0.4/whisper_live.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-live
-Version: 0.0.3
+Version: 0.0.4
 Summary: A nearly-live implementation of OpenAI's Whisper.
 Home-page: https://github.com/collabora/WhisperLive
 Author: Collabora Ltd
 Author-email: vineet.suryan@collabora.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

