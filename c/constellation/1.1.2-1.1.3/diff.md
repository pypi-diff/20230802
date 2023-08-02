# Comparing `tmp/constellation-1.1.2.tar.gz` & `tmp/constellation-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constellation-1.1.2.tar", last modified: Mon Jul 31 14:09:00 2023, max compression
+gzip compressed data, was "constellation-1.1.3.tar", last modified: Wed Aug  2 10:24:05 2023, max compression
```

## Comparing `constellation-1.1.2.tar` & `constellation-1.1.3.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-31 14:09:00.076382 constellation-1.1.2/
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     1096 2023-05-23 18:31:17.000000 constellation-1.1.2/LICENSE
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      960 2023-07-31 14:09:00.076382 constellation-1.1.2/PKG-INFO
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      481 2023-05-23 18:31:17.000000 constellation-1.1.2/README.md
-drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-31 14:09:00.076382 constellation-1.1.2/constellation/
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      337 2023-05-23 18:31:17.000000 constellation-1.1.2/constellation/__init__.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     4910 2023-07-31 11:59:53.000000 constellation-1.1.2/constellation/config.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)    10451 2023-07-27 08:09:53.000000 constellation-1.1.2/constellation/constellation.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     6866 2023-05-23 18:31:17.000000 constellation-1.1.2/constellation/docker_util.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     1460 2023-05-23 18:31:17.000000 constellation-1.1.2/constellation/notifier.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      536 2023-05-23 18:31:17.000000 constellation-1.1.2/constellation/util.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     2883 2023-07-31 14:08:33.000000 constellation-1.1.2/constellation/vault.py
-drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-31 14:09:00.076382 constellation-1.1.2/constellation.egg-info/
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      960 2023-07-31 14:09:00.000000 constellation-1.1.2/constellation.egg-info/PKG-INFO
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      566 2023-07-31 14:09:00.000000 constellation-1.1.2/constellation.egg-info/SOURCES.txt
--rw-rw-r--   0 aehill    (1000) aehill    (1000)        1 2023-07-31 14:09:00.000000 constellation-1.1.2/constellation.egg-info/dependency_links.txt
--rw-rw-r--   0 aehill    (1000) aehill    (1000)        1 2023-07-31 14:09:00.000000 constellation-1.1.2/constellation.egg-info/not-zip-safe
--rw-rw-r--   0 aehill    (1000) aehill    (1000)       36 2023-07-31 14:09:00.000000 constellation-1.1.2/constellation.egg-info/requires.txt
--rw-rw-r--   0 aehill    (1000) aehill    (1000)       14 2023-07-31 14:09:00.000000 constellation-1.1.2/constellation.egg-info/top_level.txt
--rw-rw-r--   0 aehill    (1000) aehill    (1000)       63 2023-07-31 14:09:00.076382 constellation-1.1.2/setup.cfg
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     1007 2023-07-31 14:08:47.000000 constellation-1.1.2/setup.py
-drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-31 14:09:00.076382 constellation-1.1.2/test/
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     7550 2023-07-31 11:59:53.000000 constellation-1.1.2/test/test_config.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)    14233 2023-07-27 08:09:53.000000 constellation-1.1.2/test/test_constellation.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     7595 2023-05-23 18:31:17.000000 constellation-1.1.2/test/test_docker_util.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     1805 2023-05-23 18:31:17.000000 constellation-1.1.2/test/test_notify.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      398 2023-05-23 18:31:17.000000 constellation-1.1.2/test/test_util.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     5455 2023-07-31 14:07:08.000000 constellation-1.1.2/test/test_vault.py
+drwxrwxr-x   0 rfitzjoh  (1001) rfitzjoh  (1001)        0 2023-08-02 10:24:05.743935 constellation-1.1.3/
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)     1060 2023-08-02 10:24:05.743935 constellation-1.1.3/PKG-INFO
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)      480 2023-08-02 10:23:45.000000 constellation-1.1.3/README.md
+drwxrwxr-x   0 rfitzjoh  (1001) rfitzjoh  (1001)        0 2023-08-02 10:24:05.739935 constellation-1.1.3/constellation/
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)      337 2023-08-02 10:23:45.000000 constellation-1.1.3/constellation/__init__.py
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)     4910 2023-08-02 10:23:45.000000 constellation-1.1.3/constellation/config.py
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)    10451 2023-08-02 10:23:45.000000 constellation-1.1.3/constellation/constellation.py
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)     6886 2023-08-02 10:23:45.000000 constellation-1.1.3/constellation/docker_util.py
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)     1460 2023-08-02 10:23:45.000000 constellation-1.1.3/constellation/notifier.py
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)      536 2023-08-02 10:23:45.000000 constellation-1.1.3/constellation/util.py
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)     2883 2023-08-02 10:23:45.000000 constellation-1.1.3/constellation/vault.py
+drwxrwxr-x   0 rfitzjoh  (1001) rfitzjoh  (1001)        0 2023-08-02 10:24:05.739935 constellation-1.1.3/constellation.egg-info/
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)     1060 2023-08-02 10:24:05.000000 constellation-1.1.3/constellation.egg-info/PKG-INFO
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)      558 2023-08-02 10:24:05.000000 constellation-1.1.3/constellation.egg-info/SOURCES.txt
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)        1 2023-08-02 10:24:05.000000 constellation-1.1.3/constellation.egg-info/dependency_links.txt
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)        1 2023-08-02 10:24:05.000000 constellation-1.1.3/constellation.egg-info/not-zip-safe
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)       36 2023-08-02 10:24:05.000000 constellation-1.1.3/constellation.egg-info/requires.txt
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)       14 2023-08-02 10:24:05.000000 constellation-1.1.3/constellation.egg-info/top_level.txt
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)       63 2023-08-02 10:24:05.743935 constellation-1.1.3/setup.cfg
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)     1007 2023-08-02 10:23:45.000000 constellation-1.1.3/setup.py
+drwxrwxr-x   0 rfitzjoh  (1001) rfitzjoh  (1001)        0 2023-08-02 10:24:05.743935 constellation-1.1.3/test/
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)     7550 2023-08-02 10:23:45.000000 constellation-1.1.3/test/test_config.py
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)    14233 2023-08-02 10:23:45.000000 constellation-1.1.3/test/test_constellation.py
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)     7976 2023-08-02 10:23:45.000000 constellation-1.1.3/test/test_docker_util.py
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)     1805 2023-08-02 10:23:45.000000 constellation-1.1.3/test/test_notify.py
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)      398 2023-08-02 10:23:45.000000 constellation-1.1.3/test/test_util.py
+-rw-rw-r--   0 rfitzjoh  (1001) rfitzjoh  (1001)     5455 2023-08-02 10:23:45.000000 constellation-1.1.3/test/test_vault.py
```

### Comparing `constellation-1.1.2/PKG-INFO` & `constellation-1.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: constellation
-Version: 1.1.2
+Version: 1.1.3
 Summary: Deploy scripts for constellations of docker containers
 Home-page: https://github.com/reside-ic/constellation
 Author: Rich FitzJohn
 Author-email: r.fitzjohn@imperial.ac.uk
 License: MIT
+Description: ## constellation
+        
+        [![Build Status](https://github.com/reside-ic/constellation/actions/workflows/test.yml/badge.svg)](https://github.com/reside-ic/constellation/actions)
+        [![codecov.io](https://codecov.io/github/reside-ic/constellation/coverage.svg?branch=master)](https://codecov.io/github/reside-ic/constellation?branch=master)
+        
+        ## Installation
+        
+        From local sources
+        
+        ```
+        python3 setup.py install --user
+        ```
+        
+        (you may need `--upgrade` to upgrade older versions of python packages).
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## constellation
-
-[![Build Status](https://github.com/reside-ic/constellation/actions/workflows/test.yml/badge.svg))](https://github.com/reside-ic/constellation/actions)
-[![codecov.io](https://codecov.io/github/reside-ic/constellation/coverage.svg?branch=master)](https://codecov.io/github/reside-ic/constellation?branch=master)
-
-## Installation
-
-From local sources
-
-```
-python3 setup.py install --user
-```
-
-(you may need `--upgrade` to upgrade older versions of python packages).
-
-
```

### Comparing `constellation-1.1.2/constellation/config.py` & `constellation-1.1.3/constellation/config.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.2/constellation/constellation.py` & `constellation-1.1.3/constellation/constellation.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.2/constellation/docker_util.py` & `constellation-1.1.3/constellation/docker_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     try:
         client.volumes.get(name)
     except docker.errors.NotFound:
         print("Creating docker volume '{}'".format(name))
         client.volumes.create(name)
 
 
-def exec_safely(container, args):
-    ans = container.exec_run(args)
+def exec_safely(container, args, **kwargs):
+    ans = container.exec_run(args, **kwargs)
     if ans[0] != 0:
         print(ans[1].decode("UTF-8"))
         raise Exception("Error running command (see above for log)")
     return ans
 
 
 def return_logs_and_remove(image, args=None, mounts=None):
```

### Comparing `constellation-1.1.2/constellation/notifier.py` & `constellation-1.1.3/constellation/notifier.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.2/constellation/util.py` & `constellation-1.1.3/constellation/util.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.2/constellation/vault.py` & `constellation-1.1.3/constellation/vault.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.2/constellation.egg-info/PKG-INFO` & `constellation-1.1.3/constellation.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: constellation
-Version: 1.1.2
+Version: 1.1.3
 Summary: Deploy scripts for constellations of docker containers
 Home-page: https://github.com/reside-ic/constellation
 Author: Rich FitzJohn
 Author-email: r.fitzjohn@imperial.ac.uk
 License: MIT
+Description: ## constellation
+        
+        [![Build Status](https://github.com/reside-ic/constellation/actions/workflows/test.yml/badge.svg)](https://github.com/reside-ic/constellation/actions)
+        [![codecov.io](https://codecov.io/github/reside-ic/constellation/coverage.svg?branch=master)](https://codecov.io/github/reside-ic/constellation?branch=master)
+        
+        ## Installation
+        
+        From local sources
+        
+        ```
+        python3 setup.py install --user
+        ```
+        
+        (you may need `--upgrade` to upgrade older versions of python packages).
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## constellation
-
-[![Build Status](https://github.com/reside-ic/constellation/actions/workflows/test.yml/badge.svg))](https://github.com/reside-ic/constellation/actions)
-[![codecov.io](https://codecov.io/github/reside-ic/constellation/coverage.svg?branch=master)](https://codecov.io/github/reside-ic/constellation?branch=master)
-
-## Installation
-
-From local sources
-
-```
-python3 setup.py install --user
-```
-
-(you may need `--upgrade` to upgrade older versions of python packages).
-
-
```

### Comparing `constellation-1.1.2/constellation.egg-info/SOURCES.txt` & `constellation-1.1.3/constellation.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.cfg
 setup.py
 constellation/__init__.py
 constellation/config.py
 constellation/constellation.py
 constellation/docker_util.py
```

### Comparing `constellation-1.1.2/setup.py` & `constellation-1.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "docker",
     "hvac",
     "pytest",
     "pyyaml",
     "vault_dev"]
 
 setup(name="constellation",
-      version="1.1.2",
+      version="1.1.3",
       description="Deploy scripts for constellations of docker containers",
       long_description=long_description,
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
       ],
```

### Comparing `constellation-1.1.2/test/test_config.py` & `constellation-1.1.3/test/test_config.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.2/test/test_constellation.py` & `constellation-1.1.3/test/test_constellation.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.2/test/test_docker_util.py` & `constellation-1.1.3/test/test_docker_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,25 @@
     container = cl.containers.run("alpine", ["sleep", "10"],
                                   detach=True, auto_remove=True)
     with pytest.raises(Exception):
         exec_safely(container, "missing_command")
     container.kill()
 
 
+def test_exec_can_pass_kwargs():
+    cl = docker.client.from_env()
+    container = cl.containers.run("alpine", ["sleep", "10"],
+                                  detach=True, auto_remove=True)
+    res = exec_safely(container, "ls", workdir="/bin")
+    out = res.output.decode("UTF-8").strip().split("\n")
+    container.kill()
+    assert res.exit_code == 0
+    assert "ls" in out
+
+
 def test_remove_network_removes_network():
     cl = docker.client.from_env()
     name = "constellation_test_nw"
 
     cl.networks.create(name)
 
     f = io.StringIO()
```

### Comparing `constellation-1.1.2/test/test_notify.py` & `constellation-1.1.3/test/test_notify.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.2/test/test_vault.py` & `constellation-1.1.3/test/test_vault.py`

 * *Files identical despite different names*

