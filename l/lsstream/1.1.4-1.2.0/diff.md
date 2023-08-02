# Comparing `tmp/lsstream-1.1.4.tar.gz` & `tmp/lsstream-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsstream-1.1.4.tar", last modified: Wed Aug  2 19:44:29 2023, max compression
+gzip compressed data, was "lsstream-1.2.0.tar", last modified: Wed Aug  2 20:38:48 2023, max compression
```

## Comparing `lsstream-1.1.4.tar` & `lsstream-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:44:29.533567 lsstream-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-02 19:44:19.000000 lsstream-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-02 19:44:29.533567 lsstream-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-02 19:44:19.000000 lsstream-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-02 19:44:19.000000 lsstream-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:44:29.533567 lsstream-1.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:44:29.529567 lsstream-1.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:44:29.533567 lsstream-1.1.4/src/lsstream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/file_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/style.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-02 19:44:19.000000 lsstream-1.1.4/src/lsstream/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:44:29.533567 lsstream-1.1.4/src/lsstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-02 19:44:29.000000 lsstream-1.1.4/src/lsstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-02 19:44:29.000000 lsstream-1.1.4/src/lsstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:44:29.000000 lsstream-1.1.4/src/lsstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:44:29.000000 lsstream-1.1.4/src/lsstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 19:44:29.000000 lsstream-1.1.4/src/lsstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:38:48.107345 lsstream-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-02 20:38:38.000000 lsstream-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 20:38:48.107345 lsstream-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-02 20:38:38.000000 lsstream-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-02 20:38:38.000000 lsstream-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:38:48.107345 lsstream-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:38:48.107345 lsstream-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:38:48.107345 lsstream-1.2.0/src/lsstream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/file_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-02 20:38:38.000000 lsstream-1.2.0/src/lsstream/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:38:48.107345 lsstream-1.2.0/src/lsstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 20:38:48.000000 lsstream-1.2.0/src/lsstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-02 20:38:48.000000 lsstream-1.2.0/src/lsstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:38:48.000000 lsstream-1.2.0/src/lsstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:38:48.000000 lsstream-1.2.0/src/lsstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 20:38:48.000000 lsstream-1.2.0/src/lsstream.egg-info/top_level.txt
```

### Comparing `lsstream-1.1.4/LICENSE` & `lsstream-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lsstream-1.1.4/PKG-INFO` & `lsstream-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 1.1.4
+Version: 1.2.0
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,20 +30,32 @@
 
 Install the `lsstream` package via pip through your command line:
 
 ```bash
 > pip install lsstream
 ```
 
+or
+
+```bash
+> pip3 install lsstream
+```
+
 ## 🎯 Usage
 
 To run `lsstream`, type the following command in your command line:
 
 ```bash
-> python -m lsstream.main
+> python -m lsstream.run
+```
+
+or
+
+```bash
+> python3 -m lsstream.run
 ```
 
 Simply follow the on-screen prompts to streamline your streaming experience! :sparkles:
 
 ## 💡 Features
 
 - **Batch File Generation**: Generates multiple .txt files in a snap. Just input your media titles and links, and `lsstream` will use the correct template to create your files.
```

### Comparing `lsstream-1.1.4/README.md` & `lsstream-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,32 @@
 
 Install the `lsstream` package via pip through your command line:
 
 ```bash
 > pip install lsstream
 ```
 
+or
+
+```bash
+> pip3 install lsstream
+```
+
 ## 🎯 Usage
 
 To run `lsstream`, type the following command in your command line:
 
 ```bash
-> python -m lsstream.main
+> python -m lsstream.run
+```
+
+or
+
+```bash
+> python3 -m lsstream.run
 ```
 
 Simply follow the on-screen prompts to streamline your streaming experience! :sparkles:
 
 ## 💡 Features
 
 - **Batch File Generation**: Generates multiple .txt files in a snap. Just input your media titles and links, and `lsstream` will use the correct template to create your files.
```

### Comparing `lsstream-1.1.4/pyproject.toml` & `lsstream-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lsstream"
-version = "1.1.4"
+version = "1.2.0"
 authors = [
   { name="Wermutton", email="redacted@redacted.redacted" },
 ]
 description = "To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `lsstream-1.1.4/src/lsstream/file_generation.py` & `lsstream-1.2.0/src/lsstream/file_generation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 import os
 import pyperclip
-from .defaults import EMBED_TEMPLATE     # choose the template you want
+from .defaults import EMBED_TEMPLATE    
 from .style import color
 from .prompts import prompt_directory, prompt_details
 
 # Creates the files and returns its contents
 def create_file(movie_title, media_link, output_directory):
     output_file_path = os.path.join(output_directory, f'{movie_title}.txt')
     file_content = EMBED_TEMPLATE.format(LINK=media_link, TITLE=movie_title)
 
     with open(output_file_path, 'w') as f:
         f.write(file_content)
     
     return output_file_path, file_content 
 
-# Sets up the embed code and places it in user's clipboard
-def embed_clipboard(movie_title, media_link):
-    embed_content = EMBED_TEMPLATE.format(LINK=media_link, TITLE=movie_title)
-    
-    # Copy the file content to clipboard
-    pyperclip.copy(embed_content)
-
-    return f"✔ Embed code for \"{movie_title}\" successfully pasted to clipboard!"
-
-
 # Loop for file and content generation
 def create_content():
+    movie_titles = []
+    embed_contents = []
     new_contents = []
     new_files = []
+    count = 0
 
     output_directory = prompt_directory()
 
     while True:
         movie_title, media_link = prompt_details()
+        movie_titles.append(f'"{movie_title}"')
         new_file, new_content = create_file(movie_title, media_link, output_directory)  
-        print('\n', color(embed_clipboard(movie_title, media_link), 'green'))
+
+        embed_content = EMBED_TEMPLATE.format(LINK = media_link, TITLE = movie_title)
+        embed_contents.append(embed_content) 
 
         new_files.append(new_file)
         new_contents.append(new_content)  
 
         continue_prompt = input(color('\nContinue? (Y/N): ', 'white'))
         if continue_prompt.lower() != 'y':
+            print('\n', color(f"✔ Embed code(s) for {', '.join(movie_titles)} successfully pasted to clipboard!", 'green'))
             break
     
+    pyperclip.copy('\n'.join(embed_contents))
+    
     return new_files, new_contents
```

### Comparing `lsstream-1.1.4/src/lsstream/prompts.py` & `lsstream-1.2.0/src/lsstream/prompts.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.1.4/src/lsstream/run.py` & `lsstream-1.2.0/src/lsstream/run.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.1.4/src/lsstream.egg-info/PKG-INFO` & `lsstream-1.2.0/src/lsstream.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 1.1.4
+Version: 1.2.0
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,20 +30,32 @@
 
 Install the `lsstream` package via pip through your command line:
 
 ```bash
 > pip install lsstream
 ```
 
+or
+
+```bash
+> pip3 install lsstream
+```
+
 ## 🎯 Usage
 
 To run `lsstream`, type the following command in your command line:
 
 ```bash
-> python -m lsstream.main
+> python -m lsstream.run
+```
+
+or
+
+```bash
+> python3 -m lsstream.run
 ```
 
 Simply follow the on-screen prompts to streamline your streaming experience! :sparkles:
 
 ## 💡 Features
 
 - **Batch File Generation**: Generates multiple .txt files in a snap. Just input your media titles and links, and `lsstream` will use the correct template to create your files.
```

