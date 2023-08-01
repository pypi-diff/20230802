# Comparing `tmp/classroom_extensions-0.0.6.tar.gz` & `tmp/classroom_extensions-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classroom_extensions-0.0.6.tar", last modified: Fri Jul 21 22:34:11 2023, max compression
+gzip compressed data, was "classroom_extensions-0.0.7.tar", last modified: Tue Aug  1 22:20:34 2023, max compression
```

## Comparing `classroom_extensions-0.0.6.tar` & `classroom_extensions-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:34:11.209051 classroom_extensions-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-07-21 22:34:11.209051 classroom_extensions-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:34:11.209051 classroom_extensions-0.0.6/classroom_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/mariadb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/mariadb_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/mongodb_install.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/plantuml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:34:11.209051 classroom_extensions-0.0.6/classroom_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-07-21 22:34:11.000000 classroom_extensions-0.0.6/classroom_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-21 22:34:11.000000 classroom_extensions-0.0.6/classroom_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:34:11.000000 classroom_extensions-0.0.6/classroom_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 22:34:11.000000 classroom_extensions-0.0.6/classroom_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-21 22:34:11.000000 classroom_extensions-0.0.6/classroom_extensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:34:11.209051 classroom_extensions-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:34:11.209051 classroom_extensions-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/tests/test_mariadb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/tests/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/tests/test_nodejs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/tests/test_plantuml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:20:34.853248 classroom_extensions-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-08-01 22:20:34.853248 classroom_extensions-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:20:34.853248 classroom_extensions-0.0.7/classroom_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/mariadb_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/mongodb_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/plantuml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:20:34.853248 classroom_extensions-0.0.7/classroom_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-08-01 22:20:34.000000 classroom_extensions-0.0.7/classroom_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 22:20:34.000000 classroom_extensions-0.0.7/classroom_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:20:34.000000 classroom_extensions-0.0.7/classroom_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 22:20:34.000000 classroom_extensions-0.0.7/classroom_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 22:20:34.000000 classroom_extensions-0.0.7/classroom_extensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:20:34.853248 classroom_extensions-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:20:34.853248 classroom_extensions-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/tests/test_mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/tests/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/tests/test_plantuml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/tests/test_web.py
```

### Comparing `classroom_extensions-0.0.6/LICENSE` & `classroom_extensions-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.6/PKG-INFO` & `classroom_extensions-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classroom_extensions
-Version: 0.0.6
+Version: 0.0.7
 Summary: IPython extensions used for teaching
 Author-email: Marcos Dias de Assuncao <assuncao@acm.org>
 Maintainer-email: Marcos Dias de Assuncao <assuncao@acm.org>
 License: MIT
 Project-URL: Homepage, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Bug Reports, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Say Thanks!, https://saythanks.io/to/assuncaomarcos
@@ -79,27 +79,27 @@
 To ease the creation of notebooks on Google Colab, a second extension (`mariadb_install`)
 installs MariaDB and the required libraries to run the first extension without
 worrying about setting things up.
 
 Server-Side JavaScript
 ----------------------
 
-This extension, called `node`, customizes the `%%javascript` cell magic to enable
+This extension, called `web`, customizes the `%%javascript` cell magic to enable
 executing JavaScript code on the server or container hosting the Jupyter Notebook or
 on Google Colab. Node.js executes the code provided in a cell whose `--target` argument
-receives the value `node`. It also enables starting long-running Node.js server
+receives the value `web`. It also enables starting long-running Node.js server
 processes that will listen on given ports without blocking the code cell of
 the notebook. In addition to executing JavaScript code on the server side, when run
 on the browser, the magic enables printing the output of the browser's console in
 the result section of the code cell.
 
 Custom HTML Magic
 -----------------
 
-The `html` extension customizes the `%%html` magic. After rendering the HTML code
+The `web` extension also customizes the `%%html` magic. After rendering the HTML code
 inserted in the cell, the extension displays a high-level copy of the browser's
 console. This behavior helps in teaching HTML or JavaScript that writes on the console.
 
 PlantUML Magics
 ---------------
 
 PlantUML is a textual Domain-Specific Language (DSL) used for creating diagrams,
```

### Comparing `classroom_extensions-0.0.6/README.rst` & `classroom_extensions-0.0.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,27 @@
 To ease the creation of notebooks on Google Colab, a second extension (`mariadb_install`)
 installs MariaDB and the required libraries to run the first extension without
 worrying about setting things up.
 
 Server-Side JavaScript
 ----------------------
 
-This extension, called `node`, customizes the `%%javascript` cell magic to enable
+This extension, called `web`, customizes the `%%javascript` cell magic to enable
 executing JavaScript code on the server or container hosting the Jupyter Notebook or
 on Google Colab. Node.js executes the code provided in a cell whose `--target` argument
-receives the value `node`. It also enables starting long-running Node.js server
+receives the value `web`. It also enables starting long-running Node.js server
 processes that will listen on given ports without blocking the code cell of
 the notebook. In addition to executing JavaScript code on the server side, when run
 on the browser, the magic enables printing the output of the browser's console in
 the result section of the code cell.
 
 Custom HTML Magic
 -----------------
 
-The `html` extension customizes the `%%html` magic. After rendering the HTML code
+The `web` extension also customizes the `%%html` magic. After rendering the HTML code
 inserted in the cell, the extension displays a high-level copy of the browser's
 console. This behavior helps in teaching HTML or JavaScript that writes on the console.
 
 PlantUML Magics
 ---------------
 
 PlantUML is a textual Domain-Specific Language (DSL) used for creating diagrams,
```

### Comparing `classroom_extensions-0.0.6/classroom_extensions/mariadb.py` & `classroom_extensions-0.0.7/classroom_extensions/mariadb.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.6/classroom_extensions/mariadb_install.py` & `classroom_extensions-0.0.7/classroom_extensions/mariadb_install.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 # -*- coding: utf-8 -*-
 
 """
 An extension to install MariaDB, create the config file required by the
 MariaDB Jupyter to access it, and load a sample database.
 
 Note: This extension assumes that you are working in Google Colab
-running Ubuntu 20.04.
+running Ubuntu 22.04.
 """
 import time
 from os import path
 import json
 from argparse import ArgumentParser
 from IPython.core.magic import magics_class, line_magic, Magics
 from IPython.core.getipython import get_ipython
 from .util import exec_cmd, get_os_release, is_colab, get_user
 
-SAMPLE_DB = "https://www.mariadbtutorial.com/wp-content/uploads/2019/10/nation.zip"
-START_DB_TIMEOUT = 5  # Timeout for starting MariaDB
+__all__ = ["load_ipython_extension", "unload_ipython_extension", "MariaDBInstaller"]
+
+_SAMPLE_DB = "https://www.mariadbtutorial.com/wp-content/uploads/2019/10/nation.zip"
+_START_DB_TIMEOUT = 5  # Timeout for starting MariaDB
 
 
 @magics_class
 class MariaDBInstaller(Magics):
     """
     Implements the behaviour of the magic for installing MariaDB on Google Colab.
     """
@@ -62,22 +64,22 @@
         Check if running on Colab with the right Ubuntu release
 
         Returns:
             True if running on Google Colab on Ubuntu 2x.xx container
         """
         return is_colab() and get_os_release().startswith("2")
 
-    @classmethod
-    def _start_mariadb(cls) -> None:
+    @staticmethod
+    def _start_mariadb() -> None:
         """Starts MariaDB"""
 
         service_name = "mariadb" if get_os_release().startswith("22") else "mysql"
         get_ipython().system_raw(f"service {service_name} start &")
         print("Waiting for a few seconds for MariaDB server to start...")
-        time.sleep(START_DB_TIMEOUT)
+        time.sleep(_START_DB_TIMEOUT)
 
     @line_magic
     def install_mariadb(self, line: str):
         """Install MariaDB, mariadb_kernel, sqlparse, etc"""
 
         if not self._meet_requirements():
             print(
@@ -123,15 +125,15 @@
         # Load the sample database, if required
         if load_sample_db:
             self._load_sample_db()
         print("Done.")
 
     def _load_sample_db(self):
         """Configure a sample MariaDB database"""
-        exec_cmd(f"wget {SAMPLE_DB}")
+        exec_cmd(f"wget {_SAMPLE_DB}")
         exec_cmd("unzip -o nation.zip")
         print("Importing nation database...")
         exec_cmd(
             f'mariadb -e "source nation.sql" --user={self._db_user} --password={self._db_pass}'
         )
         exec_cmd("rm nation.zip")
 
@@ -143,10 +145,21 @@
     Args:
         ipython: (InteractiveShell) The currently active `InteractiveShell` instance.
 
     Returns:
         None
     """
     try:
-        ipython.register_magics(MariaDBInstaller(ipython))
-    except NameError:
+        mariadb_installer = MariaDBInstaller(ipython)
+        ipython.register_magics(mariadb_installer)
+        ipython.mariadb_installer = mariadb_installer
+    except (NameError, AttributeError):
+        print("IPython shell not available.")
+
+
+def unload_ipython_extension(ipython):
+    """Does some clean up"""
+
+    try:
+        del ipython.mariadb_installer
+    except (NameError, AttributeError):
         print("IPython shell not available.")
```

### Comparing `classroom_extensions-0.0.6/classroom_extensions/mongodb.py` & `classroom_extensions-0.0.7/classroom_extensions/mongodb.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.6/classroom_extensions/mongodb_install.py` & `classroom_extensions-0.0.7/classroom_extensions/mongodb_install.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
 An extension to install MongoDB and MongoDB Shell (mongosh).
 
 Note: This extension assumes that you are working in Google Colab
-running Ubuntu 20.04.
+running Ubuntu 22.04.
 """
 from os import path
 import os
 import glob
 import time
 from argparse import ArgumentParser
 from IPython.core.getipython import get_ipython
 from IPython.core.magic import magics_class, line_magic, Magics
 from .util import exec_cmd, get_os_release, is_colab
 
-_START_DB_TIMEOUT = 5  # Timeout for starting MariaDB
+__all__ = ["load_ipython_extension", "unload_ipython_extension", "MongoDBInstaller"]
+
+_START_DB_TIMEOUT = 5  # Timeout for starting MongoDB
 _SOFTWARE_DESC = {"mongo": "MongoDB"}
 
 _INSTALL_CMDS = {
     "mongo": [
         "apt update -y",
         "apt-get install gnupg curl",
         """curl -fsSL https://pgp.mongodb.com/server-6.0.asc | \
              gpg -o /usr/share/keyrings/mongodb-server-6.0.gpg \
              --dearmor""",
         "sudo apt-get install gnupg",
         "echo 'deb [ arch=amd64,arm64 signed-by=/usr/share/keyrings/mongodb-server-6.0.gpg ] "
         "https://repo.mongodb.org/apt/ubuntu jammy/mongodb-org/6.0 multiverse' "
         "| tee /etc/apt/sources.list.d/mongodb-org-6.0.list",
-        "sudo apt update",
+        "apt update -y",
         "apt-get install -y mongodb-org",
     ],
 }
 
 _SAMPLE_DBS_URL = "https://github.com/neelabalan/mongodb-sample-dataset.git"
 
 
@@ -152,10 +154,21 @@
     Args:
         ipython: (InteractiveShell) The currently active `InteractiveShell` instance.
 
     Returns:
         None
     """
     try:
-        ipython.register_magics(MongoDBInstaller(ipython))
-    except NameError:
+        mongodb_installer = MongoDBInstaller(ipython)
+        ipython.register_magics(mongodb_installer)
+        ipython.mongodb_installer = mongodb_installer
+    except (NameError, AttributeError):
+        print("IPython shell not available.")
+
+
+def unload_ipython_extension(ipython):
+    """Does some clean up"""
+
+    try:
+        del ipython.mongodb_installer
+    except (NameError, AttributeError):
         print("IPython shell not available.")
```

### Comparing `classroom_extensions-0.0.6/classroom_extensions/node.py` & `classroom_extensions-0.0.7/classroom_extensions/web.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,163 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 The code customizes IPython's %%javascript magic by introducing line arguments
 that allow for executing the JavaScript code on the server side (via Node.js).
 When executed on the browser, the magic creates a section in the code cell that
-mimics the browser's console
+mimics the browser's console. It also customizes `%%html` to enable the result
+section of the cell to mimic the browser's console.
 """
 
-from argparse import ArgumentParser
 from functools import partial
 from typing import Any, Callable, AnyStr
 from os import path, environ
 from asyncio import streams
 import asyncio
 import contextlib
 import io
 import uuid
 import shutil
+import sys
+import os
 import psutil
-from IPython.core.magic import magics_class, cell_magic
+from IPython.core.magic import magics_class, cell_magic, line_magic
 from IPython.core.magics.display import DisplayMagics
-from IPython.display import display, Javascript
-
+from IPython.display import display, Javascript, HTML
+from IPython.core import magic_arguments
+from IPython.utils.process import arg_split
+
+__all__ = [
+    "load_ipython_extension",
+    "unload_ipython_extension",
+    "WebMagics",
+    "JavascriptWithConsole",
+    "HTMLWithConsole",
+    "NodeProcessManager",
+]
 
 # timeout to wait for a node server process to start (in seconds)
 START_SERVER_TIMEOUT = 5
 
+# This code JavaScript will be included with the cell's code to
+# redirect the output of calls to console.[log, error, warn] to the
+# result section of the cell
+_CELL_CONSOLE = """
+function c_msg(type, o_func, ...args) {
+    let p = document.createElement("p");
+    p.classList.add(`console-${type}`);
+    p.textContent = args.join(" ");
+    document.getElementById('console-box').appendChild(p);
+    o_func(...args);
+}
+
+const o_log = console.log.bind(console)
+const o_error = console.error.bind(console);
+const o_warn = console.warn.bind(console);
+
+console.log = c_msg.bind(console, 'log', o_log);
+console.error = c_msg.bind(console, 'error', o_error);
+console.warn = c_msg.bind(console, 'warn', o_warn);
+
+window.addEventListener("error", (event) => {
+    console.error(`${event.type}: ${event.message}`);
+});
+
+var console_elems = {}
+console_elems.stl = document.createElement('style');
+console_elems.stl.textContent = `
+:root {
+    --font-log: Consolas, Monaco, 'Courier New', monospace;
+}
+
+.console-box {
+    max-width: 70vw;
+}
+
+.console-error, .console-log, .console-warn {
+    font-family: var(--font-log);
+    white-space: nowrap;
+    font-weight: 520;
+    font-size: 0.9rem;
+    line-height: 1.1rem;
+    padding: 2px 10px;
+    overflow-y: auto;
+    border-bottom: 1px solid #A9A9A9;
+    color: black;
+    margin: 0;
+}
+
+.console-error {
+    color: #8B0000;
+    border-bottom-color: #FFC0CB;
+    background-color: #FFE4E1;
+}
+
+.console-warn {
+    color: #A0522D;
+    border-bottom-color: #FFDEAD;
+    background-color: #FFFACD;
+}
+
+@media (max-width: 600px) {
+    .console-box {
+        max-width: 95vw;
+    }
+}
+
+@media (max-width: 992px) {
+    .console-box {
+        max-width: 90vw;
+    }
+}
+
+@media (min-width: 993px) {
+    .console-box {
+        max-width: 85vw;
+    }
+}
+
+@media (min-width: 1200px) {
+    .console-box {
+        max-width: 70vw;
+    }
+}
+`;
+document.head.appendChild(console_elems.stl);
+console_elems.c_box = document.createElement('div');
+console_elems.c_box.className = 'console-box';
+console_elems.c_box.id = 'console-box';
+document.getElementById('output-footer').appendChild(console_elems.c_box);
+"""
+
+_CONSOLE_TITLE = """
+var console_elems = {}
+console_elems.stl = document.createElement('style');
+console_elems.stl.textContent = `
+:root {
+    --font-title: 'Lato', 'Lucida Grande', 'Lucida Sans Unicode', Tahoma, Sans-Serif;
+}
+.console-title {
+    font-family: var(--font-title);
+    font-weight: 700;
+    color: black;
+    font-size: 1.1rem;
+    line-height: 1;
+    padding: 9px 10px;
+    white-space: nowrap;
+    margin: 0;
+}
+`;
+document.head.appendChild(console_elems.stl);
+console_elems.h_title = document.createElement('h2');
+console_elems.h_title.className = 'console-title';
+console_elems.h_title.textContent = 'Console:';
+document.getElementById('output-footer').appendChild(console_elems.h_title);
+"""
+
 
 class NodeProcessManager:
     """Used to manage the execution of Node processes"""
 
     _node_cmd: str = "/usr/bin/node"
 
     def __init__(self):
@@ -200,167 +328,154 @@
                 print(f"Error: process not found {process_error}")
         self._daemons.clear()
 
     def __del__(self):
         self.clean_up()
 
 
-# This code JavaScript will be included with the cell's code to
-# redirect the output of calls to console.[log, error, warn] to the
-# result section of the cell
-_CELL_CONSOLE = """
-function c_msg(type, o_func, ...args) {
-    let p = document.createElement("p");
-    p.classList.add(`console-${type}`);
-    p.textContent = args.join(" ");
-    document.getElementById('console-box').appendChild(p);
-    o_func(...args);
-}
-
-const o_log = console.log.bind(console)
-const o_error = console.error.bind(console);
-const o_warn = console.warn.bind(console);
-
-console.log = c_msg.bind(console, 'log', o_log);
-console.error = c_msg.bind(console, 'error', o_error);
-console.warn = c_msg.bind(console, 'warn', o_warn);
-
-window.addEventListener("error", (event) => {
-    console.error(`${event.type}: ${event.message}`);
-});
-
-var console_elems = {}
-console_elems.stl = document.createElement('style');
-console_elems.stl.textContent = `
-:root {
-    --font-log: Consolas, Monaco, 'Courier New', monospace;
-}
-
-.console-box {
-    max-width: 70vw;
-}
-
-.console-error, .console-log, .console-warn {
-    font-family: var(--font-log);
-    white-space: nowrap;
-    font-weight: 520;
-    font-size: 0.9rem;
-    line-height: 1.1rem;
-    padding: 2px 10px;
-    overflow-y: auto;
-    border-bottom: 1px solid #A9A9A9;
-    color: black;
-    margin: 0;
-}
-
-.console-error {
-    color: #8B0000;
-    border-bottom-color: #FFC0CB;
-    background-color: #FFE4E1;
-}
-
-.console-warn {
-    color: #A0522D;
-    border-bottom-color: #FFDEAD;
-    background-color: #FFFACD;
-}
-
-@media (max-width: 600px) {
-    .console-box {
-        max-width: 95vw;
-    }
-}
-
-@media (max-width: 992px) {
-    .console-box {
-        max-width: 90vw;
-    }
-}
-
-@media (min-width: 993px) {
-    .console-box {
-        max-width: 85vw;
-    }
-}
-
-@media (min-width: 1200px) {
-    .console-box {
-        max-width: 70vw;
-    }
-}
-`;
-document.head.appendChild(console_elems.stl);
-console_elems.c_box = document.createElement('div');
-console_elems.c_box.className = 'console-box';
-console_elems.c_box.id = 'console-box';
-document.getElementById('output-footer').appendChild(console_elems.c_box);
-"""
-
-
 class JavascriptWithConsole(Javascript):
     """
     This class extends JavaScript to intercept calls to console.log
     and make a result section of the cell.
     """
 
-    CELL_CONSOLE: str = _CELL_CONSOLE
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def _repr_javascript_(self):
         """Creates the full JavaScript code to be delivered to the browser"""
-        return self.CELL_CONSOLE + super()._repr_javascript_()
+        return _CELL_CONSOLE + super()._repr_javascript_()
 
 
-@magics_class
-class NodeMagics(DisplayMagics):
+class HTMLWithConsole(HTML):
     """
-    Implements the customizations to the %%javascript magic
-    that enables JavaScript execution by Node.js
+    This adds a copy of the browser's console with the messages
+    triggered when loading/executing the HTML/JavaScript code.
     """
 
-    _arg_parser: ArgumentParser
-    _proc_mgmt: NodeProcessManager
-    _in_notebook: bool
+    def __init__(self, data: AnyStr = None, console: bool = False):
+        """
+        Creates a new object representing the HTML code to be rendered.
 
-    def __init__(self, shell):
-        super().__init__(shell=shell)
-        self._arg_parser = self._create_parser()
-        self._proc_mgmt = NodeProcessManager()
-        self._in_notebook = shell.has_trait("kernel")
+        Args:
+            data: the HTML content
+            console: True if the browser console must be displayed
+        """
+        super().__init__(data=data)
+        self.console = console
 
-    @classmethod
-    def _create_parser(cls) -> ArgumentParser:
-        """Creates a parser to the line arguments"""
-        parser = ArgumentParser()
-        parser.add_argument(
+    def _repr_html_(self) -> str:
+        """
+        Creates the HTML content.
+
+        Returns:
+            The HTML code to be rendered.
+        """
+        html: str = ""
+        if self.console:
+            html += f"<script>{_CONSOLE_TITLE}{_CELL_CONSOLE}</script>"
+        return html + super()._repr_html_()
+
+
+def javascript_args(func):
+    """Single decorator for adding JavaScript args"""
+    args = [
+        magic_arguments.argument(
             "-t",
             "--target",
             type=str,
             choices=["browser", "node", "disk"],
             default="browser",
             help="the target for script execution",
-        )
-        parser.add_argument(
+        ),
+        magic_arguments.argument(
             "-f",
             "--filename",
             type=str,
             help="filename when cell contents are saved to disk",
-        )
-        parser.add_argument(
+        ),
+        magic_arguments.argument(
             "-p",
             "--port",
             type=int,
             help="a port number if the cell starts a Node server process",
+        ),
+    ]
+    for arg in args:
+        func = arg(func)
+    return func
+
+
+def html_args(func):
+    """Single decorator for adding HTML args"""
+    args = [
+        magic_arguments.argument(
+            "-c",
+            "--console",
+            action="store_true",
+            help="Whether to display a copy of the browser's console or not",
         )
-        return parser
+    ]
+    for arg in args:
+        func = arg(func)
+    return func
+
+
+def http_server_args(func):
+    """Single decorator for adding HTTP server args"""
+    args = [
+        magic_arguments.argument(
+            "--action",
+            "-a",
+            default="start",
+            choices=["start", "stop"],
+            help="action to execute (default: start)",
+        ),
+        magic_arguments.argument(
+            "--bind",
+            "-b",
+            default="0.0.0.0",
+            help="specify alternate bind address (default: all interfaces)",
+        ),
+        magic_arguments.argument(
+            "--directory",
+            "-d",
+            default=os.getcwd(),
+            help="specify alternate directory (default: current directory)",
+        ),
+        magic_arguments.argument(
+            "--port",
+            "-p",
+            default=8000,
+            type=int,
+            help="specify alternate port (default: 8000)",
+        ),
+    ]
+    for arg in args:
+        func = arg(func)
+    return func
 
-    @classmethod
-    def _save_script(cls, filename: str, cell_content: str) -> str:
+
+@magics_class
+class WebMagics(DisplayMagics):
+    """
+    Implements the customizations to the %%javascript magic
+    that enables JavaScript execution by Node.js
+    """
+
+    _proc_mgmt: NodeProcessManager
+    _in_notebook: bool
+
+    def __init__(self, shell):
+        super().__init__(shell=shell)
+        self._proc_mgmt = NodeProcessManager()
+        self._in_notebook = shell.has_trait("kernel")
+
+    @staticmethod
+    def _save_script(filename: str, cell_content: str) -> str:
         """
         Creates the JavaScript file for Node to run
 
         Args:
             filename: the file name
             cell_content: the cell contents to save into the file
 
@@ -386,57 +501,98 @@
         """
         if self._in_notebook:
             loop = asyncio.get_event_loop()
             loop.create_task(self._proc_mgmt.execute(js_file, port))
         else:
             asyncio.run(self._proc_mgmt.execute(js_file, port))
 
+    @magic_arguments.magic_arguments()
+    @javascript_args
     @cell_magic
     def javascript(self, line: str = None, cell: str = None) -> None:
         """
         Method called when executing %%javascript
         Args:
             line: line arguments (e.g. --target, --filename)
             cell: the JavaScript code to execute
 
         Returns:
             None
         """
-        args = self._arg_parser.parse_args(line.split() if line else "")
+        argv = arg_split(line, posix=not sys.platform.startswith("win"))
+        args = self.javascript.parser.parse_args(argv)
 
         if args.target == "node":
             if not args.filename:
                 raise ValueError("--filename is required when using --target=node")
             js_file = self._save_script(args.filename, cell)
             self._run_on_node(js_file, args.port)
         elif args.target == "browser":
             display(JavascriptWithConsole(cell))
         elif args.target == "disk":
             if not args.filename:
                 raise ValueError("--filename is required when using --target=disk")
             self._save_script(args.filename, cell)
 
+    @magic_arguments.magic_arguments()
+    @html_args
+    @cell_magic
+    def html(self, line=None, cell=None) -> None:
+        argv = arg_split(line, posix=not sys.platform.startswith("win"))
+        args = self.html.parser.parse_args(argv)
+        html = HTMLWithConsole(cell, args.console)
+        display(html)
+
+    @magic_arguments.magic_arguments()
+    @http_server_args
+    @line_magic
+    def http_server(self, line=None) -> None:
+        """Line magic to start/stop a python Web server"""
+        argv = arg_split(line, posix=not sys.platform.startswith("win"))
+        args = self.http_server.parser.parse_args(argv)
+
+        def start_web_server(address, directory, port):
+            stop_web_server(port)  # Stop any server that is currently running
+            print(f"Starting server listening on port {port}...")
+            self.shell.system_raw(
+                f"python -m http.server {port} --bind {address} --directory {directory} &"
+            )
+
+        def stop_web_server(port):
+            print(f"Stopping any server listening on port {port}...")
+            stop_cmd = (
+                r"ps -x | grep -e '[h]ttp.server\s*"
+                + str(port)
+                + "' | awk '{print $1}' | xargs -I {} kill {}"
+            )
+            self.shell.system_raw(stop_cmd)
+
+        if args.action == "start":
+            start_web_server(args.bind, args.directory, args.port)
+        else:
+            stop_web_server(args.port)
+
 
 def load_ipython_extension(ipython):
     """
     Loads the ipython extension
 
     Args:
         ipython: (InteractiveShell) The currently active `InteractiveShell` instance.
 
     Returns:
         None
     """
     try:
-        node_magics = NodeMagics(ipython)
-        ipython.register_magics(node_magics)
-        ipython.node_magics = node_magics
+        web_magics = WebMagics(ipython)
+        ipython.register_magics(web_magics)
+        ipython.node_magics = web_magics
     except (NameError, AttributeError):
         print("IPython shell not available.")
 
 
 def unload_ipython_extension(ipython):
     """Unloads the extension"""
     try:
-        del ipython.node_magics
+        del ipython.web_magics
     except (NameError, AttributeError):
         print("IPython shell not available.")
```

### Comparing `classroom_extensions-0.0.6/classroom_extensions/plantuml.py` & `classroom_extensions-0.0.7/classroom_extensions/plantuml.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.6/classroom_extensions/util.py` & `classroom_extensions-0.0.7/classroom_extensions/util.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.6/classroom_extensions.egg-info/PKG-INFO` & `classroom_extensions-0.0.7/classroom_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classroom-extensions
-Version: 0.0.6
+Version: 0.0.7
 Summary: IPython extensions used for teaching
 Author-email: Marcos Dias de Assuncao <assuncao@acm.org>
 Maintainer-email: Marcos Dias de Assuncao <assuncao@acm.org>
 License: MIT
 Project-URL: Homepage, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Bug Reports, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Say Thanks!, https://saythanks.io/to/assuncaomarcos
@@ -79,27 +79,27 @@
 To ease the creation of notebooks on Google Colab, a second extension (`mariadb_install`)
 installs MariaDB and the required libraries to run the first extension without
 worrying about setting things up.
 
 Server-Side JavaScript
 ----------------------
 
-This extension, called `node`, customizes the `%%javascript` cell magic to enable
+This extension, called `web`, customizes the `%%javascript` cell magic to enable
 executing JavaScript code on the server or container hosting the Jupyter Notebook or
 on Google Colab. Node.js executes the code provided in a cell whose `--target` argument
-receives the value `node`. It also enables starting long-running Node.js server
+receives the value `web`. It also enables starting long-running Node.js server
 processes that will listen on given ports without blocking the code cell of
 the notebook. In addition to executing JavaScript code on the server side, when run
 on the browser, the magic enables printing the output of the browser's console in
 the result section of the code cell.
 
 Custom HTML Magic
 -----------------
 
-The `html` extension customizes the `%%html` magic. After rendering the HTML code
+The `web` extension also customizes the `%%html` magic. After rendering the HTML code
 inserted in the cell, the extension displays a high-level copy of the browser's
 console. This behavior helps in teaching HTML or JavaScript that writes on the console.
 
 PlantUML Magics
 ---------------
 
 PlantUML is a textual Domain-Specific Language (DSL) used for creating diagrams,
```

### Comparing `classroom_extensions-0.0.6/classroom_extensions.egg-info/SOURCES.txt` & `classroom_extensions-0.0.7/classroom_extensions.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 LICENSE
 README.rst
 pyproject.toml
 classroom_extensions/__init__.py
-classroom_extensions/html.py
 classroom_extensions/mariadb.py
 classroom_extensions/mariadb_install.py
 classroom_extensions/mongodb.py
 classroom_extensions/mongodb_install.py
-classroom_extensions/node.py
 classroom_extensions/plantuml.py
 classroom_extensions/util.py
+classroom_extensions/web.py
 classroom_extensions.egg-info/PKG-INFO
 classroom_extensions.egg-info/SOURCES.txt
 classroom_extensions.egg-info/dependency_links.txt
 classroom_extensions.egg-info/requires.txt
 classroom_extensions.egg-info/top_level.txt
-tests/test_html.py
 tests/test_mariadb.py
 tests/test_mongodb.py
-tests/test_nodejs.py
-tests/test_plantuml.py
+tests/test_plantuml.py
+tests/test_web.py
```

### Comparing `classroom_extensions-0.0.6/pyproject.toml` & `classroom_extensions-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.6/tests/test_mariadb.py` & `classroom_extensions-0.0.7/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.6/tests/test_mongodb.py` & `classroom_extensions-0.0.7/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.6/tests/test_nodejs.py` & `classroom_extensions-0.0.7/tests/test_web.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,48 +2,48 @@
 # -*- coding: utf-8 -*-
 """ Tests the JavaScript magics """
 
 import unittest
 import asyncio
 from os import path
 from IPython.utils import io
-from classroom_extensions.node import NodeProcessManager
-from classroom_extensions.node import JavascriptWithConsole
-import classroom_extensions.node as node_ext
+from classroom_extensions.web import NodeProcessManager
+from classroom_extensions.web import JavascriptWithConsole, HTMLWithConsole
+import classroom_extensions.web as node_ext
 from .base import BaseTestCase
 
 
 class TestNodeJs(BaseTestCase):
     """Testcase for the NodeJs extension"""
 
     def setUp(self) -> None:
         # Loads the extension
-        self.ipython.extension_manager.load_extension("classroom_extensions.node")
+        self.ipython.extension_manager.load_extension("classroom_extensions.web")
 
     def tearDown(self) -> None:
-        self.ipython.extension_manager.unload_extension("classroom_extensions.node")
+        self.ipython.extension_manager.unload_extension("classroom_extensions.web")
 
     def test_process_manager(self):
         """Tests the process manager"""
         print("Test process manager.")
         proc_manager = NodeProcessManager()
         where_ls = ""
 
         def stdout_callback(data):
             nonlocal where_ls
             where_ls += data
 
         async def run_cmd():
             async with proc_manager.open_process(
-                "which", "uname", stdout_callback=stdout_callback
-            ):
+                "ls", "/usr/bin/pwd", stdout_callback=stdout_callback
+            ) :
                 pass
 
         asyncio.run(run_cmd())
-        self.assertRegex(text=where_ls, expected_regex=r"uname")
+        self.assertRegex(text=where_ls, expected_regex=r"pwd")
 
     def test_node_script(self):
         """Tests executing server-side JavaScript"""
         print("Test executing Node.js script.")
         cell_output: str
         console_content = "------"
         with io.capture_output() as captured:
@@ -110,18 +110,48 @@
             "text/plain": f"<{JavascriptWithConsole.__module__}."
             f"{JavascriptWithConsole.__qualname__} object>"
         }
         cell_content = "console.log('----');"
         self.ipython.run_cell_magic("javascript", line="", cell=f"{cell_content}")
         self.assertEqual(expected_dir, self.publisher.display_output.pop())
 
+    def test_html_javascript(self):
+        """Test HTML with JavaScript"""
+        print("Testing HTML with JavaScript")
+        expected_dir = {
+            "text/plain": f"<{HTMLWithConsole.__module__}."
+            f"{HTMLWithConsole.__qualname__} object>"
+        }
+        cell_content = "console.log('----');"
+        self.ipython.run_cell_magic("html", line="--console", cell=f"{cell_content}")
+        self.assertEqual(expected_dir, self.publisher.display_output.pop())
+
+    def test_html_console(self):
+        """Tests the HTML with console."""
+
+        html_code = """
+            <div class="container">
+            <h1>An H1 Title</h1>
+            <h2>An H2 Title</h2>
+            <p>A paragraph with some text.</p>
+            </div>
+        """
+
+        html = HTMLWithConsole(data=html_code, console=True)
+        self.assertRegex(html._repr_html_(), "console_elems")
+
     def test_incorrect_loading(self):
         """Tests incorrectly loading the extension."""
         expected = "IPython shell not available.\n"
         output = self.capture_output(node_ext.load_ipython_extension, None)
         self.assertEqual(output, expected)
         output = self.capture_output(node_ext.unload_ipython_extension, None)
         self.assertEqual(output, expected)
 
+    def test_http_server(self):
+        """ Tests start/stop of HTTP server """
+        self.ipython.run_line_magic("http_server", line="--action=start --bind=0.0.0.0 --port=8000 --directory=/tmp")
+        self.ipython.run_line_magic("http_server", line="--action=stop --port=8000")
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `classroom_extensions-0.0.6/tests/test_plantuml.py` & `classroom_extensions-0.0.7/tests/test_plantuml.py`

 * *Files identical despite different names*

