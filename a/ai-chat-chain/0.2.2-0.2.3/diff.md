# Comparing `tmp/ai_chat_chain-0.2.2.tar.gz` & `tmp/ai_chat_chain-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_chat_chain-0.2.2.tar", max compression
+gzip compressed data, was "ai_chat_chain-0.2.3.tar", max compression
```

## Comparing `ai_chat_chain-0.2.2.tar` & `ai_chat_chain-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       86 2023-08-01 02:01:08.212743 ai_chat_chain-0.2.2/ai_chat/__init__.py
--rw-r--r--   0        0        0     5648 2023-08-02 04:03:38.564159 ai_chat_chain-0.2.2/ai_chat/chat.py
--rw-r--r--   0        0        0      136 2023-08-02 04:11:37.726103 ai_chat_chain-0.2.2/ai_chat/defaults.py
--rw-r--r--   0        0        0     1124 2023-08-02 03:55:49.962573 ai_chat_chain-0.2.2/ai_chat/openai.py
--rw-r--r--   0        0        0      115 2023-08-01 14:14:24.976709 ai_chat_chain-0.2.2/ai_chat/store/__init__.py
--rw-r--r--   0        0        0     1037 2023-08-02 02:12:02.573850 ai_chat_chain-0.2.2/ai_chat/store/base.py
--rw-r--r--   0        0        0     5124 2023-08-02 02:40:37.516755 ai_chat_chain-0.2.2/ai_chat/store/sqlite.py
--rw-r--r--   0        0        0     3682 2023-08-01 15:38:29.364571 ai_chat_chain-0.2.2/ai_chat/store/supabase.py
--rw-r--r--   0        0        0     1522 2023-08-02 04:11:37.717065 ai_chat_chain-0.2.2/ai_chat/types.py
--rw-r--r--   0        0        0     1060 2023-08-01 01:56:16.723448 ai_chat_chain-0.2.2/ai_chat/util.py
--rw-r--r--   0        0        0      851 2023-08-02 04:14:44.302007 ai_chat_chain-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1051 2023-08-02 03:00:19.324279 ai_chat_chain-0.2.2/README.md
--rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 ai_chat_chain-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-08-01 02:01:08.212743 ai_chat_chain-0.2.3/ai_chat/__init__.py
+-rw-r--r--   0        0        0     5661 2023-08-02 04:16:47.621971 ai_chat_chain-0.2.3/ai_chat/chat.py
+-rw-r--r--   0        0        0      136 2023-08-02 04:11:37.726103 ai_chat_chain-0.2.3/ai_chat/defaults.py
+-rw-r--r--   0        0        0     1124 2023-08-02 03:55:49.962573 ai_chat_chain-0.2.3/ai_chat/openai.py
+-rw-r--r--   0        0        0      115 2023-08-01 14:14:24.976709 ai_chat_chain-0.2.3/ai_chat/store/__init__.py
+-rw-r--r--   0        0        0     1037 2023-08-02 02:12:02.573850 ai_chat_chain-0.2.3/ai_chat/store/base.py
+-rw-r--r--   0        0        0     5124 2023-08-02 02:40:37.516755 ai_chat_chain-0.2.3/ai_chat/store/sqlite.py
+-rw-r--r--   0        0        0     3682 2023-08-01 15:38:29.364571 ai_chat_chain-0.2.3/ai_chat/store/supabase.py
+-rw-r--r--   0        0        0     1522 2023-08-02 04:11:37.717065 ai_chat_chain-0.2.3/ai_chat/types.py
+-rw-r--r--   0        0        0     1060 2023-08-01 01:56:16.723448 ai_chat_chain-0.2.3/ai_chat/util.py
+-rw-r--r--   0        0        0      851 2023-08-02 04:17:17.203916 ai_chat_chain-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1051 2023-08-02 03:00:19.324279 ai_chat_chain-0.2.3/README.md
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 ai_chat_chain-0.2.3/PKG-INFO
```

### Comparing `ai_chat_chain-0.2.2/ai_chat/chat.py` & `ai_chat_chain-0.2.3/ai_chat/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,16 +111,16 @@
 
         if save:
             request_id, response_id = self.save_interaction(in_role, content, out_role, reply)
         else:
             request_id, response_id = None, None
 
         return ChatResponse(
-            request_id=None,
-            response_id=None,
+            request_id=request_id,
+            response_id=response_id,
             content=reply
         )
 
     def ai_functions(self) -> AIFunctions:
         """Override to vary functions based on state."""
         return self.functions
```

### Comparing `ai_chat_chain-0.2.2/ai_chat/openai.py` & `ai_chat_chain-0.2.3/ai_chat/openai.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.2.2/ai_chat/store/base.py` & `ai_chat_chain-0.2.3/ai_chat/store/base.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.2.2/ai_chat/store/sqlite.py` & `ai_chat_chain-0.2.3/ai_chat/store/sqlite.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.2.2/ai_chat/store/supabase.py` & `ai_chat_chain-0.2.3/ai_chat/store/supabase.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.2.2/ai_chat/types.py` & `ai_chat_chain-0.2.3/ai_chat/types.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.2.2/ai_chat/util.py` & `ai_chat_chain-0.2.3/ai_chat/util.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.2.2/pyproject.toml` & `ai_chat_chain-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-chat-chain"
-version = "0.2.2"
+version = "0.2.3"
 description = "maintain chat conversation state"
 authors = ["erik aronesty <erik@q32.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ai_chat"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ai_chat_chain-0.2.2/README.md` & `ai_chat_chain-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.2.2/PKG-INFO` & `ai_chat_chain-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-chat-chain
-Version: 0.2.2
+Version: 0.2.3
 Summary: maintain chat conversation state
 License: MIT
 Author: erik aronesty
 Author-email: erik@q32.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

