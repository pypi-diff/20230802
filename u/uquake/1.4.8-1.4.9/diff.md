# Comparing `tmp/uquake-1.4.8.tar.gz` & `tmp/uquake-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uquake-1.4.8.tar", max compression
+gzip compressed data, was "uquake-1.4.9.tar", max compression
```

## Comparing `uquake-1.4.8.tar` & `uquake-1.4.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     2399 2023-07-18 13:46:01.800875 uquake-1.4.8/pyproject.toml
--rw-r--r--   0        0        0      158 2023-01-25 01:11:29.666160 uquake-1.4.8/uquake/__init__.py
--rw-r--r--   0        0        0      191 2023-01-15 00:23:22.715786 uquake-1.4.8/uquake/core/__init__.py
--rw-r--r--   0        0        0     4143 2023-05-26 14:14:51.615907 uquake-1.4.8/uquake/core/data_ensemble.py
--rw-r--r--   0        0        0      658 2023-01-15 00:23:22.715786 uquake-1.4.8/uquake/core/decorators.py
--rw-r--r--   0        0        0    35168 2023-05-26 12:44:33.128508 uquake-1.4.8/uquake/core/event.py
--rw-r--r--   0        0        0     6233 2023-01-15 00:23:22.715786 uquake-1.4.8/uquake/core/focal_mechanism.py
--rw-r--r--   0        0        0    38730 2023-05-26 12:30:49.530264 uquake-1.4.8/uquake/core/inventory.py
--rw-r--r--   0        0        0      239 2023-01-15 00:23:22.715786 uquake-1.4.8/uquake/core/logging.py
--rw-r--r--   0        0        0    13782 2023-01-25 01:08:23.561456 uquake-1.4.8/uquake/core/stream.py
--rw-r--r--   0        0        0     4964 2023-07-18 13:43:22.013456 uquake-1.4.8/uquake/core/trace.py
--rw-r--r--   0        0        0       67 2023-01-15 00:23:22.715786 uquake-1.4.8/uquake/core/util/__init__.py
--rw-r--r--   0        0        0     4206 2023-01-15 00:23:22.715786 uquake-1.4.8/uquake/core/util/base.py
--rw-r--r--   0        0        0     5713 2023-01-15 00:23:22.715786 uquake-1.4.8/uquake/core/util/decorator.py
--rw-r--r--   0        0        0      620 2023-04-16 18:19:34.782672 uquake-1.4.8/uquake/core/util/requests.py
--rw-r--r--   0        0        0    13768 2023-01-15 00:23:22.715786 uquake-1.4.8/uquake/core/util/tools.py
--rw-r--r--   0        0        0       28 2023-01-15 00:23:22.715786 uquake-1.4.8/uquake/grid/__init__.py
--rw-r--r--   0        0        0    22173 2023-04-27 00:23:45.744173 uquake-1.4.8/uquake/grid/base.py
--rw-r--r--   0        0        0     4660 2023-05-06 10:03:22.429231 uquake-1.4.8/uquake/grid/hdf5.py
--rw-r--r--   0        0        0    47247 2023-04-27 00:26:03.338550 uquake-1.4.8/uquake/grid/nlloc.py
--rw-r--r--   0        0        0        0 2023-01-15 00:23:22.715786 uquake-1.4.8/uquake/imaging/__init__.py
--rw-r--r--   0        0        0    10043 2023-03-08 09:37:25.089762 uquake-1.4.8/uquake/imaging/plot.py
--rw-r--r--   0        0        0     2474 2023-01-15 00:23:22.715786 uquake-1.4.8/uquake/imaging/stereonet.py
--rw-r--r--   0        0        0    59743 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/imaging/waveform.py
--rw-r--r--   0        0        0      423 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/io/__init__.py
--rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/io/event/__init__.py
--rw-r--r--   0        0        0     3417 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/io/event/core.py
--rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/io/grid/__init__.py
--rw-r--r--   0        0        0     8496 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/io/grid/core.py
--rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/io/inventory/__init__.py
--rw-r--r--   0        0        0     6531 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/io/inventory/core.py
--rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/io/waveform/__init__.py
--rw-r--r--   0        0        0     9262 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/io/waveform/core.py
--rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/nlloc/__init__.py
--rw-r--r--   0        0        0    48293 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/nlloc/nlloc.py
--rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/waveform/__init__.py
--rw-r--r--   0        0        0    34528 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/waveform/amp_measures.py
--rw-r--r--   0        0        0    15799 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/waveform/mag.py
--rw-r--r--   0        0        0     5354 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/waveform/mag_utils.py
--rw-r--r--   0        0        0     2827 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/waveform/parseval_utils.py
--rw-r--r--   0        0        0    21331 2023-05-16 01:15:39.357070 uquake-1.4.8/uquake/waveform/pick.py
--rw-r--r--   0        0        0    45461 2023-04-04 17:02:48.691928 uquake-1.4.8/uquake/waveform/simple_mag.py
--rw-r--r--   0        0        0    32225 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/waveform/smom_measure.py
--rw-r--r--   0        0        0    33065 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/waveform/smom_measure_legacy.py
--rw-r--r--   0        0        0     4456 2023-01-15 00:23:22.719786 uquake-1.4.8/uquake/waveform/transforms.py
--rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 uquake-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0     2399 2023-08-02 15:43:43.118751 uquake-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-01-25 01:11:29.666160 uquake-1.4.9/uquake/__init__.py
+-rw-r--r--   0        0        0      191 2023-01-15 00:23:22.715786 uquake-1.4.9/uquake/core/__init__.py
+-rw-r--r--   0        0        0     4143 2023-05-26 14:14:51.615907 uquake-1.4.9/uquake/core/data_ensemble.py
+-rw-r--r--   0        0        0      658 2023-01-15 00:23:22.715786 uquake-1.4.9/uquake/core/decorators.py
+-rw-r--r--   0        0        0    35168 2023-05-26 12:44:33.128508 uquake-1.4.9/uquake/core/event.py
+-rw-r--r--   0        0        0     6233 2023-01-15 00:23:22.715786 uquake-1.4.9/uquake/core/focal_mechanism.py
+-rw-r--r--   0        0        0    39003 2023-08-02 15:42:09.382424 uquake-1.4.9/uquake/core/inventory.py
+-rw-r--r--   0        0        0      239 2023-01-15 00:23:22.715786 uquake-1.4.9/uquake/core/logging.py
+-rw-r--r--   0        0        0    13782 2023-01-25 01:08:23.561456 uquake-1.4.9/uquake/core/stream.py
+-rw-r--r--   0        0        0     4964 2023-07-18 13:43:22.013456 uquake-1.4.9/uquake/core/trace.py
+-rw-r--r--   0        0        0       67 2023-01-15 00:23:22.715786 uquake-1.4.9/uquake/core/util/__init__.py
+-rw-r--r--   0        0        0     4206 2023-01-15 00:23:22.715786 uquake-1.4.9/uquake/core/util/base.py
+-rw-r--r--   0        0        0     5713 2023-01-15 00:23:22.715786 uquake-1.4.9/uquake/core/util/decorator.py
+-rw-r--r--   0        0        0      620 2023-04-16 18:19:34.782672 uquake-1.4.9/uquake/core/util/requests.py
+-rw-r--r--   0        0        0    13768 2023-01-15 00:23:22.715786 uquake-1.4.9/uquake/core/util/tools.py
+-rw-r--r--   0        0        0       28 2023-01-15 00:23:22.715786 uquake-1.4.9/uquake/grid/__init__.py
+-rw-r--r--   0        0        0    22173 2023-04-27 00:23:45.744173 uquake-1.4.9/uquake/grid/base.py
+-rw-r--r--   0        0        0     4660 2023-05-06 10:03:22.429231 uquake-1.4.9/uquake/grid/hdf5.py
+-rw-r--r--   0        0        0    47247 2023-04-27 00:26:03.338550 uquake-1.4.9/uquake/grid/nlloc.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.715786 uquake-1.4.9/uquake/imaging/__init__.py
+-rw-r--r--   0        0        0    10043 2023-03-08 09:37:25.089762 uquake-1.4.9/uquake/imaging/plot.py
+-rw-r--r--   0        0        0     2474 2023-01-15 00:23:22.715786 uquake-1.4.9/uquake/imaging/stereonet.py
+-rw-r--r--   0        0        0    59743 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/imaging/waveform.py
+-rw-r--r--   0        0        0      423 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/io/event/__init__.py
+-rw-r--r--   0        0        0     3417 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/io/event/core.py
+-rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/io/grid/__init__.py
+-rw-r--r--   0        0        0     8496 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/io/grid/core.py
+-rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/io/inventory/__init__.py
+-rw-r--r--   0        0        0     6531 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/io/inventory/core.py
+-rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/io/waveform/__init__.py
+-rw-r--r--   0        0        0     9262 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/io/waveform/core.py
+-rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/nlloc/__init__.py
+-rw-r--r--   0        0        0    48241 2023-07-18 18:09:25.413132 uquake-1.4.9/uquake/nlloc/nlloc.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/waveform/__init__.py
+-rw-r--r--   0        0        0    34528 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/waveform/amp_measures.py
+-rw-r--r--   0        0        0    15799 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/waveform/mag.py
+-rw-r--r--   0        0        0     5354 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/waveform/mag_utils.py
+-rw-r--r--   0        0        0     2827 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/waveform/parseval_utils.py
+-rw-r--r--   0        0        0    21331 2023-05-16 01:15:39.357070 uquake-1.4.9/uquake/waveform/pick.py
+-rw-r--r--   0        0        0    45461 2023-04-04 17:02:48.691928 uquake-1.4.9/uquake/waveform/simple_mag.py
+-rw-r--r--   0        0        0    32225 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/waveform/smom_measure.py
+-rw-r--r--   0        0        0    33065 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/waveform/smom_measure_legacy.py
+-rw-r--r--   0        0        0     4456 2023-01-15 00:23:22.719786 uquake-1.4.9/uquake/waveform/transforms.py
+-rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 uquake-1.4.9/PKG-INFO
```

### Comparing `uquake-1.4.8/pyproject.toml` & `uquake-1.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uquake"
-version = "1.4.8"
+version = "1.4.9"
 description = "extension of the ObsPy library for local seismicity"
 authors = ["uQuake development team <dev@uQuake.org>"]
 license = "MIT"
 
 # poetry config virtualenvs.create false; poetry env info
 
 [tool.poetry.dependencies]
```

### Comparing `uquake-1.4.8/uquake/core/data_ensemble.py` & `uquake-1.4.9/uquake/core/data_ensemble.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/core/decorators.py` & `uquake-1.4.9/uquake/core/decorators.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/core/event.py` & `uquake-1.4.9/uquake/core/event.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/core/focal_mechanism.py` & `uquake-1.4.9/uquake/core/focal_mechanism.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/core/inventory.py` & `uquake-1.4.9/uquake/core/inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,19 +96,27 @@
 
     @property
     def response(self):
         if len(self.response_stages) == 0:
             return
 
         input_units = self.response_stages[0].input_units
+
+        if input_units == 'M/S':
+            input_units_description = 'Velocity'
+        elif input_units == 'M/S/S':
+            input_units_description = 'Acceleration'
+        elif input_units == 'M':
+            input_units_description = 'Displacement'
+
         i_s = InstrumentSensitivity(self.sensitivity,
                                     self.frequency,
                                     input_units=input_units,
                                     output_units='COUNT',
-                                    input_units_description='Velocity',
+                                    input_units_description=input_units_description,
                                     output_units_description='ADC Count')
 
         return Response(instrument_sensitivity=i_s,
                         response_stages=self.response_stages)
 
 
 def geophone_response(resonance_frequency, gain, damping=0.707,
```

### Comparing `uquake-1.4.8/uquake/core/stream.py` & `uquake-1.4.9/uquake/core/stream.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/core/trace.py` & `uquake-1.4.9/uquake/core/trace.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/core/util/base.py` & `uquake-1.4.9/uquake/core/util/base.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/core/util/decorator.py` & `uquake-1.4.9/uquake/core/util/decorator.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/core/util/requests.py` & `uquake-1.4.9/uquake/core/util/requests.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/core/util/tools.py` & `uquake-1.4.9/uquake/core/util/tools.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/grid/base.py` & `uquake-1.4.9/uquake/grid/base.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/grid/hdf5.py` & `uquake-1.4.9/uquake/grid/hdf5.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/grid/nlloc.py` & `uquake-1.4.9/uquake/grid/nlloc.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/imaging/plot.py` & `uquake-1.4.9/uquake/imaging/plot.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/imaging/stereonet.py` & `uquake-1.4.9/uquake/imaging/stereonet.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/imaging/waveform.py` & `uquake-1.4.9/uquake/imaging/waveform.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/io/event/core.py` & `uquake-1.4.9/uquake/io/event/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/io/grid/core.py` & `uquake-1.4.9/uquake/io/grid/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/io/inventory/core.py` & `uquake-1.4.9/uquake/io/inventory/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/io/waveform/core.py` & `uquake-1.4.9/uquake/io/waveform/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/nlloc/nlloc.py` & `uquake-1.4.9/uquake/nlloc/nlloc.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 from ..core.inventory import Inventory
 from ..core.logging import logger
 from ..core.event import (Catalog)
 
 from uuid import uuid4
 from pathlib import Path
 import json
+import secrets
+import string
 
 test_station_code = 'STN'
 
 
 def validate(value, choices):
     if value not in choices:
         msg = f'value should be one of the following choices\n:'
@@ -908,15 +910,15 @@
 
         sites = []
         for site in inventory.sites:
             sites.append(Site(site.code, site.x, site.y, site.z))
         return cls(sites)
 
     @classmethod
-    def generate_random_srces_in_grid(cls, gd, n_srces=1):
+    def generate_random_srces_in_grid(cls, gd, n_srces=1, label_root='sta'):
         """
         generate n_srces random srces inside the grid provided. This function
         is mainly used for testing purposes
         :param gd: a grid
         :type gd: uquake.grid.base.Grid or an object inheriting from Grid
         :param n_srces: number of Srces to generate
         :return: a list of srces
@@ -927,15 +929,14 @@
         >>> grid_spacing = [1, 1, 1]
         >>> grid_origin = [0, 0, 0]
         >>> grid = Grid(grid_dimensions, grid_spacing, grid_origin, value=1)
         >>> srces = Srces.generate_random_srces_in_grid(grid, nb_seeds=10)
         """
 
         srces = []
-        label_root = test_station_code
         for i, point in enumerate(gd.generate_random_points_in_grid(
                 n_points=n_srces)):
             label = f'{label_root}{i:02d}'
             site = Site(label, point[0], point[1], point[2])
             srces.append(site)
         return cls(srces)
 
@@ -959,16 +960,14 @@
         :param units: units of measurement used to express x, y, and z
         ( 'METERS' or 'KILOMETERS')
 
         """
 
         validate(units.upper(), self.__valid_measurement_units__)
 
-        self.sites.append(Site(label, x, y, z, elev=elev))
-
         self.units = units.upper()
 
     def __repr__(self):
         line = ""
 
         for site in self.sites:
             # test if site name is shorter than 6 characters
```

### Comparing `uquake-1.4.8/uquake/waveform/amp_measures.py` & `uquake-1.4.9/uquake/waveform/amp_measures.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/waveform/mag.py` & `uquake-1.4.9/uquake/waveform/mag.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/waveform/mag_utils.py` & `uquake-1.4.9/uquake/waveform/mag_utils.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/waveform/parseval_utils.py` & `uquake-1.4.9/uquake/waveform/parseval_utils.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/waveform/pick.py` & `uquake-1.4.9/uquake/waveform/pick.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/waveform/simple_mag.py` & `uquake-1.4.9/uquake/waveform/simple_mag.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/waveform/smom_measure.py` & `uquake-1.4.9/uquake/waveform/smom_measure.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/waveform/smom_measure_legacy.py` & `uquake-1.4.9/uquake/waveform/smom_measure_legacy.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/uquake/waveform/transforms.py` & `uquake-1.4.9/uquake/waveform/transforms.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.8/PKG-INFO` & `uquake-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uquake
-Version: 1.4.8
+Version: 1.4.9
 Summary: extension of the ObsPy library for local seismicity
 License: MIT
 Author: uQuake development team
 Author-email: dev@uQuake.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

