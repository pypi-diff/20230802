# Comparing `tmp/flow-agent-package-0.0.7.tar.gz` & `tmp/flow-agent-package-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow-agent-package-0.0.7.tar", last modified: Wed Aug  2 20:46:23 2023, max compression
+gzip compressed data, was "flow-agent-package-0.0.8.tar", last modified: Wed Aug  2 20:57:52 2023, max compression
```

## Comparing `flow-agent-package-0.0.7.tar` & `flow-agent-package-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 20:46:23.459340 flow-agent-package-0.0.7/
--rw-rw-rw-   0        0        0       39 2023-08-02 16:07:21.000000 flow-agent-package-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      106 2023-08-02 20:46:23.457342 flow-agent-package-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 flow-agent-package-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 20:46:23.327193 flow-agent-package-0.0.7/flow_agent_package/
--rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 flow-agent-package-0.0.7/flow_agent_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:46:23.418748 flow-agent-package-0.0.7/flow_agent_package/tools/
--rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 flow-agent-package-0.0.7/flow_agent_package/tools/__init__.py
--rw-rw-rw-   0        0        0     6502 2023-08-02 18:48:29.000000 flow-agent-package-0.0.7/flow_agent_package/tools/agent_tool.py
--rw-rw-rw-   0        0        0     3582 2023-08-02 20:45:32.000000 flow-agent-package-0.0.7/flow_agent_package/tools/get_flow_tool.py
--rw-rw-rw-   0        0        0      784 2023-08-02 19:56:57.000000 flow-agent-package-0.0.7/flow_agent_package/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:46:23.444306 flow-agent-package-0.0.7/flow_agent_package/yamls/
--rw-rw-rw-   0        0        0      520 2023-08-02 20:32:04.000000 flow-agent-package-0.0.7/flow_agent_package/yamls/agent_tool.yaml
--rw-rw-rw-   0        0        0      407 2023-08-02 20:31:48.000000 flow-agent-package-0.0.7/flow_agent_package/yamls/get_flow_tool.yaml
-drwxrwxrwx   0        0        0        0 2023-08-02 20:46:23.351630 flow-agent-package-0.0.7/flow_agent_package.egg-info/
--rw-rw-rw-   0        0        0      106 2023-08-02 20:46:23.000000 flow-agent-package-0.0.7/flow_agent_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-08-02 20:46:23.000000 flow-agent-package-0.0.7/flow_agent_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 20:46:23.000000 flow-agent-package-0.0.7/flow_agent_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-08-02 20:46:23.000000 flow-agent-package-0.0.7/flow_agent_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-08-02 20:46:23.000000 flow-agent-package-0.0.7/flow_agent_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 20:46:23.459340 flow-agent-package-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-08-02 20:46:13.000000 flow-agent-package-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:46:23.452825 flow-agent-package-0.0.7/tests/
--rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 flow-agent-package-0.0.7/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:57:52.263958 flow-agent-package-0.0.8/
+-rw-rw-rw-   0        0        0       39 2023-08-02 16:07:21.000000 flow-agent-package-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      106 2023-08-02 20:57:52.262452 flow-agent-package-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 flow-agent-package-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 20:57:52.212789 flow-agent-package-0.0.8/flow_agent_package/
+-rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 flow-agent-package-0.0.8/flow_agent_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:57:52.252932 flow-agent-package-0.0.8/flow_agent_package/tools/
+-rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 flow-agent-package-0.0.8/flow_agent_package/tools/__init__.py
+-rw-rw-rw-   0        0        0     6379 2023-08-02 20:57:13.000000 flow-agent-package-0.0.8/flow_agent_package/tools/agent_tool.py
+-rw-rw-rw-   0        0        0     3582 2023-08-02 20:45:32.000000 flow-agent-package-0.0.8/flow_agent_package/tools/get_flow_tool.py
+-rw-rw-rw-   0        0        0      784 2023-08-02 19:56:57.000000 flow-agent-package-0.0.8/flow_agent_package/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:57:52.258452 flow-agent-package-0.0.8/flow_agent_package/yamls/
+-rw-rw-rw-   0        0        0      520 2023-08-02 20:32:04.000000 flow-agent-package-0.0.8/flow_agent_package/yamls/agent_tool.yaml
+-rw-rw-rw-   0        0        0      407 2023-08-02 20:31:48.000000 flow-agent-package-0.0.8/flow_agent_package/yamls/get_flow_tool.yaml
+drwxrwxrwx   0        0        0        0 2023-08-02 20:57:52.235400 flow-agent-package-0.0.8/flow_agent_package.egg-info/
+-rw-rw-rw-   0        0        0      106 2023-08-02 20:57:52.000000 flow-agent-package-0.0.8/flow_agent_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-08-02 20:57:52.000000 flow-agent-package-0.0.8/flow_agent_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 20:57:52.000000 flow-agent-package-0.0.8/flow_agent_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-08-02 20:57:52.000000 flow-agent-package-0.0.8/flow_agent_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-08-02 20:57:52.000000 flow-agent-package-0.0.8/flow_agent_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 20:57:52.263958 flow-agent-package-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-08-02 20:57:48.000000 flow-agent-package-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:57:52.261451 flow-agent-package-0.0.8/tests/
+-rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 flow-agent-package-0.0.8/tests/test_my_tool_1.py
```

### Comparing `flow-agent-package-0.0.7/README.md` & `flow-agent-package-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.7/flow_agent_package/tools/agent_tool.py` & `flow-agent-package-0.0.8/flow_agent_package/tools/agent_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,20 @@
 from datetime import datetime
 from pathlib import Path
 from tempfile import mkdtemp
 from typing import Dict, List, Union
 
 from promptflow.contracts.run_mode import RunMode
 from promptflow.runtime.contracts.runtime import SubmitFlowRequest
-from promptflow.executor import FlowExecutionCoodinator  # noqa: E402
 from flow_agent_package.tools.utils import AgentToolConfiguration
 
 from promptflow import ToolProvider, tool
 from promptflow.core.tools_manager import register_builtin_method, register_apis
 from promptflow.runtime import PromptFlowRuntime
 from promptflow.core.thread_local_singleton import ThreadLocalSingleton
-from langchain import LLMMathChain, SerpAPIWrapper
 from langchain.agents import Tool
 from langchain.agents import AgentType, initialize_agent
 from langchain.chat_models import AzureChatOpenAI
 import os
 import urllib.request
 import urllib.error
 import json
```

### Comparing `flow-agent-package-0.0.7/flow_agent_package/tools/get_flow_tool.py` & `flow-agent-package-0.0.8/flow_agent_package/tools/get_flow_tool.py`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.7/flow_agent_package/tools/utils.py` & `flow-agent-package-0.0.8/flow_agent_package/tools/utils.py`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.7/flow_agent_package/yamls/agent_tool.yaml` & `flow-agent-package-0.0.8/flow_agent_package/yamls/agent_tool.yaml`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.7/flow_agent_package.egg-info/SOURCES.txt` & `flow-agent-package-0.0.8/flow_agent_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

