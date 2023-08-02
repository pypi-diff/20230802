# Comparing `tmp/cave_utils-1.5.3.tar.gz` & `tmp/cave_utils-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_utils-1.5.3.tar", last modified: Thu Jul 27 18:30:05 2023, max compression
+gzip compressed data, was "cave_utils-1.6.0.tar", last modified: Wed Aug  2 17:26:47 2023, max compression
```

## Comparing `cave_utils-1.5.3.tar` & `cave_utils-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-27 18:30:05.333078 cave_utils-1.5.3/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.3/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.3/NOTICE.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1602 2023-07-27 18:30:05.333078 cave_utils-1.5.3/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      927 2023-07-27 18:29:04.000000 cave_utils-1.5.3/README.md
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-27 18:30:05.333078 cave_utils-1.5.3/cave_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      131 2023-06-22 13:25:50.000000 cave_utils-1.5.3/cave_utils/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-06-27 13:54:10.000000 cave_utils-1.5.3/cave_utils/arguments.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1325 2023-06-16 14:30:37.000000 cave_utils-1.5.3/cave_utils/log.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-16 14:28:26.000000 cave_utils-1.5.3/cave_utils/socket.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    57226 2023-07-21 14:29:30.000000 cave_utils-1.5.3/cave_utils/validator.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-27 18:30:05.333078 cave_utils-1.5.3/cave_utils.egg-info/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1602 2023-07-27 18:30:05.000000 cave_utils-1.5.3/cave_utils.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      383 2023-07-27 18:30:05.000000 cave_utils-1.5.3/cave_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-27 18:30:05.000000 cave_utils-1.5.3/cave_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-07-27 18:30:05.000000 cave_utils-1.5.3/cave_utils.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-07-27 18:30:05.000000 cave_utils-1.5.3/cave_utils.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.3/pyproject.toml
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-27 18:30:05.333078 cave_utils-1.5.3/setup.cfg
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      993 2023-07-27 18:28:53.000000 cave_utils-1.5.3/setup.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-27 18:30:05.333078 cave_utils-1.5.3/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      305 2023-06-27 13:54:32.000000 cave_utils-1.5.3/test/test_arguments.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       39 2023-06-22 13:14:02.000000 cave_utils-1.5.3/test/test_import.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-08-02 17:26:47.056281 cave_utils-1.6.0/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.6.0/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.6.0/NOTICE.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     2550 2023-08-02 17:26:47.056281 cave_utils-1.6.0/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1874 2023-08-02 17:20:10.000000 cave_utils-1.6.0/README.md
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-08-02 17:26:47.056281 cave_utils-1.6.0/cave_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      131 2023-06-22 13:25:50.000000 cave_utils-1.6.0/cave_utils/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-06-27 13:54:10.000000 cave_utils-1.6.0/cave_utils/arguments.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1325 2023-06-16 14:30:37.000000 cave_utils-1.6.0/cave_utils/log.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-16 14:28:26.000000 cave_utils-1.6.0/cave_utils/socket.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    59194 2023-08-02 17:20:10.000000 cave_utils-1.6.0/cave_utils/validator.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-08-02 17:26:47.056281 cave_utils-1.6.0/cave_utils.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     2550 2023-08-02 17:26:47.000000 cave_utils-1.6.0/cave_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      383 2023-08-02 17:26:47.000000 cave_utils-1.6.0/cave_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-08-02 17:26:47.000000 cave_utils-1.6.0/cave_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-08-02 17:26:47.000000 cave_utils-1.6.0/cave_utils.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-08-02 17:26:47.000000 cave_utils-1.6.0/cave_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.6.0/pyproject.toml
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-08-02 17:26:47.056281 cave_utils-1.6.0/setup.cfg
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      993 2023-07-31 18:27:01.000000 cave_utils-1.6.0/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-08-02 17:26:47.056281 cave_utils-1.6.0/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      305 2023-06-27 13:54:32.000000 cave_utils-1.6.0/test/test_arguments.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       39 2023-06-22 13:14:02.000000 cave_utils-1.6.0/test/test_import.py
```

### Comparing `cave_utils-1.5.3/LICENSE` & `cave_utils-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.3/NOTICE.md` & `cave_utils-1.6.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.3/PKG-INFO` & `cave_utils-1.6.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: cave_utils
-Version: 1.5.3
-Summary: Cave utilities for the CAVE App at the MIT
-Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.3.tar.gz
-Author: Connor Makowski
-Author-email: connor.m.makowski@gmail.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE.md
-
 Cave Utilities for the Cave App
 ==========
 Basic utilities for the MIT Cave App. This package is intended to be used by the Cave App and the Cave API.
 
 Setup
 ----------
 
@@ -51,7 +32,35 @@
     # x.print_warnings()
     # x.write_warnings('./warnings.txt')
     # x.write_errors('./errors.txt')
     ```
 
 2. Run the following command:
     `cave test test_init.py`
+
+# Live Utils Development 
+1. In your cave_app, update the following file:
+
+    `utils/run_server.sh`
+    ```
+    #!/bin/bash
+
+    SCRIPT_DIR=$( cd -- "$( dirname -- "${BASH_SOURCE[0]}" )" &> /dev/null && pwd )
+    APP_DIR=$(dirname "$SCRIPT_DIR")
+
+    pip install -e /cave_utils
+
+    source ./utils/helpers/shell_functions.sh
+    source ./utils/helpers/ensure_postgres_running.sh
+    source ./utils/helpers/ensure_db_setup.sh
+
+    python "$APP_DIR/manage.py" runserver 0.0.0.0:8000 2>&1 | pipe_log "INFO"
+    ```
+
+2. In your cave_app, set `LIVE_API_VALIDATION=True` in the `.env` file
+    - This will validate your data every time an api command is called for each session
+    - Outputs will be stored in `logs/validation/{session_name}.log`
+
+3. Use the following command to run your cave_app:
+    `cave run --docker-args "--volume {local_path_to_cave_utils}/cave_utils:/cave_utils"`
+    
+    As you edit cave_utils, the logs will be updated live
```

### Comparing `cave_utils-1.5.3/cave_utils/arguments.py` & `cave_utils-1.6.0/cave_utils/arguments.py`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.3/cave_utils/log.py` & `cave_utils-1.6.0/cave_utils/log.py`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.3/cave_utils/validator.py` & `cave_utils-1.6.0/cave_utils/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -968,16 +968,16 @@
             "bar": str,
             "order": int,
             "color": dict,
             "apiCommand": str,
             "apiCommandKeys": list,
         }
         self.accepted_values = {
-            "type": ["map", "stats", "kpi", "pane", "button"],
-            "bar": ["upper", "lower"],
+            "type": ["map", "stats", "kpi", "pane", "modal", "button"],
+            "bar": ["upper", "lower", "upperLeft", "lowerLeft", "upperRight", "lowerRight"],
         }
         self.required_fields = ["icon", "type", "bar"]
         self.optional_fields = ["order", "color", "apiCommand", "apiCommandKeys"]
 
     def additional_validations(self, **kwargs):
         color = self.data.get("color")
         if color:
@@ -1380,14 +1380,73 @@
             "order",
         ]
 
         if is_optional_viewport:
             self.required_fields += ["icon", "name"]
 
 
+class ModalsValidator(CoreValidator):
+    def populate_data(self, **kwargs):
+        self.field_types = {
+            "data": dict,
+            "allowModification": bool,
+            "sendToApi": bool,
+            "sendToClient": bool,
+        }
+
+        self.accepted_values = {}
+
+        self.required_fields = ["data"]
+
+        self.optional_fields = ["allowModification", "sendToApi", "sendToClient"]
+
+    def additional_validations(self, **kwargs):
+        CustomKeyValidator(
+            data=self.data.get("data", {}),
+            log=self.log,
+            prepend_path=["data"],
+            validator=ModalsDataValidator,
+            **kwargs,
+        )
+
+
+class ModalsDataValidator(CoreValidator):
+    def populate_data(self, **kwargs):
+        self.field_types = {
+            "name": str,
+            "props": dict,
+            "layout": dict,
+            "teamSyncCommand": str,
+            "teamSyncCommandKeys": list,
+        }
+
+        self.accepted_values = {}
+
+        self.required_fields = ["name", "props"]
+
+        self.optional_fields = ["layout", "teamSyncCommand", "teamSyncCommandKeys"]
+
+    def additional_validations(self, **kwargs):
+        props_data = self.data.get("props", {})
+        CustomKeyValidator(
+            data=props_data,
+            log=self.log,
+            prepend_path=["props"],
+            validator=PropValidator,
+            **kwargs,
+        )
+        LayoutValidator(
+            data=self.data.get("layout", {}),
+            log=self.log,
+            prepend_path=["layout"],
+            acceptable_keys=list(props_data.keys()),
+            **kwargs,
+        )
+
+
 class PanesValidator(CoreValidator):
     def populate_data(self, **kwargs):
         self.field_types = {
             "data": dict,
             "allowModification": bool,
             "sendToApi": bool,
             "sendToClient": bool,
@@ -1601,14 +1660,15 @@
             "arcs": dict,
             "categories": dict,
             "dashboards": dict,
             "geos": dict,
             "kpis": dict,
             "kwargs": dict,
             "maps": dict,
+            "modals": dict,
             "nodes": dict,
             "panes": dict,
             "settings": dict,
             "stats": dict,
         }
         self.required_fields = [
             "appBar",
@@ -1619,15 +1679,15 @@
             "kpis",
             "maps",
             "nodes",
             "panes",
             "settings",
             "stats",
         ]
-        self.optional_fields = ["kwargs"]
+        self.optional_fields = ["kwargs", "modals"]
         self.accepted_values = {}
 
     def additional_validations(self, **kwargs):
         # Validate Categories
         ## Note this happens first to give useful feedback as categories are used in other validations
         CategoriesValidator(
             data=self.data.get("categories", {}),
@@ -1729,14 +1789,23 @@
             categories_key_levels=categories_key_levels,
             node_prop_options=node_prop_options,
             arc_prop_options=arc_prop_options,
             geo_prop_options=geo_prop_options,
             **kwargs,
         )
 
+        # Validate Modals
+        ModalsValidator(
+            data=self.data.get("modals", {}),
+            log=self.log,
+            prepend_path=["modals"],
+            categories_key_values=categories_key_values,
+            **kwargs,
+        )
+
         # Validate Panes
         PanesValidator(
             data=self.data.get("panes", {}),
             log=self.log,
             prepend_path=["panes"],
             categories_key_values=categories_key_values,
             **kwargs,
```

### Comparing `cave_utils-1.5.3/cave_utils.egg-info/PKG-INFO` & `cave_utils-1.6.0/cave_utils.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cave-utils
-Version: 1.5.3
+Version: 1.6.0
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.3.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.6.0.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
@@ -51,7 +51,35 @@
     # x.print_warnings()
     # x.write_warnings('./warnings.txt')
     # x.write_errors('./errors.txt')
     ```
 
 2. Run the following command:
     `cave test test_init.py`
+
+# Live Utils Development 
+1. In your cave_app, update the following file:
+
+    `utils/run_server.sh`
+    ```
+    #!/bin/bash
+
+    SCRIPT_DIR=$( cd -- "$( dirname -- "${BASH_SOURCE[0]}" )" &> /dev/null && pwd )
+    APP_DIR=$(dirname "$SCRIPT_DIR")
+
+    pip install -e /cave_utils
+
+    source ./utils/helpers/shell_functions.sh
+    source ./utils/helpers/ensure_postgres_running.sh
+    source ./utils/helpers/ensure_db_setup.sh
+
+    python "$APP_DIR/manage.py" runserver 0.0.0.0:8000 2>&1 | pipe_log "INFO"
+    ```
+
+2. In your cave_app, set `LIVE_API_VALIDATION=True` in the `.env` file
+    - This will validate your data every time an api command is called for each session
+    - Outputs will be stored in `logs/validation/{session_name}.log`
+
+3. Use the following command to run your cave_app:
+    `cave run --docker-args "--volume {local_path_to_cave_utils}/cave_utils:/cave_utils"`
+    
+    As you edit cave_utils, the logs will be updated live
```

### Comparing `cave_utils-1.5.3/setup.py` & `cave_utils-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'cave_utils',
   packages=['cave_utils'],
-  version = '1.5.3',
+  version = '1.6.0',
   license='MIT',
   description = 'Cave utilities for the CAVE App at the MIT',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'connor.m.makowski@gmail.com',
   url = 'https://github.com/mit-cave/cave_utils',
-  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.3.tar.gz',
+  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.6.0.tar.gz',
   keywords = [],
   install_requires=[
     'pamda>=2.1.2',
   ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

