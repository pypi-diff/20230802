# Comparing `tmp/tom-antares-1.2.4.tar.gz` & `tmp/tom-antares-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom-antares-1.2.4.tar", last modified: Sun Feb  5 03:02:22 2023, max compression
+gzip compressed data, was "tom-antares-1.2.5.tar", last modified: Wed Aug  2 21:52:05 2023, max compression
```

## Comparing `tom-antares-1.2.4.tar` & `tom-antares-1.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 03:02:22.182213 tom-antares-1.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 03:02:22.178213 tom-antares-1.2.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-05 03:02:09.000000 tom-antares-1.2.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 03:02:22.178213 tom-antares-1.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-02-05 03:02:09.000000 tom-antares-1.2.4/.github/workflows/github-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-02-05 03:02:09.000000 tom-antares-1.2.4/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-05 03:02:09.000000 tom-antares-1.2.4/.github/workflows/run-canary-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-02-05 03:02:09.000000 tom-antares-1.2.4/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-02-05 03:02:09.000000 tom-antares-1.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-05 03:02:09.000000 tom-antares-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-02-05 03:02:22.182213 tom-antares-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-02-05 03:02:09.000000 tom-antares-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-05 03:02:09.000000 tom-antares-1.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-05 03:02:22.182213 tom-antares-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-02-05 03:02:09.000000 tom-antares-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 03:02:22.178213 tom-antares-1.2.4/tom_antares/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 03:02:09.000000 tom-antares-1.2.4/tom_antares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-02-05 03:02:09.000000 tom-antares-1.2.4/tom_antares/antares.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 03:02:22.182213 tom-antares-1.2.4/tom_antares/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 03:02:09.000000 tom-antares-1.2.4/tom_antares/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-02-05 03:02:09.000000 tom-antares-1.2.4/tom_antares/tests/boot_django.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-02-05 03:02:09.000000 tom-antares-1.2.4/tom_antares/tests/django_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-02-05 03:02:09.000000 tom-antares-1.2.4/tom_antares/tests/factories.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      429 2023-02-05 03:02:09.000000 tom-antares-1.2.4/tom_antares/tests/run_canary_tests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      429 2023-02-05 03:02:09.000000 tom-antares-1.2.4/tom_antares/tests/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-02-05 03:02:09.000000 tom-antares-1.2.4/tom_antares/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-05 03:02:09.000000 tom-antares-1.2.4/tom_antares/tests/tests_canary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 03:02:22.182213 tom-antares-1.2.4/tom_antares.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-02-05 03:02:22.000000 tom-antares-1.2.4/tom_antares.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-05 03:02:22.000000 tom-antares-1.2.4/tom_antares.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-05 03:02:22.000000 tom-antares-1.2.4/tom_antares.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-05 03:02:22.000000 tom-antares-1.2.4/tom_antares.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-05 03:02:22.000000 tom-antares-1.2.4/tom_antares.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:52:05.083542 tom-antares-1.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:52:05.083542 tom-antares-1.2.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-02 21:51:52.000000 tom-antares-1.2.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:52:05.083542 tom-antares-1.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 21:51:52.000000 tom-antares-1.2.5/.github/workflows/github-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-02 21:51:52.000000 tom-antares-1.2.5/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 21:51:52.000000 tom-antares-1.2.5/.github/workflows/run-canary-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-02 21:51:52.000000 tom-antares-1.2.5/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-02 21:51:52.000000 tom-antares-1.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 21:51:52.000000 tom-antares-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-02 21:52:05.083542 tom-antares-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-02 21:51:52.000000 tom-antares-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 21:51:52.000000 tom-antares-1.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:52:05.083542 tom-antares-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-02 21:51:52.000000 tom-antares-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:52:05.083542 tom-antares-1.2.5/tom_antares/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:51:52.000000 tom-antares-1.2.5/tom_antares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-08-02 21:51:52.000000 tom-antares-1.2.5/tom_antares/antares.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:52:05.083542 tom-antares-1.2.5/tom_antares/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:51:52.000000 tom-antares-1.2.5/tom_antares/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 21:51:52.000000 tom-antares-1.2.5/tom_antares/tests/boot_django.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-08-02 21:51:52.000000 tom-antares-1.2.5/tom_antares/tests/django_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-08-02 21:51:52.000000 tom-antares-1.2.5/tom_antares/tests/factories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      429 2023-08-02 21:51:52.000000 tom-antares-1.2.5/tom_antares/tests/run_canary_tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      429 2023-08-02 21:51:52.000000 tom-antares-1.2.5/tom_antares/tests/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-08-02 21:51:52.000000 tom-antares-1.2.5/tom_antares/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-02 21:51:52.000000 tom-antares-1.2.5/tom_antares/tests/tests_canary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:52:05.083542 tom-antares-1.2.5/tom_antares.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-02 21:52:04.000000 tom-antares-1.2.5/tom_antares.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-02 21:52:05.000000 tom-antares-1.2.5/tom_antares.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:52:04.000000 tom-antares-1.2.5/tom_antares.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-02 21:52:04.000000 tom-antares-1.2.5/tom_antares.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 21:52:04.000000 tom-antares-1.2.5/tom_antares.egg-info/top_level.txt
```

### Comparing `tom-antares-1.2.4/.github/workflows/github-release.yml` & `tom-antares-1.2.5/.github/workflows/github-release.yml`

 * *Files identical despite different names*

### Comparing `tom-antares-1.2.4/.github/workflows/pypi-release.yml` & `tom-antares-1.2.5/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `tom-antares-1.2.4/.github/workflows/run-tests.yml` & `tom-antares-1.2.5/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `tom-antares-1.2.4/.gitignore` & `tom-antares-1.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tom-antares-1.2.4/LICENSE` & `tom-antares-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tom-antares-1.2.4/PKG-INFO` & `tom-antares-1.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tom-antares
-Version: 1.2.4
+Version: 1.2.5
 Summary: Antares broker module for the TOM Toolkit
 Home-page: https://tomtoolkit.github.io
 Author: TOM Toolkit Project
 Author-email: llindstrom@lco.global, dmcollom@gmail.com
 Keywords: tomtoolkit,astronomy,astrophysics,cosmology,science,fits,observatory,antares
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -30,19 +30,18 @@
 
 ## Installation
 
 Install the module into your TOM environment:
 
     pip install tom-antares
 
-Add `tom_antares.antares.AntaresBroker` to the `TOM_ALERT_CLASSES` in your TOM's
+Add `tom_antares.antares.ANTARESBroker` to the `TOM_ALERT_CLASSES` in your TOM's
 `settings.py`:
 
     TOM_ALERT_CLASSES = [
-        'tom_alerts.brokers.mars.MARSBroker',
         ...
         'tom_antares.antares.ANTARESBroker'
     ]
 
 ## Running the tests
 
 In order to run the tests, run the following in your virtualenv:
```

### Comparing `tom-antares-1.2.4/README.md` & `tom-antares-1.2.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 
 ## Installation
 
 Install the module into your TOM environment:
 
     pip install tom-antares
 
-Add `tom_antares.antares.AntaresBroker` to the `TOM_ALERT_CLASSES` in your TOM's
+Add `tom_antares.antares.ANTARESBroker` to the `TOM_ALERT_CLASSES` in your TOM's
 `settings.py`:
 
     TOM_ALERT_CLASSES = [
-        'tom_alerts.brokers.mars.MARSBroker',
         ...
         'tom_antares.antares.ANTARESBroker'
     ]
 
 ## Running the tests
 
 In order to run the tests, run the following in your virtualenv:
```

### Comparing `tom-antares-1.2.4/setup.py` & `tom-antares-1.2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         'Topic :: Scientific/Engineering :: Physics'
     ],
     keywords=['tomtoolkit', 'astronomy', 'astrophysics', 'cosmology', 'science', 'fits', 'observatory', 'antares'],
     packages=find_packages(),
     use_scm_version=True,  # use_scm_version and setup_requires setuptools_scm are required for automated releases
     setup_requires=['setuptools_scm', 'wheel'],
     install_requires=[
-        'tomtoolkit~=2.12.0',
-        'antares-client~=1.2',
+        'tomtoolkit>=2.12,<3.0',
+        'antares-client>=1.2,<2.0',
         'elasticsearch-dsl>=7.3,<7.5'
     ],
     extras_require={
-        'test': ['factory_boy>=3.1,<3.3']
+        'test': ['factory_boy>=3.1,<3.4']
     },
     include_package_data=True,
 )
```

### Comparing `tom-antares-1.2.4/tom_antares/antares.py` & `tom-antares-1.2.5/tom_antares/antares.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,20 @@
         min_value=0.0
     )
     esquery = forms.JSONField(
         required=False,
         label='Elastic Search query in JSON format',
         widget=forms.TextInput(attrs={'placeholder': '{"query":{}}'}),
     )
+    max_alerts = forms.FloatField(
+        label='Maximum number of alerts to fetch',
+        widget=forms.TextInput(attrs={'placeholder': 'Max Alerts'}),
+        min_value=1,
+        initial=20
+    )
 
     # cone_search = ConeSearchField()
     # api_search_tags = forms.MultipleChoiceField(choices=get_tag_choices)
 
     # TODO: add section for searching API in addition to consuming stream
 
     # TODO: add layout
@@ -217,14 +223,18 @@
                     css_class='form-row'
                 )
             ),
             Fieldset(
                 'View Tags',
                 'tag'
             ),
+            Fieldset(
+                'Max Alerts',
+                'max_alerts'
+            ),
             HTML('<hr/>'),
             HTML('<p style="color:blue;font-size:30px">Advanced query</p>'),
             Fieldset(
                  '',
                  'esquery'
             ),
             HTML('''
@@ -314,14 +324,15 @@
         ssr = parameters.get('sr')
         mjd_gt = parameters.get('mjd__gt')
         mjd_lt = parameters.get('mjd__lt')
         mag_min = parameters.get('mag__min')
         mag_max = parameters.get('mag__max')
         elsquery = parameters.get('esquery')
         ztfid = parameters.get('ztfid')
+        max_alerts = parameters.get('max_alerts', 20)
         if ztfid:
             query = {
                 "query": {
                     "bool": {
                         "must": [
                             {
                                 "match": {
@@ -380,15 +391,15 @@
                     }
                 }
 
         loci = antares_client.search.search(query)
 #        if ztfid:
 #            loci = get_by_ztf_object_id(ztfid)
         alerts = []
-        while len(alerts) < 20:
+        while len(alerts) < max_alerts:
             try:
                 locus = next(loci)
             except (marshmallow.exceptions.ValidationError, StopIteration):
                 break
             alerts.append(self.alert_to_dict(locus))
         return iter(alerts)
```

### Comparing `tom-antares-1.2.4/tom_antares/tests/boot_django.py` & `tom-antares-1.2.5/tom_antares/tests/boot_django.py`

 * *Files identical despite different names*

### Comparing `tom-antares-1.2.4/tom_antares/tests/factories.py` & `tom-antares-1.2.5/tom_antares/tests/factories.py`

 * *Files identical despite different names*

### Comparing `tom-antares-1.2.4/tom_antares/tests/tests.py` & `tom-antares-1.2.5/tom_antares/tests/tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,19 +23,26 @@
 
     @mock.patch('tom_antares.antares.antares_client')
     def test_fetch_alerts(self, mock_client):
         """Test the ANTARES-specific fetch_alerts logic."""
         # NOTE: if .side_effect is going to return a list, it needs a function that returns a list
         mock_client.search.search.side_effect = lambda loci: iter(self.loci)
         expected_alert = ANTARESBroker.alert_to_dict(self.locus)
-        alerts = ANTARESBroker().fetch_alerts({'tag': [self.tag]})
+        alerts = ANTARESBroker().fetch_alerts({'tag': [self.tag], 'max_alerts': 3})
 
         # TODO: compare iterator length with len(self.loci)
         self.assertEqual(next(alerts), expected_alert)
 
+    @mock.patch('tom_antares.antares.antares_client')
+    def test_fetch_alerts_max_alerts(self, mock_client):
+        """Tests that the max_alerts parameter actually affects the length of the alert stream"""
+        mock_client.search.search.side_effect = lambda loci: iter(self.loci)
+        alerts = ANTARESBroker().fetch_alerts({'max_alerts': 4})
+        self.assertEqual(len(list(alerts)), 4)
+
     def test_to_target_with_horizons_targetname(self):
         """
         Test that the expected names are created.
 
         The to_target logic in ANTARESBroker only has one branch, which occurs
         when the alert from ANTARES contains a horizons_targetname property
```

### Comparing `tom-antares-1.2.4/tom_antares/tests/tests_canary.py` & `tom-antares-1.2.5/tom_antares/tests/tests_canary.py`

 * *Files identical despite different names*

### Comparing `tom-antares-1.2.4/tom_antares.egg-info/PKG-INFO` & `tom-antares-1.2.5/tom_antares.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tom-antares
-Version: 1.2.4
+Version: 1.2.5
 Summary: Antares broker module for the TOM Toolkit
 Home-page: https://tomtoolkit.github.io
 Author: TOM Toolkit Project
 Author-email: llindstrom@lco.global, dmcollom@gmail.com
 Keywords: tomtoolkit,astronomy,astrophysics,cosmology,science,fits,observatory,antares
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -30,19 +30,18 @@
 
 ## Installation
 
 Install the module into your TOM environment:
 
     pip install tom-antares
 
-Add `tom_antares.antares.AntaresBroker` to the `TOM_ALERT_CLASSES` in your TOM's
+Add `tom_antares.antares.ANTARESBroker` to the `TOM_ALERT_CLASSES` in your TOM's
 `settings.py`:
 
     TOM_ALERT_CLASSES = [
-        'tom_alerts.brokers.mars.MARSBroker',
         ...
         'tom_antares.antares.ANTARESBroker'
     ]
 
 ## Running the tests
 
 In order to run the tests, run the following in your virtualenv:
```

### Comparing `tom-antares-1.2.4/tom_antares.egg-info/SOURCES.txt` & `tom-antares-1.2.5/tom_antares.egg-info/SOURCES.txt`

 * *Files identical despite different names*

