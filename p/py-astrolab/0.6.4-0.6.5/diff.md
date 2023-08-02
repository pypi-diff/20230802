# Comparing `tmp/py_astrolab-0.6.4.tar.gz` & `tmp/py_astrolab-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.6.4.tar", max compression
+gzip compressed data, was "py_astrolab-0.6.5.tar", max compression
```

## Comparing `py_astrolab-0.6.4.tar` & `py_astrolab-0.6.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.4/README.md
--rwxr-xr-x   0        0        0     4901 2023-08-01 09:27:23.596932 py_astrolab-0.6.4/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    15760 2023-07-30 15:40:50.145067 py_astrolab-0.6.4/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.4/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    80380 2023-07-29 10:08:55.050610 py_astrolab-0.6.4/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.4/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.4/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.4/py_astrolab/charts/templates/minimal.xml
--rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.4/py_astrolab/charts/wonderful_mistake.py
--rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.4/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12935 2023-07-27 22:22:27.571322 py_astrolab-0.6.4/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.4/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.4/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.4/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.4/py_astrolab/report.py
--rwxr-xr-x   0        0        0    17933 2023-08-02 17:08:55.626774 py_astrolab-0.6.4/py_astrolab/transits.py
--rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.4/py_astrolab/types.py
--rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.4/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      664 2023-08-02 17:16:47.356398 py_astrolab-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.4/PKG-INFO
+-rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.5/README.md
+-rwxr-xr-x   0        0        0     4901 2023-08-01 09:27:23.596932 py_astrolab-0.6.5/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    15760 2023-07-30 15:40:50.145067 py_astrolab-0.6.5/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.5/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    80380 2023-07-29 10:08:55.050610 py_astrolab-0.6.5/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.5/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.5/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.5/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.5/py_astrolab/charts/wonderful_mistake.py
+-rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.5/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12935 2023-07-27 22:22:27.571322 py_astrolab-0.6.5/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.5/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.5/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.5/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.5/py_astrolab/report.py
+-rwxr-xr-x   0        0        0    18590 2023-08-02 17:25:56.651200 py_astrolab-0.6.5/py_astrolab/transits.py
+-rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.5/py_astrolab/types.py
+-rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.5/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      664 2023-08-02 17:27:48.299087 py_astrolab-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.5/PKG-INFO
```

### Comparing `py_astrolab-0.6.4/py_astrolab/__init__.py` & `py_astrolab-0.6.5/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/aspects.py` & `py_astrolab-0.6.5/py_astrolab/aspects.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.6.5/py_astrolab/charts/charts_svg.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.6.5/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.6.5/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.6.5/py_astrolab/charts/templates/minimal.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/charts/wonderful_mistake.py` & `py_astrolab-0.6.5/py_astrolab/charts/wonderful_mistake.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/fetch_geonames.py` & `py_astrolab-0.6.5/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/kr.config.json` & `py_astrolab-0.6.5/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/main.py` & `py_astrolab-0.6.5/py_astrolab/main.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/print_all_data.py` & `py_astrolab-0.6.5/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/relationship_score.py` & `py_astrolab-0.6.5/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/report.py` & `py_astrolab-0.6.5/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/transits.py` & `py_astrolab-0.6.5/py_astrolab/transits.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             jd = self.datetime_to_jd(time)
             for planet in self.planets:
                 lon = self.calc_long(jd, planet)
                 positions[planet].append(lon)
         return times, positions
 
     def __find_aspects(self, times, positions, natal_positions, look_for_planets, waxing_only, waning_only):
-        aspects = {}
+        aspect_list = [] 
         current_aspects = set()
         for planet1, planet2 in product(self.planets, natal_positions.keys()):
             if planet1 not in look_for_planets:
                 continue
             planet2_number = next((planet for planet, info in self.planet_names.items() if info['name'] == planet2), None)
             if planet2_number is None:
                 continue
@@ -234,18 +234,37 @@
                         elif exact_time:
                             p1_long = self.calc_long(self.datetime_to_jd(exact_time), planet1)
                             duration = None
                         p1_sign = self.get_zodiac_sign(p1_long)
                         p2_sign = getattr(self.user, p2_name.lower())['signs'][0]
                         p1_house = self.point_in_house(p1_long)
                         p2_house = getattr(self.user, p2_name.lower())['house']   
-                        aspect_dict = {'p1_name': p1_name, 'p2_name': p2_name, 'p1_sign': p1_sign, 'p2_sign': p2_sign, 'p1_house': p1_house, 'p2_house': p2_house, 'aspect': aspect_name, 'start': start_time, 'exact': exact_time, 'finish': finish_time, 'duration': duration, 'start_orb': start_orb, 'exact_orb': exact_orb}
-                        aspects.setdefault(start_time, []).append(aspect_dict)
+                        aspect_dict = {
+                            'p1_name': p1_name,
+                            'p2_name': p2_name,
+                            'p1_sign': p1_sign,
+                            'p2_sign': p2_sign,
+                            'p1_house': p1_house,
+                            'p2_house': p2_house,
+                            'aspect': aspect_name,
+                            'start': start_time,
+                            'exact': exact_time,
+                            'finish': finish_time,
+                            'duration': duration,
+                            'start_orb': start_orb,
+                            'exact_orb': exact_orb
+                        }
+                        if waning_only:
+                            if exact_time:
+                                aspect_list.append(aspect_dict)
+                        else:
+                            aspect_list.append(aspect_dict)
                     current_aspects.add(aspect_tuple)
-        return aspects
+        aspect_list.sort(key=lambda x: x['start'] if x['start'] else x['exact'])
+        return aspect_list
 
     def get_zodiac_sign(self, lon):
         signs = ['Ari', 'Tau', 'Gem', 'Can', 'Leo', 'Vir', 
                 'Lib', 'Sco', 'Sag', 'Cap', 'Aqu', 'Pis']
         return signs[int(lon // 30)]
 
     def calculate_transitions(self):
```

### Comparing `py_astrolab-0.6.4/py_astrolab/types.py` & `py_astrolab-0.6.5/py_astrolab/types.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/py_astrolab/utilities.py` & `py_astrolab-0.6.5/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.4/pyproject.toml` & `py_astrolab-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.6.4"
+version = "0.6.5"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.6.4/PKG-INFO` & `py_astrolab-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.6.4
+Version: 0.6.5
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

