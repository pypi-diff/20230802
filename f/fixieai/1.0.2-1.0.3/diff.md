# Comparing `tmp/fixieai-1.0.2.tar.gz` & `tmp/fixieai-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixieai-1.0.2.tar", max compression
+gzip compressed data, was "fixieai-1.0.3.tar", max compression
```

## Comparing `fixieai-1.0.2.tar` & `fixieai-1.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    11357 2023-01-18 21:21:47.580356 fixieai-1.0.2/LICENSE
--rw-r--r--   0        0        0     1456 2023-08-01 22:36:16.720638 fixieai-1.0.2/fixieai/__init__.py
--rw-r--r--   0        0        0     1301 2023-08-01 22:36:16.721137 fixieai-1.0.2/fixieai/agents/__init__.py
--rw-r--r--   0        0        0    10564 2023-08-01 22:36:16.721458 fixieai-1.0.2/fixieai/agents/agent_base.py
--rw-r--r--   0        0        0    12042 2023-08-01 22:36:16.721808 fixieai-1.0.2/fixieai/agents/agent_base_test.py
--rw-r--r--   0        0        0    15267 2023-08-01 22:36:16.722088 fixieai-1.0.2/fixieai/agents/agent_func.py
--rw-r--r--   0        0        0     8715 2023-08-01 22:36:16.722561 fixieai-1.0.2/fixieai/agents/agent_func_test.py
--rw-r--r--   0        0        0     2965 2023-08-01 22:36:16.723036 fixieai-1.0.2/fixieai/agents/api.py
--rw-r--r--   0        0        0      863 2023-03-07 19:11:26.788937 fixieai-1.0.2/fixieai/agents/api_test.py
--rw-r--r--   0        0        0     3786 2023-08-01 22:36:16.723341 fixieai-1.0.2/fixieai/agents/code_shot.py
--rw-r--r--   0        0        0     3306 2023-08-01 22:36:16.723647 fixieai-1.0.2/fixieai/agents/code_shot_test.py
--rw-r--r--   0        0        0     7152 2023-08-01 22:36:16.723851 fixieai-1.0.2/fixieai/agents/corpora.py
--rw-r--r--   0        0        0     1943 2023-08-01 22:36:16.724099 fixieai-1.0.2/fixieai/agents/corpora_test.py
--rw-r--r--   0        0        0     2279 2023-08-01 22:36:16.724302 fixieai-1.0.2/fixieai/agents/exceptions.py
--rw-r--r--   0        0        0     1046 2023-04-28 22:19:21.471721 fixieai-1.0.2/fixieai/agents/llm_settings.py
--rw-r--r--   0        0        0      891 2023-08-01 22:36:16.724477 fixieai-1.0.2/fixieai/agents/metadata.py
--rw-r--r--   0        0        0     9000 2023-08-01 22:36:16.724791 fixieai-1.0.2/fixieai/agents/oauth.py
--rw-r--r--   0        0        0     4048 2023-08-01 22:36:16.725207 fixieai-1.0.2/fixieai/agents/openai_proxy.py
--rw-r--r--   0        0        0     1627 2023-08-01 22:36:16.725754 fixieai-1.0.2/fixieai/agents/openai_proxy_test.py
--rw-r--r--   0        0        0     2439 2023-08-01 22:36:16.726056 fixieai-1.0.2/fixieai/agents/standalone.py
--rw-r--r--   0        0        0     4414 2023-08-01 22:36:16.726252 fixieai-1.0.2/fixieai/agents/standalone_test.py
--rw-r--r--   0        0        0     1918 2023-08-01 22:36:16.726392 fixieai-1.0.2/fixieai/agents/token.py
--rw-r--r--   0        0        0     4951 2023-08-01 22:36:16.726565 fixieai-1.0.2/fixieai/agents/user_storage.py
--rw-r--r--   0        0        0     3388 2023-08-01 22:36:16.726979 fixieai-1.0.2/fixieai/agents/user_storage_test.py
--rw-r--r--   0        0        0     7966 2023-08-01 22:36:16.727450 fixieai-1.0.2/fixieai/agents/utils.py
--rw-r--r--   0        0        0     5253 2023-03-23 20:13:08.313763 fixieai-1.0.2/fixieai/agents/utils_test.py
--rw-r--r--   0        0        0        0 2023-03-05 05:28:15.595965 fixieai-1.0.2/fixieai/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-05 05:28:15.596298 fixieai-1.0.2/fixieai/cli/agent/__init__.py
--rw-r--r--   0        0        0     1616 2023-08-01 22:36:16.727834 fixieai-1.0.2/fixieai/cli/agent/agent_config.py
--rw-r--r--   0        0        0    36492 2023-08-01 22:36:16.728418 fixieai-1.0.2/fixieai/cli/agent/commands.py
--rw-r--r--   0        0        0    16037 2023-08-01 22:36:16.728847 fixieai-1.0.2/fixieai/cli/agent/commands_test.py
--rw-r--r--   0        0        0     3488 2023-08-01 22:36:16.729052 fixieai-1.0.2/fixieai/cli/agent/loader.py
--rw-r--r--   0        0        0     1753 2023-04-28 22:19:21.473177 fixieai-1.0.2/fixieai/cli/agent/tunnel.py
--rw-r--r--   0        0        0        0 2023-03-09 00:55:55.386842 fixieai-1.0.2/fixieai/cli/auth/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-28 22:19:21.473334 fixieai-1.0.2/fixieai/cli/auth/commands.py
--rw-r--r--   0        0        0     1942 2023-03-09 00:55:55.387018 fixieai-1.0.2/fixieai/cli/auth/oauth_flow.py
--rw-r--r--   0        0        0     2667 2023-03-30 02:57:14.483320 fixieai-1.0.2/fixieai/cli/auth/user_config.py
--rw-r--r--   0        0        0     2120 2023-03-30 02:57:14.484045 fixieai-1.0.2/fixieai/cli/auth/user_config_test.py
--rwxr-xr-x   0        0        0     3290 2023-08-01 22:36:16.729416 fixieai-1.0.2/fixieai/cli/cli.py
--rw-r--r--   0        0        0        0 2023-03-05 05:28:15.597413 fixieai-1.0.2/fixieai/cli/session/__init__.py
--rw-r--r--   0        0        0     4761 2023-04-28 22:19:21.473661 fixieai-1.0.2/fixieai/cli/session/commands.py
--rw-r--r--   0        0        0     4720 2023-08-01 22:36:16.729694 fixieai-1.0.2/fixieai/cli/session/console.py
--rw-r--r--   0        0        0     1523 2023-03-30 02:57:14.484239 fixieai-1.0.2/fixieai/cli/utils.py
--rw-r--r--   0        0        0      655 2023-03-23 17:48:13.070582 fixieai-1.0.2/fixieai/cli/utils_test.py
--rw-r--r--   0        0        0      397 2023-08-01 22:36:16.729937 fixieai-1.0.2/fixieai/client/__init__.py
--rw-r--r--   0        0        0    11895 2023-08-01 22:36:16.730272 fixieai-1.0.2/fixieai/client/agent.py
--rwxr-xr-x   0        0        0    12849 2023-08-01 22:36:16.730796 fixieai-1.0.2/fixieai/client/client.py
--rw-r--r--   0        0        0     4987 2023-03-10 06:52:38.294179 fixieai-1.0.2/fixieai/client/client_test.py
--rwxr-xr-x   0        0        0     8750 2023-03-10 07:20:36.810915 fixieai-1.0.2/fixieai/client/session.py
--rw-r--r--   0        0        0     1402 2023-08-01 22:36:16.730968 fixieai-1.0.2/fixieai/client/utils.py
--rw-r--r--   0        0        0     2394 2023-08-01 22:36:16.731469 fixieai-1.0.2/fixieai/constants.py
--rw-r--r--   0        0        0     2026 2023-08-01 22:37:06.436334 fixieai-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1241 1970-01-01 00:00:00.000000 fixieai-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-07 23:45:43.683245 fixieai-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1456 2023-08-02 18:07:05.054190 fixieai-1.0.3/fixieai/__init__.py
+-rw-r--r--   0        0        0     1301 2023-06-05 22:24:43.848729 fixieai-1.0.3/fixieai/agents/__init__.py
+-rw-r--r--   0        0        0    10564 2023-06-05 22:24:43.849458 fixieai-1.0.3/fixieai/agents/agent_base.py
+-rw-r--r--   0        0        0    12042 2023-06-05 22:24:43.849590 fixieai-1.0.3/fixieai/agents/agent_base_test.py
+-rw-r--r--   0        0        0    15267 2023-06-05 22:24:43.849720 fixieai-1.0.3/fixieai/agents/agent_func.py
+-rw-r--r--   0        0        0     8715 2023-06-05 22:24:43.849847 fixieai-1.0.3/fixieai/agents/agent_func_test.py
+-rw-r--r--   0        0        0     2965 2023-06-05 22:24:43.849947 fixieai-1.0.3/fixieai/agents/api.py
+-rw-r--r--   0        0        0      863 2023-03-09 19:26:37.964207 fixieai-1.0.3/fixieai/agents/api_test.py
+-rw-r--r--   0        0        0     3786 2023-06-05 22:24:43.850060 fixieai-1.0.3/fixieai/agents/code_shot.py
+-rw-r--r--   0        0        0     3306 2023-06-05 22:24:43.850149 fixieai-1.0.3/fixieai/agents/code_shot_test.py
+-rw-r--r--   0        0        0     7152 2023-06-05 22:24:43.850261 fixieai-1.0.3/fixieai/agents/corpora.py
+-rw-r--r--   0        0        0     1943 2023-06-05 22:24:43.850315 fixieai-1.0.3/fixieai/agents/corpora_test.py
+-rw-r--r--   0        0        0     2279 2023-06-05 22:24:43.850379 fixieai-1.0.3/fixieai/agents/exceptions.py
+-rw-r--r--   0        0        0     1046 2023-03-30 16:24:35.974599 fixieai-1.0.3/fixieai/agents/llm_settings.py
+-rw-r--r--   0        0        0      891 2023-06-05 22:24:43.850459 fixieai-1.0.3/fixieai/agents/metadata.py
+-rw-r--r--   0        0        0     9000 2023-06-05 22:24:43.850566 fixieai-1.0.3/fixieai/agents/oauth.py
+-rw-r--r--   0        0        0     4048 2023-04-25 03:00:21.707100 fixieai-1.0.3/fixieai/agents/openai_proxy.py
+-rw-r--r--   0        0        0     1627 2023-04-25 03:00:21.707249 fixieai-1.0.3/fixieai/agents/openai_proxy_test.py
+-rw-r--r--   0        0        0     2439 2023-06-05 22:24:43.850673 fixieai-1.0.3/fixieai/agents/standalone.py
+-rw-r--r--   0        0        0     4414 2023-06-05 22:24:43.850780 fixieai-1.0.3/fixieai/agents/standalone_test.py
+-rw-r--r--   0        0        0     1918 2023-06-05 22:24:43.850853 fixieai-1.0.3/fixieai/agents/token.py
+-rw-r--r--   0        0        0     4951 2023-06-05 22:24:43.850975 fixieai-1.0.3/fixieai/agents/user_storage.py
+-rw-r--r--   0        0        0     3388 2023-06-05 22:24:43.851664 fixieai-1.0.3/fixieai/agents/user_storage_test.py
+-rw-r--r--   0        0        0     7966 2023-04-25 03:00:21.707832 fixieai-1.0.3/fixieai/agents/utils.py
+-rw-r--r--   0        0        0     5253 2023-03-25 02:35:27.951289 fixieai-1.0.3/fixieai/agents/utils_test.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:26:37.965971 fixieai-1.0.3/fixieai/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:26:37.966917 fixieai-1.0.3/fixieai/cli/agent/__init__.py
+-rw-r--r--   0        0        0     1616 2023-06-05 22:24:43.852159 fixieai-1.0.3/fixieai/cli/agent/agent_config.py
+-rw-r--r--   0        0        0    36492 2023-08-02 18:07:05.054626 fixieai-1.0.3/fixieai/cli/agent/commands.py
+-rw-r--r--   0        0        0    16037 2023-06-13 15:44:25.677117 fixieai-1.0.3/fixieai/cli/agent/commands_test.py
+-rw-r--r--   0        0        0     3488 2023-06-05 22:24:43.852973 fixieai-1.0.3/fixieai/cli/agent/loader.py
+-rw-r--r--   0        0        0     1753 2023-08-02 18:07:01.662520 fixieai-1.0.3/fixieai/cli/agent/tunnel.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:26:37.967623 fixieai-1.0.3/fixieai/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-01 23:07:48.256193 fixieai-1.0.3/fixieai/cli/auth/commands.py
+-rw-r--r--   0        0        0     1942 2023-03-09 19:26:37.968039 fixieai-1.0.3/fixieai/cli/auth/oauth_flow.py
+-rw-r--r--   0        0        0     2667 2023-03-30 16:24:35.975821 fixieai-1.0.3/fixieai/cli/auth/user_config.py
+-rw-r--r--   0        0        0     2120 2023-03-30 16:24:35.975913 fixieai-1.0.3/fixieai/cli/auth/user_config_test.py
+-rwxr-xr-x   0        0        0     3290 2023-04-12 15:22:13.299089 fixieai-1.0.3/fixieai/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:26:37.968257 fixieai-1.0.3/fixieai/cli/session/__init__.py
+-rw-r--r--   0        0        0     4761 2023-04-12 01:22:58.394077 fixieai-1.0.3/fixieai/cli/session/commands.py
+-rw-r--r--   0        0        0     4720 2023-06-05 22:24:43.853234 fixieai-1.0.3/fixieai/cli/session/console.py
+-rw-r--r--   0        0        0     1523 2023-03-30 16:24:35.976029 fixieai-1.0.3/fixieai/cli/utils.py
+-rw-r--r--   0        0        0      655 2023-03-22 17:59:48.856855 fixieai-1.0.3/fixieai/cli/utils_test.py
+-rw-r--r--   0        0        0      397 2023-08-02 18:07:05.055211 fixieai-1.0.3/fixieai/client/__init__.py
+-rw-r--r--   0        0        0    11895 2023-06-13 15:44:25.677595 fixieai-1.0.3/fixieai/client/agent.py
+-rwxr-xr-x   0        0        0    12854 2023-08-02 18:07:24.238360 fixieai-1.0.3/fixieai/client/client.py
+-rw-r--r--   0        0        0     4987 2023-03-10 17:44:40.327464 fixieai-1.0.3/fixieai/client/client_test.py
+-rwxr-xr-x   0        0        0     8750 2023-03-10 05:45:43.499628 fixieai-1.0.3/fixieai/client/session.py
+-rw-r--r--   0        0        0     1402 2023-06-05 22:24:43.853545 fixieai-1.0.3/fixieai/client/utils.py
+-rw-r--r--   0        0        0     2394 2023-06-05 22:24:43.853647 fixieai-1.0.3/fixieai/constants.py
+-rw-r--r--   0        0        0     2026 2023-08-02 18:07:36.470235 fixieai-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1241 1970-01-01 00:00:00.000000 fixieai-1.0.3/PKG-INFO
```

### Comparing `fixieai-1.0.2/LICENSE` & `fixieai-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/__init__.py` & `fixieai-1.0.3/fixieai/__init__.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/__init__.py` & `fixieai-1.0.3/fixieai/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/agent_base.py` & `fixieai-1.0.3/fixieai/agents/agent_base.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/agent_base_test.py` & `fixieai-1.0.3/fixieai/agents/agent_base_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/agent_func.py` & `fixieai-1.0.3/fixieai/agents/agent_func.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/agent_func_test.py` & `fixieai-1.0.3/fixieai/agents/agent_func_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/api.py` & `fixieai-1.0.3/fixieai/agents/api.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/api_test.py` & `fixieai-1.0.3/fixieai/agents/api_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/code_shot.py` & `fixieai-1.0.3/fixieai/agents/code_shot.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/code_shot_test.py` & `fixieai-1.0.3/fixieai/agents/code_shot_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/corpora.py` & `fixieai-1.0.3/fixieai/agents/corpora.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/corpora_test.py` & `fixieai-1.0.3/fixieai/agents/corpora_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/exceptions.py` & `fixieai-1.0.3/fixieai/agents/exceptions.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/llm_settings.py` & `fixieai-1.0.3/fixieai/agents/llm_settings.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/metadata.py` & `fixieai-1.0.3/fixieai/agents/metadata.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/oauth.py` & `fixieai-1.0.3/fixieai/agents/oauth.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/openai_proxy.py` & `fixieai-1.0.3/fixieai/agents/openai_proxy.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/openai_proxy_test.py` & `fixieai-1.0.3/fixieai/agents/openai_proxy_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/standalone.py` & `fixieai-1.0.3/fixieai/agents/standalone.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/standalone_test.py` & `fixieai-1.0.3/fixieai/agents/standalone_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/token.py` & `fixieai-1.0.3/fixieai/agents/token.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/user_storage.py` & `fixieai-1.0.3/fixieai/agents/user_storage.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/user_storage_test.py` & `fixieai-1.0.3/fixieai/agents/user_storage_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/utils.py` & `fixieai-1.0.3/fixieai/agents/utils.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/agents/utils_test.py` & `fixieai-1.0.3/fixieai/agents/utils_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/agent/agent_config.py` & `fixieai-1.0.3/fixieai/cli/agent/agent_config.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/agent/commands.py` & `fixieai-1.0.3/fixieai/cli/agent/commands.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/agent/commands_test.py` & `fixieai-1.0.3/fixieai/cli/agent/commands_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/agent/loader.py` & `fixieai-1.0.3/fixieai/cli/agent/loader.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/agent/tunnel.py` & `fixieai-1.0.3/fixieai/cli/agent/tunnel.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/auth/commands.py` & `fixieai-1.0.3/fixieai/cli/auth/commands.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/auth/oauth_flow.py` & `fixieai-1.0.3/fixieai/cli/auth/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/auth/user_config.py` & `fixieai-1.0.3/fixieai/cli/auth/user_config.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/auth/user_config_test.py` & `fixieai-1.0.3/fixieai/cli/auth/user_config_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/cli.py` & `fixieai-1.0.3/fixieai/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/session/commands.py` & `fixieai-1.0.3/fixieai/cli/session/commands.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/session/console.py` & `fixieai-1.0.3/fixieai/cli/session/console.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/utils.py` & `fixieai-1.0.3/fixieai/cli/utils.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/cli/utils_test.py` & `fixieai-1.0.3/fixieai/cli/utils_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/client/agent.py` & `fixieai-1.0.3/fixieai/client/agent.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/client/client.py` & `fixieai-1.0.3/fixieai/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from fixieai import constants
 from fixieai.client import utils
 from fixieai.client.agent import Agent
 from fixieai.client.session import Session
 
 
-class FixieEnvironment(enum.Enum):
+class FixieEnvironment(str, enum.Enum):
     PYTHON = "PYTHON"
     NODEJS = "NODEJS"
 
 
 _CLIENT: Optional["FixieClient"] = None
 _SESSION: Optional[Session] = None
```

### Comparing `fixieai-1.0.2/fixieai/client/client_test.py` & `fixieai-1.0.3/fixieai/client/client_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/client/session.py` & `fixieai-1.0.3/fixieai/client/session.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/client/utils.py` & `fixieai-1.0.3/fixieai/client/utils.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/fixieai/constants.py` & `fixieai-1.0.3/fixieai/constants.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.2/pyproject.toml` & `fixieai-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fixieai"
-version = "1.0.2"
+version = "1.0.3"
 description = "SDK for the Fixie.ai platform. See: https://fixie.ai"
 authors = ["Fixie.ai Team <hello@fixie.ai>"]
 packages = [
     { include = "fixieai/" },
 ]
 
 [build-system]
```

### Comparing `fixieai-1.0.2/PKG-INFO` & `fixieai-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixieai
-Version: 1.0.2
+Version: 1.0.3
 Summary: SDK for the Fixie.ai platform. See: https://fixie.ai
 Author: Fixie.ai Team
 Author-email: hello@fixie.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

