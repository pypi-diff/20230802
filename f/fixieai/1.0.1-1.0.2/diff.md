# Comparing `tmp/fixieai-1.0.1.tar.gz` & `tmp/fixieai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixieai-1.0.1.tar", max compression
+gzip compressed data, was "fixieai-1.0.2.tar", max compression
```

## Comparing `fixieai-1.0.1.tar` & `fixieai-1.0.2.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0    11357 2023-02-07 23:45:43.683245 fixieai-1.0.1/LICENSE
--rw-r--r--   0        0        0     1388 2023-06-05 22:24:43.848602 fixieai-1.0.1/fixieai/__init__.py
--rw-r--r--   0        0        0     1301 2023-06-05 22:24:43.848729 fixieai-1.0.1/fixieai/agents/__init__.py
--rw-r--r--   0        0        0    10564 2023-06-05 22:24:43.849458 fixieai-1.0.1/fixieai/agents/agent_base.py
--rw-r--r--   0        0        0    12042 2023-06-05 22:24:43.849590 fixieai-1.0.1/fixieai/agents/agent_base_test.py
--rw-r--r--   0        0        0    15267 2023-06-05 22:24:43.849720 fixieai-1.0.1/fixieai/agents/agent_func.py
--rw-r--r--   0        0        0     8715 2023-06-05 22:24:43.849847 fixieai-1.0.1/fixieai/agents/agent_func_test.py
--rw-r--r--   0        0        0     2965 2023-06-05 22:24:43.849947 fixieai-1.0.1/fixieai/agents/api.py
--rw-r--r--   0        0        0      863 2023-03-09 19:26:37.964207 fixieai-1.0.1/fixieai/agents/api_test.py
--rw-r--r--   0        0        0     3786 2023-06-05 22:24:43.850060 fixieai-1.0.1/fixieai/agents/code_shot.py
--rw-r--r--   0        0        0     3306 2023-06-05 22:24:43.850149 fixieai-1.0.1/fixieai/agents/code_shot_test.py
--rw-r--r--   0        0        0     7152 2023-06-05 22:24:43.850261 fixieai-1.0.1/fixieai/agents/corpora.py
--rw-r--r--   0        0        0     1943 2023-06-05 22:24:43.850315 fixieai-1.0.1/fixieai/agents/corpora_test.py
--rw-r--r--   0        0        0     2279 2023-06-05 22:24:43.850379 fixieai-1.0.1/fixieai/agents/exceptions.py
--rw-r--r--   0        0        0     1046 2023-03-30 16:24:35.974599 fixieai-1.0.1/fixieai/agents/llm_settings.py
--rw-r--r--   0        0        0      891 2023-06-05 22:24:43.850459 fixieai-1.0.1/fixieai/agents/metadata.py
--rw-r--r--   0        0        0     9000 2023-06-05 22:24:43.850566 fixieai-1.0.1/fixieai/agents/oauth.py
--rw-r--r--   0        0        0     4048 2023-04-25 03:00:21.707100 fixieai-1.0.1/fixieai/agents/openai_proxy.py
--rw-r--r--   0        0        0     1627 2023-04-25 03:00:21.707249 fixieai-1.0.1/fixieai/agents/openai_proxy_test.py
--rw-r--r--   0        0        0     2439 2023-06-05 22:24:43.850673 fixieai-1.0.1/fixieai/agents/standalone.py
--rw-r--r--   0        0        0     4414 2023-06-05 22:24:43.850780 fixieai-1.0.1/fixieai/agents/standalone_test.py
--rw-r--r--   0        0        0     1918 2023-06-05 22:24:43.850853 fixieai-1.0.1/fixieai/agents/token.py
--rw-r--r--   0        0        0     4951 2023-06-05 22:24:43.850975 fixieai-1.0.1/fixieai/agents/user_storage.py
--rw-r--r--   0        0        0     3388 2023-06-05 22:24:43.851664 fixieai-1.0.1/fixieai/agents/user_storage_test.py
--rw-r--r--   0        0        0     7966 2023-04-25 03:00:21.707832 fixieai-1.0.1/fixieai/agents/utils.py
--rw-r--r--   0        0        0     5253 2023-03-25 02:35:27.951289 fixieai-1.0.1/fixieai/agents/utils_test.py
--rw-r--r--   0        0        0        0 2023-03-09 19:26:37.965971 fixieai-1.0.1/fixieai/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-09 19:26:37.966917 fixieai-1.0.1/fixieai/cli/agent/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-05 22:24:43.852159 fixieai-1.0.1/fixieai/cli/agent/agent_config.py
--rw-r--r--   0        0        0    35054 2023-06-13 15:56:30.159010 fixieai-1.0.1/fixieai/cli/agent/commands.py
--rw-r--r--   0        0        0    16037 2023-06-13 15:44:25.677117 fixieai-1.0.1/fixieai/cli/agent/commands_test.py
--rw-r--r--   0        0        0     3488 2023-06-05 22:24:43.852973 fixieai-1.0.1/fixieai/cli/agent/loader.py
--rw-r--r--   0        0        0     1753 2023-04-01 03:10:09.936255 fixieai-1.0.1/fixieai/cli/agent/tunnel.py
--rw-r--r--   0        0        0        0 2023-03-09 19:26:37.967623 fixieai-1.0.1/fixieai/cli/auth/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-01 23:07:48.256193 fixieai-1.0.1/fixieai/cli/auth/commands.py
--rw-r--r--   0        0        0     1942 2023-03-09 19:26:37.968039 fixieai-1.0.1/fixieai/cli/auth/oauth_flow.py
--rw-r--r--   0        0        0     2667 2023-03-30 16:24:35.975821 fixieai-1.0.1/fixieai/cli/auth/user_config.py
--rw-r--r--   0        0        0     2120 2023-03-30 16:24:35.975913 fixieai-1.0.1/fixieai/cli/auth/user_config_test.py
--rwxr-xr-x   0        0        0     3290 2023-04-12 15:22:13.299089 fixieai-1.0.1/fixieai/cli/cli.py
--rw-r--r--   0        0        0        0 2023-03-09 19:26:37.968257 fixieai-1.0.1/fixieai/cli/session/__init__.py
--rw-r--r--   0        0        0     4761 2023-04-12 01:22:58.394077 fixieai-1.0.1/fixieai/cli/session/commands.py
--rw-r--r--   0        0        0     4720 2023-06-05 22:24:43.853234 fixieai-1.0.1/fixieai/cli/session/console.py
--rw-r--r--   0        0        0     1523 2023-03-30 16:24:35.976029 fixieai-1.0.1/fixieai/cli/utils.py
--rw-r--r--   0        0        0      655 2023-03-22 17:59:48.856855 fixieai-1.0.1/fixieai/cli/utils_test.py
--rw-r--r--   0        0        0      322 2023-03-09 19:26:37.968576 fixieai-1.0.1/fixieai/client/__init__.py
--rw-r--r--   0        0        0    11895 2023-06-13 15:44:25.677595 fixieai-1.0.1/fixieai/client/agent.py
--rwxr-xr-x   0        0        0    12607 2023-06-13 15:56:45.258897 fixieai-1.0.1/fixieai/client/client.py
--rw-r--r--   0        0        0     4987 2023-03-10 17:44:40.327464 fixieai-1.0.1/fixieai/client/client_test.py
--rwxr-xr-x   0        0        0     8750 2023-03-10 05:45:43.499628 fixieai-1.0.1/fixieai/client/session.py
--rw-r--r--   0        0        0     1402 2023-06-05 22:24:43.853545 fixieai-1.0.1/fixieai/client/utils.py
--rw-r--r--   0        0        0     2394 2023-06-05 22:24:43.853647 fixieai-1.0.1/fixieai/constants.py
--rw-r--r--   0        0        0     2026 2023-06-13 16:02:31.198419 fixieai-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 fixieai-1.0.1/setup.py
--rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 fixieai-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-18 21:21:47.580356 fixieai-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1456 2023-08-01 22:36:16.720638 fixieai-1.0.2/fixieai/__init__.py
+-rw-r--r--   0        0        0     1301 2023-08-01 22:36:16.721137 fixieai-1.0.2/fixieai/agents/__init__.py
+-rw-r--r--   0        0        0    10564 2023-08-01 22:36:16.721458 fixieai-1.0.2/fixieai/agents/agent_base.py
+-rw-r--r--   0        0        0    12042 2023-08-01 22:36:16.721808 fixieai-1.0.2/fixieai/agents/agent_base_test.py
+-rw-r--r--   0        0        0    15267 2023-08-01 22:36:16.722088 fixieai-1.0.2/fixieai/agents/agent_func.py
+-rw-r--r--   0        0        0     8715 2023-08-01 22:36:16.722561 fixieai-1.0.2/fixieai/agents/agent_func_test.py
+-rw-r--r--   0        0        0     2965 2023-08-01 22:36:16.723036 fixieai-1.0.2/fixieai/agents/api.py
+-rw-r--r--   0        0        0      863 2023-03-07 19:11:26.788937 fixieai-1.0.2/fixieai/agents/api_test.py
+-rw-r--r--   0        0        0     3786 2023-08-01 22:36:16.723341 fixieai-1.0.2/fixieai/agents/code_shot.py
+-rw-r--r--   0        0        0     3306 2023-08-01 22:36:16.723647 fixieai-1.0.2/fixieai/agents/code_shot_test.py
+-rw-r--r--   0        0        0     7152 2023-08-01 22:36:16.723851 fixieai-1.0.2/fixieai/agents/corpora.py
+-rw-r--r--   0        0        0     1943 2023-08-01 22:36:16.724099 fixieai-1.0.2/fixieai/agents/corpora_test.py
+-rw-r--r--   0        0        0     2279 2023-08-01 22:36:16.724302 fixieai-1.0.2/fixieai/agents/exceptions.py
+-rw-r--r--   0        0        0     1046 2023-04-28 22:19:21.471721 fixieai-1.0.2/fixieai/agents/llm_settings.py
+-rw-r--r--   0        0        0      891 2023-08-01 22:36:16.724477 fixieai-1.0.2/fixieai/agents/metadata.py
+-rw-r--r--   0        0        0     9000 2023-08-01 22:36:16.724791 fixieai-1.0.2/fixieai/agents/oauth.py
+-rw-r--r--   0        0        0     4048 2023-08-01 22:36:16.725207 fixieai-1.0.2/fixieai/agents/openai_proxy.py
+-rw-r--r--   0        0        0     1627 2023-08-01 22:36:16.725754 fixieai-1.0.2/fixieai/agents/openai_proxy_test.py
+-rw-r--r--   0        0        0     2439 2023-08-01 22:36:16.726056 fixieai-1.0.2/fixieai/agents/standalone.py
+-rw-r--r--   0        0        0     4414 2023-08-01 22:36:16.726252 fixieai-1.0.2/fixieai/agents/standalone_test.py
+-rw-r--r--   0        0        0     1918 2023-08-01 22:36:16.726392 fixieai-1.0.2/fixieai/agents/token.py
+-rw-r--r--   0        0        0     4951 2023-08-01 22:36:16.726565 fixieai-1.0.2/fixieai/agents/user_storage.py
+-rw-r--r--   0        0        0     3388 2023-08-01 22:36:16.726979 fixieai-1.0.2/fixieai/agents/user_storage_test.py
+-rw-r--r--   0        0        0     7966 2023-08-01 22:36:16.727450 fixieai-1.0.2/fixieai/agents/utils.py
+-rw-r--r--   0        0        0     5253 2023-03-23 20:13:08.313763 fixieai-1.0.2/fixieai/agents/utils_test.py
+-rw-r--r--   0        0        0        0 2023-03-05 05:28:15.595965 fixieai-1.0.2/fixieai/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-05 05:28:15.596298 fixieai-1.0.2/fixieai/cli/agent/__init__.py
+-rw-r--r--   0        0        0     1616 2023-08-01 22:36:16.727834 fixieai-1.0.2/fixieai/cli/agent/agent_config.py
+-rw-r--r--   0        0        0    36492 2023-08-01 22:36:16.728418 fixieai-1.0.2/fixieai/cli/agent/commands.py
+-rw-r--r--   0        0        0    16037 2023-08-01 22:36:16.728847 fixieai-1.0.2/fixieai/cli/agent/commands_test.py
+-rw-r--r--   0        0        0     3488 2023-08-01 22:36:16.729052 fixieai-1.0.2/fixieai/cli/agent/loader.py
+-rw-r--r--   0        0        0     1753 2023-04-28 22:19:21.473177 fixieai-1.0.2/fixieai/cli/agent/tunnel.py
+-rw-r--r--   0        0        0        0 2023-03-09 00:55:55.386842 fixieai-1.0.2/fixieai/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-28 22:19:21.473334 fixieai-1.0.2/fixieai/cli/auth/commands.py
+-rw-r--r--   0        0        0     1942 2023-03-09 00:55:55.387018 fixieai-1.0.2/fixieai/cli/auth/oauth_flow.py
+-rw-r--r--   0        0        0     2667 2023-03-30 02:57:14.483320 fixieai-1.0.2/fixieai/cli/auth/user_config.py
+-rw-r--r--   0        0        0     2120 2023-03-30 02:57:14.484045 fixieai-1.0.2/fixieai/cli/auth/user_config_test.py
+-rwxr-xr-x   0        0        0     3290 2023-08-01 22:36:16.729416 fixieai-1.0.2/fixieai/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-03-05 05:28:15.597413 fixieai-1.0.2/fixieai/cli/session/__init__.py
+-rw-r--r--   0        0        0     4761 2023-04-28 22:19:21.473661 fixieai-1.0.2/fixieai/cli/session/commands.py
+-rw-r--r--   0        0        0     4720 2023-08-01 22:36:16.729694 fixieai-1.0.2/fixieai/cli/session/console.py
+-rw-r--r--   0        0        0     1523 2023-03-30 02:57:14.484239 fixieai-1.0.2/fixieai/cli/utils.py
+-rw-r--r--   0        0        0      655 2023-03-23 17:48:13.070582 fixieai-1.0.2/fixieai/cli/utils_test.py
+-rw-r--r--   0        0        0      397 2023-08-01 22:36:16.729937 fixieai-1.0.2/fixieai/client/__init__.py
+-rw-r--r--   0        0        0    11895 2023-08-01 22:36:16.730272 fixieai-1.0.2/fixieai/client/agent.py
+-rwxr-xr-x   0        0        0    12849 2023-08-01 22:36:16.730796 fixieai-1.0.2/fixieai/client/client.py
+-rw-r--r--   0        0        0     4987 2023-03-10 06:52:38.294179 fixieai-1.0.2/fixieai/client/client_test.py
+-rwxr-xr-x   0        0        0     8750 2023-03-10 07:20:36.810915 fixieai-1.0.2/fixieai/client/session.py
+-rw-r--r--   0        0        0     1402 2023-08-01 22:36:16.730968 fixieai-1.0.2/fixieai/client/utils.py
+-rw-r--r--   0        0        0     2394 2023-08-01 22:36:16.731469 fixieai-1.0.2/fixieai/constants.py
+-rw-r--r--   0        0        0     2026 2023-08-01 22:37:06.436334 fixieai-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1241 1970-01-01 00:00:00.000000 fixieai-1.0.2/PKG-INFO
```

### Comparing `fixieai-1.0.1/LICENSE` & `fixieai-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/__init__.py` & `fixieai-1.0.2/fixieai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from fixieai.agents import Message
 from fixieai.agents import OAuthHandler
 from fixieai.agents import OAuthParams
 from fixieai.agents import StandaloneAgent
 from fixieai.agents import UrlDocumentCorpus
 from fixieai.agents import UserStorage
 from fixieai.client import FixieClient
+from fixieai.client import FixieEnvironment
 from fixieai.client import get_agents
 from fixieai.client import get_client
 from fixieai.client import get_embeds
 from fixieai.client import query
 
 __all__ = [
     "AgentQuery",
@@ -38,14 +39,15 @@
     "StandaloneAgent",
     "LlmSettings",
     "OAuthParams",
     "OAuthHandler",
     "UrlDocumentCorpus",
     "UserStorage",
     "FixieClient",
+    "FixieEnvironment",
     "get_agents",
     "get_client",
     "get_embeds",
     "query",
 ]
 
 __version__ = importlib.metadata.version(__name__)
```

### Comparing `fixieai-1.0.1/fixieai/agents/__init__.py` & `fixieai-1.0.2/fixieai/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/agent_base.py` & `fixieai-1.0.2/fixieai/agents/agent_base.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/agent_base_test.py` & `fixieai-1.0.2/fixieai/agents/agent_base_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/agent_func.py` & `fixieai-1.0.2/fixieai/agents/agent_func.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/agent_func_test.py` & `fixieai-1.0.2/fixieai/agents/agent_func_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/api.py` & `fixieai-1.0.2/fixieai/agents/api.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/api_test.py` & `fixieai-1.0.2/fixieai/agents/api_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/code_shot.py` & `fixieai-1.0.2/fixieai/agents/code_shot.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/code_shot_test.py` & `fixieai-1.0.2/fixieai/agents/code_shot_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/corpora.py` & `fixieai-1.0.2/fixieai/agents/corpora.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/corpora_test.py` & `fixieai-1.0.2/fixieai/agents/corpora_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/exceptions.py` & `fixieai-1.0.2/fixieai/agents/exceptions.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/llm_settings.py` & `fixieai-1.0.2/fixieai/agents/llm_settings.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/metadata.py` & `fixieai-1.0.2/fixieai/agents/metadata.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/oauth.py` & `fixieai-1.0.2/fixieai/agents/oauth.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/openai_proxy.py` & `fixieai-1.0.2/fixieai/agents/openai_proxy.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/openai_proxy_test.py` & `fixieai-1.0.2/fixieai/agents/openai_proxy_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/standalone.py` & `fixieai-1.0.2/fixieai/agents/standalone.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/standalone_test.py` & `fixieai-1.0.2/fixieai/agents/standalone_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/token.py` & `fixieai-1.0.2/fixieai/agents/token.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/user_storage.py` & `fixieai-1.0.2/fixieai/agents/user_storage.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/user_storage_test.py` & `fixieai-1.0.2/fixieai/agents/user_storage_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/utils.py` & `fixieai-1.0.2/fixieai/agents/utils.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/agents/utils_test.py` & `fixieai-1.0.2/fixieai/agents/utils_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/agent/agent_config.py` & `fixieai-1.0.2/fixieai/cli/agent/agent_config.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/agent/commands.py` & `fixieai-1.0.2/fixieai/cli/agent/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import contextlib
 import functools
 import io
+import json
 import os
 import pathlib
 import random
 import re
 import shlex
 import socket
 import subprocess
@@ -587,15 +588,14 @@
                 python_exe,
                 host,
                 port,
                 agent_env,
                 agent_dir,
                 startup_timeout_seconds=10.0,
             ) as popen:
-
                 # The server has started up, so we can replace the revision.
                 replace_revision(current_url)
 
                 while True:
                     if reload:
                         changed_file = _wait_for_agent_changes_or_event(
                             agent_dir, requires_action
@@ -678,15 +678,17 @@
     file_bytes = text.encode("utf-8")
     tarinfo = tarfile.TarInfo(path)
     tarinfo.size = len(file_bytes)
     tarball.addfile(tarinfo, io.BytesIO(file_bytes))
 
 
 @contextlib.contextmanager
-def _agent_code_package(agent_dir: str, agent_id: str, console: rich_console.Console):
+def _agent_py_code_package(
+    agent_dir: str, agent_id: str, console: rich_console.Console
+):
     """Yields a file-like code package that can be deployed to Fixie."""
 
     with tempfile.TemporaryFile() as tarball_file:
         with tarfile.open(fileobj=tarball_file, mode="w:gz") as tarball:
             tarball.add(
                 agent_dir,
                 arcname="agent",
@@ -707,14 +709,29 @@
                 tarball,
             )
 
         tarball_file.seek(0)
         yield tarball_file
 
 
+@contextlib.contextmanager
+def _agent_js_code_package(agent_dir: str):
+    agent_path = os.path.abspath(agent_dir)
+    with tempfile.TemporaryDirectory() as tarball_dir:
+        package_json_path = os.path.join(agent_path, "package.json")
+        with open(package_json_path) as package_json_file:
+            package_json = json.load(package_json_file)
+        tarball_path = os.path.join(
+            tarball_dir, f"{package_json['name']}-{package_json['version']}.tgz"
+        )
+        subprocess.check_call(["npm", "pack", agent_path], cwd=tarball_dir)
+        tarball_file = open(tarball_path, "rb")
+        yield tarball_file
+
+
 @agent.command("deploy", help="Deploy the current agent.")
 @click.argument("path", callback=_validate_agent_path, required=False)
 @click.option(
     "--metadata-only",
     is_flag=True,
     default=None,
     help="(No longer supported.)",
@@ -768,38 +785,54 @@
         config.public = True
 
     client: fixieai.FixieClient = ctx.obj.client
     agent_id = f"{client.get_current_username()}/{config.handle}"
     console.print(f"🦊 Deploying agent [green]{agent_id}[/]...")
 
     agent_dir = os.path.dirname(path) or "."
-    if validate:
+    package_json_path = os.path.join(agent_dir, "package.json")
+    is_js_agent = os.path.exists(package_json_path)
+    if validate and not is_js_agent:
         # Validate that the agent loads in a virtual environment before deploying.
         python_exe, agent_env = _configure_venv(console, agent_dir)
         agent_env[FIXIE_ALLOWED_AGENT_ID] = agent_id
         _validate_agent_loads_or_exit(
             console, agent_dir, config.handle, python_exe, agent_env
         )
 
     _ = _ensure_agent_updated(client, agent_id, config)
 
     metadata_dict = {**dict(metadata or []), **_cli_revision_metadata("deploy")}
 
     if config.deployment_url is None:
         # Deploy the code to Fixie.
-        with _agent_code_package(
-            agent_dir, agent_id, console
-        ) as tarball_file, _spinner(console, "Deploying..."):
-            revision_id = client.create_agent_revision(
-                config.handle,
-                make_current=make_current,
-                metadata=metadata_dict,
-                python_gzip_tarfile=tarball_file,
-                reindex_corpora=reindex,
-            )
+        if is_js_agent:
+            with _agent_js_code_package(agent_dir) as tarball_file, _spinner(
+                console, "Deploying..."
+            ):
+                revision_id = client.create_agent_revision(
+                    config.handle,
+                    make_current=make_current,
+                    metadata=metadata_dict,
+                    gzip_tarfile=tarball_file,
+                    reindex_corpora=reindex,
+                    environment=fixieai.client.FixieEnvironment.NODEJS,
+                )
+        else:
+            with _agent_py_code_package(
+                agent_dir, agent_id, console
+            ) as tarball_file, _spinner(console, "Deploying..."):
+                revision_id = client.create_agent_revision(
+                    config.handle,
+                    make_current=make_current,
+                    metadata=metadata_dict,
+                    gzip_tarfile=tarball_file,
+                    reindex_corpora=reindex,
+                    environment=fixieai.client.FixieEnvironment.PYTHON,
+                )
     else:
         # Create a new revision with the specified URL.
         with _spinner(console, "Deploying..."):
             revision_id = client.create_agent_revision(
                 config.handle,
                 make_current=make_current,
                 metadata=metadata_dict,
```

### Comparing `fixieai-1.0.1/fixieai/cli/agent/commands_test.py` & `fixieai-1.0.2/fixieai/cli/agent/commands_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/agent/loader.py` & `fixieai-1.0.2/fixieai/cli/agent/loader.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/agent/tunnel.py` & `fixieai-1.0.2/fixieai/cli/agent/tunnel.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/auth/commands.py` & `fixieai-1.0.2/fixieai/cli/auth/commands.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/auth/oauth_flow.py` & `fixieai-1.0.2/fixieai/cli/auth/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/auth/user_config.py` & `fixieai-1.0.2/fixieai/cli/auth/user_config.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/auth/user_config_test.py` & `fixieai-1.0.2/fixieai/cli/auth/user_config_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/cli.py` & `fixieai-1.0.2/fixieai/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/session/commands.py` & `fixieai-1.0.2/fixieai/cli/session/commands.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/session/console.py` & `fixieai-1.0.2/fixieai/cli/session/console.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/utils.py` & `fixieai-1.0.2/fixieai/cli/utils.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/cli/utils_test.py` & `fixieai-1.0.2/fixieai/cli/utils_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/client/agent.py` & `fixieai-1.0.2/fixieai/client/agent.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/client/client.py` & `fixieai-1.0.2/fixieai/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
 
+import enum
 import logging
 from typing import Any, BinaryIO, Dict, List, Optional
 
 import requests
 from gql import Client
 from gql import gql
 from gql.transport.requests import RequestsHTTPTransport
 
 from fixieai import constants
 from fixieai.client import utils
 from fixieai.client.agent import Agent
 from fixieai.client.session import Session
 
+
+class FixieEnvironment(enum.Enum):
+    PYTHON = "PYTHON"
+    NODEJS = "NODEJS"
+
+
 _CLIENT: Optional["FixieClient"] = None
 _SESSION: Optional[Session] = None
 
 
 def get_client() -> FixieClient:
     """Return the global FixieClient instance."""
     global _CLIENT
@@ -217,27 +224,29 @@
         self,
         handle: str,
         make_current: bool,
         *,
         reindex_corpora: bool = False,
         metadata: Optional[Dict[str, str]] = None,
         external_url: Optional[str] = None,
-        python_gzip_tarfile: Optional[BinaryIO] = None,
+        gzip_tarfile: Optional[BinaryIO] = None,
+        environment: FixieEnvironment = FixieEnvironment.PYTHON,
     ) -> str:
         """Creates a new Agent revision.
 
         Args:
             handle: The handle of the Agent. Must be owned by the current user.
             make_current: Whether the new revision should be made the current (active) revision.
             reindex_corpora: Whether to reindex all corpora for the new revision.
             metadata: Optional client-provided metadata to associate with the revision.
             external_url: The URL at which the revision is hosted, if hosted externally.
-            python_gzip_tarfile: A file-like of a gzip-compressed tarfile containing the files to deploy.
+            gzip_tarfile: A file-like of a gzip-compressed tarfile containing the files to deploy.
+            environment: The environment in which the revision should be run.
 
-        Exactly one of `external_url` and `python_gzip_tarfile` must be provided.
+        Exactly one of `external_url` and `gzip_tarfile` must be provided.
         """
 
         mutation = gql(
             """
             mutation CreateAgentRevision(
                 $handle: String!,
                 $metadata: [RevisionMetadataKeyValuePairInput!]!,
@@ -256,15 +265,15 @@
                     }
                 }
             }
             """
         )
 
         with utils.patched_gql_file_uploader(
-            python_gzip_tarfile, "upload.tar.gz", "application/gzip"
+            gzip_tarfile, "upload.tar.gz", "application/gzip"
         ):
             result = self._gqlclient.execute(
                 mutation,
                 variable_values={
                     "handle": handle,
                     "metadata": [
                         {"key": key, "value": value} for key, value in metadata.items()
@@ -273,18 +282,18 @@
                     else [],
                     "makeCurrent": make_current,
                     "reindexCorpora": reindex_corpora,
                     "externalDeployment": {"url": external_url}
                     if external_url
                     else None,
                     "managedDeployment": {
-                        "environment": "PYTHON",
-                        "codePackage": python_gzip_tarfile,
+                        "environment": environment,
+                        "codePackage": gzip_tarfile,
                     }
-                    if python_gzip_tarfile
+                    if gzip_tarfile
                     else None,
                 },
                 upload_files=True,
             )
 
         revision_id = result["createAgentRevision"]["revision"]["id"]
         assert isinstance(revision_id, str)
@@ -355,22 +364,21 @@
             """
         )
         _ = self._gqlclient.execute(
             mutation, variable_values={"handle": handle, "revisionId": revision_id}
         )
 
     def deploy_agent(
-        self,
-        handle: str,
-        gzip_tarfile: BinaryIO,
+        self, handle: str, gzip_tarfile: BinaryIO, environment: FixieEnvironment
     ):
         """Deploys an agent implementation.
 
         Args:
             handle: The handle of the Agent to deploy. Must be owned by the current user.
             gzip_tarfile: A file-like of a gzip-compressed tarfile containing the files to deploy.
         """
         return self.create_agent_revision(
             handle,
             make_current=True,
-            python_gzip_tarfile=gzip_tarfile,
+            gzip_tarfile=gzip_tarfile,
+            environment=environment,
         )
```

### Comparing `fixieai-1.0.1/fixieai/client/client_test.py` & `fixieai-1.0.2/fixieai/client/client_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/client/session.py` & `fixieai-1.0.2/fixieai/client/session.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/client/utils.py` & `fixieai-1.0.2/fixieai/client/utils.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/fixieai/constants.py` & `fixieai-1.0.2/fixieai/constants.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.1/pyproject.toml` & `fixieai-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fixieai"
-version = "1.0.1"
+version = "1.0.2"
 description = "SDK for the Fixie.ai platform. See: https://fixie.ai"
 authors = ["Fixie.ai Team <hello@fixie.ai>"]
 packages = [
     { include = "fixieai/" },
 ]
 
 [build-system]
```

### Comparing `fixieai-1.0.1/PKG-INFO` & `fixieai-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: fixieai
-Version: 1.0.1
+Version: 1.0.2
 Summary: SDK for the Fixie.ai platform. See: https://fixie.ai
 Author: Fixie.ai Team
 Author-email: hello@fixie.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: Pillow
 Requires-Dist: PyJWT[crypto] (>=2.6.0,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: fastapi (>=0.89.1,<0.90.0)
 Requires-Dist: gql[requests] (>=3.4.1,<4.0.0)
```

