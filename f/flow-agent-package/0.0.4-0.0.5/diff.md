# Comparing `tmp/flow-agent-package-0.0.4.tar.gz` & `tmp/flow-agent-package-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow-agent-package-0.0.4.tar", last modified: Wed Aug  2 18:53:03 2023, max compression
+gzip compressed data, was "flow-agent-package-0.0.5.tar", last modified: Wed Aug  2 20:06:44 2023, max compression
```

## Comparing `flow-agent-package-0.0.4.tar` & `flow-agent-package-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 18:53:03.052877 flow-agent-package-0.0.4/
--rw-rw-rw-   0        0        0       39 2023-08-02 16:07:21.000000 flow-agent-package-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      106 2023-08-02 18:53:03.051878 flow-agent-package-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 flow-agent-package-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 18:53:02.932009 flow-agent-package-0.0.4/flow_agent_package/
--rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 flow-agent-package-0.0.4/flow_agent_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 18:53:03.014230 flow-agent-package-0.0.4/flow_agent_package/tools/
--rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 flow-agent-package-0.0.4/flow_agent_package/tools/__init__.py
--rw-rw-rw-   0        0        0     6502 2023-08-02 18:48:29.000000 flow-agent-package-0.0.4/flow_agent_package/tools/agent_tool.py
--rw-rw-rw-   0        0        0     3682 2023-08-02 18:52:29.000000 flow-agent-package-0.0.4/flow_agent_package/tools/get_flow_tool.py
--rw-rw-rw-   0        0        0      784 2023-08-02 17:10:14.000000 flow-agent-package-0.0.4/flow_agent_package/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 18:53:03.031803 flow-agent-package-0.0.4/flow_agent_package/yamls/
--rw-rw-rw-   0        0        0      473 2023-08-02 16:47:19.000000 flow-agent-package-0.0.4/flow_agent_package/yamls/agent_tool.yaml
--rw-rw-rw-   0        0        0      378 2023-08-02 17:32:22.000000 flow-agent-package-0.0.4/flow_agent_package/yamls/get_flow_tool.yaml
-drwxrwxrwx   0        0        0        0 2023-08-02 18:53:02.962478 flow-agent-package-0.0.4/flow_agent_package.egg-info/
--rw-rw-rw-   0        0        0      106 2023-08-02 18:53:02.000000 flow-agent-package-0.0.4/flow_agent_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-08-02 18:53:02.000000 flow-agent-package-0.0.4/flow_agent_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 18:53:02.000000 flow-agent-package-0.0.4/flow_agent_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-08-02 18:53:02.000000 flow-agent-package-0.0.4/flow_agent_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-08-02 18:53:02.000000 flow-agent-package-0.0.4/flow_agent_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 18:53:03.052877 flow-agent-package-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      414 2023-08-02 18:52:55.000000 flow-agent-package-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 18:53:03.048880 flow-agent-package-0.0.4/tests/
--rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 flow-agent-package-0.0.4/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:06:44.655217 flow-agent-package-0.0.5/
+-rw-rw-rw-   0        0        0       39 2023-08-02 16:07:21.000000 flow-agent-package-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      106 2023-08-02 20:06:44.655217 flow-agent-package-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 flow-agent-package-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 20:06:44.536091 flow-agent-package-0.0.5/flow_agent_package/
+-rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 flow-agent-package-0.0.5/flow_agent_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:06:44.629664 flow-agent-package-0.0.5/flow_agent_package/tools/
+-rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 flow-agent-package-0.0.5/flow_agent_package/tools/__init__.py
+-rw-rw-rw-   0        0        0     6502 2023-08-02 18:48:29.000000 flow-agent-package-0.0.5/flow_agent_package/tools/agent_tool.py
+-rw-rw-rw-   0        0        0     3584 2023-08-02 19:56:33.000000 flow-agent-package-0.0.5/flow_agent_package/tools/get_flow_tool.py
+-rw-rw-rw-   0        0        0      784 2023-08-02 19:56:57.000000 flow-agent-package-0.0.5/flow_agent_package/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:06:44.643712 flow-agent-package-0.0.5/flow_agent_package/yamls/
+-rw-rw-rw-   0        0        0      473 2023-08-02 16:47:19.000000 flow-agent-package-0.0.5/flow_agent_package/yamls/agent_tool.yaml
+-rw-rw-rw-   0        0        0      378 2023-08-02 17:32:22.000000 flow-agent-package-0.0.5/flow_agent_package/yamls/get_flow_tool.yaml
+drwxrwxrwx   0        0        0        0 2023-08-02 20:06:44.571255 flow-agent-package-0.0.5/flow_agent_package.egg-info/
+-rw-rw-rw-   0        0        0      106 2023-08-02 20:06:44.000000 flow-agent-package-0.0.5/flow_agent_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-08-02 20:06:44.000000 flow-agent-package-0.0.5/flow_agent_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 20:06:44.000000 flow-agent-package-0.0.5/flow_agent_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-08-02 20:06:44.000000 flow-agent-package-0.0.5/flow_agent_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-08-02 20:06:44.000000 flow-agent-package-0.0.5/flow_agent_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 20:06:44.656217 flow-agent-package-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-08-02 19:58:15.000000 flow-agent-package-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:06:44.651217 flow-agent-package-0.0.5/tests/
+-rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 flow-agent-package-0.0.5/tests/test_my_tool_1.py
```

### Comparing `flow-agent-package-0.0.4/README.md` & `flow-agent-package-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.4/flow_agent_package/tools/agent_tool.py` & `flow-agent-package-0.0.5/flow_agent_package/tools/agent_tool.py`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.4/flow_agent_package/tools/get_flow_tool.py` & `flow-agent-package-0.0.5/flow_agent_package/tools/get_flow_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     batch_inputs = flow_json["flowRunSettings"]["batch_inputs"]
     connections = []
     for node in graph["nodes"]:
         if node.get("connection"):
             connections.append(node.get("connection"))
         if node.get("inputs", {}).get("connection"):
             connections.append(node["inputs"]["connection"])
-    print(f"connections: {connections}")
     connection_configs = {}
     for connection_name in set(connections):
         url = f"{endpoint}/rp/workspaces/subscriptions/{workspace.subscription_id}/resourcegroups/" + \
           f"{workspace.resource_group}/providers/Microsoft.MachineLearningServices/workspaces/" + \
           f"{workspace.name}/connections/{connection_name}/listsecrets?api-version=2023-02-01-preview"
 
         connection_json = requests.post(url, headers=headers).json()
@@ -69,15 +68,14 @@
                 "api_base": connection_json["properties"]["target"],
                 "api_type": "azure",
                 "api_version": "2023-03-15-preview"
             }
         }
         connection_configs[connection_name] = config
     
-    print(f"connection configs: {connection_configs}")
     final_json = {
         "flowId": correct_flow["flowId"],
         "flow": graph,
         "batch_inputs": batch_inputs,
         "connections": connection_configs
     }
     return final_json
```

### Comparing `flow-agent-package-0.0.4/flow_agent_package/tools/utils.py` & `flow-agent-package-0.0.5/flow_agent_package/tools/utils.py`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.4/flow_agent_package.egg-info/SOURCES.txt` & `flow-agent-package-0.0.5/flow_agent_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

