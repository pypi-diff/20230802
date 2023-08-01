# Comparing `tmp/agentshell-0.0.6.tar.gz` & `tmp/agentshell-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentshell-0.0.6.tar", last modified: Sat Jul 29 00:35:08 2023, max compression
+gzip compressed data, was "agentshell-0.0.7.tar", last modified: Tue Aug  1 23:28:23 2023, max compression
```

## Comparing `agentshell-0.0.6.tar` & `agentshell-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:08.257503 agentshell-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-29 00:34:55.000000 agentshell-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-29 00:35:08.257503 agentshell-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-29 00:34:55.000000 agentshell-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:08.253503 agentshell-0.0.6/agentshell/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-29 00:34:55.000000 agentshell-0.0.6/agentshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-29 00:34:55.000000 agentshell-0.0.6/agentshell/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-29 00:34:55.000000 agentshell-0.0.6/agentshell/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:35:08.257503 agentshell-0.0.6/agentshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-29 00:35:08.000000 agentshell-0.0.6/agentshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-29 00:35:08.000000 agentshell-0.0.6/agentshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:35:08.000000 agentshell-0.0.6/agentshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 00:35:08.000000 agentshell-0.0.6/agentshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 00:35:08.000000 agentshell-0.0.6/agentshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:35:08.257503 agentshell-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-29 00:34:55.000000 agentshell-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:28:23.444087 agentshell-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-01 23:28:14.000000 agentshell-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-08-01 23:28:23.444087 agentshell-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-08-01 23:28:14.000000 agentshell-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:28:23.444087 agentshell-0.0.7/agentshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-01 23:28:14.000000 agentshell-0.0.7/agentshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-08-01 23:28:14.000000 agentshell-0.0.7/agentshell/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-08-01 23:28:14.000000 agentshell-0.0.7/agentshell/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:28:23.444087 agentshell-0.0.7/agentshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-08-01 23:28:23.000000 agentshell-0.0.7/agentshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-01 23:28:23.000000 agentshell-0.0.7/agentshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:28:23.000000 agentshell-0.0.7/agentshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 23:28:23.000000 agentshell-0.0.7/agentshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 23:28:23.000000 agentshell-0.0.7/agentshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 23:28:23.444087 agentshell-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-01 23:28:14.000000 agentshell-0.0.7/setup.py
```

### Comparing `agentshell-0.0.6/LICENSE` & `agentshell-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agentshell-0.0.6/PKG-INFO` & `agentshell-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentshell
-Version: 0.0.6
+Version: 0.0.7
 Summary: A shell for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentshell
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentshell-0.0.6/README.md` & `agentshell-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `agentshell-0.0.6/agentshell/__init__.py` & `agentshell-0.0.7/agentshell/__init__.py`

 * *Files identical despite different names*

### Comparing `agentshell-0.0.6/agentshell/action.py` & `agentshell-0.0.7/agentshell/action.py`

 * *Files identical despite different names*

### Comparing `agentshell-0.0.6/agentshell/main.py` & `agentshell-0.0.7/agentshell/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,27 +269,30 @@
     # Execute command in the current working directory
     command_to_run = f"cd {cwd} && {command}"
     process = subprocess.run(command_to_run, shell=True, text=True, capture_output=True)
 
     # If the process completed successfully
     if process.returncode == 0:
         result = process.stdout
+        error = process.stderr
+
+        success = error == "" or error is None
 
         result_split = result.strip().split("\n")
         updated_directory = result_split[-1]
         if os.path.isdir(updated_directory):
             cwd = updated_directory
             set_cwd(cwd, shell_id)
             result_split = result_split[:-1]
             result_split = "\n".join(result_split)
         else:
             result_split = "\n".join(result_split)
 
         add_to_shell_history(shell_id, command, success="True", output=result)
-        return { "success": True, "output": result_split, "error": None }
+        return { "success": success, "output": result_split, "error": error }
 
     else:  # If the process did not complete successfully
         output = process.stdout
         error = process.stderr
         add_to_shell_history(
             shell_id, command, success="False", output=output, error=error
         )
```

### Comparing `agentshell-0.0.6/agentshell.egg-info/PKG-INFO` & `agentshell-0.0.7/agentshell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentshell
-Version: 0.0.6
+Version: 0.0.7
 Summary: A shell for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentshell
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentshell-0.0.6/setup.py` & `agentshell-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="agentshell",
-    version="0.0.6",
+    version="0.0.7",
     description="A shell for your agent.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentshell",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

