# Comparing `tmp/th2_data_services-2.0.0.dev5585651073.tar.gz` & `tmp/th2_data_services-2.0.0.dev5738217622.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev5585651073.tar", last modified: Tue Jul 18 09:24:11 2023, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev5738217622.tar", last modified: Wed Aug  2 11:27:17 2023, max compression
```

## Comparing `th2_data_services-2.0.0.dev5585651073.tar` & `th2_data_services-2.0.0.dev5738217622.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23948 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-18 09:24:01.000000 th2_data_services-2.0.0.dev5585651073/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    36165 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4528 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    16098 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5425 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    14965 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    16448 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10769 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/sse_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5463 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     7000 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    29935 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    24568 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-02 11:27:05.000000 th2_data_services-2.0.0.dev5738217622/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36165 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4528 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16098 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5425 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15496 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14965 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16550 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10769 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34532 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/sse_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5463 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7000 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    29935 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev5585651073/PKG-INFO` & `th2_data_services-2.0.0.dev5738217622/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3535 3835 3635 3130 3733 0a53 756d 6d61  5585651073.Summa
+00000040: 3537 3338 3231 3736 3232 0a53 756d 6d61  5738217622.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
@@ -1774,54 +1774,98 @@
 00006ed0: 7669 6465 7229 0a20 2020 2020 2020 202d  vider).        -
 00006ee0: 205b 5468 3220 4461 7461 2053 6572 7669   [Th2 Data Servi
 00006ef0: 6365 7320 5574 696c 735d 2868 7474 7073  ces Utils](https
 00006f00: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
 00006f10: 322d 6e65 742f 7468 322d 6461 7461 2d73  2-net/th2-data-s
 00006f20: 6572 7669 6365 732d 7574 696c 7329 0a20  ervices-utils). 
 00006f30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006f40: 2320 332e 204f 6666 6963 6961 6c20 4461  # 3. Official Da
-00006f50: 7461 536f 7572 6365 2069 6d70 6c65 6d65  taSource impleme
-00006f60: 6e74 6174 696f 6e73 0a20 2020 2020 2020  ntations.       
-00006f70: 200a 2020 2020 2020 2020 2d20 5b4c 6967   .        - [Lig
-00006f80: 6874 7765 6967 6874 2044 6174 6120 5072  htweight Data Pr
-00006f90: 6f76 6964 6572 2044 6174 6120 536f 7572  ovider Data Sour
-00006fa0: 6365 5d28 6874 7470 733a 2f2f 6769 7468  ce](https://gith
-00006fb0: 7562 2e63 6f6d 2f74 6832 2d6e 6574 2f74  ub.com/th2-net/t
-00006fc0: 6832 2d64 732d 736f 7572 6365 2d6c 7764  h2-ds-source-lwd
-00006fd0: 7029 0a20 2020 2020 2020 200a 2020 2020  p).        .    
-00006fe0: 2020 2020 0a20 2020 2020 2020 2023 2034      .        # 4
-00006ff0: 2e20 4150 490a 2020 2020 2020 2020 0a20  . API.        . 
-00007000: 2020 2020 2020 2049 6620 796f 7520 6172         If you ar
-00007010: 6520 6c6f 6f6b 696e 6720 666f 7220 636c  e looking for cl
-00007020: 6173 7365 7320 6465 7363 7269 7074 696f  asses descriptio
-00007030: 6e20 7365 6520 7468 6520 5b41 5049 2044  n see the [API D
-00007040: 6f63 756d 656e 7461 7469 6f6e 5d28 646f  ocumentation](do
-00007050: 6375 6d65 6e74 6174 696f 6e2f 6170 692f  cumentation/api/
-00007060: 696e 6465 782e 6d64 292e 0a20 2020 2020  index.md)..     
-00007070: 2020 200a 2020 2020 2020 2020 2320 352e     .        # 5.
-00007080: 2045 7861 6d70 6c65 730a 2020 2020 2020   Examples.      
-00007090: 2020 0a20 2020 2020 2020 202d 205b 6765    .        - [ge
-000070a0: 745f 7374 6172 7465 645f 6578 616d 706c  t_started_exampl
-000070b0: 652e 7079 5d28 6578 616d 706c 6573 2f67  e.py](examples/g
-000070c0: 6574 5f73 7461 7274 6564 5f65 7861 6d70  et_started_examp
-000070d0: 6c65 2e70 7929 0a20 2020 2020 2020 200a  le.py).        .
-000070e0: 506c 6174 666f 726d 3a20 554e 4b4e 4f57  Platform: UNKNOW
-000070f0: 4e0a 5265 7175 6972 6573 2d50 7974 686f  N.Requires-Pytho
-00007100: 6e3a 203e 3d33 2e37 0a44 6573 6372 6970  n: >=3.7.Descrip
-00007110: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-00007120: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-00007130: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00007140: 2072 6470 0a50 726f 7669 6465 732d 4578   rdp.Provides-Ex
-00007150: 7472 613a 2072 6470 350a 5072 6f76 6964  tra: rdp5.Provid
-00007160: 6573 2d45 7874 7261 3a20 7264 7036 0a50  es-Extra: rdp6.P
-00007170: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
-00007180: 7764 700a 5072 6f76 6964 6573 2d45 7874  wdp.Provides-Ext
-00007190: 7261 3a20 6c77 6470 310a 5072 6f76 6964  ra: lwdp1.Provid
-000071a0: 6573 2d45 7874 7261 3a20 6c77 6470 320a  es-Extra: lwdp2.
-000071b0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000071c0: 6c77 6470 2d64 6576 0a50 726f 7669 6465  lwdp-dev.Provide
-000071d0: 732d 4578 7472 613a 2075 7469 6c73 2d72  s-Extra: utils-r
-000071e0: 7074 2d76 6965 7765 720a 5072 6f76 6964  pt-viewer.Provid
-000071f0: 6573 2d45 7874 7261 3a20 7574 696c 732d  es-Extra: utils-
-00007200: 7270 742d 7669 6577 6572 350a 5072 6f76  rpt-viewer5.Prov
-00007210: 6964 6573 2d45 7874 7261 3a20 7574 696c  ides-Extra: util
-00007220: 732d 6164 7661 6e63 6564 0a              s-advanced.
+00006f40: 2320 332e 2042 6573 7420 7072 6163 7469  # 3. Best practi
+00006f50: 6365 730a 2020 2020 2020 2020 4465 7065  ces.        Depe
+00006f60: 6e64 696e 6720 6f6e 2068 6f77 2079 6f75  nding on how you
+00006f70: 2077 6f72 6b20 7769 7468 2060 4461 7461   work with `Data
+00006f80: 206f 626a 6563 7460 2c20 6974 2063 616e   object`, it can
+00006f90: 2062 6520 736c 6f77 206f 6620 6661 7374   be slow of fast
+00006fa0: 2e20 200a 2020 2020 2020 2020 4173 2077  .  .        As w
+00006fb0: 6974 6820 6120 7265 6c61 7469 6f6e 616c  ith a relational
+00006fc0: 2064 6174 6162 6173 652c 2079 6f75 2063   database, you c
+00006fd0: 616e 2077 7269 7465 2061 2071 7565 7279  an write a query
+00006fe0: 2074 6861 7420 7769 6c6c 2072 6574 7572   that will retur
+00006ff0: 6e20 6461 7461 2073 6c6f 776c 7920 6f72  n data slowly or
+00007000: 2071 7569 636b 6c79 2c20 0a20 2020 2020   quickly, .     
+00007010: 2020 2074 6865 2073 616d 6520 7768 656e     the same when
+00007020: 2077 6f72 6b69 6e67 2077 6974 6820 6120   working with a 
+00007030: 6044 6174 6120 6f62 6a65 6374 602e 0a20  `Data object`.. 
+00007040: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00007050: 466f 6c6c 6f77 2074 6865 2072 756c 6573  Follow the rules
+00007060: 2074 6f20 6d61 6b65 2079 6f75 7220 776f   to make your wo
+00007070: 726b 2077 6974 6820 4461 7461 206f 626a  rk with Data obj
+00007080: 6563 7420 6661 7374 3a0a 2020 2020 2020  ect fast:.      
+00007090: 2020 312e 2055 7365 2060 4461 7461 2e75    1. Use `Data.u
+000070a0: 7365 5f63 6163 6865 2829 6020 6966 2079  se_cache()` if y
+000070b0: 6f75 2069 7465 7261 7465 2064 6174 6120  ou iterate data 
+000070c0: 6d6f 7265 2074 6861 6e20 6f6e 6520 7469  more than one ti
+000070d0: 6d65 2e0a 2020 2020 2020 2020 322e 2054  me..        2. T
+000070e0: 7279 2074 6f20 646f 6e27 7420 6974 6572  ry to don't iter
+000070f0: 6174 6520 6f6e 6520 6044 6174 6120 6f62  ate one `Data ob
+00007100: 6a65 6374 6020 696e 7369 6465 2074 6865  ject` inside the
+00007110: 206f 7468 6572 206f 6e65 2e20 200a 2020   other one.  .  
+00007120: 2020 2020 2020 2020 2049 6620 796f 7520           If you 
+00007130: 7368 6f75 6c64 2074 6f20 646f 2069 742c  should to do it,
+00007140: 2075 7365 2073 686f 7274 2060 4461 7461   use short `Data
+00007150: 206f 626a 6563 7460 2066 6972 7374 2061   object` first a
+00007160: 6e64 206c 6f6e 6720 6044 6174 6120 6f62  nd long `Data ob
+00007170: 6a65 6374 6020 696e 7369 6465 2074 6865  ject` inside the
+00007180: 206c 6f6f 702e 2020 0a20 2020 2020 2020   loop.  .       
+00007190: 2020 2020 4974 276c 6c20 616c 6c6f 7720      It'll allow 
+000071a0: 796f 7520 6f70 656e 2074 6865 2063 6163  you open the cac
+000071b0: 6865 2066 696c 6520 6f72 2063 7265 6174  he file or creat
+000071c0: 6520 6120 7265 7175 6573 7420 746f 2060  e a request to `
+000071d0: 4461 7461 2073 6f75 7263 6560 206c 6573  Data source` les
+000071e0: 7320 6e75 6d62 6572 206f 6620 7469 6d65  s number of time
+000071f0: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+00007200: 2020 2020 2320 342e 204f 6666 6963 6961      # 4. Officia
+00007210: 6c20 4461 7461 536f 7572 6365 2069 6d70  l DataSource imp
+00007220: 6c65 6d65 6e74 6174 696f 6e73 0a20 2020  lementations.   
+00007230: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00007240: 5b4c 6967 6874 7765 6967 6874 2044 6174  [Lightweight Dat
+00007250: 6120 5072 6f76 6964 6572 2044 6174 6120  a Provider Data 
+00007260: 536f 7572 6365 5d28 6874 7470 733a 2f2f  Source](https://
+00007270: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
+00007280: 6574 2f74 6832 2d64 732d 736f 7572 6365  et/th2-ds-source
+00007290: 2d6c 7764 7029 0a20 2020 2020 2020 200a  -lwdp).        .
+000072a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000072b0: 2023 2035 2e20 4150 490a 2020 2020 2020   # 5. API.      
+000072c0: 2020 0a20 2020 2020 2020 2049 6620 796f    .        If yo
+000072d0: 7520 6172 6520 6c6f 6f6b 696e 6720 666f  u are looking fo
+000072e0: 7220 636c 6173 7365 7320 6465 7363 7269  r classes descri
+000072f0: 7074 696f 6e20 7365 6520 7468 6520 5b41  ption see the [A
+00007300: 5049 2044 6f63 756d 656e 7461 7469 6f6e  PI Documentation
+00007310: 5d28 646f 6375 6d65 6e74 6174 696f 6e2f  ](documentation/
+00007320: 6170 692f 696e 6465 782e 6d64 292e 0a20  api/index.md).. 
+00007330: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00007340: 2320 362e 2045 7861 6d70 6c65 730a 2020  # 6. Examples.  
+00007350: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00007360: 205b 6765 745f 7374 6172 7465 645f 6578   [get_started_ex
+00007370: 616d 706c 652e 7079 5d28 6578 616d 706c  ample.py](exampl
+00007380: 6573 2f67 6574 5f73 7461 7274 6564 5f65  es/get_started_e
+00007390: 7861 6d70 6c65 2e70 7929 0a20 2020 2020  xample.py).     
+000073a0: 2020 200a 506c 6174 666f 726d 3a20 554e     .Platform: UN
+000073b0: 4b4e 4f57 4e0a 5265 7175 6972 6573 2d50  KNOWN.Requires-P
+000073c0: 7974 686f 6e3a 203e 3d33 2e37 0a44 6573  ython: >=3.7.Des
+000073d0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+000073e0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+000073f0: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
+00007400: 7472 613a 2072 6470 0a50 726f 7669 6465  tra: rdp.Provide
+00007410: 732d 4578 7472 613a 2072 6470 350a 5072  s-Extra: rdp5.Pr
+00007420: 6f76 6964 6573 2d45 7874 7261 3a20 7264  ovides-Extra: rd
+00007430: 7036 0a50 726f 7669 6465 732d 4578 7472  p6.Provides-Extr
+00007440: 613a 206c 7764 700a 5072 6f76 6964 6573  a: lwdp.Provides
+00007450: 2d45 7874 7261 3a20 6c77 6470 310a 5072  -Extra: lwdp1.Pr
+00007460: 6f76 6964 6573 2d45 7874 7261 3a20 6c77  ovides-Extra: lw
+00007470: 6470 320a 5072 6f76 6964 6573 2d45 7874  dp2.Provides-Ext
+00007480: 7261 3a20 6c77 6470 2d64 6576 0a50 726f  ra: lwdp-dev.Pro
+00007490: 7669 6465 732d 4578 7472 613a 2075 7469  vides-Extra: uti
+000074a0: 6c73 2d72 7074 2d76 6965 7765 720a 5072  ls-rpt-viewer.Pr
+000074b0: 6f76 6964 6573 2d45 7874 7261 3a20 7574  ovides-Extra: ut
+000074c0: 696c 732d 7270 742d 7669 6577 6572 350a  ils-rpt-viewer5.
+000074d0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+000074e0: 7574 696c 732d 6164 7661 6e63 6564 0a    utils-advanced.
```

### Comparing `th2_data_services-2.0.0.dev5585651073/README.md` & `th2_data_services-2.0.0.dev5738217622/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1471,27 +1471,66 @@
 00005be0: 2d6e 6574 2f74 6832 2d72 7074 2d64 6174  -net/th2-rpt-dat
 00005bf0: 612d 7072 6f76 6964 6572 290a 2d20 5b54  a-provider).- [T
 00005c00: 6832 2044 6174 6120 5365 7276 6963 6573  h2 Data Services
 00005c10: 2055 7469 6c73 5d28 6874 7470 733a 2f2f   Utils](https://
 00005c20: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
 00005c30: 6574 2f74 6832 2d64 6174 612d 7365 7276  et/th2-data-serv
 00005c40: 6963 6573 2d75 7469 6c73 290a 0a23 2033  ices-utils)..# 3
-00005c50: 2e20 4f66 6669 6369 616c 2044 6174 6153  . Official DataS
-00005c60: 6f75 7263 6520 696d 706c 656d 656e 7461  ource implementa
-00005c70: 7469 6f6e 730a 0a2d 205b 4c69 6768 7477  tions..- [Lightw
-00005c80: 6569 6768 7420 4461 7461 2050 726f 7669  eight Data Provi
-00005c90: 6465 7220 4461 7461 2053 6f75 7263 655d  der Data Source]
-00005ca0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00005cb0: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
-00005cc0: 6473 2d73 6f75 7263 652d 6c77 6470 290a  ds-source-lwdp).
-00005cd0: 0a0a 2320 342e 2041 5049 0a0a 4966 2079  ..# 4. API..If y
-00005ce0: 6f75 2061 7265 206c 6f6f 6b69 6e67 2066  ou are looking f
-00005cf0: 6f72 2063 6c61 7373 6573 2064 6573 6372  or classes descr
-00005d00: 6970 7469 6f6e 2073 6565 2074 6865 205b  iption see the [
-00005d10: 4150 4920 446f 6375 6d65 6e74 6174 696f  API Documentatio
-00005d20: 6e5d 2864 6f63 756d 656e 7461 7469 6f6e  n](documentation
-00005d30: 2f61 7069 2f69 6e64 6578 2e6d 6429 2e0a  /api/index.md)..
-00005d40: 0a23 2035 2e20 4578 616d 706c 6573 0a0a  .# 5. Examples..
-00005d50: 2d20 5b67 6574 5f73 7461 7274 6564 5f65  - [get_started_e
-00005d60: 7861 6d70 6c65 2e70 795d 2865 7861 6d70  xample.py](examp
-00005d70: 6c65 732f 6765 745f 7374 6172 7465 645f  les/get_started_
-00005d80: 6578 616d 706c 652e 7079 290a            example.py).
+00005c50: 2e20 4265 7374 2070 7261 6374 6963 6573  . Best practices
+00005c60: 0a44 6570 656e 6469 6e67 206f 6e20 686f  .Depending on ho
+00005c70: 7720 796f 7520 776f 726b 2077 6974 6820  w you work with 
+00005c80: 6044 6174 6120 6f62 6a65 6374 602c 2069  `Data object`, i
+00005c90: 7420 6361 6e20 6265 2073 6c6f 7720 6f66  t can be slow of
+00005ca0: 2066 6173 742e 2020 0a41 7320 7769 7468   fast.  .As with
+00005cb0: 2061 2072 656c 6174 696f 6e61 6c20 6461   a relational da
+00005cc0: 7461 6261 7365 2c20 796f 7520 6361 6e20  tabase, you can 
+00005cd0: 7772 6974 6520 6120 7175 6572 7920 7468  write a query th
+00005ce0: 6174 2077 696c 6c20 7265 7475 726e 2064  at will return d
+00005cf0: 6174 6120 736c 6f77 6c79 206f 7220 7175  ata slowly or qu
+00005d00: 6963 6b6c 792c 200a 7468 6520 7361 6d65  ickly, .the same
+00005d10: 2077 6865 6e20 776f 726b 696e 6720 7769   when working wi
+00005d20: 7468 2061 2060 4461 7461 206f 626a 6563  th a `Data objec
+00005d30: 7460 2e0a 0a46 6f6c 6c6f 7720 7468 6520  t`...Follow the 
+00005d40: 7275 6c65 7320 746f 206d 616b 6520 796f  rules to make yo
+00005d50: 7572 2077 6f72 6b20 7769 7468 2044 6174  ur work with Dat
+00005d60: 6120 6f62 6a65 6374 2066 6173 743a 0a31  a object fast:.1
+00005d70: 2e20 5573 6520 6044 6174 612e 7573 655f  . Use `Data.use_
+00005d80: 6361 6368 6528 2960 2069 6620 796f 7520  cache()` if you 
+00005d90: 6974 6572 6174 6520 6461 7461 206d 6f72  iterate data mor
+00005da0: 6520 7468 616e 206f 6e65 2074 696d 652e  e than one time.
+00005db0: 0a32 2e20 5472 7920 746f 2064 6f6e 2774  .2. Try to don't
+00005dc0: 2069 7465 7261 7465 206f 6e65 2060 4461   iterate one `Da
+00005dd0: 7461 206f 626a 6563 7460 2069 6e73 6964  ta object` insid
+00005de0: 6520 7468 6520 6f74 6865 7220 6f6e 652e  e the other one.
+00005df0: 2020 0a20 2020 4966 2079 6f75 2073 686f    .   If you sho
+00005e00: 756c 6420 746f 2064 6f20 6974 2c20 7573  uld to do it, us
+00005e10: 6520 7368 6f72 7420 6044 6174 6120 6f62  e short `Data ob
+00005e20: 6a65 6374 6020 6669 7273 7420 616e 6420  ject` first and 
+00005e30: 6c6f 6e67 2060 4461 7461 206f 626a 6563  long `Data objec
+00005e40: 7460 2069 6e73 6964 6520 7468 6520 6c6f  t` inside the lo
+00005e50: 6f70 2e20 200a 2020 2049 7427 6c6c 2061  op.  .   It'll a
+00005e60: 6c6c 6f77 2079 6f75 206f 7065 6e20 7468  llow you open th
+00005e70: 6520 6361 6368 6520 6669 6c65 206f 7220  e cache file or 
+00005e80: 6372 6561 7465 2061 2072 6571 7565 7374  create a request
+00005e90: 2074 6f20 6044 6174 6120 736f 7572 6365   to `Data source
+00005ea0: 6020 6c65 7373 206e 756d 6265 7220 6f66  ` less number of
+00005eb0: 2074 696d 6573 2e0a 0a23 2034 2e20 4f66   times...# 4. Of
+00005ec0: 6669 6369 616c 2044 6174 6153 6f75 7263  ficial DataSourc
+00005ed0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+00005ee0: 730a 0a2d 205b 4c69 6768 7477 6569 6768  s..- [Lightweigh
+00005ef0: 7420 4461 7461 2050 726f 7669 6465 7220  t Data Provider 
+00005f00: 4461 7461 2053 6f75 7263 655d 2868 7474  Data Source](htt
+00005f10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00005f20: 7468 322d 6e65 742f 7468 322d 6473 2d73  th2-net/th2-ds-s
+00005f30: 6f75 7263 652d 6c77 6470 290a 0a0a 2320  ource-lwdp)...# 
+00005f40: 352e 2041 5049 0a0a 4966 2079 6f75 2061  5. API..If you a
+00005f50: 7265 206c 6f6f 6b69 6e67 2066 6f72 2063  re looking for c
+00005f60: 6c61 7373 6573 2064 6573 6372 6970 7469  lasses descripti
+00005f70: 6f6e 2073 6565 2074 6865 205b 4150 4920  on see the [API 
+00005f80: 446f 6375 6d65 6e74 6174 696f 6e5d 2864  Documentation](d
+00005f90: 6f63 756d 656e 7461 7469 6f6e 2f61 7069  ocumentation/api
+00005fa0: 2f69 6e64 6578 2e6d 6429 2e0a 0a23 2036  /index.md)...# 6
+00005fb0: 2e20 4578 616d 706c 6573 0a0a 2d20 5b67  . Examples..- [g
+00005fc0: 6574 5f73 7461 7274 6564 5f65 7861 6d70  et_started_examp
+00005fd0: 6c65 2e70 795d 2865 7861 6d70 6c65 732f  le.py](examples/
+00005fe0: 6765 745f 7374 6172 7465 645f 6578 616d  get_started_exam
+00005ff0: 706c 652e 7079 290a                      ple.py).
```

### Comparing `th2_data_services-2.0.0.dev5585651073/setup.py` & `th2_data_services-2.0.0.dev5738217622/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/data.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/json_tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,25 +15,32 @@
 from collections import defaultdict
 from datetime import datetime
 from functools import partial
 from os import listdir, path
 from typing import List, Dict, Tuple, Callable
 
 from th2_data_services.utils.event_utils.event_utils import extract_start_timestamp
-from th2_data_services.utils.event_utils.select import get_children_from_parents_as_list, get_children_from_parent_id
+from th2_data_services.utils.event_utils.select import (
+    get_children_from_parents_as_list,
+    get_children_from_parent_id,
+)
 
 
 # TODO
 #   1. What index is?
-#   2.
+#   2. JsonTREE should become a class, from my point of view
 
 
 # NOT STREAMING
 def get_event_tree_from_parent_events(
-    events: List[Dict], parents: List[Dict], depth: int, max_children: int, body_to_simple_processors: Dict = None
+    events: List[Dict],
+    parents: List[Dict],
+    depth: int,
+    max_children: int,
+    body_to_simple_processors: Dict = None,
 ) -> Tuple[Dict, Dict]:
     """Generate tree object based on parents events list.
 
     Args:
         events (Dict[List]): TH2-Events
         parents (Dict[List]): TH2-Events
         depth (int): Max iteration
@@ -122,23 +129,29 @@
 
             if body_to_simple_processors is not None:
                 event_type = child["eventType"]
                 if event_type in body_to_simple_processors:
                     leaf["body"] = body_to_simple_processors[event_type](child["body"])
 
         current_children = get_children_from_parents_as_list(events, current_children, max_children)
-        print(f"get_event_tree_from_parent - {iteration} len_children={len(current_children)} {datetime.now()}")
+        print(
+            f"get_event_tree_from_parent - {iteration} len_children={len(current_children)} {datetime.now()}"
+        )
         iteration += 1
 
     return tree, index
 
 
 # NOT STREAMING
 def get_event_tree_from_parent_id(
-    events: List[Dict], parent_id: str, depth: int, max_children: int, body_to_simple_processors: Dict = None
+    events: List[Dict],
+    parent_id: str,
+    depth: int,
+    max_children: int,
+    body_to_simple_processors: Dict = None,
 ) -> Dict:
     """Generate tree object based on parent event id.
 
     Args:
         events (List[Dict]): TH2-Events
         parent_id (str): Parent ID
         depth (int): Max Iteration
@@ -171,15 +184,19 @@
     """
     current_children, parent = get_children_from_parent_id(events, parent_id, max_children)
     print(f"get_event_tree_from_parent - initial {datetime.now()}")
     tree, _ = get_event_tree_from_parent_events(
         events, current_children, depth, max_children, body_to_simple_processors
     )
     tree["info"].update(
-        {"name": parent["eventName"], "type": parent["eventType"], "time": extract_start_timestamp(parent)}
+        {
+            "name": parent["eventName"],
+            "type": parent["eventType"],
+            "time": extract_start_timestamp(parent),
+        }
     )
     if len(parent["body"]) != 0:
         tree["body"] = parent["body"]
 
     return tree
 
 
@@ -200,15 +217,17 @@
                               json_file_path="path/to/output.json",
                               # file_categorizer=lambda key, leaf: key
             )
     """
     path = json_file_path.replace(".json", "_summary.json")
     arranged_tree = {}
     summary = {"stats": tree["info"]["stats"]}
-    types_set = list(set((type_[: type_.index(" [")] for type_ in tree["info"]["stats"] if type_ != "TOTAL")))
+    types_set = list(
+        set((type_[: type_.index(" [")] for type_ in tree["info"]["stats"] if type_ != "TOTAL"))
+    )
     summary["types_list"] = types_set
 
     with open(path, "w") as summary_file:
         json.dump(summary, summary_file, indent=3)
 
     if file_categorizer is not None:
         for key, leaf in tree.items():
@@ -273,15 +292,17 @@
             with open(path.join(dir_path, file)) as f:
                 tree = json.load(f)
                 # TODO: Does data change here? How does this work?
                 processor(tree)
 
 
 # STREAMING
-def tree_walk(tree: Dict, processor: Callable, tree_filter: Callable = None, root_path: List = []) -> None:
+def tree_walk(
+    tree: Dict, processor: Callable, tree_filter: Callable = None, root_path: List = []
+) -> None:
     """Process tree by processor [Recursive method].
 
     Args:
         tree: TH2-Events transformed into tree (from util functions)
         processor (Callable): Processor function
         tree_filter (Callable, optional): Tree filter function. Defaults to None.
         root_path (List, optional): Root path. Defaults to [].
@@ -318,19 +339,23 @@
     Examples:
         >>> tree_walk_from_jsons(
                 path_to_json_files="path/to/files.json",
                 processor=lambda path, name, leaf: leaf.update({name: "/".join(path)}),
                 tree_filter=lambda path, name, leaf: "[fail]" in name
             )
     """
-    process_trees_from_jsons(path_pattern, lambda tree: tree_walk(tree, processor, tree_filter=tree_filter))
+    process_trees_from_jsons(
+        path_pattern, lambda tree: tree_walk(tree, processor, tree_filter=tree_filter)
+    )
 
 
 # STREAMING
-def tree_update_totals(categorizer: Callable, tree: Dict, path: List[str], name: str, leaf: Dict) -> None:
+def tree_update_totals(
+    categorizer: Callable, tree: Dict, path: List[str], name: str, leaf: Dict
+) -> None:
     """Updates tree by categorizer function as keys.
 
     Args:
         categorizer: Categorizer function
         tree: Tree
         path: Event path (from root to event)
         name: Event name
@@ -366,20 +391,24 @@
             {
                 'Outgoing message': 941,
                 'sendMessage': 95,
                 ...
             }
     """
     result = {}
-    tree_walk(tree, processor=partial(tree_update_totals, categorizer, result), tree_filter=tree_filter)
+    tree_walk(
+        tree, processor=partial(tree_update_totals, categorizer, result), tree_filter=tree_filter
+    )
     return result
 
 
 # STREAMING
-def tree_get_category_totals_from_jsons(path_pattern, categorizer: Callable, tree_filter: Callable) -> Dict:
+def tree_get_category_totals_from_jsons(
+    path_pattern, categorizer: Callable, tree_filter: Callable
+) -> Dict:
     """Returns category totals from JSON file(s).
 
     Args:
         path_pattern: Path to JSON file(s)
         categorizer: Categorizer function
         tree_filter: Tree filter function
 
@@ -388,15 +417,17 @@
 
     Examples:
         # TODO: Add example
     """
     result = {}
     process_trees_from_jsons(
         path_pattern,
-        lambda tree: tree_walk(tree, partial(tree_update_totals, categorizer, result), tree_filter=tree_filter),
+        lambda tree: tree_walk(
+            tree, partial(tree_update_totals, categorizer, result), tree_filter=tree_filter
+        ),
     )
     return result
 
 
 # NOT STREAMING
 def search_tree(tree: Dict, tree_filter: Callable[[List, str, Dict], Dict]) -> List[Dict]:
     """Searches tree by filter function.
@@ -418,15 +449,17 @@
     """
     result = []
     tree_walk(tree, lambda path, name, leaf: result.append((path, leaf)), tree_filter=tree_filter)
     return result
 
 
 # NOT STREAMING
-def search_tree_from_jsons(path_to_json_files, tree_filter: Callable[[List, str, Dict], Dict]) -> List:
+def search_tree_from_jsons(
+    path_to_json_files, tree_filter: Callable[[List, str, Dict], Dict]
+) -> List:
     """Searches tree by filter function from JSON file(s).
 
     Args:
         path_to_json_files: JSON file(s) location
         tree_filter: Filter function.
 
     Returns:
@@ -437,10 +470,12 @@
                 path_to_json_files="path/to/files.json",
                 tree_filter=lambda path, name, leaf: "[fail]" in name
             )
     """
     result = []
     process_trees_from_jsons(
         path_to_json_files,
-        lambda tree: tree_walk(tree, lambda path, name, leaf: result.append((path, leaf)), tree_filter=tree_filter),
+        lambda tree: tree_walk(
+            tree, lambda path, name, leaf: result.append((path, leaf)), tree_filter=tree_filter
+        ),
     )
     return result
```

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/misc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,48 +152,49 @@
                     if not objects_filter(expanded_object):
                         continue
 
                 if anchor == 0:
                     anchor = timestamp_function(expanded_object)
 
                 if not categories:
-                    epoch = timestamp_aggregation_key(
+                    seconds_int = timestamp_aggregation_key(
                         anchor, timestamp_function(expanded_object), aggregation_level
                     )
                     category = categorizer(expanded_object)
                     categories_set.add(category)
-                    if epoch not in frequencies:
-                        frequencies[epoch] = {category: 1}
-                    elif category not in frequencies[epoch]:
-                        frequencies[epoch][category] = 1
+                    if seconds_int not in frequencies:
+                        frequencies[seconds_int] = {category: 1}
+                    elif category not in frequencies[seconds_int]:
+                        frequencies[seconds_int][category] = 1
                     else:
-                        frequencies[epoch][category] += 1
+                        frequencies[seconds_int][category] += 1
                 else:
                     for i in range(len(categories)):
                         if categorizer(expanded_object) == categories[i]:
-                            epoch = timestamp_aggregation_key(
+                            seconds_int = timestamp_aggregation_key(
                                 anchor, timestamp_function(expanded_object), aggregation_level
                             )
-                            if epoch not in frequencies:
-                                frequencies[epoch] = [0] * len(categories)
-                            frequencies[epoch][i] += 1
+                            if seconds_int not in frequencies:
+                                frequencies[seconds_int] = [0] * len(categories)
+                            frequencies[seconds_int][i] += 1
     except KeyError:
         # Print the object if a user provided wrong categorizer.
         if obj is not None:
             print(f"Problem object: \n" f"{pprint.pformat(obj)}")
         raise
 
     header = ["timestamp"]
     if categories:
         header.extend(categories)
     else:
         header.extend(categories_set)
 
     results = [header]
     timestamps = list(sorted(frequencies.keys()))
+    # Expected that timestamp is seconds.
     for timestamp in timestamps:
         line = [datetime.fromtimestamp(timestamp, tz=timezone.utc).strftime("%Y-%m-%dT%H:%M:%S")]
         if categories:
             line.extend(frequencies[timestamp])
         else:
             for category in categories_set:
                 line.append(frequencies[timestamp][category]) if category in frequencies[
```

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/script_report_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from typing import List, Dict
 
 from th2_data_services.utils.message_utils import message_utils
 from th2_data_services.utils.event_utils import event_utils
 from datetime import datetime
-import th2_data_services.utils.az_tree
+import th2_data_services.utils.json_tree
 
 # TODO
 #   1. Takes flat_list to put result in this dict.
 #   It's better to create this dict inside and return as a result.
 #   Now don't return anything!
 from th2_data_services.utils.viewer_structs.verification import (
     verification_fields_to_flat_dict,
@@ -256,15 +256,17 @@
             return item
         if found and keys_found > 0:
             return item
 
     return None
 
 
-def find_corresponding_verification(expectation_string, verifications_list, already_used_verifications_set):  # noqa
+def find_corresponding_verification(
+    expectation_string, verifications_list, already_used_verifications_set
+):  # noqa
     # TODO: Add docstrings
     for item in verifications_list:
         found = True
         keys_found = 0
         if item[0] in already_used_verifications_set:
             continue
         tags = item[1]["body"]
@@ -316,15 +318,17 @@
     # TODO: Add docstrings
     value = formatted_val[3:]
     if " [" in value:
         value = value[: value.index(" [")]
     return value
 
 
-def extract_ids_from_dict(fields, is_this_request, is_this_verification, custom_id_tags, r_result, i_result):  # noqa
+def extract_ids_from_dict(
+    fields, is_this_request, is_this_verification, custom_id_tags, r_result, i_result
+):  # noqa
     # TODO: Add docstrings
     for id_field in custom_id_tags:
         if id_field in fields:
             v = fields[id_field]
             if is_this_verification:
                 v = get_val_from_verification(v)
             if len(v) > 3:
@@ -343,28 +347,36 @@
     i_result = {}
     for step_name, step_leaf in report_leaf.items():
         if step_name in ["info", "body"]:
             continue
         if "multiSendMessage" in step_name:
             messages = find_child_by_type(step_leaf, "Outgoing message")
             for sub_step_name, sub_step in messages:
-                extract_ids_from_dict(sub_step["body"], True, False, custom_id_tags, r_result, i_result)
+                extract_ids_from_dict(
+                    sub_step["body"], True, False, custom_id_tags, r_result, i_result
+                )
         if "place" in step_name:
             outgoing = find_child_by_type(step_leaf, "Outgoing message")
             if len(outgoing) != 0:
-                extract_ids_from_dict(outgoing[0][1]["body"], True, False, custom_id_tags, r_result, i_result)
+                extract_ids_from_dict(
+                    outgoing[0][1]["body"], True, False, custom_id_tags, r_result, i_result
+                )
             for sub_leaf_name, sub_leaf in step_leaf.items():
                 if "response" in sub_leaf_name and "Received" in sub_leaf_name:
-                    extract_ids_from_dict(sub_leaf["body"], False, False, custom_id_tags, r_result, i_result)
+                    extract_ids_from_dict(
+                        sub_leaf["body"], False, False, custom_id_tags, r_result, i_result
+                    )
         if "Check sequence rule" in step_name:
             actual_messages_leaf = find_child_by_type(step_leaf, "preFiltering")[0][1]
             for v, v_leaf in actual_messages_leaf.items():
                 if v in ["info", "body"]:
                     continue
-                extract_ids_from_dict(v_leaf["body"], False, True, custom_id_tags, r_result, i_result)
+                extract_ids_from_dict(
+                    v_leaf["body"], False, True, custom_id_tags, r_result, i_result
+                )
 
     result = {}
     result.update(r_result)
     result.update(i_result)
     return result
 
 
@@ -417,29 +429,33 @@
             request_data["TH2_event"] = step_leaf["info"]["id"]
             requests.append(request_data)
         if "multiSendMessage" in step_name:
             messages = find_child_by_type(step_leaf, "Outgoing message")
             for sub_step_name, sub_step in messages:
                 request_data = {
                     "REQ_orig_name": sub_step_name,
-                    "REQ_id": process_step_request_id(sub_step["body"], alias_by_id, custom_id_tags),
+                    "REQ_id": process_step_request_id(
+                        sub_step["body"], alias_by_id, custom_id_tags
+                    ),
                     "TH2_event": sub_step["info"]["id"],
                 }
                 request_data.update(sub_step["body"])
                 requests.append(request_data)
         if "Check sequence rule" in step_name:
             actual_messages_leaf = find_child_by_type(step_leaf, "preFiltering")[0][1]
             check_rule_actual_messages = []
             for v, v_leaf in actual_messages_leaf.items():
                 if v in ["info", "body"]:
                     continue
 
                 check_rule_actual = {"TH2_event": v_leaf["info"]["id"]}
                 if "attachedMessageIds" in v_leaf["info"]:
-                    check_rule_actual["EVN_attached_msg_id"] = v_leaf["info"]["attachedMessageIds"][0]
+                    check_rule_actual["EVN_attached_msg_id"] = v_leaf["info"]["attachedMessageIds"][
+                        0
+                    ]
                 for tag, val in v_leaf["body"].items():
                     check_rule_actual[tag] = get_val_from_verification(val)
                 check_rule_actual_messages.append(check_rule_actual)
 
             i_summary = 0
             i_extra = 0
             sequence_leaf = find_child_by_type(step_leaf, "checkSequence")[0][1]
@@ -477,17 +493,21 @@
                             "#ExpectedMessage": r["expectedMessage"],
                         }
                     else:
                         summary[summary_key] = ver[1]["body"]
                         summary[summary_key]["TH2_event"] = ver[1]["info"]["id"]
                 elif r["expectedMessage"] != "" and r["actualMessage"] == "":
                     missing_key = (
-                        str(i_summary) + " [fail] Missing " + format_expected_event(r["expectedMessage"], alias_by_id)
+                        str(i_summary)
+                        + " [fail] Missing "
+                        + format_expected_event(r["expectedMessage"], alias_by_id)
+                    )
+                    missing_filter = find_corresponding_missing_filter(
+                        r["expectedMessage"], verifications
                     )
-                    missing_filter = find_corresponding_missing_filter(r["expectedMessage"], verifications)
                     if missing_filter is None:
                         summary[missing_key] = {
                             "#Error": "Cant find corresponding filter",
                             "#ExpectedMessage": r["expectedMessage"],
                         }
                     else:
                         summary[missing_key] = missing_filter[1]["body"]
@@ -501,15 +521,17 @@
                             next_extra_found = True
                         else:
                             i_extra = i_extra + 1
                     if i_extra < len(check_rule_actual_messages):
                         extra_key = (
                             str(i_summary)
                             + " [fail] Extra "
-                            + format_actual_event(check_rule_actual_messages[i_extra], r["actualMessage"], alias_by_id)
+                            + format_actual_event(
+                                check_rule_actual_messages[i_extra], r["actualMessage"], alias_by_id
+                            )
                         )
                         summary[extra_key] = check_rule_actual_messages[i_extra]
                         i_extra = i_extra + 1
                     else:
                         extra_key = str(i_summary) + " [fail] Extra " + r["actualMessage"] + "[??]"
                         summary[extra_key] = {"#Error": "Cant find actual message"}
 
@@ -550,15 +572,15 @@
     return generate_generic_tree_and_index_from_parents_list(events, parents)
 
 
 # TODO
 #   1. Hardcoded values -- it's better to move them to function parameters with that values
 def generate_generic_tree_and_index_from_parents_list(events, parents):  # noqa
     # TODO: Add docstrings
-    tree, index = th2_data_services.utils.az_tree.get_event_tree_from_parent_events(
+    tree, index = th2_data_services.utils.json_tree.get_event_tree_from_parent_events(
         events,
         parents,
         depth=10,
         max_children=1000000,
         body_to_simple_processors={
             "Outgoing message": simplify_body_outgoing_message,
             "message": simplify_body_outgoing_message,
@@ -569,34 +591,38 @@
 
     return tree, index
 
 
 def generate_model_matrix_tree_and_index(events, parents_filter, extra=None):  # noqa
     # TODO: Add docstrings
     tree, index = generate_generic_tree_and_index(events, parents_filter)
-    th2_data_services.utils.az_tree.transform_tree(
+    th2_data_services.utils.json_tree.transform_tree(
         index,
         {
             "ModelCase": matrix_model_test_case_processor
             if extra is None
             else extra_post_processor(matrix_model_test_case_processor, extra)
         },
     )
     return tree, index
 
 
-def generate_matrix_json_report_limited_batches(events, reports_path, parents_filter, par_btch_len, extra=None):  # noqa
+def generate_matrix_json_report_limited_batches(
+    events, reports_path, parents_filter, par_btch_len, extra=None
+):  # noqa
     # TODO: Add docstrings
     post_processors = {
         "ModelCase": matrix_model_test_case_processor
         if extra is None
         else extra_post_processor(matrix_model_test_case_processor, extra)
     }
 
-    generate_generic_json_report_limited_batches(events, reports_path, parents_filter, par_btch_len, post_processors)
+    generate_generic_json_report_limited_batches(
+        events, reports_path, parents_filter, par_btch_len, post_processors
+    )
 
 
 def extra_post_processor(main_processor, extra_processor):  # noqa
     # TODO: Add docstrings
     return lambda report_leaf: extra_processor(main_processor(report_leaf))
 
 
@@ -610,46 +636,54 @@
         raise SystemError("Reports parents not found")
 
     n_steps = (len(parents) // par_btch_len) + 1
     print("Building ", len(parents), "trees in ", n_steps, " steps")
     for i in range(n_steps):
         print("Step", i + 1)
         number_base = i * par_btch_len
-        batch_end = (i + 1) * par_btch_len if (i + 1) * par_btch_len < len(parents) else len(parents)
+        batch_end = (
+            (i + 1) * par_btch_len if (i + 1) * par_btch_len < len(parents) else len(parents)
+        )
         sublist = parents[number_base:batch_end]
         tree, index = generate_generic_tree_and_index_from_parents_list(events, sublist)
         if post_processors_dict is not None:
             print("Post processing ", datetime.now())
-            th2_data_services.utils.az_tree.transform_tree(index, post_processors_dict)
+            th2_data_services.utils.json_tree.transform_tree(index, post_processors_dict)
         tree_shtrikh = {}
         for k, v in tree.items():
             if k == "info":
                 tree_shtrikh[k] = v
                 continue
 
             if " " not in k:
                 print("$$$$ " + k)
             k_shtrikh = str(int(k[: k.index(" ")]) + number_base) + k[k.index(" ") :]
             tree_shtrikh[k_shtrikh] = v
 
         print("Saving json ", datetime.now())
-        th2_data_services.utils.az_tree.save_tree_as_json(tree_shtrikh, reports_path, lambda n, l: n)
+        th2_data_services.utils.json_tree.save_tree_as_json(
+            tree_shtrikh, reports_path, lambda n, l: n
+        )
 
 
 def generate_generic_json_report(events, reports_path, parents_filter, one_file=False):  # noqa
     # TODO: Add docstrings
     tree, index = generate_generic_tree_and_index(events, parents_filter)
-    th2_data_services.utils.az_tree.save_tree_as_json(tree, reports_path, lambda n, l: "all" if one_file else n)
+    th2_data_services.utils.json_tree.save_tree_as_json(
+        tree, reports_path, lambda n, l: "all" if one_file else n
+    )
 
 
 def generate_model_matrix_json_report(events, reports_path, parents_filter, one_file=False):  # noqa
     # TODO: Add docstrings
     tree, index = generate_model_matrix_tree_and_index(events, parents_filter)
 
-    th2_data_services.utils.az_tree.save_tree_as_json(tree, reports_path, lambda n, l: "all" if one_file else n)
+    th2_data_services.utils.json_tree.save_tree_as_json(
+        tree, reports_path, lambda n, l: "all" if one_file else n
+    )
 
 
 ############################
 # PrepareStory and its functions  [start]
 ###########################
 # If I remember correct - the idea to create a function, that will help to create
 # bug reports faster!
@@ -692,15 +726,19 @@
     for s_t_n in sub_table_names:
         header.extend([s_t_n, "", " "])
     result.append(header)
     for i in range(max_keys):
         row = []
         for j in range(len(sub_table_names)):
             key = keys_lists[j][i] if i < len(keys_lists[j]) else ""
-            val = collected_data[story_item[sub_table_names[j]]][1][key] if i < len(keys_lists[j]) else ""
+            val = (
+                collected_data[story_item[sub_table_names[j]]][1][key]
+                if i < len(keys_lists[j])
+                else ""
+            )
             row.extend([key, val, " "])
         result.append(row)
     return result
 
 
 def collect_ids_for_story(story_items_list, smart, events, messages):  # noqa
     # TODO: Add docstrings
@@ -725,27 +763,33 @@
                     smart.add(v)
                 if v.startswith("event:"):
                     events.add(v)
                 if v.startswith("message:"):
                     messages.add(v)
 
 
-def prepare_story(story_items_list, json_path=None, events=None, event_body_processors=None, messages=None):  # noqa
+def prepare_story(
+    story_items_list, json_path=None, events=None, event_body_processors=None, messages=None
+):  # noqa
     # TODO: Add docstrings
     smart_report_elements_to_collect = set()
     events_to_collect = set()
     messages_to_collect = set()
 
-    collect_ids_for_story(story_items_list, smart_report_elements_to_collect, events_to_collect, messages_to_collect)
+    collect_ids_for_story(
+        story_items_list, smart_report_elements_to_collect, events_to_collect, messages_to_collect
+    )
 
     collected_data = {}
     # print(smart_report_elements_to_collect)
     if json_path is not None:
-        th2_data_services.utils.az_tree.tree_walk_from_jsons(
-            json_path, lambda p, n, l: collect_element(p, l, smart_report_elements_to_collect, collected_data), None
+        th2_data_services.utils.json_tree.tree_walk_from_jsons(
+            json_path,
+            lambda p, n, l: collect_element(p, l, smart_report_elements_to_collect, collected_data),
+            None,
         )
     if events is not None:
         # print("Collecting ", events_to_collect)
         for e in events:
             e_key = "event:" + e["eventId"]
             if e_key in events_to_collect:
                 b = e["body"]
@@ -775,15 +819,19 @@
                         }
                         b.update(message_utils.message_to_dict(m))
                         collected_data[key] = (m, b)
 
     result = []
     for item in story_items_list:
         if type(item) == str:
-            if item.startswith("smart:") or item.startswith("event:") or item.startswith("message:"):
+            if (
+                item.startswith("smart:")
+                or item.startswith("event:")
+                or item.startswith("message:")
+            ):
                 table = [["field", "value"]]
                 l = collected_data[item]
                 for k, v in l[1].items():
                     if type(v) not in [dict, list]:
                         table.append([k, str(v)])
                 result.append(table)
             elif item.startswith("message_raw:"):
@@ -874,15 +922,17 @@
         },
     },
 }
 
 
 def test_verification_fields_to_flat_dict():  # noqa
     flat_list = {}
-    verification_fields_to_flat_dict(collection=ver_dict, flat_list=flat_list, prefix="hz", failed_collection=True)
+    verification_fields_to_flat_dict(
+        collection=ver_dict, flat_list=flat_list, prefix="hz", failed_collection=True
+    )
     print(flat_list)
     """
     failed_collection=False
     {'hzField A': '   value [*]', 
      'hzField B': '!  2531410 [2531410]', 
      'hzSub message A.Field C': ' # 9 [9]'}
      
@@ -891,15 +941,17 @@
      'hzField B': '!# 2531410 [2531410]', 
      'hzSub message A.Field C': ' # 9 [9]'}
     """
 
 
 def test_verification_fields_to_simple_dict():  # noqa
     flat_list = {}
-    verification_fields_to_simple_dict(collection=ver_dict, parent=flat_list, failed_collection=True)
+    verification_fields_to_simple_dict(
+        collection=ver_dict, parent=flat_list, failed_collection=True
+    )
     print(flat_list)
     """
     failed_collection=False
     {'Field A': '   value [*]', 
      'Field B': '!  2531410 [2531410]', 
      '# Sub message A': {'Field C': ' # 9 [9]'}}
```

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3535 3835 3635 3130 3733 0a53 756d 6d61  5585651073.Summa
+00000040: 3537 3338 3231 3736 3232 0a53 756d 6d61  5738217622.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
@@ -1774,54 +1774,98 @@
 00006ed0: 7669 6465 7229 0a20 2020 2020 2020 202d  vider).        -
 00006ee0: 205b 5468 3220 4461 7461 2053 6572 7669   [Th2 Data Servi
 00006ef0: 6365 7320 5574 696c 735d 2868 7474 7073  ces Utils](https
 00006f00: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
 00006f10: 322d 6e65 742f 7468 322d 6461 7461 2d73  2-net/th2-data-s
 00006f20: 6572 7669 6365 732d 7574 696c 7329 0a20  ervices-utils). 
 00006f30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006f40: 2320 332e 204f 6666 6963 6961 6c20 4461  # 3. Official Da
-00006f50: 7461 536f 7572 6365 2069 6d70 6c65 6d65  taSource impleme
-00006f60: 6e74 6174 696f 6e73 0a20 2020 2020 2020  ntations.       
-00006f70: 200a 2020 2020 2020 2020 2d20 5b4c 6967   .        - [Lig
-00006f80: 6874 7765 6967 6874 2044 6174 6120 5072  htweight Data Pr
-00006f90: 6f76 6964 6572 2044 6174 6120 536f 7572  ovider Data Sour
-00006fa0: 6365 5d28 6874 7470 733a 2f2f 6769 7468  ce](https://gith
-00006fb0: 7562 2e63 6f6d 2f74 6832 2d6e 6574 2f74  ub.com/th2-net/t
-00006fc0: 6832 2d64 732d 736f 7572 6365 2d6c 7764  h2-ds-source-lwd
-00006fd0: 7029 0a20 2020 2020 2020 200a 2020 2020  p).        .    
-00006fe0: 2020 2020 0a20 2020 2020 2020 2023 2034      .        # 4
-00006ff0: 2e20 4150 490a 2020 2020 2020 2020 0a20  . API.        . 
-00007000: 2020 2020 2020 2049 6620 796f 7520 6172         If you ar
-00007010: 6520 6c6f 6f6b 696e 6720 666f 7220 636c  e looking for cl
-00007020: 6173 7365 7320 6465 7363 7269 7074 696f  asses descriptio
-00007030: 6e20 7365 6520 7468 6520 5b41 5049 2044  n see the [API D
-00007040: 6f63 756d 656e 7461 7469 6f6e 5d28 646f  ocumentation](do
-00007050: 6375 6d65 6e74 6174 696f 6e2f 6170 692f  cumentation/api/
-00007060: 696e 6465 782e 6d64 292e 0a20 2020 2020  index.md)..     
-00007070: 2020 200a 2020 2020 2020 2020 2320 352e     .        # 5.
-00007080: 2045 7861 6d70 6c65 730a 2020 2020 2020   Examples.      
-00007090: 2020 0a20 2020 2020 2020 202d 205b 6765    .        - [ge
-000070a0: 745f 7374 6172 7465 645f 6578 616d 706c  t_started_exampl
-000070b0: 652e 7079 5d28 6578 616d 706c 6573 2f67  e.py](examples/g
-000070c0: 6574 5f73 7461 7274 6564 5f65 7861 6d70  et_started_examp
-000070d0: 6c65 2e70 7929 0a20 2020 2020 2020 200a  le.py).        .
-000070e0: 506c 6174 666f 726d 3a20 554e 4b4e 4f57  Platform: UNKNOW
-000070f0: 4e0a 5265 7175 6972 6573 2d50 7974 686f  N.Requires-Pytho
-00007100: 6e3a 203e 3d33 2e37 0a44 6573 6372 6970  n: >=3.7.Descrip
-00007110: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-00007120: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-00007130: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00007140: 2072 6470 0a50 726f 7669 6465 732d 4578   rdp.Provides-Ex
-00007150: 7472 613a 2072 6470 350a 5072 6f76 6964  tra: rdp5.Provid
-00007160: 6573 2d45 7874 7261 3a20 7264 7036 0a50  es-Extra: rdp6.P
-00007170: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
-00007180: 7764 700a 5072 6f76 6964 6573 2d45 7874  wdp.Provides-Ext
-00007190: 7261 3a20 6c77 6470 310a 5072 6f76 6964  ra: lwdp1.Provid
-000071a0: 6573 2d45 7874 7261 3a20 6c77 6470 320a  es-Extra: lwdp2.
-000071b0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000071c0: 6c77 6470 2d64 6576 0a50 726f 7669 6465  lwdp-dev.Provide
-000071d0: 732d 4578 7472 613a 2075 7469 6c73 2d72  s-Extra: utils-r
-000071e0: 7074 2d76 6965 7765 720a 5072 6f76 6964  pt-viewer.Provid
-000071f0: 6573 2d45 7874 7261 3a20 7574 696c 732d  es-Extra: utils-
-00007200: 7270 742d 7669 6577 6572 350a 5072 6f76  rpt-viewer5.Prov
-00007210: 6964 6573 2d45 7874 7261 3a20 7574 696c  ides-Extra: util
-00007220: 732d 6164 7661 6e63 6564 0a              s-advanced.
+00006f40: 2320 332e 2042 6573 7420 7072 6163 7469  # 3. Best practi
+00006f50: 6365 730a 2020 2020 2020 2020 4465 7065  ces.        Depe
+00006f60: 6e64 696e 6720 6f6e 2068 6f77 2079 6f75  nding on how you
+00006f70: 2077 6f72 6b20 7769 7468 2060 4461 7461   work with `Data
+00006f80: 206f 626a 6563 7460 2c20 6974 2063 616e   object`, it can
+00006f90: 2062 6520 736c 6f77 206f 6620 6661 7374   be slow of fast
+00006fa0: 2e20 200a 2020 2020 2020 2020 4173 2077  .  .        As w
+00006fb0: 6974 6820 6120 7265 6c61 7469 6f6e 616c  ith a relational
+00006fc0: 2064 6174 6162 6173 652c 2079 6f75 2063   database, you c
+00006fd0: 616e 2077 7269 7465 2061 2071 7565 7279  an write a query
+00006fe0: 2074 6861 7420 7769 6c6c 2072 6574 7572   that will retur
+00006ff0: 6e20 6461 7461 2073 6c6f 776c 7920 6f72  n data slowly or
+00007000: 2071 7569 636b 6c79 2c20 0a20 2020 2020   quickly, .     
+00007010: 2020 2074 6865 2073 616d 6520 7768 656e     the same when
+00007020: 2077 6f72 6b69 6e67 2077 6974 6820 6120   working with a 
+00007030: 6044 6174 6120 6f62 6a65 6374 602e 0a20  `Data object`.. 
+00007040: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00007050: 466f 6c6c 6f77 2074 6865 2072 756c 6573  Follow the rules
+00007060: 2074 6f20 6d61 6b65 2079 6f75 7220 776f   to make your wo
+00007070: 726b 2077 6974 6820 4461 7461 206f 626a  rk with Data obj
+00007080: 6563 7420 6661 7374 3a0a 2020 2020 2020  ect fast:.      
+00007090: 2020 312e 2055 7365 2060 4461 7461 2e75    1. Use `Data.u
+000070a0: 7365 5f63 6163 6865 2829 6020 6966 2079  se_cache()` if y
+000070b0: 6f75 2069 7465 7261 7465 2064 6174 6120  ou iterate data 
+000070c0: 6d6f 7265 2074 6861 6e20 6f6e 6520 7469  more than one ti
+000070d0: 6d65 2e0a 2020 2020 2020 2020 322e 2054  me..        2. T
+000070e0: 7279 2074 6f20 646f 6e27 7420 6974 6572  ry to don't iter
+000070f0: 6174 6520 6f6e 6520 6044 6174 6120 6f62  ate one `Data ob
+00007100: 6a65 6374 6020 696e 7369 6465 2074 6865  ject` inside the
+00007110: 206f 7468 6572 206f 6e65 2e20 200a 2020   other one.  .  
+00007120: 2020 2020 2020 2020 2049 6620 796f 7520           If you 
+00007130: 7368 6f75 6c64 2074 6f20 646f 2069 742c  should to do it,
+00007140: 2075 7365 2073 686f 7274 2060 4461 7461   use short `Data
+00007150: 206f 626a 6563 7460 2066 6972 7374 2061   object` first a
+00007160: 6e64 206c 6f6e 6720 6044 6174 6120 6f62  nd long `Data ob
+00007170: 6a65 6374 6020 696e 7369 6465 2074 6865  ject` inside the
+00007180: 206c 6f6f 702e 2020 0a20 2020 2020 2020   loop.  .       
+00007190: 2020 2020 4974 276c 6c20 616c 6c6f 7720      It'll allow 
+000071a0: 796f 7520 6f70 656e 2074 6865 2063 6163  you open the cac
+000071b0: 6865 2066 696c 6520 6f72 2063 7265 6174  he file or creat
+000071c0: 6520 6120 7265 7175 6573 7420 746f 2060  e a request to `
+000071d0: 4461 7461 2073 6f75 7263 6560 206c 6573  Data source` les
+000071e0: 7320 6e75 6d62 6572 206f 6620 7469 6d65  s number of time
+000071f0: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+00007200: 2020 2020 2320 342e 204f 6666 6963 6961      # 4. Officia
+00007210: 6c20 4461 7461 536f 7572 6365 2069 6d70  l DataSource imp
+00007220: 6c65 6d65 6e74 6174 696f 6e73 0a20 2020  lementations.   
+00007230: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00007240: 5b4c 6967 6874 7765 6967 6874 2044 6174  [Lightweight Dat
+00007250: 6120 5072 6f76 6964 6572 2044 6174 6120  a Provider Data 
+00007260: 536f 7572 6365 5d28 6874 7470 733a 2f2f  Source](https://
+00007270: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
+00007280: 6574 2f74 6832 2d64 732d 736f 7572 6365  et/th2-ds-source
+00007290: 2d6c 7764 7029 0a20 2020 2020 2020 200a  -lwdp).        .
+000072a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000072b0: 2023 2035 2e20 4150 490a 2020 2020 2020   # 5. API.      
+000072c0: 2020 0a20 2020 2020 2020 2049 6620 796f    .        If yo
+000072d0: 7520 6172 6520 6c6f 6f6b 696e 6720 666f  u are looking fo
+000072e0: 7220 636c 6173 7365 7320 6465 7363 7269  r classes descri
+000072f0: 7074 696f 6e20 7365 6520 7468 6520 5b41  ption see the [A
+00007300: 5049 2044 6f63 756d 656e 7461 7469 6f6e  PI Documentation
+00007310: 5d28 646f 6375 6d65 6e74 6174 696f 6e2f  ](documentation/
+00007320: 6170 692f 696e 6465 782e 6d64 292e 0a20  api/index.md).. 
+00007330: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00007340: 2320 362e 2045 7861 6d70 6c65 730a 2020  # 6. Examples.  
+00007350: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00007360: 205b 6765 745f 7374 6172 7465 645f 6578   [get_started_ex
+00007370: 616d 706c 652e 7079 5d28 6578 616d 706c  ample.py](exampl
+00007380: 6573 2f67 6574 5f73 7461 7274 6564 5f65  es/get_started_e
+00007390: 7861 6d70 6c65 2e70 7929 0a20 2020 2020  xample.py).     
+000073a0: 2020 200a 506c 6174 666f 726d 3a20 554e     .Platform: UN
+000073b0: 4b4e 4f57 4e0a 5265 7175 6972 6573 2d50  KNOWN.Requires-P
+000073c0: 7974 686f 6e3a 203e 3d33 2e37 0a44 6573  ython: >=3.7.Des
+000073d0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+000073e0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+000073f0: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
+00007400: 7472 613a 2072 6470 0a50 726f 7669 6465  tra: rdp.Provide
+00007410: 732d 4578 7472 613a 2072 6470 350a 5072  s-Extra: rdp5.Pr
+00007420: 6f76 6964 6573 2d45 7874 7261 3a20 7264  ovides-Extra: rd
+00007430: 7036 0a50 726f 7669 6465 732d 4578 7472  p6.Provides-Extr
+00007440: 613a 206c 7764 700a 5072 6f76 6964 6573  a: lwdp.Provides
+00007450: 2d45 7874 7261 3a20 6c77 6470 310a 5072  -Extra: lwdp1.Pr
+00007460: 6f76 6964 6573 2d45 7874 7261 3a20 6c77  ovides-Extra: lw
+00007470: 6470 320a 5072 6f76 6964 6573 2d45 7874  dp2.Provides-Ext
+00007480: 7261 3a20 6c77 6470 2d64 6576 0a50 726f  ra: lwdp-dev.Pro
+00007490: 7669 6465 732d 4578 7472 613a 2075 7469  vides-Extra: uti
+000074a0: 6c73 2d72 7074 2d76 6965 7765 720a 5072  ls-rpt-viewer.Pr
+000074b0: 6f76 6964 6573 2d45 7874 7261 3a20 7574  ovides-Extra: ut
+000074c0: 696c 732d 7270 742d 7669 6577 6572 350a  ils-rpt-viewer5.
+000074d0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+000074e0: 7574 696c 732d 6164 7661 6e63 6564 0a    utils-advanced.
```

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

