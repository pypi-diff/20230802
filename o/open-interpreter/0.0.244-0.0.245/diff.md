# Comparing `tmp/open_interpreter-0.0.244.tar.gz` & `tmp/open_interpreter-0.0.245.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.244.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.245.tar", max compression
```

## Comparing `open_interpreter-0.0.244.tar` & `open_interpreter-0.0.245.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.244/LICENSE
--rw-r--r--   0        0        0     6233 2023-07-30 18:09:16.115763 open_interpreter-0.0.244/README.md
--rw-r--r--   0        0        0      695 2023-07-30 17:49:07.642871 open_interpreter-0.0.244/cli/__init__.py
--rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.244/interpreter/__init__.py
--rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.244/interpreter/exec.py
--rw-r--r--   0        0        0     9018 2023-07-30 19:07:02.203175 open_interpreter-0.0.244/interpreter/interpreter.py
--rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.244/interpreter/json_utils.py
--rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.244/interpreter/openai_utils.py
--rw-r--r--   0        0        0     2977 2023-08-01 22:42:16.182950 open_interpreter-0.0.244/interpreter/system_message.txt
--rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.244/interpreter/view.py
--rw-r--r--   0        0        0      578 2023-08-01 22:42:29.860043 open_interpreter-0.0.244/pyproject.toml
--rw-r--r--   0        0        0     6857 1970-01-01 00:00:00.000000 open_interpreter-0.0.244/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.245/LICENSE
+-rw-r--r--   0        0        0     6396 2023-08-02 00:13:19.900301 open_interpreter-0.0.245/README.md
+-rw-r--r--   0        0        0      695 2023-07-30 17:49:07.642871 open_interpreter-0.0.245/cli/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.245/interpreter/__init__.py
+-rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.245/interpreter/exec.py
+-rw-r--r--   0        0        0     9018 2023-07-30 19:07:02.203175 open_interpreter-0.0.245/interpreter/interpreter.py
+-rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.245/interpreter/json_utils.py
+-rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.245/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     3090 2023-08-02 00:14:15.256798 open_interpreter-0.0.245/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.245/interpreter/view.py
+-rw-r--r--   0        0        0      578 2023-08-02 00:14:33.072959 open_interpreter-0.0.245/pyproject.toml
+-rw-r--r--   0        0        0     7020 1970-01-01 00:00:00.000000 open_interpreter-0.0.245/PKG-INFO
```

### Comparing `open_interpreter-0.0.244/LICENSE` & `open_interpreter-0.0.245/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.244/README.md` & `open_interpreter-0.0.245/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Open Interpreter
 
 A minimal, open-source implementation of OpenAI's code interpreter.
 
 ![Interpreter Demo](https://github.com/KillianLucas/open-interpreter/assets/63927363/a1597f66-d298-4172-bc0b-35b36e1479eb)
 
+```shell
+pip install open-interpreter
+```
+```shell
+interpreter
+```
+
 ## What is this?
 
 <br>
 
 > Having access to a junior programmer working at the speed of your fingertips ... can make new workflows effortless and efficient, as well as open the benefits of programming to new audiences.
 >
 > — _OpenAI's Code Interpreter Release_
@@ -25,18 +32,20 @@
 
 **⚠️ Note: You'll be asked to approve any code before it's run.**
 
 <br>
 
 [How does this compare to OpenAI's code interpreter?](https://github.com/KillianLucas/open-interpreter#comparison-to-chatgpts-code-interpreter)<br>
 
-## Demo Notebook
+## Demos
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing)
 
+https://github.com/KillianLucas/open-interpreter/assets/63927363/bfd31800-3587-4d8e-91ac-195482860633
+
 ## Features
 
 - Generated code runs locally (with confirmation).
 - Interactive, streaming chat inside your terminal.
 - Uses `pip` and `apt-get` to extend itself.
 
 ## Quick Start
```

### Comparing `open_interpreter-0.0.244/cli/__init__.py` & `open_interpreter-0.0.245/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.244/interpreter/exec.py` & `open_interpreter-0.0.245/interpreter/exec.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.244/interpreter/interpreter.py` & `open_interpreter-0.0.245/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.244/interpreter/json_utils.py` & `open_interpreter-0.0.245/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.244/interpreter/openai_utils.py` & `open_interpreter-0.0.245/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.244/interpreter/system_message.txt` & `open_interpreter-0.0.245/interpreter/system_message.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 [Preferred Packages]
 Audio effects: `pedalboard`
 YouTube downloading: `yt-dlp`
 Video: `ffmpeg`
 OS actions like reading emails, opening files: (If Mac user) Write Applescript in a multiline string then use `subprocess` to run it.
 File conversion: `pandoc`
 
+Note: Selenium has been updated to no longer require webdriver_manager. Just use `driver = webdriver.Chrome()`.
+
 [Traceback Protocol]
 If you encounter an error, do not try to use an alternative method yet. Instead:
 
 **Write a message to the user explaining what happened and theorizing why. Do not try to run_code immediatly after run_code has errored.**
 
 If a solution is apparent (and is not simply changing methods / using a new package) attempt it.
 If not, list these steps in a message to the user, then follow them one-by-one:
```

### Comparing `open_interpreter-0.0.244/interpreter/view.py` & `open_interpreter-0.0.245/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.244/pyproject.toml` & `open_interpreter-0.0.245/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
     {include = "cli"}
 ]
-version = "0.0.244"
+version = "0.0.245"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.244/PKG-INFO` & `open_interpreter-0.0.245/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.244
+Version: 0.0.245
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -18,14 +18,21 @@
 
 # Open Interpreter
 
 A minimal, open-source implementation of OpenAI's code interpreter.
 
 ![Interpreter Demo](https://github.com/KillianLucas/open-interpreter/assets/63927363/a1597f66-d298-4172-bc0b-35b36e1479eb)
 
+```shell
+pip install open-interpreter
+```
+```shell
+interpreter
+```
+
 ## What is this?
 
 <br>
 
 > Having access to a junior programmer working at the speed of your fingertips ... can make new workflows effortless and efficient, as well as open the benefits of programming to new audiences.
 >
 > — _OpenAI's Code Interpreter Release_
@@ -43,18 +50,20 @@
 
 **⚠️ Note: You'll be asked to approve any code before it's run.**
 
 <br>
 
 [How does this compare to OpenAI's code interpreter?](https://github.com/KillianLucas/open-interpreter#comparison-to-chatgpts-code-interpreter)<br>
 
-## Demo Notebook
+## Demos
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing)
 
+https://github.com/KillianLucas/open-interpreter/assets/63927363/bfd31800-3587-4d8e-91ac-195482860633
+
 ## Features
 
 - Generated code runs locally (with confirmation).
 - Interactive, streaming chat inside your terminal.
 - Uses `pip` and `apt-get` to extend itself.
 
 ## Quick Start
```

