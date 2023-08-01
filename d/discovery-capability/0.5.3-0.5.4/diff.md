# Comparing `tmp/discovery-capability-0.5.3.tar.gz` & `tmp/discovery-capability-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.5.3.tar", last modified: Tue Aug  1 23:06:59 2023, max compression
+gzip compressed data, was "discovery-capability-0.5.4.tar", last modified: Tue Aug  1 23:21:33 2023, max compression
```

## Comparing `discovery-capability-0.5.3.tar` & `discovery-capability-0.5.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.983235 discovery-capability-0.5.3/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.3/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.3/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-01 23:06:59.983548 discovery-capability-0.5.3/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.3/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.824773 discovery-capability-0.5.3/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-01 23:06:59.000000 discovery-capability-0.5.3/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     2353 2023-08-01 23:06:59.000000 discovery-capability-0.5.3/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-01 23:06:59.000000 discovery-capability-0.5.3/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-08-01 23:06:59.000000 discovery-capability-0.5.3/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-08-01 23:06:59.000000 discovery-capability-0.5.3/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.825168 discovery-capability-0.5.3/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-08-01 15:56:54.000000 discovery-capability-0.5.3/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.828684 discovery-capability-0.5.3/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.3/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13234 2023-08-01 16:23:26.000000 discovery-capability-0.5.3/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.3/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)    20338 2023-08-01 15:46:02.000000 discovery-capability-0.5.3/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.5.3/ds_capability/components/feature_build.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.829540 discovery-capability-0.5.3/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.3/ds_capability/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.835373 discovery-capability-0.5.3/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.3/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.3/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.3/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11239 2023-07-30 18:52:11.000000 discovery-capability-0.5.3/ds_capability/intent/feature_build_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    68101 2023-07-28 18:34:45.000000 discovery-capability-0.5.3/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    20073 2023-08-01 22:56:33.000000 discovery-capability-0.5.3/ds_capability/intent/feature_build_model_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.839527 discovery-capability-0.5.3/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.3/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.3/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.3/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.3/ds_capability/managers/feature_select_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.972256 discovery-capability-0.5.3/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.3/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.3/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-08-01 23:06:59.984563 discovery-capability-0.5.3/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.5.3/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.973330 discovery-capability-0.5.3/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.3/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.974864 discovery-capability-0.5.3/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.3/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3127 2023-08-01 15:50:17.000000 discovery-capability-0.5.3/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.3/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.975757 discovery-capability-0.5.3/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.3/test/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:06:59.980856 discovery-capability-0.5.3/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.3/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.3/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3099 2023-07-29 22:54:26.000000 discovery-capability-0.5.3/test/intent/fb_correlate_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.3/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-29 21:30:04.000000 discovery-capability-0.5.3/test/intent/fb_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.3/test/intent/fb_model_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:21:33.362438 discovery-capability-0.5.4/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.4/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.4/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-01 23:21:33.362750 discovery-capability-0.5.4/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.4/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:21:33.227442 discovery-capability-0.5.4/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-01 23:21:33.000000 discovery-capability-0.5.4/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     2353 2023-08-01 23:21:33.000000 discovery-capability-0.5.4/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-01 23:21:33.000000 discovery-capability-0.5.4/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-08-01 23:21:33.000000 discovery-capability-0.5.4/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-08-01 23:21:33.000000 discovery-capability-0.5.4/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:21:33.228022 discovery-capability-0.5.4/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-08-01 23:21:08.000000 discovery-capability-0.5.4/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:21:33.231322 discovery-capability-0.5.4/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.4/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13234 2023-08-01 16:23:26.000000 discovery-capability-0.5.4/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.4/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20338 2023-08-01 15:46:02.000000 discovery-capability-0.5.4/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.5.4/ds_capability/components/feature_build.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:21:33.232046 discovery-capability-0.5.4/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.4/ds_capability/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:21:33.236064 discovery-capability-0.5.4/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.4/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.4/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.4/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11239 2023-07-30 18:52:11.000000 discovery-capability-0.5.4/ds_capability/intent/feature_build_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    68101 2023-07-28 18:34:45.000000 discovery-capability-0.5.4/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20077 2023-08-01 23:18:03.000000 discovery-capability-0.5.4/ds_capability/intent/feature_build_model_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:21:33.238727 discovery-capability-0.5.4/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.4/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.4/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.4/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.4/ds_capability/managers/feature_select_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:21:33.352896 discovery-capability-0.5.4/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.4/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.4/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-08-01 23:21:33.363838 discovery-capability-0.5.4/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.5.4/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:21:33.353954 discovery-capability-0.5.4/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.4/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:21:33.355698 discovery-capability-0.5.4/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.4/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3127 2023-08-01 15:50:17.000000 discovery-capability-0.5.4/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.4/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:21:33.356726 discovery-capability-0.5.4/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.4/test/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 23:21:33.361788 discovery-capability-0.5.4/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.4/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.4/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3099 2023-07-29 22:54:26.000000 discovery-capability-0.5.4/test/intent/fb_correlate_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.4/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-29 21:30:04.000000 discovery-capability-0.5.4/test/intent/fb_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.4/test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.5.3/LICENSE.txt` & `discovery-capability-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/PKG-INFO` & `discovery-capability-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.5.3
+Version: 0.5.4
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.5.3/README.rst` & `discovery-capability-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.5.4/discovery_capability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.5.3
+Version: 0.5.4
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.5.3/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.5.4/discovery_capability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.5.4/ds_capability/components/abstract_common_component.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/components/commons.py` & `discovery-capability-0.5.4/ds_capability/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/components/discovery.py` & `discovery-capability-0.5.4/ds_capability/components/discovery.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/components/feature_build.py` & `discovery-capability-0.5.4/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.5.4/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/intent/common_intent.py` & `discovery-capability-0.5.4/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/intent/feature_build_correlate_intent.py` & `discovery-capability-0.5.4/ds_capability/intent/feature_build_correlate_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.5.4/ds_capability/intent/feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/intent/feature_build_model_intent.py` & `discovery-capability-0.5.4/ds_capability/intent/feature_build_model_intent.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,28 +235,28 @@
         if drop_zero_sum:
             diff = diff.sort_values(on_key)
             diff = diff.reset_index(drop=True)
 
         return pa.Table.from_pandas(diff)
 
     def model_profiling(self, canonical: pa.Table, profiling: str, headers: [str, list]=None, drop: bool=None,
-                        d_type: [str, list]=None, exclude: bool=None, regex: [str, list]=None,
+                        d_types: [str, list]=None, exclude: bool=None, regex: [str, list]=None,
                         re_ignore_case: bool=None, connector_name: str=None, seed: int=None, save_intent: bool=None,
                         column_name: [int, str]=None, intent_order: int=None, replace_intent: bool=None,
                         remove_duplicates: bool=None, **kwargs) -> pa.Table:
         """ Data profiling provides, analyzing, and creating useful summaries of data. The process yields a high-level
         overview which aids in the discovery of data quality issues, risks, and overall trends. It can be used to
         identify any errors, anomalies, or patterns that may exist within the data. There are three types of data
         profiling available 'dictionary', 'schema' or 'quality'
 
         :param canonical: a direct or generated pd.DataFrame. see context notes below
         :param profiling: The profiling name. Options are 'dictionary', 'schema' or 'quality'
         :param headers: (optional) a filter of headers from the 'other' dataset
         :param drop: (optional) to drop or not drop the headers if specified
-        :param d_type: (optional) a filter on data type for the 'other' dataset. int, float, bool, object
+        :param d_types: (optional) a filter on data type for the 'other' dataset. int, float, bool, object
         :param exclude: (optional) to exclude or include the data types if specified
         :param regex: (optional) a regular expression to search the headers. example '^((?!_amt).)*$)' excludes '_amt'
         :param re_ignore_case: (optional) true if the regex should ignore case. Default is False
         :param connector_name::(optional) a connector name where the outcome is sent
         :param seed:(optional) this is a placeholder, here for compatibility across methods
         :param save_intent: (optional) if the intent contract should be saved to the property manager
         :param column_name: (optional) the column name that groups intent to create a column
@@ -274,15 +274,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # intent action
         canonical = self._get_canonical(canonical)
-        columns = Commons.filter_headers(canonical, headers=headers, drop=drop, d_type=d_type, exclude=exclude,
+        columns = Commons.filter_headers(canonical, headers=headers, drop=drop, d_types=d_types, exclude=exclude,
                                          regex=regex, re_ignore_case=re_ignore_case)
         _seed = self._seed() if seed is None else seed
         if profiling == 'dictionary':
             result =  DataDiscovery.data_dictionary(canonical=canonical, table_cast=True, stylise=False)
         elif profiling == 'quality':
             result =  DataDiscovery.data_quality(canonical=canonical, stylise=False)
         elif profiling == 'schema':
```

### Comparing `discovery-capability-0.5.3/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.5.4/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.5.4/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.5.4/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.5.4/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.5.4/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.5.4/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.5.4/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.5.4/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.5.4/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.5.4/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.5.4/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.5.4/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.5.4/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.5.4/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.5.4/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.5.4/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.5.4/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.5.4/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.5.4/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.5.4/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.5.4/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.5.4/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.5.4/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/ds_capability/sample/sample_data.py` & `discovery-capability-0.5.4/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/setup.py` & `discovery-capability-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/test/component/discovery_test.py` & `discovery-capability-0.5.4/test/component/discovery_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/test/component/synthetic_test.py` & `discovery-capability-0.5.4/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.5.4/test/intent/fb_analysis_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/test/intent/fb_correlate_intent_test.py` & `discovery-capability-0.5.4/test/intent/fb_correlate_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.5.4/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/test/intent/fb_intent_test.py` & `discovery-capability-0.5.4/test/intent/fb_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.3/test/intent/fb_model_intent_test.py` & `discovery-capability-0.5.4/test/intent/fb_model_intent_test.py`

 * *Files identical despite different names*

