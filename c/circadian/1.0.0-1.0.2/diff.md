# Comparing `tmp/circadian-1.0.0.tar.gz` & `tmp/circadian-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circadian-1.0.0.tar", last modified: Wed Jul 26 14:13:40 2023, max compression
+gzip compressed data, was "circadian-1.0.2.tar", last modified: Wed Aug  2 00:18:52 2023, max compression
```

## Comparing `circadian-1.0.0.tar` & `circadian-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:40.611133 circadian-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-26 14:13:28.000000 circadian-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 14:13:28.000000 circadian-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-07-26 14:13:40.611133 circadian-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-26 14:13:28.000000 circadian-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:40.611133 circadian-1.0.0/circadian/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37330 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23484 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/lights.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    42836 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/phasetools.py
--rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/prc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25459 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:40.611133 circadian-1.0.0/circadian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-26 14:13:28.000000 circadian-1.0.0/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:13:40.611133 circadian-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-26 14:13:28.000000 circadian-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:18:52.061050 circadian-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-02 00:18:42.000000 circadian-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 00:18:42.000000 circadian-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-08-02 00:18:52.061050 circadian-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-08-02 00:18:42.000000 circadian-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:18:52.061050 circadian-1.0.2/circadian/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 00:18:42.000000 circadian-1.0.2/circadian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32709 2023-08-02 00:18:42.000000 circadian-1.0.2/circadian/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-08-02 00:18:42.000000 circadian-1.0.2/circadian/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23484 2023-08-02 00:18:42.000000 circadian-1.0.2/circadian/lights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-08-02 00:18:42.000000 circadian-1.0.2/circadian/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49868 2023-08-02 00:18:42.000000 circadian-1.0.2/circadian/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-02 00:18:42.000000 circadian-1.0.2/circadian/phasetools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-08-02 00:18:42.000000 circadian-1.0.2/circadian/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-08-02 00:18:42.000000 circadian-1.0.2/circadian/prc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-08-02 00:18:42.000000 circadian-1.0.2/circadian/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-08-02 00:18:42.000000 circadian-1.0.2/circadian/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-08-02 00:18:42.000000 circadian-1.0.2/circadian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:18:52.061050 circadian-1.0.2/circadian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-08-02 00:18:52.000000 circadian-1.0.2/circadian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-02 00:18:52.000000 circadian-1.0.2/circadian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:18:52.000000 circadian-1.0.2/circadian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-02 00:18:52.000000 circadian-1.0.2/circadian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:18:51.000000 circadian-1.0.2/circadian.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 00:18:52.000000 circadian-1.0.2/circadian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 00:18:52.000000 circadian-1.0.2/circadian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 00:18:42.000000 circadian-1.0.2/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:18:52.061050 circadian-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-08-02 00:18:42.000000 circadian-1.0.2/setup.py
```

### Comparing `circadian-1.0.0/LICENSE` & `circadian-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `circadian-1.0.0/PKG-INFO` & `circadian-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circadian
-Version: 1.0.0
+Version: 1.0.2
 Summary: Tools for the simulation and analysis of circadian rhythms
 Home-page: https://github.com/Arcascope/circadian
 Author: Arcascope Inc.
 Author-email: support@arcascope.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `circadian-1.0.0/README.md` & `circadian-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `circadian-1.0.0/circadian/_modidx.py` & `circadian-1.0.2/circadian/_modidx.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,16 +25,15 @@
                                   'circadian.lights.LightSchedule.__sub__': ( 'api/lights.html#lightschedule.__sub__',
                                                                               'circadian/lights.py'),
                                   'circadian.lights.LightSchedule.concatenate_at': ( 'api/lights.html#lightschedule.concatenate_at',
                                                                                      'circadian/lights.py'),
                                   'circadian.lights.LightSchedule.from_pulse': ( 'api/lights.html#lightschedule.from_pulse',
                                                                                  'circadian/lights.py'),
                                   'circadian.lights.LightSchedule.plot': ('api/lights.html#lightschedule.plot', 'circadian/lights.py')},
-            'circadian.metrics': { 'circadian.metrics.esri': ('api/metrics.html#esri', 'circadian/metrics.py'),
-                                   'circadian.metrics.esri_trajectory': ('api/metrics.html#esri_trajectory', 'circadian/metrics.py')},
+            'circadian.metrics': {'circadian.metrics.esri': ('api/metrics.html#esri', 'circadian/metrics.py')},
             'circadian.models': { 'circadian.models.CircadianModel': ('api/models.html#circadianmodel', 'circadian/models.py'),
                                   'circadian.models.CircadianModel.__call__': ( 'api/models.html#circadianmodel.__call__',
                                                                                 'circadian/models.py'),
                                   'circadian.models.CircadianModel.__init__': ( 'api/models.html#circadianmodel.__init__',
                                                                                 'circadian/models.py'),
                                   'circadian.models.CircadianModel._default_initial_condition': ( 'api/models.html#circadianmodel._default_initial_condition',
                                                                                                   'circadian/models.py'),
@@ -103,14 +102,24 @@
                                   'circadian.models.Hannay19TP.__str__': ('api/models.html#hannay19tp.__str__', 'circadian/models.py'),
                                   'circadian.models.Hannay19TP.amplitude': ('api/models.html#hannay19tp.amplitude', 'circadian/models.py'),
                                   'circadian.models.Hannay19TP.cbt': ('api/models.html#hannay19tp.cbt', 'circadian/models.py'),
                                   'circadian.models.Hannay19TP.derv': ('api/models.html#hannay19tp.derv', 'circadian/models.py'),
                                   'circadian.models.Hannay19TP.dlmos': ('api/models.html#hannay19tp.dlmos', 'circadian/models.py'),
                                   'circadian.models.Hannay19TP.integrate': ('api/models.html#hannay19tp.integrate', 'circadian/models.py'),
                                   'circadian.models.Hannay19TP.phase': ('api/models.html#hannay19tp.phase', 'circadian/models.py'),
+                                  'circadian.models.Hilaire07': ('api/models.html#hilaire07', 'circadian/models.py'),
+                                  'circadian.models.Hilaire07.__init__': ('api/models.html#hilaire07.__init__', 'circadian/models.py'),
+                                  'circadian.models.Hilaire07.__repr__': ('api/models.html#hilaire07.__repr__', 'circadian/models.py'),
+                                  'circadian.models.Hilaire07.__str__': ('api/models.html#hilaire07.__str__', 'circadian/models.py'),
+                                  'circadian.models.Hilaire07.amplitude': ('api/models.html#hilaire07.amplitude', 'circadian/models.py'),
+                                  'circadian.models.Hilaire07.cbt': ('api/models.html#hilaire07.cbt', 'circadian/models.py'),
+                                  'circadian.models.Hilaire07.derv': ('api/models.html#hilaire07.derv', 'circadian/models.py'),
+                                  'circadian.models.Hilaire07.dlmos': ('api/models.html#hilaire07.dlmos', 'circadian/models.py'),
+                                  'circadian.models.Hilaire07.integrate': ('api/models.html#hilaire07.integrate', 'circadian/models.py'),
+                                  'circadian.models.Hilaire07.phase': ('api/models.html#hilaire07.phase', 'circadian/models.py'),
                                   'circadian.models.Jewett99': ('api/models.html#jewett99', 'circadian/models.py'),
                                   'circadian.models.Jewett99.__init__': ('api/models.html#jewett99.__init__', 'circadian/models.py'),
                                   'circadian.models.Jewett99.__repr__': ('api/models.html#jewett99.__repr__', 'circadian/models.py'),
                                   'circadian.models.Jewett99.__str__': ('api/models.html#jewett99.__str__', 'circadian/models.py'),
                                   'circadian.models.Jewett99.amplitude': ('api/models.html#jewett99.amplitude', 'circadian/models.py'),
                                   'circadian.models.Jewett99.cbt': ('api/models.html#jewett99.cbt', 'circadian/models.py'),
                                   'circadian.models.Jewett99.derv': ('api/models.html#jewett99.derv', 'circadian/models.py'),
@@ -195,82 +204,33 @@
                                                                                           'circadian/prc.py'),
                                'circadian.prc.RimmerLightPulseLight.pulse_rimmer_start': ( 'api/prc.html#rimmerlightpulselight.pulse_rimmer_start',
                                                                                            'circadian/prc.py'),
                                'circadian.prc.get_pulse': ('api/prc.html#get_pulse', 'circadian/prc.py'),
                                'circadian.prc.heaviside': ('api/prc.html#heaviside', 'circadian/prc.py'),
                                'circadian.prc.make_pulse': ('api/prc.html#make_pulse', 'circadian/prc.py')},
             'circadian.readers': { 'circadian.readers.WearableData': ('api/readers.html#wearabledata', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.__getitem__': ( 'api/readers.html#wearabledata.__getitem__',
-                                                                                   'circadian/readers.py'),
-                                   'circadian.readers.WearableData.__post_init__': ( 'api/readers.html#wearabledata.__post_init__',
-                                                                                     'circadian/readers.py'),
-                                   'circadian.readers.WearableData._copy_with_metadata': ( 'api/readers.html#wearabledata._copy_with_metadata',
-                                                                                           'circadian/readers.py'),
-                                   'circadian.readers.WearableData.activity': ( 'api/readers.html#wearabledata.activity',
+                                   'circadian.readers.WearableData.__init__': ( 'api/readers.html#wearabledata.__init__',
                                                                                 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.aggregate': ( 'api/readers.html#wearabledata.aggregate',
-                                                                                 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.build_sleep_chunks': ( 'api/readers.html#wearabledata.build_sleep_chunks',
+                                   'circadian.readers.WearableData._validate_columns': ( 'api/readers.html#wearabledata._validate_columns',
+                                                                                         'circadian/readers.py'),
+                                   'circadian.readers.WearableData._validate_metadata': ( 'api/readers.html#wearabledata._validate_metadata',
                                                                                           'circadian/readers.py'),
-                                   'circadian.readers.WearableData.date_bounds': ( 'api/readers.html#wearabledata.date_bounds',
-                                                                                   'circadian/readers.py'),
-                                   'circadian.readers.WearableData.datetime': ( 'api/readers.html#wearabledata.datetime',
-                                                                                'circadian/readers.py'),
-                                   'circadian.readers.WearableData.fillna': ( 'api/readers.html#wearabledata.fillna',
-                                                                              'circadian/readers.py'),
-                                   'circadian.readers.WearableData.filter': ( 'api/readers.html#wearabledata.filter',
-                                                                              'circadian/readers.py'),
-                                   'circadian.readers.WearableData.from_json': ( 'api/readers.html#wearabledata.from_json',
-                                                                                 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.get_date': ( 'api/readers.html#wearabledata.get_date',
+                                   'circadian.readers.WearableData.add_metadata': ( 'api/readers.html#wearabledata.add_metadata',
+                                                                                    'circadian/readers.py'),
+                                   'circadian.readers.WearableData.is_valid': ( 'api/readers.html#wearabledata.is_valid',
                                                                                 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.get_timestamp': ( 'api/readers.html#wearabledata.get_timestamp',
-                                                                                     'circadian/readers.py'),
-                                   'circadian.readers.WearableData.groupby': ( 'api/readers.html#wearabledata.groupby',
-                                                                               'circadian/readers.py'),
-                                   'circadian.readers.WearableData.head': ('api/readers.html#wearabledata.head', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.heartrate': ( 'api/readers.html#wearabledata.heartrate',
-                                                                                 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.join': ('api/readers.html#wearabledata.join', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.light_estimate': ( 'api/readers.html#wearabledata.light_estimate',
+                                   'circadian.readers.WearableData.rename_columns': ( 'api/readers.html#wearabledata.rename_columns',
                                                                                       'circadian/readers.py'),
-                                   'circadian.readers.WearableData.plot_heartrate': ( 'api/readers.html#wearabledata.plot_heartrate',
+                                   'circadian.readers.combine_wearable_dataframes': ( 'api/readers.html#combine_wearable_dataframes',
                                                                                       'circadian/readers.py'),
-                                   'circadian.readers.WearableData.plot_hr_steps': ( 'api/readers.html#wearabledata.plot_hr_steps',
-                                                                                     'circadian/readers.py'),
-                                   'circadian.readers.WearableData.plot_light_activity': ( 'api/readers.html#wearabledata.plot_light_activity',
-                                                                                           'circadian/readers.py'),
-                                   'circadian.readers.WearableData.scatter_hr_steps': ( 'api/readers.html#wearabledata.scatter_hr_steps',
-                                                                                        'circadian/readers.py'),
-                                   'circadian.readers.WearableData.steps': ('api/readers.html#wearabledata.steps', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.steps_hr_loglinear': ( 'api/readers.html#wearabledata.steps_hr_loglinear',
-                                                                                          'circadian/readers.py'),
-                                   'circadian.readers.WearableData.tail': ('api/readers.html#wearabledata.tail', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.time_hour_bounds': ( 'api/readers.html#wearabledata.time_hour_bounds',
-                                                                                        'circadian/readers.py'),
-                                   'circadian.readers.WearableData.time_total': ( 'api/readers.html#wearabledata.time_total',
-                                                                                  'circadian/readers.py'),
-                                   'circadian.readers.WearableData.timestamp': ( 'api/readers.html#wearabledata.timestamp',
-                                                                                 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.to_json': ( 'api/readers.html#wearabledata.to_json',
-                                                                               'circadian/readers.py'),
-                                   'circadian.readers.WearableData.trim_by_hour': ( 'api/readers.html#wearabledata.trim_by_hour',
-                                                                                    'circadian/readers.py'),
-                                   'circadian.readers.WearableData.trim_by_idx': ( 'api/readers.html#wearabledata.trim_by_idx',
-                                                                                   'circadian/readers.py'),
-                                   'circadian.readers.WearableData.trim_by_timestamp': ( 'api/readers.html#wearabledata.trim_by_timestamp',
-                                                                                         'circadian/readers.py'),
-                                   'circadian.readers.WearableData.utc_to_hrs': ( 'api/readers.html#wearabledata.utc_to_hrs',
-                                                                                  'circadian/readers.py'),
-                                   'circadian.readers.WearableData.wake': ('api/readers.html#wearabledata.wake', 'circadian/readers.py'),
-                                   'circadian.readers.combine_wearable_streams': ( 'api/readers.html#combine_wearable_streams',
-                                                                                   'circadian/readers.py'),
-                                   'circadian.readers.read_actiwatch': ('api/readers.html#read_actiwatch', 'circadian/readers.py'),
-                                   'circadian.readers.read_standard_csv': ('api/readers.html#read_standard_csv', 'circadian/readers.py'),
-                                   'circadian.readers.read_standard_json': ('api/readers.html#read_standard_json', 'circadian/readers.py')},
+                                   'circadian.readers.interval_fraction': ('api/readers.html#interval_fraction', 'circadian/readers.py'),
+                                   'circadian.readers.load_actiwatch': ('api/readers.html#load_actiwatch', 'circadian/readers.py'),
+                                   'circadian.readers.load_csv': ('api/readers.html#load_csv', 'circadian/readers.py'),
+                                   'circadian.readers.load_json': ('api/readers.html#load_json', 'circadian/readers.py'),
+                                   'circadian.readers.resample_df': ('api/readers.html#resample_df', 'circadian/readers.py')},
             'circadian.sleep': { 'circadian.sleep.TwoProcessModel': ('api/sleep.html#twoprocessmodel', 'circadian/sleep.py'),
                                  'circadian.sleep.TwoProcessModel.__call__': ( 'api/sleep.html#twoprocessmodel.__call__',
                                                                                'circadian/sleep.py'),
                                  'circadian.sleep.TwoProcessModel.__init__': ( 'api/sleep.html#twoprocessmodel.__init__',
                                                                                'circadian/sleep.py'),
                                  'circadian.sleep.TwoProcessModel.check_wake_status': ( 'api/sleep.html#twoprocessmodel.check_wake_status',
                                                                                         'circadian/sleep.py'),
@@ -303,8 +263,9 @@
                                  'circadian.utils.redact_dates': ('api/utils.html#redact_dates', 'circadian/utils.py'),
                                  'circadian.utils.simple_norm_stepshr_sleep_classifier': ( 'api/utils.html#simple_norm_stepshr_sleep_classifier',
                                                                                            'circadian/utils.py'),
                                  'circadian.utils.split_drop_data': ('api/utils.html#split_drop_data', 'circadian/utils.py'),
                                  'circadian.utils.split_missing_data': ('api/utils.html#split_missing_data', 'circadian/utils.py'),
                                  'circadian.utils.subtract_clock_times': ('api/utils.html#subtract_clock_times', 'circadian/utils.py'),
                                  'circadian.utils.times_to_angle': ('api/utils.html#times_to_angle', 'circadian/utils.py'),
-                                 'circadian.utils.timezone_mapper': ('api/utils.html#timezone_mapper', 'circadian/utils.py')}}}
+                                 'circadian.utils.timezone_mapper': ('api/utils.html#timezone_mapper', 'circadian/utils.py'),
+                                 'circadian.utils.utc_to_hrs': ('api/utils.html#utc_to_hrs', 'circadian/utils.py')}}}
```

### Comparing `circadian-1.0.0/circadian/cli.py` & `circadian-1.0.2/circadian/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .metrics import *
 import matplotlib.pyplot as plt
 from .plots import Actogram
 from .models import Hannay19
 from .utils import phase_ic_guess
 from .utils import simple_norm_stepshr_sleep_classifier
 from .sleep import cluster_sleep_periods_scipy, sleep_midpoint
-from .readers import WearableData, read_standard_csv, read_standard_json
+from .readers import load_json, load_csv
 
 mytz = timezone('EST')
 
 # %% ../nbs/api/09_cli.ipynb 6
 def main_acto():
     parser = argparse.ArgumentParser(description="""Make an actogram""")
 
@@ -320,18 +320,18 @@
         len_out = wake_predicted.shape[0]
         wake_predicted = np.hstack((wake_predicted, len(steps) - len_out))
         wake_predicted = np.where(wake_predicted > 0.50, 1.0, 0.0)
         return wake_predicted
 
 
     if args.json:
-        awObj = read_standard_json(args.json)
+        awObj = load_json(args.json)
 
     if args.csv:
-        awObj = read_standard_csv(args.csv)
+        awObj = load_csv(args.csv)
 
     if args.csv or args.json:
         if args.t1 or args.t2:
             t1 = args.t1 or 0
             t2 = args.t2 or np.floor(np.squeeze(awObj.time_total)[-1]/24.0)+1
             awObj.trim_data(t1*24.0, t2*24.0)
         hr = awObj.heartrate
```

### Comparing `circadian-1.0.0/circadian/lights.py` & `circadian-1.0.2/circadian/lights.py`

 * *Files identical despite different names*

### Comparing `circadian-1.0.0/circadian/models.py` & `circadian-1.0.2/circadian/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/api/00_models.ipynb.
 
 # %% auto 0
-__all__ = ['DynamicalTrajectory', 'CircadianModel', 'Forger99', 'Hannay19', 'Hannay19TP', 'Jewett99']
+__all__ = ['DynamicalTrajectory', 'CircadianModel', 'Forger99', 'Hannay19', 'Hannay19TP', 'Jewett99', 'Hilaire07']
 
 # %% ../nbs/api/00_models.ipynb 4
 import warnings
 import numpy as np
 from abc import ABC
 from typing import Tuple
 from scipy.signal import find_peaks
@@ -278,32 +278,34 @@
     @initial_condition.setter
     def initial_condition(self, value):
         self._initial_condition = value
 
 # %% ../nbs/api/00_models.ipynb 20
 @patch_to(CircadianModel)
 def derv(self,
+         t: float, # time
          state: np.ndarray, # dynamical state of the model
          input: np.ndarray, # inputs to the model such as light or wake state
          ) -> np.ndarray:
     "Right-hand-side of the differential equation model with state and light as inputs"
     return NotImplementedError("derv is not implemented for this model")
 
 # %% ../nbs/api/00_models.ipynb 21
 @patch_to(CircadianModel)
 def step_rk4(self,
-            state: np.ndarray, # dynamical state of the model
-            input: np.ndarray, # inputs to the model such as light or wake state
-            dt: float, # step size in hours 
-            ) -> np.ndarray:
+             t: float, # time
+             state: np.ndarray, # dynamical state of the model
+             input: np.ndarray, # inputs to the model such as light or wake state
+             dt: float, # step size in hours 
+             ) -> np.ndarray:
     "Integrate the state of the model for one timestep using a fourth-order Runge-Kutta algorithm. Assumes a constant light value for the time step"
-    k1 = self.derv(state, input)
-    k2 = self.derv(state + k1 * dt / 2.0, input)
-    k3 = self.derv(state + k2 * dt / 2.0, input)
-    k4 = self.derv(state + k3 * dt, input)
+    k1 = self.derv(t, state, input)
+    k2 = self.derv(t, state + k1 * dt / 2.0, input)
+    k3 = self.derv(t, state + k2 * dt / 2.0, input)
+    k4 = self.derv(t, state + k3 * dt, input)
     state = state + (dt / 6.0) * (k1 + 2.0*k2 + 2.0*k3 + k4)
     return state
 
 # %% ../nbs/api/00_models.ipynb 22
 @patch_to(CircadianModel)
 def integrate(self,
               time: np.ndarray, # time points for integration. Time difference between consecutive values determines step size of the solver
@@ -326,17 +328,18 @@
     
     n = len(time)
     sol = np.zeros((n, *initial_condition.shape))
     sol[0,...] = initial_condition
     state = initial_condition
 
     for idx in range(1, n):
-        dt = time[idx] - time[idx-1]
+        t = time[idx]
+        dt = t - time[idx-1]
         input_value = input[idx,...]
-        state = self.step_rk4(state, input_value, dt)
+        state = self.step_rk4(t, state, input_value, dt)
         sol[idx,...] = state
     
     self._trajectory = DynamicalTrajectory(time, sol)
     return self._trajectory
 
 # %% ../nbs/api/00_models.ipynb 23
 @patch_to(CircadianModel)
@@ -425,16 +428,24 @@
     "Calculates a default initial condition by simulating the given model on a 16 hour light, 8 hour darkness schedule until convergence"
     # input checking
     if not isinstance(model, CircadianModel):
         raise TypeError("model must be a CircadianModel")
     model._default_initial_condition = 0.5 * np.ones(model._num_states)
     schedule = LightSchedule.Regular(lights_on=8, lights_off=24)    
     time = np.arange(0.0, 24.0, 0.1)
-    light_input = schedule(time)
-    default_initial_condition = model.equilibrate(time, light_input, num_loops)
+    if model._num_inputs == 1:
+        light_input = schedule(time)
+        default_initial_condition = model.equilibrate(time, light_input, num_loops)
+    elif model._num_inputs == 2:
+        light_input = schedule(time)
+        wake_input = np.zeros_like(light_input)
+        wake_input[light_input > 0] = 0
+        wake_input[light_input == 0] = 1
+        input = np.stack((light_input, wake_input), axis=1)
+        default_initial_condition = model.equilibrate(time, input, num_loops)
     return default_initial_condition
 
 def _check_cbtmin_spacing(
         cbtmin_times: np.ndarray, # array of times when the cbtmin occurs
         min_spacing: float=6.0, # minimum spacing between cbtmin markers
         ) -> bool:
     "Checks if the spacing between cbtmin markers is valid"
@@ -475,14 +486,15 @@
     
     def __str__(self) -> str:
         return "Forger99"
 
 # %% ../nbs/api/00_models.ipynb 33
 @patch_to(Forger99)
 def derv(self, 
+         t: float, # time
          state: np.ndarray, # dynamical state (x, xc, n)
          input: float # light intensity in lux
          ) -> np.ndarray: # derivative of the state
      "Right-hand-side of the differential equation model"
      x = state[0,...]
      xc = state[1,...]
      n = state[2,...]
@@ -609,14 +621,15 @@
     
     def __str__(self) -> str:
         return "Hannay19"
 
 # %% ../nbs/api/00_models.ipynb 41
 @patch_to(Hannay19)
 def derv(self,
+         t: float, # time
          state: np.ndarray, # dynamical state (R, Psi, n)
          input: float # light intensity in lux
          ) -> np.ndarray: # derivative of the state
     "Right-hand-side of the differential equation model"
     R = state[0,...]
     Psi = state[1,...]
     n = state[2,...]
@@ -748,14 +761,15 @@
     
     def __str__(self) -> str:
         return "Hannay19TP"
 
 # %% ../nbs/api/00_models.ipynb 49
 @patch_to(Hannay19TP)
 def derv(self,
+         t: float, # time
          state: np.ndarray, # dynamical state (Rv, Rd, Psiv, Psid, n)
          input: float # light intensity in lux
          ) -> np.ndarray: # derivative of the state
      "Right-hand-side of the differential equation model"
      Rv = state[0,...]
      Rd = state[1,...]
      Psiv = state[2,...]
@@ -890,14 +904,15 @@
     
     def __str__(self) -> str:
         return "Jewett99"
 
 # %% ../nbs/api/00_models.ipynb 57
 @patch_to(Jewett99)
 def derv(self,
+         t: float, # time
          state: np.ndarray, # dynamical state (x, xc, n)
          input: float # light intensity in lux
          ) -> np.ndarray: # derivative of the state
     "Right-hand-side of the differential equation model"
     x = state[0,...]
     xc = state[1,...]
     n = state[2,...]
@@ -983,10 +998,160 @@
 def dlmos(self,
           trajectory: DynamicalTrajectory=None # trajectory to calculate the dlmo. If None, the current trajectory is used
           ) -> np.ndarray:
     "Finds the Dim Light Melatonin Onset (DLMO) markers for the model along a trajectory"
     if trajectory is None:
         trajectory = self.trajectory
     else:
+        if not isinstance(trajectory, DynamicalTrajectory):
+            raise ValueError("trajectory must be a DynamicalTrajectory")
+    return self.cbt(trajectory) - self.cbt_to_dlmo
+
+# %% ../nbs/api/00_models.ipynb 64
+class Hilaire07(CircadianModel):
+    "Implementation of Hilaire's 2007 model from the article 'Addition of a non-photic component to a light-based mathematical model of the human circadian pacemaker'"
+    def __init__(self, params=None):
+        default_params = {
+            'taux': 24.2, 'G': 37.0, 'k': 0.55, 'mu': 0.13, 'beta': 0.007, 
+            'q': 1.0/3.0, 'rho': 0.032, 'I0': 9500.0, 'p': 0.5, 'a0': 0.1, 
+            'phi_xcx': -2.98, 'phi_ref': 0.97, 'cbt_to_dlmo': 7.0,
+            }
+        num_states = 3 # x, xc, n
+        num_inputs = 2 # light, wake
+        default_initial_condition = np.array([-0.0480751, -1.22504441, 0.51854818])
+        super(Hilaire07, self).__init__(default_params, num_states, num_inputs, default_initial_condition)
+        if params is not None:
+            self.parameters = params
+
+    def integrate(self,
+                  time: np.ndarray, # time points for integration. Time difference between each consecutive pair of values determines step size of the solver
+                  initial_condition: np.ndarray=None, # initial state of the model
+                  input: np.ndarray=None, # model input (such as light or wake) for each time point
+                  ) -> DynamicalTrajectory:
+        "Solve the model for specific timepoints given initial conditions and model inputs"
+        # input checking for Jewett99
+        if input is not None:
+            _light_input_checking(input[0,...])
+            _wake_input_checking(input[1,...])
+        return super().integrate(time, initial_condition, input)
+
+    def __repr__(self) -> str:
+        return self.__str__()
+    
+    def __str__(self) -> str:
+        return "Hilaire07"
+
+# %% ../nbs/api/00_models.ipynb 65
+@patch_to(Hilaire07)
+def derv(self,
+         t: float, # time
+         state: np.ndarray, # dynamical state (x, xc, n)
+         input: np.ndarray # model input (light, wake)
+         ) -> np.ndarray: # derivative of the state
+     "Right-hand-side of the differential equation model"
+     x = state[0,...]
+     xc = state[1,...]
+     n = state[2,...]
+     light = input[0,...] 
+     wake = input[1,...]
+     
+     alpha = self.a0 * (np.power(light / self.I0, self.p)) * (light / (light + 100.0))
+     Bhat = self.G * (1 - n) * alpha * (1 - 0.4 * x) * (1 - 0.4 * xc) 
+     # From article: sigma equals either 1 (for sleep/rest) or 0 (for wake/activity),
+     sigma = 1.0 if wake < 0.5 else 0.0
+     # Calculate psi_cx
+     C = t % 24
+     CBTmin = self.phi_xcx + self.phi_ref
+     CBTminlocal = CBTmin * 24.0 / (2*np.pi)
+     psi_cx = C - CBTminlocal
+     psi_cx = psi_cx % 24
+     # Define Ns
+     Nsh = self.rho * (1.0/3.0 - sigma)
+     if (psi_cx > 16.5 and psi_cx < 21.0):
+          Nsh = self.rho * (1.0/3.0)
+     Ns = Nsh * (1 - np.tanh(10.0 * x))
+
+     mu_term = self.mu * (1.0 / 3.0 * x + 4.0 / 3.0 * np.power(x, 3.0) - 256.0 / 105.0 * np.power(x, 7.0))
+     taux_term = (np.power((24.0 / (0.99729 * self.taux)), 2) + self.k * Bhat)
+     
+     dydt = np.zeros_like(state)
+     dydt[0,...] = np.pi / 12.0 * (xc + mu_term + Bhat + Ns)
+     dydt[1,...] = np.pi / 12.0 * (self.q * Bhat * xc - x * taux_term)
+     dydt[2,...] = 60.0 * (alpha * (1.0 - n) - self.beta * n)
+     
+     return dydt
+
+# %% ../nbs/api/00_models.ipynb 66
+@patch_to(Hilaire07)
+def phase(self,
+          trajectory: DynamicalTrajectory=None, # trajectory to calculate the phase. If None, the current trajectory is used
+          time: float=None # a time point to calculate the phase at. If None, the phase is calculated for the entire trajectory
+          ) -> float:
+    if trajectory is None:
+        trajectory = self.trajectory
+    else: 
+        if not isinstance(trajectory, DynamicalTrajectory):
+            raise ValueError("trajectory must be a DynamicalTrajectory")
+    if time is None:
+        x = trajectory.states[:, 0]
+        y = -1.0 * trajectory.states[:, 1]
+    else:
+        if not isinstance(time, (float, int)):
+            raise ValueError("time must be a float or an int")
+        else:
+            state = trajectory(time)
+            x = state[0] 
+            y = -1.0 * state[1]
+    return np.angle(x + complex(0,1) * y)
+
+# %% ../nbs/api/00_models.ipynb 67
+@patch_to(Hilaire07)
+def amplitude(self,
+              trajectory: DynamicalTrajectory=None, # trajectory to calculate the amplitude. If None, the current trajectory is used
+              time: float=None # a time point to calculate the amplitude at. If None, the amplitude is calculated for the entire trajectory
+              ) -> float:
+    if trajectory is None:
+        trajectory = self.trajectory
+    else: 
+        if not isinstance(trajectory, DynamicalTrajectory):
+            raise ValueError("trajectory must be a DynamicalTrajectory")
+    if time is None:
+        x = trajectory.states[:, 0]
+        y = -1.0 * trajectory.states[:, 1]
+    else:
+        if not isinstance(time, (float, int)):
+            raise ValueError("time must be a float or an int")
+        else:
+            state = trajectory(time)
+            x = state[0] 
+            y = -1.0 * state[1]
+    return np.sqrt(x**2 + y**2)
+
+# %% ../nbs/api/00_models.ipynb 68
+@patch_to(Hilaire07)
+def cbt(self,
+        trajectory: DynamicalTrajectory=None, # trajectory to calculate the cbt. If None, the current trajectory is used
+        ) -> np.ndarray:
+    "Finds the core body temperature minumum markers for the model along a trajectory as the corrected minimum of x"
+    if trajectory is None:
+        trajectory = self.trajectory
+    else:
+        if not isinstance(trajectory, DynamicalTrajectory):
+            raise ValueError("trajectory must be a DynamicalTrajectory")
+    inverted_x = -1*trajectory.states[:,0]
+    cbt_min_idxs, _ = find_peaks(inverted_x)
+    cbtmin_times = trajectory.time[cbt_min_idxs] + self.phi_ref
+    _check_cbtmin_spacing(cbtmin_times)
+    return cbtmin_times
+
+# %% ../nbs/api/00_models.ipynb 69
+@patch_to(Hilaire07)
+def dlmos(self,
+          trajectory: DynamicalTrajectory=None # trajectory to calculate the dlmo. If None, the current trajectory is used
+          ) -> np.ndarray:
+    "Finds the Dim Light Melatonin Onset (DLMO) markers for the model along a trajectory"
+    if trajectory is None:
+        trajectory = self.trajectory
+    else:
         if not isinstance(trajectory, DynamicalTrajectory):
             raise ValueError("trajectory must be a DynamicalTrajectory")
     return self.cbt(trajectory) - self.cbt_to_dlmo
```

### Comparing `circadian-1.0.0/circadian/phasetools.py` & `circadian-1.0.2/circadian/phasetools.py`

 * *Files identical despite different names*

### Comparing `circadian-1.0.0/circadian/plots.py` & `circadian-1.0.2/circadian/plots.py`

 * *Files identical despite different names*

### Comparing `circadian-1.0.0/circadian/prc.py` & `circadian-1.0.2/circadian/prc.py`

 * *Files identical despite different names*

### Comparing `circadian-1.0.0/circadian/sleep.py` & `circadian-1.0.2/circadian/sleep.py`

 * *Files identical despite different names*

### Comparing `circadian-1.0.0/circadian/utils.py` & `circadian-1.0.2/circadian/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/api/07_utils.ipynb.
 
 # %% auto 0
-__all__ = ['phase_difference', 'amplitude_percent_change', 'NpEncoder', 'simple_norm_stepshr_sleep_classifier', 'phase_ic_guess',
-           'abs_hour_diff', 'cut_phases_12', 'convert_binary', 'cal_days_diff', 'interpolateLinear',
+__all__ = ['phase_difference', 'amplitude_percent_change', 'utc_to_hrs', 'NpEncoder', 'simple_norm_stepshr_sleep_classifier',
+           'phase_ic_guess', 'abs_hour_diff', 'cut_phases_12', 'convert_binary', 'cal_days_diff', 'interpolateLinear',
            'interpolateLinearExt', 'parse_dt', 'circular_mean', 'phase_coherence', 'phase_coherence_clock',
            'angle_difference', 'subtract_clock_times', 'circular_av_clock', 'circular_scatter', 'times_to_angle',
            'timezone_mapper', 'split_missing_data', 'split_drop_data', 'redact_dates']
 
 # %% ../nbs/api/07_utils.ipynb 4
 import copy
 import json
@@ -36,27 +36,33 @@
 def amplitude_percent_change(amplitude_1: float, # amplitude between (0, inf)
                              amplitude_2: float # amplitude between (0, inf)
                              ):
     "Percent change between two amplitudes"
     return (amplitude_2 - amplitude_1) / amplitude_1 * 100
 
 # %% ../nbs/api/07_utils.ipynb 9
+def utc_to_hrs(d: pd.Timestamp # UTC timestamp to convert
+               ) -> float: # hours since midnight
+    "Convert UTC timestamp to hours since midnight"
+    return d.hour + d.minute / 60.0 + d.second / 3600.0
+
+# %% ../nbs/api/07_utils.ipynb 11
 class NpEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.floating):
             return float(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         if isinstance(obj, datetime.datetime):
             return obj.isoformat()
         return super(NpEncoder, self).default(obj)
 
-# %% ../nbs/api/07_utils.ipynb 10
+# %% ../nbs/api/07_utils.ipynb 12
 pd.options.mode.chained_assignment = None  # default='warn'
 
 def simple_norm_stepshr_sleep_classifier(t):
         t[0,:] = torch.tanh((t[0,:] - 10.0)/ 100.0)
         t[1, torch.nonzero(t[1,:])] = torch.tanh((t[1,torch.nonzero(t[1,:])] - 60.0) / 30.0)
         return t 
 
@@ -143,15 +149,15 @@
 
 
 def parse_dt(date, time):
     strDate = date + ' ' + time
     return pd.to_datetime(strDate, format='%m/%d/%Y %I:%M %p')
 
 
-# %% ../nbs/api/07_utils.ipynb 12
+# %% ../nbs/api/07_utils.ipynb 14
 def circular_mean(series):
     Z=complex(0,0)
     series=np.array(series)
     for i in range(len(series)):
         Z+=np.exp(series[i]*complex(0,1))
 
     Z=Z/float(len(series))
@@ -218,15 +224,15 @@
     ax.set_theta_zero_location("N")
     ax.set_theta_direction(-1)
     ax.set_thetagrids(list(range(0,360,45)), list(range(0,24,3)))
     ax.set_rmax(1.2)
     ax.set_rticks([0.0,0.2,0.6,0.8,1.0])
     ax.annotate("", xytext=(0.0,0.0), xy=(circular_mean(angles),phase_coherence(angles)),arrowprops=dict(facecolor=color))
 
-# %% ../nbs/api/07_utils.ipynb 14
+# %% ../nbs/api/07_utils.ipynb 16
 class NpEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.floating):
             return float(obj)
         if isinstance(obj, np.ndarray):
@@ -325,15 +331,15 @@
 
     if len(idx_long) > 0:
         return ([date_time[i] for i in idx_long], [ts_split[idx] for idx in idx_long], [steps_split[i] for i in idx_long],
                 [hr_split[i] for i in idx_long], [wake_split[i] for i in idx_long])
     else:
         return None
 
-# %% ../nbs/api/07_utils.ipynb 16
+# %% ../nbs/api/07_utils.ipynb 18
 def redact_dates(infile: str, # the input file in json format
                  outfile: str, # the output file in json format with dates redacted, for user privacy
                  gzip_opt: bool = False # if the input file is gzipped, if the extension is .gz, this is set to True
                  ) -> None:
     gzip_opt = gzip_opt if gzip_opt else infile.endswith(".gz")
     fileobj = gzip.open(infile, 'r') if gzip_opt else open(infile, 'r')
     data = json.load(fileobj)
```

### Comparing `circadian-1.0.0/circadian.egg-info/PKG-INFO` & `circadian-1.0.2/circadian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circadian
-Version: 1.0.0
+Version: 1.0.2
 Summary: Tools for the simulation and analysis of circadian rhythms
 Home-page: https://github.com/Arcascope/circadian
 Author: Arcascope Inc.
 Author-email: support@arcascope.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `circadian-1.0.0/circadian.egg-info/SOURCES.txt` & `circadian-1.0.2/circadian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circadian-1.0.0/settings.ini` & `circadian-1.0.2/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = circadian
 lib_name = circadian
-version = 1.0.0
+version = 1.0.2
 min_python = 3.7
 license = apache2
 doc_path = _docs
 lib_path = circadian
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `circadian-1.0.0/setup.py` & `circadian-1.0.2/setup.py`

 * *Files identical despite different names*

