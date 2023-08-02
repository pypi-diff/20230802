# Comparing `tmp/pypomes_scheduling-0.2.2.tar.gz` & `tmp/pypomes_scheduling-0.2.3.tar.gz`

## Comparing `pypomes_scheduling-0.2.2.tar` & `pypomes_scheduling-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/src/pypomes_scheduling/__threaded_scheduler.py
--rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/src/pypomes_scheduling/__threaded_scheduler.py
+-rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.3/PKG-INFO
```

### Comparing `pypomes_scheduling-0.2.2/src/pypomes_scheduling/__threaded_scheduler.py` & `pypomes_scheduling-0.2.3/src/pypomes_scheduling/__threaded_scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,45 +12,43 @@
 
     This implementation may run as single or multiple instances, each on its own thread.
     """
     _scheduler: BlockingScheduler
     _logger: logging.Logger
     _stopped: bool
 
-    def __init__(self, timezone: pytz.timezone, retry_interval: int, logger: logging.Logger = None):
+    def __init__(self, timezone: pytz.timezone, retry_interval: int, logger: logging.Logger = None) -> None:
 
         threading.Thread.__init__(self)
 
         self._stopped = False
         self._logger = logger
         self._scheduler = BlockingScheduler(logging=logger,
                                             timezone=timezone,
                                             jobstore_retry_interval=retry_interval)
         if self._logger is not None:
             self._logger.info("Instanced, with timezone "
                               f"'{timezone}' and retry interval '{retry_interval}'")
 
-    def run(self):
-        """
-        Start the scheduler in its own thread.
-        """
+    def run(self) -> None:
+        """Start the scheduler in its own thread."""
         # stay in loop until 'stop()' is invoked
         while not self._stopped:
             if self._logger is not None:
                 self._logger.info("Started")
 
             # start the scheduler, blocking the thread until it is interrupted
             self._scheduler.start()
 
         self._scheduler.shutdown()
         if self._logger is not None:
             self._logger.info("Finished")
 
     def schedule_job(self, job: callable, job_id: str, job_name: str, job_cron: str = None,
-                     job_start: datetime = None, job_args: tuple = None, job_kwargs: dict = None):
+                     job_start: datetime = None, job_args: tuple = None, job_kwargs: dict = None) -> None:
         """
         Schedule the given *job*, with the given parameters.
 
         :param job: the callable object to be scheduled
         :param job_id: the id of the scheduled job
         :param job_name: the name of the scheduled job
         :param job_cron: the CRON expression directing the execution times
@@ -97,14 +95,14 @@
                                 args=job_args,
                                 kwargs=job_kwargs,
                                 id=job_id,
                                 name=job_name)
         if self._logger is not None:
             self._logger.info(f"Job '{job_name}' scheduled, with CRON '{job_cron}'")
 
-    def stop(self):
+    def stop(self) -> None:
         """
-        Stop the scheduler.
+          Stop the scheduler.
         """
         if self._logger is not None:
             self._logger.info("Finishing...")
         self._stopped = True
```

### Comparing `pypomes_scheduling-0.2.2/src/pypomes_scheduling/scheduling_pomes.py` & `pypomes_scheduling-0.2.3/src/pypomes_scheduling/scheduling_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 import pytz
 import re
 import sys
 from .__threaded_scheduler import __ThreadedScheduler
 
 __DEFAULT_BADGE: Final[str] = "__default__"
 
-__REGEX_VERIFY_CRON: Final[str] = "/(@(annually|yearly|monthly|weekly|daily|hourly|reboot))|" \
-                                  "(@every (\d+(ns|us|µs|ms|s|m|h))+)|((((\d+,)+\d+|(\d+(\/|-)\d+)|\d+|\*) ?){5,7})"
+__REGEX_VERIFY_CRON: Final[str] = (
+    "/(@(annually|yearly|monthly|weekly|daily|hourly|reboot))|"
+    "(@every (\d+(ns|us|µs|ms|s|m|h))+)|((((\d+,)+\d+|(\d+(\/|-)\d+)|\d+|\*) ?){5,7})"
+)
 
 # dict holding the schedulers created:
 #   { <badge-1>: <scheduler-instance-1>,
 #     ...
 #     <badge-n>: <scheduler-instance-n>
 #   }
 __schedulers: dict = {}
@@ -48,30 +50,30 @@
         except Exception as e:
             errors.append(f"Error creating the job scheduler '{curr_badge}': "
                           f"{exc_format(e, sys.exc_info())}")
 
     return result
 
 
-def scheduler_destroy(badge: str = None):
+def scheduler_destroy(badge: str = None) -> None:
     """
     Destroy the scheduler identified by *badge*. *Noop* if the scheduler does not exist.
 
     :param badge:  optional badge identifying the scheduler
     """
     # define the badge
     curr_badge: str = badge or __DEFAULT_BADGE
 
     # does the scheduler exist ?
     if __schedulers.get(curr_badge) is not None:
         # yes, discard it
         __schedulers.pop(curr_badge)
 
 
-def scheduler_start(errors: list[str], badge: str = None):
+def scheduler_start(errors: list[str], badge: str = None) -> bool:
     """
     Start the scheduler.
 
     :param errors: incidental errors
     :param badge: optional badge identifying the scheduler
     :return: True if the scheduler has been started, False otherwise
     """
@@ -89,15 +91,15 @@
         except Exception as e:
             errors.append(f"Error starting the scheduler '{badge or __DEFAULT_BADGE}': "
                           f"{exc_format(e, sys.exc_info())}")
 
     return result
 
 
-def scheduler_stop(errors: list[str], badge: str = None):
+def scheduler_stop(errors: list[str], badge: str = None) -> bool:
     """
     Stop the scheduler.
 
     :param errors: incidental errors
     :param badge: optional badge identifying the scheduler
     :return: True if the scheduler has been stopped, False otherwise
     """
@@ -115,16 +117,17 @@
     return result
 
 
 def scheduler_add_job(errors: list[str], job: callable, job_id: str, job_name: str,
                       job_cron: str = None, job_start: datetime = None,
                       job_args: tuple = None, job_kwargs: dict = None, badge: str = None) -> bool:
     """
-    Schedule the job identified as *job_id* and named as *job_name*,
-    with the *CRON* expression *job_cron*, starting at the timestamp *job_start*.
+    Schedule the job identified as *job_id* and named as *job_name*.
+
+    The scheduling is performed with the *CRON* expression *job_cron*, starting at the timestamp *job_start*.
     Positional arguments for the scheduled job may be provided in *job_args*.
     Named arguments for the scheduled job may be provided in *job_kwargs*.
     Return *True* if the scheduling was successful.
 
     :param errors: incidental errors
     :param job: the job to be scheduled
     :param job_id: the id of the job to be scheduled
@@ -151,14 +154,15 @@
 
 
 def scheduler_add_jobs(errors: list[str],
                        jobs: list[tuple[callable, str, str, str, datetime, tuple, dict]],
                        badge: str = None) -> int:
     """
     Schedule the jobs described in *jobs*, starting at the given *start*.
+
     Each element in the job list is a *tuple* with the corresponding job data:
     *(callable function, job id, job name, CRON expression, start timestamp, job args, job kwargs)*.
     Only the first three data items are required.
 
     :param errors: incidental errors
     :param jobs: list of tuples containing the jobs to schedule
     :param badge: optional badge identifying the scheduler
@@ -192,15 +196,14 @@
     Retrieve the scheduler identified by *badge*.
 
     :param errors: incidental errors
     :param badge: optional badge identifying the scheduler
     :param must_exist: True if scheduler must exist
     :return: the scheduler retrieved, or None otherwise
     """
-    
     curr_badge = badge or __DEFAULT_BADGE
     result: __ThreadedScheduler = __schedulers[curr_badge]
     if must_exist and result is None:
         errors.append(f"Job scheduler '{curr_badge}' has not been created")
     elif not must_exist and result is not None:
         errors.append(f"Job scheduler '{curr_badge}' has already been created")
         
@@ -208,16 +211,17 @@
 
 
 def __scheduler_add_job(errors: list[str], scheduler: __ThreadedScheduler,
                         job: callable, job_id: str, job_name: str,
                         job_cron: str = None, job_start: datetime = None,
                         job_args: tuple = None, job_kwargs: dict = None) -> bool:
     """
-    Use *scheduler* to schedule the job identified as *job_id* and named as *job_name*,
-    with the *CRON* expression *job_cron*, starting at the timestamp *job_start*.
+    Use *scheduler* to schedule the job identified as *job_id* and named as *job_name*.
+
+    The scheduling is performed with the *CRON* expression *job_cron*, starting at the timestamp *job_start*.
     Positional arguments for the scheduled job may be provided in *job_args*.
     Named arguments for the scheduled job may be provided in *job_kwargs*.
     Return *True* if the scheduling was successful.
 
     :param errors: incidental errors
     :param scheduler: the scheduler to use
     :param job: the job to be scheduled
```

### Comparing `pypomes_scheduling-0.2.2/LICENSE` & `pypomes_scheduling-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.2.2/pyproject.toml` & `pypomes_scheduling-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=23.2.1",
-    "pypomes_core>=0.2.1",
+    "pypomes_core>=0.2.2",
     "APScheduler>=3.10.1",
     "setuptools>=68.0.0",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Scheduling"
```

### Comparing `pypomes_scheduling-0.2.2/PKG-INFO` & `pypomes_scheduling-0.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pypomes_scheduling
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection of Python pomes, pennyeach (scheduling module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Scheduling
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Scheduling/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: apscheduler>=3.10.1
 Requires-Dist: pip>=23.2.1
-Requires-Dist: pypomes-core>=0.2.1
+Requires-Dist: pypomes-core>=0.2.2
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.41.0
```

