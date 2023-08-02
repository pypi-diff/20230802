# Comparing `tmp/agentaction-0.1.5.tar.gz` & `tmp/agentaction-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentaction-0.1.5.tar", last modified: Fri Jul 28 08:03:22 2023, max compression
+gzip compressed data, was "agentaction-0.1.7.tar", last modified: Wed Aug  2 00:59:58 2023, max compression
```

## Comparing `agentaction-0.1.5.tar` & `agentaction-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:22.773369 agentaction-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-28 08:03:12.000000 agentaction-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-28 08:03:22.773369 agentaction-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-28 08:03:12.000000 agentaction-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:22.773369 agentaction-0.1.5/agentaction/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-28 08:03:12.000000 agentaction-0.1.5/agentaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-07-28 08:03:12.000000 agentaction-0.1.5/agentaction/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:22.773369 agentaction-0.1.5/agentaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-28 08:03:22.000000 agentaction-0.1.5/agentaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 08:03:22.000000 agentaction-0.1.5/agentaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:03:22.000000 agentaction-0.1.5/agentaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 08:03:22.000000 agentaction-0.1.5/agentaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 08:03:22.000000 agentaction-0.1.5/agentaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:03:22.773369 agentaction-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-28 08:03:12.000000 agentaction-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:59:58.160959 agentaction-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-02 00:59:42.000000 agentaction-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-02 00:59:58.160959 agentaction-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-08-02 00:59:42.000000 agentaction-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:59:58.160959 agentaction-0.1.7/agentaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-02 00:59:42.000000 agentaction-0.1.7/agentaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-08-02 00:59:42.000000 agentaction-0.1.7/agentaction/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:59:58.160959 agentaction-0.1.7/agentaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-02 00:59:58.000000 agentaction-0.1.7/agentaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-02 00:59:58.000000 agentaction-0.1.7/agentaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:59:58.000000 agentaction-0.1.7/agentaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 00:59:58.000000 agentaction-0.1.7/agentaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 00:59:58.000000 agentaction-0.1.7/agentaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:59:58.160959 agentaction-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-02 00:59:42.000000 agentaction-0.1.7/setup.py
```

### Comparing `agentaction-0.1.5/LICENSE` & `agentaction-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agentaction-0.1.5/PKG-INFO` & `agentaction-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentaction
-Version: 0.1.5
+Version: 0.1.7
 Summary: Action chaining and history for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentaction
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -16,14 +16,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 Action chaining and history for agents
 
 
+[![Lint and Test](https://github.com/AutonomousResearchGroup/agentaction/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentaction/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/agentaction.svg)](https://badge.fury.io/py/agentaction)
+
 # Why Use This?
 This package helps manage and simplify the task of handling actions for an agent, especially a looping agent with chained functions. Actions can be anything, but the intended purpose is to work with openai function calling or other JSON/function calling LLM completion paradigms.
 
 This package facilitates action creation, retrieval, and management, all while supporting vector search powered by chromadb to efficiently locate relevant actions.
 
 # Installation
 
@@ -70,15 +73,15 @@
 
 # Import the actions
 import_actions("./actions")
 
 # Use an action
 result = use_action("sample_function", {"name": "John"})
 actions = search_actions("hello")
-print(result)  # Should print: {"success": True, "result": "Hello, John"}
+print(result)  # Should print: {"success": True, "output": "Hello, John"}
 ```
 
 You can use the `get_available_actions` and `get_action` functions to search for and retrieve actions, respectively. And, don't forget to use the `add_to_action_history` function to keep track of which actions your agent has performed.
 
 ## Usage Guide
 
 ### Action Creation and Addition
```

### Comparing `agentaction-0.1.5/README.md` & `agentaction-0.1.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # agentaction <a href="https://discord.gg/qetWd7J9De"><img style="float: right" src="https://dcbadge.vercel.app/api/server/qetWd7J9De" alt=""></a>
 
 Action chaining and history for agents
 
 <img src="resources/image.jpg">
 
+[![Lint and Test](https://github.com/AutonomousResearchGroup/agentaction/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentaction/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/agentaction.svg)](https://badge.fury.io/py/agentaction)
+
 # Why Use This?
 This package helps manage and simplify the task of handling actions for an agent, especially a looping agent with chained functions. Actions can be anything, but the intended purpose is to work with openai function calling or other JSON/function calling LLM completion paradigms.
 
 This package facilitates action creation, retrieval, and management, all while supporting vector search powered by chromadb to efficiently locate relevant actions.
 
 # Installation
 
@@ -54,15 +57,15 @@
 
 # Import the actions
 import_actions("./actions")
 
 # Use an action
 result = use_action("sample_function", {"name": "John"})
 actions = search_actions("hello")
-print(result)  # Should print: {"success": True, "result": "Hello, John"}
+print(result)  # Should print: {"success": True, "output": "Hello, John"}
 ```
 
 You can use the `get_available_actions` and `get_action` functions to search for and retrieve actions, respectively. And, don't forget to use the `add_to_action_history` function to keep track of which actions your agent has performed.
 
 ## Usage Guide
 
 ### Action Creation and Addition
```

### Comparing `agentaction-0.1.5/agentaction/__init__.py` & `agentaction-0.1.7/agentaction/__init__.py`

 * *Files identical despite different names*

### Comparing `agentaction-0.1.5/agentaction/main.py` & `agentaction-0.1.7/agentaction/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     create_memory,
     delete_memory,
     get_memories,
     search_memory,
     wipe_category,
 )
 
+from agentlogger import log
+
 # Create an empty dictionary to hold the actions
 actions = {}
 
 
 def compose_action_prompt(action, values):
     """
     Composes a prompt based on the given action and observation.
@@ -164,24 +166,23 @@
     Arguments:
     function_name (str): The name of the action's function to execute.
     arguments (dict): The arguments required by the action's function.
 
     Returns:
     dict: Contains the "success" key
             True if the action was found and executed, otherwise False.
-            If the action was found and executed, also contains "result" key
+            If the action was found and executed, also contains "output" key
     """
     if function_name not in actions:
         add_to_action_history(function_name, arguments, success=False)
-        return {"success": False, "response": "Action not found"}
+        log("Warning: action was hallucinated: " + function_name, type="warning")
+        return {"success": False, "output": None, "error": "Action not found"}
 
     add_to_action_history(function_name, arguments)
-    result = actions[function_name]["handler"](arguments)
-
-    return {"success": True, "result": result}
+    return actions[function_name]["handler"](arguments)
 
 
 def add_action(name, action):
     """
     Add an action to the actions dictionary and 'actions' collection in memory.
 
     Arguments:
```

### Comparing `agentaction-0.1.5/agentaction.egg-info/PKG-INFO` & `agentaction-0.1.7/agentaction.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentaction
-Version: 0.1.5
+Version: 0.1.7
 Summary: Action chaining and history for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentaction
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -16,14 +16,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 Action chaining and history for agents
 
 
+[![Lint and Test](https://github.com/AutonomousResearchGroup/agentaction/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentaction/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/agentaction.svg)](https://badge.fury.io/py/agentaction)
+
 # Why Use This?
 This package helps manage and simplify the task of handling actions for an agent, especially a looping agent with chained functions. Actions can be anything, but the intended purpose is to work with openai function calling or other JSON/function calling LLM completion paradigms.
 
 This package facilitates action creation, retrieval, and management, all while supporting vector search powered by chromadb to efficiently locate relevant actions.
 
 # Installation
 
@@ -70,15 +73,15 @@
 
 # Import the actions
 import_actions("./actions")
 
 # Use an action
 result = use_action("sample_function", {"name": "John"})
 actions = search_actions("hello")
-print(result)  # Should print: {"success": True, "result": "Hello, John"}
+print(result)  # Should print: {"success": True, "output": "Hello, John"}
 ```
 
 You can use the `get_available_actions` and `get_action` functions to search for and retrieve actions, respectively. And, don't forget to use the `add_to_action_history` function to keep track of which actions your agent has performed.
 
 ## Usage Guide
 
 ### Action Creation and Addition
```

### Comparing `agentaction-0.1.5/setup.py` & `agentaction-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = [line for line in readme if "<img" not in line]
     # now join all the lines back together
     readme = "\n".join(readme)
 
 
 setup(
     name="agentaction",
-    version="0.1.5",
+    version="0.1.7",
     description="Action chaining and history for agents",
     long_description=readme,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentaction",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

