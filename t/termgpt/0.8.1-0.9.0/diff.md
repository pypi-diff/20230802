# Comparing `tmp/termgpt-0.8.1.tar.gz` & `tmp/termgpt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termgpt-0.8.1.tar", last modified: Wed Jun 14 16:26:47 2023, max compression
+gzip compressed data, was "termgpt-0.9.0.tar", last modified: Wed Aug  2 09:28:37 2023, max compression
```

## Comparing `termgpt-0.8.1.tar` & `termgpt-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:26:47.817546 termgpt-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 16:26:47.817546 termgpt-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-14 16:26:16.000000 termgpt-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:26:47.817546 termgpt-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-14 16:26:16.000000 termgpt-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:26:47.817546 termgpt-0.8.1/termgpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:26:47.817546 termgpt-0.8.1/termgpt/models/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/models/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/models/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:26:47.817546 termgpt-0.8.1/termgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 16:26:47.000000 termgpt-0.8.1/termgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-14 16:26:47.000000 termgpt-0.8.1/termgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:26:47.000000 termgpt-0.8.1/termgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-14 16:26:47.000000 termgpt-0.8.1/termgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 16:26:47.000000 termgpt-0.8.1/termgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 16:26:47.000000 termgpt-0.8.1/termgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:28:37.857117 termgpt-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-02 09:28:37.857117 termgpt-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-08-02 09:28:26.000000 termgpt-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:28:37.857117 termgpt-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 09:28:26.000000 termgpt-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:28:37.857117 termgpt-0.9.0/termgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:28:26.000000 termgpt-0.9.0/termgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-02 09:28:26.000000 termgpt-0.9.0/termgpt/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:28:37.857117 termgpt-0.9.0/termgpt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-02 09:28:26.000000 termgpt-0.9.0/termgpt/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-08-02 09:28:26.000000 termgpt-0.9.0/termgpt/models/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-08-02 09:28:26.000000 termgpt-0.9.0/termgpt/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-08-02 09:28:26.000000 termgpt-0.9.0/termgpt/models/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 09:28:26.000000 termgpt-0.9.0/termgpt/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 09:28:26.000000 termgpt-0.9.0/termgpt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:28:37.857117 termgpt-0.9.0/termgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-02 09:28:37.000000 termgpt-0.9.0/termgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-02 09:28:37.000000 termgpt-0.9.0/termgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:28:37.000000 termgpt-0.9.0/termgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-02 09:28:37.000000 termgpt-0.9.0/termgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 09:28:37.000000 termgpt-0.9.0/termgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 09:28:37.000000 termgpt-0.9.0/termgpt.egg-info/top_level.txt
```

### Comparing `termgpt-0.8.1/PKG-INFO` & `termgpt-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termgpt
-Version: 0.8.1
+Version: 0.9.0
 Summary: A chatGPT client on the terminal
 Home-page: https://github.com/tcapelle/termgpt
 Author: Thomas Capelle
 Author-email: tcapelle@pm.me
 License: MIT
 Keywords: artificial intelligence,generative models,natural language processing,openai
 Classifier: Development Status :: 4 - Beta
```

### Comparing `termgpt-0.8.1/README.md` & `termgpt-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [![PyPI version](https://badge.fury.io/py/termgpt.svg)](https://badge.fury.io/py/termgpt)
 
 # OpenAI Chatbot
 
+![](assets/termGPT.gif)
+
 This program uses the OpenAI API to create a chatbot that can converse with users. The chatbot is powered by the GPT-3.5-turbo (or 4) language model and can answer a wide range of questions. If you are like me and want to stay in the terminal, this is the tool for you.
 
 # Breaking change: Now you can call gpt3 or gpt4 (if you have an api key for it)
 Beware that using gpt4 is expensive (15x more than 3.5-turbo), so use it with care.
 
 ## Install
 You will need and `openAI` api key, the app expects that the key is available as an environment variable: `OPENAI_API_KEY`.
```

### Comparing `termgpt-0.8.1/setup.py` & `termgpt-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `termgpt-0.8.1/termgpt/chat.py` & `termgpt-0.9.0/termgpt/chat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import argparse, atexit
 from dataclasses import dataclass
 
-from termgpt.models import AnthropicChat, CLAUDE, OpenAIChat, GPT3, GPT4
+from termgpt.models import OpenAIChat
+
+# Anthropic
+CLAUDE = "claude-2"
+
+# OpenAI
+GPT3 = "gpt-3.5-turbo"
+GPT4 = "gpt-4"
 
 def parse_args():
     parser = argparse.ArgumentParser(usage="termGPT [options] [file]", description="Chat with GPT-3/4. If no file is provided, you will be prompted to enter a question.")
     parser.add_argument("file", type=str, nargs="?", default=None, help="File to read [optional]")
     parser.add_argument("-r", "--resume", action="store_true", help="Resume previous session")
     parser.add_argument("-c", "--command", type=str, default=None, help="Command to run [optional]")
     parser.add_argument("-o", "--outfile", type=str, default=None, help="Output file [optional]")
@@ -13,14 +20,15 @@
     return parser.parse_args()
 
 exit_commands = ["exit", "quit", "q", "bye", "goodbye", "stop", "end", "finish", "done"]
 
 def main(model_name):
     args = parse_args()
     if model_name == CLAUDE:
+        from termgpt.models.anthropic import AnthropicChat
         chat = AnthropicChat(model_name=CLAUDE, file=args.file, resume=args.resume, command=args.command, out_file=args.outfile, markdown=args.no_markdown)
     else:
         chat = OpenAIChat(model_name, file=args.file, resume=args.resume, command=args.command, out_file=args.outfile, markdown=args.no_markdown)
     atexit.register(chat.save)
     if not args.command:
         while (q := chat.input()) not in exit_commands:
             _ = chat(q)
```

### Comparing `termgpt-0.8.1/termgpt/models/anthropic.py` & `termgpt-0.9.0/termgpt/models/anthropic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import os
 
 import anthropic
 
 from termgpt.models.base import ChatWithHistory
 
-CLAUDE = "claude-v1"  # anthropic
+CLAUDE = "claude-2"
 
 class AnthropicChat(ChatWithHistory):
     """Class to handle chat with Claude, supports history and load from file"""
 
-    def __init__(self, model_name, file=None, resume=False, command=None, out_file=None, markdown=True):
+    def __init__(self, model_name=CLAUDE, file=None, resume=False, command=None, out_file=None, markdown=True):
         try:
-            self.client = anthropic.Client(os.environ['ANTHROPIC_API_KEY'])
+            self.client = anthropic.Anthropic()
         except ImportError:
             "Please install anthropic to use this chatbot\nYou can do it with `pip install anthropic`"
         self.model_name = model_name
         super().__init__(file, resume, command, out_file, markdown)
 
     def call(self):
         prompt = self.preprocess_query()
-        response = self.client.completion(
+        response = self.client.completions.create(
             prompt=prompt + anthropic.AI_PROMPT,
             stop_sequences = [anthropic.HUMAN_PROMPT],
             model=self.model_name,
             max_tokens_to_sample=1000,
         )
-        return response["completion"]
+        return response.completion
 
     def preprocess_query(self):
         query = ""
         for h in self.history:
             if h["role"] == "user" or h["role"] == "system":
                 query += "\n\nHuman: " + h["content"] + "\n"
             elif h["role"] == "assistant":
```

### Comparing `termgpt-0.8.1/termgpt/models/base.py` & `termgpt-0.9.0/termgpt/models/base.py`

 * *Files identical despite different names*

### Comparing `termgpt-0.8.1/termgpt/models/openai.py` & `termgpt-0.9.0/termgpt/models/openai.py`

 * *Files identical despite different names*

### Comparing `termgpt-0.8.1/termgpt/roles.py` & `termgpt-0.9.0/termgpt/roles.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,15 @@
     - If the question is not related to the terminal, just say "I'm not sure how to respond to that
     - If there are multiple ways of performing the same action, reply the simplest one.
     For example, if the questions is "How do I create a new file named "hello.txt?", 
     reply: touch hello.txt instead of echo > hello.txt
     """)
 
 document_role = dedent("""\
-    I will ask question about this document.
-    - If the question is not related to the document, just say "I'm not sure how to respond to that
+    I will ask question about this document. Use this document as context to answer.
     The document:
     """)
 
 if __name__ == "__main__":
     print(f"assistant_role = {assistant_role!r}")
     print(f"commander_role = {commander_role!r}")
     print(f"document_role = {document_role!r}")
```

### Comparing `termgpt-0.8.1/termgpt.egg-info/PKG-INFO` & `termgpt-0.9.0/termgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termgpt
-Version: 0.8.1
+Version: 0.9.0
 Summary: A chatGPT client on the terminal
 Home-page: https://github.com/tcapelle/termgpt
 Author: Thomas Capelle
 Author-email: tcapelle@pm.me
 License: MIT
 Keywords: artificial intelligence,generative models,natural language processing,openai
 Classifier: Development Status :: 4 - Beta
```

