# Comparing `tmp/agentware-0.1.4.tar.gz` & `tmp/agentware-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/agentware-0.1.4.tar", last modified: Fri Jul 14 09:48:37 2023, max compression
+gzip compressed data, was "dist/agentware-0.1.5.tar", last modified: Wed Aug  2 05:58:33 2023, max compression
```

## Comparing `agentware-0.1.4.tar` & `agentware-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.269218 agentware-0.1.4/
--rw-r--r--   0 weiduan    (501) staff       (20)      221 2023-07-14 09:48:37.268511 agentware-0.1.4/PKG-INFO
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.252893 agentware-0.1.4/agentware/
--rw-r--r--   0 weiduan    (501) staff       (20)      168 2023-07-12 13:20:22.000000 agentware-0.1.4/agentware/__init__.py
--rw-r--r--   0 weiduan    (501) staff       (20)     4439 2023-07-13 10:10:58.000000 agentware-0.1.4/agentware/agent.py
--rw-r--r--   0 weiduan    (501) staff       (20)     1799 2023-07-10 15:16:08.000000 agentware-0.1.4/agentware/agent_logger.py
--rw-r--r--   0 weiduan    (501) staff       (20)    23058 2023-07-13 12:23:05.000000 agentware-0.1.4/agentware/base.py
--rw-r--r--   0 weiduan    (501) staff       (20)      224 2023-07-13 12:26:26.000000 agentware-0.1.4/agentware/error_codes.py
--rw-r--r--   0 weiduan    (501) staff       (20)      250 2023-07-12 14:52:41.000000 agentware-0.1.4/agentware/hub.py
--rw-r--r--   0 weiduan    (501) staff       (20)    13831 2023-07-13 12:05:53.000000 agentware-0.1.4/agentware/memory.py
--rw-r--r--   0 weiduan    (501) staff       (20)      225 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/singleton.py
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.256797 agentware-0.1.4/agentware/utils/
--rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-14 05:21:12.000000 agentware-0.1.4/agentware/utils/__init__.py
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.262251 agentware-0.1.4/agentware/utils/json_fixes/
--rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/utils/json_fixes/__init__.py
--rw-r--r--   0 weiduan    (501) staff       (20)     2268 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/utils/json_fixes/auto_fix.py
--rw-r--r--   0 weiduan    (501) staff       (20)      800 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/utils/json_fixes/bracket_termination.py
--rw-r--r--   0 weiduan    (501) staff       (20)     1052 2023-07-10 15:16:07.000000 agentware-0.1.4/agentware/utils/json_fixes/escaping.py
--rw-r--r--   0 weiduan    (501) staff       (20)      795 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/utils/json_fixes/master_json_fix_method.py
--rw-r--r--   0 weiduan    (501) staff       (20)      674 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/utils/json_fixes/missing_quotes.py
--rw-r--r--   0 weiduan    (501) staff       (20)     6003 2023-07-14 09:47:09.000000 agentware-0.1.4/agentware/utils/json_fixes/parsing.py
--rw-r--r--   0 weiduan    (501) staff       (20)      565 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/utils/json_fixes/utilities.py
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.263733 agentware-0.1.4/agentware/utils/json_validation/
--rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-14 09:17:54.000000 agentware-0.1.4/agentware/utils/json_validation/__init__.py
--rw-r--r--   0 weiduan    (501) staff       (20)     1071 2023-07-10 15:16:07.000000 agentware-0.1.4/agentware/utils/json_validation/validate_json.py
--rw-r--r--   0 weiduan    (501) staff       (20)     2255 2023-07-10 15:16:07.000000 agentware-0.1.4/agentware/utils/num_token_utils.py
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.255812 agentware-0.1.4/agentware.egg-info/
--rw-r--r--   0 weiduan    (501) staff       (20)      221 2023-07-14 09:48:37.000000 agentware-0.1.4/agentware.egg-info/PKG-INFO
--rw-r--r--   0 weiduan    (501) staff       (20)      939 2023-07-14 09:48:37.000000 agentware-0.1.4/agentware.egg-info/SOURCES.txt
--rw-r--r--   0 weiduan    (501) staff       (20)        1 2023-07-14 09:48:37.000000 agentware-0.1.4/agentware.egg-info/dependency_links.txt
--rw-r--r--   0 weiduan    (501) staff       (20)       43 2023-07-14 09:48:37.000000 agentware-0.1.4/agentware.egg-info/requires.txt
--rw-r--r--   0 weiduan    (501) staff       (20)       16 2023-07-14 09:48:37.000000 agentware-0.1.4/agentware.egg-info/top_level.txt
--rw-r--r--   0 weiduan    (501) staff       (20)       38 2023-07-14 09:48:37.269381 agentware-0.1.4/setup.cfg
--rw-r--r--   0 weiduan    (501) staff       (20)      467 2023-07-14 09:48:34.000000 agentware-0.1.4/setup.py
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.267492 agentware-0.1.4/tests/
--rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-12 09:22:40.000000 agentware-0.1.4/tests/__init__.py
--rw-r--r--   0 weiduan    (501) staff       (20)     1819 2023-07-13 10:12:38.000000 agentware-0.1.4/tests/agent_test.py
--rw-r--r--   0 weiduan    (501) staff       (20)      549 2023-07-10 15:16:07.000000 agentware-0.1.4/tests/connector_test.py
--rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-10 14:52:15.000000 agentware-0.1.4/tests/memory_test.py
--rw-r--r--   0 weiduan    (501) staff       (20)      281 2023-07-12 14:42:06.000000 agentware-0.1.4/tests/utils.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-08-02 05:58:33.919923 agentware-0.1.5/
+-rw-r--r--   0 weiduan    (501) staff       (20)      221 2023-08-02 05:58:33.918943 agentware-0.1.5/PKG-INFO
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-08-02 05:58:33.889627 agentware-0.1.5/agentware/
+-rw-r--r--   0 weiduan    (501) staff       (20)      291 2023-07-26 17:18:40.000000 agentware-0.1.5/agentware/__init__.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     4657 2023-08-02 05:33:13.000000 agentware-0.1.5/agentware/agent.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     1799 2023-07-10 15:16:08.000000 agentware-0.1.5/agentware/agent_logger.py
+-rw-r--r--   0 weiduan    (501) staff       (20)    26764 2023-07-28 01:31:24.000000 agentware-0.1.5/agentware/base.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     1217 2023-07-24 03:31:11.000000 agentware-0.1.5/agentware/core_engines.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      224 2023-07-13 12:26:26.000000 agentware-0.1.5/agentware/error_codes.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      250 2023-07-12 14:52:41.000000 agentware-0.1.5/agentware/hub.py
+-rw-r--r--   0 weiduan    (501) staff       (20)    14900 2023-07-28 01:58:19.000000 agentware-0.1.5/agentware/memory.py
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-23 07:31:06.000000 agentware-0.1.5/agentware/perception.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      225 2023-07-10 14:52:15.000000 agentware-0.1.5/agentware/singleton.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-08-02 05:58:33.898616 agentware-0.1.5/agentware/utils/
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-14 05:21:12.000000 agentware-0.1.5/agentware/utils/__init__.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-08-02 05:58:33.907382 agentware-0.1.5/agentware/utils/json_fixes/
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-10 14:52:15.000000 agentware-0.1.5/agentware/utils/json_fixes/__init__.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     2268 2023-07-10 14:52:15.000000 agentware-0.1.5/agentware/utils/json_fixes/auto_fix.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      800 2023-07-10 14:52:15.000000 agentware-0.1.5/agentware/utils/json_fixes/bracket_termination.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     1052 2023-07-10 15:16:07.000000 agentware-0.1.5/agentware/utils/json_fixes/escaping.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      795 2023-07-10 14:52:15.000000 agentware-0.1.5/agentware/utils/json_fixes/master_json_fix_method.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      674 2023-07-10 14:52:15.000000 agentware-0.1.5/agentware/utils/json_fixes/missing_quotes.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     6003 2023-07-14 09:47:09.000000 agentware-0.1.5/agentware/utils/json_fixes/parsing.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      565 2023-07-10 14:52:15.000000 agentware-0.1.5/agentware/utils/json_fixes/utilities.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-08-02 05:58:33.910043 agentware-0.1.5/agentware/utils/json_validation/
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-14 09:17:54.000000 agentware-0.1.5/agentware/utils/json_validation/__init__.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     1071 2023-07-10 15:16:07.000000 agentware-0.1.5/agentware/utils/json_validation/validate_json.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     2255 2023-07-10 15:16:07.000000 agentware-0.1.5/agentware/utils/num_token_utils.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-08-02 05:58:33.895164 agentware-0.1.5/agentware.egg-info/
+-rw-r--r--   0 weiduan    (501) staff       (20)      221 2023-08-02 05:58:33.000000 agentware-0.1.5/agentware.egg-info/PKG-INFO
+-rw-r--r--   0 weiduan    (501) staff       (20)     1047 2023-08-02 05:58:33.000000 agentware-0.1.5/agentware.egg-info/SOURCES.txt
+-rw-r--r--   0 weiduan    (501) staff       (20)        1 2023-08-02 05:58:33.000000 agentware-0.1.5/agentware.egg-info/dependency_links.txt
+-rw-r--r--   0 weiduan    (501) staff       (20)       43 2023-08-02 05:58:33.000000 agentware-0.1.5/agentware.egg-info/requires.txt
+-rw-r--r--   0 weiduan    (501) staff       (20)       16 2023-08-02 05:58:33.000000 agentware-0.1.5/agentware.egg-info/top_level.txt
+-rw-r--r--   0 weiduan    (501) staff       (20)       38 2023-08-02 05:58:33.920170 agentware-0.1.5/setup.cfg
+-rw-r--r--   0 weiduan    (501) staff       (20)      467 2023-08-02 05:58:29.000000 agentware-0.1.5/setup.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-08-02 05:58:33.917696 agentware-0.1.5/tests/
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-12 09:22:40.000000 agentware-0.1.5/tests/__init__.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     2632 2023-07-28 01:38:55.000000 agentware-0.1.5/tests/agent_workflow_test.py
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-27 09:05:03.000000 agentware-0.1.5/tests/config_test.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     3941 2023-08-02 05:44:41.000000 agentware-0.1.5/tests/connector_test.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     1524 2023-07-27 09:37:22.000000 agentware-0.1.5/tests/helper_agents_test.py
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-10 14:52:15.000000 agentware-0.1.5/tests/memory_test.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     1503 2023-07-28 01:46:43.000000 agentware-0.1.5/tests/utils.py
```

### Comparing `agentware-0.1.4/agentware/agent.py` & `agentware-0.1.5/agentware/agent.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from agentware.agent_logger import Logger
 from agentware.memory import Memory
-from agentware.base import BaseAgent, OneshotAgent, Connector
+from agentware.base import BaseAgent
 from agentware.hub import register_agent
 import yaml
 import openai
 import re
 import json
 import os
 import datetime
@@ -17,20 +17,19 @@
 
 logger = Logger()
 
 
 class Agent(BaseAgent):
 
     @classmethod
-    def fetch(cls, agent_id: int):
+    def pull(cls, agent_id: int):
         logger.info("Creating agent from connector")
         agent = cls()
-        memory = Memory.fetch(agent_id)
+        memory = Memory.pull(agent_id, agent)
         agent.memory = memory
-        agent.set_config(memory.get_main_agent_config())
         return agent
 
     def __init__(self):
         """ Creates a new agent instead of fetching from connector
 
         Construct the agent with or without memory.
 
@@ -39,85 +38,97 @@
 
         :type arg2: The data type of the second argument
         :ivar attribute1: A description of the first attribute
         :ivar attribute2: A description of the second attribute
         """
         super().__init__()
         self.id = None
-        self._memory = Memory()
+        self._memory = Memory(self)
+        self._update_mode = False
         openai.api_key = agentware.openai_api_key
 
-    def set_config(self, config: Dict):
-        self._memory.set_main_agent_config(config)
+    def update(self):
+        return self.UpdateContext(self)
 
-    def get_config(self):
-        return self._memory.get_main_agent_config()
+    class UpdateContext:
+        def __init__(self, obj):
+            self.obj = obj
+
+        def __enter__(self):
+            self.obj._update_mode = True
+            return self.obj
+
+        def __exit__(self, exc_type, exc_val, exc_tb):
+            # update knowledge
+            self.obj._update_mode = False
 
     def run(self, prompt):
         output_valid = False
         num_retries = 0
         raw_output = ""
-        format_instruction = f"{self.format_instruction}. {self.output_schema}"
-        self._memory.prepare_run(self.prompt_prefix, prompt)
-        parsed_output = ""
-        logger.info(f"Making a working copy of memory: {self._memory}")
-        memory_with_error = copy.deepcopy(self._memory)
-        # Add format instruction to the last memory unit
-        memory_with_error.delete_memory(-1)
-        memory_with_error.add_memory({
-            "role": self._memory.get_memory()[-1].role,
-            "content": self._memory.get_memory()[-1].content + format_instruction
+        logger.debug(f"Adding prompt to memory: {prompt}")
+        self._memory.update_context(self._prompt_prefix, prompt)
+        self._memory.add_memory({
+            "role": "user",
+            "content": f"{self._prompt_prefix} {prompt} {self._format_instruction}."
         })
+        memory_with_error = copy.deepcopy(self._memory)
+        logger.info(f"Copy of memory made: {memory_with_error}")
         while True:
             if num_retries > 0:
                 logger.debug(f"Retrying for the {num_retries} time")
             try:
                 messages = memory_with_error.to_messages()
-                logger.info(
-                    f"memory before running is {self._memory}")
                 raw_output = self._run(messages)
                 try:
-                    parsed_output = self.parse_output(raw_output)
-                    new_memory = ""
-                    if self.termination_observation in parsed_output:
-                        new_memory = parsed_output[self.termination_observation]
+                    output = ""
+                    if self._output_schema:
+                        output = self.parse_output(raw_output)
+                        if self._termination_observation in output:
+                            # Whatever sub structure in outupt is dumped to str
+                            output = json.dumps(
+                                output[self._termination_observation])
+                    else:
+                        output = raw_output
+                    logger.debug(f"Adding response to memory: {output}")
                     self._memory.add_memory({
                         "role": "assistant",
-                        "content": new_memory
+                        "content": output
                     })
 
                     output_valid = True
-                    return parsed_output
+                    return output
                 except Exception as err:
                     logger.warning(f"Error parsing with exception {err}")
 
                     traceback.print_exc()
                     if num_retries >= 1:
                         # Delete the previous error information
                         memory_with_error.delete_memory(-1)
                         memory_with_error.delete_memory(-1)
                     memory_with_error.add_memory({
                         "role": "assistant",
                         "content": raw_output
                     })
                     memory_with_error.add_memory({
                         "role": "user",
-                        "content": f"Failed to parse output. Ignore all the format instructions you were given previously. Your output must be a json that strictly follow the schema while not including it {self.output_schema}"
+                        "content": f"Failed to parse output. Ignore all the format instructions you were given previously. Your output must be a json that strictly follow the schema while not including it {self._output_schema}"
                     })
             except Exception as e:
                 logger.warning(f"Error getting agent output with error {e}")
             if output_valid or num_retries >= self.MAX_NUM_RETRIES:
                 break
             num_retries += 1
-        return parsed_output
 
-    def register(self, agent_id: str):
+    def register(self, agent_id: str = ""):
+        if not agent_id:
+            agent_id = self._config["name"]
         assert agent_id
         register_agent(agent_id)
         self.agent_id = agent_id
         self._memory.agent_id = agent_id
 
     def push(self):
         # Check agent id valid
         assert self.agent_id
         logger.debug(f"Pushing agent with name {self.agent_id}")
-        self._memory.update_check_point()
+        self._memory.update_agent()
```

### Comparing `agentware-0.1.4/agentware/agent_logger.py` & `agentware-0.1.5/agentware/agent_logger.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.4/agentware/base.py` & `agentware-0.1.5/agentware/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,70 @@
+from agentware.utils.json_fixes.parsing import fix_and_parse_json
+from agentware.utils.json_validation.validate_json import validate_json
+from typing import List, Dict
+from agentware.utils.num_token_utils import count_message_tokens
+from agentware.core_engines import OpenAICoreEngine
+from agentware import KNOWLEDGE_BASE_IDENTIFIER_PREFIX
+from datetime import datetime
+from agentware.agent_logger import Logger
+from pymilvus import Milvus, connections, utility
 import os
 import time
 import json
 import requests
 import openai
 import agentware
 import copy
 
 from typing import List, Dict, Tuple
 from pymilvus import Collection, DataType, FieldSchema, CollectionSchema
-from pymilvus import Milvus, connections, utility
-from agentware.agent_logger import Logger
-from datetime import datetime
-from agentware.utils.num_token_utils import count_message_tokens
-from typing import List, Dict
-from agentware.utils.json_validation.validate_json import validate_json
-from agentware.utils.json_fixes.parsing import fix_and_parse_json
+
 
 logger = Logger()
 
 
+class AgentConfig:
+    def __init__(self, config: Dict[str, any]):
+        assert "name" in config
+        self.name = config['name']
+        assert "conversation_setup" in config
+        assert "prompt_prefix" in config
+        if "output_format" in config:
+            assert "instruction" in config
+
+        # "name": "tool_query",
+        # "conversation_setup": "You will be given a json file that has two keys 'observations' and 'facts', each containing a list. The 'observations' field is a list of new observations, while the 'facts' field contains the facts before the observations, each with and id. Your job is to help find out which of the facts are no longer true, give the ids of the them, and the updated facts that are true given the observations",
+        # "prompt_prefix": "List the ids of the facts if they are wrong given the observations:",
+        # "output_format": {
+        #     "instruction": "Your output MUST be a json that has a field named \"wrong_facts\".",
+        #     "examples": [
+        #         {
+        #             "condition": "",
+        #             "output": "{\"wrong_facts\": [{\"id\": <int id of the wrong fact, must be in accordance with the facts in question>, <another id>, ...]}"
+        #         }
+        #     ],
+        #     "output_schema":
+        #     {
+        #         "$schema": "http://json-schema.org/draft-07/schema#",
+        #         "type": "object",
+        #         "properties": {
+        #             "wrong_facts": {
+        #                 "type": "array",
+        #                 "items": {
+        #                     "type": "integer"
+        #                 }
+        #             }
+        #         },
+        #         "required": ["wrong_facts"],
+        #         "additionalProperties": false
+        #     },
+        #     "termination_observation": "wrong_facts"
+        # }
+
+
 class Node:
     def __init__(self, node_name: str, embedding: List[float] = []):
         self.name = node_name
         self.embeds = embedding
         self.created_at = int(time.time())
 
     def __repr__(self):
@@ -31,15 +73,15 @@
 
 class Command:
     def __init__(self, name: str, description: str, endpoint: str, input_schema: str, output_schema: str):
         self.name = name
         self.description = description
         self.endpoint = endpoint
         self.input_schema = input_schema
-        self.output_schema = output_schema
+        self._output_schema = output_schema
         self.created_at = int(time.time())\
 
 
     def to_prompt(self) -> str:
         return f"""{self.name}: {self.description}
 input must strictly be a json following this schema:
 {self.input_schema}"""
@@ -76,192 +118,224 @@
 
     def __str__(self) -> str:
         return f"<{self.role}>: {self.content}[{self.num_tokens} tokens]"
 
 
 class Knowledge:
 
-    def __init__(self, created_at: int, content: str, embeds: List = []):
+    def __init__(self, created_at: int, content: str, embeds: List = [], id="", num_tokens: int = 0):
         self.created_at = int(created_at)
         self.content = content
         self.embeds = embeds
-        self.num_tokens = count_message_tokens({
-            "content": content
-        })
+        self.id = id
+        if num_tokens <= 0:
+            self.num_tokens = count_message_tokens({
+                "content": content
+            })
+        else:
+            self.num_tokens = num_tokens
 
     @classmethod
     def from_json(cls, knowledge_json: Dict):
         embeds = []
         if "embeds" in knowledge_json:
             embeds = knowledge_json["embeds"]
-        return cls(knowledge_json["created_at"], knowledge_json["content"], embeds)
+        id = ""
+        if "id" in knowledge_json:
+            id = knowledge_json["id"]
+        return cls(knowledge_json["created_at"], knowledge_json["content"], embeds, id)
 
     def to_json(self):
         return {
             "created_at": self.created_at,
             "content": self.content,
-            "embeds": self.embeds
+            "embeds": self.embeds,
+            "id": self.id
         }
 
     def _to_str(self, created_at: int, content: str) -> str:
         return f"knowledge created at {datetime.fromtimestamp(created_at)}. content: {content}"
 
     def __repr__(self):
-        return f"knowledge({self.content}, created at {self.created_at})"
+        return f"knowledge({self.content}, created at {self.created_at}, id {self.id})"
 
     def update_embeds(self, embeds: List[float]) -> None:
         self.embeds = embeds
 
 
 class BaseAgent:
     """
         Base agent class with
         - config initialization
         - parse and retry
     """
-    MODEL_NAME = "gpt-3.5-turbo"
+    MODEL_NAME = "gpt-3.5-turbo-16k-0613"
     MAX_NUM_RETRIES = 3
 
     def __init__(self):
         self._config = None
+        self._format_instruction = ""
+        self._output_schema = ""
+        self._prompt_prefix = ""
+        self._format_examples = ""
+        self._core_engine = OpenAICoreEngine()
 
     @classmethod
     def init(cls, cfg: Dict[str, any]):
         agent = cls()
         if not cfg:
             raise Exception("Invalid config")
         if (not cfg["name"]):
             raise Exception("config missing required entry {cfg}")
-        agent._config = cfg
+        agent.set_config(cfg)
+        return agent
+
+    def set_core_engine(self, core_engine):
+        logger.debug(f"Setting core engine to {core_engine}")
+        self._core_engine = core_engine
+
+    def get_embeds(self, text: str) -> List[float]:
+        return self._core_engine.get_embeds(text)
+
+    def set_config(self, cfg: Dict[str, any]):
+        self._config = cfg
         # output format
         if "output_format" in cfg:
-            agent.format_instruction = None
+            self._format_instruction = ""
             if "instruction" in cfg["output_format"]:
-                agent.format_instruction = cfg["output_format"]["instruction"]
-            agent.output_schema = None
+                self._format_instruction = cfg["output_format"]["instruction"]
+            self._output_schema = ""
             if "output_schema" in cfg["output_format"]:
-                agent.output_schema = cfg["output_format"]["output_schema"]
-            agent.termination_observation = None
+                self._output_schema = cfg["output_format"]["output_schema"]
+            if "examples" in cfg["output_format"]:
+                self._format_examples = ""
+                for example in cfg["output_format"]["examples"]:
+                    example_output = example["output"]
+                    if example["condition"]:
+                        condition = example["condition"]
+                        self._format_examples += f"In the case of {condition}, output in the form of {example_output}"
+                    else:
+                        self._format_examples += f"Output in the form of {example_output}"
+                        # Empty condition means one output format for all cases
+                        break
+            self._format_instruction += self._format_examples
+            self._termination_observation = ""
             if "termination_observation" in cfg["output_format"]:
-                agent.termination_observation = cfg["output_format"]["termination_observation"]
+                self._termination_observation = cfg["output_format"]["termination_observation"]
         if "prompt_prefix" in cfg:
-            agent.prompt_prefix = cfg["prompt_prefix"]
-        return agent
+            self.prompt_prefix = cfg["prompt_prefix"]
 
     def get_config(self) -> Dict[str, any]:
         return self._config
 
     def _messages_to_str(self, messages: List[Dict[str, str]]) -> str:
         message_prefix = "\n************* Conversation *************\n"
         message_suffix = "\n********* End of Conversation *********\n"
         message_str = "\n---------------------------------\n".join(
             [f"<{m['role']}>: {m['content']}" for m in messages])
         return message_prefix + message_str + message_suffix
 
     def _run(self, messages: List[Dict[str, str]]) -> str:
         logger.debug(
             f"Sending raw messages: {self._messages_to_str(messages)}")
-        completion = openai.ChatCompletion.create(
-            model=self.MODEL_NAME, messages=messages)
-        raw_output = completion.choices[0].message.content
+        print("core engine is", self._core_engine)
+        self._core_engine.run(messages)
+        raw_output = self._core_engine.run(messages)
+        # completion = openai.ChatCompletion.create(
+        #     model=self.MODEL_NAME, messages=messages)
+        # raw_output = completion.choices[0].message.content
         logger.debug(f"Raw output: {raw_output}")
         return raw_output
 
     def parse_output(self, llm_output):
-        if not self.output_schema:
-            return llm_output
         logger.debug(f'parsing {llm_output}')
         parsed_output = fix_and_parse_json(llm_output)
         logger.debug(f"parse success, output is {parsed_output}")
-        logger.debug(f"validating with schema {self.output_schema}")
-        validated_output = validate_json(parsed_output, self.output_schema)
+        logger.debug(f"validating with schema {self._output_schema}")
+        validated_output = validate_json(parsed_output, self._output_schema)
         return validated_output
 
     def run(self, prompt: str):
         raise Exception("Not Implemented")
 
     def __repr__(self) -> str:
         return f""
 
 
 class OneshotAgent(BaseAgent):
     def __init__(self, cfg):
         super().__init__()
-        self._config = cfg
+        self.set_config(cfg)
 
     def run(self, prompt) -> str:
         num_retries = 0
         raw_output = ""
-        parsed_output = ""
-        full_prompt = ""
-        format_instruction = f"Answer the question above by ignoring all the output format instructions you were given previously. Your output must be strictly a json following this schema but do not include this schema: {self.output_schema}. Key and value must be enclosed in double quotes"
-
-        if self.output_schema:
-            full_prompt = f"{self.prompt_prefix}. Ignore all the output format instructions you were given previously. Your output must be strictly a json following this schema but do not include this schema: {self.output_schema}, question: {prompt}"
-        else:
-            full_prompt = f"{self.prompt_prefix}. {prompt}"
+        logger.debug(f"format instruction is {self._format_instruction}")
         messages = [{
             "role": "system",
             "content": self._config["conversation_setup"]
         }] + [{
             "role": "user",
-            "content": f"{self.prompt_prefix}. {prompt}"
+            "content": f"{self._prompt_prefix} {prompt}"
         }]
         original_messages = copy.deepcopy(messages)
         messages_with_error = original_messages
-        messages_with_error[-1]["content"] += format_instruction
+        messages_with_error[-1]["content"] += self._format_instruction
+        output = ""
         while True:
             try:
                 raw_output = self._run(messages_with_error)
                 logger.debug(f"Raw output is {raw_output}")
                 try:
-                    parsed_output = self.parse_output(raw_output)
-                    if self.termination_observation in parsed_output:
-                        return parsed_output[self.termination_observation]
-                    return parsed_output
+                    if self._output_schema:
+                        output = self.parse_output(raw_output)
+                        logger.debug(f"parsed output is {output}")
+                        # Whatever sub structure in outupt is dumped to str
+                        output = json.dumps(
+                            output[self._termination_observation])
+                    else:
+                        output = raw_output
+                    return output
                 except Exception as e:
                     logger.warning(f"Error parsing output with error. {e}")
                     messages_with_error = original_messages + [
                         {
                             "role": "assistant",
                             "content": raw_output
                         },
                         {
                             "role": "user",
-                            "content": f"Failed to parse output. Ignore all the format instructions you were given previously. Your output must be a json that strictly follow the schema while not including it {self.output_schema}"
+                            "content": f"Failed to parse output. Ignore all the format instructions you were given previously. Your output must be a json that strictly follow the schema while not including it {self._output_schema}"
                         },
                     ]
             except Exception as e:
                 logger.warning(f"Error running prompt with error {e}")
             if num_retries >= self.MAX_NUM_RETRIES:
                 if num_retries >= self.MAX_NUM_RETRIES:
                     logger.debug("Max number of retries exceeded")
                 break
             num_retries += 1
-        return parsed_output
+        return output
 
 
 class BaseMilvusStore():
-    DEFAULT_EMBED_DIM = 1536  # openai embedding
-
     def _create_collection(self, collection_name: str) -> Collection:
         raise Exception("Not Implemented")
 
     def __init__(self, cfg: dict[str, any]) -> None:
         if not cfg:
             raise BaseException("Invalid config")
         try:
             self.milvus_uri = cfg['uri']
             self.user = cfg['user']
             self.port = cfg['port']
             self.nprobe = int(cfg['nprobe'])
             self.nlist = int(cfg['nlist'])
         except ValueError as e:
             raise BaseException(f"Missing key in config caused error {e}")
-        self.client = Milvus(self.milvus_uri, self.port)
 
         self.connect = connections.connect(
             alias="default",
             host=self.milvus_uri,
             port=self.port
         )
         logger.debug(f"Connected to vector store: {self.milvus_uri}")
@@ -289,14 +363,19 @@
                                output_fields=output_fields,
                                limit=999)
             return results
         except Exception as err:
             logger.debug("get err {}".format(err))
             return err
 
+    def remove_by_ids(self, ids_to_delete: List[int], collection_name: str):
+        c = Collection(collection_name)
+        expr = f"id in {ids_to_delete}"
+        c.delete(expr)
+
 
 class Connector():
     """
 
     modes
     - Use an agent, only have access to newly created
     - Fork an agent that allows access, have access to prefix, prompt prefix and knowledge
@@ -333,15 +412,15 @@
                 f'Request failed with status code: {response.status_code}')
             return None
 
     def _get_command_hub_id(self) -> str:
         return "command_collection"
 
     def _get_knowledge_base_id(self, agent_id: int):
-        return f"knowledge_{agent_id}"
+        return f"{KNOWLEDGE_BASE_IDENTIFIER_PREFIX}_{agent_id}"
 
     def _get_knowledge_graph_label(self, agent_id: int):
         return f"knowledge_graph_{agent_id}"
 
     def all_agents(self) -> List[str]:
         url = os.path.join(
             agentware.endpoint, "all_agents")
@@ -405,47 +484,45 @@
             return data
         else:
             # Request failed
             logger.debug(
                 f'Request failed with status code: {response.status_code}')
             return None
 
-    def update_checkpoint(self, agent_id: int, agent_config: Dict[any, any], memory_units: List[MemoryUnit], knowledges: List[Knowledge], context: str):
+    def update_agent(self, agent_id: int, agent_config: Dict[any, any], memory_units: List[MemoryUnit]):
         if agent_id is None:
             agent_id = -1
         url = os.path.join(
-            agentware.endpoint, "update_checkpoint", str(agent_id))
+            agentware.endpoint, "update_agent", str(agent_id))
         headers = {
             'Authorization': f'Bearer {agentware.api_key}'
         }
-        ckpt_data = json.dumps({
+        agent_data = json.dumps({
             "agent_config": agent_config,
             "memory_data":  [m.to_json() for m in memory_units],
-            "knowledge": [k.to_json() for k in knowledges],
-            "context": context
         })
         logger.info(
-            f"Saving checkpoint {ckpt_data}")
+            f"Saving agent {agent_data}")
         # Send GET request
-        response = requests.put(url, headers=headers, data=ckpt_data)
+        response = requests.put(url, headers=headers, data=agent_data)
         # Check the response status code
         if response.status_code == 200:
 
             logger.debug(f'Request to {url} was successful')
             data = json.loads(response.text)
             return data
         else:
             # Request failed
             logger.debug(
                 f'Request failed with status code: {response.status_code}')
             return None
 
-    def get_checkpoint(self, agent_id: str) -> Tuple[Dict[any, any], Dict[str, Dict[any, any]], List[MemoryUnit], List[Knowledge], str]:
+    def get_agent(self, agent_id: str) -> Tuple[Dict[any, any], Dict[str, Dict[any, any]], List[MemoryUnit], List[Knowledge], str]:
         # URL to send the request to
-        url = os.path.join(agentware.endpoint, "get_checkpoint")
+        url = os.path.join(agentware.endpoint, "get_agent")
         # Send GET request
         headers = {
             'Authorization': f'Bearer {agentware.api_key}'
         }
         params = {
             "agent_id": agent_id
         }
@@ -453,36 +530,29 @@
         # Check the response status code
         if response.status_code == 200:
             logger.debug(f'Request to {url} was successful')
             data = json.loads(response.text)
             print("data is", data)
             if not data["success"]:
                 raise ValueError(data["error_code"])
-            main_agent_config = data["main_agent_config"]
+            agent_config = data["agent_config"]
             memory_units = [MemoryUnit.from_json(
                 m) for m in data["memory_units"]]
-            knowledges = [Knowledge.from_json(
-                k) for k in data["knowledges"]]
-            context = data["context"]
-            return main_agent_config, memory_units, knowledges, context
+            return agent_config, memory_units
         else:
+            print("response is", response.text)
             # Request failed
             logger.debug(
-                f'Request failed with status code: {response.status_code}')
-            return None
+                f'Request failed with code: {response.status_code} error: {response.text}')
+            return None, None
 
     def save_knowledge(self, agent_id: int, knowledges: List[Knowledge]):
         knowledge_base_identifier = self._get_knowledge_base_id(agent_id)
         logger.info(
             f"Saving knowledge: {knowledges} to knowledge base {knowledge_base_identifier}")
-        for i, knowledge in enumerate(knowledges):
-            if knowledge.embeds:
-                continue
-            embeds = self.get_embeds(knowledge.content)
-            knowledges[i].update_embeds(embeds)
         # URL to send the request to
         url = os.path.join(agentware.endpoint, "save_knowledge",
                            knowledge_base_identifier)
         # Send GET request
         headers = {
             'Authorization': f'Bearer {agentware.api_key}'
         }
@@ -498,16 +568,15 @@
             return data
         else:
             # Request failed
             logger.debug(
                 f'Request failed with status code: {response.status_code}')
             return None
 
-    def search_commands(self, keyword: str, token_limit=100) -> List[Command]:
-        query_embeds = self.get_embeds(keyword)
+    def search_commands(self, query_embeds: List[float], token_limit=100) -> List[Command]:
         # URL to send the request to
         url = os.path.join(agentware.endpoint, "search_commands",
                            self._get_command_hub_id())
         # Send GET request
         headers = {
             'Authorization': f'Bearer {agentware.api_key}'
         }
@@ -525,16 +594,15 @@
         else:
             # Request failed
             logger.debug(
                 f'Request failed with status code: {response.status_code}')
             logger.debug(response.text)
             return None
 
-    def search_knowledge(self, agent_id: int, keyword: str, token_limit=100) -> List[Knowledge]:
-        query_embeds = self.get_embeds(keyword)
+    def search_knowledge(self, agent_id: int, query_embeds: List[float], token_limit=100) -> List[Knowledge]:
         # URL to send the request to
         url = os.path.join(agentware.endpoint, "search_knowledge",
                            self._get_knowledge_base_id(agent_id))
         # Send GET request
         headers = {
             'Authorization': f'Bearer {agentware.api_key}'
         }
@@ -552,14 +620,44 @@
         else:
             # Request failed
             logger.debug(
                 f'Request failed with status code: {response.status_code}')
             logger.debug(response.text)
             return None
 
+    def remove_knowledge(self, agent_id: int, ids_to_remove: List[int]):
+        knowledge_base_identifier = self._get_knowledge_base_id(agent_id)
+        # URL to send the request to
+        url = os.path.join(agentware.endpoint, "remove_knowledge")
+        # Send GET request
+        headers = {
+            'Authorization': f'Bearer {agentware.api_key}'
+        }
+        data = json.dumps({
+            "xx": 'yy',
+            "collection_name": knowledge_base_identifier,
+            "ids_to_remove": ids_to_remove
+        })
+        response = requests.put(url, headers=headers, data=data)
+        # Check the response status code
+        if response.status_code == 200:
+            logger.debug(f'Request to {url} was successful')
+            data = json.loads(response.text)
+            if "success" in data:
+                logger.debug(f"Removed ids success? {data}")
+                return data["success"]
+            else:
+                return False
+        else:
+            # Request failed
+            logger.debug(
+                f'Request failed with status code: {response.status_code}')
+            logger.debug(response.text)
+            return None
+
     def get_recent_knowledge(self, agent_id: int, token_limit=100) -> List[Knowledge]:
         url = os.path.join(agentware.endpoint, "get_recent_knowledge",
                            self._get_knowledge_base_id(agent_id))
         # Send GET request
         headers = {
             'Authorization': f'Bearer {agentware.api_key}'
         }
@@ -567,31 +665,24 @@
             "token_limit": token_limit
         })
         response = requests.get(url, headers=headers, data=data)
         # Check the response status code
         if response.status_code == 200:
             logger.debug(f'Request to {url} was successful')
             data = json.loads(response.text)
-            logger.debug(f"knowledge data is", data)
-            return data
+            logger.debug(f"knowledge data is {data}")
+            return [Knowledge.from_json(knowledge_json) for knowledge_json in data]
         else:
             # Request failed
             logger.debug(
                 f'Request failed with status code: {response.status_code}')
             logger.debug(response.text)
             return None
 
-    def get_embeds(self, text: str):
-        model = "text-embedding-ada-002"
-        text = text.replace("\n", " ")
-        logger.debug(f"Getting embedding of: {text}")
-        return openai.Embedding.create(input=[text], model=model)['data'][0]['embedding']
-
-    def search_kg(self, agent_id: int, keyword: str, token_limit=100) -> List[Knowledge]:
-        query_embeds = self.get_embeds(keyword)
+    def search_kg(self, agent_id: int, query_embeds: List[float], token_limit=100) -> List[Knowledge]:
         # URL to send the request to
         url = os.path.join(agentware.endpoint, "search_kg",
                            self._get_knowledge_graph_label(agent_id))
         # Send GET request
         headers = {
             'Authorization': f'Bearer {agentware.api_key}'
         }
```

### Comparing `agentware-0.1.4/agentware/memory.py` & `agentware-0.1.5/agentware/memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 from typing import Dict, List, Tuple
 from agentware.base import MemoryUnit, Knowledge, Connector, OneshotAgent, BaseAgent
 from agentware.agent_logger import Logger
+from agentware import HELPER_AGENT_CONFIGS_DIR_NAME
 
 import copy
 import time
 import json
+import os
 
 logger = Logger()
 
 
 class Memory():
-    HELPER_AGENT_CONFIGS_DIR = "agentware/base_agent_configs"
     MAX_NUM_TOKENS_CONTEXT = 1000
     MAX_NUM_TOKENS_MEMORY = 1000
     MAX_NUM_TOKENS_KNOWLEDGE = 200
 
-    def __init__(self):
+    def __init__(self, agent: BaseAgent):
         self._helper_agents = self.create_helper_agents()
         self._reflections = []
         self._commands = []
         self._domain_knowledge = []
         self._memory = []
-        self._context = []
+        self._context = ""
         self._num_tokens_memory = 0
         self._num_tokens_context = 0
         self._num_tokens_domain_knowledge = 0
-        self._main_agent_config = dict()
+        self._agent = agent
         self.agent_id = None
         self.connector = Connector()
 
     @classmethod
-    def fetch(cls, agent_id: int):
+    def pull(cls, agent_id: int, agent):
         connector = Connector()
         try:
-            agent_config, memory_data, domain_knowledge, context = connector.get_checkpoint(
+            agent_config, memory_data = connector.get_agent(
                 agent_id)
-
-            memory = cls.init(agent_config, context,
-                              domain_knowledge, memory_data)
+            memory = cls.init(agent_config, memory_data, agent)
         except Exception as e:
             raise e
         return memory
 
     @classmethod
     def init(cls,
-             main_agent_config: Dict[any, any],
-             context: str,
-             work_experience: List[Knowledge],
-             working_memory: List[MemoryUnit]):
+             agent_config: Dict[any, any],
+             working_memory: List[MemoryUnit],
+             agent: BaseAgent):
         logger.debug("initializing memory")
-        memory = cls()
-        memory.set_main_agent_config(main_agent_config)
-        memory._context = context
-        memory._work_experience = work_experience
+        memory = cls(agent)
+        memory._context = agent_config["conversation_setup"]
         memory._memory = working_memory
+        agent.set_config(agent_config)
         return memory
 
     def create_helper_agents(self) -> Dict[str, OneshotAgent]:
-        facts_agent_config_path = f"{self.HELPER_AGENT_CONFIGS_DIR}/facts.json"
-        ref_q_agent_config_path = f"{self.HELPER_AGENT_CONFIGS_DIR}/reflection_question.json"
-        ref_agent_config_path = f"{self.HELPER_AGENT_CONFIGS_DIR}/reflection.json"
-        summarize_agent_config_path = f"{self.HELPER_AGENT_CONFIGS_DIR}/summarize.json"
-        tool_query_agent_config_path = f"{self.HELPER_AGENT_CONFIGS_DIR}/tool_query.json"
+        config_dir_absolute_path = os.path.join(os.path.dirname(
+            os.path.abspath(__file__)), HELPER_AGENT_CONFIGS_DIR_NAME)
+        facts_agent_config_path = f"{config_dir_absolute_path}/facts.json"
+        ref_q_agent_config_path = f"{config_dir_absolute_path}/reflection_question.json"
+        ref_agent_config_path = f"{config_dir_absolute_path}/reflection.json"
+        summarize_agent_config_path = f"{config_dir_absolute_path}/summarize.json"
+        tool_query_agent_config_path = f"{config_dir_absolute_path}/tool_query.json"
+        conflict_resolver_agent_config_path = f"{config_dir_absolute_path}/conflict_resolver.json"
 
         agents = dict()
         fact_agent_config = None
         with open(facts_agent_config_path, "r") as f:
             fact_agent_config = json.loads(f.read())
         agents["fact"] = OneshotAgent(fact_agent_config)
         # Summarize agent
@@ -84,22 +84,21 @@
             ref_agent_config = json.loads(f.read())
         agents["reflection"] = OneshotAgent(ref_agent_config)
         # Tool query
         tool_query_agent_config = None
         with open(tool_query_agent_config_path, "r") as f:
             tool_query_agent_config = json.loads(f.read())
         agents["tool_query"] = OneshotAgent(tool_query_agent_config)
+        conflict_resolver_agent_config = None
+        with open(conflict_resolver_agent_config_path, "r") as f:
+            conflict_resolver_agent_config = json.loads(f.read())
+        agents["conflict_resolver"] = OneshotAgent(
+            conflict_resolver_agent_config)
         return agents
 
-    def get_main_agent_config(self) -> Dict[str, any]:
-        return self._main_agent_config
-
-    def set_main_agent_config(self, config: Dict[str, any]):
-        self._main_agent_config = config
-
     def get_num_tokens_memory(self):
         return self._num_tokens_memory
 
     def get_context(self) -> str:
         return self._context
 
     def get_domain_knowledge(self) -> List[Knowledge]:
@@ -138,52 +137,63 @@
         for q in questions:
             answer = self._helper_agents["reflection"].run(
                 f"```{memory_text}``` {q}. Answer the question above within 10 tokens")
             answers.append(answer)
         logger.debug(answers)
 
     def get_query_term(self, seed) -> str:
-        return self._helper_agents["tool_query"].run(seed)
+        """ Extract search keywords from the query sentence.
+        """
+        return seed
 
-    def prepare_run(self, prompt_prefix: str, prompt: str):
+    def update_context(self, prompt_prefix: str, prompt: str):
         logger.info(
-            f"Preparing for running prompt {prompt}\n and prefix {prompt_prefix}")
-        super().prepare_run(prompt_prefix, prompt)
+            f"Preparing for running prompt {prompt} and prefix {prompt_prefix}")
         # Get relevant knowledge
         keyword = self.get_query_term(prompt)
         logger.debug(f"search keywords for knowledge retrieval: {keyword}")
         new_knowledges = []
         if keyword:
             new_knowledges = self.connector.search_knowledge(
-                self.agent_id, keyword, token_limit=self.MAX_NUM_TOKENS_DOMAIN_KNOWLEDGE)
+                self.agent_id, self._agent.get_embeds(keyword), token_limit=self.MAX_NUM_TOKENS_KNOWLEDGE)
+            logger.debug(f"Updated new knowledge to {new_knowledges}")
         else:
             logger.debug(
                 "Keyword is empty, fetching most recent knowledge instead")
             new_knowledges = self.connector.get_recent_knowledge(
                 self.agent_id)
-            self.update_knowledge(new_knowledges)
+        self.update_knowledge(new_knowledges)
         # query for commands
-        # self._commands = self.connector.search_commands(keyword)
+        # self._commands = self.connector.search_commands(self._agent.get_embeds(keyword))
         print("domain knowledges are", self._domain_knowledge)
         # print("commands are", self._commands)
 
     def reflect(self, memory_text, context=None) -> List[Knowledge]:
         # context gives information on what job the agent is doing.
-        logger.debug("Making reflection from")
-        logger.debug(memory_text)
+        logger.debug(f"Making reflection from {memory_text}")
         # Make reflection on compressed memory
         # Step1: Extract facts.
-        # TODO: 解决first name / last name -> full name的问题
-        # 发现facts和reflection比较冗余。暂时只保留reflection了
         facts = self._helper_agents["fact"].run(
             f"```{memory_text}```, extract all facts and insights concisely from the text above and make sure each fact has clear meaning if viewed independently. Each fact should not exceed 10 tokens.")
-        facts = [f["subject_concept"] + " " + f["fact"] for f in facts]
-        logger.debug(facts)
-        knowledges = [Knowledge(int(time.time()), fact) for fact in facts]
-        return knowledges
+        logger.debug(f"facts are {facts}")
+        new_knowledges = [Knowledge(int(time.time()), fact) for fact in facts]
+        # Get keywords from memory text
+        keyword = self.get_query_term(memory_text)
+        relevant_knowledges = self.connector.search_knowledge(
+            self.agent_id, self._agent.get_embeds(keyword), token_limit=self.MAX_NUM_TOKENS_KNOWLEDGE)
+        # Compare the facts in memory with the relevant knowledge, mark the ones that need to be updated
+        knowledge_ids_to_remove = []
+        logger.debug()
+        observations_old_facts = {
+            "observations": facts,
+            "facts": [k.to_json() for k in relevant_knowledges]
+        }
+        knowledge_ids_to_remove = self._helper_agents["conflict_resolver"].run(
+            json.dumps(observations_old_facts))
+        return new_knowledges, knowledge_ids_to_remove
 
     def _compress_memory(self, reflect=False) -> Tuple[List[MemoryUnit], List[Knowledge]]:
         """ Compress memory and maybe do reflection
 
         Reflection is implemented in a similar way as the Stanford paper
         """
         # Let LLM summarize the first half of the memory
@@ -193,51 +203,60 @@
         logger.info("memory before compressing is")
         logger.info(self.__str__())
         compress_until_index = 0
         current_num_tokens = 0
         for i, m in enumerate(self._memory):
             print("m is", m)
             current_num_tokens += m.num_tokens
-            if current_num_tokens > self.num_tokens_memory/2:
+            if current_num_tokens > self._num_tokens_memory/2:
                 compress_until_index = i
                 break
-        num_tokens_not_compressed = self.num_tokens_memory - current_num_tokens
+        num_tokens_not_compressed = self._num_tokens_memory - current_num_tokens
         print(
             f"From {len(self._memory)} memory units, compressing from 0 to {compress_until_index}")
         memory_to_compress = self._memory[:(compress_until_index+1)]
         # Format memory to text
         memory_text = ""
         for m in memory_to_compress:
             memory_text += f"{m.role}: {m.content}\n"
         compressed_memory_content = self._helper_agents["summarizer"].run(
             f"```{memory_text}```. Please make a summary of the conversation above in no more than 200 tokens. Respond with the summarization")
         compressed_memory = MemoryUnit(
             "user",  f"A summary of our past conversation: {compressed_memory_content}")
         self._memory = [compressed_memory] + \
             self._memory[compress_until_index:]
-        self.num_tokens_memory = num_tokens_not_compressed + compressed_memory.num_tokens
+        self._num_tokens_memory = num_tokens_not_compressed + compressed_memory.num_tokens
         logger.info("memory after compressing is")
         logger.info(self.__str__())
-        reflections = self.reflect(memory_text)
-        # Save checkpoint and add to knowledge
+        reflections, ids_to_remove = self.reflect(memory_text)
+        # Remove knowledges
+        logger.debug(f"Removing ids {ids_to_remove} from knowledge base")
+        try:
+            self.connector.remove_knowledge(self.agent_id, ids_to_remove)
+        except Exception as e:
+            logger.warning(f"Failed to remove ids with error {e}")
+        # Save agent and add to knowledge
         if self.connector:
+            for i, knowledge in enumerate(reflections):
+                if knowledge.embeds:
+                    continue
+                embeds = self._agent.get_embeds(knowledge.content)
+                reflections[i].update_embeds(embeds)
             self.connector.save_knowledge(self.agent_id, reflections)
             self.connector.update_longterm_memory(
                 self.agent_id, memory_to_compress)
-            # Update current checkpoint
-            self.update_check_point(self.agent_id)
+            # Update current agent
+            self.update_agent()
         return memory_to_compress
 
-    def update_check_point(self):
-        self.connector.update_checkpoint(
+    def update_agent(self):
+        self.connector.update_agent(
             self.agent_id,
-            self._main_agent_config,
-            self._memory,
-            self._domain_knowledge,
-            self._context)
+            self._agent._config,
+            self._memory)
 
     def add_memory(self, memory: Dict[str, str]):
         new_memory = MemoryUnit(memory["role"], memory["content"])
         self._memory.append(new_memory)
         self._num_tokens_memory += new_memory.num_tokens
         if self._num_tokens_memory > self.MAX_NUM_TOKENS_MEMORY:
             self._compress_memory(reflect=True)
@@ -247,30 +266,35 @@
             self._num_tokens_domain_knowledge += k.num_tokens
             if self._num_tokens_domain_knowledge > self.MAX_NUM_TOKENS_KNOWLEDGE:
                 break
 
     def delete_memory(self, memory_index: int):
         if memory_index >= len(self._memory):
             logger.debug(
-                f"Deleting index {memory_index} out of range of 0-{len(self._memory - 1)}")
+                f"Deleting index {memory_index} out of range of 0-{len(self._memory)-1}")
+            return
+        if memory_index < 0:
+            if memory_index + len(self._memory) - 1 < 0:
+                logger.debug(
+                    f"Deleting index {memory_index} out of range of 0-{len(self._memory)-1}")
+                return
         self._num_tokens_memory -= self._memory[memory_index].num_tokens
         del self._memory[memory_index]
 
     def to_messages(self):
         domain_knowledge_str = "No domain knowledge obtained"
         if self._domain_knowledge:
             domain_knowledge_str = f"Your domain knowledge is between the triple apostrophes: ```{';'.join([k.content for k in self._domain_knowledge])}```"
         commands_str = "No command"
         # TODO: Maybe it shouldn't be pronounced as
         if self._commands:
             commands_str = f"""The external tools you can use is between the triple apostrophes```{
                 ';'.join([c.to_prompt() for c in self._commands])
             }```"""
         commands_str = ""
-        logger.debug(f"context is { self._context}")
         return [
             {
                 "role": "system",
                 "content": self._context
             },
             {
                 "role": "system",
@@ -298,22 +322,16 @@
             [m.__str__() for m in self.get_memory()])
         return prefix + context_str + knowledge_str + memory_str + suffix
 
     def __repr__(self):
         return self.__str__()
 
     def __deepcopy__(self, memodict={}):
-        #          main_agent_config: Dict[any, any],
-        #  agents: Dict[str, BaseAgent],
-        #  context: str,
-        #  work_experience: List[Knowledge],
-        #  memory: List[MemoryUnit],
-        #  connector: BaseConnector):
-        cpyobj = type(self)(self._main_agent_config, self._helper_agents, self._context,
-                            self._domain_knowledge, self._memory, self.connector)  # shallow copy of whole object
+        cpyobj = type(self).init(self._agent._config,
+                                 self._memory, self._agent)  # shallow copy of whole object
         cpyobj._domain_knowledge = copy.deepcopy(
             self._domain_knowledge, memodict)
         cpyobj._commands = copy.deepcopy(
             self._commands, memodict)
         cpyobj._memory = copy.deepcopy(self._memory, memodict)
         cpyobj._helper_agents = {agent_name: copy.deepcopy(
             agent) for agent_name, agent in self._helper_agents.items()}
```

### Comparing `agentware-0.1.4/agentware/utils/json_fixes/auto_fix.py` & `agentware-0.1.5/agentware/utils/json_fixes/auto_fix.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.4/agentware/utils/json_fixes/bracket_termination.py` & `agentware-0.1.5/agentware/utils/json_fixes/bracket_termination.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.4/agentware/utils/json_fixes/escaping.py` & `agentware-0.1.5/agentware/utils/json_fixes/escaping.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.4/agentware/utils/json_fixes/master_json_fix_method.py` & `agentware-0.1.5/agentware/utils/json_fixes/master_json_fix_method.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.4/agentware/utils/json_fixes/missing_quotes.py` & `agentware-0.1.5/agentware/utils/json_fixes/missing_quotes.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.4/agentware/utils/json_fixes/parsing.py` & `agentware-0.1.5/agentware/utils/json_fixes/parsing.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.4/agentware/utils/json_fixes/utilities.py` & `agentware-0.1.5/agentware/utils/json_fixes/utilities.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.4/agentware/utils/json_validation/validate_json.py` & `agentware-0.1.5/agentware/utils/json_validation/validate_json.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.4/agentware/utils/num_token_utils.py` & `agentware-0.1.5/agentware/utils/num_token_utils.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.4/agentware.egg-info/SOURCES.txt` & `agentware-0.1.5/agentware.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 setup.py
 agentware/__init__.py
 agentware/agent.py
 agentware/agent_logger.py
 agentware/base.py
+agentware/core_engines.py
 agentware/error_codes.py
 agentware/hub.py
 agentware/memory.py
+agentware/perception.py
 agentware/singleton.py
 agentware.egg-info/PKG-INFO
 agentware.egg-info/SOURCES.txt
 agentware.egg-info/dependency_links.txt
 agentware.egg-info/requires.txt
 agentware.egg-info/top_level.txt
 agentware/utils/__init__.py
@@ -21,11 +23,13 @@
 agentware/utils/json_fixes/master_json_fix_method.py
 agentware/utils/json_fixes/missing_quotes.py
 agentware/utils/json_fixes/parsing.py
 agentware/utils/json_fixes/utilities.py
 agentware/utils/json_validation/__init__.py
 agentware/utils/json_validation/validate_json.py
 tests/__init__.py
-tests/agent_test.py
+tests/agent_workflow_test.py
+tests/config_test.py
 tests/connector_test.py
+tests/helper_agents_test.py
 tests/memory_test.py
 tests/utils.py
```

### Comparing `agentware-0.1.4/tests/agent_test.py` & `agentware-0.1.5/tests/agent_workflow_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,79 @@
 import unittest
-import json
-import agentware
 
 from agentware import hub
 from agentware.base import OneshotAgent, Connector
 from agentware.agent import Agent
 from agentware.agent_logger import Logger
-from tests.utils import DbClient
+from utils import DbClient, FakeCoreEngine, SummarizerCoreEngine, FactCoreEngine
 logger = Logger()
 
 TEST_CFG = {
-    "name": "test/3PO",
-    "description": ""
+    "name": "test agent",
+            "conversation_setup": "You are DarthHololens, an AI assistant who lives in the universe of Star Wars series and knows everything about this world",
+            "prompt_prefix": "Constraint: answer in no more than 200 tokens"
 }
 
 
-class AgentTests(unittest.TestCase):
+class AgentWorkflowTests(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         cls.db_client = DbClient()
+        cls.main_core_engine = FakeCoreEngine("software " * 200)
+        cls.summarizer_core_engine = FakeCoreEngine(
+            "{\"summary\": \"this is a summary\"}")
 
     def setUp(self):
-        self.db_client = DbClient()
+        self.db_client.client.flushall()
 
     def tearDown(self):
-        self.db_client.client.flushall()
+        pass
 
     def test_register_agent(self):
-        agent_id = "some agent id"
+        agent_id = "some agent idz"
         hub.register_agent(agent_id)
         agent_ids = hub.list_agents()
+        print('agents are', agent_ids)
         assert agent_ids[0] == agent_id
 
     def test_duplicate_register_fail(self):
         agent_id = "some_agent_id"
         hub.register_agent(agent_id)
         self.assertRaises(ValueError, hub.register_agent, agent_id)
 
     def test_fail_to_fetch_unexist(self):
-        self.assertRaises(ValueError, Agent.fetch, "some/unexisted")
+        self.assertRaises(ValueError, Agent.pull, "some/unexisted")
 
     def test_register_and_push_and_fetch_and_run_agent(self):
         agent = Agent()
         agent_id = "some_agent_name"
         agent.register(agent_id)
-        config = {
-            "name": "test agent",
-            "conversation_setup": "You are DarthHololens, an AI assistant who lives in the universe of Star Wars series and knows everything about this world",
-            "prompt_prefix": "Constraint: answer in no more than 200 tokens"
-        }
-        agent.set_config(config)
+        agent.set_config(TEST_CFG)
         agent.push()
         agents = hub.list_agents()
+        print("agents are", agents)
         assert agents[0] == agent_id
-        updated_agent = Agent.fetch(agent_id)
-        assert updated_agent.get_config() == config
-        # Run some queries until compression happens
+        updated_agent = Agent.pull(agent_id)
+        assert updated_agent.get_config() == TEST_CFG
+
+    def test_memory_compression(self):
+        agent = Agent.init(TEST_CFG)
+        agent.set_core_engine(self.main_core_engine)
+        agent._memory._helper_agents["summarizer"].set_core_engine(
+            SummarizerCoreEngine())
+        agent._memory._helper_agents["fact"].set_core_engine(
+            FactCoreEngine())
+        for i in range(10):
+            agent.run("What is your name?")
+
+    def test_agent_reflection_run_in_update_mode(self):
+        agent = Agent.init(TEST_CFG)
+        assert agent._update_mode == False
+        with agent.update():
+            assert agent._update_mode == True
+            agent.run("What is your name?")
+        assert agent._update_mode == False
 
 
 if __name__ == '__main__':
     unittest.main()
```

