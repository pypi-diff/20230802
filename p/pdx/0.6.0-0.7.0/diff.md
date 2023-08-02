# Comparing `tmp/pdx-0.6.0.tar.gz` & `tmp/pdx-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdx-0.6.0.tar", max compression
+gzip compressed data, was "pdx-0.7.0.tar", max compression
```

## Comparing `pdx-0.6.0.tar` & `pdx-0.7.0.tar`

### file list

```diff
@@ -1,51 +1,55 @@
--rw-r--r--   0        0        0    11346 2023-06-17 05:57:05.771799 pdx-0.6.0/LICENSE
--rw-r--r--   0        0        0     1727 2023-07-27 12:59:32.744111 pdx-0.6.0/README.md
--rw-r--r--   0        0        0      831 2023-07-30 15:55:42.728662 pdx-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      249 2023-07-27 11:10:49.057117 pdx-0.6.0/src/pdx/__init__.py
--rw-r--r--   0        0        0     3060 2023-07-29 16:39:10.239255 pdx-0.6.0/src/pdx/agent/__init__.py
--rw-r--r--   0        0        0     1327 2023-07-27 11:10:49.057529 pdx-0.6.0/src/pdx/agent/config.py
--rw-r--r--   0        0        0     1999 2023-07-29 16:39:10.239382 pdx-0.6.0/src/pdx/agent/metadata.py
--rw-r--r--   0        0        0     1947 2023-07-27 11:10:49.057944 pdx-0.6.0/src/pdx/agent/tester.py
--rw-r--r--   0        0        0     1949 2023-07-29 16:39:10.239496 pdx-0.6.0/src/pdx/cache/__init__.py
--rw-r--r--   0        0        0      615 2023-07-29 16:39:10.239587 pdx-0.6.0/src/pdx/cache/cache.py
--rw-r--r--   0        0        0     1037 2023-07-29 16:39:10.239680 pdx-0.6.0/src/pdx/cache/in_memory_cache.py
--rw-r--r--   0        0        0      297 2023-07-29 16:39:10.239791 pdx-0.6.0/src/pdx/cache/utils.py
--rw-r--r--   0        0        0     1673 2023-07-27 12:55:20.723471 pdx-0.6.0/src/pdx/cli.py
--rw-r--r--   0        0        0        0 2023-06-28 14:39:53.768534 pdx-0.6.0/src/pdx/commands/__init__.py
--rw-r--r--   0        0        0     1317 2023-06-28 15:01:30.272225 pdx-0.6.0/src/pdx/commands/create.py
--rw-r--r--   0        0        0     1043 2023-06-17 06:02:47.694295 pdx-0.6.0/src/pdx/exceptions.py
--rw-r--r--   0        0        0     2172 2023-07-27 11:10:49.058505 pdx-0.6.0/src/pdx/logger.py
--rw-r--r--   0        0        0       90 2023-07-30 15:55:53.185728 pdx-0.6.0/src/pdx/metadata.py
--rw-r--r--   0        0        0        0 2023-07-27 11:10:49.058730 pdx-0.6.0/src/pdx/models/__init__.py
--rw-r--r--   0        0        0       59 2023-07-27 11:10:49.058958 pdx-0.6.0/src/pdx/models/anthropic/__init__.py
--rw-r--r--   0        0        0     3860 2023-07-27 11:10:49.059167 pdx-0.6.0/src/pdx/models/anthropic/client.py
--rw-r--r--   0        0        0     2751 2023-07-29 16:39:10.240085 pdx-0.6.0/src/pdx/models/anthropic/completion.py
--rw-r--r--   0        0        0       57 2023-06-17 06:00:09.710685 pdx-0.6.0/src/pdx/models/anthropic/constants.py
--rw-r--r--   0        0        0     1698 2023-06-17 06:01:13.890539 pdx-0.6.0/src/pdx/models/anthropic/exceptions.py
--rw-r--r--   0        0        0     3543 2023-06-17 06:01:20.740652 pdx-0.6.0/src/pdx/models/api_client.py
--rw-r--r--   0        0        0     2090 2023-07-29 16:39:10.240255 pdx-0.6.0/src/pdx/models/config.py
--rw-r--r--   0        0        0      766 2023-07-29 16:39:10.240384 pdx-0.6.0/src/pdx/models/metadata.py
--rw-r--r--   0        0        0     3764 2023-07-27 11:10:49.059941 pdx-0.6.0/src/pdx/models/model.py
--rw-r--r--   0        0        0       57 2023-07-27 11:10:49.060153 pdx-0.6.0/src/pdx/models/openai/__init__.py
--rw-r--r--   0        0        0     2165 2023-07-27 11:10:49.060479 pdx-0.6.0/src/pdx/models/openai/client.py
--rw-r--r--   0        0        0     3988 2023-07-29 16:39:10.240529 pdx-0.6.0/src/pdx/models/openai/completion.py
--rw-r--r--   0        0        0     1414 2023-06-17 06:01:07.686125 pdx-0.6.0/src/pdx/models/openai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713048 pdx-0.6.0/src/pdx/models/utils.py
--rw-r--r--   0        0        0     2205 2023-07-29 16:39:10.240666 pdx-0.6.0/src/pdx/prompt/__init__.py
--rw-r--r--   0        0        0     3081 2023-07-27 11:10:49.060934 pdx-0.6.0/src/pdx/prompt/config.py
--rw-r--r--   0        0        0     1537 2023-07-29 16:39:10.240787 pdx-0.6.0/src/pdx/prompt/prompt_chain.py
--rw-r--r--   0        0        0     1703 2023-07-29 16:39:10.240918 pdx-0.6.0/src/pdx/prompt/prompt_session.py
--rw-r--r--   0        0        0     2727 2023-07-27 11:10:49.061477 pdx-0.6.0/src/pdx/prompt/prompt_template.py
--rw-r--r--   0        0        0     5210 2023-07-27 11:10:49.061629 pdx-0.6.0/src/pdx/prompt/prompt_tree.py
--rw-r--r--   0        0        0      128 2023-07-29 16:39:10.241044 pdx-0.6.0/src/pdx/settings.py
--rw-r--r--   0        0        0       54 2023-06-28 14:16:27.138776 pdx-0.6.0/src/pdx/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 14:38:23.123005 pdx-0.6.0/src/pdx/templates/simple/Readme.md
--rw-r--r--   0        0        0      405 2023-06-28 14:33:23.114668 pdx-0.6.0/src/pdx/templates/simple/__init__.py
--rw-r--r--   0        0        0      192 2023-06-28 14:54:47.892150 pdx-0.6.0/src/pdx/templates/simple/templates/1_prompt.defaults.yaml
--rw-r--r--   0        0        0      159 2023-06-28 14:27:03.141095 pdx-0.6.0/src/pdx/templates/simple/templates/1_prompt.jinja
--rw-r--r--   0        0        0      191 2023-06-28 14:54:26.649501 pdx-0.6.0/src/pdx/templates/simple/tests/test_1.yaml
--rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713573 pdx-0.6.0/src/pdx/utils/__init__.py
--rw-r--r--   0        0        0      595 2023-06-17 06:00:09.714358 pdx-0.6.0/src/pdx/utils/rw.py
--rw-r--r--   0        0        0     2051 2023-07-27 11:10:49.062145 pdx-0.6.0/src/pdx/worker/__init__.py
--rw-r--r--   0        0        0     1905 2023-07-27 11:10:49.062500 pdx-0.6.0/src/pdx/worker/metadata.py
--rw-r--r--   0        0        0     2798 1970-01-01 00:00:00.000000 pdx-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-17 05:57:05.771799 pdx-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1727 2023-07-27 12:59:32.744111 pdx-0.7.0/README.md
+-rw-r--r--   0        0        0      831 2023-08-02 14:28:47.331492 pdx-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-07-27 11:10:49.057117 pdx-0.7.0/src/pdx/__init__.py
+-rw-r--r--   0        0        0     3060 2023-07-29 16:39:10.239255 pdx-0.7.0/src/pdx/agent/__init__.py
+-rw-r--r--   0        0        0     1327 2023-07-27 11:10:49.057529 pdx-0.7.0/src/pdx/agent/config.py
+-rw-r--r--   0        0        0     1999 2023-07-29 16:39:10.239382 pdx-0.7.0/src/pdx/agent/metadata.py
+-rw-r--r--   0        0        0     1947 2023-07-27 11:10:49.057944 pdx-0.7.0/src/pdx/agent/tester.py
+-rw-r--r--   0        0        0     1949 2023-07-29 16:39:10.239496 pdx-0.7.0/src/pdx/cache/__init__.py
+-rw-r--r--   0        0        0      615 2023-07-29 16:39:10.239587 pdx-0.7.0/src/pdx/cache/cache.py
+-rw-r--r--   0        0        0     1037 2023-07-29 16:39:10.239680 pdx-0.7.0/src/pdx/cache/in_memory_cache.py
+-rw-r--r--   0        0        0      297 2023-07-29 16:39:10.239791 pdx-0.7.0/src/pdx/cache/utils.py
+-rw-r--r--   0        0        0     1673 2023-07-27 12:55:20.723471 pdx-0.7.0/src/pdx/cli.py
+-rw-r--r--   0        0        0        0 2023-06-28 14:39:53.768534 pdx-0.7.0/src/pdx/commands/__init__.py
+-rw-r--r--   0        0        0     1317 2023-06-28 15:01:30.272225 pdx-0.7.0/src/pdx/commands/create.py
+-rw-r--r--   0        0        0     1043 2023-06-17 06:02:47.694295 pdx-0.7.0/src/pdx/exceptions.py
+-rw-r--r--   0        0        0     2172 2023-07-27 11:10:49.058505 pdx-0.7.0/src/pdx/logger.py
+-rw-r--r--   0        0        0       90 2023-08-02 14:09:00.551170 pdx-0.7.0/src/pdx/metadata.py
+-rw-r--r--   0        0        0        0 2023-07-27 11:10:49.058730 pdx-0.7.0/src/pdx/models/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-27 11:10:49.058958 pdx-0.7.0/src/pdx/models/anthropic/__init__.py
+-rw-r--r--   0        0        0     3860 2023-07-27 11:10:49.059167 pdx-0.7.0/src/pdx/models/anthropic/client.py
+-rw-r--r--   0        0        0     2751 2023-07-29 16:39:10.240085 pdx-0.7.0/src/pdx/models/anthropic/completion.py
+-rw-r--r--   0        0        0       57 2023-06-17 06:00:09.710685 pdx-0.7.0/src/pdx/models/anthropic/constants.py
+-rw-r--r--   0        0        0     1698 2023-06-17 06:01:13.890539 pdx-0.7.0/src/pdx/models/anthropic/exceptions.py
+-rw-r--r--   0        0        0     3543 2023-06-17 06:01:20.740652 pdx-0.7.0/src/pdx/models/api_client.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:09:00.551255 pdx-0.7.0/src/pdx/models/cohere/__init__.py
+-rw-r--r--   0        0        0     2544 2023-08-02 14:09:00.551533 pdx-0.7.0/src/pdx/models/cohere/client.py
+-rw-r--r--   0        0        0     1105 2023-08-02 14:09:00.551718 pdx-0.7.0/src/pdx/models/cohere/exceptions.py
+-rw-r--r--   0        0        0     3338 2023-08-02 14:09:00.551902 pdx-0.7.0/src/pdx/models/cohere/generation.py
+-rw-r--r--   0        0        0     2244 2023-08-02 14:18:48.369137 pdx-0.7.0/src/pdx/models/config.py
+-rw-r--r--   0        0        0      821 2023-08-02 14:09:00.552392 pdx-0.7.0/src/pdx/models/metadata.py
+-rw-r--r--   0        0        0     3764 2023-07-27 11:10:49.059941 pdx-0.7.0/src/pdx/models/model.py
+-rw-r--r--   0        0        0       57 2023-07-27 11:10:49.060153 pdx-0.7.0/src/pdx/models/openai/__init__.py
+-rw-r--r--   0        0        0     2165 2023-07-27 11:10:49.060479 pdx-0.7.0/src/pdx/models/openai/client.py
+-rw-r--r--   0        0        0     3988 2023-07-29 16:39:10.240529 pdx-0.7.0/src/pdx/models/openai/completion.py
+-rw-r--r--   0        0        0     1414 2023-06-17 06:01:07.686125 pdx-0.7.0/src/pdx/models/openai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713048 pdx-0.7.0/src/pdx/models/utils.py
+-rw-r--r--   0        0        0     2205 2023-07-29 16:39:10.240666 pdx-0.7.0/src/pdx/prompt/__init__.py
+-rw-r--r--   0        0        0     3081 2023-07-27 11:10:49.060934 pdx-0.7.0/src/pdx/prompt/config.py
+-rw-r--r--   0        0        0     1537 2023-07-29 16:39:10.240787 pdx-0.7.0/src/pdx/prompt/prompt_chain.py
+-rw-r--r--   0        0        0     1703 2023-07-29 16:39:10.240918 pdx-0.7.0/src/pdx/prompt/prompt_session.py
+-rw-r--r--   0        0        0     2727 2023-07-27 11:10:49.061477 pdx-0.7.0/src/pdx/prompt/prompt_template.py
+-rw-r--r--   0        0        0     5210 2023-07-27 11:10:49.061629 pdx-0.7.0/src/pdx/prompt/prompt_tree.py
+-rw-r--r--   0        0        0      128 2023-07-29 16:39:10.241044 pdx-0.7.0/src/pdx/settings.py
+-rw-r--r--   0        0        0       54 2023-06-28 14:16:27.138776 pdx-0.7.0/src/pdx/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 14:38:23.123005 pdx-0.7.0/src/pdx/templates/simple/Readme.md
+-rw-r--r--   0        0        0      405 2023-06-28 14:33:23.114668 pdx-0.7.0/src/pdx/templates/simple/__init__.py
+-rw-r--r--   0        0        0      192 2023-06-28 14:54:47.892150 pdx-0.7.0/src/pdx/templates/simple/templates/1_prompt.defaults.yaml
+-rw-r--r--   0        0        0      159 2023-06-28 14:27:03.141095 pdx-0.7.0/src/pdx/templates/simple/templates/1_prompt.jinja
+-rw-r--r--   0        0        0      191 2023-06-28 14:54:26.649501 pdx-0.7.0/src/pdx/templates/simple/tests/test_1.yaml
+-rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713573 pdx-0.7.0/src/pdx/utils/__init__.py
+-rw-r--r--   0        0        0      595 2023-06-17 06:00:09.714358 pdx-0.7.0/src/pdx/utils/rw.py
+-rw-r--r--   0        0        0     2051 2023-07-27 11:10:49.062145 pdx-0.7.0/src/pdx/worker/__init__.py
+-rw-r--r--   0        0        0     1905 2023-07-27 11:10:49.062500 pdx-0.7.0/src/pdx/worker/metadata.py
+-rw-r--r--   0        0        0     2798 1970-01-01 00:00:00.000000 pdx-0.7.0/PKG-INFO
```

### Comparing `pdx-0.6.0/LICENSE` & `pdx-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/README.md` & `pdx-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/pyproject.toml` & `pdx-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdx"
-version = "0.6.0"
+version = "0.7.0"
 description = "Prompt Engineering and Dev-Ops toolkits. A faster way to build and manage applications powered by Language Models."
 keywords = ["prompt", "LLM", "prompt engineering", "dev-ops", "observability", "apps"]
 authors = ["Adithya Krishnan <krishsandeep@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "pdx", from = "src"}]
```

### Comparing `pdx-0.6.0/src/pdx/agent/__init__.py` & `pdx-0.7.0/src/pdx/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/agent/config.py` & `pdx-0.7.0/src/pdx/agent/config.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/agent/metadata.py` & `pdx-0.7.0/src/pdx/agent/metadata.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/agent/tester.py` & `pdx-0.7.0/src/pdx/agent/tester.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/cache/__init__.py` & `pdx-0.7.0/src/pdx/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/cache/cache.py` & `pdx-0.7.0/src/pdx/cache/cache.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/cache/in_memory_cache.py` & `pdx-0.7.0/src/pdx/cache/in_memory_cache.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/cli.py` & `pdx-0.7.0/src/pdx/cli.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/commands/create.py` & `pdx-0.7.0/src/pdx/commands/create.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/exceptions.py` & `pdx-0.7.0/src/pdx/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/logger.py` & `pdx-0.7.0/src/pdx/logger.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/models/anthropic/client.py` & `pdx-0.7.0/src/pdx/models/anthropic/client.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/models/anthropic/completion.py` & `pdx-0.7.0/src/pdx/models/anthropic/completion.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/models/anthropic/exceptions.py` & `pdx-0.7.0/src/pdx/models/anthropic/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/models/api_client.py` & `pdx-0.7.0/src/pdx/models/api_client.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/models/config.py` & `pdx-0.7.0/src/pdx/models/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 from typing import Optional
 from pydantic import BaseModel, Field
 
 # Available LLM completion models
 OPENAI_COMPLETION_MODELS = ["text-davinci-003", "gpt-3.5-turbo", "gpt-4"]
-ANTHROPIC_COMPLETION_MODELS = ["claude-v1", "claude-v1-100k", "claude-instant-v1", "claude-instant-v1-100k",
+ANTHROPIC_COMPLETION_MODELS = ["claude-2", "claude-2.0", "claude-v1", "claude-v1-100k", "claude-instant-v1", "claude-instant-v1-100k",
                                "claude-v1.3", "claude-v1.3-100k", "claude-v1.2" "claude-v1.0", "claude-instant-v1.1",
                                "claude-instant-v1.1-100k", "claude-instant-v1.0"]
+COHERE_COMPLETION_MODELS = ["command", "command-nightly", "command-light",
+                            "command-light-nightly"]
 
 
 class ModelConfig(BaseModel):
     id: str
     params: dict = Field(default_factory=dict)
     name: Optional[str] = Field(default=None)
     provider: Optional[str] = Field(default=None)
```

### Comparing `pdx-0.6.0/src/pdx/models/metadata.py` & `pdx-0.7.0/src/pdx/models/metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from typing import Optional
+from typing import Optional, Any
 from pydantic import BaseModel, Field
 
 
 class ModelTokenUsage(BaseModel):
     response: Optional[int] = Field(default=None)
     prompt: Optional[int] = Field(default=None)
     total: Optional[int] = Field(default=None)
 
 
 class ResponseMetadata(BaseModel):
     model: str
     api_log_id: Optional[str] = Field(default=None)
     stop: Optional[str] = Field(default=None)
     stop_reason: Optional[str] = Field(default=None)
+    warnings: Optional[Any] = Field(default=None)
     token_usage: Optional[ModelTokenUsage] = Field(default=None)
     latency: Optional[float] = Field(default=None)
 
 
 class ModelResponse(BaseModel):
     metadata: Optional[ResponseMetadata] = Field(default=None)
     request_params: Optional[dict] = Field(default=None)
```

### Comparing `pdx-0.6.0/src/pdx/models/model.py` & `pdx-0.7.0/src/pdx/models/model.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/models/openai/client.py` & `pdx-0.7.0/src/pdx/models/openai/client.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/models/openai/completion.py` & `pdx-0.7.0/src/pdx/models/openai/completion.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/models/openai/exceptions.py` & `pdx-0.7.0/src/pdx/models/openai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/prompt/__init__.py` & `pdx-0.7.0/src/pdx/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/prompt/config.py` & `pdx-0.7.0/src/pdx/prompt/config.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/prompt/prompt_chain.py` & `pdx-0.7.0/src/pdx/prompt/prompt_chain.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/prompt/prompt_session.py` & `pdx-0.7.0/src/pdx/prompt/prompt_session.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/prompt/prompt_template.py` & `pdx-0.7.0/src/pdx/prompt/prompt_template.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/prompt/prompt_tree.py` & `pdx-0.7.0/src/pdx/prompt/prompt_tree.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/utils/rw.py` & `pdx-0.7.0/src/pdx/utils/rw.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/worker/__init__.py` & `pdx-0.7.0/src/pdx/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/src/pdx/worker/metadata.py` & `pdx-0.7.0/src/pdx/worker/metadata.py`

 * *Files identical despite different names*

### Comparing `pdx-0.6.0/PKG-INFO` & `pdx-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdx
-Version: 0.6.0
+Version: 0.7.0
 Summary: Prompt Engineering and Dev-Ops toolkits. A faster way to build and manage applications powered by Language Models.
 License: Apache-2.0
 Keywords: prompt,LLM,prompt engineering,dev-ops,observability,apps
 Author: Adithya Krishnan
 Author-email: krishsandeep@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
```

