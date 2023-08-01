# Comparing `tmp/open_interpreter-0.0.242.tar.gz` & `tmp/open_interpreter-0.0.243.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.242.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.243.tar", max compression
```

## Comparing `open_interpreter-0.0.242.tar` & `open_interpreter-0.0.243.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.242/LICENSE
--rw-r--r--   0        0        0     6230 2023-07-30 17:46:07.554643 open_interpreter-0.0.242/README.md
--rw-r--r--   0        0        0      695 2023-07-30 17:49:07.642871 open_interpreter-0.0.242/cli/__init__.py
--rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.242/interpreter/__init__.py
--rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.242/interpreter/exec.py
--rw-r--r--   0        0        0     9021 2023-07-26 02:25:34.682450 open_interpreter-0.0.242/interpreter/interpreter.py
--rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.242/interpreter/json_utils.py
--rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.242/interpreter/openai_utils.py
--rw-r--r--   0        0        0     2539 2023-07-30 17:17:18.374017 open_interpreter-0.0.242/interpreter/system_message.txt
--rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.242/interpreter/view.py
--rw-r--r--   0        0        0      578 2023-07-30 17:49:44.394183 open_interpreter-0.0.242/pyproject.toml
--rw-r--r--   0        0        0     6854 1970-01-01 00:00:00.000000 open_interpreter-0.0.242/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.243/LICENSE
+-rw-r--r--   0        0        0     6233 2023-07-30 18:09:16.115763 open_interpreter-0.0.243/README.md
+-rw-r--r--   0        0        0      695 2023-07-30 17:49:07.642871 open_interpreter-0.0.243/cli/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.243/interpreter/__init__.py
+-rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.243/interpreter/exec.py
+-rw-r--r--   0        0        0     9018 2023-07-30 19:07:02.203175 open_interpreter-0.0.243/interpreter/interpreter.py
+-rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.243/interpreter/json_utils.py
+-rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.243/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     2773 2023-08-01 22:33:54.346866 open_interpreter-0.0.243/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.243/interpreter/view.py
+-rw-r--r--   0        0        0      578 2023-08-01 22:34:35.526155 open_interpreter-0.0.243/pyproject.toml
+-rw-r--r--   0        0        0     6857 1970-01-01 00:00:00.000000 open_interpreter-0.0.243/PKG-INFO
```

### Comparing `open_interpreter-0.0.242/LICENSE` & `open_interpreter-0.0.243/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.242/README.md` & `open_interpreter-0.0.243/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 ```
 
 ### Python
 
 ```python
 import interpreter
 
-interpreter.api_key = "<openai_api_key>"
+interpreter.api_key = "your_openai_api_key"
 interpreter.chat() # Starts an interactive chat
 ```
 
 ## Comparison to ChatGPT's Code Interpreter
 
 OpenAI's recent release of [Code Interpreter](https://openai.com/blog/chatgpt-plugins#code-interpreter) with GPT-4 presents a fantastic opportunity to accomplish real-world tasks with ChatGPT.
```

### Comparing `open_interpreter-0.0.242/cli/__init__.py` & `open_interpreter-0.0.243/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.242/interpreter/exec.py` & `open_interpreter-0.0.243/interpreter/exec.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.242/interpreter/interpreter.py` & `open_interpreter-0.0.243/interpreter/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,15 @@
             function_args["forbidden_commands"] = self.forbidden_commands
 
           user_declined = False
           
           if self.no_confirm == False:
             # Ask the user for confirmation
             print()
-            response = input("Would you like to run the above code? (y/n) ")
+            response = input("  Would you like to run this code? (y/n) ")
             print()
             if response.lower().strip() != "y":
               user_declined = True
             else:
               user_declined = False
 
           if user_declined:
```

### Comparing `open_interpreter-0.0.242/interpreter/json_utils.py` & `open_interpreter-0.0.243/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.242/interpreter/openai_utils.py` & `open_interpreter-0.0.243/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.242/interpreter/system_message.txt` & `open_interpreter-0.0.243/interpreter/system_message.txt`

 * *Files 14% similar despite different names*

```diff
@@ -16,19 +16,22 @@
 
 When a user refers to a filename, they're likely referring to an existing file in the directory you're currently in (run_code executes on the user's machine).
 
 When using `for` or `while` loops, always include a status message like `print(f'{i}/{total}')`. Even for short loops, this is critical.
 
 Write messages to the user in Markdown.
 
+Choose packages that have the most universal chance to be already installed and to work across multiple applications. Things like ffmpeg, pandoc, that are well-supported, famous, and powerful.
+
 [Preferred Packages]
 Audio effects: `pedalboard`
 YouTube downloading: `yt-dlp`
 Video: `ffmpeg`
-OS actions like reading emails, opening files: Write Applescript in a multiline string then use `subprocess` to run it.
+OS actions like reading emails, opening files: (If Mac user) Write Applescript in a multiline string then use `subprocess` to run it.
+File conversion: `pandoc`
 
 [Traceback Protocol]
 If you encounter an error, do not try to use an alternative method yet. Instead:
 
 **Write a message to the user explaining what happened and theorizing why. Do not try to run_code immediatly after run_code has errored.**
 
 If a solution is apparent (and is not simply changing methods / using a new package) attempt it.
```

### Comparing `open_interpreter-0.0.242/interpreter/view.py` & `open_interpreter-0.0.243/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.242/pyproject.toml` & `open_interpreter-0.0.243/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
     {include = "cli"}
 ]
-version = "0.0.242"
+version = "0.0.243"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.242/PKG-INFO` & `open_interpreter-0.0.243/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.242
+Version: 0.0.243
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -72,15 +72,15 @@
 ```
 
 ### Python
 
 ```python
 import interpreter
 
-interpreter.api_key = "<openai_api_key>"
+interpreter.api_key = "your_openai_api_key"
 interpreter.chat() # Starts an interactive chat
 ```
 
 ## Comparison to ChatGPT's Code Interpreter
 
 OpenAI's recent release of [Code Interpreter](https://openai.com/blog/chatgpt-plugins#code-interpreter) with GPT-4 presents a fantastic opportunity to accomplish real-world tasks with ChatGPT.
```

