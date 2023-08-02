# Comparing `tmp/lsstream-1.0.0.tar.gz` & `tmp/lsstream-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsstream-1.0.0.tar", last modified: Sat Jul 22 17:03:19 2023, max compression
+gzip compressed data, was "lsstream-1.1.2.tar", last modified: Wed Aug  2 19:32:30 2023, max compression
```

## Comparing `lsstream-1.0.0.tar` & `lsstream-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:03:19.901510 lsstream-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-22 17:03:08.000000 lsstream-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-22 17:03:19.901510 lsstream-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-22 17:03:08.000000 lsstream-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-22 17:03:08.000000 lsstream-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 17:03:19.901510 lsstream-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:03:19.901510 lsstream-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:03:19.901510 lsstream-1.0.0/src/lsstream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 17:03:08.000000 lsstream-1.0.0/src/lsstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-22 17:03:08.000000 lsstream-1.0.0/src/lsstream/file_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-22 17:03:08.000000 lsstream-1.0.0/src/lsstream/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-22 17:03:08.000000 lsstream-1.0.0/src/lsstream/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-22 17:03:08.000000 lsstream-1.0.0/src/lsstream/style.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-22 17:03:08.000000 lsstream-1.0.0/src/lsstream/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-22 17:03:08.000000 lsstream-1.0.0/src/lsstream/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:03:19.901510 lsstream-1.0.0/src/lsstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-22 17:03:19.000000 lsstream-1.0.0/src/lsstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-22 17:03:19.000000 lsstream-1.0.0/src/lsstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 17:03:19.000000 lsstream-1.0.0/src/lsstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-22 17:03:19.000000 lsstream-1.0.0/src/lsstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 17:03:19.000000 lsstream-1.0.0/src/lsstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:32:30.343445 lsstream-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-02 19:32:20.000000 lsstream-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-02 19:32:30.343445 lsstream-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-02 19:32:20.000000 lsstream-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-02 19:32:20.000000 lsstream-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:32:30.343445 lsstream-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:32:30.343445 lsstream-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:32:30.343445 lsstream-1.1.2/src/lsstream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:32:20.000000 lsstream-1.1.2/src/lsstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-02 19:32:20.000000 lsstream-1.1.2/src/lsstream/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-02 19:32:20.000000 lsstream-1.1.2/src/lsstream/file_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-02 19:32:20.000000 lsstream-1.1.2/src/lsstream/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-08-02 19:32:20.000000 lsstream-1.1.2/src/lsstream/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-02 19:32:20.000000 lsstream-1.1.2/src/lsstream/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 19:32:20.000000 lsstream-1.1.2/src/lsstream/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:32:30.343445 lsstream-1.1.2/src/lsstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-02 19:32:30.000000 lsstream-1.1.2/src/lsstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-02 19:32:30.000000 lsstream-1.1.2/src/lsstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:32:30.000000 lsstream-1.1.2/src/lsstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:32:30.000000 lsstream-1.1.2/src/lsstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 19:32:30.000000 lsstream-1.1.2/src/lsstream.egg-info/top_level.txt
```

### Comparing `lsstream-1.0.0/LICENSE` & `lsstream-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lsstream-1.0.0/pyproject.toml` & `lsstream-1.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lsstream"
-version = "1.0.0"
+version = "1.1.2"
 authors = [
   { name="Wermutton", email="redacted@redacted.redacted" },
 ]
 description = "To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   "pyfiglet",
+  "pyperclip",
   "termcolor",
   "colorama"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `lsstream-1.0.0/src/lsstream/main.py` & `lsstream-1.1.2/src/lsstream/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import webbrowser
-from .style import intro, color
-from .file_generation import create_content
-from .prompts import prompt_test_html
-from .test import test_html
+from style import intro, color
+from file_generation import create_content
+from prompts import prompt_test_html
+from test import test_html, open_canvas_test_page
 
 # Delete current batch of html files
 def end_session(new_files, new_contents):
     end_prompt = input(color('\nAre you done with this session? (Y/N): ', 'white'))
     if end_prompt.lower() == 'y':
         if os.path.exists('temp.html'):
             os.remove('temp.html')
@@ -44,15 +44,16 @@
                 break
             else:
                 print(color('\nInvalid option, please choose A, B, or C.', 'red'))
 
 def lsstream():    
     new_files, new_contents = create_content()
 
-    if prompt_test_html(new_contents): test_html(new_contents)
+    # if prompt_test_html(new_contents): test_html(new_contents)
+    if prompt_test_html(): open_canvas_test_page()
 
     end_session(new_files, new_contents) 
 
 
 def main():
     print(color(intro.renderText('LSSTREAM'), 'green'))
     lsstream()
```

