# Comparing `tmp/py_astrolab-0.6.2.tar.gz` & `tmp/py_astrolab-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.6.2.tar", max compression
+gzip compressed data, was "py_astrolab-0.6.4.tar", max compression
```

## Comparing `py_astrolab-0.6.2.tar` & `py_astrolab-0.6.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.2/README.md
--rwxr-xr-x   0        0        0     4901 2023-08-01 09:27:23.596932 py_astrolab-0.6.2/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    15760 2023-07-30 15:40:50.145067 py_astrolab-0.6.2/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.2/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    80380 2023-07-29 10:08:55.050610 py_astrolab-0.6.2/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.2/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.2/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.2/py_astrolab/charts/templates/minimal.xml
--rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.2/py_astrolab/charts/wonderful_mistake.py
--rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.2/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12935 2023-07-27 22:22:27.571322 py_astrolab-0.6.2/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.2/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.2/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.2/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.2/py_astrolab/report.py
--rwxr-xr-x   0        0        0    20501 2023-08-02 09:40:02.508864 py_astrolab-0.6.2/py_astrolab/transits.py
--rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.2/py_astrolab/types.py
--rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.2/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      664 2023-08-02 09:40:58.962869 py_astrolab-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.2/PKG-INFO
+-rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.4/README.md
+-rwxr-xr-x   0        0        0     4901 2023-08-01 09:27:23.596932 py_astrolab-0.6.4/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    15760 2023-07-30 15:40:50.145067 py_astrolab-0.6.4/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.4/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    80380 2023-07-29 10:08:55.050610 py_astrolab-0.6.4/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.4/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.4/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.4/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.4/py_astrolab/charts/wonderful_mistake.py
+-rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.4/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12935 2023-07-27 22:22:27.571322 py_astrolab-0.6.4/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.4/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.4/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.4/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.4/py_astrolab/report.py
+-rwxr-xr-x   0        0        0    17933 2023-08-02 17:08:55.626774 py_astrolab-0.6.4/py_astrolab/transits.py
+-rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.4/py_astrolab/types.py
+-rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.4/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      664 2023-08-02 17:16:47.356398 py_astrolab-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.4/PKG-INFO
```

### Comparing `py_astrolab-0.6.2/py_astrolab/__init__.py` & `py_astrolab-0.6.4/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/aspects.py` & `py_astrolab-0.6.4/py_astrolab/aspects.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.6.4/py_astrolab/charts/charts_svg.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.6.4/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.6.4/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.6.4/py_astrolab/charts/templates/minimal.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/charts/wonderful_mistake.py` & `py_astrolab-0.6.4/py_astrolab/charts/wonderful_mistake.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/fetch_geonames.py` & `py_astrolab-0.6.4/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/kr.config.json` & `py_astrolab-0.6.4/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/main.py` & `py_astrolab-0.6.4/py_astrolab/main.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/print_all_data.py` & `py_astrolab-0.6.4/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/relationship_score.py` & `py_astrolab-0.6.4/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/report.py` & `py_astrolab-0.6.4/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/transits.py` & `py_astrolab-0.6.4/py_astrolab/transits.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,43 +19,45 @@
         self.settings = settings
         self.natal_aspects_changes = {}
         self.transit_aspects_changes = {}
         self.previous_natal_aspects = None
         self.previous_transit_aspects = None
 
         self.planets = range(swe.SUN, swe.SATURN)
-        self.aspects = [0, 60, 90, 120, 180]
+        self.aspects = [0, 30, 60, 90, 120, 150, 180]
         self.planet_names = {
             swe.SUN: {'name': 'Sun', 'orbit': 3, 'interval': timedelta(minutes=5)}, # 6 giorni in aspetto
             # 365 giorni / 360 gradi = 1 giorni per grado
             # 3 gradi di orbita * 2 * 1 giorni = 6 giorni in aspetto
             swe.MOON: {'name': 'Moon','orbit': 1, 'interval': timedelta(minutes=5)}, # 3,6 ore in aspetto
             # 27.3 giorni / 360 gradi = 1 ora e 49 minuti per grado (109 minuti)
             # 1 gradi di orbita * 2 * 1 ora e 49 minuti = 3,6 ore
             swe.MERCURY: {'name': 'Mercury','orbit': 3, 'interval': timedelta(hours=1)}, # 1,5 giorni in aspetto
             # 88 giorni / 360 gradi = 5,9 ore per grado (351 minuti)
             # 3 gradi di orbita * 2 * 5,9 ore = 1,5 giorni
             swe.VENUS: {'name': 'Venus','orbit': 3, 'interval': timedelta(hours=1)}, # 3,75 giorni in aspetto
             # 225 giorni / 360 gradi = 15 ore per grado
             # 3 gradi di orbita * 2 * 15 ore = 3,75 giorni
-            swe.MARS: {'name': 'Mars','orbit': 5, 'interval': timedelta(hours=1)}, # 38 giorni
+            swe.MARS: {'name': 'Mars','orbit': 5, 'interval': timedelta(hours=1)}, # 20 giorni
             # 687 giorni / 360 gradi = 1.9 giorni per grado (45,6 ore)
-            # 5 gradi di orbita * 2 * 1.9 giorni = 38 giorni
+            # 5 gradi di orbita * 2 * 1.9 giorni = 20 giorni
             swe.JUPITER: {'name': 'Jupiter','orbit': 5, 'interval': timedelta(hours=1)}, # 4 mesi in aspetto
             # (11.86 anni * 365.25 giorni/anno) / 360 gradi = 12 giorni per grado
             # 5 gradi di orbita * 2 * 12 giorni = 120 giorni (4 mesi)
             swe.SATURN: {'name': 'Saturn','orbit': 5, 'interval': timedelta(days=1)} # 10 mesi
             # (29.5 anni * 365.25 giorni/anno) / 360 gradi = 30 giorni per grado
             # 5 gradi di orbita * 2 * 30 giorni = 300 giorni (10 mesi)
         }
         self.aspect_names = {
             0: 'conjunction',
+            30: 'semi-sextile',
             60: 'sextile',
             90: 'square',
             120: 'trine',
+            150: 'quincunx',
             180: 'opposition',
         }
         self.julday_cache = dict()
         self.long_cache = dict()
         self.times, self.positions = self.calculate_positions()
         self.orb_cache = dict()
     
@@ -74,23 +76,18 @@
         lon1 = self.calc_long(jd, planet1)
         lon2 = self.calc_long(jd, planet2) if not natal_planet_orb else natal_planet_orb
         angle = self.angle_difference(lon1, lon2)
         orb = abs(abs(angle) - aspect)
         self.orb_cache[cache_tuple] = orb
         return orb
 
-    def aspects_transits_transits(self, look_for_planets=None, activation_only=False):
-        look_for_planets = set(self.planet_names.keys()) if look_for_planets is None else look_for_planets
-        aspects = self.find_transit_transit_aspects(self.times, self.positions, look_for_planets, activation_only)
-        return aspects
-
-    def aspects_natal_transits(self, look_for_planets = None, activation_only=False):
+    def find_aspects(self, look_for_planets, waxing_only, waning_only):
         look_for_planets = set(self.planet_names.keys()) if look_for_planets is None else look_for_planets
         natal_positions = {planet_data['name']: planet_data['abs_pos'] for planet_data in self.user.planets_list}
-        aspects = self.find_natal_transit_aspects(self.times, self.positions, natal_positions, look_for_planets, activation_only)
+        aspects = self.__find_aspects(self.times, self.positions, natal_positions, look_for_planets, waxing_only, waning_only)
         return aspects
 
     def angle_difference(self, angle1, angle2):
         return 180 - abs(abs(angle1 - angle2) - 180)
 
     def jd_to_datetime(self, jd):
         if jd in self.julday_cache:
@@ -189,95 +186,65 @@
         for time in times:
             jd = self.datetime_to_jd(time)
             for planet in self.planets:
                 lon = self.calc_long(jd, planet)
                 positions[planet].append(lon)
         return times, positions
 
-    def find_transit_transit_aspects(self, times, positions, look_for_planets, activation_only):
-        aspects = {}
-        current_aspects = set()
-        for planet1, planet2 in combinations(self.planets, 2):
-            if planet1 not in look_for_planets:
-                continue
-            orbit_tolerance = min(self.planet_names[planet1]['orbit'], self.planet_names[planet2]['orbit'])
-            interval = min(self.planet_names[planet1]['interval'], self.planet_names[planet2]['interval'])
-            for time1, time2, lon1_1, lon1_2, lon2_1, lon2_2 in zip(times, times[1:], positions[planet1], positions[planet1][1:], positions[planet2], positions[planet2][1:]):
-                for a in self.aspects:
-                    p1_name = self.planet_names[planet1]['name']
-                    p2_name = self.planet_names[planet2]['name']
-                    aspect_name = self.aspect_names[a]
-                    aspect_tuple = (p1_name, p2_name, aspect_name)
-                    diff1 = self.angle_difference(lon1_1, lon2_1)
-                    diff2 = self.angle_difference(lon1_2, lon2_2)
-                    if ((diff1 - a) * (diff2 - a) <= 0) or (abs(diff1 - a) <= orbit_tolerance) or (abs(diff2 - a) <= orbit_tolerance):
-                        if aspect_tuple not in current_aspects:
-                            if time1 == self.start and not activation_only:
-                                start_time, orb = self.backward_binary_search(planet1, planet2, a, orbit_tolerance, None, interval)
-                            else:
-                                start_time, orb = self.binary_search(time1, time2, planet1, planet2, a, orbit_tolerance, None)
-                                start_time = start_time if abs(orb - orbit_tolerance) < 0.1 else None
-                            if activation_only:
-                                finish_time = None
-                            else:
-                                finish_time, _ = self.forward_binary_search(planet1, planet2, a, orbit_tolerance, start_time, None, interval)
-                            if start_time is not None:
-                                p1_sign = self.get_zodiac_sign(self.calc_long(self.datetime_to_jd(start_time), planet1))
-                                p2_sign = self.get_zodiac_sign(self.calc_long(self.datetime_to_jd(start_time), planet2))
-                                duration = finish_time-start_time if finish_time is not None else None
-                                aspect_dict = {'p1_name': p1_name, 'p2_name': p2_name, 'p1_sign': p1_sign, 'p2_sign': p2_sign, 'aspect': aspect_name, 'start': start_time, 'finish': finish_time, 'duration': duration, 'orb': orb}
-                                aspects.setdefault(start_time, []).append(aspect_dict)
-                            current_aspects.add(aspect_tuple)
-                    else:
-                        current_aspects.discard(aspect_tuple)
-        return aspects
-
-    def find_natal_transit_aspects(self, times, positions, natal_positions, look_for_planets, activation_only):
+    def __find_aspects(self, times, positions, natal_positions, look_for_planets, waxing_only, waning_only):
         aspects = {}
         current_aspects = set()
         for planet1, planet2 in product(self.planets, natal_positions.keys()):
             if planet1 not in look_for_planets:
                 continue
             planet2_number = next((planet for planet, info in self.planet_names.items() if info['name'] == planet2), None)
-            interval = self.planet_names[planet1]['interval']
             if planet2_number is None:
                 continue
+            interval = self.planet_names[planet1]['interval']
             orbit_tolerance = self.planet_names[planet1]['orbit']
             natal_position = natal_positions[planet2]
             for time1, time2, lon1_1, lon1_2 in zip(times, times[1:], positions[planet1], positions[planet1][1:]):
                 for a in self.aspects:
                     p1_name = self.planet_names[planet1]['name']
                     p2_name = planet2
                     aspect_name = self.aspect_names[a]
                     aspect_tuple = (p1_name, p2_name, aspect_name)
                     diff1 = self.angle_difference(lon1_1, natal_position)
                     diff2 = self.angle_difference(lon1_2, natal_position)
-                    if ((diff1 - a) * (diff2 - a) <= 0) or (abs(diff1 - a) <= orbit_tolerance) or (abs(diff2 - a) <= orbit_tolerance):
-                        if aspect_tuple not in current_aspects:
-                            if time1 == self.start and not activation_only:
-                                start_time, orb = self.backward_binary_search(planet1, planet2_number, a, orbit_tolerance, natal_position, interval)
-                            else:
-                                start_time, orb = self.binary_search(time1, time2, planet1, planet2_number, a, orbit_tolerance, natal_position)
-                                start_time = start_time if abs(orb - orbit_tolerance) < 0.1 else None
-                            if activation_only:
-                                finish_time = None
-                            else:
-                                finish_time, _ = self.forward_binary_search(planet1, planet2_number, a, orbit_tolerance, start_time, natal_position, interval)
-                            if start_time:
-                                p1_long = self.calc_long(self.datetime_to_jd(start_time), planet1)
-                                p1_sign = self.get_zodiac_sign(p1_long)
-                                p2_sign = getattr(self.user, p2_name.lower())['signs'][0]
-                                p1_house = self.point_in_house(p1_long)
-                                p2_house = getattr(self.user, p2_name.lower())['house']
-                                duration = finish_time-start_time if finish_time is not None else None
-                                aspect_dict = {'p1_name': p1_name, 'p2_name': p2_name, 'p1_sign': p1_sign, 'p2_sign': p2_sign, 'p1_house': p1_house, 'p2_house': p2_house, 'aspect': aspect_name, 'start': start_time, 'finish': finish_time, 'duration': duration, 'orb': orb}
-                                aspects.setdefault(start_time, []).append(aspect_dict)
-                            current_aspects.add(aspect_tuple)
-                    else:
-                        current_aspects.discard(aspect_tuple)
+                    if not ((diff1 - a) * (diff2 - a) <= 0) and not (abs(diff1 - a) <= orbit_tolerance) and not (abs(diff2 - a) <= orbit_tolerance):
+                        current_aspects.discard((self.planet_names[planet1]['name'], planet2, self.aspect_names[a]))
+                        continue
+                    aspect_tuple = (self.planet_names[planet1]['name'], planet2, self.aspect_names[a])
+                    if aspect_tuple in current_aspects:
+                        continue
+                    start_time, start_orb = None, None
+                    if time1 == self.start and not waxing_only and not waning_only:
+                        start_time, start_orb = self.backward_binary_search(planet1, planet2_number, a, orbit_tolerance, natal_position, interval)
+                    elif not waning_only:
+                        start_time, start_orb = self.binary_search(time1, time2, planet1, planet2_number, a, orbit_tolerance, natal_position)
+                        if waxing_only and abs(start_orb - orbit_tolerance) >= 0.1:
+                            start_time = None
+                    finish_time = None if waxing_only or waning_only else self.forward_binary_search(planet1, planet2_number, a, orbit_tolerance, start_time, natal_position, interval)[0]
+                    exact_time, exact_orb = (self.binary_search(self.start, self.end, planet1, planet2_number, a, 0, natal_position) if waning_only else (None, None))
+                    if waning_only and exact_orb >= 0.1:
+                        exact_time = None
+                    if start_time or exact_time:
+                        if start_time:
+                            p1_long = self.calc_long(self.datetime_to_jd(start_time), planet1)
+                            duration = finish_time-start_time if finish_time is not None else None
+                        elif exact_time:
+                            p1_long = self.calc_long(self.datetime_to_jd(exact_time), planet1)
+                            duration = None
+                        p1_sign = self.get_zodiac_sign(p1_long)
+                        p2_sign = getattr(self.user, p2_name.lower())['signs'][0]
+                        p1_house = self.point_in_house(p1_long)
+                        p2_house = getattr(self.user, p2_name.lower())['house']   
+                        aspect_dict = {'p1_name': p1_name, 'p2_name': p2_name, 'p1_sign': p1_sign, 'p2_sign': p2_sign, 'p1_house': p1_house, 'p2_house': p2_house, 'aspect': aspect_name, 'start': start_time, 'exact': exact_time, 'finish': finish_time, 'duration': duration, 'start_orb': start_orb, 'exact_orb': exact_orb}
+                        aspects.setdefault(start_time, []).append(aspect_dict)
+                    current_aspects.add(aspect_tuple)
         return aspects
 
     def get_zodiac_sign(self, lon):
         signs = ['Ari', 'Tau', 'Gem', 'Can', 'Leo', 'Vir', 
                 'Lib', 'Sco', 'Sag', 'Cap', 'Aqu', 'Pis']
         return signs[int(lon // 30)]
```

### Comparing `py_astrolab-0.6.2/py_astrolab/types.py` & `py_astrolab-0.6.4/py_astrolab/types.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/py_astrolab/utilities.py` & `py_astrolab-0.6.4/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.2/pyproject.toml` & `py_astrolab-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.6.2"
+version = "0.6.4"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.6.2/PKG-INFO` & `py_astrolab-0.6.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.6.2
+Version: 0.6.4
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

