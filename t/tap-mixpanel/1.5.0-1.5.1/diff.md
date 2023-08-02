# Comparing `tmp/tap-mixpanel-1.5.0.tar.gz` & `tmp/tap-mixpanel-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-mixpanel-1.5.0.tar", last modified: Thu May 25 00:50:09 2023, max compression
+gzip compressed data, was "tap-mixpanel-1.5.1.tar", last modified: Wed Aug  2 14:35:27 2023, max compression
```

## Comparing `tap-mixpanel-1.5.0.tar` & `tap-mixpanel-1.5.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/MANIFEST.in
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tests/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tests/tap_tester/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8083 2023-05-25 00:45:30.000000 tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_start_date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2505 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_automatic_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8220 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_discovery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7496 2023-05-25 00:45:30.000000 tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_all_fields_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8779 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_bookmark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      164 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tests/tap_tester/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15708 2023-05-25 00:45:30.000000 tap-mixpanel-1.5.0/tests/tap_tester/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tests/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tests/unittests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4296 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4819 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_transform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7646 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_support_eu_endpoints.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3438 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_request_timeout_param_value.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1523 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_transform_event_times.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5065 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tests/unittests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1717 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_attribution_window.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11184 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_error_handling.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3709 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      146 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      727 2023-05-25 00:45:30.000000 tap-mixpanel-1.5.0/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/LICENSE
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1400 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12936 2023-05-25 00:45:30.000000 tap-mixpanel-1.5.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5161 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tap_mixpanel/transform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12294 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tap_mixpanel/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      603 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/export.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/cohort_members.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3390 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/funnels.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      139 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/engage.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      510 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/cohorts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      449 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/revenue.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      335 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/annotations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34637 2023-05-25 00:45:30.000000 tap-mixpanel-1.5.0/tap_mixpanel/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7134 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tap_mixpanel/schema.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3191 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tap_mixpanel/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3548 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tap_mixpanel/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1162 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tap_mixpanel/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 14:35:27.804443 tap-mixpanel-1.5.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2023-05-01 19:21:05.000000 tap-mixpanel-1.5.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2023-05-01 19:21:05.000000 tap-mixpanel-1.5.1/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      229 2023-08-02 14:35:27.804443 tap-mixpanel-1.5.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12936 2023-05-30 20:50:11.000000 tap-mixpanel-1.5.1/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-08-02 14:35:27.804443 tap-mixpanel-1.5.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      727 2023-08-02 14:31:29.000000 tap-mixpanel-1.5.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 14:35:27.796443 tap-mixpanel-1.5.1/tap_mixpanel/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3191 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tap_mixpanel/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12338 2023-08-02 14:31:29.000000 tap-mixpanel-1.5.1/tap_mixpanel/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1162 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tap_mixpanel/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7134 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tap_mixpanel/schema.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 14:35:27.800443 tap-mixpanel-1.5.1/tap_mixpanel/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      335 2023-05-01 19:21:05.000000 tap-mixpanel-1.5.1/tap_mixpanel/schemas/annotations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2023-05-01 19:21:05.000000 tap-mixpanel-1.5.1/tap_mixpanel/schemas/cohort_members.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      510 2023-05-01 19:21:05.000000 tap-mixpanel-1.5.1/tap_mixpanel/schemas/cohorts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      139 2023-05-01 19:21:05.000000 tap-mixpanel-1.5.1/tap_mixpanel/schemas/engage.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      603 2023-05-01 19:21:05.000000 tap-mixpanel-1.5.1/tap_mixpanel/schemas/export.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3390 2023-05-01 19:21:05.000000 tap-mixpanel-1.5.1/tap_mixpanel/schemas/funnels.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      449 2023-05-01 19:21:05.000000 tap-mixpanel-1.5.1/tap_mixpanel/schemas/revenue.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34816 2023-08-02 14:31:29.000000 tap-mixpanel-1.5.1/tap_mixpanel/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3548 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tap_mixpanel/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5161 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tap_mixpanel/transform.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 14:35:27.800443 tap-mixpanel-1.5.1/tap_mixpanel.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      229 2023-08-02 14:35:27.000000 tap-mixpanel-1.5.1/tap_mixpanel.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1400 2023-08-02 14:35:27.000000 tap-mixpanel-1.5.1/tap_mixpanel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-02 14:35:27.000000 tap-mixpanel-1.5.1/tap_mixpanel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-08-02 14:35:27.000000 tap-mixpanel-1.5.1/tap_mixpanel.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-08-02 14:35:27.000000 tap-mixpanel-1.5.1/tap_mixpanel.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-08-02 14:35:27.000000 tap-mixpanel-1.5.1/tap_mixpanel.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 14:35:27.800443 tap-mixpanel-1.5.1/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-01 19:21:05.000000 tap-mixpanel-1.5.1/tests/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 14:35:27.804443 tap-mixpanel-1.5.1/tests/tap_tester/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      164 2023-05-01 19:21:05.000000 tap-mixpanel-1.5.1/tests/tap_tester/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15708 2023-05-30 20:50:11.000000 tap-mixpanel-1.5.1/tests/tap_tester/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7496 2023-05-30 20:50:11.000000 tap-mixpanel-1.5.1/tests/tap_tester/test_mixpanel_all_fields_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2505 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tests/tap_tester/test_mixpanel_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8779 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tests/tap_tester/test_mixpanel_bookmark.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8220 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tests/tap_tester/test_mixpanel_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8083 2023-05-30 20:50:11.000000 tap-mixpanel-1.5.1/tests/tap_tester/test_mixpanel_start_date.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 14:35:27.804443 tap-mixpanel-1.5.1/tests/unittests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-01 19:21:05.000000 tap-mixpanel-1.5.1/tests/unittests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1717 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tests/unittests/test_attribution_window.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5065 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tests/unittests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3709 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tests/unittests/test_discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12720 2023-08-02 14:31:29.000000 tap-mixpanel-1.5.1/tests/unittests/test_error_handling.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4296 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tests/unittests/test_main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3438 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tests/unittests/test_request_timeout_param_value.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7646 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tests/unittests/test_support_eu_endpoints.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4819 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tests/unittests/test_sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tests/unittests/test_transform.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1523 2023-05-24 15:46:27.000000 tap-mixpanel-1.5.1/tests/unittests/test_transform_event_times.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_start_date.py` & `tap-mixpanel-1.5.1/tests/tap_tester/test_mixpanel_start_date.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_automatic_fields.py` & `tap-mixpanel-1.5.1/tests/tap_tester/test_mixpanel_automatic_fields.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_discovery.py` & `tap-mixpanel-1.5.1/tests/tap_tester/test_mixpanel_discovery.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_all_fields_pagination.py` & `tap-mixpanel-1.5.1/tests/tap_tester/test_mixpanel_all_fields_pagination.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_bookmark.py` & `tap-mixpanel-1.5.1/tests/tap_tester/test_mixpanel_bookmark.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/tap_tester/base.py` & `tap-mixpanel-1.5.1/tests/tap_tester/base.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/unittests/test_main.py` & `tap-mixpanel-1.5.1/tests/unittests/test_main.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/unittests/test_sync.py` & `tap-mixpanel-1.5.1/tests/unittests/test_sync.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/unittests/test_transform.py` & `tap-mixpanel-1.5.1/tests/unittests/test_transform.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/unittests/test_support_eu_endpoints.py` & `tap-mixpanel-1.5.1/tests/unittests/test_support_eu_endpoints.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/unittests/test_request_timeout_param_value.py` & `tap-mixpanel-1.5.1/tests/unittests/test_request_timeout_param_value.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/unittests/test_transform_event_times.py` & `tap-mixpanel-1.5.1/tests/unittests/test_transform_event_times.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/unittests/test_client.py` & `tap-mixpanel-1.5.1/tests/unittests/test_client.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/unittests/test_attribution_window.py` & `tap-mixpanel-1.5.1/tests/unittests/test_attribution_window.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tests/unittests/test_error_handling.py` & `tap-mixpanel-1.5.1/tests/unittests/test_error_handling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import unittest
 import requests
 
+import jsonlines
 from unittest import mock
 from parameterized import parameterized
 
 from tap_mixpanel import client
+from tap_mixpanel import streams
 
 # Mock response
 REQUEST_TIMEOUT = 300
 
 
 class MockResponse:
     """Mocked standard HTTPResponse to test error handling."""
@@ -245,7 +247,44 @@
         """
         mock_client = client.MixpanelClient(api_secret="mock_api_secret", api_domain="mock_api_domain", request_timeout=REQUEST_TIMEOUT)
         with self.assertRaises(requests.models.ProtocolError):
             mock_client.check_access()
 
         # Verify that requests.Session.request is called 5 times
         self.assertEqual(mock_request.call_count, 5)
+
+    @mock.patch("jsonlines.jsonlines.Reader.iter", side_effect=requests.exceptions.ChunkedEncodingError)
+    def test_ChunkedEncodingError(self, mock_jsonlines, mock_time):
+        """
+        Check whether the request backoffs properly for `check_access` method for 5 times in case of Timeout error.
+        """
+        mock_client = client.MixpanelClient(api_secret="mock_api_secret", api_domain="mock_api_domain", request_timeout=REQUEST_TIMEOUT)
+        mock_client._MixpanelClient__verified = True
+
+        fake_response = MockResponse(500)
+        fake_response.iter_lines = lambda : []
+        mock_client.perform_request = lambda *args, **kwargs: fake_response
+
+        stream = streams.Export(mock_client)
+
+        with self.assertRaises(requests.exceptions.ChunkedEncodingError) as error:
+            stream.get_and_transform_records(
+                querystring={},
+                project_timezone=None,
+                max_bookmark_value=None,
+                state=None,
+                config=None,
+                catalog=None,
+                selected_streams=None,
+                last_datetime=None,
+                endpoint_total=None,
+                limit=None,
+                total_records=None,
+                parent_total=None,
+                record_count=None,
+                page=None,
+                offset=None,
+                parent_record=None,
+                date_total=None,
+            )
+
+        self.assertEqual(mock_jsonlines.call_count, 5)
```

### Comparing `tap-mixpanel-1.5.0/tests/unittests/test_discover.py` & `tap-mixpanel-1.5.1/tests/unittests/test_discover.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/setup.py` & `tap-mixpanel-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-mixpanel',
-      version='1.5.0',
+      version='1.5.1',
       description='Singer.io tap for extracting data from the mixpanel API',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_mixpanel'],
       install_requires=[
           'backoff==1.8.0',
           'requests==2.22.0',
```

### Comparing `tap-mixpanel-1.5.0/LICENSE` & `tap-mixpanel-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tap_mixpanel.egg-info/SOURCES.txt` & `tap-mixpanel-1.5.1/tap_mixpanel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/README.md` & `tap-mixpanel-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tap_mixpanel/transform.py` & `tap-mixpanel-1.5.1/tap_mixpanel/transform.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tap_mixpanel/client.py` & `tap-mixpanel-1.5.1/tap_mixpanel/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 
 import backoff
 import jsonlines
 import requests
 import singer
-from requests.exceptions import ConnectionError, Timeout
+from requests.exceptions import ChunkedEncodingError, ConnectionError, Timeout
 from requests.models import ProtocolError
 from singer import metrics
 
 LOGGER = singer.get_logger()
 
 BACKOFF_MAX_TRIES_REQUEST = 7
 REQUEST_TIMEOUT = 300
@@ -200,15 +200,15 @@
         elif response.status_code != 200:
             LOGGER.error("Error status_code = %s", response.status_code)
             raise_for_error(response)
         return True
 
     @backoff.on_exception(
         backoff.expo,
-        (Server5xxError, Server429Error, ReadTimeoutError, ConnectionError, Timeout, ProtocolError),
+        (Server5xxError, Server429Error, ReadTimeoutError, ConnectionError, Timeout, ProtocolError, ChunkedEncodingError),
         max_tries=BACKOFF_MAX_TRIES_REQUEST,
         factor=3,
         logger=LOGGER,
     )
     def perform_request(
         self, method, url=None, params=None, json=None, stream=False, **kwargs
     ):
```

### Comparing `tap-mixpanel-1.5.0/tap_mixpanel/schemas/export.json` & `tap-mixpanel-1.5.1/tap_mixpanel/schemas/export.json`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tap_mixpanel/schemas/funnels.json` & `tap-mixpanel-1.5.1/tap_mixpanel/schemas/funnels.json`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tap_mixpanel/streams.py` & `tap-mixpanel-1.5.1/tap_mixpanel/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import json
 import math
 from copy import deepcopy
 from datetime import datetime, timedelta
 
 import urllib
 import pytz
+import requests
+import backoff
 import singer
 from singer import Transformer, metadata, metrics, utils
 from singer.utils import strptime_to_utc
 
 from tap_mixpanel.client import MixpanelClient
 from tap_mixpanel.transform import transform_datetime, transform_record
 
@@ -691,14 +693,21 @@
     replication_keys = ["time"]
     url = "https://data.mixpanel.com/api/2.0"
     bookmark_query_field_from = "from_date"
     bookmark_query_field_to = "to_date"
     replication_method = "INCREMENTAL"
     params = {}
 
+
+    @backoff.on_exception(
+        backoff.expo,
+        (requests.exceptions.ChunkedEncodingError,),
+        max_tries=5,
+        factor=2,
+    )
     def get_and_transform_records(
         self,
         querystring,
         project_timezone,
         max_bookmark_value,
         state,
         config,
```

### Comparing `tap-mixpanel-1.5.0/tap_mixpanel/schema.py` & `tap-mixpanel-1.5.1/tap_mixpanel/schema.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tap_mixpanel/__init__.py` & `tap-mixpanel-1.5.1/tap_mixpanel/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tap_mixpanel/sync.py` & `tap-mixpanel-1.5.1/tap_mixpanel/sync.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.5.0/tap_mixpanel/discover.py` & `tap-mixpanel-1.5.1/tap_mixpanel/discover.py`

 * *Files identical despite different names*

