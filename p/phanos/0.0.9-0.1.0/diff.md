# Comparing `tmp/phanos-0.0.9.tar.gz` & `tmp/phanos-0.1.0.tar.gz`

## Comparing `phanos-0.0.9.tar` & `phanos-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.9/CHANGELOG.md
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.9/Pipfile
--rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.9/Pipfile.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 phanos-0.0.9/requirements.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/Activate.ps1
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/activate
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/activate.csh
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/activate.fish
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/pip
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/pip3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/pip3.10
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/pip3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/python -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/python3 -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.9/deactivate/bin/python3.11 -> /usr/bin/python3.11
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 phanos-0.0.9/src/phanos/__init__.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.0.9/src/phanos/log.py
--rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 phanos-0.0.9/src/phanos/metrics.py
--rw-r--r--   0        0        0    17201 2020-02-02 00:00:00.000000 phanos-0.0.9/src/phanos/publisher.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 phanos-0.0.9/src/phanos/tree.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 phanos-0.0.9/test/__init__.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 phanos-0.0.9/test/dummy_api.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.9/test/requirements.txt
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.9/test/run_tests.py
--rw-r--r--   0        0        0    20704 2020-02-02 00:00:00.000000 phanos-0.0.9/test/test_metric.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.9/test/testing_data.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.9/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.9/LICENSE
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 phanos-0.0.9/README.md
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 phanos-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 phanos-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 phanos-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.1.0/Pipfile
+-rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.1.0/Pipfile.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 phanos-0.1.0/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.1.0/deactivate/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.1.0/deactivate/bin/Activate.ps1
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.1.0/deactivate/bin/activate
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.1.0/deactivate/bin/activate.csh
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.1.0/deactivate/bin/activate.fish
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.0/deactivate/bin/pip
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.0/deactivate/bin/pip3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.0/deactivate/bin/pip3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.0/deactivate/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.0/deactivate/bin/python -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.0/deactivate/bin/python3 -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.0/deactivate/bin/python3.11 -> /usr/bin/python3.11
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 phanos-0.1.0/src/phanos/__init__.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 phanos-0.1.0/src/phanos/config.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.1.0/src/phanos/log.py
+-rw-r--r--   0        0        0    17355 2020-02-02 00:00:00.000000 phanos-0.1.0/src/phanos/metrics.py
+-rw-r--r--   0        0        0    20338 2020-02-02 00:00:00.000000 phanos-0.1.0/src/phanos/publisher.py
+-rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 phanos-0.1.0/src/phanos/tree.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 phanos-0.1.0/test/__init__.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 phanos-0.1.0/test/dummy_api.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.1.0/test/requirements.txt
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 phanos-0.1.0/test/run_tests.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 phanos-0.1.0/test/test_config.py
+-rw-r--r--   0        0        0    26021 2020-02-02 00:00:00.000000 phanos-0.1.0/test/test_metric.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 phanos-0.1.0/test/testing_data.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 phanos-0.1.0/README.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 phanos-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 phanos-0.1.0/PKG-INFO
```

### Comparing `phanos-0.0.9/Pipfile.lock` & `phanos-0.1.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `phanos-0.0.9/deactivate/bin/Activate.ps1` & `phanos-0.1.0/deactivate/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `phanos-0.0.9/deactivate/bin/activate` & `phanos-0.1.0/deactivate/bin/activate`

 * *Files identical despite different names*

### Comparing `phanos-0.0.9/deactivate/bin/activate.csh` & `phanos-0.1.0/deactivate/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `phanos-0.0.9/deactivate/bin/activate.fish` & `phanos-0.1.0/deactivate/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `phanos-0.0.9/src/phanos/log.py` & `phanos-0.1.0/src/phanos/log.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.9/src/phanos/metrics.py` & `phanos-0.1.0/src/phanos/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+""" Module with metric types corresponding with Prometheus metrics and custom Time profiling metric """
 from __future__ import annotations
 
 import logging
 import sys
 import typing
 from datetime import datetime as dt
 
 from flask import current_app as app
 from imp_prof import Record
+
 from . import log
 
 
 class MetricWrapper(log.InstanceLoggerMixin):
     """Wrapper around all Prometheus metric types"""
 
     name: str
@@ -24,57 +26,50 @@
     operations: typing.Dict[str, typing.Callable]
     default_operation: str
 
     def __init__(
         self,
         name: str,
         units: str,
+        job: str,
         labels: typing.Optional[typing.List[str]] = None,
-        logger: typing.Optional[logging.Logger] = None,
+        logger: typing.Optional[log.LoggerLike] = None,
     ) -> None:
         """
         Initialize Metric and stores it into publisher instance
 
         Set values that are in Type Record.
 
         :param units: units of measurement
         :param labels: label_names of metric viz. Type Record
         """
         self.name = name
         self.item = []
         self.units = units
         self._values = []
         self.method = []
-        self.job = ""
+        self.job = job
         self.label_names = list(set(labels)) if labels else []
         self._label_values = []
         self.operations = {}
         self.default_operation = ""
-        super().__init__(
-            logged_name="phanos", logger=logger or logging.getLogger(__name__)
-        )
+        super().__init__(logged_name="phanos", logger=logger or logging.getLogger(__name__))
 
     def to_records(self) -> typing.List[Record]:
         """Convert measured values into Type Record
 
         :returns: List of records
         :raises RuntimeError: if one of records would be incomplete
         """
         records = []
-        if not (len(self.method) == len(self._values) == len(self._label_values)):
-            self.error(
-                f"{self.to_records.__qualname__}: one of records missing method || value || label_values"
-            )
-            raise RuntimeError(
-                f"{len(self.method)}, {len(self._values)}, {len(self._label_values)}"
-            )
+        if not len(self.method) == len(self._values) == len(self._label_values):
+            self.error(f"{self.to_records.__qualname__}: one of records missing method || value || label_values")
+            raise RuntimeError(f"{len(self.method)}, {len(self._values)}, {len(self._label_values)}")
         for i in range(len(self._values)):
-            label_value = (
-                self._label_values[i] if self._label_values is not None else {}
-            )
+            label_value = self._label_values[i] if self._label_values is not None else {}
             record: Record = {
                 "item": self.method[i].split(":")[0],
                 "metric": self.metric,
                 "units": self.units,
                 "job": self.job,
                 "method": self.method[i],
                 "labels": label_value,
@@ -118,78 +113,86 @@
         :param method: measured method
         :param value: measured value
         :param label_values: values of labels
         :param args: will be passed to specific operation of given metric
         :param kwargs: will be passed to specific operation of given metric
         :raise ValueError: if operation does not exist for given metric.
         """
-        try:
-            with app.app_context():
-                if self.job == "":
+        if self.job == "":
+            try:
+                with app.app_context():
                     self.job = app.import_name
-        except RuntimeError:
-            pass
+            except RuntimeError:
+                pass
 
         if label_values is None:
             label_values = {}
+
+        labels_ok = self._check_labels(list(label_values.keys()))
+        if labels_ok:
+            self._label_values.append(label_values)
+        else:
+            self.error(
+                f"{self.store_operation.__qualname__}: expected labels: {self.label_names}, "
+                f"labels given: {label_values.keys()}"
+            )
+            raise ValueError("Unknown or missing label")
+        if operation is None:
+            operation = self.default_operation
+        self.method.append(method)
+
         try:
-            labels_ok = self._check_labels(list(label_values.keys()))
-            if labels_ok:
-                self._label_values.append(label_values)
-            else:
-                self.error(
-                    f"{self.store_operation.__qualname__}: expected labels: {self.label_names}, "
-                    f"labels given: {label_values.keys()}"
-                )
-                raise ValueError("Unknown or missing label")
-            if operation is None:
-                operation = self.default_operation
-            self.method.append(method)
             self.operations[operation](value, args, kwargs)
         except KeyError as exc:
             self.error(
                 f"{self.store_operation.__qualname__}: operation {operation} unknown."
                 f"Known operations: {self.operations.keys()}"
             )
             raise ValueError("Unknown operation") from exc
+        if self._values:
+            self.debug("%r stored value %s", self.name, self._values[-1])
 
     def cleanup(self) -> None:
         """Cleanup after all records was sent"""
         if self._values is not None:
             self._values.clear()
         if self._label_values is not None:
             self._label_values.clear()
         if self.method is not None:
             self.method.clear()
         if self.item is not None:
             self.item.clear()
         self.debug("%s: metric %s cleared", self.cleanup.__qualname__, self.name)
 
+    def set_job(self, job):
+        self.job = job
+
 
 class Histogram(MetricWrapper):
     """class representing histogram metric of Prometheus"""
 
     metric: str
 
     def __init__(
         self,
         name: str,
         units: str,
+        job: str = "",
         labels: typing.Optional[typing.List[str]] = None,
-        logger: typing.Optional[logging.Logger] = None,
+        logger: typing.Optional[log.LoggerLike] = None,
     ) -> None:
         """
         Initialize Histogram metric and stores it into publisher instance
 
         Set values that are in Type Record.
 
         :param units: units of measurement
         :param labels: label_names of metric viz. Type Record
         """
-        super().__init__(name, units, labels, logger)
+        super().__init__(name, units, job, labels, logger)
         self.metric = "histogram"
         self.default_operation = "observe"
         self.operations = {"observe": self._observe}
 
     def _observe(self, value: float, *args, **kwargs) -> None:
         """Method representing observe action of Histogram
 
@@ -209,26 +212,27 @@
 
     metric: str
 
     def __init__(
         self,
         name: str,
         units: str,
+        job: str = "",
         labels: typing.Optional[typing.List[str]] = None,
-        logger: typing.Optional[logging.Logger] = None,
+        logger: typing.Optional[log.LoggerLike] = None,
     ) -> None:
         """
         Initialize Summary metric and stores it into publisher instance
 
         Set values that are in Type Record.
 
         :param units: units of measurement
         :param labels: label_names of metric viz. Type Record
         """
-        super().__init__(name, units, labels, logger)
+        super().__init__(name, units, job, labels, logger)
         self.metric = "summary"
         self.default_operation = "observe"
         self.operations = {"observe": self._observe}
 
     def _observe(self, value: float, *args, **kwargs) -> None:
         """Method representing observe action of Summary
 
@@ -248,26 +252,27 @@
 
     metric: str
 
     def __init__(
         self,
         name: str,
         units: str,
+        job: str = "",
         labels: typing.Optional[typing.List[str]] = None,
-        logger: typing.Optional[logging.Logger] = None,
+        logger: typing.Optional[log.LoggerLike] = None,
     ) -> None:
         """
         Initialize Counter metric and stores it into publisher instance
 
         Set values that are in Type Record.
 
         :param units: units of measurement
         :param labels: label_names of metric viz. Type Record
         """
-        super().__init__(name, units, labels, logger)
+        super().__init__(name, units, job, labels, logger)
         self.metric = "counter"
         self.default_operation = "inc"
         self.operations = {"inc": self._inc}
 
     def _inc(self, value: float, *args, **kwargs) -> None:
         """Method representing inc action of counter
 
@@ -287,35 +292,34 @@
 
     metric: str
 
     def __init__(
         self,
         name: str,
         units: typing.Optional[str] = None,
+        job: str = "",
         labels: typing.Optional[typing.List[str]] = None,
-        logger: typing.Optional[logging.Logger] = None,
+        logger: typing.Optional[log.LoggerLike] = None,
     ) -> None:
         """
         Initialize Info metric and stores it into publisher instance
 
         Set values that are in Type Record.
 
         :param units: units of measurement
         :param labels: label_names of metric viz. Type Record
         """
         if units is None:
             units = "info"
-        super().__init__(name, units, labels, logger)
+        super().__init__(name, units, job, labels, logger)
         self.metric = "info"
         self.default_operation = "info"
         self.operations = {"info": self._info}
 
-    def _info(
-        self, value: typing.Dict[typing.Any, typing.Any], *args, **kwargs
-    ) -> None:
+    def _info(self, value: typing.Dict[typing.Any, typing.Any], *args, **kwargs) -> None:
         """Method representing info action of info
 
         :param value: measured value
         :raises ValueError: if value is not dictionary
         """
         _ = args
         _ = kwargs
@@ -330,26 +334,27 @@
 
     metric: str
 
     def __init__(
         self,
         name: str,
         units: str,
+        job: str = "",
         labels: typing.Optional[typing.List[str]] = None,
-        logger: typing.Optional[logging.Logger] = None,
+        logger: typing.Optional[log.LoggerLike] = None,
     ) -> None:
         """
         Initialize Gauge metric and stores it into publisher instance
 
         Set values that are in Type Record.
 
         :param units: units of measurement
         :param labels: label_names of metric viz. Type Record
         """
-        super().__init__(name, units, labels, logger)
+        super().__init__(name, units, job, labels, logger)
         self.metric = "gauge"
         self.default_operation = "inc"
         self.operations = {
             "inc": self._inc,
             "dec": self._dec,
             "set": self._set,
         }
@@ -401,29 +406,30 @@
     states: typing.List[str]
 
     def __init__(
         self,
         name: str,
         states: typing.List[str],
         units: typing.Optional[str] = None,
+        job: str = "",
         labels: typing.Optional[typing.List[str]] = None,
-        logger: typing.Optional[logging.Logger] = None,
+        logger: typing.Optional[log.LoggerLike] = None,
     ) -> None:
         """
         Initialize Enum metric and stores it into publisher instance
 
         Set values that are in Type Record
 
         :param units: units of measurement
         :param states: states which can enum have
         :param labels: label_names of metric viz. Type Record
         """
         if units is None:
             units = "enum"
-        super().__init__(name, units, labels, logger)
+        super().__init__(name, units, job, labels, logger)
         self.metric = "enum"
         self.default_operation = "state"
         self.states = states
         self.operations = {"state": self._state}
 
     def _state(self, value: str, *args, **kwargs) -> None:
         """Method representing state action of enum
@@ -439,33 +445,34 @@
                 f"Allowed values: {self.states!r}"
             )
             raise ValueError("Invalid state for Enum metric")
         self._values.append(("state", value))
 
 
 class TimeProfiler(Histogram):
-    """class for measuring multiple time records in one endpoint.
-     Used for measuring time consuming operations
+    """Class for measuring multiple time records in one endpoint.
+    Used for measuring time-consuming operations
 
     measured unit is milliseconds
     """
 
     _start_ts: typing.List[dt]
 
     def __init__(
         self,
         name: str,
+        job: str = "",
         labels: typing.Optional[typing.List[str]] = None,
-        logger: typing.Optional[logging.Logger] = None,
+        logger: typing.Optional[log.LoggerLike] = None,
     ) -> None:
         """
         :param labels: label_names of metric viz. Type Record
         :raises RuntimeError: if start timestamps < number of stop measurement operation
         """
-        super().__init__(name, "mS", labels, logger)
+        super().__init__(name, "mS", job, labels, logger)
         self.operations = {"stop": self._stop}
         self.default_operation = "stop"
         self._start_ts = []
         self.debug("TimeProfiler metric initialized")
 
     # ############################### measurement operations -> checking labels, not sending records
     def _stop(self, *args, **kwargs) -> None:
@@ -474,20 +481,16 @@
         _ = kwargs
         try:
             method_time = dt.now() - self._start_ts.pop(-1)
             self._observe(
                 method_time.total_seconds() * 1000.0,
             )
         except IndexError:
-            self.error(
-                f"{self._stop.__qualname__}: Cannot record operation. No start ts exists."
-            )
-            raise RuntimeError(
-                "Number of start timestamps < number of stop measurement operations"
-            )
+            self.error(f"{self._stop.__qualname__}: Cannot record operation. No start ts exists.")
+            raise RuntimeError("Number of start timestamps < number of stop measurement operations")
 
     # ############################### helper operations -> not checking labels, not checking records
     def start(self, *args, **kwargs) -> None:
         """Starts time measurement - stores dt.now()"""
         _ = args
         _ = kwargs
         self._start_ts.append(dt.now())
@@ -503,21 +506,22 @@
 
     measured in bytes
     """
 
     def __init__(
         self,
         name: str,
+        job: str = "",
         labels: typing.Optional[typing.List[str]] = None,
-        logger: typing.Optional[logging.Logger] = None,
+        logger: typing.Optional[log.LoggerLike] = None,
     ) -> None:
         """
         :param labels: label_names of metric viz. Type Record
         """
-        super().__init__(name, "B", labels, logger)
+        super().__init__(name, "B", job, labels, logger)
         self.operations = {"rec": self._rec}
         self.default_operation = "rec"
         self.debug("ResponseSize metric initialized")
 
     def _rec(self, value: str, *args, **kwargs) -> None:
         """records size of response"""
         _ = args
```

### Comparing `phanos-0.0.9/src/phanos/publisher.py` & `phanos-0.1.0/src/phanos/publisher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """ """
 from __future__ import annotations
+import inspect
 import logging
 import sys
 import threading
 import typing
 from abc import abstractmethod
-from logging import Logger
 
 import imp_prof.messaging.publisher
-
 from imp_prof.messaging.publisher import BlockingPublisher
-
 from .metrics import MetricWrapper, TimeProfiler, ResponseSize
 from .tree import MethodTreeNode
 from . import log
 
 TIME_PROFILER = "time_profiler"
 RESPONSE_SIZE = "response_size"
 
@@ -27,72 +25,70 @@
         """converts Record type into profiling string
 
         :param name: name of profiler
         :param record: metric record which to convert
         """
         value = record["value"][1]
         if not record.get("labels"):
-            return (
-                f"profiler: {name}, "
-                f"method: {record.get('method')}, "
-                f"value: {value} {record.get('units')}"
-            )
+            return f"profiler: {name}, " f"method: {record.get('method')}, " f"value: {value} {record.get('units')}"
         # format labels as this "key=value, key2=value2"
         labels = ", ".join(f"{k}={v}" for k, v in record["labels"].items())
         return (
             f"profiler: {name}, "
             f"method: {record.get('method')}, "
             f"value: {value} {record.get('units')}, "
             f"labels: {labels}"
         )
 
 
 class BaseHandler:
-    """ " base class for record handling"""
+    """base class for record handling"""
 
     handler_name: str
 
     def __init__(self, handler_name: str) -> None:
         """
         :param handler_name: name of handler. used for managing handlers"""
         self.handler_name = handler_name
 
     @abstractmethod
     def handle(
-        self, records: typing.List[imp_prof.Record], profiler_name: str = "profiler"
+        self,
+        records: typing.List[imp_prof.Record],
+        profiler_name: str = "profiler",
     ) -> None:
         """
         method for handling records
 
         :param profiler_name: name of profiler
         :param records: list of records to handle
         """
         raise NotImplementedError
 
 
 class ImpProfHandler(BaseHandler):
     """RabbitMQ record handler"""
 
-    _publisher: BlockingPublisher
-    _logger: logging.Logger
+    publisher: BlockingPublisher
+    logger: typing.Optional[log.LoggerLike]
 
     def __init__(
         self,
         handler_name: str,
         host: str = "127.0.0.1",
         port: int = 5672,
         user: typing.Optional[str] = None,
         password: typing.Optional[str] = None,
         heartbeat: int = 47,
         timeout: float = 23,
         retry_delay: float = 0.137,
         retry: int = 3,
         exchange_name: str = "profiling",
         exchange_type: str = "fanout",
-        logger: typing.Optional[Logger] = None,
+        logger: typing.Optional[log.LoggerLike] = None,
         **kwargs,
     ) -> None:
         """Creates BlockingPublisher instance (connection not established yet),
          sets logger and create time profiler and response size profiler
 
         :param handler_name: name of handler. used for managing handlers
         :param host: rabbitMQ server host
@@ -113,388 +109,449 @@
             e.g., on_close_callback or ConnectionClosed exception) with
             `reason_code` of `InternalCloseReasons.BLOCKED_CONNECTION_TIMEOUT`.
         :param kwargs: other connection params, like `timeout goes here`
         :param logger: logger
         """
         super().__init__(handler_name)
 
-        self._logger = logger or logging.getLogger(__name__)
-        self._publisher = BlockingPublisher(
+        self.logger = logger or logging.getLogger(__name__)
+        self.publisher = BlockingPublisher(
             host=host,
             port=port,
             user=user,
             password=password,
             heartbeat=heartbeat,
             timeout=timeout,
             retry_delay=retry_delay,
             retry=retry,
             exchange_name=exchange_name,
             exchange_type=exchange_type,
             logger=logger,
             **kwargs,
         )
         try:
-            self._publisher.connect()
+            self.publisher.connect()
         except imp_prof.messaging.publisher.NETWORK_ERRORS as err:
-            self._logger.error(
-                f"ImpProfHandler cannot connect to RabbitMQ because of {err}"
-            )
+            self.logger.error(f"ImpProfHandler cannot connect to RabbitMQ because of {err}")
             raise RuntimeError("Cannot connect to RabbitMQ") from err
 
-        self._logger.info("ImpProfHandler created successfully")
-        self._publisher.close()
+        self.logger.info("ImpProfHandler created successfully")
+        self.publisher.close()
 
     def handle(
         self,
         records: typing.List[imp_prof.Record],
         profiler_name: str = "profiler",
     ) -> None:
         """Sends list of records to rabitMq queue
 
         :param profiler_name: name of profiler (not used)
         :param records: list of records to publish
         """
 
         _ = profiler_name
         for record in records:
-            _ = self._publisher.publish(record)
+            _ = self.publisher.publish(record)
 
 
 class LoggerHandler(BaseHandler):
     """logger handler"""
 
-    _logger: logging.Logger
-    _formatter: OutputFormatter
+    logger: log.LoggerLike
+    formatter: OutputFormatter
     level: int
 
     def __init__(
         self,
         handler_name: str,
-        logger: typing.Optional[logging.Logger] = None,
+        logger: typing.Optional[log.LoggerLike] = None,
         level: int = 10,
     ) -> None:
         """
 
         :param handler_name: name of handler. used for managing handlers
         :param logger: logger instance if none -> creates new with name PHANOS
         :param level: level of logger in which prints records. default is DEBUG
         """
         super().__init__(handler_name)
         if logger is not None:
-            self._logger = logger
+            self.logger = logger
         else:
-            self._logger = logging.getLogger("PHANOS")
-            self._logger.setLevel(10)
+            self.logger = logging.getLogger("PHANOS")
+            self.logger.setLevel(10)
             handler = logging.StreamHandler(sys.stdout)
             handler.setLevel(10)
-            self._logger.addHandler(handler)
+            self.logger.addHandler(handler)
         self.level = level
-        self._formatter = OutputFormatter()
+        self.formatter = OutputFormatter()
 
-    def handle(
-        self, records: typing.List[imp_prof.Record], profiler_name: str = "profiler"
-    ) -> None:
+    def handle(self, records: typing.List[imp_prof.Record], profiler_name: str = "profiler") -> None:
         """logs list of records
 
         :param profiler_name: name of profiler
         :param records: list of records
         """
         for record in records:
-            self._logger.log(
-                self.level, self._formatter.record_to_str(profiler_name, record)
-            )
+            self.logger.log(self.level, self.formatter.record_to_str(profiler_name, record))
 
 
 class StreamHandler(BaseHandler):
     """Stream handler of Records."""
 
-    _formatter: OutputFormatter
+    formatter: OutputFormatter
     output: typing.TextIO
     _lock: threading.Lock
 
     def __init__(self, handler_name: str, output: typing.TextIO = sys.stdout) -> None:
         """
 
         :param handler_name: name of profiler
         :param output: stream output. Default 'sys.stdout'
         """
         super().__init__(handler_name)
         self.output = output
-        self._formatter = OutputFormatter()
+        self.formatter = OutputFormatter()
         self._lock = threading.Lock()
 
-    def handle(
-        self, records: typing.List[imp_prof.Record], profiler_name: str = "profiler"
-    ) -> None:
+    def handle(self, records: typing.List[imp_prof.Record], profiler_name: str = "profiler") -> None:
         """logs list of records
 
         :param profiler_name: name of profiler
         :param records: list of records
         """
         for record in records:
             with self._lock:
                 print(
-                    self._formatter.record_to_str(profiler_name, record),
+                    self.formatter.record_to_str(profiler_name, record),
                     file=self.output,
                     flush=True,
                 )
 
 
 class PhanosProfiler(log.InstanceLoggerMixin):
     """Class responsible for sending records to IMP_prof RabbitMQ publish queue"""
 
-    _metrics: typing.Dict[str, MetricWrapper]
+    metrics: typing.Dict[str, MetricWrapper]
 
     _root: MethodTreeNode
     current_node: MethodTreeNode
 
     time_profile: typing.Optional[TimeProfiler]
     resp_size_profile: typing.Optional[ResponseSize]
 
     before_func: typing.Optional[typing.Callable]
     after_func: typing.Optional[typing.Callable]
     before_root_func: typing.Optional[typing.Callable]
     after_root_func: typing.Optional[typing.Callable]
 
-    _handlers: typing.Dict[str, BaseHandler]
+    handlers: typing.Dict[str, BaseHandler]
     handle_records: bool
+    job: str
+    error_occurred: bool
 
     def __init__(self) -> None:
         """Initialize ProfilesPublisher
 
         Initialization just creates new instance!!
 
         """
 
-        self._metrics = {}
-        self._handlers = {}
+        self.metrics = {}
+        self.handlers = {}
+        self.job = ""
+        self.error_occurred = False
 
-        self.request_size_profile = None
+        self.resp_size_profile = None
         self.time_profile = None
 
         self.before_func = None
         self.after_func = None
         self.before_root_func = None
         self.after_root_func = None
         super().__init__(logged_name="phanos")
 
     def config(
         self,
         logger=None,
+        job: str = "",
         time_profile: bool = True,
-        request_size_profile: bool = True,
+        request_size_profile: bool = False,
         handle_records: bool = True,
     ) -> None:
         """configure PhanosProfiler
+        :param job: name of job
         :param logger: logger instance
         :param time_profile: should create instance time profiler
         :param request_size_profile: should create instance of request size profiler
         :param handle_records: should handle recorded records
         """
         self.logger = logger or logging.getLogger(__name__)
+        self.job = job
         if time_profile:
             self.create_time_profiler()
         if request_size_profile:
             self.create_response_size_profiler()
         self.handle_records = handle_records
 
         self._root = MethodTreeNode(None, self.logger)
         self.current_node = self._root
 
+    def dict_config(self, settings: dict[str, typing.Any]) -> None:
+        """
+        Configure profiler instance with dictionary config.
+        Set up profiling from config file, instead fo changing code for various environments.
+
+        Example:
+            ```
+            {
+                "job": "my_app",
+                "logger": "my_app_debug_logger",
+                "time_profile": True,
+                "handle_records": True,
+                "handlers": {
+                    "stdout_handler": {
+                        "class": "phanos.publisher.StreamHandler",
+                        "handler_name": "stdout_handler",
+                        "output": "ext://sys.stdout",
+                    }
+                }
+            }
+            ```
+
+        :param settings: dictionary of desired profiling set up
+        """
+        from . import config as phanos_config
+
+        if "logger" in settings:
+            self.logger = logging.getLogger(settings["logger"])
+        if "job" in settings:
+            self.job = settings["job"]
+        if settings.get("time_profile"):
+            self.create_time_profiler()
+        self.handle_records = settings.get("handle_records", True)
+        if "handlers" in settings:
+            named_handlers = phanos_config.create_handlers(settings["handlers"])
+            for handler in named_handlers.values():
+                self.add_handler(handler)
+
     def create_time_profiler(self) -> None:
         """Create time profiling metric"""
-        self.time_profile = TimeProfiler(TIME_PROFILER, logger=self.logger)
+        self.time_profile = TimeProfiler(TIME_PROFILER, job=self.job, logger=self.logger)
         self.add_metric(self.time_profile)
         self.debug("Phanos - time profiler created")
 
     def create_response_size_profiler(self) -> None:
         """create response size profiling metric"""
-        self.resp_size_profile = ResponseSize(RESPONSE_SIZE, logger=self.logger)
+        self.resp_size_profile = ResponseSize(RESPONSE_SIZE, job=self.job, logger=self.logger)
         self.add_metric(self.resp_size_profile)
         self.debug("Phanos - response size profiler created")
 
     def delete_metric(self, item: str) -> None:
         """deletes one metric instance
         :param item: name of the metric instance
         :raises KeyError: if metric does not exist
         """
         try:
-            _ = self._metrics.pop(item)
+            _ = self.metrics.pop(item)
         except KeyError:
             self.error(f"{self.delete_metric.__qualname__}: metric {item} do not exist")
             raise KeyError(f"metric {item} do not exist")
 
         if item == "time_profiler":
             self.time_profile = None
         if item == "response_size":
             self.resp_size_profile = None
         self.debug(f"metric {item} deleted")
 
-    def delete_metrics(
-        self, rm_time_profile: bool = False, rm_resp_size_profile: bool = False
-    ) -> None:
+    def delete_metrics(self, rm_time_profile: bool = False, rm_resp_size_profile: bool = False) -> None:
         """deletes all custom metric instances
 
         :param rm_time_profile: should pre created time_profiler be deleted
         :param rm_resp_size_profile: should pre created response_size_profiler be deleted
         """
-        names = list(self._metrics.keys())
+        names = list(self.metrics.keys())
         for name in names:
-            if (name != TIME_PROFILER or rm_time_profile) and (
-                name != RESPONSE_SIZE or rm_resp_size_profile
-            ):
+            if (name != TIME_PROFILER or rm_time_profile) and (name != RESPONSE_SIZE or rm_resp_size_profile):
                 self.delete_metric(name)
 
     def clear(self):
         """clear all records from all metrics and clear method tree"""
-        for metric in self._metrics.values():
+        for metric in self.metrics.values():
             metric.cleanup()
 
         self.current_node = self._root
         self._root.clear_tree()
 
     def add_metric(self, metric: MetricWrapper) -> None:
         """adds new metric to profiling
 
         :param metric: metric instance
         """
-        if self._metrics.get(metric.name, None):
-            self.warning(
-                f"Metric {metric.name} already exist. Overwriting with new metric"
-            )
-        self._metrics[metric.name] = metric
+        if self.metrics.get(metric.name, None):
+            self.warning(f"Metric {metric.name} already exist. Overwriting with new metric")
+        self.metrics[metric.name] = metric
         self.debug(f"Metric {metric.name} added to phanos profiler")
 
     def add_handler(self, handler: BaseHandler) -> None:
         """Add handler to profiler
 
         :param handler: handler instance
         """
-        if self._handlers.get(handler.handler_name, None):
-            self.warning(
-                f"Handler {handler.handler_name} already exist. Overwriting with new handler"
-            )
-        self._handlers[handler.handler_name] = handler
+        if self.handlers.get(handler.handler_name, None):
+            self.warning(f"Handler {handler.handler_name} already exist. Overwriting with new handler")
+        self.handlers[handler.handler_name] = handler
         self.debug(f"Handler {handler.handler_name} added to phanos profiler")
 
     def delete_handler(self, handler_name: str) -> None:
         """Delete handler from profiler
 
         :param handler_name: name of handler:
         :raises KeyError: if handler do not exist
         """
         try:
-            _ = self._handlers.pop(handler_name)
+            _ = self.handlers.pop(handler_name)
         except KeyError:
-            self.error(
-                f"{self.delete_handler.__qualname__}: handler {handler_name} do not exist"
-            )
+            self.error(f"{self.delete_handler.__qualname__}: handler {handler_name} do not exist")
             raise KeyError(f"handler {handler_name} do not exist")
         self.debug(f"handler {handler_name} deleted")
 
     def delete_handlers(self) -> None:
         """delete all handlers"""
-        self._handlers.clear()
-        self.debug(f"all handlers deleted")
+        self.handlers.clear()
+        self.debug("all handlers deleted")
 
     def profile(self, func: typing.Callable) -> typing.Callable:
         """
         Decorator specifying which methods should be profiled.
         Default profiler is time profiler which measures execution time of decorated methods
 
         Usage: decorate methods which you want to be profiled
 
         :param func: method or function which should be profiled
         """
 
-        def inner(*args, **kwargs) -> typing.Any:
-            if self._handlers and self.handle_records:
-                self.current_node = self.current_node.add_child(
-                    MethodTreeNode(func, self.logger)
-                )
+        def before_function_handling(args, kwargs):
+            """Handlers profiling before profiled function execution (records start time)
+
+            Saves method context into MethodTreeNode, calls _before_root_func, _before_func
+            """
+            if self.handlers and self.handle_records:
+                if self.current_node == self._root:
+                    self.error_occurred = False
+                self.current_node = self.current_node.add_child(MethodTreeNode(func, self.logger))
 
                 if self.current_node.parent == self._root:
-                    self.debug("before root execution")
-                    self._before_root_func(*args, **kwargs)
-                self.debug("before func execution")
-                self._before_func(*args, **kwargs)
-
-            result = func(*args, **kwargs)
-
-            if self._handlers and self.handle_records:
-                self.debug("after func execution")
-                self._after_func(*args, **kwargs)
+                    self._before_root_func(func, args, kwargs)
+                self._before_func(func, args, kwargs)
+
+        def after_function_handling(result, args, kwargs):
+            """Handles profiling after profiled function execution (records stop time)
+
+            Deletes method context from MethodTreeNode, calls _after_root_func, _after_func and handle records
+            if root function was executed
+            """
+            if self.handlers and self.handle_records:
+                self._after_func(result, args, kwargs)
 
                 if self.current_node.parent == self._root:
-                    self.debug("after root execution")
-                    self._after_root_func(*args, **kwargs)
-                    self._handle_records_clear()
+                    self._after_root_func(result, args, kwargs)
+                    self.handle_records_clear()
+                if self.current_node.parent and not self.error_occurred:
+                    self.current_node = self.current_node.parent
+                    self.current_node.delete_child()
+                elif not self.error_occurred:
+                    self.error(f"{self.profile.__qualname__}: node {self.current_node.context!r} have no parent.")
+                    raise ValueError(f"{self.current_node.context!r} have no parent")
+
+        async def async_inner(*args, **kwargs) -> typing.Any:
+            """async decorator version"""
+            before_function_handling(args, kwargs)
+            try:
+                result = await func(*args, **kwargs)
+            except Exception as e:
+                # in case of exception handle measured records, cleanup and reraise
+                self.force_handle_records_clear()
+                self.error_occurred = True
+                raise e
+            after_function_handling(result, args, kwargs)
+            return result
 
-                self.current_node = self.current_node.parent
-                self.current_node.delete_child()
+        def sync_inner(*args, **kwargs) -> typing.Any:
+            """sync decorator version"""
+            before_function_handling(args, kwargs)
+            try:
+                result = func(*args, **kwargs)
+            except Exception as e:
+                # in case of exception handle measured records, cleanup and reraise
+                self.force_handle_records_clear()
+                self.error_occurred = True
+                raise e
+            after_function_handling(result, args, kwargs)
             return result
 
-        return inner
+        if inspect.iscoroutinefunction(func):
+            return async_inner
+        return sync_inner
 
-    def _before_root_func(self, function: typing.Callable, *args, **kwargs) -> None:
+    def _before_root_func(self, func, args, kwargs) -> None:
         """method executing before root function
 
-        :param function: root function
+        :param func: root function
         """
         # users custom metrics operation recording
         if callable(self.before_root_func):
-            self.before_root_func(function=function, *args, **kwargs)
+            self.before_root_func(func, args, kwargs)
         # place for phanos metrics if needed
 
-    def _after_root_func(self, fn_result: typing.Any, *args, **kwargs) -> None:
+    def _after_root_func(self, fn_result: typing.Any, args, kwargs) -> None:
         """method executing after the root function
 
 
         :param fn_result: result of function
         """
         # phanos metrics
         if self.resp_size_profile:
             self.resp_size_profile.store_operation(
-                operation="rec",
-                method=self.current_node.context,
-                value=fn_result,
-                label_values={},
+                method=self.current_node.context, operation="rec", value=fn_result, label_values={}
             )
         # users custom metrics operation recording
         if callable(self.after_root_func):
-            self.after_root_func(fn_result=fn_result, *args, **kwargs)
+            self.after_root_func(fn_result, args, kwargs)
 
-    def _before_func(self, func, *args, **kwargs) -> None:
+    def _before_func(self, func, args, kwargs) -> None:
         # users custom metrics operation recording
         if callable(self.before_func):
-            self.before_func(function=func, *args, **kwargs)
+            self.before_func(func, args, kwargs)
         # phanos metrics
         if self.time_profile:
             self.time_profile.start()
 
-    def _after_func(self, fn_result: typing.Any, *args, **kwargs) -> None:
+    def _after_func(self, fn_result, args, kwargs) -> None:
         # phanos metrics
-        if self.time_profile:
-            self.time_profile.store_operation(
-                operation="stop", method=self.current_node.context, label_values={}
-            )
+        if self.time_profile and not self.error_occurred:
+            self.time_profile.store_operation(method=self.current_node.context, operation="stop", label_values={})
         # users custom metrics operation recording
         if callable(self.after_func):
-            self.after_func(fn_result=fn_result, *args, **kwargs)
+            self.after_func(fn_result, args, kwargs)
 
-    def _handle_records_clear(self) -> None:
-        """Pass records to each registered Handler and clear stored records"""
+    def handle_records_clear(self) -> None:
+        """Pass records to each registered Handler and clear stored records
+        method DO NOT clear MethodContext tree
+        """
         # send records and log em
-        for metric in self._metrics.values():
+        for metric in self.metrics.values():
             records = metric.to_records()
-            for handler in self._handlers.values():
-                self.debug(
-                    f"handler %s handling metric %s", handler.handler_name, metric.name
-                )
+            for handler in self.handlers.values():
+                self.debug(f"handler %s handling metric %s", handler.handler_name, metric.name)
                 handler.handle(records, metric.name)
             metric.cleanup()
 
     def force_handle_records_clear(self) -> None:
-        """Method to force records handling with Method tree clear"""
+        """Method to force records handling
+
+        forces record handling. As side effect clears all metrics and clears MethodContext tree
+        """
         # send records and log em
-        self._handle_records_clear()
+        self.debug("Forcing record handling")
+        self.handle_records_clear()
+        self.current_node = self._root
         self._root.clear_tree()
```

### Comparing `phanos-0.0.9/test/dummy_api.py` & `phanos-0.1.0/test/dummy_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,34 @@
-from abc import abstractmethod
-from functools import partial
+import asyncio
 from time import sleep
 
-
+import flask
 from flask import Flask
 from flask_restx import Api, Resource, Namespace
 
 from src.phanos import phanos_profiler
+from src.phanos.publisher import LoggerHandler
 
 ns = Namespace("dummy")
 
 
 def dummy_method():
     pass
 
 
+@phanos_profiler.profile
+def test_inside_list_comp():
+    return 5
+
+
+@phanos_profiler.profile
+def test_list_comp():
+    _ = [test_inside_list_comp() for i in range(1)]
+
+
 class DummyDbAccess:
     @staticmethod
     def test_static():
         pass
 
     @classmethod
     def test_class(cls):
@@ -36,36 +46,71 @@
     def second_access(self):
         self.first_access()
         sleep(0.3)
 
     def third_access(self):
         self.second_access()
 
+    @phanos_profiler.profile
+    def raise_access(self):
+        self.first_access()
+        raise RuntimeError()
+
+
+class AsyncTest:
+    @staticmethod
+    @phanos_profiler.profile
+    async def async_access_short():
+        await asyncio.sleep(0.1)
+
+    @staticmethod
+    @phanos_profiler.profile
+    async def async_access_long():
+        await asyncio.sleep(0.2)
+
 
 @ns.route("/one")
 class DummyResource(Resource):
     access = DummyDbAccess()
 
     @phanos_profiler.profile
     def get(self):
         self.access.first_access()
         self.access.second_access()
         return {"success": True}, 201
 
+    @phanos_profiler.profile
+    def get_(self):
+        self.access.third_access()
+        return {"success": True}, 201
+
+    # for testing nested api calls
+    @phanos_profiler.profile
+    def post(self):
+        with app.app_context():
+            return app.test_client().delete("/api/dummy/one")
+
+    @phanos_profiler.profile
+    def delete(self):
+        with app.app_context():
+            response = app.test_client().put("/api/dummy/one")
+        return response.json, response.status_code
+
+    @phanos_profiler.profile
+    def put(self):
+        flask.abort(400, "some shit")
+        return {"success", True}, 200
+
 
 app = Flask("TEST")
 api = Api(
     app,
     prefix="/api",
 )
 api.add_namespace(ns)
 
 if __name__ == "__main__":
-    from src.phanos import phanos_profiler
-    from src.phanos.publisher import LoggerHandler
-
     phanos_profiler.config()
     handler = LoggerHandler("asd")
     phanos_profiler.add_handler(handler)
-    print("starting profle")
-    resource = DummyResource()
-    res = resource.get()
+    print("starting profile")
+    _ = test_list_comp()
```

### Comparing `phanos-0.0.9/test/testing_data.py` & `phanos-0.1.0/test/testing_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,17 +40,15 @@
         "job": "TEST",
         "method": "DummyResource:get.first_access",
         "labels": {},
         "value": ("observe", 2.0),
     },
 )
 test_handler_out = "profiler: test_name, method: DummyResource:get.first_access, value: 2.0 mS, labels: test=value\n"
-test_handler_out_no_lbl = (
-    "profiler: test_name, method: DummyResource:get.first_access, value: 2.0 mS\n"
-)
+test_handler_out_no_lbl = "profiler: test_name, method: DummyResource:get.first_access, value: 2.0 mS\n"
 
 hist_no_lbl = [
     {
         "item": "test",
         "metric": "histogram",
         "units": "V",
         "job": "TEST",
@@ -179,7 +177,12 @@
     },
     {
         "method": "DummyDbAccess:second_access",
         "value": 4.0,
         "place": "after_root",
     },
 ]
+
+methods_between_out = [
+    "dummy_api:test_list_comp.test_inside_list_comp",
+    "DummyResource:get_.third_access.second_access.first_access",
+]
```

### Comparing `phanos-0.0.9/.gitignore` & `phanos-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `phanos-0.0.9/LICENSE` & `phanos-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phanos-0.0.9/README.md` & `phanos-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,95 @@
 # PHANOS
+
 Python client to gather data for Prometheus logging in server with multiple instances and workers.
 
 ## Profiling
 
 ### Default metrics
 
 Phanos contains two default metrics. Time profiler measuring execution time of
 decorated methods and response size profiler measuring response size of decorated method
-of endpoint. Both can be deleted by `phanos_profiler.delete_metric(phanos.publisher.TIME_PROFILER)`
-and `phanos_profiler.delete_metric(phanos.publisher.RESPONSE_SIZE)` if not deleted, measurements are
+of endpoint. Both can be deleted by `phanos.profiler.delete_metric(phanos.publisher.TIME_PROFILER)`
+and `phanos.profiler.delete_metric(phanos.publisher.RESPONSE_SIZE)` if not deleted, measurements are
 made automatically.
 
+### Configuration
+
+It is possible to configure profile with configration dictionary with method `PhanosProfiler.dict_config(settings)` _(similar to `logging` `dictConfig`)_. 
+Attributes are:
+
+- `job`_(optional)_ job _label_ for prometheus; usually name of app
+- `logger` _(optional)_ name of logger
+- `time_profile` _(optional)_ by default _profiler_ tracks execution time of profiled function/object
+- `handle_records` _(optional)_ should handle recorded records #TODO @miroslav.bulicka descrive better
+- `handlers` _(optional)_ serialized named handlers to publish profiled records
+  - `class` class handler to initialized
+  - `handler_name` handler name required argument of publishers
+  - `**other argumend` - specific arguments required to construct instance of class f.e.: `output`
+
+Example of configuration dict:
+
+```python
+settings = {
+    "job": "my_app", 
+    "logger": "my_app_debug_logger", 
+    "time_profile": True, 
+    "handle_records": True, 
+    "handlers": {
+        "stdout_handler_ref": {
+                "class": "phanos.publisher.StreamHandler", 
+                "handler_name": "stdout_handler", 
+                "output": "ext://sys.stdout"
+            }
+        }
+}
+```
+
+
 ### Usage
 
-1. decorate methods from which you want to send metrics `@phanos_profiler.profile`
-   ```python
-   from phanos import phanos_profiler
-   # some code
-   @phanos_profiler.profile
-   def some_method():
-      # some code
-   ```
+1. decorate methods from which you want to send metrics `@phanos.profile` shortcut for `@phanos.profiler.profile`
+
+    ```python
+    import phanos
+   
+    # some code
+    @phanos.profile
+    def some_method():
+        # some code
+    
+    # is equivalent to
+    @phanos.profiler.profile
+    def some_method():
+        # some code
+    ```
 
 2. Instantiate handlers you need for measured records at app construction.
-   ```python      
-   from phanos import phanos_profiler
-   from phanos.publisher import LoggerHandler, ImpProfHandler
-   # some code
-   class SomeApp(Flask):
+
+    ```python      
+    import phanos
+    from phanos.publisher import LoggerHandler, ImpProfHandler
+    # some code
+    class SomeApp(Flask):
       """some code""" 
-   phanos_profiler.config(logger, should_time_profile, should_resp_size_profile, should_handle_records)
-   log_handler = LoggerHandler('logger_name', logger_instance, logging_level)
-   phanos_profiler.addHandler(log_handler)    
-      # some code
-   ```
+    phanos.profiler.config(logger, should_time_profile, should_resp_size_profile, should_handle_records)
+    log_handler = LoggerHandler('logger_name', logger_instance, logging_level)
+    phanos.profiler.addHandler(log_handler)    
+    # some code
+    ```
+   
 In `config` method you can select if you want to turn off  time profiling, response size profiling
  or records handling. Default is turned on.
 After root method is executed all measured records are handled by all handlers added to
-`phanos_profiler`
+`phanos.profiler`
 
 ## Handlers
 
 Each handler have handler_name parameter. This string can be used to delete handlers later
-with `phanos_profiler.deleteHandler(handler_name)`.
+with `phanos.profiler.deleteHandler(handler_name)`.
 
 Records can be handled by these handlers:
  - `StreamHandler(handler_name, output)` - write records to given output (default is sys.stdout)
  - `LoggerHandler(handler_name, logger, level)` - logs string representation of records with given logger and with given level
 (default level is `logging.DEBUG`) 
  - `ImpProfHandler(handler_name, **rabbit_connection_params, logger)` - sending records to RabbitMQ queue of IMP_prof
 
@@ -77,44 +120,48 @@
   - `__init__()` method needs to call `super().__init__()`
   - `self.default_operation` and `self.operations` needs to be set
 - Implement method for each operation wanted
 - If special cleanup is needed after sending records implement method `cleanup()` calling `super().cleanup()` inside
 
 ### Add metrics automatic measurements
 
-'phanos_profiler' contains these four arguments:
+"phanos.profiler' contains these four arguments:
  
 - before_func : callable - executes before each profiled method
 - after_func : callable - executes after each profiled method
 - before_root_func : callable - executes before each profiled root method (first method in profiling tree)
 - after_root_func : callable - executes after each profiled root method (first method in profiling tree)
 
 Implement these methods with all your measurement. Example:
-   ```python
-   def before_function(function):
-      # this operation will be recorded
-      my_metric.store_operation(
-          operation="my_operation",
-          method=phanos_profiler.current_node.context,
-          value=measured_value,
-          label_values={"label_name": "label_value"},
-      )
-      # this won't be recorded
-      my_metric.my_method()
-      next_metric....
-   # some code 
-   phanos_profiler.before_func = before_function
-   ```
 
-`phanos_profiler` will record operation `"my_operation"` with value `measured_value` and given labels before
-each method decorated with `phanos_profiler.profile`.
+```python
+import phanos
+
+def before_function(*args, func=None, **kwargs):
+    # this operation will be recorded
+    my_metric.store_operation(
+        operation="my_operation",
+        method=phanos.profiler.current_node.context,
+        value=measured_value,
+        label_values={"label_name": "label_value"},
+    )
+    # this won't be recorded
+    my_metric.my_method()
+    next_metric....
+# some code 
+phanos.profiler.before_func = before_function
+```
+
+`phanos.profiler` will record operation `"my_operation"` with value `measured_value` and given labels before
+each method decorated with `phanos.profiler.profile` shortcut(`phanos.profile`).
+
+What must/can be done:
 
-What must/can be done
-- 'before_' functions must have 'function' parameter where function which is executed is passed.
+- 'before_' functions must have 'func' parameter passed as kwarg where function which is executed is passed.
 'after_' function needs to have 'fn_result' parameter where function result is passed
 - all four functions can access `*args` and `**kwargs` of decorated methods.
-- Each 'store_operation' must have parameter `method=phanos_profiler.current_node.context` so 
+- Each 'store_operation' must have parameter `method=phanos.profiler.current_node.context` so 
 method context is correctly saved. 
 - current_node.context stores context of method calling in format: 
 `"root_class.__name__:root_method.__name__.currently_executed.__name__"` if root is function then instead of 
 class name its module name.
```

### Comparing `phanos-0.0.9/pyproject.toml` & `phanos-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "phanos"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Miroslav Bulička", email="bulickamiroslav@gmail.com" },
 ]
 description = "Python client to gather data for Prometheus logging in server with multiple instances and workers."
 readme = "README.md"
 requires-python = ">=3.10.6"
 classifiers = [
+    "Intended Audience :: Developers",
+    "Intended Audience :: System Administrators",
+    "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Topic :: System :: Monitoring",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pip>=23.1.2",
     "Flask>=2.2.3",
     "pika>=1.3.2",
```

### Comparing `phanos-0.0.9/PKG-INFO` & `phanos-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,118 @@
 Metadata-Version: 2.1
 Name: phanos
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python client to gather data for Prometheus logging in server with multiple instances and workers.
 Project-URL: Homepage, https://github.com/kajotgames/phanos
 Project-URL: Bug Tracker, https://github.com/kajotgames/phanos/issues
 Author-email: Miroslav Bulička <bulickamiroslav@gmail.com>
 License-File: LICENSE
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.10.6
 Requires-Dist: flask-restx>=1.1.0
 Requires-Dist: flask>=2.2.3
 Requires-Dist: imp-prof>=0.1.2
 Requires-Dist: pika>=1.3.2
 Requires-Dist: pip>=23.1.2
 Description-Content-Type: text/markdown
 
 # PHANOS
+
 Python client to gather data for Prometheus logging in server with multiple instances and workers.
 
 ## Profiling
 
 ### Default metrics
 
 Phanos contains two default metrics. Time profiler measuring execution time of
 decorated methods and response size profiler measuring response size of decorated method
-of endpoint. Both can be deleted by `phanos_profiler.delete_metric(phanos.publisher.TIME_PROFILER)`
-and `phanos_profiler.delete_metric(phanos.publisher.RESPONSE_SIZE)` if not deleted, measurements are
+of endpoint. Both can be deleted by `phanos.profiler.delete_metric(phanos.publisher.TIME_PROFILER)`
+and `phanos.profiler.delete_metric(phanos.publisher.RESPONSE_SIZE)` if not deleted, measurements are
 made automatically.
 
+### Configuration
+
+It is possible to configure profile with configration dictionary with method `PhanosProfiler.dict_config(settings)` _(similar to `logging` `dictConfig`)_. 
+Attributes are:
+
+- `job`_(optional)_ job _label_ for prometheus; usually name of app
+- `logger` _(optional)_ name of logger
+- `time_profile` _(optional)_ by default _profiler_ tracks execution time of profiled function/object
+- `handle_records` _(optional)_ should handle recorded records #TODO @miroslav.bulicka descrive better
+- `handlers` _(optional)_ serialized named handlers to publish profiled records
+  - `class` class handler to initialized
+  - `handler_name` handler name required argument of publishers
+  - `**other argumend` - specific arguments required to construct instance of class f.e.: `output`
+
+Example of configuration dict:
+
+```python
+settings = {
+    "job": "my_app", 
+    "logger": "my_app_debug_logger", 
+    "time_profile": True, 
+    "handle_records": True, 
+    "handlers": {
+        "stdout_handler_ref": {
+                "class": "phanos.publisher.StreamHandler", 
+                "handler_name": "stdout_handler", 
+                "output": "ext://sys.stdout"
+            }
+        }
+}
+```
+
+
 ### Usage
 
-1. decorate methods from which you want to send metrics `@phanos_profiler.profile`
-   ```python
-   from phanos import phanos_profiler
-   # some code
-   @phanos_profiler.profile
-   def some_method():
-      # some code
-   ```
+1. decorate methods from which you want to send metrics `@phanos.profile` shortcut for `@phanos.profiler.profile`
+
+    ```python
+    import phanos
+   
+    # some code
+    @phanos.profile
+    def some_method():
+        # some code
+    
+    # is equivalent to
+    @phanos.profiler.profile
+    def some_method():
+        # some code
+    ```
 
 2. Instantiate handlers you need for measured records at app construction.
-   ```python      
-   from phanos import phanos_profiler
-   from phanos.publisher import LoggerHandler, ImpProfHandler
-   # some code
-   class SomeApp(Flask):
+
+    ```python      
+    import phanos
+    from phanos.publisher import LoggerHandler, ImpProfHandler
+    # some code
+    class SomeApp(Flask):
       """some code""" 
-   phanos_profiler.config(logger, should_time_profile, should_resp_size_profile, should_handle_records)
-   log_handler = LoggerHandler('logger_name', logger_instance, logging_level)
-   phanos_profiler.addHandler(log_handler)    
-      # some code
-   ```
+    phanos.profiler.config(logger, should_time_profile, should_resp_size_profile, should_handle_records)
+    log_handler = LoggerHandler('logger_name', logger_instance, logging_level)
+    phanos.profiler.addHandler(log_handler)    
+    # some code
+    ```
+   
 In `config` method you can select if you want to turn off  time profiling, response size profiling
  or records handling. Default is turned on.
 After root method is executed all measured records are handled by all handlers added to
-`phanos_profiler`
+`phanos.profiler`
 
 ## Handlers
 
 Each handler have handler_name parameter. This string can be used to delete handlers later
-with `phanos_profiler.deleteHandler(handler_name)`.
+with `phanos.profiler.deleteHandler(handler_name)`.
 
 Records can be handled by these handlers:
  - `StreamHandler(handler_name, output)` - write records to given output (default is sys.stdout)
  - `LoggerHandler(handler_name, logger, level)` - logs string representation of records with given logger and with given level
 (default level is `logging.DEBUG`) 
  - `ImpProfHandler(handler_name, **rabbit_connection_params, logger)` - sending records to RabbitMQ queue of IMP_prof
 
@@ -96,44 +143,48 @@
   - `__init__()` method needs to call `super().__init__()`
   - `self.default_operation` and `self.operations` needs to be set
 - Implement method for each operation wanted
 - If special cleanup is needed after sending records implement method `cleanup()` calling `super().cleanup()` inside
 
 ### Add metrics automatic measurements
 
-'phanos_profiler' contains these four arguments:
+"phanos.profiler' contains these four arguments:
  
 - before_func : callable - executes before each profiled method
 - after_func : callable - executes after each profiled method
 - before_root_func : callable - executes before each profiled root method (first method in profiling tree)
 - after_root_func : callable - executes after each profiled root method (first method in profiling tree)
 
 Implement these methods with all your measurement. Example:
-   ```python
-   def before_function(function):
-      # this operation will be recorded
-      my_metric.store_operation(
-          operation="my_operation",
-          method=phanos_profiler.current_node.context,
-          value=measured_value,
-          label_values={"label_name": "label_value"},
-      )
-      # this won't be recorded
-      my_metric.my_method()
-      next_metric....
-   # some code 
-   phanos_profiler.before_func = before_function
-   ```
 
-`phanos_profiler` will record operation `"my_operation"` with value `measured_value` and given labels before
-each method decorated with `phanos_profiler.profile`.
+```python
+import phanos
+
+def before_function(*args, func=None, **kwargs):
+    # this operation will be recorded
+    my_metric.store_operation(
+        operation="my_operation",
+        method=phanos.profiler.current_node.context,
+        value=measured_value,
+        label_values={"label_name": "label_value"},
+    )
+    # this won't be recorded
+    my_metric.my_method()
+    next_metric....
+# some code 
+phanos.profiler.before_func = before_function
+```
+
+`phanos.profiler` will record operation `"my_operation"` with value `measured_value` and given labels before
+each method decorated with `phanos.profiler.profile` shortcut(`phanos.profile`).
+
+What must/can be done:
 
-What must/can be done
-- 'before_' functions must have 'function' parameter where function which is executed is passed.
+- 'before_' functions must have 'func' parameter passed as kwarg where function which is executed is passed.
 'after_' function needs to have 'fn_result' parameter where function result is passed
 - all four functions can access `*args` and `**kwargs` of decorated methods.
-- Each 'store_operation' must have parameter `method=phanos_profiler.current_node.context` so 
+- Each 'store_operation' must have parameter `method=phanos.profiler.current_node.context` so 
 method context is correctly saved. 
 - current_node.context stores context of method calling in format: 
 `"root_class.__name__:root_method.__name__.currently_executed.__name__"` if root is function then instead of 
 class name its module name.
```

