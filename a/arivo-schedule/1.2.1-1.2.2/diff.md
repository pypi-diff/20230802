# Comparing `tmp/arivo_schedule-1.2.1.tar.gz` & `tmp/arivo_schedule-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arivo_schedule-1.2.1.tar", last modified: Tue Jun  6 12:07:50 2023, max compression
+gzip compressed data, was "arivo_schedule-1.2.2.tar", last modified: Wed Aug  2 13:57:01 2023, max compression
```

## Comparing `arivo_schedule-1.2.1.tar` & `arivo_schedule-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 senfth    (1000) senfth    (1000)        0 2023-06-06 12:07:50.745273 arivo_schedule-1.2.1/
--rw-rw-r--   0 senfth    (1000) senfth    (1000)     1933 2023-06-06 06:57:48.000000 arivo_schedule-1.2.1/AUTHORS.rst
--rw-rw-r--   0 senfth    (1000) senfth    (1000)     6415 2023-06-06 06:57:48.000000 arivo_schedule-1.2.1/HISTORY.rst
--rw-rw-r--   0 senfth    (1000) senfth    (1000)     1099 2023-06-06 06:57:48.000000 arivo_schedule-1.2.1/LICENSE.txt
--rw-rw-r--   0 senfth    (1000) senfth    (1000)      147 2023-06-06 06:57:48.000000 arivo_schedule-1.2.1/MANIFEST.in
--rw-rw-r--   0 senfth    (1000) senfth    (1000)     3252 2023-06-06 12:07:50.745273 arivo_schedule-1.2.1/PKG-INFO
--rw-rw-r--   0 senfth    (1000) senfth    (1000)     2282 2023-06-06 06:57:48.000000 arivo_schedule-1.2.1/README.rst
-drwxrwxr-x   0 senfth    (1000) senfth    (1000)        0 2023-06-06 12:07:50.745273 arivo_schedule-1.2.1/arivo_schedule.egg-info/
--rw-rw-r--   0 senfth    (1000) senfth    (1000)     3252 2023-06-06 12:07:50.000000 arivo_schedule-1.2.1/arivo_schedule.egg-info/PKG-INFO
--rw-rw-r--   0 senfth    (1000) senfth    (1000)      267 2023-06-06 12:07:50.000000 arivo_schedule-1.2.1/arivo_schedule.egg-info/SOURCES.txt
--rw-rw-r--   0 senfth    (1000) senfth    (1000)        1 2023-06-06 12:07:50.000000 arivo_schedule-1.2.1/arivo_schedule.egg-info/dependency_links.txt
--rw-rw-r--   0 senfth    (1000) senfth    (1000)        9 2023-06-06 12:07:50.000000 arivo_schedule-1.2.1/arivo_schedule.egg-info/top_level.txt
-drwxrwxr-x   0 senfth    (1000) senfth    (1000)        0 2023-06-06 12:07:50.745273 arivo_schedule-1.2.1/schedule/
--rw-rw-r--   0 senfth    (1000) senfth    (1000)    31066 2023-06-06 08:53:24.000000 arivo_schedule-1.2.1/schedule/__init__.py
--rw-rw-r--   0 senfth    (1000) senfth    (1000)       93 2023-06-06 12:07:50.745273 arivo_schedule-1.2.1/setup.cfg
--rw-rw-r--   0 senfth    (1000) senfth    (1000)     1426 2023-06-06 12:07:45.000000 arivo_schedule-1.2.1/setup.py
--rw-rw-r--   0 senfth    (1000) senfth    (1000)    37190 2023-06-06 08:53:09.000000 arivo_schedule-1.2.1/test_schedule.py
+drwxrwxr-x   0 breast    (1000) breast    (1000)        0 2023-08-02 13:57:01.782868 arivo_schedule-1.2.2/
+-rw-rw-r--   0 breast    (1000) breast    (1000)     1933 2023-08-02 13:17:57.000000 arivo_schedule-1.2.2/AUTHORS.rst
+-rw-rw-r--   0 breast    (1000) breast    (1000)     6415 2023-08-02 13:17:57.000000 arivo_schedule-1.2.2/HISTORY.rst
+-rw-rw-r--   0 breast    (1000) breast    (1000)     1099 2023-08-02 13:17:57.000000 arivo_schedule-1.2.2/LICENSE.txt
+-rw-rw-r--   0 breast    (1000) breast    (1000)      147 2023-08-02 13:17:57.000000 arivo_schedule-1.2.2/MANIFEST.in
+-rw-rw-r--   0 breast    (1000) breast    (1000)     3232 2023-08-02 13:57:01.782868 arivo_schedule-1.2.2/PKG-INFO
+-rw-rw-r--   0 breast    (1000) breast    (1000)     2282 2023-08-02 13:17:57.000000 arivo_schedule-1.2.2/README.rst
+drwxrwxr-x   0 breast    (1000) breast    (1000)        0 2023-08-02 13:57:01.782868 arivo_schedule-1.2.2/arivo_schedule.egg-info/
+-rw-rw-r--   0 breast    (1000) breast    (1000)     3232 2023-08-02 13:57:01.000000 arivo_schedule-1.2.2/arivo_schedule.egg-info/PKG-INFO
+-rw-rw-r--   0 breast    (1000) breast    (1000)      267 2023-08-02 13:57:01.000000 arivo_schedule-1.2.2/arivo_schedule.egg-info/SOURCES.txt
+-rw-rw-r--   0 breast    (1000) breast    (1000)        1 2023-08-02 13:57:01.000000 arivo_schedule-1.2.2/arivo_schedule.egg-info/dependency_links.txt
+-rw-rw-r--   0 breast    (1000) breast    (1000)        9 2023-08-02 13:57:01.000000 arivo_schedule-1.2.2/arivo_schedule.egg-info/top_level.txt
+drwxrwxr-x   0 breast    (1000) breast    (1000)        0 2023-08-02 13:57:01.782868 arivo_schedule-1.2.2/schedule/
+-rw-rw-r--   0 breast    (1000) breast    (1000)    31005 2023-08-02 13:20:11.000000 arivo_schedule-1.2.2/schedule/__init__.py
+-rw-rw-r--   0 breast    (1000) breast    (1000)       93 2023-08-02 13:57:01.782868 arivo_schedule-1.2.2/setup.cfg
+-rw-rw-r--   0 breast    (1000) breast    (1000)     1426 2023-08-02 13:54:48.000000 arivo_schedule-1.2.2/setup.py
+-rw-rw-r--   0 breast    (1000) breast    (1000)    38463 2023-08-02 13:44:31.000000 arivo_schedule-1.2.2/test_schedule.py
```

### Comparing `arivo_schedule-1.2.1/AUTHORS.rst` & `arivo_schedule-1.2.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `arivo_schedule-1.2.1/HISTORY.rst` & `arivo_schedule-1.2.2/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `arivo_schedule-1.2.1/LICENSE.txt` & `arivo_schedule-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arivo_schedule-1.2.1/PKG-INFO` & `arivo_schedule-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: arivo_schedule
-Version: 1.2.1
+Version: 1.2.2
 Summary: Job scheduling for humans.
 Home-page: https://github.com/ts-accessio/schedule
 Author: Daniel Bader
 Author-email: mail@dbader.org
 License: MIT
 Keywords: schedule,periodic,jobs,scheduling,clockwork,cron,scheduler,job scheduling
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -91,9 +90,7 @@
 Daniel Bader - `@dbader_org <https://twitter.com/dbader_org>`_ - mail@dbader.org
 
 Inspired by `Adam Wiggins' <https://github.com/adamwiggins>`_ article `"Rethinking Cron" <https://adam.herokuapp.com/past/2010/4/13/rethinking_cron/>`_ and the `clockwork <https://github.com/Rykian/clockwork>`_ Ruby module.
 
 Distributed under the MIT license. See `LICENSE.txt <https://github.com/dbader/schedule/blob/master/LICENSE.txt>`_ for more information.
 
 https://github.com/dbader/schedule
-
-
```

### Comparing `arivo_schedule-1.2.1/README.rst` & `arivo_schedule-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `arivo_schedule-1.2.1/arivo_schedule.egg-info/PKG-INFO` & `arivo_schedule-1.2.2/arivo_schedule.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: arivo-schedule
-Version: 1.2.1
+Version: 1.2.2
 Summary: Job scheduling for humans.
 Home-page: https://github.com/ts-accessio/schedule
 Author: Daniel Bader
 Author-email: mail@dbader.org
 License: MIT
 Keywords: schedule,periodic,jobs,scheduling,clockwork,cron,scheduler,job scheduling
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -91,9 +90,7 @@
 Daniel Bader - `@dbader_org <https://twitter.com/dbader_org>`_ - mail@dbader.org
 
 Inspired by `Adam Wiggins' <https://github.com/adamwiggins>`_ article `"Rethinking Cron" <https://adam.herokuapp.com/past/2010/4/13/rethinking_cron/>`_ and the `clockwork <https://github.com/Rykian/clockwork>`_ Ruby module.
 
 Distributed under the MIT license. See `LICENSE.txt <https://github.com/dbader/schedule/blob/master/LICENSE.txt>`_ for more information.
 
 https://github.com/dbader/schedule
-
-
```

### Comparing `arivo_schedule-1.2.1/schedule/__init__.py` & `arivo_schedule-1.2.2/schedule/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -707,14 +707,24 @@
         self._schedule_next_run()
 
         if self._is_overdue(self.next_run):
             logger.debug("Cancelling job %s", self)
             return CancelJob
         return ret
 
+    def _localize(self, dt: datetime.datetime):
+        if not self.at_time_zone:
+            return dt
+        try:
+            return self.at_time_zone.localize(dt)
+        except Exception:
+            # if the code above fails, we are using dateutil
+            from dateutil.tz import UTC, tzlocal
+            return dt.replace(tzinfo=tzlocal()).astimezone(self.at_time_zone)
+
     def _schedule_next_run(self) -> None:
         """
         Compute the instant when this job should run next.
         """
         if self.unit not in ("seconds", "minutes", "hours", "days", "weeks"):
             raise ScheduleValueError(
                 "Invalid unit (valid units are `seconds`, `minutes`, `hours`, "
@@ -725,15 +735,17 @@
             if not (self.latest >= self.interval):
                 raise ScheduleError("`latest` is greater than `interval`")
             interval = random.randint(self.interval, self.latest)
         else:
             interval = self.interval
 
         self.period = datetime.timedelta(**{self.unit: interval})
-        self.next_run = datetime.datetime.now() + self.period
+        # localize here to avoid errors due to daylight savings time
+        self.next_run = self._localize(datetime.datetime.now())
+        self.next_run += self.period
         if self.start_day is not None:
             if self.unit != "weeks":
                 raise ScheduleValueError("`unit` should be 'weeks'")
             weekdays = (
                 "monday",
                 "tuesday",
                 "wednesday",
@@ -747,63 +759,50 @@
                     "Invalid start day (valid start days are {})".format(weekdays)
                 )
             weekday = weekdays.index(self.start_day)
             days_ahead = weekday - self.next_run.weekday()
             if days_ahead <= 0:  # Target day already happened this week
                 days_ahead += 7
             self.next_run += datetime.timedelta(days_ahead) - self.period
+
         if self.at_time is not None:
             if self.unit not in ("days", "hours", "minutes") and self.start_day is None:
                 raise ScheduleValueError("Invalid unit without specifying start day")
             kwargs = {"second": self.at_time.second, "microsecond": 0}
             if self.unit == "days" or self.start_day is not None:
                 kwargs["hour"] = self.at_time.hour
             if self.unit in ["days", "hours"] or self.start_day is not None:
                 kwargs["minute"] = self.at_time.minute
             self.next_run = self.next_run.replace(**kwargs)  # type: ignore
 
-            if self.at_time_zone is not None:
-                # Convert next_run from the expected timezone into the local time
-                # self.next_run is a naive datetime so after conversion remove tzinfo
-                try:
-                    self.next_run = (
-                        self.at_time_zone.localize(self.next_run)
-                        .astimezone()
-                        .replace(tzinfo=None)
-                    )
-                except Exception:
-                    # if the code above fails, we are using dateutil
-                    self.next_run = self.next_run.replace(tzinfo=self.at_time_zone).astimezone().replace(tzinfo=None)
-
             # Make sure we run at the specified time *today* (or *this hour*)
             # as well. This accounts for when a job takes so long it finished
             # in the next period.
-            if not self.last_run or (self.next_run - self.last_run) > self.period:
-                now = datetime.datetime.now()
-                if (
-                    self.unit == "days"
-                    and self.at_time > now.time()
-                    and self.interval == 1
-                ):
+            if not self.last_run or (self.next_run - self._localize(self.last_run)) > self.period:
+                now = self._localize(datetime.datetime.now())
+                if self.unit == "days" and self.at_time > now.time() and self.interval == 1:
                     self.next_run = self.next_run - datetime.timedelta(days=1)
                 elif self.unit == "hours" and (
-                    self.at_time.minute > now.minute
-                    or (
-                        self.at_time.minute == now.minute
-                        and self.at_time.second > now.second
-                    )
+                        self.at_time.minute > now.minute
+                        or (
+                                self.at_time.minute == now.minute
+                                and self.at_time.second > now.second
+                        )
                 ):
                     self.next_run = self.next_run - datetime.timedelta(hours=1)
                 elif self.unit == "minutes" and self.at_time.second > now.second:
                     self.next_run = self.next_run - datetime.timedelta(minutes=1)
         if self.start_day is not None and self.at_time is not None:
             # Let's see if we will still make that time we specified today
-            if (self.next_run - datetime.datetime.now()).days >= 7:
+            if (self.next_run - self._localize(datetime.datetime.now())).days >= 7:
                 self.next_run -= self.period
 
+        if self.at_time_zone is not None:
+            self.next_run = self.next_run.astimezone().replace(tzinfo=None)
+
     def _is_overdue(self, when: datetime.datetime):
         return self.cancel_after is not None and when > self.cancel_after
 
     def _decode_datetimestr(
         self, datetime_str: str, formats: List[str]
     ) -> Optional[datetime.datetime]:
         for f in formats:
```

### Comparing `arivo_schedule-1.2.1/setup.py` & `arivo_schedule-1.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import codecs
 from setuptools import setup
 
 
-SCHEDULE_VERSION = "1.2.1"
+SCHEDULE_VERSION = "1.2.2"
 
 
 def read_file(filename):
     """
     Read a utf8 encoded text file and return its contents.
     """
     with codecs.open(filename, "r", "utf8") as f:
```

### Comparing `arivo_schedule-1.2.1/test_schedule.py` & `arivo_schedule-1.2.2/test_schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,14 +283,36 @@
         with self.assertRaises(IntervalError):
             every(interval=2).friday
         with self.assertRaises(IntervalError):
             every(interval=2).saturday
         with self.assertRaises(IntervalError):
             every(interval=2).sunday
 
+    def test_at_time_tz(self):
+        """Test schedule with utc time having different date than local time"""
+        mock_job = make_mock_job()
+        # mocked times are local time
+        from dateutil.tz import UTC, tzlocal
+        with mock_datetime(2023, 8, 1, 11, 30):
+            job = every().day.at("00:30", "Europe/Vienna").do(mock_job)
+            initial_run = datetime.datetime(2023, 8, 1, 22, 30, tzinfo=UTC).astimezone(tzlocal()).replace(tzinfo=None)
+            self.assertEqual(initial_run, job.next_run)
+
+        rt1 = datetime.datetime(2023, 8, 1, 22, 15, tzinfo=UTC).astimezone(tzlocal()).replace(tzinfo=None)
+        with mock_datetime(rt1.year, rt1.month, rt1.day, rt1.hour, rt1.minute):
+            self.assertEqual(False, job.should_run)
+
+        rt2 = datetime.datetime(2023, 8, 1, 22, 35, tzinfo=UTC).astimezone(tzlocal()).replace(tzinfo=None)
+        with mock_datetime(rt2.year, rt2.month, rt2.day, rt2.hour, rt2.minute):
+            self.assertEqual(True, job.should_run)
+            job.run()
+            self.assertEqual(datetime.datetime.now(), job.last_run)
+            next_run_time = datetime.datetime(2023, 8, 2, 22, 30, tzinfo=UTC).astimezone(tzlocal()).replace(tzinfo=None)
+            self.assertEqual(next_run_time, job.next_run)
+
     def test_until_time(self):
         mock_job = make_mock_job()
         # Check argument parsing
         with mock_datetime(2020, 1, 1, 10, 0, 0) as m:
             assert every().day.until(datetime.datetime(3000, 1, 1, 20, 30)).do(
                 mock_job
             ).cancel_after == datetime.datetime(3000, 1, 1, 20, 30, 0)
```

