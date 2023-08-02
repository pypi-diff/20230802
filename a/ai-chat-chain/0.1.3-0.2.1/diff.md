# Comparing `tmp/ai_chat_chain-0.1.3.tar.gz` & `tmp/ai_chat_chain-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_chat_chain-0.1.3.tar", max compression
+gzip compressed data, was "ai_chat_chain-0.2.1.tar", max compression
```

## Comparing `ai_chat_chain-0.1.3.tar` & `ai_chat_chain-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       86 2023-08-01 02:01:08.212743 ai_chat_chain-0.1.3/ai_chat/__init__.py
--rw-r--r--   0        0        0     5503 2023-08-01 19:46:36.964204 ai_chat_chain-0.1.3/ai_chat/chat.py
--rw-r--r--   0        0        0      136 2023-08-01 02:01:47.995647 ai_chat_chain-0.1.3/ai_chat/defaults.py
--rw-r--r--   0        0        0     1124 2023-08-01 19:47:07.364101 ai_chat_chain-0.1.3/ai_chat/openai.py
--rw-r--r--   0        0        0      115 2023-08-01 14:14:24.976709 ai_chat_chain-0.1.3/ai_chat/store/__init__.py
--rw-r--r--   0        0        0     1043 2023-08-01 17:00:50.526537 ai_chat_chain-0.1.3/ai_chat/store/base.py
--rw-r--r--   0        0        0     5127 2023-08-01 15:38:29.361570 ai_chat_chain-0.1.3/ai_chat/store/sqlite.py
--rw-r--r--   0        0        0     3682 2023-08-01 15:38:29.364571 ai_chat_chain-0.1.3/ai_chat/store/supabase.py
--rw-r--r--   0        0        0     1498 2023-08-01 19:45:19.241783 ai_chat_chain-0.1.3/ai_chat/types.py
--rw-r--r--   0        0        0     1060 2023-08-01 01:56:16.723448 ai_chat_chain-0.1.3/ai_chat/util.py
--rw-r--r--   0        0        0      851 2023-08-01 20:01:10.645931 ai_chat_chain-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      907 2023-08-01 17:08:52.775187 ai_chat_chain-0.1.3/README.md
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 ai_chat_chain-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-08-01 02:01:08.212743 ai_chat_chain-0.2.1/ai_chat/__init__.py
+-rw-r--r--   0        0        0     5515 2023-08-02 03:13:46.266704 ai_chat_chain-0.2.1/ai_chat/chat.py
+-rw-r--r--   0        0        0      136 2023-08-01 02:01:47.995647 ai_chat_chain-0.2.1/ai_chat/defaults.py
+-rw-r--r--   0        0        0     1122 2023-08-02 03:00:19.320279 ai_chat_chain-0.2.1/ai_chat/openai.py
+-rw-r--r--   0        0        0      115 2023-08-01 14:14:24.976709 ai_chat_chain-0.2.1/ai_chat/store/__init__.py
+-rw-r--r--   0        0        0     1037 2023-08-02 02:12:02.573850 ai_chat_chain-0.2.1/ai_chat/store/base.py
+-rw-r--r--   0        0        0     5124 2023-08-02 02:40:37.516755 ai_chat_chain-0.2.1/ai_chat/store/sqlite.py
+-rw-r--r--   0        0        0     3682 2023-08-01 15:38:29.364571 ai_chat_chain-0.2.1/ai_chat/store/supabase.py
+-rw-r--r--   0        0        0     1510 2023-08-02 02:40:37.496752 ai_chat_chain-0.2.1/ai_chat/types.py
+-rw-r--r--   0        0        0     1060 2023-08-01 01:56:16.723448 ai_chat_chain-0.2.1/ai_chat/util.py
+-rw-r--r--   0        0        0      851 2023-08-02 03:14:00.718241 ai_chat_chain-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1051 2023-08-02 03:00:19.324279 ai_chat_chain-0.2.1/README.md
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 ai_chat_chain-0.2.1/PKG-INFO
```

### Comparing `ai_chat_chain-0.1.3/ai_chat/chat.py` & `ai_chat_chain-0.2.1/ai_chat/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 
 from ai_chat.types import Message, Function, ChatResponse, AiConfig, AIFunctions
 from ai_chat.store.base import Store
 from ai_chat.util import uuid
 
 
 class Chat(ABC):
-    def __init__(self, store: Store, ai: "AiConfig", thread_id: str, state=None):
+    def __init__(self, *, ai: "AiConfig", thread_id: str | None = None, store: Store | None = None):
         """Thread of conversation"""
         self.ai = ai
         self.functions = self.ai.functions
         self.thread_id = thread_id
         self.store = store
-        self.state = state or {}
 
     def function_kws(self):
         """Override this to provide other kwargs to functions"""
         return {"chat": self}
 
     def recent_messages(self, content: str):
         return self.store.get_messages(self, content)
@@ -29,15 +28,14 @@
 
     def chat(self, content, history: list["Message"] | None = None) -> ChatResponse:
         """Continue a conversation"""
 
         # this can include embeddings/search if you want, so that's why the content is there
         last_messages = history or self.recent_messages(content)
 
-
         prompt = [
             {
                 "role": "system",
                 "content": self.get_system()
             }
         ]
 
@@ -130,15 +128,16 @@
         return self.ai_functions() and self.ai_functions()
 
     def add_message(self, role: str, content: str | Function):
         if isinstance(content, Function):
             role = "function:" + content.name
             content = content.arguments
         user_chat = self.structure_reply(content, role)
-        self.store.add_message(user_chat, self)
+        if self.store:
+            self.store.add_message(user_chat, self)
         return user_chat.id
 
     def save_interaction(self, in_role: str, content: str, out_role: str, reply: str | Function):
         is_error = in_role == "function_all" and reply.startswith(self.ai.error_prefix)
 
         if not is_error:
             user_id = self.add_message(in_role, content)
```

### Comparing `ai_chat_chain-0.1.3/ai_chat/openai.py` & `ai_chat_chain-0.2.1/ai_chat/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import openai
 
 from ai_chat.chat import Chat
 from ai_chat.types import AIFunctions
 from ai_chat import Function
 
 
-
 class OpenaiChat(Chat):
     def chat_complete(self, prompt, functions: AIFunctions) -> tuple[str, str, Function | None]:
         openai.api_key = os.getenv("OPENAI_API_KEY")
 
         args = dict(
             messages=prompt,
             **self.ai.model_params,
```

### Comparing `ai_chat_chain-0.1.3/ai_chat/store/base.py` & `ai_chat_chain-0.2.1/ai_chat/store/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,13 +32,13 @@
         ...
 
     @abstractmethod
     def set_glob(self, key: str, state: State):
         ...
 
     @abstractmethod
-    def get_glob(self, key: str) -> list[State]:
+    def get_glob(self, key: str) -> State:
         ...
 
     @abstractmethod
     def enum_glob(self, key: str) -> list[tuple[str, State]]:
         ...
```

### Comparing `ai_chat_chain-0.1.3/ai_chat/store/sqlite.py` & `ai_chat_chain-0.2.1/ai_chat/store/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def add_message(self, message: "Message", chat: "Chat"):
         """Add chat to db, must guarantee sort order somehow."""
         query = """
             INSERT INTO messages (id, role, content, thread_id, ai_id, created_at)
             VALUES (?, ?, ?, ?, ?, ?);
         """
-        params = (message.id, message.role, message.content, message.thread_id, chat.ai.id, time.time())
+        params = (message.id, message.role, message.content, chat.thread_id, chat.ai.id, time.time())
         self.conn.execute(query, params)
         self.conn.commit()
 
     def set_state(self, chat: "Chat", key: str, state: "State"):
         """Add state to db, this is generally 'across chats'."""
         query = """
             INSERT OR REPLACE INTO state (key, content, ai_id, created_at)
```

### Comparing `ai_chat_chain-0.1.3/ai_chat/store/supabase.py` & `ai_chat_chain-0.2.1/ai_chat/store/supabase.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.1.3/ai_chat/types.py` & `ai_chat_chain-0.2.1/ai_chat/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,17 +25,17 @@
             **(model_params or {})}
 
 
 class Message:
     id: str
     role: str
     content: str
-    thread_id: str
+    thread_id: str | None
 
-    def __init__(self, *, id, role, content, thread_id, **data):
+    def __init__(self, *, id, role, content, thread_id=None, **data):
         self.__dict__ = data
         self.id = id
         self.role = role
         self.content = content
         self.thread_id = thread_id
```

### Comparing `ai_chat_chain-0.1.3/ai_chat/util.py` & `ai_chat_chain-0.2.1/ai_chat/util.py`

 * *Files identical despite different names*

### Comparing `ai_chat_chain-0.1.3/pyproject.toml` & `ai_chat_chain-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-chat-chain"
-version = "0.1.3"
+version = "0.2.1"
 description = "maintain chat conversation state"
 authors = ["erik aronesty <erik@q32.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ai_chat"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ai_chat_chain-0.1.3/README.md` & `ai_chat_chain-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -15,20 +15,30 @@
 
 ```python
 from ai_chat import AiConfig
 
 # only supports openai for now, todo: add other models
 from ai_chat.openai import OpenaiChat
 from ai_chat.store import SupabaseStore
+from ai_functions import AIFunctions
 
 # supports SqliteStore() as well as MemoryStore() for storing the chain of prompts
 
 store = SupabaseStore()
 conf = AiConfig(id="persona-id-1", system="You are a silly friend.")
-session = OpenaiChat(store, conf, "session-1")
+session = OpenaiChat(store=store, ai=conf, thread_id="session-1")
+
+def search_google():
+    ...
+
+def get_calendar():
+    ...
+
+def add_calendar():
+    ...
 
 session.functions = AIFunctions([search_google, get_calendar, add_calendar])
 
 print(session.chat("hello").content)
 
 # this contains the hello, and the reply in the context
 print(session.chat("cool").content)
```

### Comparing `ai_chat_chain-0.1.3/PKG-INFO` & `ai_chat_chain-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-chat-chain
-Version: 0.1.3
+Version: 0.2.1
 Summary: maintain chat conversation state
 License: MIT
 Author: erik aronesty
 Author-email: erik@q32.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -36,20 +36,30 @@
 
 ```python
 from ai_chat import AiConfig
 
 # only supports openai for now, todo: add other models
 from ai_chat.openai import OpenaiChat
 from ai_chat.store import SupabaseStore
+from ai_functions import AIFunctions
 
 # supports SqliteStore() as well as MemoryStore() for storing the chain of prompts
 
 store = SupabaseStore()
 conf = AiConfig(id="persona-id-1", system="You are a silly friend.")
-session = OpenaiChat(store, conf, "session-1")
+session = OpenaiChat(store=store, ai=conf, thread_id="session-1")
+
+def search_google():
+    ...
+
+def get_calendar():
+    ...
+
+def add_calendar():
+    ...
 
 session.functions = AIFunctions([search_google, get_calendar, add_calendar])
 
 print(session.chat("hello").content)
 
 # this contains the hello, and the reply in the context
 print(session.chat("cool").content)
```

