# Comparing `tmp/open_interpreter-0.0.243.tar.gz` & `tmp/open_interpreter-0.0.244.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.243.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.244.tar", max compression
```

## Comparing `open_interpreter-0.0.243.tar` & `open_interpreter-0.0.244.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.243/LICENSE
--rw-r--r--   0        0        0     6233 2023-07-30 18:09:16.115763 open_interpreter-0.0.243/README.md
--rw-r--r--   0        0        0      695 2023-07-30 17:49:07.642871 open_interpreter-0.0.243/cli/__init__.py
--rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.243/interpreter/__init__.py
--rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.243/interpreter/exec.py
--rw-r--r--   0        0        0     9018 2023-07-30 19:07:02.203175 open_interpreter-0.0.243/interpreter/interpreter.py
--rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.243/interpreter/json_utils.py
--rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.243/interpreter/openai_utils.py
--rw-r--r--   0        0        0     2773 2023-08-01 22:33:54.346866 open_interpreter-0.0.243/interpreter/system_message.txt
--rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.243/interpreter/view.py
--rw-r--r--   0        0        0      578 2023-08-01 22:34:35.526155 open_interpreter-0.0.243/pyproject.toml
--rw-r--r--   0        0        0     6857 1970-01-01 00:00:00.000000 open_interpreter-0.0.243/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.244/LICENSE
+-rw-r--r--   0        0        0     6233 2023-07-30 18:09:16.115763 open_interpreter-0.0.244/README.md
+-rw-r--r--   0        0        0      695 2023-07-30 17:49:07.642871 open_interpreter-0.0.244/cli/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.244/interpreter/__init__.py
+-rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.244/interpreter/exec.py
+-rw-r--r--   0        0        0     9018 2023-07-30 19:07:02.203175 open_interpreter-0.0.244/interpreter/interpreter.py
+-rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.244/interpreter/json_utils.py
+-rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.244/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     2977 2023-08-01 22:42:16.182950 open_interpreter-0.0.244/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.244/interpreter/view.py
+-rw-r--r--   0        0        0      578 2023-08-01 22:42:29.860043 open_interpreter-0.0.244/pyproject.toml
+-rw-r--r--   0        0        0     6857 1970-01-01 00:00:00.000000 open_interpreter-0.0.244/PKG-INFO
```

### Comparing `open_interpreter-0.0.243/LICENSE` & `open_interpreter-0.0.244/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.243/README.md` & `open_interpreter-0.0.244/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.243/cli/__init__.py` & `open_interpreter-0.0.244/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.243/interpreter/exec.py` & `open_interpreter-0.0.244/interpreter/exec.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.243/interpreter/interpreter.py` & `open_interpreter-0.0.244/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.243/interpreter/json_utils.py` & `open_interpreter-0.0.244/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.243/interpreter/openai_utils.py` & `open_interpreter-0.0.244/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.243/interpreter/system_message.txt` & `open_interpreter-0.0.244/interpreter/system_message.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 When a user refers to a filename, they're likely referring to an existing file in the directory you're currently in (run_code executes on the user's machine).
 
 When using `for` or `while` loops, always include a status message like `print(f'{i}/{total}')`. Even for short loops, this is critical.
 
 Write messages to the user in Markdown.
 
+In general, try to make plans with as few steps as possible. Just write code that should generally work, then make sure it did. In general we want to run as few code blocks per user request as possible.
+
 Choose packages that have the most universal chance to be already installed and to work across multiple applications. Things like ffmpeg, pandoc, that are well-supported, famous, and powerful.
 
 [Preferred Packages]
 Audio effects: `pedalboard`
 YouTube downloading: `yt-dlp`
 Video: `ffmpeg`
 OS actions like reading emails, opening files: (If Mac user) Write Applescript in a multiline string then use `subprocess` to run it.
```

### Comparing `open_interpreter-0.0.243/interpreter/view.py` & `open_interpreter-0.0.244/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.243/pyproject.toml` & `open_interpreter-0.0.244/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
     {include = "cli"}
 ]
-version = "0.0.243"
+version = "0.0.244"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.243/PKG-INFO` & `open_interpreter-0.0.244/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.243
+Version: 0.0.244
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

