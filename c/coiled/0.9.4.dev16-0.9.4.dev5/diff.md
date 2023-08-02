# Comparing `tmp/coiled-0.9.4.dev16.tar.gz` & `tmp/coiled-0.9.4.dev5.tar.gz`

## Comparing `coiled-0.9.4.dev16.tar` & `coiled-0.9.4.dev5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/analytics.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/auth.py
--rw-r--r--   0        0        0    25197 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/capture_environment.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/context.py
--rw-r--r--   0        0        0   102304 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/exceptions.py
--rw-r--r--   0        0        0     7798 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/function.py
--rw-r--r--   0        0        0    20053 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/scan.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/shutdown.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/types.py
--rw-r--r--   0        0        0    56663 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/utils.py
--rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/config.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/core.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/env.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/login.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/prefect.py
--rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/utils.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    48989 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    27132 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/v2/__init__.py
--rw-r--r--   0        0        0   100331 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/v2/cluster.py
--rw-r--r--   0        0        0    59205 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16304 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/.gitignore
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/README.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/pyproject.toml
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 coiled-0.9.4.dev16/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/analytics.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/auth.py
+-rw-r--r--   0        0        0    25197 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/capture_environment.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/context.py
+-rw-r--r--   0        0        0   102304 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/exceptions.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/run.py
+-rw-r--r--   0        0        0    20053 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/scan.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/shutdown.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/types.py
+-rw-r--r--   0        0        0    56663 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/utils.py
+-rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/config.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/core.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/env.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/utils.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    48989 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    27132 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/v2/__init__.py
+-rw-r--r--   0        0        0   100308 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    59205 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16304 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/.gitignore
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/README.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/pyproject.toml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 coiled-0.9.4.dev5/PKG-INFO
```

### Comparing `coiled-0.9.4.dev16/coiled/__init__.py` & `coiled-0.9.4.dev5/coiled/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     GCPOptions,
     better_cluster_logs,
     cluster_logs,
     create_cluster,
     delete_cluster,
     list_clusters,
 )
-from .function import run, function
+from .run import run
 from importlib_metadata import version
 
 inspect = _inspect.callback
 del _inspect
 
 # Register coiled configuration values with Dask's config system
 from . import config
```

### Comparing `coiled-0.9.4.dev16/coiled/analytics.py` & `coiled-0.9.4.dev5/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/auth.py` & `coiled-0.9.4.dev5/coiled/auth.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/capture_environment.py` & `coiled-0.9.4.dev5/coiled/capture_environment.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cluster.py` & `coiled-0.9.4.dev5/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/coiled.yaml` & `coiled-0.9.4.dev5/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/context.py` & `coiled-0.9.4.dev5/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/core.py` & `coiled-0.9.4.dev5/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/exceptions.py` & `coiled-0.9.4.dev5/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/function.py` & `coiled-0.9.4.dev5/coiled/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import os
 import sys
 import threading
-import warnings
 from typing import Optional, Union
 
 import dask.distributed
 from dask.base import tokenize
 from dask.utils import parse_timedelta
 
 import coiled
@@ -28,15 +27,15 @@
         self.keepalive = parse_timedelta(keepalive)
 
         token = tokenize(
             sys.executable,
             # TODO: include something about the software environment
             **cluster_kwargs,
         )
-        self._name = f"function-{token[:8]}"
+        self._name = f"run-{token[:8]}"
 
     @property
     def cluster(self) -> coiled.Cluster:
         with _lock:
             try:
                 return _clusters[self._name]
             except KeyError:
@@ -72,15 +71,15 @@
         """Submit function call for asynchronous execution
 
         This immediately returns a Dask Future, allowing for the submission of
         many tasks in parallel.
 
         Example
         -------
-        >>> @coiled.function()
+        >>> @coiled.run()
         ... def f(x):
         ...    return x + 1
 
         >>> f(10)  # calling the function blocks until finished
         11
         >>> f.submit(10)  # immediately returns a future
         <Future: pending, key=f-1234>
@@ -94,15 +93,15 @@
         Returns
         -------
         future: dask.distributed.Future
         """
         return self.client.submit(self.function, *args, **kwargs)
 
 
-def function(
+def run(
     *,
     software: Optional[str] = None,
     container: Optional[str] = None,
     vm_type: Optional[Union[str, list[str]]] = None,
     cpu: Optional[Union[int, list[int]]] = None,
     memory: Optional[Union[str, list[str]]] = None,
     gpu: Optional[bool] = None,
@@ -134,19 +133,19 @@
         from that image. Note that this should not be used with package sync or when specifying
         an existing Coiled software environment.
     vm_type
         Instance type, or list of instance types, that you would like to use.
         You can use ``coiled.list_instance_types()`` to see a list of allowed types.
     cpu
         Number, or range, of CPUs requested. Specify a range by
-        using a list of two elements, for example: ``cpu=[2, 8]``.
+        using a list of two elements, for example: ``worker_cpu=[2, 8]``.
     memory
-        Amount of memory to request for each VM, Coiled will use a +/- 10% buffer
+        Amount of memory to request for each worker, Coiled will use a +/- 10% buffer
         from the memory that you specify. You may specify a range of memory by using a
-        list of two elements, for example: ``memory=["2GiB", "4GiB"]``.
+        list of two elements, for example: ``worker_memory=["2GiB", "4GiB"]``.
     gpu
         Whether to attach a GPU; this would be a single NVIDIA T4.
     region
         The cloud provider region in which to run the cluster.
     arm
         Whether to use ARM instances for cluster; default is x86 (Intel) instances.
     keepalive
@@ -156,20 +155,20 @@
         Shut down the cluster after this duration if no activity has occurred. Default is "24 hours".
 
 
     See the :class:`coiled.Cluster` docstring for additional parameter descriptions.
 
     .. warning::
 
-        ``@coiled.function`` is an experimental feature and is subject to breaking changes.
+        ``@coiled.run`` is an experimental feature and is subject to breaking changes.
 
     Examples
     --------
     >>> import coiled
-    >>> @coiled.function()
+    >>> @coiled.run()
     ... def f(x):
     ...    return x + 1
 
     >>> f(10)  # calling the function blocks until finished
     11
     >>> f.submit(10)  # immediately returns a future
     <Future: pending, key=f-1234>
@@ -206,25 +205,14 @@
             environ=environ,
             scheduler_gpu=gpu,
             region=region,
             arm=arm,
             shutdown_on_close=shutdown_on_close,
             compute_purchase_option=compute_purchase_option,
             extra_worker_on_scheduler=True,
-            tags={"coiled-cluster-type": "function"},
+            tags={"coiled-cluster-type": "run/python"},
             worker_options={"nthreads": 1},
         )
 
         return Function(func, cluster_kwargs, keepalive=keepalive)
 
     return decorator
-
-
-# Small backwards compatibility shim
-def run(*args, **kwargs):
-    warnings.warn(
-        "coiled.run has been renamed to coiled.function. "
-        "Please use coiled.function as coiled.run will be removed in a future release.",
-        FutureWarning,
-        stacklevel=2,
-    )
-    return function(*args, **kwargs)
```

### Comparing `coiled-0.9.4.dev16/coiled/scan.py` & `coiled-0.9.4.dev5/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/shutdown.py` & `coiled-0.9.4.dev5/coiled/shutdown.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/software.py` & `coiled-0.9.4.dev5/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/types.py` & `coiled-0.9.4.dev5/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/utils.py` & `coiled-0.9.4.dev5/coiled/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/websockets.py` & `coiled-0.9.4.dev5/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/config.py` & `coiled-0.9.4.dev5/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/core.py` & `coiled-0.9.4.dev5/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/curl.py` & `coiled-0.9.4.dev5/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/env.py` & `coiled-0.9.4.dev5/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/login.py` & `coiled-0.9.4.dev5/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/package_sync.py` & `coiled-0.9.4.dev5/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/prefect.py` & `coiled-0.9.4.dev5/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/run.py` & `coiled-0.9.4.dev5/coiled/cli/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,58 +122,57 @@
     try:
         print()
         print(f"Setting up [bold]{shlex.join(command)}[/bold]...")
         print("-" * len(f"Setting up {shlex.join(command)}..."))
         print()
         name = name or f"run-{uuid.uuid4().hex[:8]}"
 
-        with coiled.Cloud(account=account) as cloud:
-            with coiled.Cluster(
-                name=name,
-                cloud=cloud,
-                n_workers=0,
-                software=software,
-                container=container,
-                scheduler_options={"idle_timeout": "24 hours"},
-                scheduler_vm_types=list(vm_type) if vm_type else None,
-                worker_vm_types=list(vm_type) if vm_type else None,
-                allow_ssh=True,
-                extra_worker_on_scheduler=True,
-                environ=env,
-                scheduler_gpu=gpu,
-                region=region,
-                tags={"coiled-cluster-type": "run/cli"},
-            ) as cluster:
-                info["cluster_id"] = cluster.cluster_id
-                with Client(cluster) as client:
-                    # Extract and upload files from `command`
-                    command = shlex.split(" ".join(command))
-                    info["files-implicit"] = []
-                    for idx, i in enumerate(command):
-                        if os.path.exists(i) and os.path.isfile(i):
-                            client.upload_file(i, load=False)
-                            info["files-implicit"].append(i)
-                            command[idx] = os.path.basename(i)
-                    # Upload user-specified files too
-                    info["files-explicit"] = file
-                    for f in file:
-                        client.upload_file(f, load=False)
-
-                    def run_command(command):
-                        subprocess.run(command, cwd=get_worker().local_directory)
-
-                    info["command-parsed"] = command
-
-                    # keep track of time before we start executing user code
-                    start_ns = time.time_ns()
-
-                    # TODO execute command in non-blocking way so we can also tail logs while it runs
-                    client.submit(run_command, command=["echo", "@start-coiled-run"]).result()
-                    client.submit(run_command, command=command).result()
-                    client.submit(run_command, command=["echo", "@stop-coiled-run"]).result()
+        with coiled.Cluster(
+            name=name,
+            account=account,
+            n_workers=0,
+            software=software,
+            container=container,
+            scheduler_options={"idle_timeout": "24 hours"},
+            scheduler_vm_types=list(vm_type) if vm_type else None,
+            worker_vm_types=list(vm_type) if vm_type else None,
+            allow_ssh=True,
+            extra_worker_on_scheduler=True,
+            environ=env,
+            scheduler_gpu=gpu,
+            region=region,
+            tags={"coiled-cluster-type": "run/cli"},
+        ) as cluster:
+            info["cluster_id"] = cluster.cluster_id
+            with Client(cluster) as client:
+                # Extract and upload files from `command`
+                command = shlex.split(" ".join(command))
+                info["files-implicit"] = []
+                for idx, i in enumerate(command):
+                    if os.path.exists(i) and os.path.isfile(i):
+                        client.upload_file(i, load=False)
+                        info["files-implicit"].append(i)
+                        command[idx] = os.path.basename(i)
+                # Upload user-specified files too
+                info["files-explicit"] = file
+                for f in file:
+                    client.upload_file(f, load=False)
+
+                def run_command(command):
+                    subprocess.run(command, cwd=get_worker().local_directory)
+
+                info["command-parsed"] = command
+
+                # keep track of time before we start executing user code
+                start_ns = time.time_ns()
+
+                # TODO execute command in non-blocking way so we can also tail logs while it runs
+                client.submit(run_command, command=["echo", "@start-coiled-run"]).result()
+                client.submit(run_command, command=command).result()
+                client.submit(run_command, command=["echo", "@stop-coiled-run"]).result()
 
         if cluster.cluster_id:
             print()
 
             print("Output")
             print("-" * len("Output"))
             print()
```

### Comparing `coiled-0.9.4.dev16/coiled/cli/utils.py` & `coiled-0.9.4.dev5/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/cluster/__init__.py` & `coiled-0.9.4.dev5/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/cluster/better_logs.py` & `coiled-0.9.4.dev5/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/cluster/logs.py` & `coiled-0.9.4.dev5/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/cluster/metrics.py` & `coiled-0.9.4.dev5/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/cluster/ssh.py` & `coiled-0.9.4.dev5/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/cluster/utils.py` & `coiled-0.9.4.dev5/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/notebook/__init__.py` & `coiled-0.9.4.dev5/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/notebook/notebook.py` & `coiled-0.9.4.dev5/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/setup/__init__.py` & `coiled-0.9.4.dev5/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/setup/amp.py` & `coiled-0.9.4.dev5/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/setup/aws.py` & `coiled-0.9.4.dev5/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/setup/entry.py` & `coiled-0.9.4.dev5/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/setup/gcp.py` & `coiled-0.9.4.dev5/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/cli/setup/prometheus.py` & `coiled-0.9.4.dev5/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/extensions/prefect/runners.py` & `coiled-0.9.4.dev5/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/extensions/prefect/workers.py` & `coiled-0.9.4.dev5/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/v2/__init__.py` & `coiled-0.9.4.dev5/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/v2/cluster.py` & `coiled-0.9.4.dev5/coiled/v2/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -947,31 +947,26 @@
             # fall back to the note if no error is present
             # this only really happens if a user specified
             # a critical package to ignore
             failure_str = ", ".join([f'{pkg["name"]} - {pkg["error"] or pkg["note"]}' for pkg in halting_failures])
             raise RuntimeError(
                 f"""Issues with critical packages: {failure_str}
 
-Your software environment has conflicting dependency requirements.
-
-Consider creating a new environment.
-
-By specifying your packages at once, you're more likely to get a consistent set of versions.
+Your software environment has conflicting dependency requirements. In this situation, Coiled recommends creating a
+new environment. By specifying your list of desired packages together, you're much more likely to get a set of
+consistent versions.
 
 If you use conda:
-
     conda create -n myenv -c conda-forge coiled package1 package2 package3
 
 If you use pip/venv, create a new environment and then:
-
     pip install coiled package1 package2 package3
 or
     pip install -r requirements.txt
-
-If that does not solve your issue, please contact support@coiled.io."""
+"""
             )
 
     @track_context
     async def _attach_to_cluster(self, is_new_cluster: bool):
         # update our view of workers in case someone tries scaling
         # it might be better to continually update this while waiting for the
         # cluster in _security below, but this seems OK for now
```

### Comparing `coiled-0.9.4.dev16/coiled/v2/core.py` & `coiled-0.9.4.dev5/coiled/v2/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/v2/cwi_log_link.py` & `coiled-0.9.4.dev5/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/v2/states.py` & `coiled-0.9.4.dev5/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/v2/widgets/__init__.py` & `coiled-0.9.4.dev5/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/v2/widgets/rich.py` & `coiled-0.9.4.dev5/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/coiled/v2/widgets/util.py` & `coiled-0.9.4.dev5/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/README.md` & `coiled-0.9.4.dev5/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/pyproject.toml` & `coiled-0.9.4.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.9.4.dev16/PKG-INFO` & `coiled-0.9.4.dev5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.9.4.dev16
+Version: 0.9.4.dev5
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.9.4.dev16 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.9.4.dev5 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: gilknocker>=0.4.1 Requires-Dist: importlib-metadata Requires-
 Dist: ipywidgets Requires-Dist: jmespath Requires-Dist: jsondiff Requires-Dist:
 packaging Requires-Dist: pip Requires-Dist: pip>=19.3 Requires-Dist:
```

