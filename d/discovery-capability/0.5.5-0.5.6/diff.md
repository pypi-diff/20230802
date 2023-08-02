# Comparing `tmp/discovery-capability-0.5.5.tar.gz` & `tmp/discovery-capability-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.5.5.tar", last modified: Tue Aug  1 23:30:00 2023, max compression
+gzip compressed data, was "discovery-capability-0.5.6.tar", last modified: Wed Aug  2 15:30:27 2023, max compression
```

## Comparing `discovery-capability-0.5.5.tar` & `discovery-capability-0.5.6.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:30:00.454653 discovery-capability-0.5.5/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.5/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.5/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-01 23:30:00.455493 discovery-capability-0.5.5/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.5/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:30:00.318123 discovery-capability-0.5.5/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-01 23:30:00.000000 discovery-capability-0.5.5/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     2353 2023-08-01 23:30:00.000000 discovery-capability-0.5.5/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-01 23:30:00.000000 discovery-capability-0.5.5/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-08-01 23:30:00.000000 discovery-capability-0.5.5/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-08-01 23:30:00.000000 discovery-capability-0.5.5/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:30:00.318481 discovery-capability-0.5.5/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-08-01 23:22:16.000000 discovery-capability-0.5.5/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:30:00.321430 discovery-capability-0.5.5/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.5/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13234 2023-08-01 16:23:26.000000 discovery-capability-0.5.5/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.5/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)    20338 2023-08-01 15:46:02.000000 discovery-capability-0.5.5/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.5.5/ds_capability/components/feature_build.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:30:00.322146 discovery-capability-0.5.5/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.5/ds_capability/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:30:00.326204 discovery-capability-0.5.5/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.5/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.5/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.5/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11239 2023-07-30 18:52:11.000000 discovery-capability-0.5.5/ds_capability/intent/feature_build_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    68101 2023-07-28 18:34:45.000000 discovery-capability-0.5.5/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    19736 2023-08-01 23:29:28.000000 discovery-capability-0.5.5/ds_capability/intent/feature_build_model_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:30:00.328242 discovery-capability-0.5.5/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.5/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.5/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.5/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.5/ds_capability/managers/feature_select_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:30:00.442817 discovery-capability-0.5.5/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.5/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.5/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-08-01 23:30:00.456368 discovery-capability-0.5.5/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.5.5/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:30:00.446262 discovery-capability-0.5.5/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.5/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:30:00.447908 discovery-capability-0.5.5/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.5/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3127 2023-08-01 15:50:17.000000 discovery-capability-0.5.5/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.5/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:30:00.448787 discovery-capability-0.5.5/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.5/test/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:30:00.453671 discovery-capability-0.5.5/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.5/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.5/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3099 2023-07-29 22:54:26.000000 discovery-capability-0.5.5/test/intent/fb_correlate_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.5/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-29 21:30:04.000000 discovery-capability-0.5.5/test/intent/fb_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.5/test/intent/fb_model_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 15:30:27.989583 discovery-capability-0.5.6/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.6/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.6/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-02 15:30:27.989933 discovery-capability-0.5.6/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.6/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 15:30:27.809036 discovery-capability-0.5.6/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-02 15:30:27.000000 discovery-capability-0.5.6/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     2353 2023-08-02 15:30:27.000000 discovery-capability-0.5.6/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-02 15:30:27.000000 discovery-capability-0.5.6/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-08-02 15:30:27.000000 discovery-capability-0.5.6/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-08-02 15:30:27.000000 discovery-capability-0.5.6/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 15:30:27.809498 discovery-capability-0.5.6/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-08-01 23:30:55.000000 discovery-capability-0.5.6/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 15:30:27.812720 discovery-capability-0.5.6/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.6/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13783 2023-08-02 15:29:26.000000 discovery-capability-0.5.6/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.6/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20334 2023-08-02 15:29:16.000000 discovery-capability-0.5.6/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.5.6/ds_capability/components/feature_build.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 15:30:27.813855 discovery-capability-0.5.6/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.6/ds_capability/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 15:30:27.818241 discovery-capability-0.5.6/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.6/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.6/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.6/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11239 2023-07-30 18:52:11.000000 discovery-capability-0.5.6/ds_capability/intent/feature_build_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    68101 2023-07-28 18:34:45.000000 discovery-capability-0.5.6/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    19736 2023-08-01 23:29:28.000000 discovery-capability-0.5.6/ds_capability/intent/feature_build_model_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 15:30:27.821403 discovery-capability-0.5.6/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.6/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.6/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.6/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.6/ds_capability/managers/feature_select_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 15:30:27.977398 discovery-capability-0.5.6/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.6/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.6/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-08-02 15:30:27.990695 discovery-capability-0.5.6/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.5.6/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 15:30:27.978283 discovery-capability-0.5.6/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.6/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 15:30:27.979388 discovery-capability-0.5.6/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.6/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3127 2023-08-01 15:50:17.000000 discovery-capability-0.5.6/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.6/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 15:30:27.980491 discovery-capability-0.5.6/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.6/test/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 15:30:27.988245 discovery-capability-0.5.6/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.6/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.6/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3099 2023-07-29 22:54:26.000000 discovery-capability-0.5.6/test/intent/fb_correlate_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.6/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-29 21:30:04.000000 discovery-capability-0.5.6/test/intent/fb_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.6/test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.5.5/LICENSE.txt` & `discovery-capability-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/PKG-INFO` & `discovery-capability-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.5.5
+Version: 0.5.6
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.5.5/README.rst` & `discovery-capability-0.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.5.6/discovery_capability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.5.5
+Version: 0.5.6
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.5.5/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.5.6/discovery_capability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.5.6/ds_capability/components/abstract_common_component.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from abc import abstractmethod
 import pandas as pd
 import pyarrow as pa
 from ds_core.components.abstract_component import AbstractComponent
-from ds_core.components.core_commons import DataAnalytics
 
 from ds_capability.components.commons import Commons
 
 __author__ = 'Darryl Oatridge'
 
 from ds_capability.components.discovery import DataDiscovery
 
@@ -86,58 +85,62 @@
         """ adds a description note that is included in with the 'report_column_catalog'"""
         if isinstance(description, str) and description:
             self.pm.set_intent_description(level=column_name, text=description)
             self.pm_persist(save)
         return
 
     @staticmethod
-    def canonical_report(canonical: pa.Table, headers: [str,list]=None, drop: bool=None, regex:[str,list]=None,
-                         stylise: bool=None, display_width: int=None):
-        """The Canonical Report is a data dictionary of the canonical providing a reference view of the dataset's
-        attribute properties
-
-        :param canonical: the table to view
-        :param headers: (optional) specific headers to display
-        :param drop: if the headers are to be dropped and the remaining to display
-        :param regex: (optional) specify header regex to display
-        :param stylise: (optional) if True present the report stylised.
-        :param display_width: (optional) the width of the observational display
-        """
-        stylise = stylise if isinstance(stylise, bool) else True
-        tbl = Commons.filter_columns(canonical, headers=headers, drop=drop, regex=regex)
-        return DataDiscovery.data_dictionary(canonical=tbl, stylise=stylise, display_width=display_width)
-
-    @staticmethod
     def quality_report(canonical: pa.Table, nulls_threshold: float=None, dom_threshold: float=None,
                      cat_threshold: int=None, stylise: bool=None):
         """ Analyses a dataset, passed as a DataFrame and returns a quality summary
 
         :param canonical: The table to view.
         :param cat_threshold: (optional) The threshold for the max number of unique categories. Default is 60
         :param dom_threshold: (optional) The threshold limit of a dominant value. Default 0.98
         :param nulls_threshold: (optional) The threshold limit of a nulls value. Default 0.9
         :param stylise: (optional) if the output is stylised
         """
         stylise = stylise if isinstance(stylise, bool) else True
         return DataDiscovery.data_quality(canonical=canonical, nulls_threshold=nulls_threshold,
                                           dom_threshold=dom_threshold, cat_threshold=cat_threshold, stylise=stylise)
     @staticmethod
-    def schema_report(canonical: pa.Table, headers: [str,list]=None, drop: bool=None, regex:[str,list]=None,
-               stylise: bool=True):
+    def canonical_report(canonical: pa.Table, headers: [str,list]=None, regex:[str,list]=None, d_types:list=None,
+                         drop: bool=None, stylise: bool=None, display_width: int=None):
+        """The Canonical Report is a data dictionary of the canonical providing a reference view of the dataset's
+        attribute properties
+
+        :param canonical: the table to view
+        :param headers: (optional) specific headers to display
+        :param regex: (optional) specify header regex to display. regex matching is done using the Google RE2 library.
+        :param d_types: (optional) a list of pyarrow DataType e.g [pa.string(), pa.bool_()]
+        :param drop: (optional) if the headers are to be dropped and the remaining to display
+        :param stylise: (optional) if True present the report stylised.
+        :param display_width: (optional) the width of the observational display
+        """
+        stylise = stylise if isinstance(stylise, bool) else True
+        tbl = Commons.filter_columns(canonical, headers=headers, regex=regex, d_types=d_types, drop=drop)
+        return DataDiscovery.data_dictionary(canonical=tbl, stylise=stylise, display_width=display_width)
+
+    @staticmethod
+    def schema_report(canonical: pa.Table, headers: [str,list]=None, regex:[str,list]=None, d_types:list=None,
+                      drop: bool=None, stylise: bool=True, table_cast: bool=None):
         """ presents the current canonical schema
 
-        :param canonical: The table to view.
+        :param canonical: the table to view
         :param headers: (optional) specific headers to display
-        :param drop: if the headers are to be dropped and the remaining to display
-        :param regex: (optional) specify header regex to display
-        :param stylise: (optional) if the output is stylised
+        :param regex: (optional) specify header regex to display. regex matching is done using the Google RE2 library.
+        :param d_types: (optional) a list of pyarrow DataType e.g [pa.string(), pa.bool_()]
+        :param drop: (optional) if the headers are to be dropped and the remaining to display
+        :param stylise: (optional) if True present the report stylised.
+        :param table_cast: (optional) if the column should try to be cast to its type
         """
         stylise = stylise if isinstance(stylise, bool) else True
-        tbl = Commons.filter_columns(canonical, headers=headers, drop=drop, regex=regex)
-        return DataDiscovery.data_quality(canonical=tbl, stylise=stylise)
+        table_cast = table_cast if isinstance(table_cast,bool) else True
+        tbl = Commons.filter_columns(canonical, headers=headers, regex=regex, d_types=d_types, drop=drop)
+        return DataDiscovery.data_schema(canonical=tbl, table_cast=table_cast, stylise=stylise)
 
     def report_task(self, stylise: bool=True):
         """ generates a report on the source contract
 
         :param stylise: (optional) returns a stylised DataFrame with formatting
         :return: pd.DataFrame
         """
```

### Comparing `discovery-capability-0.5.5/ds_capability/components/commons.py` & `discovery-capability-0.5.6/ds_capability/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/components/discovery.py` & `discovery-capability-0.5.6/ds_capability/components/discovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             _ = df_style.set_caption(f"dataset has {canonical.num_columns} columns")
             _ = df_style.set_properties(subset=['Attributes'],  **{'font-weight': 'bold', 'font-size': "120%"})
             return df_style
         return pa.Table.from_pandas(df)
 
 
     @staticmethod
-    def data_schema(canonical: pa.Table, table_cast: bool = None, stylise: bool = None):
+    def data_schema(canonical: pa.Table, table_cast: bool=None, stylise: bool=None):
         """ The data dictionary for a given canonical
 
         :param canonical: The canonical to interpret
         :param table_cast: (optional) attempt to cast columns to the content
         :param stylise: (optional) if the output is stylised for jupyter display
         :return: a pa.Table or stylised pandas
         """
```

### Comparing `discovery-capability-0.5.5/ds_capability/components/feature_build.py` & `discovery-capability-0.5.6/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.5.6/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/intent/common_intent.py` & `discovery-capability-0.5.6/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/intent/feature_build_correlate_intent.py` & `discovery-capability-0.5.6/ds_capability/intent/feature_build_correlate_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.5.6/ds_capability/intent/feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/intent/feature_build_model_intent.py` & `discovery-capability-0.5.6/ds_capability/intent/feature_build_model_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.5.6/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.5.6/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.5.6/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.5.6/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.5.6/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.5.6/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.5.6/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.5.6/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.5.6/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.5.6/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.5.6/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.5.6/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.5.6/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.5.6/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.5.6/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.5.6/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.5.6/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.5.6/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.5.6/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.5.6/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.5.6/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.5.6/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.5.6/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/ds_capability/sample/sample_data.py` & `discovery-capability-0.5.6/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/setup.py` & `discovery-capability-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/test/component/discovery_test.py` & `discovery-capability-0.5.6/test/component/discovery_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/test/component/synthetic_test.py` & `discovery-capability-0.5.6/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.5.6/test/intent/fb_analysis_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/test/intent/fb_correlate_intent_test.py` & `discovery-capability-0.5.6/test/intent/fb_correlate_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.5.6/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/test/intent/fb_intent_test.py` & `discovery-capability-0.5.6/test/intent/fb_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.5/test/intent/fb_model_intent_test.py` & `discovery-capability-0.5.6/test/intent/fb_model_intent_test.py`

 * *Files identical despite different names*

