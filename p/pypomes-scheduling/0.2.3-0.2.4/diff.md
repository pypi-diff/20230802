# Comparing `tmp/pypomes_scheduling-0.2.3.tar.gz` & `tmp/pypomes_scheduling-0.2.4.tar.gz`

## Comparing `pypomes_scheduling-0.2.3.tar` & `pypomes_scheduling-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/src/pypomes_scheduling/__threaded_scheduler.py
--rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/src/pypomes_scheduling/__threaded_scheduler.py
+-rw-r--r--   0        0        0     9671 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/PKG-INFO
```

### Comparing `pypomes_scheduling-0.2.3/src/pypomes_scheduling/__threaded_scheduler.py` & `pypomes_scheduling-0.2.4/src/pypomes_scheduling/__threaded_scheduler.py`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.2.3/src/pypomes_scheduling/scheduling_pomes.py` & `pypomes_scheduling-0.2.4/src/pypomes_scheduling/scheduling_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,19 +197,17 @@
 
     :param errors: incidental errors
     :param badge: optional badge identifying the scheduler
     :param must_exist: True if scheduler must exist
     :return: the scheduler retrieved, or None otherwise
     """
     curr_badge = badge or __DEFAULT_BADGE
-    result: __ThreadedScheduler = __schedulers[curr_badge]
+    result: __ThreadedScheduler = __schedulers.get(curr_badge)
     if must_exist and result is None:
         errors.append(f"Job scheduler '{curr_badge}' has not been created")
-    elif not must_exist and result is not None:
-        errors.append(f"Job scheduler '{curr_badge}' has already been created")
         
     return result
 
 
 def __scheduler_add_job(errors: list[str], scheduler: __ThreadedScheduler,
                         job: callable, job_id: str, job_name: str,
                         job_cron: str = None, job_start: datetime = None,
```

### Comparing `pypomes_scheduling-0.2.3/LICENSE` & `pypomes_scheduling-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.2.3/pyproject.toml` & `pypomes_scheduling-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_scheduling-0.2.3/PKG-INFO` & `pypomes_scheduling-0.2.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_scheduling
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection of Python pomes, pennyeach (scheduling module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Scheduling
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Scheduling/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

