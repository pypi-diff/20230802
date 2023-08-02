# Comparing `tmp/ai_chat_chain-0.2.1.tar.gz` & `tmp/ai_chat_chain-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_chat_chain-0.2.1.tar", max compression
+gzip compressed data, was "ai_chat_chain-0.2.2.tar", max compression
```

## Comparing `ai_chat_chain-0.2.1.tar` & `ai_chat_chain-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       86 2023-08-01 02:01:08.212743 ai_chat_chain-0.2.1/ai_chat/__init__.py
--rw-r--r--   0        0        0     5515 2023-08-02 03:13:46.266704 ai_chat_chain-0.2.1/ai_chat/chat.py
--rw-r--r--   0        0        0      136 2023-08-01 02:01:47.995647 ai_chat_chain-0.2.1/ai_chat/defaults.py
--rw-r--r--   0        0        0     1122 2023-08-02 03:00:19.320279 ai_chat_chain-0.2.1/ai_chat/openai.py
--rw-r--r--   0        0        0      115 2023-08-01 14:14:24.976709 ai_chat_chain-0.2.1/ai_chat/store/__init__.py
--rw-r--r--   0        0        0     1037 2023-08-02 02:12:02.573850 ai_chat_chain-0.2.1/ai_chat/store/base.py
--rw-r--r--   0        0        0     5124 2023-08-02 02:40:37.516755 ai_chat_chain-0.2.1/ai_chat/store/sqlite.py
--rw-r--r--   0        0        0     3682 2023-08-01 15:38:29.364571 ai_chat_chain-0.2.1/ai_chat/store/supabase.py
--rw-r--r--   0        0        0     1510 2023-08-02 02:40:37.496752 ai_chat_chain-0.2.1/ai_chat/types.py
--rw-r--r--   0        0        0     1060 2023-08-01 01:56:16.723448 ai_chat_chain-0.2.1/ai_chat/util.py
--rw-r--r--   0        0        0      851 2023-08-02 03:14:00.718241 ai_chat_chain-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1051 2023-08-02 03:00:19.324279 ai_chat_chain-0.2.1/README.md
--rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 ai_chat_chain-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-08-01 02:01:08.212743 ai_chat_chain-0.2.2/ai_chat/__init__.py
+-rw-r--r--   0        0        0     5648 2023-08-02 04:03:38.564159 ai_chat_chain-0.2.2/ai_chat/chat.py
+-rw-r--r--   0        0        0      136 2023-08-02 04:11:37.726103 ai_chat_chain-0.2.2/ai_chat/defaults.py
+-rw-r--r--   0        0        0     1124 2023-08-02 03:55:49.962573 ai_chat_chain-0.2.2/ai_chat/openai.py
+-rw-r--r--   0        0        0      115 2023-08-01 14:14:24.976709 ai_chat_chain-0.2.2/ai_chat/store/__init__.py
+-rw-r--r--   0        0        0     1037 2023-08-02 02:12:02.573850 ai_chat_chain-0.2.2/ai_chat/store/base.py
+-rw-r--r--   0        0        0     5124 2023-08-02 02:40:37.516755 ai_chat_chain-0.2.2/ai_chat/store/sqlite.py
+-rw-r--r--   0        0        0     3682 2023-08-01 15:38:29.364571 ai_chat_chain-0.2.2/ai_chat/store/supabase.py
+-rw-r--r--   0        0        0     1522 2023-08-02 04:11:37.717065 ai_chat_chain-0.2.2/ai_chat/types.py
+-rw-r--r--   0        0        0     1060 2023-08-01 01:56:16.723448 ai_chat_chain-0.2.2/ai_chat/util.py
+-rw-r--r--   0        0        0      851 2023-08-02 04:14:44.302007 ai_chat_chain-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1051 2023-08-02 03:00:19.324279 ai_chat_chain-0.2.2/README.md
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 ai_chat_chain-0.2.2/PKG-INFO
```

### Comparing `ai_chat_chain-0.2.1/ai_chat/chat.py` & `ai_chat_chain-0.2.2/ai_chat/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def recent_messages(self, content: str):
         return self.store.get_messages(self, content)
 
     def get_system(self):
         """Override this if you want the current state to be considered in the system prompt."""
         return self.ai.system
 
-    def chat(self, content, history: list["Message"] | None = None) -> ChatResponse:
+    def chat(self, content, history: list["Message"] | None = None, save=True) -> ChatResponse:
         """Continue a conversation"""
 
         # this can include embeddings/search if you want, so that's why the content is there
         last_messages = history or self.recent_messages(content)
 
         prompt = [
             {
@@ -55,15 +55,15 @@
                         }
                     )
 
         for msg in last_messages:
             info = self.get_prompt(msg.role, msg.content)
             prompt.append(info)
 
-        return self.chat_as(content, "user", prompt)
+        return self.chat_as(content, "user", prompt, save=save)
 
     @staticmethod
     def get_prompt(role, content):
         prompt = {
             'role': role,
             'content': content,
         }
@@ -87,36 +87,40 @@
             if not functions:
                 raise ValueError(f"Function {function_name} is not available.")
             return functions.execute(function.name, function.arguments, **self.function_kws())
         except Exception as e:
             log.exception("Got an error while running function")
             return f"{self.ai.error_prefix} '{repr(e)}' while running '{function_name}'"
 
-    def chat_as(self, content, in_role, prompt) -> ChatResponse:
+    def chat_as(self, content, in_role, prompt, save=True) -> ChatResponse:
         # add content and role to the prompt
         prompt.append(self.get_prompt(in_role, content))
 
         functions = self.get_functions()
 
         out_role, reply, function = self.chat_complete(prompt, functions)
 
         if function:
             function_result = self.execute_function(function)
 
-            # structure as the db would and save
-            self.save_interaction(in_role, content, out_role, function)
+            if save:
+                # structure as the db would and save
+                self.save_interaction(in_role, content, out_role, function)
 
             # continue chat with the functional reply, don't return until you get an assistant reply
             return self.chat_as(function_result, 'function:' + function.name, prompt)
 
-        request_id, response_id = self.save_interaction(in_role, content, out_role, reply)
+        if save:
+            request_id, response_id = self.save_interaction(in_role, content, out_role, reply)
+        else:
+            request_id, response_id = None, None
 
         return ChatResponse(
-            request_id=request_id,
-            response_id=response_id,
+            request_id=None,
+            response_id=None,
             content=reply
         )
 
     def ai_functions(self) -> AIFunctions:
         """Override to vary functions based on state."""
         return self.functions
```

### Comparing `ai_chat_chain-0.2.1/ai_chat/openai.py` & `ai_chat_chain-0.2.2/ai_chat/openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         if functions:
             args['functions'] = functions.openai_dict()
 
         log.debug(args)
 
         result = openai.ChatCompletion.create(**args)
 
-        log.debug("prompt: %s", prompt)
+        # log.debug("prompt: %s", prompt)
         log.debug("chat complete: %s", result)
 
         role = "assistant"
         message = result.choices[0].message
         content = message.content
 
         func = None
```

### Comparing `ai_chat_chain-0.2.1/ai_chat/store/base.py` & `ai_chat_chain-0.2.2/ai_chat/store/base.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.2.1/ai_chat/store/sqlite.py` & `ai_chat_chain-0.2.2/ai_chat/store/sqlite.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.2.1/ai_chat/store/supabase.py` & `ai_chat_chain-0.2.2/ai_chat/store/supabase.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.2.1/ai_chat/types.py` & `ai_chat_chain-0.2.2/ai_chat/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self, *, id, system, error_prefix=DEFAULT_ERROR_PREFIX, functions: AIFunctions = None,
                  model_params=None, seed_chat=None, max_prompt=10000, **data):
         self.__dict__ = data
         self.id = id
         self.system = system
         self.error_prefix = error_prefix
         self.functions = functions
-        self.seed_chat = seed_chat
+        self.seed_chat: list[list] = seed_chat
         self.max_prompt = max_prompt
         self.model_params = {
             **dict(model=DEFAULT_CHAT_MODEL, temperature=DEFAULT_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS),
             **(model_params or {})}
 
 
 class Message:
```

### Comparing `ai_chat_chain-0.2.1/ai_chat/util.py` & `ai_chat_chain-0.2.2/ai_chat/util.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.2.1/pyproject.toml` & `ai_chat_chain-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-chat-chain"
-version = "0.2.1"
+version = "0.2.2"
 description = "maintain chat conversation state"
 authors = ["erik aronesty <erik@q32.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ai_chat"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ai_chat_chain-0.2.1/README.md` & `ai_chat_chain-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.2.1/PKG-INFO` & `ai_chat_chain-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-chat-chain
-Version: 0.2.1
+Version: 0.2.2
 Summary: maintain chat conversation state
 License: MIT
 Author: erik aronesty
 Author-email: erik@q32.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

