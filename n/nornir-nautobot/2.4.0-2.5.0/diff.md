# Comparing `tmp/nornir_nautobot-2.4.0.tar.gz` & `tmp/nornir_nautobot-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_nautobot-2.4.0.tar", max compression
+gzip compressed data, was "nornir_nautobot-2.5.0.tar", max compression
```

## Comparing `nornir_nautobot-2.4.0.tar` & `nornir_nautobot-2.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1743 2023-06-07 15:16:40.651064 nornir_nautobot-2.4.0/README.md
--rw-r--r--   0        0        0       33 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/__init__.py
--rw-r--r--   0        0        0      126 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/exceptions.py
--rw-r--r--   0        0        0       33 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/__init__.py
--rw-r--r--   0        0        0       33 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/inventory/__init__.py
--rw-r--r--   0        0        0     5627 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/inventory/nautobot.py
--rw-r--r--   0        0        0     2667 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/processors/__init__.py
--rw-r--r--   0        0        0     5355 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/processors/get_config.py
--rw-r--r--   0        0        0     3647 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/__init__.py
--rw-r--r--   0        0        0      281 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/arista_eos.py
--rw-r--r--   0        0        0      250 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_asa.py
--rw-r--r--   0        0        0      250 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_ios.py
--rw-r--r--   0        0        0      256 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_ios_xr.py
--rw-r--r--   0        0        0      252 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_nxos.py
--rw-r--r--   0        0        0    17833 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/default.py
--rw-r--r--   0        0        0      320 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/juniper_junos.py
--rw-r--r--   0        0        0     4219 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros.py
--rw-r--r--   0        0        0     6214 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros_api.py
--rw-r--r--   0        0        0      299 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/ruckus_fastiron.py
--rw-r--r--   0        0        0     9095 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/ruckus_smartzone_api.py
--rw-r--r--   0        0        0      434 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/utils/helpers.py
--rw-r--r--   0        0        0     2119 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/utils/logger.py
--rw-r--r--   0        0        0      913 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/utils/mock.py
--rw-r--r--   0        0        0     2793 2023-06-07 15:16:52.463087 nornir_nautobot-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 nornir_nautobot-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1743 2023-08-02 18:53:06.129340 nornir_nautobot-2.5.0/README.md
+-rw-r--r--   0        0        0       33 2023-08-02 18:53:06.129340 nornir_nautobot-2.5.0/nornir_nautobot/__init__.py
+-rw-r--r--   0        0        0      126 2023-08-02 18:53:06.129340 nornir_nautobot-2.5.0/nornir_nautobot/exceptions.py
+-rw-r--r--   0        0        0       33 2023-08-02 18:53:06.129340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/__init__.py
+-rw-r--r--   0        0        0       33 2023-08-02 18:53:06.129340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/inventory/__init__.py
+-rw-r--r--   0        0        0     5627 2023-08-02 18:53:06.129340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/inventory/nautobot.py
+-rw-r--r--   0        0        0     2667 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/processors/__init__.py
+-rw-r--r--   0        0        0     5355 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/processors/get_config.py
+-rw-r--r--   0        0        0     3647 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/__init__.py
+-rw-r--r--   0        0        0      281 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/arista_eos.py
+-rw-r--r--   0        0        0      250 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_asa.py
+-rw-r--r--   0        0        0      250 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_ios.py
+-rw-r--r--   0        0        0      256 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_ios_xr.py
+-rw-r--r--   0        0        0      252 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_nxos.py
+-rw-r--r--   0        0        0    18042 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/default.py
+-rw-r--r--   0        0        0      320 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/juniper_junos.py
+-rw-r--r--   0        0        0     4219 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros.py
+-rw-r--r--   0        0        0     6214 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros_api.py
+-rw-r--r--   0        0        0      299 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/ruckus_fastiron.py
+-rw-r--r--   0        0        0     9095 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/ruckus_smartzone_api.py
+-rw-r--r--   0        0        0      434 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/utils/helpers.py
+-rw-r--r--   0        0        0     2119 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/utils/logger.py
+-rw-r--r--   0        0        0      913 2023-08-02 18:53:06.133340 nornir_nautobot-2.5.0/nornir_nautobot/utils/mock.py
+-rw-r--r--   0        0        0     2793 2023-08-02 18:53:20.913579 nornir_nautobot-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 nornir_nautobot-2.5.0/PKG-INFO
```

### Comparing `nornir_nautobot-2.4.0/README.md` & `nornir_nautobot-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.4.0/nornir_nautobot/plugins/inventory/nautobot.py` & `nornir_nautobot-2.5.0/nornir_nautobot/plugins/inventory/nautobot.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.4.0/nornir_nautobot/plugins/processors/__init__.py` & `nornir_nautobot-2.5.0/nornir_nautobot/plugins/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.4.0/nornir_nautobot/plugins/processors/get_config.py` & `nornir_nautobot-2.5.0/nornir_nautobot/plugins/processors/get_config.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/__init__.py` & `nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/default.py` & `nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,36 +158,39 @@
         task: Task,
         logger,
         obj,
         jinja_template: str,
         jinja_root_path: str,
         output_file_location: str,
         jinja_filters: Optional[dict] = None,
+        jinja_env: Optional[jinja2.Environment] = None,
     ) -> Result:
         """A small wrapper around template_file Nornir task.
 
         Args:
             task (Task): Nornir Task.
             logger (NornirLogger): Custom NornirLogger object to reflect job results (via Nautobot Jobs) and Python logger.
             obj (Device): A Nautobot Device Django ORM object instance.
             jinja_template (str): The file location of the actual Jinja template.
             jinja_root_path (str): The file folder where the file will be saved to.
             jinja_filters (dict): The filters which will be added to the jinja2 environment.
+            jinja_env (jinja2.Environment): The jinja2 environment to use. If not provided, nornir will create one.
             output_file_location (str): The filename where the file will be saved to.
 
         Returns:
             Result: Nornir Result object.
         """
         try:
             filled_template = task.run(
                 **task.host,
                 task=template_file,
                 template=jinja_template,
                 path=jinja_root_path,
                 jinja_filters=jinja_filters,
+                jinja_env=jinja_env,
             )[0].result
         except NornirSubTaskError as exc:
             if isinstance(exc.result.exception, jinja2.exceptions.UndefinedError):  # pylint: disable=no-else-raise
                 logger.log_failure(
                     obj,
                     f"There was a jinja2.exceptions.UndefinedError error: ``{str(exc.result.exception)}``",
                 )
```

### Comparing `nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros.py` & `nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros_api.py` & `nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros_api.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/ruckus_smartzone_api.py` & `nornir_nautobot-2.5.0/nornir_nautobot/plugins/tasks/dispatcher/ruckus_smartzone_api.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.4.0/nornir_nautobot/utils/logger.py` & `nornir_nautobot-2.5.0/nornir_nautobot/utils/logger.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.4.0/nornir_nautobot/utils/mock.py` & `nornir_nautobot-2.5.0/nornir_nautobot/utils/mock.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.4.0/pyproject.toml` & `nornir_nautobot-2.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir-nautobot"
-version = "v2.4.0"
+version = "v2.5.0"
 description = "Nornir Nautobot"
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Nautobot"]
 classifiers = [
   "Intended Audience :: Developers",
@@ -23,15 +23,15 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 nornir = "^3.0.0"
 requests = "^2.25.1"
 nornir-utils = "^0"
 nornir-napalm = ">=0.4.0 <1.0.0"
 nornir-jinja2 = "^0"
-nornir-netmiko = "^0"
+nornir-netmiko = "^1"
 pynautobot = "^1.0.1"
 netutils = "^1"
 routeros-api = {version = "^0.17.0", optional = true}
 httpx = "^0.24.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
```

### Comparing `nornir_nautobot-2.4.0/PKG-INFO` & `nornir_nautobot-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir-nautobot
-Version: 2.4.0
+Version: 2.5.0
 Summary: Nornir Nautobot
 Home-page: https://nautobot.com
 License: Apache-2.0
 Keywords: Nautobot
 Author: Network to Code, LLC
 Author-email: opensource@networktocode.com
 Requires-Python: >=3.7,<4.0
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: mikrotik-driver
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: netutils (>=1,<2)
 Requires-Dist: nornir (>=3.0.0,<4.0.0)
 Requires-Dist: nornir-jinja2 (>=0,<1)
 Requires-Dist: nornir-napalm (>=0.4.0,<1.0.0)
-Requires-Dist: nornir-netmiko (>=0,<1)
+Requires-Dist: nornir-netmiko (>=1,<2)
 Requires-Dist: nornir-utils (>=0,<1)
 Requires-Dist: pynautobot (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: routeros-api (>=0.17.0,<0.18.0) ; extra == "mikrotik-driver"
 Project-URL: Documentation, https://nornir-nautobot.readthedocs.io
 Project-URL: Repository, https://github.com/nautobot/nornir-nautobot
 Description-Content-Type: text/markdown
```

