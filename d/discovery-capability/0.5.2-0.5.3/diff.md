# Comparing `tmp/discovery-capability-0.5.2.tar.gz` & `tmp/discovery-capability-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.5.2.tar", last modified: Tue Aug  1 15:55:57 2023, max compression
+gzip compressed data, was "discovery-capability-0.5.3.tar", last modified: Tue Aug  1 23:06:59 2023, max compression
```

## Comparing `discovery-capability-0.5.2.tar` & `discovery-capability-0.5.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.301634 discovery-capability-0.5.2/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.2/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.2/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-01 15:55:57.301855 discovery-capability-0.5.2/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.2/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.133343 discovery-capability-0.5.2/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-01 15:55:57.000000 discovery-capability-0.5.2/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     2353 2023-08-01 15:55:57.000000 discovery-capability-0.5.2/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-01 15:55:57.000000 discovery-capability-0.5.2/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-08-01 15:55:57.000000 discovery-capability-0.5.2/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-08-01 15:55:57.000000 discovery-capability-0.5.2/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.133860 discovery-capability-0.5.2/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-27 22:41:13.000000 discovery-capability-0.5.2/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.137040 discovery-capability-0.5.2/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.2/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14475 2023-07-27 16:49:58.000000 discovery-capability-0.5.2/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.2/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)    20338 2023-08-01 15:46:02.000000 discovery-capability-0.5.2/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.5.2/ds_capability/components/feature_build.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.137784 discovery-capability-0.5.2/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.2/ds_capability/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.141549 discovery-capability-0.5.2/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.2/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.2/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.2/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11239 2023-07-30 18:52:11.000000 discovery-capability-0.5.2/ds_capability/intent/feature_build_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    68101 2023-07-28 18:34:45.000000 discovery-capability-0.5.2/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    20903 2023-07-27 23:20:42.000000 discovery-capability-0.5.2/ds_capability/intent/feature_build_model_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.143846 discovery-capability-0.5.2/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.2/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.2/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.2/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.2/ds_capability/managers/feature_select_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.293834 discovery-capability-0.5.2/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.2/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-08-01 15:55:57.302514 discovery-capability-0.5.2/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.5.2/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.294753 discovery-capability-0.5.2/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.2/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.295624 discovery-capability-0.5.2/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.2/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3127 2023-08-01 15:50:17.000000 discovery-capability-0.5.2/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.2/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.296390 discovery-capability-0.5.2/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.2/test/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.299515 discovery-capability-0.5.2/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.2/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.2/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3099 2023-07-29 22:54:26.000000 discovery-capability-0.5.2/test/intent/fb_correlate_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.2/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-29 21:30:04.000000 discovery-capability-0.5.2/test/intent/fb_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.2/test/intent/fb_model_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.983235 discovery-capability-0.5.3/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.3/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.3/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-01 23:06:59.983548 discovery-capability-0.5.3/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.3/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.824773 discovery-capability-0.5.3/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-01 23:06:59.000000 discovery-capability-0.5.3/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     2353 2023-08-01 23:06:59.000000 discovery-capability-0.5.3/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-01 23:06:59.000000 discovery-capability-0.5.3/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-08-01 23:06:59.000000 discovery-capability-0.5.3/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-08-01 23:06:59.000000 discovery-capability-0.5.3/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.825168 discovery-capability-0.5.3/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-08-01 15:56:54.000000 discovery-capability-0.5.3/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.828684 discovery-capability-0.5.3/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.3/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13234 2023-08-01 16:23:26.000000 discovery-capability-0.5.3/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.3/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20338 2023-08-01 15:46:02.000000 discovery-capability-0.5.3/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.5.3/ds_capability/components/feature_build.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.829540 discovery-capability-0.5.3/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.3/ds_capability/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.835373 discovery-capability-0.5.3/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.3/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.3/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.3/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11239 2023-07-30 18:52:11.000000 discovery-capability-0.5.3/ds_capability/intent/feature_build_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    68101 2023-07-28 18:34:45.000000 discovery-capability-0.5.3/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20073 2023-08-01 22:56:33.000000 discovery-capability-0.5.3/ds_capability/intent/feature_build_model_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.839527 discovery-capability-0.5.3/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.3/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.3/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.3/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.3/ds_capability/managers/feature_select_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.972256 discovery-capability-0.5.3/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.3/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-08-01 23:06:59.984563 discovery-capability-0.5.3/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.5.3/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.973330 discovery-capability-0.5.3/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.3/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.974864 discovery-capability-0.5.3/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.3/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3127 2023-08-01 15:50:17.000000 discovery-capability-0.5.3/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.3/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.975757 discovery-capability-0.5.3/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.3/test/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.980856 discovery-capability-0.5.3/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.3/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.3/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3099 2023-07-29 22:54:26.000000 discovery-capability-0.5.3/test/intent/fb_correlate_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.3/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-29 21:30:04.000000 discovery-capability-0.5.3/test/intent/fb_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.3/test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.5.2/LICENSE.txt` & `discovery-capability-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/PKG-INFO` & `discovery-capability-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.5.2
+Version: 0.5.3
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.5.2/README.rst` & `discovery-capability-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.5.3/discovery_capability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.5.2
+Version: 0.5.3
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.5.2/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.5.3/discovery_capability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.5.3/ds_capability/components/abstract_common_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,24 +86,29 @@
         """ adds a description note that is included in with the 'report_column_catalog'"""
         if isinstance(description, str) and description:
             self.pm.set_intent_description(level=column_name, text=description)
             self.pm_persist(save)
         return
 
     @staticmethod
-    def canonical_report(canonical: pa.Table, stylise: bool=None, display_width: int=None):
+    def canonical_report(canonical: pa.Table, headers: [str,list]=None, drop: bool=None, regex:[str,list]=None,
+                         stylise: bool=None, display_width: int=None):
         """The Canonical Report is a data dictionary of the canonical providing a reference view of the dataset's
         attribute properties
 
         :param canonical: the table to view
+        :param headers: (optional) specific headers to display
+        :param drop: if the headers are to be dropped and the remaining to display
+        :param regex: (optional) specify header regex to display
         :param stylise: (optional) if True present the report stylised.
         :param display_width: (optional) the width of the observational display
         """
         stylise = stylise if isinstance(stylise, bool) else True
-        return DataDiscovery.data_dictionary(canonical=canonical, stylise=stylise, display_width=display_width)
+        tbl = Commons.filter_columns(canonical, headers=headers, drop=drop, regex=regex)
+        return DataDiscovery.data_dictionary(canonical=tbl, stylise=stylise, display_width=display_width)
 
     @staticmethod
     def quality_report(canonical: pa.Table, nulls_threshold: float=None, dom_threshold: float=None,
                      cat_threshold: int=None, stylise: bool=None):
         """ Analyses a dataset, passed as a DataFrame and returns a quality summary
 
         :param canonical: The table to view.
@@ -111,56 +116,28 @@
         :param dom_threshold: (optional) The threshold limit of a dominant value. Default 0.98
         :param nulls_threshold: (optional) The threshold limit of a nulls value. Default 0.9
         :param stylise: (optional) if the output is stylised
         """
         stylise = stylise if isinstance(stylise, bool) else True
         return DataDiscovery.data_quality(canonical=canonical, nulls_threshold=nulls_threshold,
                                           dom_threshold=dom_threshold, cat_threshold=cat_threshold, stylise=stylise)
-
-    def report_canonical_schema(self, schema: [str, dict]=None, roots: [str, list]=None,
-                                sections: [str, list]=None, elements: [str, list]=None, stylise: bool=True):
+    @staticmethod
+    def schema_report(canonical: pa.Table, headers: [str,list]=None, drop: bool=None, regex:[str,list]=None,
+               stylise: bool=True):
         """ presents the current canonical schema
 
-        :param schema: (optional) the name of the schema
-        :param roots: (optional) one or more tree roots
-        :param sections: (optional) the section under the root
-        :param elements: (optional) the element in the section
-        :param stylise: if True present the report stylised.
-        :return: pd.DataFrame
+        :param canonical: The table to view.
+        :param headers: (optional) specific headers to display
+        :param drop: if the headers are to be dropped and the remaining to display
+        :param regex: (optional) specify header regex to display
+        :param stylise: (optional) if the output is stylised
         """
-        if not isinstance(schema, dict):
-            schema = schema if isinstance(schema, str) else self.REPORT_SCHEMA
-            if not self.pm.has_canonical_schema(name=schema):
-                raise ValueError(f"There is no Schema currently stored under the name '{schema}'")
-            schema = self.pm.get_canonical_schema(name=schema)
-        df = pd.DataFrame(columns=['root', 'section', 'element', 'value'])
-        root_list = DataAnalytics.get_tree_roots(analytics_blob=schema)
-        if isinstance(roots, (str, list)):
-            roots = Commons.list_formatter(roots)
-            for root in roots:
-                if root not in root_list:
-                    raise ValueError(f"The root '{root}' can not be found in the analytics tree roots")
-            root_list = roots
-        for root_items in root_list:
-            data_analysis = DataAnalytics.from_root(analytics_blob=schema, root=root_items)
-            for section in data_analysis.section_names:
-                if isinstance(sections, (str, list)):
-                    if section not in Commons.list_formatter(sections):
-                        continue
-                for element, value in data_analysis.get(section).items():
-                    if isinstance(elements, (str, list)):
-                        if element not in Commons.list_formatter(elements):
-                            continue
-                    to_append = [root_items, section, element, value]
-                    a_series = pd.Series(to_append, index=df.columns)
-                    # df = df.append(a_series, ignore_index=True)
-                    df = pd.concat([df, a_series.to_frame().transpose()], ignore_index=True)
-        if stylise:
-            return Commons.report(df, index_header=['root', 'section'], bold='element')
-        return df
+        stylise = stylise if isinstance(stylise, bool) else True
+        tbl = Commons.filter_columns(canonical, headers=headers, drop=drop, regex=regex)
+        return DataDiscovery.data_quality(canonical=tbl, stylise=stylise)
 
     def report_task(self, stylise: bool=True):
         """ generates a report on the source contract
 
         :param stylise: (optional) returns a stylised DataFrame with formatting
         :return: pd.DataFrame
         """
```

### Comparing `discovery-capability-0.5.2/ds_capability/components/commons.py` & `discovery-capability-0.5.3/ds_capability/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/components/discovery.py` & `discovery-capability-0.5.3/ds_capability/components/discovery.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/components/feature_build.py` & `discovery-capability-0.5.3/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.5.3/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/intent/common_intent.py` & `discovery-capability-0.5.3/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/intent/feature_build_correlate_intent.py` & `discovery-capability-0.5.3/ds_capability/intent/feature_build_correlate_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.5.3/ds_capability/intent/feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/intent/feature_build_model_intent.py` & `discovery-capability-0.5.3/ds_capability/intent/feature_build_model_intent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import inspect
 import pandas as pd
 import pyarrow as pa
-from aistac.handlers.abstract_handlers import HandlerFactory
-
 from ds_capability.components.discovery import DataDiscovery
 from ds_capability.intent.abstract_feature_build_intent import AbstractFeatureBuildIntentModel
 from ds_capability.intent.common_intent import CommonsIntentModel
 from ds_capability.components.commons import Commons
 from ds_capability.managers.feature_build_property_manager import FeatureBuildPropertyManager
 
 
@@ -237,28 +235,28 @@
         if drop_zero_sum:
             diff = diff.sort_values(on_key)
             diff = diff.reset_index(drop=True)
 
         return pa.Table.from_pandas(diff)
 
     def model_profiling(self, canonical: pa.Table, profiling: str, headers: [str, list]=None, drop: bool=None,
-                         dtype: [str, list]=None, exclude: bool=None, regex: [str, list]=None,
-                         re_ignore_case: bool=None, connector_name: str=None, seed: int=None, save_intent: bool=None,
-                         column_name: [int, str]=None, intent_order: int=None, replace_intent: bool=None,
-                         remove_duplicates: bool=None, **kwargs) -> pa.Table:
+                        d_type: [str, list]=None, exclude: bool=None, regex: [str, list]=None,
+                        re_ignore_case: bool=None, connector_name: str=None, seed: int=None, save_intent: bool=None,
+                        column_name: [int, str]=None, intent_order: int=None, replace_intent: bool=None,
+                        remove_duplicates: bool=None, **kwargs) -> pa.Table:
         """ Data profiling provides, analyzing, and creating useful summaries of data. The process yields a high-level
         overview which aids in the discovery of data quality issues, risks, and overall trends. It can be used to
         identify any errors, anomalies, or patterns that may exist within the data. There are three types of data
         profiling available 'dictionary', 'schema' or 'quality'
 
         :param canonical: a direct or generated pd.DataFrame. see context notes below
         :param profiling: The profiling name. Options are 'dictionary', 'schema' or 'quality'
         :param headers: (optional) a filter of headers from the 'other' dataset
         :param drop: (optional) to drop or not drop the headers if specified
-        :param dtype: (optional) a filter on data type for the 'other' dataset. int, float, bool, object
+        :param d_type: (optional) a filter on data type for the 'other' dataset. int, float, bool, object
         :param exclude: (optional) to exclude or include the data types if specified
         :param regex: (optional) a regular expression to search the headers. example '^((?!_amt).)*$)' excludes '_amt'
         :param re_ignore_case: (optional) true if the regex should ignore case. Default is False
         :param connector_name::(optional) a connector name where the outcome is sent
         :param seed:(optional) this is a placeholder, here for compatibility across methods
         :param save_intent: (optional) if the intent contract should be saved to the property manager
         :param column_name: (optional) the column name that groups intent to create a column
@@ -276,37 +274,26 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # intent action
         canonical = self._get_canonical(canonical)
-        columns = Commons.filter_headers(canonical, headers=headers, drop=drop, dtype=dtype, exclude=exclude,
-                                        regex=regex, re_ignore_case=re_ignore_case)
+        columns = Commons.filter_headers(canonical, headers=headers, drop=drop, d_type=d_type, exclude=exclude,
+                                         regex=regex, re_ignore_case=re_ignore_case)
         _seed = self._seed() if seed is None else seed
         if profiling == 'dictionary':
             result =  DataDiscovery.data_dictionary(canonical=canonical, table_cast=True, stylise=False)
         elif profiling == 'quality':
             result =  DataDiscovery.data_quality(canonical=canonical, stylise=False)
-        # elif profiling == 'schema':
-        #     blob = DataDiscovery.analyse_association(df=canonical, columns_list=columns)
-        #     report = pd.DataFrame(columns=['root', 'section', 'element', 'value'])
-        #     root_list = DataAnalytics.get_tree_roots(analytics_blob=blob)
-        #     for root_items in root_list:
-        #         data_analysis = DataAnalytics.from_root(analytics_blob=blob, root=root_items)
-        #         for section in data_analysis.section_names:
-        #             for element, value in data_analysis.get(section).items():
-        #                 to_append = [root_items, section, element, value]
-        #                 a_series = pd.Series(to_append, index=report.columns)
-        #                 report = pd.concat([report, a_series.to_frame().transpose()], ignore_index=True)
-        #     result = report
+        elif profiling == 'schema':
+            result = DataDiscovery.data_schema(canonical=canonical, stylise=False)
         else:
             raise ValueError(f"The report name '{profiling}' is not recognised. Use 'dictionary', 'schema' or 'quality'")
         if isinstance(connector_name, str):
             if self._pm.has_connector(connector_name):
                 handler = self._pm.get_connector_handler(connector_name)
                 handler.persist_canonical(result, **kwargs)
                 return canonical
             raise ValueError(f"The connector name {connector_name} has been given but no Connect Contract added")
-        # set the index
         return result
```

### Comparing `discovery-capability-0.5.2/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.5.3/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.5.3/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.5.3/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.5.3/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.5.3/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.5.3/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.5.3/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.5.3/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.5.3/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.5.3/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.5.3/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.5.3/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.5.3/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.5.3/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.5.3/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.5.3/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.5.3/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.5.3/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.5.3/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.5.3/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.5.3/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.5.3/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.5.3/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/ds_capability/sample/sample_data.py` & `discovery-capability-0.5.3/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/setup.py` & `discovery-capability-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/test/component/discovery_test.py` & `discovery-capability-0.5.3/test/component/discovery_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/test/component/synthetic_test.py` & `discovery-capability-0.5.3/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.5.3/test/intent/fb_analysis_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/test/intent/fb_correlate_intent_test.py` & `discovery-capability-0.5.3/test/intent/fb_correlate_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.5.3/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/test/intent/fb_intent_test.py` & `discovery-capability-0.5.3/test/intent/fb_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.2/test/intent/fb_model_intent_test.py` & `discovery-capability-0.5.3/test/intent/fb_model_intent_test.py`

 * *Files identical despite different names*

