# Comparing `tmp/apparent-0.1.2.tar.gz` & `tmp/apparent-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apparent-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "apparent-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `apparent-0.1.2.tar` & `apparent-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,28 @@
--rwxr-xr-x   0        0        0     6413 2023-07-20 20:59:05.115769 apparent-0.1.2/.gitignore
--rw-r--r--   0        0        0    11357 2023-07-06 21:22:31.764821 apparent-0.1.2/LICENSE.txt
--rwxr-xr-x   0        0        0     5054 2023-07-20 20:01:34.669401 apparent-0.1.2/README.md
--rw-r--r--   0        0        0     6148 2023-07-13 16:08:13.480811 apparent-0.1.2/apparent/.DS_Store
--rwxr-xr-x   0        0        0        0 2023-06-22 22:19:57.000000 apparent-0.1.2/apparent/__init__.py
--rw-r--r--   0        0        0     9362 2023-07-20 21:27:03.306883 apparent-0.1.2/apparent/timing.py
--rwxr-xr-x   0        0        0       92 2023-07-20 16:31:06.798096 apparent-0.1.2/bin/install-dev
--rwxr-xr-x   0        0        0      224 2023-07-20 16:37:18.635949 apparent-0.1.2/bin/test
--rwxr-xr-x   0        0        0      156 2023-07-20 16:35:45.141454 apparent-0.1.2/bin/test-coverage
--rw-r--r--   0        0        0     1575 2023-07-12 17:15:11.209433 apparent-0.1.2/doc/K.svg
--rw-r--r--   0        0        0     3930 2023-07-12 17:22:30.136488 apparent-0.1.2/doc/diffs.svg
--rw-r--r--   0        0        0     1203 2023-07-12 17:27:01.825682 apparent-0.1.2/doc/variance.md
--rw-r--r--   0        0        0     6200 2023-07-12 17:13:05.887758 apparent-0.1.2/doc/variance.svg
--rw-r--r--   0        0        0     9346 2023-07-12 17:15:49.766608 apparent-0.1.2/doc/variance_calc.svg
--rwxr-xr-x   0        0        0     1025 2023-07-20 21:27:49.647195 apparent-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 21:32:41.925459 apparent-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     3751 2023-07-07 22:04:36.624455 apparent-0.1.2/tests/timer_results_tests.py
--rw-r--r--   0        0        0     6049 2023-07-19 19:30:18.766728 apparent-0.1.2/tests/timer_tests.py
--rw-r--r--   0        0        0     1613 2023-07-12 17:32:41.188742 apparent-0.1.2/tests/variance_tests.py
--rw-r--r--   0        0        0     5725 1970-01-01 00:00:00.000000 apparent-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      835 2023-07-20 21:51:33.459428 apparent-0.1.3/.github/python-publish.yml
+-rwxr-xr-x   0        0        0     6413 2023-07-20 20:59:05.115769 apparent-0.1.3/.gitignore
+-rw-r--r--   0        0        0    11357 2023-07-06 21:22:31.764821 apparent-0.1.3/LICENSE.txt
+-rwxr-xr-x   0        0        0     5105 2023-07-20 22:12:09.800394 apparent-0.1.3/README.md
+-rw-r--r--   0        0        0     6148 2023-07-13 16:08:13.480811 apparent-0.1.3/apparent/.DS_Store
+-rwxr-xr-x   0        0        0        0 2023-06-22 22:19:57.000000 apparent-0.1.3/apparent/__init__.py
+-rw-r--r--   0        0        0     2295 2023-08-02 21:02:15.635509 apparent-0.1.3/apparent/reports.py
+-rw-r--r--   0        0        0     9459 2023-08-02 20:45:54.245193 apparent-0.1.3/apparent/timing.py
+-rwxr-xr-x   0        0        0      115 2023-08-01 16:11:59.291998 apparent-0.1.3/bin/build-docs
+-rwxr-xr-x   0        0        0       99 2023-08-01 16:10:10.091991 apparent-0.1.3/bin/install-dev
+-rwxr-xr-x   0        0        0      224 2023-07-20 16:37:18.635949 apparent-0.1.3/bin/test
+-rwxr-xr-x   0        0        0      156 2023-07-20 16:35:45.141454 apparent-0.1.3/bin/test-coverage
+-rw-r--r--   0        0        0     1575 2023-07-12 17:15:11.209433 apparent-0.1.3/doc/K.svg
+-rw-r--r--   0        0        0     3930 2023-07-12 17:22:30.136488 apparent-0.1.3/doc/diffs.svg
+-rw-r--r--   0        0        0     1203 2023-07-12 17:27:01.825682 apparent-0.1.3/doc/variance.md
+-rw-r--r--   0        0        0     6200 2023-07-12 17:13:05.887758 apparent-0.1.3/doc/variance.svg
+-rw-r--r--   0        0        0     9346 2023-07-12 17:15:49.766608 apparent-0.1.3/doc/variance_calc.svg
+-rw-r--r--   0        0        0     6717 2023-08-02 20:45:54.245535 apparent-0.1.3/html/apparent/index.html
+-rw-r--r--   0        0        0    12625 2023-08-02 20:45:54.246145 apparent-0.1.3/html/apparent/reports.html
+-rw-r--r--   0        0        0    57545 2023-08-02 20:45:54.246681 apparent-0.1.3/html/apparent/timing.html
+-rwxr-xr-x   0        0        0     1046 2023-08-02 21:09:10.812796 apparent-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 21:32:41.925459 apparent-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      669 2023-08-02 20:45:54.246950 apparent-0.1.3/tests/common.py
+-rw-r--r--   0        0        0     3418 2023-08-02 21:01:48.115843 apparent-0.1.3/tests/timer_reports_tests.py
+-rw-r--r--   0        0        0     3751 2023-07-07 22:04:36.624455 apparent-0.1.3/tests/timer_results_tests.py
+-rw-r--r--   0        0        0     5519 2023-08-02 20:45:54.247469 apparent-0.1.3/tests/timer_tests.py
+-rw-r--r--   0        0        0     1613 2023-07-12 17:32:41.188742 apparent-0.1.3/tests/variance_tests.py
+-rw-r--r--   0        0        0     5833 1970-01-01 00:00:00.000000 apparent-0.1.3/PKG-INFO
```

### Comparing `apparent-0.1.2/.gitignore` & `apparent-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `apparent-0.1.2/LICENSE.txt` & `apparent-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apparent-0.1.2/README.md` & `apparent-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 Needed something simpler than some of the giant tools and frameworks, which I can use on my desktop
 Without subscribing to some observability service.
 
 This library is not intended to replace or compete with observability tools and dashboard, but is intended 
 for day to day development use with a longer term objective of easy connectivity to observability 
 Tools and frameworks. It is intended to remain small and compact.
 
+## Installation
+
+`python -m pip install apparent`
+
 ## Collect timing information
 
 The most common use and the first to release as OSS is the timers functionality. There are many tools out there that do
 Broadly similar things. In particular, two categories of tools are similar in some ways:
 
 * Profilers (for example [yappi](https://github.com/sumerc/yappi))
 * Micro-benchmarking tools of various kinds
```

### Comparing `apparent-0.1.2/apparent/.DS_Store` & `apparent-0.1.3/apparent/.DS_Store`

 * *Files identical despite different names*

### Comparing `apparent-0.1.2/apparent/timing.py` & `apparent-0.1.3/apparent/timing.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """The main module for explicit timing measurement support. See @timed"""
 import math
 from contextlib import AbstractContextManager
 from dataclasses import asdict, dataclass
 from enum import Enum
 from functools import wraps
 from time import perf_counter
-from typing import Protocol, Type, Union
+from typing import Protocol, TypeVar
 
 
 class Units(Enum):
     MIN = 'min'
     SEC = 'sec'
     MSEC = 'msec'
 
@@ -89,20 +89,20 @@
         self._ex2 += (x - self._k) ** 2
 
     def mean(self) -> float:
         """Return the mean of the added values"""
         return self._k + self._ex / self._n
 
     def variance(self, population: bool = False) -> float:
-        """Computes the variance of the added values. By default uses sample variance. Can be population variance"""
+        """Computes the variance of the added values. By default, uses sample variance. Can be population variance"""
         return (self._ex2 - self._ex ** 2 / self._n) / (self._n if population else self._n - 1)
 
     def stdev(self) -> float:
         """Computes the standard deviation of the added values.
-        By default uses sample variance. Can be population variance"""
+        By default, uses sample variance. Can be population variance"""
         return math.sqrt(self.variance())
 
     def stdevp(self) -> float:
         """Computes the population standard deviation of the added values. """
         return math.sqrt(self.variance(population=True))
 
     @property
@@ -157,15 +157,15 @@
 
     @property
     def max(self) -> float:
         """Maximum of all observations. NaN if no observations have been recorded"""
         return self._max if self.counter > 0 else math.nan
 
     def results(self, units=Units.SEC) -> TimerResults:
-        """TimerResults object packaging the summary of currrent observations."""
+        """TimerResults object packaging the summary of current observations."""
         result = TimerResults(count=self.counter, total_time=self.sum,
                               mean=self.mean, stdevp=self.stdevp,
                               min=self.min, max=self.max,
                               timer_name=self.name)
         return result if units == Units.SEC else result.convert(units)
 
 
@@ -190,56 +190,60 @@
     def names(cls) -> list[str]:
         """Lists all the timer names in the registry.
         Since it is expected that the number of timers will be limited and the whole
         package is not intended for very high scale we return a concrete list rather than an iterator"""
         return list(cls._shared.keys())
 
     @classmethod
-    def timers(cls):
+    def timers(cls) -> list[Timer]:
         """Lists all the timers in the registry.
         Since it is expected that the number of timers will be limited and the whole
         package is not intended for very high scale we return a concrete list rather than an iterator"""
         return list(cls._shared.values())
 
     @classmethod
     def reset(cls, name: str):
         """Resets / deletes a named timer."""
         if name in cls._shared:
             del cls._shared[name]
 
 
-class TimerRegistryType(Protocol):
+class TimerRegistryProtocol(Protocol):
     """For users who want to use some other implementation of a timer registry or want to
     use several timer registries for different contexts."""
     def get(self, name: str) -> Timer:
         ...
 
     def clear(self):
         ...
 
-    def names(self):
+    def names(self) -> list[str]:
         ...
 
-    def timers(self):
+    def timers(self) -> list[Timer]:
         ...
 
     def reset(self, name: str):
         ...
 
 
+TimerRegistryType = TypeVar('TimerRegistryType', TimerRegistryProtocol, TimerRegistry)
+"""Any acceptable type for a timer registry."""
+
+
 class Timed:
     """A simple class to associate a timer registry with the timed decorator. Rarely used."""
-    _registry: Union[TimerRegistryType, Type[TimerRegistry]] = TimerRegistry
+    _registry: TimerRegistryType = TimerRegistry
 
     @classmethod
-    def registry(cls) -> Union[TimerRegistryType, Type[TimerRegistry]]:
+    def registry(cls) -> TimerRegistryType:
         return cls._registry
 
     @classmethod
-    def set_registry(cls, registry: Union[TimerRegistryType, Type[TimerRegistry]]):
+    def set_registry(cls, registry: TimerRegistryType):
         cls._registry = registry
 
 
 def timed(f):
     """A decorator for timing a function.
     The decorated function will be called with a timer context manager to
     record the time spent in the decorated function.
```

### Comparing `apparent-0.1.2/doc/K.svg` & `apparent-0.1.3/doc/K.svg`

 * *Files identical despite different names*

### Comparing `apparent-0.1.2/doc/diffs.svg` & `apparent-0.1.3/doc/diffs.svg`

 * *Files identical despite different names*

### Comparing `apparent-0.1.2/doc/variance.md` & `apparent-0.1.3/doc/variance.md`

 * *Files identical despite different names*

### Comparing `apparent-0.1.2/doc/variance.svg` & `apparent-0.1.3/doc/variance.svg`

 * *Files identical despite different names*

### Comparing `apparent-0.1.2/doc/variance_calc.svg` & `apparent-0.1.3/doc/variance_calc.svg`

 * *Files identical despite different names*

### Comparing `apparent-0.1.2/pyproject.toml` & `apparent-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apparent"
-version = "0.1.2"
+version = "0.1.3"
 description = "A toolkit for code observability in-process data collection: timing, counters, and metrics."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE.txt"}
 keywords = ["apparent", "observability", "monitoring", "timers", "timing", "counters", "metrics"]
 authors = [{name = "Arnon Moscona", email = "arnon@moscona.com"}]
 maintainers = [{name = "Arnon Moscona", email = "arnon@moscona.com"}]
@@ -24,11 +24,14 @@
 [tool.setuptools]
 packages = ["apparent"]
 
 [project.optional-dependencies]
 test = [
     "coverage"
 ]
+dev = [
+    "pdoc"
+]
 
 [tool.flit.sdist]
 include = ["doc/", "apparent/", "bin/", "LICENSE.txt"]
 exclude = ["draft/", ".idea", ".coverage", ".python-version", "todos.md"]
```

### Comparing `apparent-0.1.2/tests/timer_results_tests.py` & `apparent-0.1.3/tests/timer_results_tests.py`

 * *Files identical despite different names*

### Comparing `apparent-0.1.2/tests/timer_tests.py` & `apparent-0.1.3/tests/timer_tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #  Copyright (c) Arnon Moscona 2023. under Apache2 license
 from unittest import TestCase
 from unittest.mock import patch
 
 from apparent.timing import Timed, Timer, TimerRegistry, Units, timed
+from tests.common import CustomTimerRegistry
 
 
 @patch('apparent.timing.perf_counter')
 class TimerTests(TestCase):
     def setUp(self) -> None:
         TimerRegistry.clear()
 
@@ -125,38 +126,14 @@
         self.counter = 0
 
     @timed
     def invoke(self):
         self.counter += 1
 
 
-class CustomTimerRegistry:
-    """Used to test @timed using someting other than the default registry"""
-    def __init__(self):
-        self.reg: dict[str, Timer] = {}
-
-    def get(self, name: str) -> Timer:
-        if name not in self.reg:
-            self.reg[name] = Timer(name)
-        return self.reg[name]
-
-    def clear(self):
-        self.reg.clear()
-
-    def names(self):
-        return list(self.reg.keys())
-
-    def timers(self):
-        return list(self.reg.values())
-
-    def reset(self, name: str):
-        if name in self.reg:
-            del self.reg[name]
-
-
 class TimedTests(TestCase):
     def setUp(self) -> None:
         Timed.set_registry(TimerRegistry)
         Timed.registry().clear()
 
     def test_timed_basic_use_case(self):
```

### Comparing `apparent-0.1.2/tests/variance_tests.py` & `apparent-0.1.3/tests/variance_tests.py`

 * *Files identical despite different names*

### Comparing `apparent-0.1.2/PKG-INFO` & `apparent-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: apparent
-Version: 0.1.2
+Version: 0.1.3
 Summary: A toolkit for code observability in-process data collection: timing, counters, and metrics.
 Keywords: apparent,observability,monitoring,timers,timing,counters,metrics
 Author-email: Arnon Moscona <arnon@moscona.com>
 Maintainer-email: Arnon Moscona <arnon@moscona.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Dist: pdoc ; extra == "dev"
 Requires-Dist: coverage ; extra == "test"
 Project-URL: repository, https://github.com/arnonmoscona/apparent
+Provides-Extra: dev
 Provides-Extra: test
 
 # Apparent: a small library for observability
 
 I created this library because in every job I've had I had to create some version of it, and I generally
 Needed something simpler than some of the giant tools and frameworks, which I can use on my desktop
 Without subscribing to some observability service.
 
 This library is not intended to replace or compete with observability tools and dashboard, but is intended 
 for day to day development use with a longer term objective of easy connectivity to observability 
 Tools and frameworks. It is intended to remain small and compact.
 
+## Installation
+
+`python -m pip install apparent`
+
 ## Collect timing information
 
 The most common use and the first to release as OSS is the timers functionality. There are many tools out there that do
 Broadly similar things. In particular, two categories of tools are similar in some ways:
 
 * Profilers (for example [yappi](https://github.com/sumerc/yappi))
 * Micro-benchmarking tools of various kinds
```

