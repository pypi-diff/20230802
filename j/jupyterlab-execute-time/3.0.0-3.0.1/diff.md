# Comparing `tmp/jupyterlab_execute_time-3.0.0.tar.gz` & `tmp/jupyterlab_execute_time-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jupyterlab_execute_time-3.0.0.tar", last modified: Fri May 19 13:37:35 2023, max compression
+gzip compressed data, was "dist/jupyterlab_execute_time-3.0.1.tar", last modified: Wed Aug  2 18:15:57 2023, max compression
```

## Comparing `jupyterlab_execute_time-3.0.0.tar` & `jupyterlab_execute_time-3.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:37:35.028197 jupyterlab_execute_time-3.0.0/
--rw-r--r--   0 udoff      (501) staff       (20)     1504 2020-04-07 22:34:31.000000 jupyterlab_execute_time-3.0.0/LICENSE.txt
--rw-r--r--   0 udoff      (501) staff       (20)      466 2021-07-12 22:30:45.000000 jupyterlab_execute_time-3.0.0/MANIFEST.in
--rw-r--r--   0 udoff      (501) staff       (20)     5972 2023-05-19 13:37:35.027939 jupyterlab_execute_time-3.0.0/PKG-INFO
--rw-r--r--   0 udoff      (501) staff       (20)     4914 2022-11-03 22:49:14.000000 jupyterlab_execute_time-3.0.0/README.md
--rw-r--r--   0 udoff      (501) staff       (20)      207 2021-01-19 21:27:57.000000 jupyterlab_execute_time-3.0.0/install.json
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:37:34.971842 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/
--rw-r--r--   0 udoff      (501) staff       (20)      326 2021-01-19 21:27:57.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/__init__.py
--rw-r--r--   0 udoff      (501) staff       (20)      459 2021-01-19 21:27:57.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/_version.py
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:37:34.978344 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/
--rw-r--r--   0 udoff      (501) staff       (20)    20845 2023-05-19 13:37:29.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/build_log.json
--rw-r--r--   0 udoff      (501) staff       (20)     3302 2023-05-19 13:37:32.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/package.json
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:37:34.965808 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/schemas/
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:37:34.980699 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/schemas/jupyterlab-execute-time/
--rw-r--r--   0 udoff      (501) staff       (20)     3160 2023-05-19 13:37:29.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/schemas/jupyterlab-execute-time/package.json.orig
--rw-r--r--   0 udoff      (501) staff       (20)     1605 2023-05-19 13:37:29.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/schemas/jupyterlab-execute-time/settings.json
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:37:35.019828 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/
--rw-r--r--   0 udoff      (501) staff       (20)    19356 2023-05-19 13:37:32.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/lib_index_js.d710423855898245e472.js
--rw-r--r--   0 udoff      (501) staff       (20)    21570 2023-05-19 13:37:32.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/lib_index_js.d710423855898245e472.js.map
--rw-r--r--   0 udoff      (501) staff       (20)    28731 2023-05-19 13:37:32.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/remoteEntry.45aa7d5d0f82a73e893e.js
--rw-r--r--   0 udoff      (501) staff       (20)    27637 2023-05-19 13:37:32.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/remoteEntry.45aa7d5d0f82a73e893e.js.map
--rw-r--r--   0 udoff      (501) staff       (20)      166 2023-05-19 13:37:29.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/style.js
--rw-r--r--   0 udoff      (501) staff       (20)    22036 2023-05-19 13:37:32.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/style_index_js.3522f9e4692f1951c092.js
--rw-r--r--   0 udoff      (501) staff       (20)    18386 2023-05-19 13:37:32.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/style_index_js.3522f9e4692f1951c092.js.map
--rw-r--r--   0 udoff      (501) staff       (20)  1108307 2023-05-19 13:37:32.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/vendors-node_modules_date-fns_esm_index_js.bb5155b17a678353747a.js
--rw-r--r--   0 udoff      (501) staff       (20)   874905 2023-05-19 13:37:32.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/vendors-node_modules_date-fns_esm_index_js.bb5155b17a678353747a.js.map
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:37:34.977748 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time.egg-info/
--rw-r--r--   0 udoff      (501) staff       (20)     5972 2023-05-19 13:37:34.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time.egg-info/PKG-INFO
--rw-r--r--   0 udoff      (501) staff       (20)     1624 2023-05-19 13:37:34.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time.egg-info/SOURCES.txt
--rw-r--r--   0 udoff      (501) staff       (20)        1 2023-05-19 13:37:34.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time.egg-info/dependency_links.txt
--rw-r--r--   0 udoff      (501) staff       (20)        1 2023-03-23 18:34:40.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time.egg-info/not-zip-safe
--rw-r--r--   0 udoff      (501) staff       (20)       25 2023-05-19 13:37:34.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time.egg-info/requires.txt
--rw-r--r--   0 udoff      (501) staff       (20)       24 2023-05-19 13:37:34.000000 jupyterlab_execute_time-3.0.0/jupyterlab_execute_time.egg-info/top_level.txt
--rw-r--r--   0 udoff      (501) staff       (20)     3160 2023-05-19 13:28:42.000000 jupyterlab_execute_time-3.0.0/package.json
--rw-r--r--   0 udoff      (501) staff       (20)      277 2023-05-19 13:34:08.000000 jupyterlab_execute_time-3.0.0/pyproject.toml
--rw-r--r--   0 udoff      (501) staff       (20)       38 2023-05-19 13:37:35.028439 jupyterlab_execute_time-3.0.0/setup.cfg
--rw-r--r--   0 udoff      (501) staff       (20)     2478 2023-05-19 13:20:29.000000 jupyterlab_execute_time-3.0.0/setup.py
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:37:35.026425 jupyterlab_execute_time-3.0.0/src/
--rw-r--r--   0 udoff      (501) staff       (20)    14088 2023-05-19 13:29:37.000000 jupyterlab_execute_time-3.0.0/src/ExecuteTimeWidget.ts
--rw-r--r--   0 udoff      (501) staff       (20)     1298 2021-01-19 21:27:57.000000 jupyterlab_execute_time-3.0.0/src/formatters.ts
--rw-r--r--   0 udoff      (501) staff       (20)     1581 2022-11-07 22:15:05.000000 jupyterlab_execute_time-3.0.0/src/index.ts
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-05-19 13:37:35.027553 jupyterlab_execute_time-3.0.0/style/
--rw-r--r--   0 udoff      (501) staff       (20)     1223 2022-11-07 22:44:08.000000 jupyterlab_execute_time-3.0.0/style/base.css
--rw-r--r--   0 udoff      (501) staff       (20)       25 2021-01-19 21:27:57.000000 jupyterlab_execute_time-3.0.0/style/index.css
--rw-r--r--   0 udoff      (501) staff       (20)       21 2021-01-19 21:27:57.000000 jupyterlab_execute_time-3.0.0/style/index.js
--rw-r--r--   0 udoff      (501) staff       (20)      557 2023-05-19 13:20:29.000000 jupyterlab_execute_time-3.0.0/tsconfig.json
--rw-r--r--   0 udoff      (501) staff       (20)     3177 2020-04-07 22:34:31.000000 jupyterlab_execute_time-3.0.0/tslint.json
--rw-r--r--   0 udoff      (501) staff       (20)   239705 2023-05-19 13:23:22.000000 jupyterlab_execute_time-3.0.0/yarn.lock
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-08-02 18:15:57.779902 jupyterlab_execute_time-3.0.1/
+-rw-r--r--   0 udoff      (501) staff       (20)     1504 2020-04-07 22:34:31.000000 jupyterlab_execute_time-3.0.1/LICENSE.txt
+-rw-r--r--   0 udoff      (501) staff       (20)      466 2021-07-12 22:30:45.000000 jupyterlab_execute_time-3.0.1/MANIFEST.in
+-rw-r--r--   0 udoff      (501) staff       (20)     5972 2023-08-02 18:15:57.779699 jupyterlab_execute_time-3.0.1/PKG-INFO
+-rw-r--r--   0 udoff      (501) staff       (20)     4914 2022-11-03 22:49:14.000000 jupyterlab_execute_time-3.0.1/README.md
+-rw-r--r--   0 udoff      (501) staff       (20)      207 2021-01-19 21:27:57.000000 jupyterlab_execute_time-3.0.1/install.json
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-08-02 18:15:57.741876 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/
+-rw-r--r--   0 udoff      (501) staff       (20)      326 2021-01-19 21:27:57.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/__init__.py
+-rw-r--r--   0 udoff      (501) staff       (20)      459 2021-01-19 21:27:57.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/_version.py
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-08-02 18:15:57.749719 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/
+-rw-r--r--   0 udoff      (501) staff       (20)    20710 2023-08-02 18:14:51.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/build_log.json
+-rw-r--r--   0 udoff      (501) staff       (20)     3434 2023-08-02 18:14:54.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/package.json
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-08-02 18:15:57.732678 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/schemas/
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-08-02 18:15:57.751052 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/schemas/jupyterlab-execute-time/
+-rw-r--r--   0 udoff      (501) staff       (20)     3292 2023-08-02 18:14:51.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/schemas/jupyterlab-execute-time/package.json.orig
+-rw-r--r--   0 udoff      (501) staff       (20)     1605 2023-08-02 18:14:51.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/schemas/jupyterlab-execute-time/settings.json
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-08-02 18:15:57.772744 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/
+-rw-r--r--   0 udoff      (501) staff       (20)    19356 2023-08-02 18:14:54.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/lib_index_js.d710423855898245e472.js
+-rw-r--r--   0 udoff      (501) staff       (20)    21570 2023-08-02 18:14:54.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/lib_index_js.d710423855898245e472.js.map
+-rw-r--r--   0 udoff      (501) staff       (20)    28731 2023-08-02 18:14:54.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/remoteEntry.c3b0015b00abd9869851.js
+-rw-r--r--   0 udoff      (501) staff       (20)    27637 2023-08-02 18:14:54.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/remoteEntry.c3b0015b00abd9869851.js.map
+-rw-r--r--   0 udoff      (501) staff       (20)      166 2023-08-02 18:14:51.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/style.js
+-rw-r--r--   0 udoff      (501) staff       (20)    22036 2023-08-02 18:14:54.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/style_index_js.3522f9e4692f1951c092.js
+-rw-r--r--   0 udoff      (501) staff       (20)    18386 2023-08-02 18:14:54.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/style_index_js.3522f9e4692f1951c092.js.map
+-rw-r--r--   0 udoff      (501) staff       (20)  1108307 2023-08-02 18:14:54.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/vendors-node_modules_date-fns_esm_index_js.bb5155b17a678353747a.js
+-rw-r--r--   0 udoff      (501) staff       (20)   874905 2023-08-02 18:14:54.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/vendors-node_modules_date-fns_esm_index_js.bb5155b17a678353747a.js.map
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-08-02 18:15:57.748951 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time.egg-info/
+-rw-r--r--   0 udoff      (501) staff       (20)     5972 2023-08-02 18:15:57.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time.egg-info/PKG-INFO
+-rw-r--r--   0 udoff      (501) staff       (20)     1624 2023-08-02 18:15:57.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time.egg-info/SOURCES.txt
+-rw-r--r--   0 udoff      (501) staff       (20)        1 2023-08-02 18:15:57.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time.egg-info/dependency_links.txt
+-rw-r--r--   0 udoff      (501) staff       (20)        1 2023-03-23 18:34:40.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time.egg-info/not-zip-safe
+-rw-r--r--   0 udoff      (501) staff       (20)       17 2023-08-02 18:15:57.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time.egg-info/requires.txt
+-rw-r--r--   0 udoff      (501) staff       (20)       24 2023-08-02 18:15:57.000000 jupyterlab_execute_time-3.0.1/jupyterlab_execute_time.egg-info/top_level.txt
+-rw-r--r--   0 udoff      (501) staff       (20)     3292 2023-08-02 18:11:35.000000 jupyterlab_execute_time-3.0.1/package.json
+-rw-r--r--   0 udoff      (501) staff       (20)      513 2023-08-02 18:11:35.000000 jupyterlab_execute_time-3.0.1/pyproject.toml
+-rw-r--r--   0 udoff      (501) staff       (20)       38 2023-08-02 18:15:57.779967 jupyterlab_execute_time-3.0.1/setup.cfg
+-rw-r--r--   0 udoff      (501) staff       (20)     2816 2023-08-02 18:11:35.000000 jupyterlab_execute_time-3.0.1/setup.py
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-08-02 18:15:57.777468 jupyterlab_execute_time-3.0.1/src/
+-rw-r--r--   0 udoff      (501) staff       (20)    14088 2023-05-19 13:29:37.000000 jupyterlab_execute_time-3.0.1/src/ExecuteTimeWidget.ts
+-rw-r--r--   0 udoff      (501) staff       (20)     1298 2021-01-19 21:27:57.000000 jupyterlab_execute_time-3.0.1/src/formatters.ts
+-rw-r--r--   0 udoff      (501) staff       (20)     1581 2023-08-02 18:07:00.000000 jupyterlab_execute_time-3.0.1/src/index.ts
+drwxr-xr-x   0 udoff      (501) staff       (20)        0 2023-08-02 18:15:57.779397 jupyterlab_execute_time-3.0.1/style/
+-rw-r--r--   0 udoff      (501) staff       (20)     1223 2022-11-07 22:44:08.000000 jupyterlab_execute_time-3.0.1/style/base.css
+-rw-r--r--   0 udoff      (501) staff       (20)       25 2021-01-19 21:27:57.000000 jupyterlab_execute_time-3.0.1/style/index.css
+-rw-r--r--   0 udoff      (501) staff       (20)       21 2021-01-19 21:27:57.000000 jupyterlab_execute_time-3.0.1/style/index.js
+-rw-r--r--   0 udoff      (501) staff       (20)      557 2023-05-19 13:20:29.000000 jupyterlab_execute_time-3.0.1/tsconfig.json
+-rw-r--r--   0 udoff      (501) staff       (20)     3177 2020-04-07 22:34:31.000000 jupyterlab_execute_time-3.0.1/tslint.json
+-rw-r--r--   0 udoff      (501) staff       (20)   243533 2023-08-02 18:11:35.000000 jupyterlab_execute_time-3.0.1/yarn.lock
```

### Comparing `jupyterlab_execute_time-3.0.0/LICENSE.txt` & `jupyterlab_execute_time-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/PKG-INFO` & `jupyterlab_execute_time-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_execute_time
-Version: 3.0.0
+Version: 3.0.1
 Summary: Display cell timings in Jupyter Lab
 Home-page: https://github.com/deshaw/jupyterlab-execute-time
 Author: Marc Udoff
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jupyterlab_execute_time-3.0.0/README.md` & `jupyterlab_execute_time-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/build_log.json` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/build_log.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999914011822557%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@jupyterlab/application': {'requiredVersion': "*

 * *      "'^4.0.3'}, '@jupyterlab/application-extension': {'requiredVersion': '^4.0.3'}, "*

 * *      "'@jupyterlab/apputils-extension': {'requiredVersion': '^4.0.3'}, "*

 * *      "'@jupyterlab/cell-toolbar-extension': {'requiredVersion': '^4.0.3'}, "*

 * *      "'@jupyterlab/celltags-extension': {'requiredVersion': '^4.0.3'}, "*

 * *      "'@jupyterlab/codemirror-extension': {'requiredVersion': '^4.0.3'}, "*

 * *      "'@jupyterlab/compl […]*

```diff
@@ -136,415 +136,411 @@
                         "@jupyter/ydoc": {
                             "import": false,
                             "requiredVersion": "^1.0.2",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.1.3",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
-                        },
-                        "@jupyterlab/celltags": {
-                            "import": false,
-                            "requiredVersion": "^4.0.0-alpha.20"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^6.0.0",
+                            "requiredVersion": "^6.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/lsp": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/lsp-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/markedparser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/mathjax-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/metadataform": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/metadataform-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^5.0.0"
+                            "requiredVersion": "^5.0.3"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.8.0",
+                            "requiredVersion": "^3.8.3",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^7.0.0",
+                            "requiredVersion": "^7.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^6.0.0",
+                            "requiredVersion": "^6.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^6.0.0"
+                            "requiredVersion": "^6.0.3"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^4.0.0",
+                            "requiredVersion": "^4.0.3",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0"
+                            "requiredVersion": "^4.0.3"
                         },
                         "@lezer/common": {
                             "import": false,
                             "requiredVersion": "^1.0.0",
                             "singleton": true
                         },
                         "@lezer/highlight": {
@@ -627,15 +623,15 @@
                             "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "date-fns": {},
                         "jupyterlab-execute-time": {
                             "import": "/Users/udoff/WebstormProjects/jupyterlab-execute-time/lib/index.js",
                             "singleton": true,
-                            "version": "3.0.0"
+                            "version": "3.0.1"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/package.json` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/schemas/jupyterlab-execute-time/package.json.orig`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9559566250742721%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/observables': '^4.0.0'}",*

 * * "'devDependencies'": "{'@types/json-schema': '^7.0.11', '@types/react': '^18.0.26', 'yjs': "*

 * *                      "'^13.5.0'}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'3.0.1'"}*

```diff
@@ -3,24 +3,27 @@
         "url": "https://github.com/deshaw/jupyterlab-execute-time/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/cells": "^4.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/observables": "^4.0.0",
         "@jupyterlab/settingregistry": "^4.0.0",
         "@lumino/coreutils": "^2.0.0-rc.1",
         "@lumino/widgets": "^2.0.0-rc.1",
         "date-fns": "^2.29.3"
     },
     "description": "Display cell timings in Jupyter Lab",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@types/chai": "^4.3.4",
+        "@types/json-schema": "^7.0.11",
         "@types/mocha": "^10.0.1",
+        "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "~5.55.0",
         "@typescript-eslint/parser": "~5.55.0",
         "chai": "^4.3.7",
         "eslint": "~8.36.0",
         "eslint-config-prettier": "~8.7.0",
         "eslint-plugin-prettier": "~4.2.1",
         "husky": "^8.0.3",
@@ -28,29 +31,25 @@
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.4",
         "rimraf": "^4.4.0",
         "ts-mocha": "^10.0.0",
         "tslint": "^6.1.3",
         "tslint-config-prettier": "^1.18.0",
         "tslint-plugin-prettier": "^2.3.0",
-        "typescript": "~5.0.2"
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.0"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/deshaw/jupyterlab-execute-time",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.45aa7d5d0f82a73e893e.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "jupyterlab_execute_time/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -88,9 +87,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "3.0.0"
+    "version": "3.0.1"
 }
```

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/schemas/jupyterlab-execute-time/package.json.orig` & `jupyterlab_execute_time-3.0.1/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9633095662507427%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/observables': '^4.0.0'}",*

 * * "'devDependencies'": "{'@types/json-schema': '^7.0.11', '@types/react': '^18.0.26', 'yjs': "*

 * *                      "'^13.5.0'}",*

 * * "'version'": "'3.0.1'"}*

```diff
@@ -3,24 +3,27 @@
         "url": "https://github.com/deshaw/jupyterlab-execute-time/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/cells": "^4.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/observables": "^4.0.0",
         "@jupyterlab/settingregistry": "^4.0.0",
         "@lumino/coreutils": "^2.0.0-rc.1",
         "@lumino/widgets": "^2.0.0-rc.1",
         "date-fns": "^2.29.3"
     },
     "description": "Display cell timings in Jupyter Lab",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@types/chai": "^4.3.4",
+        "@types/json-schema": "^7.0.11",
         "@types/mocha": "^10.0.1",
+        "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "~5.55.0",
         "@typescript-eslint/parser": "~5.55.0",
         "chai": "^4.3.7",
         "eslint": "~8.36.0",
         "eslint-config-prettier": "~8.7.0",
         "eslint-plugin-prettier": "~4.2.1",
         "husky": "^8.0.3",
@@ -28,15 +31,16 @@
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.4",
         "rimraf": "^4.4.0",
         "ts-mocha": "^10.0.0",
         "tslint": "^6.1.3",
         "tslint-config-prettier": "^1.18.0",
         "tslint-plugin-prettier": "^2.3.0",
-        "typescript": "~5.0.2"
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.0"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json",
         "style/index.js"
     ],
@@ -83,9 +87,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "3.0.0"
+    "version": "3.0.1"
 }
```

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/schemas/jupyterlab-execute-time/settings.json` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/schemas/jupyterlab-execute-time/settings.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/lib_index_js.d710423855898245e472.js` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/lib_index_js.d710423855898245e472.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/lib_index_js.d710423855898245e472.js.map` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/lib_index_js.d710423855898245e472.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/remoteEntry.45aa7d5d0f82a73e893e.js` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/remoteEntry.c3b0015b00abd9869851.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -425,15 +425,15 @@
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
                     register("date-fns", "2.29.3", () => (__webpack_require__.e("vendors-node_modules_date-fns_esm_index_js").then(() => (() => (__webpack_require__( /*! ./node_modules/date-fns/esm/index.js */ "./node_modules/date-fns/esm/index.js"))))));
                     /******/
-                    register("jupyterlab-execute-time", "3.0.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab-execute-time", "3.0.1", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -814,17 +814,17 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 4, 0, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 4, 0, 3])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 4, 0, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 4, 0, 3])),
             /******/
             "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 2, 0, 1])),
             /******/
             "webpack/sharing/consume/default/@lumino/coreutils": () => (loadSingletonVersionCheck("default", "@lumino/coreutils", [1, 2, 0, 0])),
             /******/
             "webpack/sharing/consume/default/date-fns/date-fns": () => (loadStrictVersionCheckFallback("default", "date-fns", [1, 2, 29, 3], () => (__webpack_require__.e("vendors-node_modules_date-fns_esm_index_js").then(() => (() => (__webpack_require__( /*! date-fns */ "./node_modules/date-fns/esm/index.js")))))))
             /******/
@@ -1074,8 +1074,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab-execute-time");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyterlab-execute-time"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.45aa7d5d0f82a73e893e.js.map
+//# sourceMappingURL=remoteEntry.c3b0015b00abd9869851.js.map
```

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/remoteEntry.45aa7d5d0f82a73e893e.js.map` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/remoteEntry.c3b0015b00abd9869851.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9142857142857144%*

 * *Differences: {"'file'": "'remoteEntry.c3b0015b00abd9869851.js'",*

 * * "'sourcesContent'": "{insert: [(10, '__webpack_require__.S = {};\\nvar initPromises = {};\\nvar "*

 * *                     'initTokens = {};\\n__webpack_require__.I = (name, initScope) => '*

 * *                     '{\\n\\tif(!initScope) initScope = [];\\n\\t// handling circular init '*

 * *                     'calls\\n\\tvar initToken = initTokens[name];\\n\\tif(!initToken) initToken = '*

 * *                     'initTokens[name] = {};\\n\\tif(initScope.indexOf(initToke […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.45aa7d5d0f82a73e893e.js",
+    "file": "remoteEntry.c3b0015b00abd9869851.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,kJAAkJ;WAChL;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC5CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC/KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-execute-time/webpack/container-entry",
         "webpack://jupyterlab-execute-time/webpack/bootstrap",
         "webpack://jupyterlab-execute-time/webpack/runtime/compat get default export",
@@ -30,17 +30,17 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"d710423855898245e472\",\"style_index_js\":\"3522f9e4692f1951c092\",\"vendors-node_modules_date-fns_esm_index_js\":\"bb5155b17a678353747a\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-execute-time:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab-execute-time\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"date-fns\", \"2.29.3\", () => (__webpack_require__.e(\"vendors-node_modules_date-fns_esm_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/date-fns/esm/index.js */ \"./node_modules/date-fns/esm/index.js\"))))));\n\t\t\tregister(\"jupyterlab-execute-time\", \"3.0.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab-execute-time\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"date-fns\", \"2.29.3\", () => (__webpack_require__.e(\"vendors-node_modules_date-fns_esm_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/date-fns/esm/index.js */ \"./node_modules/date-fns/esm/index.js\"))))));\n\t\t\tregister(\"jupyterlab-execute-time\", \"3.0.1\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,4,0,0])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,2,0,1])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/date-fns/date-fns\": () => (loadStrictVersionCheckFallback(\"default\", \"date-fns\", [1,2,29,3], () => (__webpack_require__.e(\"vendors-node_modules_date-fns_esm_index_js\").then(() => (() => (__webpack_require__(/*! date-fns */ \"./node_modules/date-fns/esm/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/date-fns/date-fns\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,0,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,4,0,3])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,2,0,1])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/date-fns/date-fns\": () => (loadStrictVersionCheckFallback(\"default\", \"date-fns\", [1,2,29,3], () => (__webpack_require__.e(\"vendors-node_modules_date-fns_esm_index_js\").then(() => (() => (__webpack_require__(/*! date-fns */ \"./node_modules/date-fns/esm/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/date-fns/date-fns\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-execute-time\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_execute_time\"] = self[\"webpackChunkjupyterlab_execute_time\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-execute-time\");\n",
         ""
     ],
     "version": 3
```

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/style_index_js.3522f9e4692f1951c092.js` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/style_index_js.3522f9e4692f1951c092.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/style_index_js.3522f9e4692f1951c092.js.map` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/style_index_js.3522f9e4692f1951c092.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/vendors-node_modules_date-fns_esm_index_js.bb5155b17a678353747a.js` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/vendors-node_modules_date-fns_esm_index_js.bb5155b17a678353747a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time/labextension/static/vendors-node_modules_date-fns_esm_index_js.bb5155b17a678353747a.js.map` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/static/vendors-node_modules_date-fns_esm_index_js.bb5155b17a678353747a.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time.egg-info/PKG-INFO` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-execute-time
-Version: 3.0.0
+Version: 3.0.1
 Summary: Display cell timings in Jupyter Lab
 Home-page: https://github.com/deshaw/jupyterlab-execute-time
 Author: Marc Udoff
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jupyterlab_execute_time-3.0.0/jupyterlab_execute_time.egg-info/SOURCES.txt` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 jupyterlab_execute_time.egg-info/top_level.txt
 jupyterlab_execute_time/labextension/build_log.json
 jupyterlab_execute_time/labextension/package.json
 jupyterlab_execute_time/labextension/schemas/jupyterlab-execute-time/package.json.orig
 jupyterlab_execute_time/labextension/schemas/jupyterlab-execute-time/settings.json
 jupyterlab_execute_time/labextension/static/lib_index_js.d710423855898245e472.js
 jupyterlab_execute_time/labextension/static/lib_index_js.d710423855898245e472.js.map
-jupyterlab_execute_time/labextension/static/remoteEntry.45aa7d5d0f82a73e893e.js
-jupyterlab_execute_time/labextension/static/remoteEntry.45aa7d5d0f82a73e893e.js.map
+jupyterlab_execute_time/labextension/static/remoteEntry.c3b0015b00abd9869851.js
+jupyterlab_execute_time/labextension/static/remoteEntry.c3b0015b00abd9869851.js.map
 jupyterlab_execute_time/labextension/static/style.js
 jupyterlab_execute_time/labextension/static/style_index_js.3522f9e4692f1951c092.js
 jupyterlab_execute_time/labextension/static/style_index_js.3522f9e4692f1951c092.js.map
 jupyterlab_execute_time/labextension/static/vendors-node_modules_date-fns_esm_index_js.bb5155b17a678353747a.js
 jupyterlab_execute_time/labextension/static/vendors-node_modules_date-fns_esm_index_js.bb5155b17a678353747a.js.map
 src/ExecuteTimeWidget.ts
 src/formatters.ts
```

### Comparing `jupyterlab_execute_time-3.0.0/package.json` & `jupyterlab_execute_time-3.0.1/jupyterlab_execute_time/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9559566250742721%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/observables': '^4.0.0'}",*

 * * "'devDependencies'": "{'@types/json-schema': '^7.0.11', '@types/react': '^18.0.26', 'yjs': "*

 * *                      "'^13.5.0'}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.c3b0015b00abd9869851.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'3.0.1'"}*

```diff
@@ -3,24 +3,27 @@
         "url": "https://github.com/deshaw/jupyterlab-execute-time/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/cells": "^4.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/observables": "^4.0.0",
         "@jupyterlab/settingregistry": "^4.0.0",
         "@lumino/coreutils": "^2.0.0-rc.1",
         "@lumino/widgets": "^2.0.0-rc.1",
         "date-fns": "^2.29.3"
     },
     "description": "Display cell timings in Jupyter Lab",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@types/chai": "^4.3.4",
+        "@types/json-schema": "^7.0.11",
         "@types/mocha": "^10.0.1",
+        "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "~5.55.0",
         "@typescript-eslint/parser": "~5.55.0",
         "chai": "^4.3.7",
         "eslint": "~8.36.0",
         "eslint-config-prettier": "~8.7.0",
         "eslint-plugin-prettier": "~4.2.1",
         "husky": "^8.0.3",
@@ -28,24 +31,30 @@
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.4",
         "rimraf": "^4.4.0",
         "ts-mocha": "^10.0.0",
         "tslint": "^6.1.3",
         "tslint-config-prettier": "^1.18.0",
         "tslint-plugin-prettier": "^2.3.0",
-        "typescript": "~5.0.2"
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.0"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/deshaw/jupyterlab-execute-time",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.c3b0015b00abd9869851.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "jupyterlab_execute_time/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -83,9 +92,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "3.0.0"
+    "version": "3.0.1"
 }
```

### Comparing `jupyterlab_execute_time-3.0.0/setup.py` & `jupyterlab_execute_time-3.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 jupyterlab_execute_time setup.
 """
 import json
+import sys
 from pathlib import Path
 import setuptools
-from jupyter_packaging import wrap_installers, npm_builder, get_data_files
 
 HERE = Path(__file__).parent.resolve()
 
 # The name of the project
 name = "jupyterlab_execute_time"
 
 lab_path = HERE / name.replace("-", "_") / "labextension"
@@ -37,15 +37,15 @@
     url=pkg_json["homepage"],
     author="Marc Udoff",
     description=pkg_json["description"],
     license=pkg_json["license"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
-    install_requires=["jupyter_server>=2.0.1,<3"],
+    install_requires=["jupyterlab>=4,<5"],
     zip_safe=False,
     include_package_data=True,
     python_requires=">=3.7",
     platforms="Linux, Mac OS X, Windows",
     keywords=["Jupyter", "JupyterLab", "JupyterLab4"],
     classifiers=[
         "License :: OSI Approved :: BSD License",
@@ -61,17 +61,28 @@
         "Framework :: Jupyter :: JupyterLab :: 4",
         "Framework :: Jupyter :: JupyterLab :: Extensions",
         "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
     ],
 )
 
 
-post_develop = npm_builder(
-    build_cmd="install:extension", source_dir="src", build_dir=lab_path, npm="jlpm"
-)
-setup_args["cmdclass"] = wrap_installers(
-    post_develop=post_develop, ensured_targets=ensured_targets
-)
-setup_args["data_files"] = get_data_files(data_files_spec)
+try:
+    from jupyter_packaging import (
+        wrap_installers,
+        npm_builder,
+        get_data_files
+    )
+    post_develop = npm_builder(
+        build_cmd="install:extension", source_dir="src", build_dir=lab_path, npm="jlpm"
+    )
+    setup_args["cmdclass"] = wrap_installers(post_develop=post_develop, ensured_targets=ensured_targets)
+    setup_args["data_files"] = get_data_files(data_files_spec)
+except ImportError as e:
+    import logging
+    logging.basicConfig(format="%(levelname)s: %(message)s")
+    logging.warning("Build tool `jupyter-packaging` is missing. Install it with pip or conda.")
+    if not ("--name" in sys.argv or "--version" in sys.argv):
+        raise e
+
 
 if __name__ == "__main__":
     setuptools.setup(**setup_args)
```

### Comparing `jupyterlab_execute_time-3.0.0/src/ExecuteTimeWidget.ts` & `jupyterlab_execute_time-3.0.1/src/ExecuteTimeWidget.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/src/formatters.ts` & `jupyterlab_execute_time-3.0.1/src/formatters.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/src/index.ts` & `jupyterlab_execute_time-3.0.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/style/base.css` & `jupyterlab_execute_time-3.0.1/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/tsconfig.json` & `jupyterlab_execute_time-3.0.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/tslint.json` & `jupyterlab_execute_time-3.0.1/tslint.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_execute_time-3.0.0/yarn.lock` & `jupyterlab_execute_time-3.0.1/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -893,14 +893,27 @@
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
   checksum: 29ba29519fba567d0d686426b750d58bfddf6235cb3ad812ef671750637dbfcdafb5348feda44168d83f65936e5478562cffdc7ceeabac221fcdfab38f11bc31
   languageName: node
   linkType: hard
 
+"@jupyterlab/observables@npm:^4.0.0":
+  version: 4.6.5
+  resolution: "@jupyterlab/observables@npm:4.6.5"
+  dependencies:
+    "@lumino/algorithm": ^1.9.0
+    "@lumino/coreutils": ^1.11.0
+    "@lumino/disposable": ^1.10.0
+    "@lumino/messaging": ^1.10.0
+    "@lumino/signaling": ^1.10.0
+  checksum: 503b4f1c7d61fa3e7c69dc740a4d4a45948257434ebdcb875e86b03a818573250fe9824725a68c0d78715e1bac5c40cd412f387a159c8a40211115542a202030
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/observables@npm:^5.0.0":
   version: 5.0.0
   resolution: "@jupyterlab/observables@npm:5.0.0"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
@@ -1245,14 +1258,21 @@
   dependencies:
     "@lezer/highlight": "npm:^1.0.0"
     "@lezer/lr": "npm:^1.0.0"
   checksum: 271319aa7802c123845b70ffa63d7065c0f92fc6a1ddb1f8ec9f3aa965bca3df3c9fad4d4de53187ddf230e833cd3ab3a84cb2aded76ab5f6831e9a2fc310923
   languageName: node
   linkType: hard
 
+"@lumino/algorithm@npm:^1.9.0, @lumino/algorithm@npm:^1.9.2":
+  version: 1.9.2
+  resolution: "@lumino/algorithm@npm:1.9.2"
+  checksum: a89e7c63504236119634858e271db1cc649684d30ced5a6ebe2788af7c0837f1e05a6fd3047d8525eb756c42ce137f76b3688f75fd3ef915b71cd4f213dfbb96
+  languageName: node
+  linkType: hard
+
 "@lumino/algorithm@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/algorithm@npm:2.0.0"
   checksum: 663edf536e94397b449c6a2643a735e602fbb396dec86b56ad1193a768dce27c6e7da5ad0384aa90086ea44cbb64dde3f9d565e9fd81858f1eb0c6b4253f3b94
   languageName: node
   linkType: hard
 
@@ -1263,14 +1283,23 @@
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/widgets": ^2.1.1
   checksum: 442a047e43a85b48189d15a5a322f39cac01b9bee7b252aa76579c53e503f2cf2100f2e3aff61cd1d92fef07f04c0a3a6680c475890e0923456e296ceb79a692
   languageName: node
   linkType: hard
 
+"@lumino/collections@npm:^1.9.3":
+  version: 1.9.3
+  resolution: "@lumino/collections@npm:1.9.3"
+  dependencies:
+    "@lumino/algorithm": ^1.9.2
+  checksum: 1c87a12743eddd6f6b593e47945a5645e2f99ad61c5192499b0745e48ee9aff263c7145541e77dfeea4c9f50bdd017fddfa47bfc60e718de4f28533ce45bf8c3
+  languageName: node
+  linkType: hard
+
 "@lumino/collections@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/collections@npm:2.0.0"
   dependencies:
     "@lumino/algorithm": "npm:^2.0.0"
   checksum: 4a7fc3571e92a1368a1ef01300ad7b6e0d4ff13cb78b89533d5962eea66d4a7550e15d8b80fa3ab1816b1a89382f35015f9dddf72ab04654c17e5b516b845d8f
   languageName: node
@@ -1302,28 +1331,47 @@
     "@lumino/keyboard": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
   checksum: a076244e9c4f7a3c6dab02642fdd38dbbaab6e5754acaeeb84a5195dc5c2fc19343ba754c3a0f89c9b60f16c61cb793301cdb6e8d69bdc30e18ed7e32f40d524
   languageName: node
   linkType: hard
 
+"@lumino/coreutils@npm:^1.11.0":
+  version: 1.12.1
+  resolution: "@lumino/coreutils@npm:1.12.1"
+  peerDependencies:
+    crypto: 1.0.1
+  checksum: 55f1b87997f8dd0af28ff23c2d4b3aa252e515b9d3bc91b350a5c6c8526ceae61b14b55dc0d8d01691c69d42974b3d559f2b49bc7ced0f474b8f5dc52b3e83ed
+  languageName: node
+  linkType: hard
+
 "@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^2.1.1":
   version: 2.1.1
   resolution: "@lumino/coreutils@npm:2.1.1"
   checksum: dfdeb2b0282caae17b6c3edfebadf4ce7c75fc879fa60cacfef9b154412f4b35e4ffd95b1833b99d8dacb99aaaa04513570129ae2024c3f33e2677a01f0576ce
   languageName: node
   linkType: hard
 
 "@lumino/coreutils@npm:^2.0.0, @lumino/coreutils@npm:^2.0.0-rc.1":
   version: 2.0.0
   resolution: "@lumino/coreutils@npm:2.0.0"
   checksum: 341b5f569b2804e9651ecec6a441a0a0a9153656cc9dc0480eff8bb1d667df92ee4d64421fbb1469f0f503cd2ce3428c61dd3e5d2eb163e2e21748c318fd7b9e
   languageName: node
   linkType: hard
 
+"@lumino/disposable@npm:^1.10.0":
+  version: 1.10.4
+  resolution: "@lumino/disposable@npm:1.10.4"
+  dependencies:
+    "@lumino/algorithm": ^1.9.2
+    "@lumino/signaling": ^1.11.1
+  checksum: b53e259830f1d3231455548e6b95c9ae0f4b91e1b501980a1d0bb9708322bf5469b5cbb4e5005653d6f33b549d4bb7e58ce02226477876f51c124ea755152a33
+  languageName: node
+  linkType: hard
+
 "@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^2.1.1":
   version: 2.1.1
   resolution: "@lumino/disposable@npm:2.1.1"
   dependencies:
     "@lumino/signaling": ^2.1.1
   checksum: ed6cdfe13f3346178a087690d4e7baeccaed7e73ca23cb239765202409f5c01b4729a4058b4717f963462ee9ef2e5cb14ad1974e3163741267290edc3715c85c
   languageName: node
@@ -1368,14 +1416,24 @@
 "@lumino/keyboard@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/keyboard@npm:2.0.0"
   checksum: 3852ba51f437b1c1d7e552a0f844592a05e04dd5012070dc6e4384c58965d1ebf536c6875c1b7bae03cde3c715ddc36cd290992fcefc1a8c39094194f4689fdd
   languageName: node
   linkType: hard
 
+"@lumino/messaging@npm:^1.10.0":
+  version: 1.10.3
+  resolution: "@lumino/messaging@npm:1.10.3"
+  dependencies:
+    "@lumino/algorithm": ^1.9.2
+    "@lumino/collections": ^1.9.3
+  checksum: 1131e80379fa9b8a9b5d3418c90e25d4be48e2c92ec711518190772f9e8845a695bef45daddd06a129168cf6f158c8ad80ae86cb245f566e9195bbd9a0843b7a
+  languageName: node
+  linkType: hard
+
 "@lumino/messaging@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/messaging@npm:2.0.0"
   dependencies:
     "@lumino/algorithm": "npm:^2.0.0"
     "@lumino/collections": "npm:^2.0.0"
   checksum: 1e82dcf9b110834d4342dc63dfeac0ee780880fb99051bd82d00a1f83afd91b276c1cea5af85a414d92c527adc365d54f20ec780123b562f89c5a2cd3e96bf81
@@ -1389,14 +1447,21 @@
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
   checksum: 69177b26d5fc541e72533cbe7d7f7999eea541d392f1082d20dbd9e1797e7d46fba47bae9c65c06f9ccb2780cbae636e9354d9bf4423b5e1020754d4b07d4f6b
   languageName: node
   linkType: hard
 
+"@lumino/properties@npm:^1.8.2":
+  version: 1.8.2
+  resolution: "@lumino/properties@npm:1.8.2"
+  checksum: 9a53709fe58d3abbc99062f0c0fda4d5f64a4c7dca509251f0f89cdcaf881fdf6172ee852dbfe70594ee34bb97255acca771a722d62e7e2150ba8cf6f7e7d15c
+  languageName: node
+  linkType: hard
+
 "@lumino/properties@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/properties@npm:2.0.0"
   checksum: 81187a11a779eed4e20ff0035e77dee99bd271b0cf649096c4e8809dd6bdd06955b1a974bc1a115e536f8d2840b30183bb78a362b2c6991824477df6d17e6c59
   languageName: node
   linkType: hard
 
@@ -1406,14 +1471,24 @@
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
   checksum: 283ad4239b8577f68aca3d0b2606f73cc1c775f84cab25cf49aa6cd195f0d87949ef43fdff03b38b5a49ebbf2468581c6786d5f8b6159a04b2051260be5eab86
   languageName: node
   linkType: hard
 
+"@lumino/signaling@npm:^1.10.0, @lumino/signaling@npm:^1.11.1":
+  version: 1.11.1
+  resolution: "@lumino/signaling@npm:1.11.1"
+  dependencies:
+    "@lumino/algorithm": ^1.9.2
+    "@lumino/properties": ^1.8.2
+  checksum: 3d822be705d9ba8adc46ec405a4422cd4f76ed774f94da5386a511f01df4325c3c8bfa288c9c812184c94cfd0c3ef7b1121dcc9c9489750ad6cfaa7ffb2a3a67
+  languageName: node
+  linkType: hard
+
 "@lumino/signaling@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/signaling@npm:2.0.0"
   dependencies:
     "@lumino/algorithm": "npm:^2.0.0"
     "@lumino/coreutils": "npm:^2.0.0"
   checksum: fb46a1b33c4a0cec723e8c6f1a9b6e89544ee1a3b94731437639c0e9a1a29c07ff225179081846ee16c5001bf11bcaace646d1307bbb76ea6ae04006f442cd28
@@ -1596,14 +1671,21 @@
 "@types/json-schema@npm:*, @types/json-schema@npm:^7.0.5, @types/json-schema@npm:^7.0.8, @types/json-schema@npm:^7.0.9":
   version: 7.0.11
   resolution: "@types/json-schema@npm:7.0.11"
   checksum: 527bddfe62db9012fccd7627794bd4c71beb77601861055d87e3ee464f2217c85fca7a4b56ae677478367bbd248dbde13553312b7d4dbc702a2f2bbf60c4018d
   languageName: node
   linkType: hard
 
+"@types/json-schema@npm:^7.0.11":
+  version: 7.0.12
+  resolution: "@types/json-schema@npm:7.0.12"
+  checksum: 00239e97234eeb5ceefb0c1875d98ade6e922bfec39dd365ec6bd360b5c2f825e612ac4f6e5f1d13601b8b30f378f15e6faa805a3a732f4a1bbe61915163d293
+  languageName: node
+  linkType: hard
+
 "@types/json5@npm:^0.0.29":
   version: 0.0.29
   resolution: "@types/json5@npm:0.0.29"
   checksum: e60b153664572116dfea673c5bda7778dbff150498f44f998e34b5886d8afc47f16799280e4b6e241c0472aef1bc36add771c569c68fc5125fc2ae519a3eb9ac
   languageName: node
   linkType: hard
 
@@ -4238,19 +4320,22 @@
   resolution: "jupyterlab-execute-time@workspace:."
   dependencies:
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
     "@jupyterlab/cells": ^4.0.0
     "@jupyterlab/docregistry": ^4.0.0
     "@jupyterlab/notebook": ^4.0.0
+    "@jupyterlab/observables": ^4.0.0
     "@jupyterlab/settingregistry": ^4.0.0
     "@lumino/coreutils": ^2.0.0-rc.1
     "@lumino/widgets": ^2.0.0-rc.1
     "@types/chai": ^4.3.4
+    "@types/json-schema": ^7.0.11
     "@types/mocha": ^10.0.1
+    "@types/react": ^18.0.26
     "@typescript-eslint/eslint-plugin": ~5.55.0
     "@typescript-eslint/parser": ~5.55.0
     chai: ^4.3.7
     date-fns: ^2.29.3
     eslint: ~8.36.0
     eslint-config-prettier: ~8.7.0
     eslint-plugin-prettier: ~4.2.1
@@ -4260,14 +4345,15 @@
     prettier: ^2.8.4
     rimraf: ^4.4.0
     ts-mocha: ^10.0.0
     tslint: ^6.1.3
     tslint-config-prettier: ^1.18.0
     tslint-plugin-prettier: ^2.3.0
     typescript: ~5.0.2
+    yjs: ^13.5.0
   languageName: unknown
   linkType: soft
 
 "kind-of@npm:^6.0.2":
   version: 6.0.3
   resolution: "kind-of@npm:6.0.3"
   checksum: 3ab01e7b1d440b22fe4c31f23d8d38b4d9b91d9f291df683476576493d5dfd2e03848a8b05813dd0c3f0e835bc63f433007ddeceb71f05cb25c45ae1b19c6d3b
@@ -4292,14 +4378,26 @@
   bin:
     0gentesthtml: bin/gentesthtml.js
     0serve: bin/0serve.js
   checksum: bfad469101984c8d1a7d56d7170977494e2c99137603d93950ba14fa6214a38e85e32016c78dd033c80ada88959fb2abd60544cd8eab3bdf0e1a5349635ac585
   languageName: node
   linkType: hard
 
+"lib0@npm:^0.2.74":
+  version: 0.2.78
+  resolution: "lib0@npm:0.2.78"
+  dependencies:
+    isomorphic.js: ^0.2.4
+  bin:
+    0gentesthtml: bin/gentesthtml.js
+    0serve: bin/0serve.js
+  checksum: a9c90a9228e10e581bf416f4ecade967687d67e6ea3e822ef69e2628a77a2a0254ef7e2eb7e555d412f9e9467049b7fb760c079878f9a934dd85d2646a53d172
+  languageName: node
+  linkType: hard
+
 "license-webpack-plugin@npm:^2.3.14":
   version: 2.3.21
   resolution: "license-webpack-plugin@npm:2.3.21"
   dependencies:
     "@types/webpack-sources": "npm:^0.1.5"
     webpack-sources: "npm:^1.2.0"
   peerDependenciesMeta:
@@ -6712,14 +6810,23 @@
     string-width: "npm:^4.2.0"
     y18n: "npm:^5.0.5"
     yargs-parser: "npm:^20.2.2"
   checksum: b14afbb51e3251a204d81937c86a7e9d4bdbf9a2bcee38226c900d00f522969ab675703bee2a6f99f8e20103f608382936034e64d921b74df82b63c07c5e8f59
   languageName: node
   linkType: hard
 
+"yjs@npm:^13.5.0":
+  version: 13.6.7
+  resolution: "yjs@npm:13.6.7"
+  dependencies:
+    lib0: ^0.2.74
+  checksum: 8e89257c8b565ab97cf3354fca2ce0b6bc3d1abe90b9d45a218a94b35da372c88d2411b353ed8ca03a6619004c4da76c96f7c203c38506c3758c9f8c1a730ca4
+  languageName: node
+  linkType: hard
+
 "yjs@npm:^13.5.40":
   version: 13.5.50
   resolution: "yjs@npm:13.5.50"
   dependencies:
     lib0: "npm:^0.2.49"
   checksum: 1c636eadcb4191adec1b31819c8f97f90f3d9f5300856f612ec0b7313ac1ed867810c8dc16b39ddc1bba73abe247b1d2ceae70699589a384318c0b0f3dd14124
   languageName: node
```

