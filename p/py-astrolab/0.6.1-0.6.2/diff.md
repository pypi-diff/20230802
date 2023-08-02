# Comparing `tmp/py_astrolab-0.6.1.tar.gz` & `tmp/py_astrolab-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.6.1.tar", max compression
+gzip compressed data, was "py_astrolab-0.6.2.tar", max compression
```

## Comparing `py_astrolab-0.6.1.tar` & `py_astrolab-0.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.1/README.md
--rwxr-xr-x   0        0        0     4901 2023-08-01 09:27:23.596932 py_astrolab-0.6.1/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    15760 2023-07-30 15:40:50.145067 py_astrolab-0.6.1/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.1/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    80380 2023-07-29 10:08:55.050610 py_astrolab-0.6.1/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.1/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.1/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.1/py_astrolab/charts/templates/minimal.xml
--rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.1/py_astrolab/charts/wonderful_mistake.py
--rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.1/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12935 2023-07-27 22:22:27.571322 py_astrolab-0.6.1/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.1/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.1/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.1/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.1/py_astrolab/report.py
--rwxr-xr-x   0        0        0    18869 2023-08-01 17:01:51.902444 py_astrolab-0.6.1/py_astrolab/transits.py
--rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.1/py_astrolab/types.py
--rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.1/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      664 2023-08-01 17:20:01.497439 py_astrolab-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.1/PKG-INFO
+-rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.2/README.md
+-rwxr-xr-x   0        0        0     4901 2023-08-01 09:27:23.596932 py_astrolab-0.6.2/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    15760 2023-07-30 15:40:50.145067 py_astrolab-0.6.2/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.2/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    80380 2023-07-29 10:08:55.050610 py_astrolab-0.6.2/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.2/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.2/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.2/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.2/py_astrolab/charts/wonderful_mistake.py
+-rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.2/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12935 2023-07-27 22:22:27.571322 py_astrolab-0.6.2/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.2/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.2/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.2/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.2/py_astrolab/report.py
+-rwxr-xr-x   0        0        0    20501 2023-08-02 09:40:02.508864 py_astrolab-0.6.2/py_astrolab/transits.py
+-rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.2/py_astrolab/types.py
+-rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.2/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      664 2023-08-02 09:40:58.962869 py_astrolab-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.2/PKG-INFO
```

### Comparing `py_astrolab-0.6.1/py_astrolab/__init__.py` & `py_astrolab-0.6.2/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/aspects.py` & `py_astrolab-0.6.2/py_astrolab/aspects.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.6.2/py_astrolab/charts/charts_svg.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.6.2/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.6.2/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.6.2/py_astrolab/charts/templates/minimal.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/charts/wonderful_mistake.py` & `py_astrolab-0.6.2/py_astrolab/charts/wonderful_mistake.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/fetch_geonames.py` & `py_astrolab-0.6.2/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/kr.config.json` & `py_astrolab-0.6.2/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/main.py` & `py_astrolab-0.6.2/py_astrolab/main.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/print_all_data.py` & `py_astrolab-0.6.2/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/relationship_score.py` & `py_astrolab-0.6.2/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/report.py` & `py_astrolab-0.6.2/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/transits.py` & `py_astrolab-0.6.2/py_astrolab/transits.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import math
 from datetime import datetime, timedelta
 from itertools import combinations, product
 from typing import Union
 
 import swisseph as swe
 
 from py_astrolab import KrInstance
@@ -75,23 +74,23 @@
         lon1 = self.calc_long(jd, planet1)
         lon2 = self.calc_long(jd, planet2) if not natal_planet_orb else natal_planet_orb
         angle = self.angle_difference(lon1, lon2)
         orb = abs(abs(angle) - aspect)
         self.orb_cache[cache_tuple] = orb
         return orb
 
-    def aspects_transits_transits(self, look_for_planets = None):
+    def aspects_transits_transits(self, look_for_planets=None, activation_only=False):
         look_for_planets = set(self.planet_names.keys()) if look_for_planets is None else look_for_planets
-        aspects = self.find_transit_transit_aspects(self.times, self.positions, look_for_planets)
+        aspects = self.find_transit_transit_aspects(self.times, self.positions, look_for_planets, activation_only)
         return aspects
 
-    def aspects_natal_transits(self, look_for_planets = None):
+    def aspects_natal_transits(self, look_for_planets = None, activation_only=False):
         look_for_planets = set(self.planet_names.keys()) if look_for_planets is None else look_for_planets
         natal_positions = {planet_data['name']: planet_data['abs_pos'] for planet_data in self.user.planets_list}
-        aspects = self.find_natal_transit_aspects(self.times, self.positions, natal_positions, look_for_planets)
+        aspects = self.find_natal_transit_aspects(self.times, self.positions, natal_positions, look_for_planets, activation_only)
         return aspects
 
     def angle_difference(self, angle1, angle2):
         return 180 - abs(abs(angle1 - angle2) - 180)
 
     def jd_to_datetime(self, jd):
         if jd in self.julday_cache:
@@ -190,15 +189,15 @@
         for time in times:
             jd = self.datetime_to_jd(time)
             for planet in self.planets:
                 lon = self.calc_long(jd, planet)
                 positions[planet].append(lon)
         return times, positions
 
-    def find_transit_transit_aspects(self, times, positions, look_for_planets):
+    def find_transit_transit_aspects(self, times, positions, look_for_planets, activation_only):
         aspects = {}
         current_aspects = set()
         for planet1, planet2 in combinations(self.planets, 2):
             if planet1 not in look_for_planets:
                 continue
             orbit_tolerance = min(self.planet_names[planet1]['orbit'], self.planet_names[planet2]['orbit'])
             interval = min(self.planet_names[planet1]['interval'], self.planet_names[planet2]['interval'])
@@ -208,31 +207,35 @@
                     p2_name = self.planet_names[planet2]['name']
                     aspect_name = self.aspect_names[a]
                     aspect_tuple = (p1_name, p2_name, aspect_name)
                     diff1 = self.angle_difference(lon1_1, lon2_1)
                     diff2 = self.angle_difference(lon1_2, lon2_2)
                     if ((diff1 - a) * (diff2 - a) <= 0) or (abs(diff1 - a) <= orbit_tolerance) or (abs(diff2 - a) <= orbit_tolerance):
                         if aspect_tuple not in current_aspects:
-                            if time1 == self.start:
+                            if time1 == self.start and not activation_only:
                                 start_time, orb = self.backward_binary_search(planet1, planet2, a, orbit_tolerance, None, interval)
                             else:
                                 start_time, orb = self.binary_search(time1, time2, planet1, planet2, a, orbit_tolerance, None)
-                            finish_time, _ = self.forward_binary_search(planet1, planet2, a, orbit_tolerance, start_time, None, interval)
-                            exact_time, exact_orb = self.binary_search(self.start, self.end, planet1, planet2, a, 0, None)
-                            exact_time = exact_time if exact_orb < 0.1 else None
-                            p1_sign = self.get_zodiac_sign(self.calc_long(self.datetime_to_jd(start_time), planet1))
-                            p2_sign = self.get_zodiac_sign(self.calc_long(self.datetime_to_jd(start_time), planet2))
-                            aspect_dict = {'p1_name': p1_name, 'p2_name': p2_name, 'p1_sign': p1_sign, 'p2_sign': p2_sign, 'aspect': aspect_name, 'start': start_time, 'exact': exact_time, 'finish': finish_time, 'duration': finish_time-start_time, 'orb': orb}
-                            aspects.setdefault(start_time, []).append(aspect_dict)
+                                start_time = start_time if abs(orb - orbit_tolerance) < 0.1 else None
+                            if activation_only:
+                                finish_time = None
+                            else:
+                                finish_time, _ = self.forward_binary_search(planet1, planet2, a, orbit_tolerance, start_time, None, interval)
+                            if start_time is not None:
+                                p1_sign = self.get_zodiac_sign(self.calc_long(self.datetime_to_jd(start_time), planet1))
+                                p2_sign = self.get_zodiac_sign(self.calc_long(self.datetime_to_jd(start_time), planet2))
+                                duration = finish_time-start_time if finish_time is not None else None
+                                aspect_dict = {'p1_name': p1_name, 'p2_name': p2_name, 'p1_sign': p1_sign, 'p2_sign': p2_sign, 'aspect': aspect_name, 'start': start_time, 'finish': finish_time, 'duration': duration, 'orb': orb}
+                                aspects.setdefault(start_time, []).append(aspect_dict)
                             current_aspects.add(aspect_tuple)
                     else:
                         current_aspects.discard(aspect_tuple)
         return aspects
 
-    def find_natal_transit_aspects(self, times, positions, natal_positions, look_for_planets):
+    def find_natal_transit_aspects(self, times, positions, natal_positions, look_for_planets, activation_only):
         aspects = {}
         current_aspects = set()
         for planet1, planet2 in product(self.planets, natal_positions.keys()):
             if planet1 not in look_for_planets:
                 continue
             planet2_number = next((planet for planet, info in self.planet_names.items() if info['name'] == planet2), None)
             interval = self.planet_names[planet1]['interval']
@@ -246,28 +249,32 @@
                     p2_name = planet2
                     aspect_name = self.aspect_names[a]
                     aspect_tuple = (p1_name, p2_name, aspect_name)
                     diff1 = self.angle_difference(lon1_1, natal_position)
                     diff2 = self.angle_difference(lon1_2, natal_position)
                     if ((diff1 - a) * (diff2 - a) <= 0) or (abs(diff1 - a) <= orbit_tolerance) or (abs(diff2 - a) <= orbit_tolerance):
                         if aspect_tuple not in current_aspects:
-                            if time1 == self.start:
+                            if time1 == self.start and not activation_only:
                                 start_time, orb = self.backward_binary_search(planet1, planet2_number, a, orbit_tolerance, natal_position, interval)
                             else:
                                 start_time, orb = self.binary_search(time1, time2, planet1, planet2_number, a, orbit_tolerance, natal_position)
-                            finish_time, _ = self.forward_binary_search(planet1, planet2_number, a, orbit_tolerance, start_time, natal_position, interval)
-                            exact_time, exact_orb = self.binary_search(self.start, self.end, planet1, planet2_number, a, 0, natal_position)
-                            exact_time = exact_time if exact_orb < 0.1 else None
-                            p1_long = self.calc_long(self.datetime_to_jd(start_time), planet1)
-                            p1_sign = self.get_zodiac_sign(p1_long)
-                            p2_sign = getattr(self.user, p2_name.lower())['signs'][0]
-                            p1_house = self.point_in_house(p1_long)
-                            p2_house = getattr(self.user, p2_name.lower())['house']
-                            aspect_dict = {'p1_name': p1_name, 'p2_name': p2_name, 'p1_sign': p1_sign, 'p2_sign': p2_sign, 'p1_house': p1_house, 'p2_house': p2_house, 'aspect': aspect_name, 'start': start_time, 'exact': exact_time, 'finish': finish_time, 'duration': finish_time-start_time, 'orb': orb}
-                            aspects.setdefault(start_time, []).append(aspect_dict)
+                                start_time = start_time if abs(orb - orbit_tolerance) < 0.1 else None
+                            if activation_only:
+                                finish_time = None
+                            else:
+                                finish_time, _ = self.forward_binary_search(planet1, planet2_number, a, orbit_tolerance, start_time, natal_position, interval)
+                            if start_time:
+                                p1_long = self.calc_long(self.datetime_to_jd(start_time), planet1)
+                                p1_sign = self.get_zodiac_sign(p1_long)
+                                p2_sign = getattr(self.user, p2_name.lower())['signs'][0]
+                                p1_house = self.point_in_house(p1_long)
+                                p2_house = getattr(self.user, p2_name.lower())['house']
+                                duration = finish_time-start_time if finish_time is not None else None
+                                aspect_dict = {'p1_name': p1_name, 'p2_name': p2_name, 'p1_sign': p1_sign, 'p2_sign': p2_sign, 'p1_house': p1_house, 'p2_house': p2_house, 'aspect': aspect_name, 'start': start_time, 'finish': finish_time, 'duration': duration, 'orb': orb}
+                                aspects.setdefault(start_time, []).append(aspect_dict)
                             current_aspects.add(aspect_tuple)
                     else:
                         current_aspects.discard(aspect_tuple)
         return aspects
 
     def get_zodiac_sign(self, lon):
         signs = ['Ari', 'Tau', 'Gem', 'Can', 'Leo', 'Vir', 
@@ -311,13 +318,43 @@
         new_moon_obj['when'], new_moon_obj['orb'] = self.backward_binary_search(0, 1, 0, 0, None, timedelta(minutes=30))
         new_moon_long = self.calc_long(self.datetime_to_jd(new_moon_obj['when']), 1)
         sign = self.get_zodiac_sign(new_moon_long)
         new_moon_obj['sign'] = sign
         new_moon_obj['house'] = self.point_in_house(new_moon_long)
         return new_moon_obj
 
+    def lunar_phase(self):
+        jd = self.datetime_to_jd(self.start)
+        moon_longitude = self.calc_long(jd, swe.MOON)
+        sun_longitude = self.calc_long(jd, swe.SUN)
+        phase_angle = self.angle_difference(moon_longitude, sun_longitude)
+        if phase_angle < 0:
+            phase_angle += 360
+        if phase_angle < 11.25 or phase_angle >= 348.75:
+            phase_name = "New Moon"
+        elif phase_angle < 78.75:
+            phase_name = "Waxing Crescent"
+        elif phase_angle < 101.25:
+            phase_name = "First Quarter"
+        elif phase_angle < 168.75:
+            phase_name = "Waxing Gibbous"
+        elif phase_angle < 191.25:
+            phase_name = "Full Moon"
+        elif phase_angle < 258.75:
+            phase_name = "Waning Gibbous"
+        elif phase_angle < 281.25:
+            phase_name = "Last Quarter"
+        else:
+            phase_name = "Waning Crescent"
+        output = {
+            'phase': phase_name,
+            'sign': self.get_zodiac_sign(moon_longitude),
+            'house': self.point_in_house(moon_longitude)
+        }
+        return output
+
     def point_in_house(self, point_long):
         for house in self.user.houses_list:
             lower_bound = house['abs_pos']
             upper_bound = house['abs_pos'] + 30
             if lower_bound <= point_long < upper_bound:
                 return house['name']
```

### Comparing `py_astrolab-0.6.1/py_astrolab/types.py` & `py_astrolab-0.6.2/py_astrolab/types.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/py_astrolab/utilities.py` & `py_astrolab-0.6.2/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.1/pyproject.toml` & `py_astrolab-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.6.1"
+version = "0.6.2"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.6.1/PKG-INFO` & `py_astrolab-0.6.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

