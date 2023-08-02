# Comparing `tmp/whisper-live-0.0.2.tar.gz` & `tmp/whisper-live-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-live-0.0.2.tar", last modified: Wed Aug  2 07:56:47 2023, max compression
+gzip compressed data, was "whisper-live-0.0.3.tar", last modified: Wed Aug  2 08:01:08 2023, max compression
```

## Comparing `whisper-live-0.0.2.tar` & `whisper-live-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 07:56:47.682006 whisper-live-0.0.2/
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     1085 2023-07-10 09:30:36.000000 whisper-live-0.0.2/LICENSE
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     4320 2023-08-02 07:56:47.682006 whisper-live-0.0.2/PKG-INFO
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     3862 2023-08-02 07:50:34.000000 whisper-live-0.0.2/README.md
--rw-rw-r--   0 vineet    (1000) vineet    (1000)       38 2023-08-02 07:56:47.682006 whisper-live-0.0.2/setup.cfg
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     1316 2023-08-02 07:54:52.000000 whisper-live-0.0.2/setup.py
-drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 07:56:47.682006 whisper-live-0.0.2/whisper_live/
--rw-rw-r--   0 vineet    (1000) vineet    (1000)        0 2023-07-31 14:05:43.000000 whisper-live-0.0.2/whisper_live/__init__.py
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     9412 2023-08-01 19:51:31.000000 whisper-live-0.0.2/whisper_live/client.py
--rw-rw-r--   0 vineet    (1000) vineet    (1000)    12020 2023-08-02 04:39:17.000000 whisper-live-0.0.2/whisper_live/server.py
--rw-rw-r--   0 vineet    (1000) vineet    (1000)    32804 2023-07-31 14:00:59.000000 whisper-live-0.0.2/whisper_live/transcriber.py
-drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 07:56:47.682006 whisper-live-0.0.2/whisper_live.egg-info/
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     4320 2023-08-02 07:56:47.000000 whisper-live-0.0.2/whisper_live.egg-info/PKG-INFO
--rw-rw-r--   0 vineet    (1000) vineet    (1000)      304 2023-08-02 07:56:47.000000 whisper-live-0.0.2/whisper_live.egg-info/SOURCES.txt
--rw-rw-r--   0 vineet    (1000) vineet    (1000)        1 2023-08-02 07:56:47.000000 whisper-live-0.0.2/whisper_live.egg-info/dependency_links.txt
--rw-rw-r--   0 vineet    (1000) vineet    (1000)      107 2023-08-02 07:56:47.000000 whisper-live-0.0.2/whisper_live.egg-info/requires.txt
--rw-rw-r--   0 vineet    (1000) vineet    (1000)       13 2023-08-02 07:56:47.000000 whisper-live-0.0.2/whisper_live.egg-info/top_level.txt
+drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 08:01:08.449278 whisper-live-0.0.3/
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     1085 2023-07-10 09:30:36.000000 whisper-live-0.0.3/LICENSE
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     4306 2023-08-02 08:01:08.449278 whisper-live-0.0.3/PKG-INFO
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     3848 2023-08-02 08:00:41.000000 whisper-live-0.0.3/README.md
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)       38 2023-08-02 08:01:08.449278 whisper-live-0.0.3/setup.cfg
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     1316 2023-08-02 08:00:56.000000 whisper-live-0.0.3/setup.py
+drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 08:01:08.449278 whisper-live-0.0.3/whisper_live/
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)        0 2023-07-31 14:05:43.000000 whisper-live-0.0.3/whisper_live/__init__.py
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     9412 2023-08-01 19:51:31.000000 whisper-live-0.0.3/whisper_live/client.py
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)    11926 2023-08-02 08:00:21.000000 whisper-live-0.0.3/whisper_live/server.py
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)    32804 2023-07-31 14:00:59.000000 whisper-live-0.0.3/whisper_live/transcriber.py
+drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 08:01:08.449278 whisper-live-0.0.3/whisper_live.egg-info/
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     4306 2023-08-02 08:01:08.000000 whisper-live-0.0.3/whisper_live.egg-info/PKG-INFO
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)      304 2023-08-02 08:01:08.000000 whisper-live-0.0.3/whisper_live.egg-info/SOURCES.txt
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)        1 2023-08-02 08:01:08.000000 whisper-live-0.0.3/whisper_live.egg-info/dependency_links.txt
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)      107 2023-08-02 08:01:08.000000 whisper-live-0.0.3/whisper_live.egg-info/requires.txt
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)       13 2023-08-02 08:01:08.000000 whisper-live-0.0.3/whisper_live.egg-info/top_level.txt
```

### Comparing `whisper-live-0.0.2/LICENSE` & `whisper-live-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.2/PKG-INFO` & `whisper-live-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-live
-Version: 0.0.2
+Version: 0.0.3
 Summary: A nearly-live implementation of OpenAI's Whisper.
 Home-page: https://github.com/collabora/WhisperLive
 Author: Collabora Ltd
 Author-email: vineet.suryan@collabora.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -31,15 +31,15 @@
 ```
 
 ## Getting Started
 - Run the server
 ```python
  from whisper_live.server import TranscriptionServer
  server = TranscriptionServer()
- server.run_server("0.0.0.0", 9090)
+ server.run("0.0.0.0", 9090)
 ```
 
 - On the client side
     - To transcribe an audio file:
     ```python
       from whisper_live.client import TranscriptionClient
       client = TranscriptionClient("localhost", 9090, multilingual=True, language="hi", translate=True)
@@ -57,15 +57,15 @@
 
 
 ## Transcribe audio from browser
 - Run the server
 ```python
  from whisper_live.server import TranscriptionServer
  server = TranscriptionServer()
- server.run_server("0.0.0.0", 9090)
+ server.run("0.0.0.0", 9090)
 ```
 This would start the websocket server on port ```9090```.
 
 ### Chrome Extension
 - Refer to [Audio-Transcription-Chrome](https://github.com/collabora/whisper-live/tree/main/Audio-Transcription-Chrome#readme) to use Chrome extension.
 
 ### Firefox Extension
```

### Comparing `whisper-live-0.0.2/README.md` & `whisper-live-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```
 
 ## Getting Started
 - Run the server
 ```python
  from whisper_live.server import TranscriptionServer
  server = TranscriptionServer()
- server.run_server("0.0.0.0", 9090)
+ server.run("0.0.0.0", 9090)
 ```
 
 - On the client side
     - To transcribe an audio file:
     ```python
       from whisper_live.client import TranscriptionClient
       client = TranscriptionClient("localhost", 9090, multilingual=True, language="hi", translate=True)
@@ -43,15 +43,15 @@
 
 
 ## Transcribe audio from browser
 - Run the server
 ```python
  from whisper_live.server import TranscriptionServer
  server = TranscriptionServer()
- server.run_server("0.0.0.0", 9090)
+ server.run("0.0.0.0", 9090)
 ```
 This would start the websocket server on port ```9090```.
 
 ### Chrome Extension
 - Refer to [Audio-Transcription-Chrome](https://github.com/collabora/whisper-live/tree/main/Audio-Transcription-Chrome#readme) to use Chrome extension.
 
 ### Firefox Extension
```

### Comparing `whisper-live-0.0.2/setup.py` & `whisper-live-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(name="whisper-live",
-      version="0.0.2",
+      version="0.0.3",
       description="A nearly-live implementation of OpenAI's Whisper.",
       long_description=README,
       long_description_content_type="text/markdown",
       include_package_data=True,
       url="https://github.com/collabora/WhisperLive",
       author="Collabora Ltd",
       author_email="vineet.suryan@collabora.com",
```

### Comparing `whisper-live-0.0.2/whisper_live/client.py` & `whisper-live-0.0.3/whisper_live/client.py`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.2/whisper_live/server.py` & `whisper-live-0.0.3/whisper_live/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,10 +321,7 @@
         return last_segment
     
     def cleanup(self):
         logging.info("Cleaning up.")
         self.exit = True
         self.transcriber.destroy()
 
-if __name__ == "__main__":
-    server = TranscriptionServer()
-    server.run("0.0.0.0", 9090)
```

### Comparing `whisper-live-0.0.2/whisper_live/transcriber.py` & `whisper-live-0.0.3/whisper_live/transcriber.py`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.2/whisper_live.egg-info/PKG-INFO` & `whisper-live-0.0.3/whisper_live.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-live
-Version: 0.0.2
+Version: 0.0.3
 Summary: A nearly-live implementation of OpenAI's Whisper.
 Home-page: https://github.com/collabora/WhisperLive
 Author: Collabora Ltd
 Author-email: vineet.suryan@collabora.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -31,15 +31,15 @@
 ```
 
 ## Getting Started
 - Run the server
 ```python
  from whisper_live.server import TranscriptionServer
  server = TranscriptionServer()
- server.run_server("0.0.0.0", 9090)
+ server.run("0.0.0.0", 9090)
 ```
 
 - On the client side
     - To transcribe an audio file:
     ```python
       from whisper_live.client import TranscriptionClient
       client = TranscriptionClient("localhost", 9090, multilingual=True, language="hi", translate=True)
@@ -57,15 +57,15 @@
 
 
 ## Transcribe audio from browser
 - Run the server
 ```python
  from whisper_live.server import TranscriptionServer
  server = TranscriptionServer()
- server.run_server("0.0.0.0", 9090)
+ server.run("0.0.0.0", 9090)
 ```
 This would start the websocket server on port ```9090```.
 
 ### Chrome Extension
 - Refer to [Audio-Transcription-Chrome](https://github.com/collabora/whisper-live/tree/main/Audio-Transcription-Chrome#readme) to use Chrome extension.
 
 ### Firefox Extension
```

