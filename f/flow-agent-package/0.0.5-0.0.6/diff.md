# Comparing `tmp/flow-agent-package-0.0.5.tar.gz` & `tmp/flow-agent-package-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow-agent-package-0.0.5.tar", last modified: Wed Aug  2 20:06:44 2023, max compression
+gzip compressed data, was "flow-agent-package-0.0.6.tar", last modified: Wed Aug  2 20:33:36 2023, max compression
```

## Comparing `flow-agent-package-0.0.5.tar` & `flow-agent-package-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:44.655217 flow-agent-package-0.0.5/
--rw-rw-rw-   0        0        0       39 2023-08-02 16:07:21.000000 flow-agent-package-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      106 2023-08-02 20:06:44.655217 flow-agent-package-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 flow-agent-package-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:44.536091 flow-agent-package-0.0.5/flow_agent_package/
--rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 flow-agent-package-0.0.5/flow_agent_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:44.629664 flow-agent-package-0.0.5/flow_agent_package/tools/
--rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 flow-agent-package-0.0.5/flow_agent_package/tools/__init__.py
--rw-rw-rw-   0        0        0     6502 2023-08-02 18:48:29.000000 flow-agent-package-0.0.5/flow_agent_package/tools/agent_tool.py
--rw-rw-rw-   0        0        0     3584 2023-08-02 19:56:33.000000 flow-agent-package-0.0.5/flow_agent_package/tools/get_flow_tool.py
--rw-rw-rw-   0        0        0      784 2023-08-02 19:56:57.000000 flow-agent-package-0.0.5/flow_agent_package/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:44.643712 flow-agent-package-0.0.5/flow_agent_package/yamls/
--rw-rw-rw-   0        0        0      473 2023-08-02 16:47:19.000000 flow-agent-package-0.0.5/flow_agent_package/yamls/agent_tool.yaml
--rw-rw-rw-   0        0        0      378 2023-08-02 17:32:22.000000 flow-agent-package-0.0.5/flow_agent_package/yamls/get_flow_tool.yaml
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:44.571255 flow-agent-package-0.0.5/flow_agent_package.egg-info/
--rw-rw-rw-   0        0        0      106 2023-08-02 20:06:44.000000 flow-agent-package-0.0.5/flow_agent_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-08-02 20:06:44.000000 flow-agent-package-0.0.5/flow_agent_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 20:06:44.000000 flow-agent-package-0.0.5/flow_agent_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-08-02 20:06:44.000000 flow-agent-package-0.0.5/flow_agent_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-08-02 20:06:44.000000 flow-agent-package-0.0.5/flow_agent_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 20:06:44.656217 flow-agent-package-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-08-02 19:58:15.000000 flow-agent-package-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:44.651217 flow-agent-package-0.0.5/tests/
--rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 flow-agent-package-0.0.5/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:33:36.771934 flow-agent-package-0.0.6/
+-rw-rw-rw-   0        0        0       39 2023-08-02 16:07:21.000000 flow-agent-package-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      106 2023-08-02 20:33:36.770934 flow-agent-package-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 flow-agent-package-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 20:33:36.734902 flow-agent-package-0.0.6/flow_agent_package/
+-rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 flow-agent-package-0.0.6/flow_agent_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:33:36.762926 flow-agent-package-0.0.6/flow_agent_package/tools/
+-rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 flow-agent-package-0.0.6/flow_agent_package/tools/__init__.py
+-rw-rw-rw-   0        0        0     6502 2023-08-02 18:48:29.000000 flow-agent-package-0.0.6/flow_agent_package/tools/agent_tool.py
+-rw-rw-rw-   0        0        0     3584 2023-08-02 19:56:33.000000 flow-agent-package-0.0.6/flow_agent_package/tools/get_flow_tool.py
+-rw-rw-rw-   0        0        0      784 2023-08-02 19:56:57.000000 flow-agent-package-0.0.6/flow_agent_package/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:33:36.767934 flow-agent-package-0.0.6/flow_agent_package/yamls/
+-rw-rw-rw-   0        0        0      520 2023-08-02 20:32:04.000000 flow-agent-package-0.0.6/flow_agent_package/yamls/agent_tool.yaml
+-rw-rw-rw-   0        0        0      407 2023-08-02 20:31:48.000000 flow-agent-package-0.0.6/flow_agent_package/yamls/get_flow_tool.yaml
+drwxrwxrwx   0        0        0        0 2023-08-02 20:33:36.752416 flow-agent-package-0.0.6/flow_agent_package.egg-info/
+-rw-rw-rw-   0        0        0      106 2023-08-02 20:33:36.000000 flow-agent-package-0.0.6/flow_agent_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-08-02 20:33:36.000000 flow-agent-package-0.0.6/flow_agent_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 20:33:36.000000 flow-agent-package-0.0.6/flow_agent_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-08-02 20:33:36.000000 flow-agent-package-0.0.6/flow_agent_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-08-02 20:33:36.000000 flow-agent-package-0.0.6/flow_agent_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 20:33:36.772934 flow-agent-package-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-08-02 20:33:30.000000 flow-agent-package-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:33:36.768934 flow-agent-package-0.0.6/tests/
+-rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 flow-agent-package-0.0.6/tests/test_my_tool_1.py
```

### Comparing `flow-agent-package-0.0.5/README.md` & `flow-agent-package-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.5/flow_agent_package/tools/agent_tool.py` & `flow-agent-package-0.0.6/flow_agent_package/tools/agent_tool.py`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.5/flow_agent_package/tools/get_flow_tool.py` & `flow-agent-package-0.0.6/flow_agent_package/tools/get_flow_tool.py`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.5/flow_agent_package/tools/utils.py` & `flow-agent-package-0.0.6/flow_agent_package/tools/utils.py`

 * *Files identical despite different names*

### Comparing `flow-agent-package-0.0.5/flow_agent_package.egg-info/SOURCES.txt` & `flow-agent-package-0.0.6/flow_agent_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

