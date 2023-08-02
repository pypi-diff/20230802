# Comparing `tmp/whisper-live-0.0.1.tar.gz` & `tmp/whisper-live-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-live-0.0.1.tar", last modified: Wed Aug  2 07:51:04 2023, max compression
+gzip compressed data, was "whisper-live-0.0.2.tar", last modified: Wed Aug  2 07:56:47 2023, max compression
```

## Comparing `whisper-live-0.0.1.tar` & `whisper-live-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 07:51:04.141698 whisper-live-0.0.1/
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     1085 2023-07-10 09:30:36.000000 whisper-live-0.0.1/LICENSE
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     4317 2023-08-02 07:51:04.141698 whisper-live-0.0.1/PKG-INFO
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     3862 2023-08-02 07:50:34.000000 whisper-live-0.0.1/README.md
--rw-rw-r--   0 vineet    (1000) vineet    (1000)       38 2023-08-02 07:51:04.141698 whisper-live-0.0.1/setup.cfg
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     1313 2023-08-02 07:49:43.000000 whisper-live-0.0.1/setup.py
-drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 07:51:04.141698 whisper-live-0.0.1/whisper_live/
--rw-rw-r--   0 vineet    (1000) vineet    (1000)        0 2023-07-31 14:05:43.000000 whisper-live-0.0.1/whisper_live/__init__.py
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     9412 2023-08-01 19:51:31.000000 whisper-live-0.0.1/whisper_live/client.py
--rw-rw-r--   0 vineet    (1000) vineet    (1000)    12020 2023-08-02 04:39:17.000000 whisper-live-0.0.1/whisper_live/server.py
--rw-rw-r--   0 vineet    (1000) vineet    (1000)    32804 2023-07-31 14:00:59.000000 whisper-live-0.0.1/whisper_live/transcriber.py
-drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 07:51:04.141698 whisper-live-0.0.1/whisper_live.egg-info/
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     4317 2023-08-02 07:51:04.000000 whisper-live-0.0.1/whisper_live.egg-info/PKG-INFO
--rw-rw-r--   0 vineet    (1000) vineet    (1000)      304 2023-08-02 07:51:04.000000 whisper-live-0.0.1/whisper_live.egg-info/SOURCES.txt
--rw-rw-r--   0 vineet    (1000) vineet    (1000)        1 2023-08-02 07:51:04.000000 whisper-live-0.0.1/whisper_live.egg-info/dependency_links.txt
--rw-rw-r--   0 vineet    (1000) vineet    (1000)      107 2023-08-02 07:51:04.000000 whisper-live-0.0.1/whisper_live.egg-info/requires.txt
--rw-rw-r--   0 vineet    (1000) vineet    (1000)       13 2023-08-02 07:51:04.000000 whisper-live-0.0.1/whisper_live.egg-info/top_level.txt
+drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 07:56:47.682006 whisper-live-0.0.2/
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     1085 2023-07-10 09:30:36.000000 whisper-live-0.0.2/LICENSE
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     4320 2023-08-02 07:56:47.682006 whisper-live-0.0.2/PKG-INFO
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     3862 2023-08-02 07:50:34.000000 whisper-live-0.0.2/README.md
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)       38 2023-08-02 07:56:47.682006 whisper-live-0.0.2/setup.cfg
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     1316 2023-08-02 07:54:52.000000 whisper-live-0.0.2/setup.py
+drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 07:56:47.682006 whisper-live-0.0.2/whisper_live/
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)        0 2023-07-31 14:05:43.000000 whisper-live-0.0.2/whisper_live/__init__.py
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     9412 2023-08-01 19:51:31.000000 whisper-live-0.0.2/whisper_live/client.py
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)    12020 2023-08-02 04:39:17.000000 whisper-live-0.0.2/whisper_live/server.py
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)    32804 2023-07-31 14:00:59.000000 whisper-live-0.0.2/whisper_live/transcriber.py
+drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 07:56:47.682006 whisper-live-0.0.2/whisper_live.egg-info/
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     4320 2023-08-02 07:56:47.000000 whisper-live-0.0.2/whisper_live.egg-info/PKG-INFO
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)      304 2023-08-02 07:56:47.000000 whisper-live-0.0.2/whisper_live.egg-info/SOURCES.txt
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)        1 2023-08-02 07:56:47.000000 whisper-live-0.0.2/whisper_live.egg-info/dependency_links.txt
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)      107 2023-08-02 07:56:47.000000 whisper-live-0.0.2/whisper_live.egg-info/requires.txt
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)       13 2023-08-02 07:56:47.000000 whisper-live-0.0.2/whisper_live.egg-info/top_level.txt
```

### Comparing `whisper-live-0.0.1/LICENSE` & `whisper-live-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.1/PKG-INFO` & `whisper-live-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: whisper-live
-Version: 0.0.1
+Version: 0.0.2
 Summary: A nearly-live implementation of OpenAI's Whisper.
 Home-page: https://github.com/collabora/WhisperLive
-Author: makaveli10
+Author: Collabora Ltd
 Author-email: vineet.suryan@collabora.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `whisper-live-0.0.1/README.md` & `whisper-live-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.1/setup.py` & `whisper-live-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(name="whisper-live",
-      version="0.0.1",
+      version="0.0.2",
       description="A nearly-live implementation of OpenAI's Whisper.",
       long_description=README,
       long_description_content_type="text/markdown",
       include_package_data=True,
       url="https://github.com/collabora/WhisperLive",
-      author="makaveli10",
+      author="Collabora Ltd",
       author_email="vineet.suryan@collabora.com",
       license="MIT",
       classifiers=[
           "License :: OSI Approved :: MIT License",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
       ],
@@ -29,15 +29,15 @@
                  "Audio-Transcription-Firefox",
                  "requirements",
                  "whisper-finetuning"
                 )
       ),
       install_requires=[
         "PyAudio",
-        "faster-whisper==0.0.6",
+        "faster-whisper==0.6.0",
         "torch",
         "torchaudio",
         "websockets",
         "onnxruntime",
         "ffmpeg-python",
         "scipy",
         "websocket-client",
```

### Comparing `whisper-live-0.0.1/whisper_live/client.py` & `whisper-live-0.0.2/whisper_live/client.py`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.1/whisper_live/server.py` & `whisper-live-0.0.2/whisper_live/server.py`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.1/whisper_live/transcriber.py` & `whisper-live-0.0.2/whisper_live/transcriber.py`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.1/whisper_live.egg-info/PKG-INFO` & `whisper-live-0.0.2/whisper_live.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: whisper-live
-Version: 0.0.1
+Version: 0.0.2
 Summary: A nearly-live implementation of OpenAI's Whisper.
 Home-page: https://github.com/collabora/WhisperLive
-Author: makaveli10
+Author: Collabora Ltd
 Author-email: vineet.suryan@collabora.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

