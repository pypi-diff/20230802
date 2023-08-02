# Comparing `tmp/flow-agent-package-0.0.1.tar.gz` & `tmp/flow-agent-package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow-agent-package-0.0.1.tar", last modified: Wed Aug  2 16:51:22 2023, max compression
+gzip compressed data, was "flow-agent-package-0.0.2.tar", last modified: Wed Aug  2 17:11:17 2023, max compression
```

## Comparing `flow-agent-package-0.0.1.tar` & `flow-agent-package-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 16:51:22.980901 flow-agent-package-0.0.1/
--rw-rw-rw-   0        0        0       39 2023-08-02 16:07:21.000000 flow-agent-package-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      106 2023-08-02 16:51:22.979903 flow-agent-package-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 flow-agent-package-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 16:51:22.846152 flow-agent-package-0.0.1/flow_agent_package/
--rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 flow-agent-package-0.0.1/flow_agent_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:51:22.939832 flow-agent-package-0.0.1/flow_agent_package/tools/
--rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 flow-agent-package-0.0.1/flow_agent_package/tools/__init__.py
--rw-rw-rw-   0        0        0     6528 2023-08-02 16:47:37.000000 flow-agent-package-0.0.1/flow_agent_package/tools/agent_tool.py
--rw-rw-rw-   0        0        0     3638 2023-08-02 16:09:41.000000 flow-agent-package-0.0.1/flow_agent_package/tools/get_flow_tool.py
--rw-rw-rw-   0        0        0      253 2023-08-02 16:08:42.000000 flow-agent-package-0.0.1/flow_agent_package/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:51:22.962867 flow-agent-package-0.0.1/flow_agent_package/yamls/
--rw-rw-rw-   0        0        0      473 2023-08-02 16:47:19.000000 flow-agent-package-0.0.1/flow_agent_package/yamls/agent_tool.yaml
--rw-rw-rw-   0        0        0      372 2023-08-02 16:36:17.000000 flow-agent-package-0.0.1/flow_agent_package/yamls/get_flow_tool.yaml
-drwxrwxrwx   0        0        0        0 2023-08-02 16:51:22.887316 flow-agent-package-0.0.1/flow_agent_package.egg-info/
--rw-rw-rw-   0        0        0      106 2023-08-02 16:51:22.000000 flow-agent-package-0.0.1/flow_agent_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-08-02 16:51:22.000000 flow-agent-package-0.0.1/flow_agent_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 16:51:22.000000 flow-agent-package-0.0.1/flow_agent_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-08-02 16:51:22.000000 flow-agent-package-0.0.1/flow_agent_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-08-02 16:51:22.000000 flow-agent-package-0.0.1/flow_agent_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 16:51:22.981901 flow-agent-package-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      414 2023-08-02 16:50:41.000000 flow-agent-package-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:51:22.978900 flow-agent-package-0.0.1/tests/
--rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 flow-agent-package-0.0.1/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:11:17.795108 flow-agent-package-0.0.2/
+-rw-rw-rw-   0        0        0       39 2023-08-02 16:07:21.000000 flow-agent-package-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      106 2023-08-02 17:11:17.794056 flow-agent-package-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 flow-agent-package-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 17:11:17.755938 flow-agent-package-0.0.2/flow_agent_package/
+-rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 flow-agent-package-0.0.2/flow_agent_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:11:17.787056 flow-agent-package-0.0.2/flow_agent_package/tools/
+-rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 flow-agent-package-0.0.2/flow_agent_package/tools/__init__.py
+-rw-rw-rw-   0        0        0     6528 2023-08-02 16:47:37.000000 flow-agent-package-0.0.2/flow_agent_package/tools/agent_tool.py
+-rw-rw-rw-   0        0        0     3638 2023-08-02 16:09:41.000000 flow-agent-package-0.0.2/flow_agent_package/tools/get_flow_tool.py
+-rw-rw-rw-   0        0        0      784 2023-08-02 17:10:14.000000 flow-agent-package-0.0.2/flow_agent_package/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:11:17.792065 flow-agent-package-0.0.2/flow_agent_package/yamls/
+-rw-rw-rw-   0        0        0      473 2023-08-02 16:47:19.000000 flow-agent-package-0.0.2/flow_agent_package/yamls/agent_tool.yaml
+-rw-rw-rw-   0        0        0      372 2023-08-02 16:36:17.000000 flow-agent-package-0.0.2/flow_agent_package/yamls/get_flow_tool.yaml
+drwxrwxrwx   0        0        0        0 2023-08-02 17:11:17.779524 flow-agent-package-0.0.2/flow_agent_package.egg-info/
+-rw-rw-rw-   0        0        0      106 2023-08-02 17:11:17.000000 flow-agent-package-0.0.2/flow_agent_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-08-02 17:11:17.000000 flow-agent-package-0.0.2/flow_agent_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 17:11:17.000000 flow-agent-package-0.0.2/flow_agent_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-08-02 17:11:17.000000 flow-agent-package-0.0.2/flow_agent_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-08-02 17:11:17.000000 flow-agent-package-0.0.2/flow_agent_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 17:11:17.795108 flow-agent-package-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      414 2023-08-02 17:11:12.000000 flow-agent-package-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:11:17.793055 flow-agent-package-0.0.2/tests/
+-rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 flow-agent-package-0.0.2/tests/test_my_tool_1.py
```

### Comparing `flow-agent-package-0.0.1/README.md` & `flow-agent-package-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.1/flow_agent_package/tools/agent_tool.py` & `flow-agent-package-0.0.2/flow_agent_package/tools/agent_tool.py`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.1/flow_agent_package/tools/get_flow_tool.py` & `flow-agent-package-0.0.2/flow_agent_package/tools/get_flow_tool.py`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.1/flow_agent_package.egg-info/SOURCES.txt` & `flow-agent-package-0.0.2/flow_agent_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

