# Comparing `tmp/pyGuardPoint-0.9.8.tar.gz` & `tmp/pyGuardPoint-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.9.8.tar", last modified: Mon Jul 31 10:19:44 2023, max compression
+gzip compressed data, was "pyGuardPoint-0.9.9.tar", last modified: Wed Aug  2 09:22:37 2023, max compression
```

## Comparing `pyGuardPoint-0.9.8.tar` & `pyGuardPoint-0.9.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 10:19:44.574489 pyGuardPoint-0.9.8/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.9.8/LICENSE.txt
--rw-rw-rw-   0        0        0     6116 2023-07-31 10:19:44.574489 pyGuardPoint-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     5857 2023-07-26 10:18:05.000000 pyGuardPoint-0.9.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-31 10:19:44.561455 pyGuardPoint-0.9.8/pyGuardPoint/
--rw-rw-rw-   0        0        0      266 2023-04-20 12:58:39.000000 pyGuardPoint-0.9.8/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11195 2023-04-20 13:33:25.000000 pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     1083 2023-04-20 13:02:16.000000 pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_cardholdertypes.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1195 2023-05-12 10:57:02.000000 pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5586 2023-04-20 11:51:01.000000 pyGuardPoint-0.9.8/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.9.8/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2915 2023-07-26 07:31:58.000000 pyGuardPoint-0.9.8/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.9.8/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0    10663 2023-07-26 10:12:29.000000 pyGuardPoint-0.9.8/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    17658 2023-05-12 10:58:18.000000 pyGuardPoint-0.9.8/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.9.8/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     3140 2023-05-04 10:22:18.000000 pyGuardPoint-0.9.8/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 10:19:44.572458 pyGuardPoint-0.9.8/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0     6116 2023-07-31 10:19:44.000000 pyGuardPoint-0.9.8/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2023-07-31 10:19:44.000000 pyGuardPoint-0.9.8/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 10:19:44.000000 pyGuardPoint-0.9.8/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.9.8/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-07-31 10:19:44.000000 pyGuardPoint-0.9.8/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 10:19:44.000000 pyGuardPoint-0.9.8/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 10:19:44.574489 pyGuardPoint-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0      565 2023-07-31 10:19:07.000000 pyGuardPoint-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 09:22:37.284077 pyGuardPoint-0.9.9/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.9.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     6116 2023-08-02 09:22:37.283087 pyGuardPoint-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5857 2023-07-26 10:18:05.000000 pyGuardPoint-0.9.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 09:22:37.276080 pyGuardPoint-0.9.9/pyGuardPoint/
+-rw-rw-rw-   0        0        0      266 2023-04-20 12:58:39.000000 pyGuardPoint-0.9.9/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    11195 2023-04-20 13:33:25.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     1083 2023-04-20 13:02:16.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_cardholdertypes.py
+-rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1195 2023-05-12 10:57:02.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5584 2023-08-02 09:21:03.000000 pyGuardPoint-0.9.9/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.9.9/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2915 2023-07-26 07:31:58.000000 pyGuardPoint-0.9.9/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0    10663 2023-07-31 14:11:21.000000 pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    17658 2023-05-12 10:58:18.000000 pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3140 2023-05-04 10:22:18.000000 pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 09:22:37.282077 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0     6116 2023-08-02 09:22:37.000000 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2023-08-02 09:22:37.000000 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 09:22:37.000000 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-08-02 09:22:37.000000 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-02 09:22:37.000000 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 09:22:37.284077 pyGuardPoint-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      565 2023-08-02 09:21:40.000000 pyGuardPoint-0.9.9/setup.py
```

### Comparing `pyGuardPoint-0.9.8/LICENSE.txt` & `pyGuardPoint-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/PKG-INFO` & `pyGuardPoint-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-0.9.8/README.rst` & `pyGuardPoint-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_cardholdertypes.py` & `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_cardholdertypes.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-0.9.9/pyGuardPoint/_odata_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             last_pass_date = earliest_last_pass.strftime('%Y-%m-%dT%H:%M:%SZ')
             filter_phrases.append(f'(lastPassDate%20ge%20{last_pass_date})')
 
     # Filter out expired cardholders
     if filter_expired:
         # end_of_day = datetime.utcnow().strftime('%Y-%m-%dT23:59:59Z')
         start_of_day = datetime.utcnow().strftime('%Y-%m-%dT00:00:00Z')
-        filter_phrases.append(f'(fromDateValid%20ge%20{start_of_day})')
+        filter_phrases.append(f'(toDateValid%20ge%20{start_of_day})')
 
     # Filter by Cardholder Type Name
     if cardholder_type_name:
         filter_phrases.append(f"(cardholderType/typeName%20eq%20'{cardholder_type_name}')")
 
     # Filter by Areas
     if areas:
```

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-0.9.9/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/guardpoint.py` & `pyGuardPoint-0.9.9/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         if self.authType == GuardPointAuthType.BASIC:
             auth_str = "Basic " + ConvertBase64.encode(f"{self.user}:{self.key}")
         elif self.authType == GuardPointAuthType.BEARER_TOKEN:
             if self.token is None:
                 code, auth_body = self._new_token()
                 if code != 200:
                     return code, auth_body
-            if self.token_expiry < (time.time() - (30 * 60)):  # If Token will expire within 30 minutes
+            if self.token_expiry < (time.time() - (20 * 60)):  # If Token will expire within 20 minutes
                 code, auth_body = self._renew_token()
                 if code != 200:
                     return code, auth_body
             if self.token_expiry < time.time():
                 code, auth_body = self._new_token()
                 if code != 200:
                     return code, auth_body
```

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint.egg-info/PKG-INFO` & `pyGuardPoint-0.9.9/pyGuardPoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-0.9.8/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-0.9.9/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.8/setup.py` & `pyGuardPoint-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
-      version="0.9.8",
+      version="0.9.9",
       author="John Owen",
       description="Python wrapper for GuardPoint 10 Access Control System",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
       install_requires=['validators', 'fuzzywuzzy', 'Levenshtein', 'cryptography'],
       packages=['pyGuardPoint'],
```

