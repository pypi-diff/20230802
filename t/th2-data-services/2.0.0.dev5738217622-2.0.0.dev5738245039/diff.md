# Comparing `tmp/th2_data_services-2.0.0.dev5738217622.tar.gz` & `tmp/th2_data_services-2.0.0.dev5738245039.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev5738217622.tar", last modified: Wed Aug  2 11:27:17 2023, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev5738245039.tar", last modified: Wed Aug  2 11:32:49 2023, max compression
```

## Comparing `th2_data_services-2.0.0.dev5738217622.tar` & `th2_data_services-2.0.0.dev5738245039.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    29935 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24568 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-02 11:27:05.000000 th2_data_services-2.0.0.dev5738217622/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    36165 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4528 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    16098 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5425 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    15496 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    14965 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    16550 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10769 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    34532 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/sse_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5463 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     7000 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-08-02 11:26:01.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    29935 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-08-02 11:27:17.000000 th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    30034 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    24651 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-02 11:32:36.000000 th2_data_services-2.0.0.dev5738245039/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36165 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4528 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16098 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5425 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15496 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14965 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16550 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10769 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34532 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/sse_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5463 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7000 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-08-02 11:29:33.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    30034 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-08-02 11:32:49.000000 th2_data_services-2.0.0.dev5738245039/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev5738217622/PKG-INFO` & `th2_data_services-2.0.0.dev5738245039/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3537 3338 3231 3736 3232 0a53 756d 6d61  5738217622.Summa
+00000040: 3537 3338 3234 3530 3339 0a53 756d 6d61  5738245039.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
@@ -89,1783 +89,1790 @@
 00000580: 6e74 5472 6565 5d28 2365 7665 6e74 7472  ntTree](#eventtr
 00000590: 6565 290a 2020 2020 2020 2020 2020 2020  ee).            
 000005a0: 2020 2020 202a 205b 436f 6c6c 6563 7469       * [Collecti
 000005b0: 6f6e 735d 2823 636f 6c6c 6563 7469 6f6e  ons](#collection
 000005c0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
 000005d0: 2020 2020 2a20 5b48 696e 7473 5d28 2368      * [Hints](#h
 000005e0: 696e 7473 290a 2020 2020 2020 2020 2020  ints).          
-000005f0: 202a 205b 322e 342e 204c 696e 6b73 5d28   * [2.4. Links](
-00000600: 2332 342d 6c69 6e6b 7329 0a20 2020 2020  #24-links).     
-00000610: 2020 202a 205b 332e 204f 6666 6963 6961     * [3. Officia
-00000620: 6c20 4461 7461 536f 7572 6365 2069 6d70  l DataSource imp
-00000630: 6c65 6d65 6e74 6174 696f 6e73 5d28 2333  lementations](#3
-00000640: 2d6f 6666 6963 6961 6c2d 6461 7461 736f  -official-dataso
-00000650: 7572 6365 2d69 6d70 6c65 6d65 6e74 6174  urce-implementat
-00000660: 696f 6e73 290a 2020 2020 2020 2020 2a20  ions).        * 
-00000670: 5b34 2e20 4150 495d 2823 342d 6170 6929  [4. API](#4-api)
-00000680: 0a20 2020 2020 2020 202a 205b 352e 2045  .        * [5. E
-00000690: 7861 6d70 6c65 735d 2823 352d 6578 616d  xamples](#5-exam
-000006a0: 706c 6573 290a 2020 2020 2020 2020 3c21  ples).        <!
-000006b0: 2d2d 7465 2d2d 3e0a 2020 2020 2020 2020  --te-->.        
-000006c0: 0a20 2020 2020 2020 2023 2031 2e20 496e  .        # 1. In
-000006d0: 7472 6f64 7563 7469 6f6e 0a20 2020 2020  troduction.     
-000006e0: 2020 200a 2020 2020 2020 2020 5468 6973     .        This
-000006f0: 2072 6570 6f73 6974 6f72 7920 6973 2061   repository is a
-00000700: 206c 6962 7261 7279 2066 6f72 2063 7265   library for cre
-00000710: 6174 696e 6720 7468 322d 6461 7461 2d73  ating th2-data-s
-00000720: 6572 7669 6365 7320 6170 706c 6963 6174  ervices applicat
-00000730: 696f 6e73 2e0a 2020 2020 2020 2020 4461  ions..        Da
-00000740: 7461 2053 6572 7669 6365 7320 616c 6c6f  ta Services allo
-00000750: 7773 2079 6f75 2074 6f20 6d61 6e69 7075  ws you to manipu
-00000760: 6c61 7465 2074 6865 2073 7472 6561 6d20  late the stream 
-00000770: 6461 7461 2070 726f 6365 7373 696e 6720  data processing 
-00000780: 776f 726b 666c 6f77 2075 7369 6e67 2070  workflow using p
-00000790: 6970 656c 696e 696e 672e 0a20 2020 2020  ipelining..     
-000007a0: 2020 200a 2020 2020 2020 2020 5468 6520     .        The 
-000007b0: 6c69 6272 6172 7927 7320 6665 6174 7572  library's featur
-000007c0: 6573 3a0a 2020 2020 2020 2020 0a20 2020  es:.        .   
-000007d0: 2020 2020 202d 2050 726f 7669 6465 7320       - Provides 
-000007e0: 636f 7265 2069 6e74 6572 6661 6365 2066  core interface f
-000007f0: 6f72 2064 6576 656c 6f70 696e 6720 6461  or developing da
-00000800: 7461 2073 6f75 7263 6520 696d 706c 656d  ta source implem
-00000810: 656e 7461 7469 6f6e 730a 2020 2020 2020  entations.      
-00000820: 2020 2d20 576f 726b 2077 6974 6820 6974    - Work with it
-00000830: 6572 6162 6c65 206f 626a 6563 7473 2028  erable objects (
-00000840: 6c69 7374 2c20 7475 706c 652c 2065 7463  list, tuple, etc
-00000850: 2069 6e63 6c75 6469 6e67 2066 696c 6573   including files
-00000860: 2920 7669 6120 5f44 6174 6120 6f62 6a65  ) via _Data obje
-00000870: 6374 5f20 7573 696e 6720 6974 7320 6665  ct_ using its fe
-00000880: 6174 7572 6573 0a20 2020 2020 2020 202d  atures.        -
-00000890: 204d 616e 6970 756c 6174 6520 7468 6520   Manipulate the 
-000008a0: 776f 726b 666c 6f77 2074 6f20 6d61 6b65  workflow to make
-000008b0: 2073 6f6d 6520 616e 616c 7973 6973 2062   some analysis b
-000008c0: 7920 5f44 6174 6120 6f62 6a65 6374 5f20  y _Data object_ 
-000008d0: 6d65 7468 6f64 730a 2020 2020 2020 2020  methods.        
-000008e0: 2d20 5573 6520 7469 6d65 7374 616d 7020  - Use timestamp 
-000008f0: 636f 6e76 6572 7465 7220 696d 706c 656d  converter implem
-00000900: 656e 7461 7469 6f6e 7320 6f72 2075 7365  entations or use
-00000910: 2062 6173 6520 636c 6173 7320 746f 2063   base class to c
-00000920: 7265 6174 6520 6375 7374 6f6d 2063 6f6e  reate custom con
-00000930: 7665 7274 6572 730a 2020 2020 2020 2020  verters.        
-00000940: 2d20 4275 696c 6420 4576 656e 7420 5472  - Build Event Tr
-00000950: 6565 7320 2845 7665 6e74 5472 6565 2c20  ees (EventTree, 
-00000960: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
-00000970: 696f 6e20 616e 6420 5061 7265 6e74 4576  ion and ParentEv
-00000980: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00000990: 6e20 636c 6173 7365 7329 0a20 2020 2020  n classes).     
-000009a0: 2020 200a 2020 2020 2020 2020 576f 726b     .        Work
-000009b0: 666c 6f77 206d 616e 6970 756c 6174 696f  flow manipulatio
-000009c0: 6e20 746f 6f6c 7320 616c 6c6f 7773 2079  n tools allows y
-000009d0: 6f75 3a0a 2020 2020 2020 2020 0a20 2020  ou:.        .   
-000009e0: 2020 2020 202d 2046 696c 7465 7269 6e67       - Filtering
-000009f0: 2073 7472 6561 6d20 6461 7461 2028 6044   stream data (`D
-00000a00: 6174 612e 6669 6c74 6572 6020 6d65 7468  ata.filter` meth
-00000a10: 6f64 290a 2020 2020 2020 2020 2d20 5472  od).        - Tr
-00000a20: 616e 7366 6f72 6d69 6e67 2073 7472 6561  ansforming strea
-00000a30: 6d20 6461 7461 2028 6044 6174 612e 6d61  m data (`Data.ma
-00000a40: 7060 206d 6574 686f 6429 0a20 2020 2020  p` method).     
-00000a50: 2020 202d 204c 696d 6974 696e 6720 7468     - Limiting th
-00000a60: 6520 6e75 6d62 6572 206f 6620 7072 6f63  e number of proc
-00000a70: 6573 7365 6420 7374 7265 616d 696e 6720  essed streaming 
-00000a80: 6461 7461 2028 6044 6174 612e 6c69 6d69  data (`Data.limi
-00000a90: 7460 206d 6574 686f 6429 0a20 2020 2020  t` method).     
-00000aa0: 2020 200a 2020 2020 2020 2020 5468 6572     .        Ther
-00000ab0: 6520 6973 2061 6c73 6f20 616e 6f74 6865  e is also anothe
-00000ac0: 7220 7061 7274 206f 6620 5f64 6174 6120  r part of _data 
-00000ad0: 7365 7276 6963 6573 5f0a 2020 2020 2020  services_.      
-00000ae0: 2020 0a20 2020 2020 2020 202d 205b 7468    .        - [th
-00000af0: 322d 6461 7461 2d73 6572 7669 6365 732d  2-data-services-
-00000b00: 7574 696c 735d 2868 7474 7073 3a2f 2f67  utils](https://g
-00000b10: 6974 6875 622e 636f 6d2f 7468 322d 6e65  ithub.com/th2-ne
-00000b20: 742f 7468 322d 6461 7461 2d73 6572 7669  t/th2-data-servi
-00000b30: 6365 732d 7574 696c 7329 2e20 4974 2773  ces-utils). It's
-00000b40: 2061 2073 6574 206f 6620 746f 6f6c 7320   a set of tools 
-00000b50: 746f 2070 6572 666f 726d 2074 6865 206d  to perform the m
-00000b60: 6f73 740a 2020 2020 2020 2020 2020 636f  ost.          co
-00000b70: 6d6d 6f6e 2061 6e61 6c79 7369 7320 7461  mmon analysis ta
-00000b80: 736b 732e 0a20 2020 2020 2020 200a 2020  sks..        .  
-00000b90: 2020 2020 2020 2320 322e 2047 6574 7469        # 2. Getti
-00000ba0: 6e67 2073 7461 7274 6564 0a20 2020 2020  ng started.     
-00000bb0: 2020 200a 2020 2020 2020 2020 2323 2032     .        ## 2
-00000bc0: 2e31 2e20 496e 7374 616c 6c61 7469 6f6e  .1. Installation
-00000bd0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000be0: 2020 2323 2320 436f 7265 0a20 2020 2020    ### Core.     
-00000bf0: 2020 200a 2020 2020 2020 2020 2d20 4672     .        - Fr
-00000c00: 6f6d 2050 7950 4920 2870 6970 2920 2020  om PyPI (pip)   
-00000c10: 0a20 2020 2020 2020 2020 2054 6869 7320  .          This 
-00000c20: 7061 636b 6167 6520 6361 6e20 6265 2066  package can be f
-00000c30: 6f75 6e64 206f 6e20 5b50 7950 495d 2868  ound on [PyPI](h
-00000c40: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000c50: 7072 6f6a 6563 742f 7468 322d 6461 7461  project/th2-data
-00000c60: 2d73 6572 7669 6365 732f 2022 7468 322d  -services/ "th2-
-00000c70: 6461 7461 2d73 6572 7669 6365 7322 292e  data-services").
-00000c80: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
-00000c90: 0a20 2020 2020 2020 2020 2020 2070 6970  .            pip
-00000ca0: 2069 6e73 7461 6c6c 2074 6832 2d64 6174   install th2-dat
-00000cb0: 612d 7365 7276 6963 6573 0a20 2020 2020  a-services.     
-00000cc0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00000cd0: 2020 200a 2020 2020 2020 2020 2d20 4672     .        - Fr
-00000ce0: 6f6d 2053 6f75 7263 650a 2020 2020 2020  om Source.      
-00000cf0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00000d00: 2020 2020 2020 6769 7420 636c 6f6e 6520        git clone 
-00000d10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000d20: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d64  om/th2-net/th2-d
-00000d30: 6174 612d 7365 7276 6963 6573 0a20 2020  ata-services.   
-00000d40: 2020 2020 2020 2020 2070 6970 2069 6e73           pip ins
-00000d50: 7461 6c6c 2074 6832 2d64 6174 612d 7365  tall th2-data-se
-00000d60: 7276 6963 6573 2f0a 2020 2020 2020 2020  rvices/.        
-00000d70: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00000d80: 0a20 2020 2020 2020 2023 2323 2044 6174  .        ### Dat
-00000d90: 6120 736f 7572 6365 7320 2870 726f 7669  a sources (provi
-00000da0: 6465 7273 290a 2020 2020 2020 2020 0a20  ders).        . 
-00000db0: 2020 2020 2020 2053 696e 6365 2060 7631         Since `v1
-00000dc0: 2e33 2e30 602c 2074 6865 206c 6962 7261  .3.0`, the libra
-00000dd0: 7279 2064 6f65 736e 2774 2070 726f 7669  ry doesn't provi
-00000de0: 6465 2064 6174 6120 736f 7572 6365 2064  de data source d
-00000df0: 6570 656e 6465 6e63 6965 732e 0a20 2020  ependencies..   
-00000e00: 2020 2020 200a 2020 2020 2020 2020 596f       .        Yo
-00000e10: 7520 7368 6f75 6c64 2070 726f 7669 6465  u should provide
-00000e20: 2069 7420 6d61 6e75 616c 6c79 2064 7572   it manually dur
-00000e30: 696e 6720 696e 7374 616c 6c61 7469 6f6e  ing installation
-00000e40: 2e20 0a20 2020 2020 2020 2059 6f75 206a  . .        You j
-00000e50: 7573 7420 6e65 6564 2074 6f20 6164 6420  ust need to add 
-00000e60: 7371 7561 7265 2062 7261 636b 6574 7320  square brackets 
-00000e70: 6166 7465 7220 6c69 6272 6172 7920 6e61  after library na
-00000e80: 6d65 2061 6e64 2070 7574 2064 6570 656e  me and put depen
-00000e90: 6465 6e63 7920 6e61 6d65 2e0a 2020 2020  dency name..    
-00000ea0: 2020 2020 0a20 2020 2020 2020 2060 6060      .        ```
-00000eb0: 0a20 2020 2020 2020 2070 6970 2069 6e73  .        pip ins
-00000ec0: 7461 6c6c 2074 6832 2d64 6174 612d 7365  tall th2-data-se
-00000ed0: 7276 6963 6573 5b64 6570 656e 6465 6e63  rvices[dependenc
-00000ee0: 795f 6e61 6d65 5d0a 2020 2020 2020 2020  y_name].        
-00000ef0: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
-00000f00: 2020 2020 202a 2a44 6570 656e 6465 6e63       **Dependenc
-00000f10: 6965 7320 6c69 7374 2a2a 200a 2020 2020  ies list** .    
-00000f20: 2020 2020 0a20 2020 2020 2020 207c 2020      .        |  
-00000f30: 6465 7065 6e64 656e 6379 206e 616d 6520  dependency name 
-00000f40: 207c 2070 726f 7669 6465 7220 7665 7273   | provider vers
-00000f50: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
-00000f60: 2020 2020 2020 2020 207c 0a20 2020 2020           |.     
-00000f70: 2020 207c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d     |:-----------
-00000f80: 2d2d 2d2d 2d2d 3a7c 2d2d 2d2d 2d2d 2d2d  ------:|--------
-00000f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-00000fb0: 0a20 2020 2020 2020 207c 2020 2020 2020  .        |      
-00000fc0: 206c 7764 7020 2020 2020 2020 207c 206c   lwdp        | l
-00000fd0: 6174 6573 7420 7665 7273 696f 6e20 6f66  atest version of
-00000fe0: 206c 7764 7020 2020 2020 2020 2020 2020   lwdp           
-00000ff0: 2020 2020 207c 0a20 2020 2020 2020 207c       |.        |
-00001000: 2020 2020 2020 206c 7764 7032 2020 2020         lwdp2    
-00001010: 2020 207c 206c 6174 6573 7420 7665 7273     | latest vers
-00001020: 696f 6e20 6f66 206c 7764 7020 7632 2020  ion of lwdp v2  
-00001030: 2020 2020 2020 2020 2020 207c 0a20 2020             |.   
-00001040: 2020 2020 207c 2075 7469 6c73 2d72 7074       | utils-rpt
-00001050: 2d76 6965 7765 7220 207c 206c 6174 6573  -viewer  | lates
-00001060: 7420 7665 7273 696f 6e20 6f66 2075 7469  t version of uti
-00001070: 6c73 2d72 7074 2d76 6965 7765 7220 2020  ls-rpt-viewer   
-00001080: 207c 0a20 2020 2020 2020 207c 2075 7469   |.        | uti
-00001090: 6c73 2d72 7074 2d76 6965 7765 7235 207c  ls-rpt-viewer5 |
-000010a0: 206c 6174 6573 7420 7665 7273 696f 6e20   latest version 
-000010b0: 6f66 2075 7469 6c73 2d72 7074 2d76 6965  of utils-rpt-vie
-000010c0: 7765 7220 7635 207c 0a20 2020 2020 2020  wer v5 |.       
-000010d0: 207c 2020 2075 7469 6c73 2d61 6476 616e   |   utils-advan
-000010e0: 6365 6420 207c 206c 6174 6573 7420 7665  ced  | latest ve
-000010f0: 7273 696f 6e20 6f66 2064 732d 7574 696c  rsion of ds-util
-00001100: 7320 2020 2020 2020 2020 2020 207c 0a20  s            |. 
-00001110: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001120: 2a2a 4578 616d 706c 652a 2a0a 2020 2020  **Example**.    
-00001130: 2020 2020 0a20 2020 2020 2020 2060 6060      .        ```
-00001140: 0a20 2020 2020 2020 2070 6970 2069 6e73  .        pip ins
-00001150: 7461 6c6c 2074 6832 2d64 6174 612d 7365  tall th2-data-se
-00001160: 7276 6963 6573 5b6c 7764 7031 5d0a 2020  rvices[lwdp1].  
-00001170: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00001180: 2020 0a20 2020 2020 2020 2023 2320 322e    .        ## 2.
-00001190: 322e 2045 7861 6d70 6c65 0a20 2020 2020  2. Example.     
-000011a0: 2020 200a 2020 2020 2020 2020 4120 676f     .        A go
-000011b0: 6f64 2c20 7368 6f72 7420 6578 616d 706c  od, short exampl
-000011c0: 6520 6973 2077 6f72 7468 2061 2074 686f  e is worth a tho
-000011d0: 7573 616e 6420 776f 7264 732e 0a20 2020  usand words..   
-000011e0: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
-000011f0: 6973 2065 7861 6d70 6c65 2073 686f 7773  is example shows
-00001200: 2062 6173 6963 2075 7361 6765 206f 6620   basic usage of 
-00001210: 6c69 6272 6172 7927 7320 6665 6174 7572  library's featur
-00001220: 6573 2e0a 2020 2020 2020 2020 0a20 2020  es..        .   
-00001230: 2020 2020 205b 5468 6520 666f 6c6c 6f77       [The follow
-00001240: 696e 6720 6578 616d 706c 6520 6173 2061  ing example as a
-00001250: 2066 696c 655d 2865 7861 6d70 6c65 732f   file](examples/
-00001260: 6765 745f 7374 6172 7465 645f 6578 616d  get_started_exam
-00001270: 706c 652e 7079 292e 0a20 2020 2020 2020  ple.py)..       
-00001280: 200a 2020 2020 2020 2020 3c21 2d2d 2073   .        <!-- s
-00001290: 7461 7274 2067 6574 5f73 7461 7274 6564  tart get_started
-000012a0: 5f65 7861 6d70 6c65 2e70 7920 2d2d 3e0a  _example.py -->.
-000012b0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-000012c0: 6e0a 2020 2020 2020 2020 6672 6f6d 2074  n.        from t
-000012d0: 7970 696e 6720 696d 706f 7274 2054 7570  yping import Tup
-000012e0: 6c65 2c20 4c69 7374 2c20 4f70 7469 6f6e  le, List, Option
-000012f0: 616c 2c20 4765 6e65 7261 746f 720a 2020  al, Generator.  
-00001300: 2020 2020 2020 6672 6f6d 2064 6174 6574        from datet
-00001310: 696d 6520 696d 706f 7274 2064 6174 6574  ime import datet
-00001320: 696d 650a 2020 2020 2020 2020 0a20 2020  ime.        .   
-00001330: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
-00001340: 7461 5f73 6572 7669 6365 732e 6461 7461  ta_services.data
-00001350: 2069 6d70 6f72 7420 4461 7461 0a20 2020   import Data.   
-00001360: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
-00001370: 7461 5f73 6572 7669 6365 732e 6576 656e  ta_services.even
-00001380: 745f 7472 6565 2069 6d70 6f72 7420 4576  t_tree import Ev
-00001390: 656e 7454 7265 652c 2045 7665 6e74 5472  entTree, EventTr
-000013a0: 6565 436f 6c6c 6563 7469 6f6e 2c20 5061  eeCollection, Pa
-000013b0: 7265 6e74 4576 656e 7454 7265 6543 6f6c  rentEventTreeCol
-000013c0: 6c65 6374 696f 6e2c 2049 4554 4344 7269  lection, IETCDri
-000013d0: 7665 720a 2020 2020 2020 2020 6672 6f6d  ver.        from
-000013e0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
-000013f0: 6573 2e69 6e74 6572 6661 6365 7320 696d  es.interfaces im
-00001400: 706f 7274 2049 4461 7461 536f 7572 6365  port IDataSource
-00001410: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
-00001420: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00001430: 7574 696c 732e 636f 6e76 6572 7465 7273  utils.converters
-00001440: 2069 6d70 6f72 7420 4461 7465 7469 6d65   import Datetime
-00001450: 436f 6e76 6572 7465 722c 2044 6174 6574  Converter, Datet
-00001460: 696d 6553 7472 696e 6743 6f6e 7665 7274  imeStringConvert
-00001470: 6572 2c20 5072 6f74 6f62 7566 5469 6d65  er, ProtobufTime
-00001480: 7374 616d 7043 6f6e 7665 7274 6572 0a20  stampConverter. 
-00001490: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000014a0: 2320 5b30 5d20 4c69 6220 636f 6e66 6967  # [0] Lib config
-000014b0: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
-000014c0: 2320 5b30 2e31 5d20 496e 7465 7261 6374  # [0.1] Interact
-000014d0: 6976 6520 6f72 2053 6372 6970 7420 6d6f  ive or Script mo
-000014e0: 6465 0a20 2020 2020 2020 2023 2049 6620  de.        # If 
-000014f0: 796f 7520 7573 6520 7468 6520 6c69 6220  you use the lib 
-00001500: 696e 2069 6e74 6572 6163 7469 7665 206d  in interactive m
-00001510: 6f64 6520 286a 7570 7974 6572 2c20 6970  ode (jupyter, ip
-00001520: 7974 686f 6e29 2069 7427 7320 7265 636f  ython) it's reco
-00001530: 6d6d 656e 6465 6420 746f 2073 6574 2074  mmended to set t
-00001540: 6865 2073 7065 6369 616c 0a20 2020 2020  he special.     
-00001550: 2020 2023 2067 6c6f 6261 6c20 7061 7261     # global para
-00001560: 6d65 7465 7220 746f 2054 7275 652e 2049  meter to True. I
-00001570: 7427 6c6c 206b 6565 7020 6361 6368 6520  t'll keep cache 
-00001580: 6669 6c65 7320 6966 2073 6f6d 6574 6869  files if somethi
-00001590: 6e67 2077 656e 7420 7772 6f6e 672e 0a20  ng went wrong.. 
-000015a0: 2020 2020 2020 2066 726f 6d20 7468 325f         from th2_
-000015b0: 6461 7461 5f73 6572 7669 6365 732e 636f  data_services.co
-000015c0: 6e66 6967 2069 6d70 6f72 7420 6f70 7469  nfig import opti
-000015d0: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
-000015e0: 2020 2020 206f 7074 696f 6e73 2e49 4e54       options.INT
-000015f0: 4552 4143 5449 5645 5f4d 4f44 4520 3d20  ERACTIVE_MODE = 
-00001600: 5472 7565 0a20 2020 2020 2020 200a 2020  True.        .  
-00001610: 2020 2020 2020 2320 536f 6d65 2065 7861        # Some exa
-00001620: 6d70 6c65 2064 6174 610a 2020 2020 2020  mple data.      
-00001630: 2020 6576 656e 7473 203d 2044 6174 6128    events = Data(
-00001640: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
-00001650: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00001660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001670: 2020 2020 2022 6576 656e 7449 6422 3a20       "eventId": 
-00001680: 2264 656d 6f5f 626f 6f6b 5f31 3a74 6832  "demo_book_1:th2
-00001690: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
-000016a0: 3335 3730 3535 3630 3837 3330 3030 3a64  35705560873000:d
-000016b0: 3631 6539 3330 612d 3864 3030 2d31 3165  61e930a-8d00-11e
-000016c0: 642d 6161 3161 2d64 3334 6136 3135 3531  d-aa1a-d34a61551
-000016d0: 3532 645f 3122 2c0a 2020 2020 2020 2020  52d_1",.        
-000016e0: 2020 2020 2020 2020 2020 2020 2262 6174              "bat
-000016f0: 6368 4964 223a 204e 6f6e 652c 0a20 2020  chId": None,.   
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2022 6973 4261 7463 6865 6422 3a20 4661   "isBatched": Fa
-00001720: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-00001730: 2020 2020 2020 2020 2022 6576 656e 744e           "eventN
-00001740: 616d 6522 3a20 2253 6574 206f 6620 6175  ame": "Set of au
-00001750: 746f 2d67 656e 6572 6174 6564 2065 7665  to-generated eve
-00001760: 6e74 7320 666f 7220 6473 206c 6962 2074  nts for ds lib t
-00001770: 6573 7469 6e67 222c 0a20 2020 2020 2020  esting",.       
-00001780: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
-00001790: 656e 7454 7970 6522 3a20 2264 732d 6c69  entType": "ds-li
-000017a0: 622d 7465 7374 2d65 7665 6e74 222c 0a20  b-test-event",. 
-000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017c0: 2020 2022 656e 6454 696d 6573 7461 6d70     "endTimestamp
-000017d0: 223a 207b 2265 706f 6368 5365 636f 6e64  ": {"epochSecond
-000017e0: 223a 2031 3637 3239 3237 3032 352c 2022  ": 1672927025, "
-000017f0: 6e61 6e6f 223a 2035 3631 3735 3130 3030  nano": 561751000
-00001800: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00001810: 2020 2020 2020 2022 7374 6172 7454 696d         "startTim
-00001820: 6573 7461 6d70 223a 207b 2265 706f 6368  estamp": {"epoch
-00001830: 5365 636f 6e64 223a 2031 3637 3239 3237  Second": 1672927
-00001840: 3032 352c 2022 6e61 6e6f 223a 2035 3630  025, "nano": 560
-00001850: 3837 3330 3030 7d2c 0a20 2020 2020 2020  873000},.       
-00001860: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
-00001870: 7265 6e74 4576 656e 7449 6422 3a20 4e6f  rentEventId": No
-00001880: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00001890: 2020 2020 2020 2020 2273 7563 6365 7373          "success
-000018a0: 6675 6c22 3a20 5472 7565 2c0a 2020 2020  ful": True,.    
-000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018c0: 2262 6f6f 6b49 6422 3a20 2264 656d 6f5f  "bookId": "demo_
-000018d0: 626f 6f6b 5f31 222c 0a20 2020 2020 2020  book_1",.       
-000018e0: 2020 2020 2020 2020 2020 2020 2022 7363               "sc
-000018f0: 6f70 6522 3a20 2274 6832 2d73 636f 7065  ope": "th2-scope
-00001900: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001910: 2020 2020 2020 2022 6174 7461 6368 6564         "attached
-00001920: 4d65 7373 6167 6549 6473 223a 205b 5d2c  MessageIds": [],
-00001930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001940: 2020 2020 2022 626f 6479 223a 205b 5d2c       "body": [],
-00001950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001960: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00001970: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00001980: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00001990: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
-000019a0: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
-000019b0: 3031 3035 3133 3537 3035 3536 3335 3232  0105135705563522
-000019c0: 3030 303a 3961 6462 6233 6530 2d35 6638  000:9adbb3e0-5f8
-000019d0: 622d 3463 3238 2d61 3261 632d 3733 3631  b-4c28-a2ac-7361
-000019e0: 6538 6661 3730 3463 3e64 656d 6f5f 626f  e8fa704c>demo_bo
-000019f0: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
-00001a00: 3032 3330 3130 3531 3335 3730 3535 3633  0230105135705563
-00001a10: 3532 3230 3030 3a64 3631 6539 3330 612d  522000:d61e930a-
-00001a20: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
-00001a30: 3334 6136 3135 3531 3532 645f 3222 2c0a  34a6155152d_2",.
-00001a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a50: 2020 2020 2262 6174 6368 4964 223a 2022      "batchId": "
-00001a60: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
-00001a70: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
-00001a80: 3537 3035 3536 3335 3232 3030 303a 3961  5705563522000:9a
-00001a90: 6462 6233 6530 2d35 6638 622d 3463 3238  dbb3e0-5f8b-4c28
-00001aa0: 2d61 3261 632d 3733 3631 6538 6661 3730  -a2ac-7361e8fa70
-00001ab0: 3463 222c 0a20 2020 2020 2020 2020 2020  4c",.           
-00001ac0: 2020 2020 2020 2020 2022 6973 4261 7463           "isBatc
-00001ad0: 6865 6422 3a20 5472 7565 2c0a 2020 2020  hed": True,.    
-00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001af0: 2265 7665 6e74 4e61 6d65 223a 2022 506c  "eventName": "Pl
-00001b00: 6169 6e20 6576 656e 7420 3122 2c0a 2020  ain event 1",.  
-00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b20: 2020 2265 7665 6e74 5479 7065 223a 2022    "eventType": "
-00001b30: 6473 2d6c 6962 2d74 6573 742d 6576 656e  ds-lib-test-even
-00001b40: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00001b50: 2020 2020 2020 2020 2265 6e64 5469 6d65          "endTime
-00001b60: 7374 616d 7022 3a20 7b22 6570 6f63 6853  stamp": {"epochS
-00001b70: 6563 6f6e 6422 3a20 3136 3732 3932 3730  econd": 16729270
-00001b80: 3235 2c20 226e 616e 6f22 3a20 3536 3336  25, "nano": 5636
-00001b90: 3430 3030 307d 2c0a 2020 2020 2020 2020  40000},.        
-00001ba0: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-00001bb0: 7274 5469 6d65 7374 616d 7022 3a20 7b22  rtTimestamp": {"
-00001bc0: 6570 6f63 6853 6563 6f6e 6422 3a20 3136  epochSecond": 16
-00001bd0: 3732 3932 3730 3235 2c20 226e 616e 6f22  72927025, "nano"
-00001be0: 3a20 3536 3335 3232 3030 307d 2c0a 2020  : 563522000},.  
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c00: 2020 2270 6172 656e 7445 7665 6e74 4964    "parentEventId
-00001c10: 223a 2022 6465 6d6f 5f62 6f6f 6b5f 313a  ": "demo_book_1:
-00001c20: 7468 322d 7363 6f70 653a 3230 3233 3031  th2-scope:202301
-00001c30: 3035 3133 3537 3035 3536 3038 3733 3030  0513570556087300
-00001c40: 303a 6436 3165 3933 3061 2d38 6430 302d  0:d61e930a-8d00-
-00001c50: 3131 6564 2d61 6131 612d 6433 3461 3631  11ed-aa1a-d34a61
-00001c60: 3535 3135 3264 5f31 222c 0a20 2020 2020  55152d_1",.     
-00001c70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001c80: 7375 6363 6573 7366 756c 223a 2054 7275  successful": Tru
-00001c90: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001ca0: 2020 2020 2020 2022 626f 6f6b 4964 223a         "bookId":
-00001cb0: 2022 6465 6d6f 5f62 6f6f 6b5f 3122 2c0a   "demo_book_1",.
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cd0: 2020 2020 2273 636f 7065 223a 2022 7468      "scope": "th
-00001ce0: 322d 7363 6f70 6522 2c0a 2020 2020 2020  2-scope",.      
-00001cf0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00001d00: 7474 6163 6865 644d 6573 7361 6765 4964  ttachedMessageId
-00001d10: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
-00001d20: 2020 2020 2020 2020 2020 2020 2262 6f64              "bod
-00001d30: 7922 3a20 7b22 7479 7065 223a 2022 6d65  y": {"type": "me
-00001d40: 7373 6167 6522 2c20 2264 6174 6122 3a20  ssage", "data": 
-00001d50: 2264 732d 6c69 6220 7465 7374 2062 6f64  "ds-lib test bod
-00001d60: 7922 7d2c 0a20 2020 2020 2020 2020 2020  y"},.           
-00001d70: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00001d80: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00001da0: 7665 6e74 4964 223a 2022 6465 6d6f 5f62  ventId": "demo_b
-00001db0: 6f6f 6b5f 313a 7468 322d 7363 6f70 653a  ook_1:th2-scope:
-00001dc0: 3230 3233 3031 3035 3133 3537 3035 3536  2023010513570556
-00001dd0: 3335 3232 3030 303a 3961 6462 6233 6530  3522000:9adbb3e0
-00001de0: 2d35 6638 622d 3463 3238 2d61 3261 632d  -5f8b-4c28-a2ac-
-00001df0: 3733 3631 6538 6661 3730 3463 3e64 656d  7361e8fa704c>dem
-00001e00: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
-00001e10: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
-00001e20: 3535 3633 3735 3730 3030 3a64 3631 6539  5563757000:d61e9
-00001e30: 3330 612d 3864 3030 2d31 3165 642d 6161  30a-8d00-11ed-aa
-00001e40: 3161 2d64 3334 6136 3135 3531 3532 645f  1a-d34a6155152d_
-00001e50: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
-00001e60: 2020 2020 2020 2020 2262 6174 6368 4964          "batchId
-00001e70: 223a 2022 6465 6d6f 5f62 6f6f 6b5f 313a  ": "demo_book_1:
-00001e80: 7468 322d 7363 6f70 653a 3230 3233 3031  th2-scope:202301
-00001e90: 3035 3133 3537 3035 3536 3335 3232 3030  0513570556352200
-00001ea0: 303a 3961 6462 6233 6530 2d35 6638 622d  0:9adbb3e0-5f8b-
-00001eb0: 3463 3238 2d61 3261 632d 3733 3631 6538  4c28-a2ac-7361e8
-00001ec0: 6661 3730 3463 222c 0a20 2020 2020 2020  fa704c",.       
-00001ed0: 2020 2020 2020 2020 2020 2020 2022 6973               "is
-00001ee0: 4261 7463 6865 6422 3a20 5472 7565 2c0a  Batched": True,.
-00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f00: 2020 2020 2265 7665 6e74 4e61 6d65 223a      "eventName":
-00001f10: 2022 506c 6169 6e20 6576 656e 7420 3222   "Plain event 2"
-00001f20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001f30: 2020 2020 2020 2265 7665 6e74 5479 7065        "eventType
-00001f40: 223a 2022 6473 2d6c 6962 2d74 6573 742d  ": "ds-lib-test-
-00001f50: 6576 656e 7422 2c0a 2020 2020 2020 2020  event",.        
-00001f60: 2020 2020 2020 2020 2020 2020 2265 6e64              "end
-00001f70: 5469 6d65 7374 616d 7022 3a20 7b22 6570  Timestamp": {"ep
-00001f80: 6f63 6853 6563 6f6e 6422 3a20 3136 3732  ochSecond": 1672
-00001f90: 3932 3730 3235 2c20 226e 616e 6f22 3a20  927025, "nano": 
-00001fa0: 3536 3337 3931 3030 307d 2c0a 2020 2020  563791000},.    
-00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fc0: 2273 7461 7274 5469 6d65 7374 616d 7022  "startTimestamp"
-00001fd0: 3a20 7b22 6570 6f63 6853 6563 6f6e 6422  : {"epochSecond"
-00001fe0: 3a20 3136 3732 3932 3730 3235 2c20 226e  : 1672927025, "n
-00001ff0: 616e 6f22 3a20 3536 3337 3537 3030 307d  ano": 563757000}
-00002000: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002010: 2020 2020 2020 2270 6172 656e 7445 7665        "parentEve
-00002020: 6e74 4964 223a 2022 6465 6d6f 5f62 6f6f  ntId": "demo_boo
-00002030: 6b5f 313a 7468 322d 7363 6f70 653a 3230  k_1:th2-scope:20
-00002040: 3233 3031 3035 3133 3537 3035 3536 3038  2301051357055608
-00002050: 3733 3030 303a 6436 3165 3933 3061 2d38  73000:d61e930a-8
-00002060: 6430 302d 3131 6564 2d61 6131 612d 6433  d00-11ed-aa1a-d3
-00002070: 3461 3631 3535 3135 3264 5f31 222c 0a20  4a6155152d_1",. 
-00002080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002090: 2020 2022 7375 6363 6573 7366 756c 223a     "successful":
-000020a0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-000020b0: 2020 2020 2020 2020 2020 2022 626f 6f6b             "book
-000020c0: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
-000020d0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-000020e0: 2020 2020 2020 2020 2273 636f 7065 223a          "scope":
-000020f0: 2022 7468 322d 7363 6f70 6522 2c0a 2020   "th2-scope",.  
-00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002110: 2020 2261 7474 6163 6865 644d 6573 7361    "attachedMessa
-00002120: 6765 4964 7322 3a20 5b5d 2c0a 2020 2020  geIds": [],.    
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2262 6f64 7922 3a20 7b22 7479 7065 223a  "body": {"type":
-00002150: 2022 6d65 7373 6167 6522 2c20 2264 6174   "message", "dat
-00002160: 6122 3a20 2264 732d 6c69 6220 7465 7374  a": "ds-lib test
-00002170: 2062 6f64 7922 7d2c 0a20 2020 2020 2020   body"},.       
-00002180: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00002190: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-000021a0: 2020 290a 2020 2020 2020 2020 0a20 2020    ).        .   
-000021b0: 2020 2020 2023 205b 315d 2057 6f72 6b69       # [1] Worki
-000021c0: 6e67 2077 6974 6820 6120 4461 7461 206f  ng with a Data o
-000021d0: 626a 6563 742e 0a20 2020 2020 2020 2023  bject..        #
-000021e0: 205b 312e 315d 2046 696c 7465 722e 0a20   [1.1] Filter.. 
-000021f0: 2020 2020 2020 2066 696c 7465 7265 645f         filtered_
-00002200: 6576 656e 7473 3a20 4461 7461 203d 2065  events: Data = e
-00002210: 7665 6e74 732e 6669 6c74 6572 286c 616d  vents.filter(lam
-00002220: 6264 6120 653a 2065 5b22 626f 6479 225d  bda e: e["body"]
-00002230: 2021 3d20 5b5d 2920 2023 2046 696c 7465   != [])  # Filte
-00002240: 7220 6576 656e 7473 2077 6974 6820 656d  r events with em
-00002250: 7074 7920 626f 6479 2e0a 2020 2020 2020  pty body..      
-00002260: 2020 0a20 2020 2020 2020 200a 2020 2020    .        .    
-00002270: 2020 2020 2320 5b31 2e32 5d20 4d61 702e      # [1.2] Map.
-00002280: 0a20 2020 2020 2020 2064 6566 2074 7261  .        def tra
-00002290: 6e73 666f 726d 5f66 756e 6374 696f 6e28  nsform_function(
-000022a0: 7265 636f 7264 293a 0a20 2020 2020 2020  record):.       
-000022b0: 2020 2020 2072 6574 7572 6e20 7b22 6576       return {"ev
-000022c0: 656e 744e 616d 6522 3a20 7265 636f 7264  entName": record
-000022d0: 5b22 6576 656e 744e 616d 6522 5d2c 2022  ["eventName"], "
-000022e0: 7375 6363 6573 7366 756c 223a 2072 6563  successful": rec
-000022f0: 6f72 645b 2273 7563 6365 7373 6675 6c22  ord["successful"
-00002300: 5d7d 0a20 2020 2020 2020 200a 2020 2020  ]}.        .    
-00002310: 2020 2020 0a20 2020 2020 2020 2066 696c      .        fil
-00002320: 7465 7265 645f 616e 645f 6d61 7070 6564  tered_and_mapped
-00002330: 5f65 7665 6e74 7320 3d20 6669 6c74 6572  _events = filter
-00002340: 6564 5f65 7665 6e74 732e 6d61 7028 7472  ed_events.map(tr
-00002350: 616e 7366 6f72 6d5f 6675 6e63 7469 6f6e  ansform_function
-00002360: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00002370: 2020 2023 205b 312e 335d 2044 6174 6120     # [1.3] Data 
-00002380: 7069 7065 6c69 6e65 2e0a 2020 2020 2020  pipeline..      
-00002390: 2020 2320 2020 2020 2020 496e 7374 6561    #       Instea
-000023a0: 6420 6f66 2064 6f69 6e67 2064 6174 6120  d of doing data 
-000023b0: 7472 616e 7366 6f72 6d61 7469 6f6e 7320  transformations 
-000023c0: 7374 6570 2062 7920 7374 6570 2079 6f75  step by step you
-000023d0: 2063 616e 2064 6f20 6974 2069 6e20 6f6e   can do it in on
-000023e0: 6520 6c69 6e65 2e0a 2020 2020 2020 2020  e line..        
-000023f0: 6669 6c74 6572 6564 5f61 6e64 5f6d 6170  filtered_and_map
-00002400: 7065 645f 6576 656e 7473 5f62 795f 7069  ped_events_by_pi
-00002410: 7065 6c69 6e65 203d 2065 7665 6e74 732e  peline = events.
-00002420: 6669 6c74 6572 286c 616d 6264 6120 653a  filter(lambda e:
-00002430: 2065 5b22 626f 6479 225d 2021 3d20 5b5d   e["body"] != []
-00002440: 292e 6d61 7028 7472 616e 7366 6f72 6d5f  ).map(transform_
-00002450: 6675 6e63 7469 6f6e 290a 2020 2020 2020  function).      
-00002460: 2020 2320 436f 6e74 656e 7420 6f66 2074    # Content of t
-00002470: 6865 7365 2074 776f 2044 6174 6120 6f62  hese two Data ob
-00002480: 6a65 6374 7320 7368 6f75 6c64 2062 6520  jects should be 
-00002490: 6571 7561 6c2e 0a20 2020 2020 2020 2061  equal..        a
-000024a0: 7373 6572 7420 6c69 7374 2866 696c 7465  ssert list(filte
-000024b0: 7265 645f 616e 645f 6d61 7070 6564 5f65  red_and_mapped_e
-000024c0: 7665 6e74 7329 203d 3d20 6c69 7374 2866  vents) == list(f
-000024d0: 696c 7465 7265 645f 616e 645f 6d61 7070  iltered_and_mapp
-000024e0: 6564 5f65 7665 6e74 735f 6279 5f70 6970  ed_events_by_pip
-000024f0: 656c 696e 6529 0a20 2020 2020 2020 200a  eline).        .
-00002500: 2020 2020 2020 2020 2320 5b31 2e34 5d20          # [1.4] 
-00002510: 5369 6674 2e20 536b 6970 2074 6865 2066  Sift. Skip the f
-00002520: 6972 7374 2066 6577 2069 7465 6d73 206f  irst few items o
-00002530: 7220 6c69 6d69 7420 7468 656d 2e0a 2020  r limit them..  
-00002540: 2020 2020 2020 6461 7461 203d 2044 6174        data = Dat
-00002550: 6128 5b31 2c20 322c 2033 2c20 342c 2035  a([1, 2, 3, 4, 5
-00002560: 2c20 362c 2037 2c20 382c 2039 2c20 3130  , 6, 7, 8, 9, 10
-00002570: 2c20 3131 2c20 3132 2c20 3133 2c20 3134  , 11, 12, 13, 14
-00002580: 2c20 3135 5d29 0a20 2020 2020 2020 2069  , 15]).        i
-00002590: 7465 6d73 5f66 726f 6d5f 3131 5f74 6f5f  tems_from_11_to_
-000025a0: 656e 643a 2047 656e 6572 6174 6f72 203d  end: Generator =
-000025b0: 2064 6174 612e 7369 6674 2873 6b69 703d   data.sift(skip=
-000025c0: 3130 290a 2020 2020 2020 2020 6f6e 6c79  10).        only
-000025d0: 5f66 6972 7374 5f31 305f 6974 656d 733a  _first_10_items:
-000025e0: 2047 656e 6572 6174 6f72 203d 2064 6174   Generator = dat
-000025f0: 612e 7369 6674 286c 696d 6974 3d31 3029  a.sift(limit=10)
-00002600: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002610: 2020 2320 5b31 2e35 5d20 4368 616e 6769    # [1.5] Changi
-00002620: 6e67 2063 6163 6865 2073 7461 7475 732e  ng cache status.
-00002630: 0a20 2020 2020 2020 2065 7665 6e74 732e  .        events.
-00002640: 7573 655f 6361 6368 6528 5472 7565 290a  use_cache(True).
-00002650: 2020 2020 2020 2020 2320 6f72 206a 7573          # or jus
-00002660: 740a 2020 2020 2020 2020 6576 656e 7473  t.        events
-00002670: 2e75 7365 5f63 6163 6865 2829 2020 2320  .use_cache()  # 
-00002680: 4966 2079 6f75 2077 616e 7420 746f 2061  If you want to a
-00002690: 6374 6976 6174 6520 6361 6368 652e 0a20  ctivate cache.. 
-000026a0: 2020 2020 2020 2023 205b 312e 365d 2057         # [1.6] W
-000026b0: 616c 6b20 7468 726f 7567 6820 6461 7461  alk through data
-000026c0: 2e0a 2020 2020 2020 2020 666f 7220 6576  ..        for ev
-000026d0: 656e 7420 696e 2065 7665 6e74 733a 0a20  ent in events:. 
-000026e0: 2020 2020 2020 2020 2020 2023 2044 6f20             # Do 
-000026f0: 736f 6d65 7468 696e 6720 7769 7468 2065  something with e
-00002700: 7665 6e74 2028 6576 656e 7420 6973 2061  vent (event is a
-00002710: 2064 6963 7429 2e0a 2020 2020 2020 2020   dict)..        
-00002720: 2020 2020 7072 696e 7428 6576 656e 7429      print(event)
-00002730: 0a20 2020 2020 2020 2023 2041 6674 6572  .        # After
-00002740: 2066 6972 7374 2069 7465 7261 7469 6f6e   first iteration
-00002750: 2074 6865 2065 7665 6e74 7320 6861 7320   the events has 
-00002760: 6120 6361 6368 6520 6669 6c65 2e0a 2020  a cache file..  
-00002770: 2020 2020 2020 2320 4e6f 7720 7468 6579        # Now they
-00002780: 2077 696c 6c20 6265 2075 7365 6420 696e   will be used in
-00002790: 2074 6865 2063 6163 6865 2069 6e20 7468   the cache in th
-000027a0: 6520 6e65 7874 2069 7465 7261 7469 6f6e  e next iteration
-000027b0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000027c0: 2020 2023 205b 312e 375d 2047 6574 206e     # [1.7] Get n
-000027d0: 756d 6265 7220 6f66 2074 6865 2065 6c65  umber of the ele
-000027e0: 6d65 6e74 7320 696e 2074 6865 2044 6174  ments in the Dat
-000027f0: 6120 6f62 6a65 6374 2e0a 2020 2020 2020  a object..      
-00002800: 2020 6e75 6d62 6572 5f6f 665f 6576 656e    number_of_even
-00002810: 7473 203d 2065 7665 6e74 732e 6c65 6e0a  ts = events.len.
-00002820: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002830: 2023 205b 312e 385d 2043 6865 636b 2074   # [1.8] Check t
-00002840: 6861 7420 4461 7461 206f 626a 6563 7420  hat Data object 
-00002850: 6973 6e27 7420 656d 7074 792e 0a20 2020  isn't empty..   
-00002860: 2020 2020 2023 2054 6865 2064 6174 6120       # The data 
-00002870: 736f 7572 6365 2073 686f 756c 6420 6265  source should be
-00002880: 206e 6f74 2065 6d70 7479 2e0a 2020 2020   not empty..    
-00002890: 2020 2020 6173 7365 7274 2065 7665 6e74      assert event
-000028a0: 732e 6973 5f65 6d70 7479 2069 7320 4661  s.is_empty is Fa
-000028b0: 6c73 650a 2020 2020 2020 2020 0a20 2020  lse.        .   
-000028c0: 2020 2020 2023 205b 312e 395d 2043 6f6e       # [1.9] Con
-000028d0: 7665 7274 2044 6174 6120 6f62 6a65 6374  vert Data object
-000028e0: 2074 6f20 7468 6520 6c69 7374 206f 6620   to the list of 
-000028f0: 656c 656d 656e 7473 2865 7665 6e74 7320  elements(events 
-00002900: 6f72 206d 6573 7361 6765 7329 2e0a 2020  or messages)..  
-00002910: 2020 2020 2020 2320 4265 2063 6172 6566        # Be caref
-00002920: 756c 2c20 7468 6973 2063 616e 2074 616b  ul, this can tak
-00002930: 6520 746f 6f20 6d75 6368 206d 656d 6f72  e too much memor
-00002940: 792e 0a20 2020 2020 2020 2065 7665 6e74  y..        event
-00002950: 735f 6c69 7374 203d 206c 6973 7428 6576  s_list = list(ev
-00002960: 656e 7473 290a 2020 2020 2020 2020 0a20  ents).        . 
-00002970: 2020 2020 2020 2023 205b 312e 3130 5d20         # [1.10] 
-00002980: 5468 6520 6361 6368 6520 696e 6865 7269  The cache inheri
-00002990: 7461 6e63 652e 0a20 2020 2020 2020 2023  tance..        #
-000029a0: 2043 7265 6174 6573 2061 206e 6577 2044   Creates a new D
-000029b0: 6174 6120 6f62 6a65 6374 2074 6861 7420  ata object that 
-000029c0: 7769 6c6c 2075 7365 2063 6163 6865 2066  will use cache f
-000029d0: 726f 6d20 7468 6520 6576 656e 7473 2044  rom the events D
-000029e0: 6174 6120 6f62 6a65 6374 2e0a 2020 2020  ata object..    
-000029f0: 2020 2020 6576 656e 7473 5f66 696c 7465      events_filte
-00002a00: 7265 643a 2044 6174 6120 3d20 6576 656e  red: Data = even
-00002a10: 7473 2e66 696c 7465 7228 6c61 6d62 6461  ts.filter(lambda
-00002a20: 2072 6563 6f72 643a 2072 6563 6f72 642e   record: record.
-00002a30: 6765 7428 2262 6174 6368 4964 2229 290a  get("batchId")).
-00002a40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002a50: 2023 204e 6577 2044 6174 6120 6f62 6a65   # New Data obje
-00002a60: 6374 7320 646f 6e27 7420 7573 6520 7468  cts don't use th
-00002a70: 6569 7220 6f77 6e20 6361 6368 6520 6279  eir own cache by
-00002a80: 2064 6566 6175 6c74 2062 7574 2075 7365   default but use
-00002a90: 2074 6865 2063 6163 6865 206f 6620 7468   the cache of th
-00002aa0: 6520 7061 7265 6e74 2044 6174 6120 6f62  e parent Data ob
-00002ab0: 6a65 6374 2e0a 2020 2020 2020 2020 2320  ject..        # 
-00002ac0: 5573 6520 7573 655f 6361 6368 6520 6d65  Use use_cache me
-00002ad0: 7468 6f64 2074 6f20 6163 7469 7661 7465  thod to activate
-00002ae0: 2063 6163 6869 6e67 2e0a 2020 2020 2020   caching..      
-00002af0: 2020 2320 4166 7465 7220 7468 6174 2c20    # After that, 
-00002b00: 7468 6520 4461 7461 206f 626a 6563 7420  the Data object 
-00002b10: 7769 6c6c 2063 7265 6174 6520 6974 7320  will create its 
-00002b20: 6f77 6e20 6361 6368 6520 6669 6c65 2e0a  own cache file..
-00002b30: 2020 2020 2020 2020 6576 656e 7473 5f66          events_f
-00002b40: 696c 7465 7265 642e 7573 655f 6361 6368  iltered.use_cach
-00002b50: 6528 290a 2020 2020 2020 2020 0a20 2020  e().        .   
-00002b60: 2020 2020 206c 6973 7428 6576 656e 7473       list(events
-00002b70: 5f66 696c 7465 7265 6429 2020 2320 4a75  _filtered)  # Ju
-00002b80: 7374 2074 6f20 6974 6572 6174 6520 4461  st to iterate Da
-00002b90: 7461 206f 626a 6563 7420 2863 6163 6865  ta object (cache
-00002ba0: 2066 696c 6520 7769 6c6c 2062 6520 6372   file will be cr
-00002bb0: 6561 7465 6429 2e0a 2020 2020 2020 2020  eated)..        
-00002bc0: 0a20 2020 2020 2020 2066 696c 7465 7265  .        filtere
-00002bd0: 645f 6576 656e 7473 5f74 7970 6573 203d  d_events_types =
-00002be0: 2065 7665 6e74 735f 6669 6c74 6572 6564   events_filtered
-00002bf0: 2e6d 6170 286c 616d 6264 6120 7265 636f  .map(lambda reco
-00002c00: 7264 3a20 7b22 6576 656e 7454 7970 6522  rd: {"eventType"
-00002c10: 3a20 7265 636f 7264 2e67 6574 2822 6576  : record.get("ev
-00002c20: 656e 7454 7970 6522 297d 290a 2020 2020  entType")}).    
-00002c30: 2020 2020 0a20 2020 2020 2020 2065 7665      .        eve
-00002c40: 6e74 735f 7769 7468 6f75 745f 7479 7065  nts_without_type
-00002c50: 735f 7769 7468 5f62 6174 6368 203d 2066  s_with_batch = f
-00002c60: 696c 7465 7265 645f 6576 656e 7473 5f74  iltered_events_t
-00002c70: 7970 6573 2e66 696c 7465 7228 6c61 6d62  ypes.filter(lamb
-00002c80: 6461 2072 6563 6f72 643a 206e 6f74 2072  da record: not r
-00002c90: 6563 6f72 642e 6765 7428 2265 7665 6e74  ecord.get("event
-00002ca0: 5479 7065 2229 290a 2020 2020 2020 2020  Type")).        
-00002cb0: 6576 656e 7473 5f77 6974 686f 7574 5f74  events_without_t
-00002cc0: 7970 6573 5f77 6974 685f 6261 7463 682e  ypes_with_batch.
-00002cd0: 7573 655f 6361 6368 6528 290a 2020 2020  use_cache().    
-00002ce0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-00002cf0: 312e 3131 5d20 4461 7461 206f 626a 6563  1.11] Data objec
-00002d00: 7473 206a 6f69 6e69 6e67 2e0a 2020 2020  ts joining..    
-00002d10: 2020 2020 2320 596f 7520 6861 7665 2074      # You have t
-00002d20: 6865 2066 6f6c 6c6f 7769 6e67 2033 2044  he following 3 D
-00002d30: 6174 6120 6f62 6a65 6374 732e 0a20 2020  ata objects..   
-00002d40: 2020 2020 2064 3120 3d20 4461 7461 285b       d1 = Data([
-00002d50: 312c 2032 2c20 335d 290a 2020 2020 2020  1, 2, 3]).      
-00002d60: 2020 6432 203d 2044 6174 6128 5b22 6122    d2 = Data(["a"
-00002d70: 2c20 7b22 6964 223a 2031 3233 7d2c 2022  , {"id": 123}, "
-00002d80: 6322 5d29 0a20 2020 2020 2020 2064 3320  c"]).        d3 
-00002d90: 3d20 4461 7461 285b 372c 2038 2c20 395d  = Data([7, 8, 9]
-00002da0: 290a 2020 2020 2020 2020 2320 596f 7520  ).        # You 
-00002db0: 6361 6e20 6a6f 696e 2044 6174 6120 6f62  can join Data ob
-00002dc0: 6a65 6374 7320 696e 2066 6f6c 6c6f 7769  jects in followi
-00002dd0: 6e67 2077 6179 732e 0a20 2020 2020 2020  ng ways..       
-00002de0: 2023 2050 6c65 6173 6520 6e6f 7465 2c20   # Please note, 
-00002df0: 6e65 7720 4461 7461 206f 626a 6563 7420  new Data object 
-00002e00: 7769 6c6c 2068 6176 6520 6361 6368 6520  will have cache 
-00002e10: 7374 6174 7573 203d 3d20 4661 6c73 652e  status == False.
-00002e20: 0a20 2020 2020 2020 2064 6174 615f 7669  .        data_vi
-00002e30: 615f 696e 6974 203d 2044 6174 6128 5b64  a_init = Data([d
-00002e40: 312c 2064 322c 2064 335d 290a 2020 2020  1, d2, d3]).    
-00002e50: 2020 2020 6461 7461 5f76 6961 5f61 6464      data_via_add
-00002e60: 203d 2064 3120 2b20 6432 202b 2064 330a   = d1 + d2 + d3.
-00002e70: 2020 2020 2020 2020 6461 7461 5f77 6974          data_wit
-00002e80: 685f 6e6f 6e5f 6461 7461 5f6f 626a 5f76  h_non_data_obj_v
-00002e90: 6961 5f69 6e69 7420 3d20 4461 7461 285b  ia_init = Data([
-00002ea0: 6431 2c20 5b22 6122 2c20 7b22 6964 223a  d1, ["a", {"id":
-00002eb0: 2031 3233 7d2c 2022 6322 5d2c 2064 335d   123}, "c"], d3]
-00002ec0: 290a 2020 2020 2020 2020 6461 7461 5f77  ).        data_w
-00002ed0: 6974 685f 6e6f 6e5f 6461 7461 5f6f 626a  ith_non_data_obj
-00002ee0: 5f76 6961 5f61 6464 203d 2064 3120 2b20  _via_add = d1 + 
-00002ef0: 5b22 6122 2c20 7b22 6964 223a 2031 3233  ["a", {"id": 123
-00002f00: 7d2c 2022 6322 5d20 2b20 6433 0a20 2020  }, "c"] + d3.   
-00002f10: 2020 2020 2023 2059 6f75 2063 616e 206a       # You can j
-00002f20: 6f69 6e20 6375 7272 656e 7420 4461 7461  oin current Data
-00002f30: 206f 626a 6563 7420 6f6e 2070 6c61 6365   object on place
-00002f40: 2075 7369 6e67 202b 3d2e 0a20 2020 2020   using +=..     
-00002f50: 2020 2023 2049 7420 7769 6c6c 206b 6565     # It will kee
-00002f60: 7020 6361 6368 6520 7374 6174 7573 2e0a  p cache status..
-00002f70: 2020 2020 2020 2020 6431 202b 3d20 6433          d1 += d3
-00002f80: 2020 2320 6431 2077 696c 6c20 6265 636f    # d1 will beco
-00002f90: 6d65 2044 6174 6128 5b31 2c32 2c33 2c37  me Data([1,2,3,7
-00002fa0: 2c38 2c39 5d29 0a20 2020 2020 2020 200a  ,8,9]).        .
-00002fb0: 2020 2020 2020 2020 2320 5b31 2e31 325d          # [1.12]
-00002fc0: 2042 7569 6c64 2061 6e64 2072 6561 6420   Build and read 
-00002fd0: 4461 7461 206f 626a 6563 7420 6361 6368  Data object cach
-00002fe0: 6520 6669 6c65 732e 0a20 2020 2020 2020  e files..       
-00002ff0: 2065 7665 6e74 732e 6275 696c 645f 6361   events.build_ca
-00003000: 6368 6528 2263 6163 6865 5f66 696c 656e  che("cache_filen
-00003010: 616d 655f 6f72 5f70 6174 6822 290a 2020  ame_or_path").  
-00003020: 2020 2020 2020 6461 7461 5f6f 626a 5f66        data_obj_f
-00003030: 726f 6d5f 6361 6368 6520 3d20 4461 7461  rom_cache = Data
-00003040: 2e66 726f 6d5f 6361 6368 655f 6669 6c65  .from_cache_file
-00003050: 2822 6361 6368 655f 6669 6c65 6e61 6d65  ("cache_filename
-00003060: 5f6f 725f 7061 7468 2229 0a20 2020 2020  _or_path").     
-00003070: 2020 200a 2020 2020 2020 2020 2320 5b32     .        # [2
-00003080: 5d20 576f 726b 696e 6720 7769 7468 2063  ] Working with c
-00003090: 6f6e 7665 7274 6572 732e 0a20 2020 2020  onverters..     
-000030a0: 2020 2023 2054 6865 7265 2061 7265 2063     # There are c
-000030b0: 7572 7265 6e74 6c79 2074 6872 6565 2069  urrently three i
-000030c0: 6d70 6c65 6d65 6e74 6174 696f 6e73 206f  mplementations o
-000030d0: 6620 4954 696d 6573 7461 6d70 436f 6e76  f ITimestampConv
-000030e0: 6572 7465 7220 636c 6173 733a 2044 6174  erter class: Dat
-000030f0: 6574 696d 6543 6f6e 7665 7274 652c 2044  etimeConverte, D
-00003100: 6174 6574 696d 6553 7472 696e 6743 6f6e  atetimeStringCon
-00003110: 7665 7274 6572 2061 6e64 2050 726f 746f  verter and Proto
-00003120: 6275 6654 696d 6573 7461 6d70 436f 6e76  bufTimestampConv
-00003130: 6572 7465 722e 0a20 2020 2020 2020 2023  erter..        #
-00003140: 2054 6865 7920 616c 6c20 696d 706c 656d   They all implem
-00003150: 656e 7420 7361 6d65 206d 6574 686f 6473  ent same methods
-00003160: 2066 726f 6d20 6261 7365 2063 6c61 7373   from base class
-00003170: 2e0a 2020 2020 2020 2020 2320 4e6f 7465  ..        # Note
-00003180: 2074 6861 7420 736f 6d65 2061 6363 7572   that some accur
-00003190: 6163 7920 6d61 7920 6265 206c 6f73 7420  acy may be lost 
-000031a0: 6475 7269 6e67 2063 6f6e 7665 7273 696f  during conversio
-000031b0: 6e2e 0a20 2020 2020 2020 2023 2049 6620  n..        # If 
-000031c0: 666f 7220 6578 616d 706c 6520 796f 7520  for example you 
-000031d0: 7573 6520 746f 5f6d 6963 726f 7365 636f  use to_microseco
-000031e0: 6e64 7320 6e61 6e6f 7365 636f 6e64 7320  nds nanoseconds 
-000031f0: 7769 6c6c 2062 6520 6375 7420 6f66 6620  will be cut off 
-00003200: 696e 7374 6561 6420 6f66 2072 6f75 6e64  instead of round
-00003210: 696e 672e 0a20 2020 2020 2020 200a 2020  ing..        .  
-00003220: 2020 2020 2020 2320 5b32 2e31 5d20 4461        # [2.1] Da
-00003230: 7465 7469 6d65 436f 6e76 6572 7465 722e  tetimeConverter.
-00003240: 0a20 2020 2020 2020 2023 2044 6174 6574  .        # Datet
-00003250: 696d 6543 6f6e 7665 7274 6572 2074 616b  imeConverter tak
-00003260: 6573 2064 6174 6574 696d 652e 6461 7465  es datetime.date
-00003270: 7469 6d65 206f 626a 6563 7420 6173 2069  time object as i
-00003280: 6e70 7574 2e0a 2020 2020 2020 2020 0a20  nput..        . 
-00003290: 2020 2020 2020 2064 6174 6574 696d 655f         datetime_
-000032a0: 6f62 6a20 3d20 6461 7465 7469 6d65 2879  obj = datetime(y
-000032b0: 6561 723d 3230 3233 2c20 6d6f 6e74 683d  ear=2023, month=
-000032c0: 312c 2064 6179 3d35 2c20 686f 7572 3d31  1, day=5, hour=1
-000032d0: 342c 206d 696e 7574 653d 3338 2c20 7365  4, minute=38, se
-000032e0: 636f 6e64 3d32 352c 206d 6963 726f 7365  cond=25, microse
-000032f0: 636f 6e64 3d31 3436 3029 0a20 2020 2020  cond=1460).     
-00003300: 2020 200a 2020 2020 2020 2020 2320 4974     .        # It
-00003310: 2068 6173 206d 6574 686f 6473 2074 6861   has methods tha
-00003320: 7420 7265 7475 726e 2074 6865 2064 6174  t return the dat
-00003330: 6574 696d 6520 696e 2064 6966 6665 7265  etime in differe
-00003340: 6e74 2066 6f72 6d61 733a 0a20 2020 2020  nt formas:.     
-00003350: 2020 200a 2020 2020 2020 2020 6461 7465     .        date
-00003360: 5f6d 7320 3d20 4461 7465 7469 6d65 436f  _ms = DatetimeCo
-00003370: 6e76 6572 7465 722e 746f 5f6d 696c 6c69  nverter.to_milli
-00003380: 7365 636f 6e64 7328 6461 7465 7469 6d65  seconds(datetime
-00003390: 5f6f 626a 290a 2020 2020 2020 2020 6461  _obj).        da
-000033a0: 7465 5f75 7320 3d20 4461 7465 7469 6d65  te_us = Datetime
-000033b0: 436f 6e76 6572 7465 722e 746f 5f6d 6963  Converter.to_mic
-000033c0: 726f 7365 636f 6e64 7328 6461 7465 7469  roseconds(dateti
-000033d0: 6d65 5f6f 626a 290a 2020 2020 2020 2020  me_obj).        
-000033e0: 2320 436f 6e76 6572 7469 6e67 2074 6f20  # Converting to 
-000033f0: 6e61 6e6f 7365 636f 6e64 7320 6a75 7374  nanoseconds just
-00003400: 7320 6164 6473 2074 6872 6565 2074 7261  s adds three tra
-00003410: 696c 696e 6720 7a65 726f 7320 6173 2064  iling zeros as d
-00003420: 6174 6574 696d 6520 6f62 6a65 6374 2064  atetime object d
-00003430: 6f65 736e 2774 2068 6176 6520 6e61 6e6f  oesn't have nano
-00003440: 7365 636f 6e64 732e 0a20 2020 2020 2020  seconds..       
-00003450: 2064 6174 655f 6e73 203d 2044 6174 6574   date_ns = Datet
-00003460: 696d 6543 6f6e 7665 7274 6572 2e74 6f5f  imeConverter.to_
-00003470: 6e61 6e6f 7365 636f 6e64 7328 6461 7465  nanoseconds(date
-00003480: 7469 6d65 5f6f 626a 290a 2020 2020 2020  time_obj).      
-00003490: 2020 0a20 2020 2020 2020 2023 205b 322e    .        # [2.
-000034a0: 325d 2044 6174 6574 696d 6553 7472 696e  2] DatetimeStrin
-000034b0: 6743 6f6e 7665 7274 6572 0a20 2020 2020  gConverter.     
-000034c0: 2020 2023 2044 6174 6574 696d 6553 7472     # DatetimeStr
-000034d0: 696e 6743 6f6e 7665 7274 6572 2074 616b  ingConverter tak
-000034e0: 6573 2073 7472 696e 6720 696e 2022 7979  es string in "yy
-000034f0: 7979 2d4d 4d2d 6464 5448 483a 6d6d 3a73  yy-MM-ddTHH:mm:s
-00003500: 735b 2e53 5353 5353 5353 5353 5d5a 2220  s[.SSSSSSSSS]Z" 
-00003510: 666f 726d 6174 2e0a 2020 2020 2020 2020  format..        
-00003520: 0a20 2020 2020 2020 2064 6174 655f 7374  .        date_st
-00003530: 7269 6e67 203d 2022 3230 3233 2d30 312d  ring = "2023-01-
-00003540: 3035 5431 343a 3338 3a32 352e 3030 3134  05T14:38:25.0014
-00003550: 365a 220a 2020 2020 2020 2020 0a20 2020  6Z".        .   
-00003560: 2020 2020 2023 2057 6520 6861 7665 2073       # We have s
-00003570: 616d 6520 6d65 7468 6f64 7320 6173 2069  ame methods as i
-00003580: 6e20 4461 7465 7469 6d65 436f 6e76 6572  n DatetimeConver
-00003590: 7465 720a 2020 2020 2020 2020 6461 7465  ter.        date
-000035a0: 5f6d 735f 6672 6f6d 5f73 7472 696e 6720  _ms_from_string 
-000035b0: 3d20 4461 7465 7469 6d65 5374 7269 6e67  = DatetimeString
-000035c0: 436f 6e76 6572 7465 722e 746f 5f6d 696c  Converter.to_mil
-000035d0: 6c69 7365 636f 6e64 7328 6461 7465 5f73  liseconds(date_s
-000035e0: 7472 696e 6729 0a20 2020 2020 2020 2064  tring).        d
-000035f0: 6174 655f 7573 5f66 726f 6d5f 7374 7269  ate_us_from_stri
-00003600: 6e67 203d 2044 6174 6574 696d 6553 7472  ng = DatetimeStr
-00003610: 696e 6743 6f6e 7665 7274 6572 2e74 6f5f  ingConverter.to_
-00003620: 6d69 6372 6f73 6563 6f6e 6473 2864 6174  microseconds(dat
-00003630: 655f 7374 7269 6e67 290a 2020 2020 2020  e_string).      
-00003640: 2020 6461 7465 5f6e 735f 6672 6f6d 5f73    date_ns_from_s
-00003650: 7472 696e 6720 3d20 4461 7465 7469 6d65  tring = Datetime
-00003660: 5374 7269 6e67 436f 6e76 6572 7465 722e  StringConverter.
-00003670: 746f 5f6e 616e 6f73 6563 6f6e 6473 2864  to_nanoseconds(d
-00003680: 6174 655f 7374 7269 6e67 290a 2020 2020  ate_string).    
-00003690: 2020 2020 0a20 2020 2020 2020 2023 2057      .        # W
-000036a0: 6520 6361 6e20 616c 736f 2067 6574 2064  e can also get d
-000036b0: 6174 6574 696d 6520 6f62 6a65 6374 2066  atetime object f
-000036c0: 726f 6d20 7374 7269 6e67 0a20 2020 2020  rom string.     
-000036d0: 2020 2064 6174 6574 696d 655f 6672 6f6d     datetime_from
-000036e0: 5f73 7472 696e 6720 3d20 4461 7465 7469  _string = Dateti
-000036f0: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
-00003700: 722e 746f 5f64 6174 6574 696d 6528 6461  r.to_datetime(da
-00003710: 7465 5f73 7472 696e 6729 0a20 2020 2020  te_string).     
-00003720: 2020 200a 2020 2020 2020 2020 2320 5b32     .        # [2
-00003730: 2e33 5d20 5072 6f74 6f62 7566 5469 6d65  .3] ProtobufTime
-00003740: 7374 616d 7043 6f6e 7665 7274 6572 0a20  stampConverter. 
-00003750: 2020 2020 2020 2023 2050 726f 746f 6275         # Protobu
-00003760: 6620 7469 6d65 7374 616d 7073 206d 7573  f timestamps mus
-00003770: 7420 6265 2069 6e20 666f 726d 207b 2265  t be in form {"e
-00003780: 706f 6368 5365 636f 6e64 223a 2073 6563  pochSecond": sec
-00003790: 6f6e 6473 2c20 226e 616e 6f22 3a20 6e61  onds, "nano": na
-000037a0: 6e6f 7365 636f 6e64 737d 0a20 2020 2020  noseconds}.     
-000037b0: 2020 200a 2020 2020 2020 2020 7072 6f74     .        prot
-000037c0: 6f62 7566 5f74 696d 6573 7461 6d70 203d  obuf_timestamp =
-000037d0: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
-000037e0: 2031 3637 3239 3239 3530 352c 2022 6e61   1672929505, "na
-000037f0: 6e6f 223a 2031 5f34 3630 5f30 3030 7d0a  no": 1_460_000}.
-00003800: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00003810: 2064 6174 655f 6d73 5f66 726f 6d5f 7469   date_ms_from_ti
-00003820: 6d65 7374 616d 7020 3d20 5072 6f74 6f62  mestamp = Protob
-00003830: 7566 5469 6d65 7374 616d 7043 6f6e 7665  ufTimestampConve
-00003840: 7274 6572 2e74 6f5f 6d69 6c6c 6973 6563  rter.to_millisec
-00003850: 6f6e 6473 2870 726f 746f 6275 665f 7469  onds(protobuf_ti
-00003860: 6d65 7374 616d 7029 0a20 2020 2020 2020  mestamp).       
-00003870: 2064 6174 655f 7573 5f66 726f 6d5f 7469   date_us_from_ti
-00003880: 6d65 7374 616d 7020 3d20 5072 6f74 6f62  mestamp = Protob
-00003890: 7566 5469 6d65 7374 616d 7043 6f6e 7665  ufTimestampConve
-000038a0: 7274 6572 2e74 6f5f 6d69 6372 6f73 6563  rter.to_microsec
-000038b0: 6f6e 6473 2870 726f 746f 6275 665f 7469  onds(protobuf_ti
-000038c0: 6d65 7374 616d 7029 0a20 2020 2020 2020  mestamp).       
-000038d0: 2064 6174 655f 6e73 5f66 726f 6d5f 7469   date_ns_from_ti
-000038e0: 6d65 7374 616d 7020 3d20 5072 6f74 6f62  mestamp = Protob
-000038f0: 7566 5469 6d65 7374 616d 7043 6f6e 7665  ufTimestampConve
-00003900: 7274 6572 2e74 6f5f 6e61 6e6f 7365 636f  rter.to_nanoseco
-00003910: 6e64 7328 7072 6f74 6f62 7566 5f74 696d  nds(protobuf_tim
-00003920: 6573 7461 6d70 290a 2020 2020 2020 2020  estamp).        
-00003930: 6461 7465 7469 6d65 5f66 726f 6d5f 7469  datetime_from_ti
-00003940: 6d65 7374 616d 7020 3d20 5072 6f74 6f62  mestamp = Protob
-00003950: 7566 5469 6d65 7374 616d 7043 6f6e 7665  ufTimestampConve
-00003960: 7274 6572 2e74 6f5f 6461 7465 7469 6d65  rter.to_datetime
-00003970: 2870 726f 746f 6275 665f 7469 6d65 7374  (protobuf_timest
-00003980: 616d 7029 0a20 2020 2020 2020 200a 2020  amp).        .  
-00003990: 2020 2020 2020 2320 5b33 5d20 576f 726b        # [3] Work
-000039a0: 696e 6720 7769 7468 2045 7665 6e74 5472  ing with EventTr
-000039b0: 6565 2061 6e64 2045 7665 6e74 5472 6565  ee and EventTree
-000039c0: 436f 6c6c 6563 7469 6f6e 2e0a 2020 2020  Collection..    
-000039d0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-000039e0: 332e 315d 2042 7569 6c64 2061 2063 7573  3.1] Build a cus
-000039f0: 746f 6d20 4576 656e 7454 7265 650a 2020  tom EventTree.  
-00003a00: 2020 2020 2020 2320 546f 2063 7265 6174        # To creat
-00003a10: 6520 616e 2045 7665 6e74 5472 6565 206f  e an EventTree o
-00003a20: 626a 6563 7420 796f 7520 6e65 6564 2074  bject you need t
-00003a30: 6f20 7072 6f76 6964 6520 6e61 6d65 2c20  o provide name, 
-00003a40: 6964 2061 6e64 2064 6174 6120 6f66 2074  id and data of t
-00003a50: 6865 2072 6f6f 7420 6576 656e 742e 0a20  he root event.. 
-00003a60: 2020 2020 2020 2074 7265 6520 3d20 4576         tree = Ev
-00003a70: 656e 7454 7265 6528 6576 656e 745f 6e61  entTree(event_na
-00003a80: 6d65 3d22 726f 6f74 2065 7665 6e74 222c  me="root event",
-00003a90: 2065 7665 6e74 5f69 643d 2272 6f6f 745f   event_id="root_
-00003aa0: 6964 222c 2064 6174 613d 7b22 6461 7461  id", data={"data
-00003ab0: 223a 205b 312c 2032 2c20 332c 2034 2c20  ": [1, 2, 3, 4, 
-00003ac0: 355d 7d29 0a20 2020 2020 2020 200a 2020  5]}).        .  
-00003ad0: 2020 2020 2020 2320 546f 2061 6464 206e        # To add n
-00003ae0: 6577 206e 6f64 6520 7573 6520 6170 7065  ew node use appe
-00003af0: 6e64 5f65 7665 6e74 2e20 7061 7265 6e74  nd_event. parent
-00003b00: 5f69 6420 6973 206e 6563 6573 7361 7279  _id is necessary
-00003b10: 2c20 6461 7461 2069 7320 6f70 7469 6f6e  , data is option
-00003b20: 616c 2e0a 2020 2020 2020 2020 7472 6565  al..        tree
-00003b30: 2e61 7070 656e 645f 6576 656e 7428 6576  .append_event(ev
-00003b40: 656e 745f 6e61 6d65 3d22 4122 2c20 6576  ent_name="A", ev
-00003b50: 656e 745f 6964 3d22 415f 6964 222c 2064  ent_id="A_id", d
-00003b60: 6174 613d 4e6f 6e65 2c20 7061 7265 6e74  ata=None, parent
-00003b70: 5f69 643d 2272 6f6f 745f 6964 2229 0a20  _id="root_id"). 
-00003b80: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003b90: 2320 5b33 2e33 5d20 4275 696c 6469 6e67  # [3.3] Building
-00003ba0: 2074 6865 2045 7665 6e74 5472 6565 436f   the EventTreeCo
-00003bb0: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
-00003bc0: 2020 0a20 2020 2020 2020 2023 2049 6620    .        # If 
-00003bd0: 796f 7520 646f 6e27 7420 7370 6563 6966  you don't specif
-00003be0: 7920 6461 7461 5f73 6f75 7263 6520 666f  y data_source fo
-00003bf0: 7220 7468 6520 6472 6976 6572 2074 6865  r the driver the
-00003c00: 6e20 6974 2077 6f6e 2774 2072 6563 6f76  n it won't recov
-00003c10: 6572 2064 6574 6163 6865 6420 6576 656e  er detached even
-00003c20: 7473 2e0a 2020 2020 2020 2020 6472 6976  ts..        driv
-00003c30: 6572 3a20 4945 5443 4472 6976 6572 2020  er: IETCDriver  
-00003c40: 2320 596f 7520 7368 6f75 6c64 2069 6e69  # You should ini
-00003c50: 7420 4554 4344 7269 7665 7220 6f62 6a65  t ETCDriver obje
-00003c60: 6374 2e20 452e 672e 2066 726f 6d20 4c77  ct. E.g. from Lw
-00003c70: 4450 206d 6f64 756c 6520 6f72 2079 6f75  DP module or you
-00003c80: 7220 6375 7374 6f6d 2063 6c61 7373 2e0a  r custom class..
-00003c90: 2020 2020 2020 2020 6574 6320 3d20 4576          etc = Ev
-00003ca0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00003cb0: 6e28 6472 6976 6572 290a 2020 2020 2020  n(driver).      
-00003cc0: 2020 6574 632e 6275 696c 6428 6576 656e    etc.build(even
-00003cd0: 7473 290a 2020 2020 2020 2020 0a20 2020  ts).        .   
-00003ce0: 2020 2020 2023 2044 6574 6163 6865 6420       # Detached 
-00003cf0: 6576 656e 7473 2069 736e 2774 2065 6d70  events isn't emp
-00003d00: 7479 2e0a 2020 2020 2020 2020 6173 7365  ty..        asse
-00003d10: 7274 2065 7463 2e67 6574 5f64 6574 6163  rt etc.get_detac
-00003d20: 6865 645f 6576 656e 7473 2829 0a20 2020  hed_events().   
-00003d30: 2020 2020 200a 2020 2020 2020 2020 6574       .        et
-00003d40: 6320 3d20 4576 656e 7454 7265 6543 6f6c  c = EventTreeCol
-00003d50: 6c65 6374 696f 6e28 6472 6976 6572 290a  lection(driver).
-00003d60: 2020 2020 2020 2020 2320 4465 7461 6368          # Detach
-00003d70: 6564 2065 7665 6e74 7320 6172 6520 656d  ed events are em
-00003d80: 7074 7920 6265 6361 7573 6520 7468 6579  pty because they
-00003d90: 2077 6572 6520 7265 636f 7665 7265 642e   were recovered.
-00003da0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00003db0: 6e6f 7420 6574 632e 6765 745f 6465 7461  not etc.get_deta
-00003dc0: 6368 6564 5f65 7665 6e74 7328 290a 2020  ched_events().  
-00003dd0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00003de0: 2054 6865 2063 6f6c 6c65 6374 696f 6e20   The collection 
-00003df0: 6861 7320 4576 656e 7454 7265 6573 2065  has EventTrees e
-00003e00: 6163 6820 7769 7468 2061 2074 7265 6520  ach with a tree 
-00003e10: 6f66 2065 7665 6e74 732e 0a20 2020 2020  of events..     
-00003e20: 2020 2023 2055 7369 6e67 2043 6f6c 6c65     # Using Colle
-00003e30: 6374 696f 6e20 616e 6420 4576 656e 7454  ction and EventT
-00003e40: 7265 6573 2c20 796f 7520 6361 6e20 776f  rees, you can wo
-00003e50: 726b 2066 6c65 7869 626c 7920 7769 7468  rk flexibly with
-00003e60: 2065 7665 6e74 732e 0a20 2020 2020 2020   events..       
-00003e70: 200a 2020 2020 2020 2020 2320 5b33 2e33   .        # [3.3
-00003e80: 2e31 5d20 4765 7420 6c65 6176 6573 206f  .1] Get leaves o
-00003e90: 6620 616c 6c20 7472 6565 732e 0a20 2020  f all trees..   
-00003ea0: 2020 2020 206c 6561 7665 733a 2054 7570       leaves: Tup
-00003eb0: 6c65 5b64 6963 745d 203d 2065 7463 2e67  le[dict] = etc.g
-00003ec0: 6574 5f6c 6561 7665 7328 290a 2020 2020  et_leaves().    
+000005f0: 2020 2020 2a20 5b46 6965 6c64 7352 6573      * [FieldsRes
+00000600: 6f6c 7665 725d 2823 6669 656c 6473 7265  olver](#fieldsre
+00000610: 736f 6c76 6572 290a 2020 2020 2020 2020  solver).        
+00000620: 2020 202a 205b 322e 342e 204c 696e 6b73     * [2.4. Links
+00000630: 5d28 2332 342d 6c69 6e6b 7329 0a20 2020  ](#24-links).   
+00000640: 2020 2020 202a 205b 332e 2042 6573 7420       * [3. Best 
+00000650: 7072 6163 7469 6365 735d 2823 332d 6265  practices](#3-be
+00000660: 7374 2d70 7261 6374 6963 6573 290a 2020  st-practices).  
+00000670: 2020 2020 2020 2a20 5b34 2e20 4f66 6669        * [4. Offi
+00000680: 6369 616c 2044 6174 6153 6f75 7263 6520  cial DataSource 
+00000690: 696d 706c 656d 656e 7461 7469 6f6e 735d  implementations]
+000006a0: 2823 342d 6f66 6669 6369 616c 2d64 6174  (#4-official-dat
+000006b0: 6173 6f75 7263 652d 696d 706c 656d 656e  asource-implemen
+000006c0: 7461 7469 6f6e 7329 0a20 2020 2020 2020  tations).       
+000006d0: 202a 205b 352e 2041 5049 5d28 2335 2d61   * [5. API](#5-a
+000006e0: 7069 290a 2020 2020 2020 2020 2a20 5b36  pi).        * [6
+000006f0: 2e20 4578 616d 706c 6573 5d28 2336 2d65  . Examples](#6-e
+00000700: 7861 6d70 6c65 7329 0a20 2020 2020 2020  xamples).       
+00000710: 203c 212d 2d74 652d 2d3e 0a20 2020 2020   <!--te-->.     
+00000720: 2020 200a 2020 2020 2020 2020 2320 312e     .        # 1.
+00000730: 2049 6e74 726f 6475 6374 696f 6e0a 2020   Introduction.  
+00000740: 2020 2020 2020 0a20 2020 2020 2020 2054        .        T
+00000750: 6869 7320 7265 706f 7369 746f 7279 2069  his repository i
+00000760: 7320 6120 6c69 6272 6172 7920 666f 7220  s a library for 
+00000770: 6372 6561 7469 6e67 2074 6832 2d64 6174  creating th2-dat
+00000780: 612d 7365 7276 6963 6573 2061 7070 6c69  a-services appli
+00000790: 6361 7469 6f6e 732e 0a20 2020 2020 2020  cations..       
+000007a0: 2044 6174 6120 5365 7276 6963 6573 2061   Data Services a
+000007b0: 6c6c 6f77 7320 796f 7520 746f 206d 616e  llows you to man
+000007c0: 6970 756c 6174 6520 7468 6520 7374 7265  ipulate the stre
+000007d0: 616d 2064 6174 6120 7072 6f63 6573 7369  am data processi
+000007e0: 6e67 2077 6f72 6b66 6c6f 7720 7573 696e  ng workflow usin
+000007f0: 6720 7069 7065 6c69 6e69 6e67 2e0a 2020  g pipelining..  
+00000800: 2020 2020 2020 0a20 2020 2020 2020 2054        .        T
+00000810: 6865 206c 6962 7261 7279 2773 2066 6561  he library's fea
+00000820: 7475 7265 733a 0a20 2020 2020 2020 200a  tures:.        .
+00000830: 2020 2020 2020 2020 2d20 5072 6f76 6964          - Provid
+00000840: 6573 2063 6f72 6520 696e 7465 7266 6163  es core interfac
+00000850: 6520 666f 7220 6465 7665 6c6f 7069 6e67  e for developing
+00000860: 2064 6174 6120 736f 7572 6365 2069 6d70   data source imp
+00000870: 6c65 6d65 6e74 6174 696f 6e73 0a20 2020  lementations.   
+00000880: 2020 2020 202d 2057 6f72 6b20 7769 7468       - Work with
+00000890: 2069 7465 7261 626c 6520 6f62 6a65 6374   iterable object
+000008a0: 7320 286c 6973 742c 2074 7570 6c65 2c20  s (list, tuple, 
+000008b0: 6574 6320 696e 636c 7564 696e 6720 6669  etc including fi
+000008c0: 6c65 7329 2076 6961 205f 4461 7461 206f  les) via _Data o
+000008d0: 626a 6563 745f 2075 7369 6e67 2069 7473  bject_ using its
+000008e0: 2066 6561 7475 7265 730a 2020 2020 2020   features.      
+000008f0: 2020 2d20 4d61 6e69 7075 6c61 7465 2074    - Manipulate t
+00000900: 6865 2077 6f72 6b66 6c6f 7720 746f 206d  he workflow to m
+00000910: 616b 6520 736f 6d65 2061 6e61 6c79 7369  ake some analysi
+00000920: 7320 6279 205f 4461 7461 206f 626a 6563  s by _Data objec
+00000930: 745f 206d 6574 686f 6473 0a20 2020 2020  t_ methods.     
+00000940: 2020 202d 2055 7365 2074 696d 6573 7461     - Use timesta
+00000950: 6d70 2063 6f6e 7665 7274 6572 2069 6d70  mp converter imp
+00000960: 6c65 6d65 6e74 6174 696f 6e73 206f 7220  lementations or 
+00000970: 7573 6520 6261 7365 2063 6c61 7373 2074  use base class t
+00000980: 6f20 6372 6561 7465 2063 7573 746f 6d20  o create custom 
+00000990: 636f 6e76 6572 7465 7273 0a20 2020 2020  converters.     
+000009a0: 2020 202d 2042 7569 6c64 2045 7665 6e74     - Build Event
+000009b0: 2054 7265 6573 2028 4576 656e 7454 7265   Trees (EventTre
+000009c0: 652c 2045 7665 6e74 5472 6565 436f 6c6c  e, EventTreeColl
+000009d0: 6563 7469 6f6e 2061 6e64 2050 6172 656e  ection and Paren
+000009e0: 7445 7665 6e74 5472 6565 436f 6c6c 6563  tEventTreeCollec
+000009f0: 7469 6f6e 2063 6c61 7373 6573 290a 2020  tion classes).  
+00000a00: 2020 2020 2020 0a20 2020 2020 2020 2057        .        W
+00000a10: 6f72 6b66 6c6f 7720 6d61 6e69 7075 6c61  orkflow manipula
+00000a20: 7469 6f6e 2074 6f6f 6c73 2061 6c6c 6f77  tion tools allow
+00000a30: 7320 796f 753a 0a20 2020 2020 2020 200a  s you:.        .
+00000a40: 2020 2020 2020 2020 2d20 4669 6c74 6572          - Filter
+00000a50: 696e 6720 7374 7265 616d 2064 6174 6120  ing stream data 
+00000a60: 2860 4461 7461 2e66 696c 7465 7260 206d  (`Data.filter` m
+00000a70: 6574 686f 6429 0a20 2020 2020 2020 202d  ethod).        -
+00000a80: 2054 7261 6e73 666f 726d 696e 6720 7374   Transforming st
+00000a90: 7265 616d 2064 6174 6120 2860 4461 7461  ream data (`Data
+00000aa0: 2e6d 6170 6020 6d65 7468 6f64 290a 2020  .map` method).  
+00000ab0: 2020 2020 2020 2d20 4c69 6d69 7469 6e67        - Limiting
+00000ac0: 2074 6865 206e 756d 6265 7220 6f66 2070   the number of p
+00000ad0: 726f 6365 7373 6564 2073 7472 6561 6d69  rocessed streami
+00000ae0: 6e67 2064 6174 6120 2860 4461 7461 2e6c  ng data (`Data.l
+00000af0: 696d 6974 6020 6d65 7468 6f64 290a 2020  imit` method).  
+00000b00: 2020 2020 2020 0a20 2020 2020 2020 2054        .        T
+00000b10: 6865 7265 2069 7320 616c 736f 2061 6e6f  here is also ano
+00000b20: 7468 6572 2070 6172 7420 6f66 205f 6461  ther part of _da
+00000b30: 7461 2073 6572 7669 6365 735f 0a20 2020  ta services_.   
+00000b40: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00000b50: 5b74 6832 2d64 6174 612d 7365 7276 6963  [th2-data-servic
+00000b60: 6573 2d75 7469 6c73 5d28 6874 7470 733a  es-utils](https:
+00000b70: 2f2f 6769 7468 7562 2e63 6f6d 2f74 6832  //github.com/th2
+00000b80: 2d6e 6574 2f74 6832 2d64 6174 612d 7365  -net/th2-data-se
+00000b90: 7276 6963 6573 2d75 7469 6c73 292e 2049  rvices-utils). I
+00000ba0: 7427 7320 6120 7365 7420 6f66 2074 6f6f  t's a set of too
+00000bb0: 6c73 2074 6f20 7065 7266 6f72 6d20 7468  ls to perform th
+00000bc0: 6520 6d6f 7374 0a20 2020 2020 2020 2020  e most.         
+00000bd0: 2063 6f6d 6d6f 6e20 616e 616c 7973 6973   common analysis
+00000be0: 2074 6173 6b73 2e0a 2020 2020 2020 2020   tasks..        
+00000bf0: 0a20 2020 2020 2020 2023 2032 2e20 4765  .        # 2. Ge
+00000c00: 7474 696e 6720 7374 6172 7465 640a 2020  tting started.  
+00000c10: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00000c20: 2320 322e 312e 2049 6e73 7461 6c6c 6174  # 2.1. Installat
+00000c30: 696f 6e0a 2020 2020 2020 2020 0a20 2020  ion.        .   
+00000c40: 2020 2020 2023 2323 2043 6f72 650a 2020       ### Core.  
+00000c50: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00000c60: 2046 726f 6d20 5079 5049 2028 7069 7029   From PyPI (pip)
+00000c70: 2020 200a 2020 2020 2020 2020 2020 5468     .          Th
+00000c80: 6973 2070 6163 6b61 6765 2063 616e 2062  is package can b
+00000c90: 6520 666f 756e 6420 6f6e 205b 5079 5049  e found on [PyPI
+00000ca0: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+00000cb0: 7267 2f70 726f 6a65 6374 2f74 6832 2d64  rg/project/th2-d
+00000cc0: 6174 612d 7365 7276 6963 6573 2f20 2274  ata-services/ "t
+00000cd0: 6832 2d64 6174 612d 7365 7276 6963 6573  h2-data-services
+00000ce0: 2229 2e0a 2020 2020 2020 2020 2020 2020  ")..            
+00000cf0: 6060 600a 2020 2020 2020 2020 2020 2020  ```.            
+00000d00: 7069 7020 696e 7374 616c 6c20 7468 322d  pip install th2-
+00000d10: 6461 7461 2d73 6572 7669 6365 730a 2020  data-services.  
+00000d20: 2020 2020 2020 2020 2020 6060 600a 2020            ```.  
+00000d30: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00000d40: 2046 726f 6d20 536f 7572 6365 0a20 2020   From Source.   
+00000d50: 2020 2020 2020 2020 2060 6060 0a20 2020           ```.   
+00000d60: 2020 2020 2020 2020 2067 6974 2063 6c6f           git clo
+00000d70: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
+00000d80: 622e 636f 6d2f 7468 322d 6e65 742f 7468  b.com/th2-net/th
+00000d90: 322d 6461 7461 2d73 6572 7669 6365 730a  2-data-services.
+00000da0: 2020 2020 2020 2020 2020 2020 7069 7020              pip 
+00000db0: 696e 7374 616c 6c20 7468 322d 6461 7461  install th2-data
+00000dc0: 2d73 6572 7669 6365 732f 0a20 2020 2020  -services/.     
+00000dd0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00000de0: 2020 200a 2020 2020 2020 2020 2323 2320     .        ### 
+00000df0: 4461 7461 2073 6f75 7263 6573 2028 7072  Data sources (pr
+00000e00: 6f76 6964 6572 7329 0a20 2020 2020 2020  oviders).       
+00000e10: 200a 2020 2020 2020 2020 5369 6e63 6520   .        Since 
+00000e20: 6076 312e 332e 3060 2c20 7468 6520 6c69  `v1.3.0`, the li
+00000e30: 6272 6172 7920 646f 6573 6e27 7420 7072  brary doesn't pr
+00000e40: 6f76 6964 6520 6461 7461 2073 6f75 7263  ovide data sourc
+00000e50: 6520 6465 7065 6e64 656e 6369 6573 2e0a  e dependencies..
+00000e60: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000e70: 2059 6f75 2073 686f 756c 6420 7072 6f76   You should prov
+00000e80: 6964 6520 6974 206d 616e 7561 6c6c 7920  ide it manually 
+00000e90: 6475 7269 6e67 2069 6e73 7461 6c6c 6174  during installat
+00000ea0: 696f 6e2e 200a 2020 2020 2020 2020 596f  ion. .        Yo
+00000eb0: 7520 6a75 7374 206e 6565 6420 746f 2061  u just need to a
+00000ec0: 6464 2073 7175 6172 6520 6272 6163 6b65  dd square bracke
+00000ed0: 7473 2061 6674 6572 206c 6962 7261 7279  ts after library
+00000ee0: 206e 616d 6520 616e 6420 7075 7420 6465   name and put de
+00000ef0: 7065 6e64 656e 6379 206e 616d 652e 0a20  pendency name.. 
+00000f00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000f10: 6060 600a 2020 2020 2020 2020 7069 7020  ```.        pip 
+00000f20: 696e 7374 616c 6c20 7468 322d 6461 7461  install th2-data
+00000f30: 2d73 6572 7669 6365 735b 6465 7065 6e64  -services[depend
+00000f40: 656e 6379 5f6e 616d 655d 0a20 2020 2020  ency_name].     
+00000f50: 2020 2060 6060 0a20 2020 2020 2020 200a     ```.        .
+00000f60: 2020 2020 2020 2020 2a2a 4465 7065 6e64          **Depend
+00000f70: 656e 6369 6573 206c 6973 742a 2a20 0a20  encies list** . 
+00000f80: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000f90: 7c20 2064 6570 656e 6465 6e63 7920 6e61  |  dependency na
+00000fa0: 6d65 2020 7c20 7072 6f76 6964 6572 2076  me  | provider v
+00000fb0: 6572 7369 6f6e 2020 2020 2020 2020 2020  ersion          
+00000fc0: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
+00000fd0: 2020 2020 2020 7c3a 2d2d 2d2d 2d2d 2d2d        |:--------
+00000fe0: 2d2d 2d2d 2d2d 2d2d 2d3a 7c2d 2d2d 2d2d  ---------:|-----
+00000ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001010: 2d2d 7c0a 2020 2020 2020 2020 7c20 2020  --|.        |   
+00001020: 2020 2020 6c77 6470 2020 2020 2020 2020      lwdp        
+00001030: 7c20 6c61 7465 7374 2076 6572 7369 6f6e  | latest version
+00001040: 206f 6620 6c77 6470 2020 2020 2020 2020   of lwdp        
+00001050: 2020 2020 2020 2020 7c0a 2020 2020 2020          |.      
+00001060: 2020 7c20 2020 2020 2020 6c77 6470 3220    |       lwdp2 
+00001070: 2020 2020 2020 7c20 6c61 7465 7374 2076        | latest v
+00001080: 6572 7369 6f6e 206f 6620 6c77 6470 2076  ersion of lwdp v
+00001090: 3220 2020 2020 2020 2020 2020 2020 7c0a  2             |.
+000010a0: 2020 2020 2020 2020 7c20 7574 696c 732d          | utils-
+000010b0: 7270 742d 7669 6577 6572 2020 7c20 6c61  rpt-viewer  | la
+000010c0: 7465 7374 2076 6572 7369 6f6e 206f 6620  test version of 
+000010d0: 7574 696c 732d 7270 742d 7669 6577 6572  utils-rpt-viewer
+000010e0: 2020 2020 7c0a 2020 2020 2020 2020 7c20      |.        | 
+000010f0: 7574 696c 732d 7270 742d 7669 6577 6572  utils-rpt-viewer
+00001100: 3520 7c20 6c61 7465 7374 2076 6572 7369  5 | latest versi
+00001110: 6f6e 206f 6620 7574 696c 732d 7270 742d  on of utils-rpt-
+00001120: 7669 6577 6572 2076 3520 7c0a 2020 2020  viewer v5 |.    
+00001130: 2020 2020 7c20 2020 7574 696c 732d 6164      |   utils-ad
+00001140: 7661 6e63 6564 2020 7c20 6c61 7465 7374  vanced  | latest
+00001150: 2076 6572 7369 6f6e 206f 6620 6473 2d75   version of ds-u
+00001160: 7469 6c73 2020 2020 2020 2020 2020 2020  tils            
+00001170: 7c0a 2020 2020 2020 2020 0a20 2020 2020  |.        .     
+00001180: 2020 202a 2a45 7861 6d70 6c65 2a2a 0a20     **Example**. 
+00001190: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000011a0: 6060 600a 2020 2020 2020 2020 7069 7020  ```.        pip 
+000011b0: 696e 7374 616c 6c20 7468 322d 6461 7461  install th2-data
+000011c0: 2d73 6572 7669 6365 735b 6c77 6470 315d  -services[lwdp1]
+000011d0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+000011e0: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
+000011f0: 2032 2e32 2e20 4578 616d 706c 650a 2020   2.2. Example.  
+00001200: 2020 2020 2020 0a20 2020 2020 2020 2041        .        A
+00001210: 2067 6f6f 642c 2073 686f 7274 2065 7861   good, short exa
+00001220: 6d70 6c65 2069 7320 776f 7274 6820 6120  mple is worth a 
+00001230: 7468 6f75 7361 6e64 2077 6f72 6473 2e0a  thousand words..
+00001240: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001250: 2054 6869 7320 6578 616d 706c 6520 7368   This example sh
+00001260: 6f77 7320 6261 7369 6320 7573 6167 6520  ows basic usage 
+00001270: 6f66 206c 6962 7261 7279 2773 2066 6561  of library's fea
+00001280: 7475 7265 732e 0a20 2020 2020 2020 200a  tures..        .
+00001290: 2020 2020 2020 2020 5b54 6865 2066 6f6c          [The fol
+000012a0: 6c6f 7769 6e67 2065 7861 6d70 6c65 2061  lowing example a
+000012b0: 7320 6120 6669 6c65 5d28 6578 616d 706c  s a file](exampl
+000012c0: 6573 2f67 6574 5f73 7461 7274 6564 5f65  es/get_started_e
+000012d0: 7861 6d70 6c65 2e70 7929 2e0a 2020 2020  xample.py)..    
+000012e0: 2020 2020 0a20 2020 2020 2020 203c 212d      .        <!-
+000012f0: 2d20 7374 6172 7420 6765 745f 7374 6172  - start get_star
+00001300: 7465 645f 6578 616d 706c 652e 7079 202d  ted_example.py -
+00001310: 2d3e 0a20 2020 2020 2020 2060 6060 7079  ->.        ```py
+00001320: 7468 6f6e 0a20 2020 2020 2020 2066 726f  thon.        fro
+00001330: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00001340: 5475 706c 652c 204c 6973 742c 204f 7074  Tuple, List, Opt
+00001350: 696f 6e61 6c2c 2047 656e 6572 6174 6f72  ional, Generator
+00001360: 0a20 2020 2020 2020 2066 726f 6d20 6461  .        from da
+00001370: 7465 7469 6d65 2069 6d70 6f72 7420 6461  tetime import da
+00001380: 7465 7469 6d65 0a20 2020 2020 2020 200a  tetime.        .
+00001390: 2020 2020 2020 2020 6672 6f6d 2074 6832          from th2
+000013a0: 5f64 6174 615f 7365 7276 6963 6573 2e64  _data_services.d
+000013b0: 6174 6120 696d 706f 7274 2044 6174 610a  ata import Data.
+000013c0: 2020 2020 2020 2020 6672 6f6d 2074 6832          from th2
+000013d0: 5f64 6174 615f 7365 7276 6963 6573 2e65  _data_services.e
+000013e0: 7665 6e74 5f74 7265 6520 696d 706f 7274  vent_tree import
+000013f0: 2045 7665 6e74 5472 6565 2c20 4576 656e   EventTree, Even
+00001400: 7454 7265 6543 6f6c 6c65 6374 696f 6e2c  tTreeCollection,
+00001410: 2050 6172 656e 7445 7665 6e74 5472 6565   ParentEventTree
+00001420: 436f 6c6c 6563 7469 6f6e 2c20 4945 5443  Collection, IETC
+00001430: 4472 6976 6572 0a20 2020 2020 2020 2066  Driver.        f
+00001440: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
+00001450: 7669 6365 732e 696e 7465 7266 6163 6573  vices.interfaces
+00001460: 2069 6d70 6f72 7420 4944 6174 6153 6f75   import IDataSou
+00001470: 7263 650a 2020 2020 2020 2020 6672 6f6d  rce.        from
+00001480: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
+00001490: 6573 2e75 7469 6c73 2e63 6f6e 7665 7274  es.utils.convert
+000014a0: 6572 7320 696d 706f 7274 2044 6174 6574  ers import Datet
+000014b0: 696d 6543 6f6e 7665 7274 6572 2c20 4461  imeConverter, Da
+000014c0: 7465 7469 6d65 5374 7269 6e67 436f 6e76  tetimeStringConv
+000014d0: 6572 7465 722c 2050 726f 746f 6275 6654  erter, ProtobufT
+000014e0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
+000014f0: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
+00001500: 2020 2023 205b 305d 204c 6962 2063 6f6e     # [0] Lib con
+00001510: 6669 6775 7261 7469 6f6e 0a20 2020 2020  figuration.     
+00001520: 2020 2023 205b 302e 315d 2049 6e74 6572     # [0.1] Inter
+00001530: 6163 7469 7665 206f 7220 5363 7269 7074  active or Script
+00001540: 206d 6f64 650a 2020 2020 2020 2020 2320   mode.        # 
+00001550: 4966 2079 6f75 2075 7365 2074 6865 206c  If you use the l
+00001560: 6962 2069 6e20 696e 7465 7261 6374 6976  ib in interactiv
+00001570: 6520 6d6f 6465 2028 6a75 7079 7465 722c  e mode (jupyter,
+00001580: 2069 7079 7468 6f6e 2920 6974 2773 2072   ipython) it's r
+00001590: 6563 6f6d 6d65 6e64 6564 2074 6f20 7365  ecommended to se
+000015a0: 7420 7468 6520 7370 6563 6961 6c0a 2020  t the special.  
+000015b0: 2020 2020 2020 2320 676c 6f62 616c 2070        # global p
+000015c0: 6172 616d 6574 6572 2074 6f20 5472 7565  arameter to True
+000015d0: 2e20 4974 276c 6c20 6b65 6570 2063 6163  . It'll keep cac
+000015e0: 6865 2066 696c 6573 2069 6620 736f 6d65  he files if some
+000015f0: 7468 696e 6720 7765 6e74 2077 726f 6e67  thing went wrong
+00001600: 2e0a 2020 2020 2020 2020 6672 6f6d 2074  ..        from t
+00001610: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
+00001620: 2e63 6f6e 6669 6720 696d 706f 7274 206f  .config import o
+00001630: 7074 696f 6e73 0a20 2020 2020 2020 200a  ptions.        .
+00001640: 2020 2020 2020 2020 6f70 7469 6f6e 732e          options.
+00001650: 494e 5445 5241 4354 4956 455f 4d4f 4445  INTERACTIVE_MODE
+00001660: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+00001670: 0a20 2020 2020 2020 2023 2053 6f6d 6520  .        # Some 
+00001680: 6578 616d 706c 6520 6461 7461 0a20 2020  example data.   
+00001690: 2020 2020 2065 7665 6e74 7320 3d20 4461       events = Da
+000016a0: 7461 280a 2020 2020 2020 2020 2020 2020  ta(.            
+000016b0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+000016c0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+000016d0: 2020 2020 2020 2020 2265 7665 6e74 4964          "eventId
+000016e0: 223a 2022 6465 6d6f 5f62 6f6f 6b5f 313a  ": "demo_book_1:
+000016f0: 7468 322d 7363 6f70 653a 3230 3233 3031  th2-scope:202301
+00001700: 3035 3133 3537 3035 3536 3038 3733 3030  0513570556087300
+00001710: 303a 6436 3165 3933 3061 2d38 6430 302d  0:d61e930a-8d00-
+00001720: 3131 6564 2d61 6131 612d 6433 3461 3631  11ed-aa1a-d34a61
+00001730: 3535 3135 3264 5f31 222c 0a20 2020 2020  55152d_1",.     
+00001740: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001750: 6261 7463 6849 6422 3a20 4e6f 6e65 2c0a  batchId": None,.
+00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001770: 2020 2020 2269 7342 6174 6368 6564 223a      "isBatched":
+00001780: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+00001790: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+000017a0: 6e74 4e61 6d65 223a 2022 5365 7420 6f66  ntName": "Set of
+000017b0: 2061 7574 6f2d 6765 6e65 7261 7465 6420   auto-generated 
+000017c0: 6576 656e 7473 2066 6f72 2064 7320 6c69  events for ds li
+000017d0: 6220 7465 7374 696e 6722 2c0a 2020 2020  b testing",.    
+000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017f0: 2265 7665 6e74 5479 7065 223a 2022 6473  "eventType": "ds
+00001800: 2d6c 6962 2d74 6573 742d 6576 656e 7422  -lib-test-event"
+00001810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001820: 2020 2020 2020 2265 6e64 5469 6d65 7374        "endTimest
+00001830: 616d 7022 3a20 7b22 6570 6f63 6853 6563  amp": {"epochSec
+00001840: 6f6e 6422 3a20 3136 3732 3932 3730 3235  ond": 1672927025
+00001850: 2c20 226e 616e 6f22 3a20 3536 3137 3531  , "nano": 561751
+00001860: 3030 307d 2c0a 2020 2020 2020 2020 2020  000},.          
+00001870: 2020 2020 2020 2020 2020 2273 7461 7274            "start
+00001880: 5469 6d65 7374 616d 7022 3a20 7b22 6570  Timestamp": {"ep
+00001890: 6f63 6853 6563 6f6e 6422 3a20 3136 3732  ochSecond": 1672
+000018a0: 3932 3730 3235 2c20 226e 616e 6f22 3a20  927025, "nano": 
+000018b0: 3536 3038 3733 3030 307d 2c0a 2020 2020  560873000},.    
+000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018d0: 2270 6172 656e 7445 7665 6e74 4964 223a  "parentEventId":
+000018e0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+000018f0: 2020 2020 2020 2020 2020 2022 7375 6363             "succ
+00001900: 6573 7366 756c 223a 2054 7275 652c 0a20  essful": True,. 
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2020 2022 626f 6f6b 4964 223a 2022 6465     "bookId": "de
+00001930: 6d6f 5f62 6f6f 6b5f 3122 2c0a 2020 2020  mo_book_1",.    
+00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001950: 2273 636f 7065 223a 2022 7468 322d 7363  "scope": "th2-sc
+00001960: 6f70 6522 2c0a 2020 2020 2020 2020 2020  ope",.          
+00001970: 2020 2020 2020 2020 2020 2261 7474 6163            "attac
+00001980: 6865 644d 6573 7361 6765 4964 7322 3a20  hedMessageIds": 
+00001990: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+000019a0: 2020 2020 2020 2020 2262 6f64 7922 3a20          "body": 
+000019b0: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+000019c0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+000019d0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000019e0: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
+000019f0: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
+00001a00: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
+00001a10: 3032 3330 3130 3531 3335 3730 3535 3633  0230105135705563
+00001a20: 3532 3230 3030 3a39 6164 6262 3365 302d  522000:9adbb3e0-
+00001a30: 3566 3862 2d34 6332 382d 6132 6163 2d37  5f8b-4c28-a2ac-7
+00001a40: 3336 3165 3866 6137 3034 633e 6465 6d6f  361e8fa704c>demo
+00001a50: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
+00001a60: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
+00001a70: 3536 3335 3232 3030 303a 6436 3165 3933  563522000:d61e93
+00001a80: 3061 2d38 6430 302d 3131 6564 2d61 6131  0a-8d00-11ed-aa1
+00001a90: 612d 6433 3461 3631 3535 3135 3264 5f32  a-d34a6155152d_2
+00001aa0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001ab0: 2020 2020 2020 2022 6261 7463 6849 6422         "batchId"
+00001ac0: 3a20 2264 656d 6f5f 626f 6f6b 5f31 3a74  : "demo_book_1:t
+00001ad0: 6832 2d73 636f 7065 3a32 3032 3330 3130  h2-scope:2023010
+00001ae0: 3531 3335 3730 3535 3633 3532 3230 3030  5135705563522000
+00001af0: 3a39 6164 6262 3365 302d 3566 3862 2d34  :9adbb3e0-5f8b-4
+00001b00: 6332 382d 6132 6163 2d37 3336 3165 3866  c28-a2ac-7361e8f
+00001b10: 6137 3034 6322 2c0a 2020 2020 2020 2020  a704c",.        
+00001b20: 2020 2020 2020 2020 2020 2020 2269 7342              "isB
+00001b30: 6174 6368 6564 223a 2054 7275 652c 0a20  atched": True,. 
+00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b50: 2020 2022 6576 656e 744e 616d 6522 3a20     "eventName": 
+00001b60: 2250 6c61 696e 2065 7665 6e74 2031 222c  "Plain event 1",
+00001b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b80: 2020 2020 2022 6576 656e 7454 7970 6522       "eventType"
+00001b90: 3a20 2264 732d 6c69 622d 7465 7374 2d65  : "ds-lib-test-e
+00001ba0: 7665 6e74 222c 0a20 2020 2020 2020 2020  vent",.         
+00001bb0: 2020 2020 2020 2020 2020 2022 656e 6454             "endT
+00001bc0: 696d 6573 7461 6d70 223a 207b 2265 706f  imestamp": {"epo
+00001bd0: 6368 5365 636f 6e64 223a 2031 3637 3239  chSecond": 16729
+00001be0: 3237 3032 352c 2022 6e61 6e6f 223a 2035  27025, "nano": 5
+00001bf0: 3633 3634 3030 3030 7d2c 0a20 2020 2020  63640000},.     
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001c10: 7374 6172 7454 696d 6573 7461 6d70 223a  startTimestamp":
+00001c20: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
+00001c30: 2031 3637 3239 3237 3032 352c 2022 6e61   1672927025, "na
+00001c40: 6e6f 223a 2035 3633 3532 3230 3030 7d2c  no": 563522000},
+00001c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c60: 2020 2020 2022 7061 7265 6e74 4576 656e       "parentEven
+00001c70: 7449 6422 3a20 2264 656d 6f5f 626f 6f6b  tId": "demo_book
+00001c80: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+00001c90: 3330 3130 3531 3335 3730 3535 3630 3837  3010513570556087
+00001ca0: 3330 3030 3a64 3631 6539 3330 612d 3864  3000:d61e930a-8d
+00001cb0: 3030 2d31 3165 642d 6161 3161 2d64 3334  00-11ed-aa1a-d34
+00001cc0: 6136 3135 3531 3532 645f 3122 2c0a 2020  a6155152d_1",.  
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 2273 7563 6365 7373 6675 6c22 3a20    "successful": 
+00001cf0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00001d00: 2020 2020 2020 2020 2020 2262 6f6f 6b49            "bookI
+00001d10: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
+00001d20: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001d30: 2020 2020 2020 2022 7363 6f70 6522 3a20         "scope": 
+00001d40: 2274 6832 2d73 636f 7065 222c 0a20 2020  "th2-scope",.   
+00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d60: 2022 6174 7461 6368 6564 4d65 7373 6167   "attachedMessag
+00001d70: 6549 6473 223a 205b 5d2c 0a20 2020 2020  eIds": [],.     
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001d90: 626f 6479 223a 207b 2274 7970 6522 3a20  body": {"type": 
+00001da0: 226d 6573 7361 6765 222c 2022 6461 7461  "message", "data
+00001db0: 223a 2022 6473 2d6c 6962 2074 6573 7420  ": "ds-lib test 
+00001dc0: 626f 6479 227d 2c0a 2020 2020 2020 2020  body"},.        
+00001dd0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001de0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e00: 2022 6576 656e 7449 6422 3a20 2264 656d   "eventId": "dem
+00001e10: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
+00001e20: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
+00001e30: 3535 3633 3532 3230 3030 3a39 6164 6262  5563522000:9adbb
+00001e40: 3365 302d 3566 3862 2d34 6332 382d 6132  3e0-5f8b-4c28-a2
+00001e50: 6163 2d37 3336 3165 3866 6137 3034 633e  ac-7361e8fa704c>
+00001e60: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
+00001e70: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
+00001e80: 3537 3035 3536 3337 3537 3030 303a 6436  5705563757000:d6
+00001e90: 3165 3933 3061 2d38 6430 302d 3131 6564  1e930a-8d00-11ed
+00001ea0: 2d61 6131 612d 6433 3461 3631 3535 3135  -aa1a-d34a615515
+00001eb0: 3264 5f33 222c 0a20 2020 2020 2020 2020  2d_3",.         
+00001ec0: 2020 2020 2020 2020 2020 2022 6261 7463             "batc
+00001ed0: 6849 6422 3a20 2264 656d 6f5f 626f 6f6b  hId": "demo_book
+00001ee0: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+00001ef0: 3330 3130 3531 3335 3730 3535 3633 3532  3010513570556352
+00001f00: 3230 3030 3a39 6164 6262 3365 302d 3566  2000:9adbb3e0-5f
+00001f10: 3862 2d34 6332 382d 6132 6163 2d37 3336  8b-4c28-a2ac-736
+00001f20: 3165 3866 6137 3034 6322 2c0a 2020 2020  1e8fa704c",.    
+00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f40: 2269 7342 6174 6368 6564 223a 2054 7275  "isBatched": Tru
+00001f50: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00001f60: 2020 2020 2020 2022 6576 656e 744e 616d         "eventNam
+00001f70: 6522 3a20 2250 6c61 696e 2065 7665 6e74  e": "Plain event
+00001f80: 2032 222c 0a20 2020 2020 2020 2020 2020   2",.           
+00001f90: 2020 2020 2020 2020 2022 6576 656e 7454           "eventT
+00001fa0: 7970 6522 3a20 2264 732d 6c69 622d 7465  ype": "ds-lib-te
+00001fb0: 7374 2d65 7665 6e74 222c 0a20 2020 2020  st-event",.     
+00001fc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001fd0: 656e 6454 696d 6573 7461 6d70 223a 207b  endTimestamp": {
+00001fe0: 2265 706f 6368 5365 636f 6e64 223a 2031  "epochSecond": 1
+00001ff0: 3637 3239 3237 3032 352c 2022 6e61 6e6f  672927025, "nano
+00002000: 223a 2035 3633 3739 3130 3030 7d2c 0a20  ": 563791000},. 
+00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002020: 2020 2022 7374 6172 7454 696d 6573 7461     "startTimesta
+00002030: 6d70 223a 207b 2265 706f 6368 5365 636f  mp": {"epochSeco
+00002040: 6e64 223a 2031 3637 3239 3237 3032 352c  nd": 1672927025,
+00002050: 2022 6e61 6e6f 223a 2035 3633 3735 3730   "nano": 5637570
+00002060: 3030 7d2c 0a20 2020 2020 2020 2020 2020  00},.           
+00002070: 2020 2020 2020 2020 2022 7061 7265 6e74           "parent
+00002080: 4576 656e 7449 6422 3a20 2264 656d 6f5f  EventId": "demo_
+00002090: 626f 6f6b 5f31 3a74 6832 2d73 636f 7065  book_1:th2-scope
+000020a0: 3a32 3032 3330 3130 3531 3335 3730 3535  :202301051357055
+000020b0: 3630 3837 3330 3030 3a64 3631 6539 3330  60873000:d61e930
+000020c0: 612d 3864 3030 2d31 3165 642d 6161 3161  a-8d00-11ed-aa1a
+000020d0: 2d64 3334 6136 3135 3531 3532 645f 3122  -d34a6155152d_1"
+000020e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000020f0: 2020 2020 2020 2273 7563 6365 7373 6675        "successfu
+00002100: 6c22 3a20 5472 7565 2c0a 2020 2020 2020  l": True,.      
+00002110: 2020 2020 2020 2020 2020 2020 2020 2262                "b
+00002120: 6f6f 6b49 6422 3a20 2264 656d 6f5f 626f  ookId": "demo_bo
+00002130: 6f6b 5f31 222c 0a20 2020 2020 2020 2020  ok_1",.         
+00002140: 2020 2020 2020 2020 2020 2022 7363 6f70             "scop
+00002150: 6522 3a20 2274 6832 2d73 636f 7065 222c  e": "th2-scope",
+00002160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002170: 2020 2020 2022 6174 7461 6368 6564 4d65       "attachedMe
+00002180: 7373 6167 6549 6473 223a 205b 5d2c 0a20  ssageIds": [],. 
+00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021a0: 2020 2022 626f 6479 223a 207b 2274 7970     "body": {"typ
+000021b0: 6522 3a20 226d 6573 7361 6765 222c 2022  e": "message", "
+000021c0: 6461 7461 223a 2022 6473 2d6c 6962 2074  data": "ds-lib t
+000021d0: 6573 7420 626f 6479 227d 2c0a 2020 2020  est body"},.    
+000021e0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000021f0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00002200: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
+00002210: 2020 2020 2020 2020 2320 5b31 5d20 576f          # [1] Wo
+00002220: 726b 696e 6720 7769 7468 2061 2044 6174  rking with a Dat
+00002230: 6120 6f62 6a65 6374 2e0a 2020 2020 2020  a object..      
+00002240: 2020 2320 5b31 2e31 5d20 4669 6c74 6572    # [1.1] Filter
+00002250: 2e0a 2020 2020 2020 2020 6669 6c74 6572  ..        filter
+00002260: 6564 5f65 7665 6e74 733a 2044 6174 6120  ed_events: Data 
+00002270: 3d20 6576 656e 7473 2e66 696c 7465 7228  = events.filter(
+00002280: 6c61 6d62 6461 2065 3a20 655b 2262 6f64  lambda e: e["bod
+00002290: 7922 5d20 213d 205b 5d29 2020 2320 4669  y"] != [])  # Fi
+000022a0: 6c74 6572 2065 7665 6e74 7320 7769 7468  lter events with
+000022b0: 2065 6d70 7479 2062 6f64 792e 0a20 2020   empty body..   
+000022c0: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
+000022d0: 2020 2020 2020 2023 205b 312e 325d 204d         # [1.2] M
+000022e0: 6170 2e0a 2020 2020 2020 2020 6465 6620  ap..        def 
+000022f0: 7472 616e 7366 6f72 6d5f 6675 6e63 7469  transform_functi
+00002300: 6f6e 2872 6563 6f72 6429 3a0a 2020 2020  on(record):.    
+00002310: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+00002320: 2265 7665 6e74 4e61 6d65 223a 2072 6563  "eventName": rec
+00002330: 6f72 645b 2265 7665 6e74 4e61 6d65 225d  ord["eventName"]
+00002340: 2c20 2273 7563 6365 7373 6675 6c22 3a20  , "successful": 
+00002350: 7265 636f 7264 5b22 7375 6363 6573 7366  record["successf
+00002360: 756c 225d 7d0a 2020 2020 2020 2020 0a20  ul"]}.        . 
+00002370: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002380: 6669 6c74 6572 6564 5f61 6e64 5f6d 6170  filtered_and_map
+00002390: 7065 645f 6576 656e 7473 203d 2066 696c  ped_events = fil
+000023a0: 7465 7265 645f 6576 656e 7473 2e6d 6170  tered_events.map
+000023b0: 2874 7261 6e73 666f 726d 5f66 756e 6374  (transform_funct
+000023c0: 696f 6e29 0a20 2020 2020 2020 200a 2020  ion).        .  
+000023d0: 2020 2020 2020 2320 5b31 2e33 5d20 4461        # [1.3] Da
+000023e0: 7461 2070 6970 656c 696e 652e 0a20 2020  ta pipeline..   
+000023f0: 2020 2020 2023 2020 2020 2020 2049 6e73       #       Ins
+00002400: 7465 6164 206f 6620 646f 696e 6720 6461  tead of doing da
+00002410: 7461 2074 7261 6e73 666f 726d 6174 696f  ta transformatio
+00002420: 6e73 2073 7465 7020 6279 2073 7465 7020  ns step by step 
+00002430: 796f 7520 6361 6e20 646f 2069 7420 696e  you can do it in
+00002440: 206f 6e65 206c 696e 652e 0a20 2020 2020   one line..     
+00002450: 2020 2066 696c 7465 7265 645f 616e 645f     filtered_and_
+00002460: 6d61 7070 6564 5f65 7665 6e74 735f 6279  mapped_events_by
+00002470: 5f70 6970 656c 696e 6520 3d20 6576 656e  _pipeline = even
+00002480: 7473 2e66 696c 7465 7228 6c61 6d62 6461  ts.filter(lambda
+00002490: 2065 3a20 655b 2262 6f64 7922 5d20 213d   e: e["body"] !=
+000024a0: 205b 5d29 2e6d 6170 2874 7261 6e73 666f   []).map(transfo
+000024b0: 726d 5f66 756e 6374 696f 6e29 0a20 2020  rm_function).   
+000024c0: 2020 2020 2023 2043 6f6e 7465 6e74 206f       # Content o
+000024d0: 6620 7468 6573 6520 7477 6f20 4461 7461  f these two Data
+000024e0: 206f 626a 6563 7473 2073 686f 756c 6420   objects should 
+000024f0: 6265 2065 7175 616c 2e0a 2020 2020 2020  be equal..      
+00002500: 2020 6173 7365 7274 206c 6973 7428 6669    assert list(fi
+00002510: 6c74 6572 6564 5f61 6e64 5f6d 6170 7065  ltered_and_mappe
+00002520: 645f 6576 656e 7473 2920 3d3d 206c 6973  d_events) == lis
+00002530: 7428 6669 6c74 6572 6564 5f61 6e64 5f6d  t(filtered_and_m
+00002540: 6170 7065 645f 6576 656e 7473 5f62 795f  apped_events_by_
+00002550: 7069 7065 6c69 6e65 290a 2020 2020 2020  pipeline).      
+00002560: 2020 0a20 2020 2020 2020 2023 205b 312e    .        # [1.
+00002570: 345d 2053 6966 742e 2053 6b69 7020 7468  4] Sift. Skip th
+00002580: 6520 6669 7273 7420 6665 7720 6974 656d  e first few item
+00002590: 7320 6f72 206c 696d 6974 2074 6865 6d2e  s or limit them.
+000025a0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+000025b0: 4461 7461 285b 312c 2032 2c20 332c 2034  Data([1, 2, 3, 4
+000025c0: 2c20 352c 2036 2c20 372c 2038 2c20 392c  , 5, 6, 7, 8, 9,
+000025d0: 2031 302c 2031 312c 2031 322c 2031 332c   10, 11, 12, 13,
+000025e0: 2031 342c 2031 355d 290a 2020 2020 2020   14, 15]).      
+000025f0: 2020 6974 656d 735f 6672 6f6d 5f31 315f    items_from_11_
+00002600: 746f 5f65 6e64 3a20 4765 6e65 7261 746f  to_end: Generato
+00002610: 7220 3d20 6461 7461 2e73 6966 7428 736b  r = data.sift(sk
+00002620: 6970 3d31 3029 0a20 2020 2020 2020 206f  ip=10).        o
+00002630: 6e6c 795f 6669 7273 745f 3130 5f69 7465  nly_first_10_ite
+00002640: 6d73 3a20 4765 6e65 7261 746f 7220 3d20  ms: Generator = 
+00002650: 6461 7461 2e73 6966 7428 6c69 6d69 743d  data.sift(limit=
+00002660: 3130 290a 2020 2020 2020 2020 0a20 2020  10).        .   
+00002670: 2020 2020 2023 205b 312e 355d 2043 6861       # [1.5] Cha
+00002680: 6e67 696e 6720 6361 6368 6520 7374 6174  nging cache stat
+00002690: 7573 2e0a 2020 2020 2020 2020 6576 656e  us..        even
+000026a0: 7473 2e75 7365 5f63 6163 6865 2854 7275  ts.use_cache(Tru
+000026b0: 6529 0a20 2020 2020 2020 2023 206f 7220  e).        # or 
+000026c0: 6a75 7374 0a20 2020 2020 2020 2065 7665  just.        eve
+000026d0: 6e74 732e 7573 655f 6361 6368 6528 2920  nts.use_cache() 
+000026e0: 2023 2049 6620 796f 7520 7761 6e74 2074   # If you want t
+000026f0: 6f20 6163 7469 7661 7465 2063 6163 6865  o activate cache
+00002700: 2e0a 2020 2020 2020 2020 2320 5b31 2e36  ..        # [1.6
+00002710: 5d20 5761 6c6b 2074 6872 6f75 6768 2064  ] Walk through d
+00002720: 6174 612e 0a20 2020 2020 2020 2066 6f72  ata..        for
+00002730: 2065 7665 6e74 2069 6e20 6576 656e 7473   event in events
+00002740: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00002750: 446f 2073 6f6d 6574 6869 6e67 2077 6974  Do something wit
+00002760: 6820 6576 656e 7420 2865 7665 6e74 2069  h event (event i
+00002770: 7320 6120 6469 6374 292e 0a20 2020 2020  s a dict)..     
+00002780: 2020 2020 2020 2070 7269 6e74 2865 7665         print(eve
+00002790: 6e74 290a 2020 2020 2020 2020 2320 4166  nt).        # Af
+000027a0: 7465 7220 6669 7273 7420 6974 6572 6174  ter first iterat
+000027b0: 696f 6e20 7468 6520 6576 656e 7473 2068  ion the events h
+000027c0: 6173 2061 2063 6163 6865 2066 696c 652e  as a cache file.
+000027d0: 0a20 2020 2020 2020 2023 204e 6f77 2074  .        # Now t
+000027e0: 6865 7920 7769 6c6c 2062 6520 7573 6564  hey will be used
+000027f0: 2069 6e20 7468 6520 6361 6368 6520 696e   in the cache in
+00002800: 2074 6865 206e 6578 7420 6974 6572 6174   the next iterat
+00002810: 696f 6e2e 0a20 2020 2020 2020 200a 2020  ion..        .  
+00002820: 2020 2020 2020 2320 5b31 2e37 5d20 4765        # [1.7] Ge
+00002830: 7420 6e75 6d62 6572 206f 6620 7468 6520  t number of the 
+00002840: 656c 656d 656e 7473 2069 6e20 7468 6520  elements in the 
+00002850: 4461 7461 206f 626a 6563 742e 0a20 2020  Data object..   
+00002860: 2020 2020 206e 756d 6265 725f 6f66 5f65       number_of_e
+00002870: 7665 6e74 7320 3d20 6576 656e 7473 2e6c  vents = events.l
+00002880: 656e 0a20 2020 2020 2020 200a 2020 2020  en.        .    
+00002890: 2020 2020 2320 5b31 2e38 5d20 4368 6563      # [1.8] Chec
+000028a0: 6b20 7468 6174 2044 6174 6120 6f62 6a65  k that Data obje
+000028b0: 6374 2069 736e 2774 2065 6d70 7479 2e0a  ct isn't empty..
+000028c0: 2020 2020 2020 2020 2320 5468 6520 6461          # The da
+000028d0: 7461 2073 6f75 7263 6520 7368 6f75 6c64  ta source should
+000028e0: 2062 6520 6e6f 7420 656d 7074 792e 0a20   be not empty.. 
+000028f0: 2020 2020 2020 2061 7373 6572 7420 6576         assert ev
+00002900: 656e 7473 2e69 735f 656d 7074 7920 6973  ents.is_empty is
+00002910: 2046 616c 7365 0a20 2020 2020 2020 200a   False.        .
+00002920: 2020 2020 2020 2020 2320 5b31 2e39 5d20          # [1.9] 
+00002930: 436f 6e76 6572 7420 4461 7461 206f 626a  Convert Data obj
+00002940: 6563 7420 746f 2074 6865 206c 6973 7420  ect to the list 
+00002950: 6f66 2065 6c65 6d65 6e74 7328 6576 656e  of elements(even
+00002960: 7473 206f 7220 6d65 7373 6167 6573 292e  ts or messages).
+00002970: 0a20 2020 2020 2020 2023 2042 6520 6361  .        # Be ca
+00002980: 7265 6675 6c2c 2074 6869 7320 6361 6e20  reful, this can 
+00002990: 7461 6b65 2074 6f6f 206d 7563 6820 6d65  take too much me
+000029a0: 6d6f 7279 2e0a 2020 2020 2020 2020 6576  mory..        ev
+000029b0: 656e 7473 5f6c 6973 7420 3d20 6c69 7374  ents_list = list
+000029c0: 2865 7665 6e74 7329 0a20 2020 2020 2020  (events).       
+000029d0: 200a 2020 2020 2020 2020 2320 5b31 2e31   .        # [1.1
+000029e0: 305d 2054 6865 2063 6163 6865 2069 6e68  0] The cache inh
+000029f0: 6572 6974 616e 6365 2e0a 2020 2020 2020  eritance..      
+00002a00: 2020 2320 4372 6561 7465 7320 6120 6e65    # Creates a ne
+00002a10: 7720 4461 7461 206f 626a 6563 7420 7468  w Data object th
+00002a20: 6174 2077 696c 6c20 7573 6520 6361 6368  at will use cach
+00002a30: 6520 6672 6f6d 2074 6865 2065 7665 6e74  e from the event
+00002a40: 7320 4461 7461 206f 626a 6563 742e 0a20  s Data object.. 
+00002a50: 2020 2020 2020 2065 7665 6e74 735f 6669         events_fi
+00002a60: 6c74 6572 6564 3a20 4461 7461 203d 2065  ltered: Data = e
+00002a70: 7665 6e74 732e 6669 6c74 6572 286c 616d  vents.filter(lam
+00002a80: 6264 6120 7265 636f 7264 3a20 7265 636f  bda record: reco
+00002a90: 7264 2e67 6574 2822 6261 7463 6849 6422  rd.get("batchId"
+00002aa0: 2929 0a20 2020 2020 2020 200a 2020 2020  )).        .    
+00002ab0: 2020 2020 2320 4e65 7720 4461 7461 206f      # New Data o
+00002ac0: 626a 6563 7473 2064 6f6e 2774 2075 7365  bjects don't use
+00002ad0: 2074 6865 6972 206f 776e 2063 6163 6865   their own cache
+00002ae0: 2062 7920 6465 6661 756c 7420 6275 7420   by default but 
+00002af0: 7573 6520 7468 6520 6361 6368 6520 6f66  use the cache of
+00002b00: 2074 6865 2070 6172 656e 7420 4461 7461   the parent Data
+00002b10: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
+00002b20: 2023 2055 7365 2075 7365 5f63 6163 6865   # Use use_cache
+00002b30: 206d 6574 686f 6420 746f 2061 6374 6976   method to activ
+00002b40: 6174 6520 6361 6368 696e 672e 0a20 2020  ate caching..   
+00002b50: 2020 2020 2023 2041 6674 6572 2074 6861       # After tha
+00002b60: 742c 2074 6865 2044 6174 6120 6f62 6a65  t, the Data obje
+00002b70: 6374 2077 696c 6c20 6372 6561 7465 2069  ct will create i
+00002b80: 7473 206f 776e 2063 6163 6865 2066 696c  ts own cache fil
+00002b90: 652e 0a20 2020 2020 2020 2065 7665 6e74  e..        event
+00002ba0: 735f 6669 6c74 6572 6564 2e75 7365 5f63  s_filtered.use_c
+00002bb0: 6163 6865 2829 0a20 2020 2020 2020 200a  ache().        .
+00002bc0: 2020 2020 2020 2020 6c69 7374 2865 7665          list(eve
+00002bd0: 6e74 735f 6669 6c74 6572 6564 2920 2023  nts_filtered)  #
+00002be0: 204a 7573 7420 746f 2069 7465 7261 7465   Just to iterate
+00002bf0: 2044 6174 6120 6f62 6a65 6374 2028 6361   Data object (ca
+00002c00: 6368 6520 6669 6c65 2077 696c 6c20 6265  che file will be
+00002c10: 2063 7265 6174 6564 292e 0a20 2020 2020   created)..     
+00002c20: 2020 200a 2020 2020 2020 2020 6669 6c74     .        filt
+00002c30: 6572 6564 5f65 7665 6e74 735f 7479 7065  ered_events_type
+00002c40: 7320 3d20 6576 656e 7473 5f66 696c 7465  s = events_filte
+00002c50: 7265 642e 6d61 7028 6c61 6d62 6461 2072  red.map(lambda r
+00002c60: 6563 6f72 643a 207b 2265 7665 6e74 5479  ecord: {"eventTy
+00002c70: 7065 223a 2072 6563 6f72 642e 6765 7428  pe": record.get(
+00002c80: 2265 7665 6e74 5479 7065 2229 7d29 0a20  "eventType")}). 
+00002c90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002ca0: 6576 656e 7473 5f77 6974 686f 7574 5f74  events_without_t
+00002cb0: 7970 6573 5f77 6974 685f 6261 7463 6820  ypes_with_batch 
+00002cc0: 3d20 6669 6c74 6572 6564 5f65 7665 6e74  = filtered_event
+00002cd0: 735f 7479 7065 732e 6669 6c74 6572 286c  s_types.filter(l
+00002ce0: 616d 6264 6120 7265 636f 7264 3a20 6e6f  ambda record: no
+00002cf0: 7420 7265 636f 7264 2e67 6574 2822 6576  t record.get("ev
+00002d00: 656e 7454 7970 6522 2929 0a20 2020 2020  entType")).     
+00002d10: 2020 2065 7665 6e74 735f 7769 7468 6f75     events_withou
+00002d20: 745f 7479 7065 735f 7769 7468 5f62 6174  t_types_with_bat
+00002d30: 6368 2e75 7365 5f63 6163 6865 2829 0a20  ch.use_cache(). 
+00002d40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002d50: 2320 5b31 2e31 315d 2044 6174 6120 6f62  # [1.11] Data ob
+00002d60: 6a65 6374 7320 6a6f 696e 696e 672e 0a20  jects joining.. 
+00002d70: 2020 2020 2020 2023 2059 6f75 2068 6176         # You hav
+00002d80: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00002d90: 3320 4461 7461 206f 626a 6563 7473 2e0a  3 Data objects..
+00002da0: 2020 2020 2020 2020 6431 203d 2044 6174          d1 = Dat
+00002db0: 6128 5b31 2c20 322c 2033 5d29 0a20 2020  a([1, 2, 3]).   
+00002dc0: 2020 2020 2064 3220 3d20 4461 7461 285b       d2 = Data([
+00002dd0: 2261 222c 207b 2269 6422 3a20 3132 337d  "a", {"id": 123}
+00002de0: 2c20 2263 225d 290a 2020 2020 2020 2020  , "c"]).        
+00002df0: 6433 203d 2044 6174 6128 5b37 2c20 382c  d3 = Data([7, 8,
+00002e00: 2039 5d29 0a20 2020 2020 2020 2023 2059   9]).        # Y
+00002e10: 6f75 2063 616e 206a 6f69 6e20 4461 7461  ou can join Data
+00002e20: 206f 626a 6563 7473 2069 6e20 666f 6c6c   objects in foll
+00002e30: 6f77 696e 6720 7761 7973 2e0a 2020 2020  owing ways..    
+00002e40: 2020 2020 2320 506c 6561 7365 206e 6f74      # Please not
+00002e50: 652c 206e 6577 2044 6174 6120 6f62 6a65  e, new Data obje
+00002e60: 6374 2077 696c 6c20 6861 7665 2063 6163  ct will have cac
+00002e70: 6865 2073 7461 7475 7320 3d3d 2046 616c  he status == Fal
+00002e80: 7365 2e0a 2020 2020 2020 2020 6461 7461  se..        data
+00002e90: 5f76 6961 5f69 6e69 7420 3d20 4461 7461  _via_init = Data
+00002ea0: 285b 6431 2c20 6432 2c20 6433 5d29 0a20  ([d1, d2, d3]). 
+00002eb0: 2020 2020 2020 2064 6174 615f 7669 615f         data_via_
+00002ec0: 6164 6420 3d20 6431 202b 2064 3220 2b20  add = d1 + d2 + 
+00002ed0: 6433 0a20 2020 2020 2020 2064 6174 615f  d3.        data_
+00002ee0: 7769 7468 5f6e 6f6e 5f64 6174 615f 6f62  with_non_data_ob
+00002ef0: 6a5f 7669 615f 696e 6974 203d 2044 6174  j_via_init = Dat
+00002f00: 6128 5b64 312c 205b 2261 222c 207b 2269  a([d1, ["a", {"i
+00002f10: 6422 3a20 3132 337d 2c20 2263 225d 2c20  d": 123}, "c"], 
+00002f20: 6433 5d29 0a20 2020 2020 2020 2064 6174  d3]).        dat
+00002f30: 615f 7769 7468 5f6e 6f6e 5f64 6174 615f  a_with_non_data_
+00002f40: 6f62 6a5f 7669 615f 6164 6420 3d20 6431  obj_via_add = d1
+00002f50: 202b 205b 2261 222c 207b 2269 6422 3a20   + ["a", {"id": 
+00002f60: 3132 337d 2c20 2263 225d 202b 2064 330a  123}, "c"] + d3.
+00002f70: 2020 2020 2020 2020 2320 596f 7520 6361          # You ca
+00002f80: 6e20 6a6f 696e 2063 7572 7265 6e74 2044  n join current D
+00002f90: 6174 6120 6f62 6a65 6374 206f 6e20 706c  ata object on pl
+00002fa0: 6163 6520 7573 696e 6720 2b3d 2e0a 2020  ace using +=..  
+00002fb0: 2020 2020 2020 2320 4974 2077 696c 6c20        # It will 
+00002fc0: 6b65 6570 2063 6163 6865 2073 7461 7475  keep cache statu
+00002fd0: 732e 0a20 2020 2020 2020 2064 3120 2b3d  s..        d1 +=
+00002fe0: 2064 3320 2023 2064 3120 7769 6c6c 2062   d3  # d1 will b
+00002ff0: 6563 6f6d 6520 4461 7461 285b 312c 322c  ecome Data([1,2,
+00003000: 332c 372c 382c 395d 290a 2020 2020 2020  3,7,8,9]).      
+00003010: 2020 0a20 2020 2020 2020 2023 205b 312e    .        # [1.
+00003020: 3132 5d20 4275 696c 6420 616e 6420 7265  12] Build and re
+00003030: 6164 2044 6174 6120 6f62 6a65 6374 2063  ad Data object c
+00003040: 6163 6865 2066 696c 6573 2e0a 2020 2020  ache files..    
+00003050: 2020 2020 6576 656e 7473 2e62 7569 6c64      events.build
+00003060: 5f63 6163 6865 2822 6361 6368 655f 6669  _cache("cache_fi
+00003070: 6c65 6e61 6d65 5f6f 725f 7061 7468 2229  lename_or_path")
+00003080: 0a20 2020 2020 2020 2064 6174 615f 6f62  .        data_ob
+00003090: 6a5f 6672 6f6d 5f63 6163 6865 203d 2044  j_from_cache = D
+000030a0: 6174 612e 6672 6f6d 5f63 6163 6865 5f66  ata.from_cache_f
+000030b0: 696c 6528 2263 6163 6865 5f66 696c 656e  ile("cache_filen
+000030c0: 616d 655f 6f72 5f70 6174 6822 290a 2020  ame_or_path").  
+000030d0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+000030e0: 205b 325d 2057 6f72 6b69 6e67 2077 6974   [2] Working wit
+000030f0: 6820 636f 6e76 6572 7465 7273 2e0a 2020  h converters..  
+00003100: 2020 2020 2020 2320 5468 6572 6520 6172        # There ar
+00003110: 6520 6375 7272 656e 746c 7920 7468 7265  e currently thre
+00003120: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+00003130: 7320 6f66 2049 5469 6d65 7374 616d 7043  s of ITimestampC
+00003140: 6f6e 7665 7274 6572 2063 6c61 7373 3a20  onverter class: 
+00003150: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
+00003160: 2c20 4461 7465 7469 6d65 5374 7269 6e67  , DatetimeString
+00003170: 436f 6e76 6572 7465 7220 616e 6420 5072  Converter and Pr
+00003180: 6f74 6f62 7566 5469 6d65 7374 616d 7043  otobufTimestampC
+00003190: 6f6e 7665 7274 6572 2e0a 2020 2020 2020  onverter..      
+000031a0: 2020 2320 5468 6579 2061 6c6c 2069 6d70    # They all imp
+000031b0: 6c65 6d65 6e74 2073 616d 6520 6d65 7468  lement same meth
+000031c0: 6f64 7320 6672 6f6d 2062 6173 6520 636c  ods from base cl
+000031d0: 6173 732e 0a20 2020 2020 2020 2023 204e  ass..        # N
+000031e0: 6f74 6520 7468 6174 2073 6f6d 6520 6163  ote that some ac
+000031f0: 6375 7261 6379 206d 6179 2062 6520 6c6f  curacy may be lo
+00003200: 7374 2064 7572 696e 6720 636f 6e76 6572  st during conver
+00003210: 7369 6f6e 2e0a 2020 2020 2020 2020 2320  sion..        # 
+00003220: 4966 2066 6f72 2065 7861 6d70 6c65 2079  If for example y
+00003230: 6f75 2075 7365 2074 6f5f 6d69 6372 6f73  ou use to_micros
+00003240: 6563 6f6e 6473 206e 616e 6f73 6563 6f6e  econds nanosecon
+00003250: 6473 2077 696c 6c20 6265 2063 7574 206f  ds will be cut o
+00003260: 6666 2069 6e73 7465 6164 206f 6620 726f  ff instead of ro
+00003270: 756e 6469 6e67 2e0a 2020 2020 2020 2020  unding..        
+00003280: 0a20 2020 2020 2020 2023 205b 322e 315d  .        # [2.1]
+00003290: 2044 6174 6574 696d 6543 6f6e 7665 7274   DatetimeConvert
+000032a0: 6572 2e0a 2020 2020 2020 2020 2320 4461  er..        # Da
+000032b0: 7465 7469 6d65 436f 6e76 6572 7465 7220  tetimeConverter 
+000032c0: 7461 6b65 7320 6461 7465 7469 6d65 2e64  takes datetime.d
+000032d0: 6174 6574 696d 6520 6f62 6a65 6374 2061  atetime object a
+000032e0: 7320 696e 7075 742e 0a20 2020 2020 2020  s input..       
+000032f0: 200a 2020 2020 2020 2020 6461 7465 7469   .        dateti
+00003300: 6d65 5f6f 626a 203d 2064 6174 6574 696d  me_obj = datetim
+00003310: 6528 7965 6172 3d32 3032 332c 206d 6f6e  e(year=2023, mon
+00003320: 7468 3d31 2c20 6461 793d 352c 2068 6f75  th=1, day=5, hou
+00003330: 723d 3134 2c20 6d69 6e75 7465 3d33 382c  r=14, minute=38,
+00003340: 2073 6563 6f6e 643d 3235 2c20 6d69 6372   second=25, micr
+00003350: 6f73 6563 6f6e 643d 3134 3630 290a 2020  osecond=1460).  
+00003360: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00003370: 2049 7420 6861 7320 6d65 7468 6f64 7320   It has methods 
+00003380: 7468 6174 2072 6574 7572 6e20 7468 6520  that return the 
+00003390: 6461 7465 7469 6d65 2069 6e20 6469 6666  datetime in diff
+000033a0: 6572 656e 7420 666f 726d 6173 3a0a 2020  erent formas:.  
+000033b0: 2020 2020 2020 0a20 2020 2020 2020 2064        .        d
+000033c0: 6174 655f 6d73 203d 2044 6174 6574 696d  ate_ms = Datetim
+000033d0: 6543 6f6e 7665 7274 6572 2e74 6f5f 6d69  eConverter.to_mi
+000033e0: 6c6c 6973 6563 6f6e 6473 2864 6174 6574  lliseconds(datet
+000033f0: 696d 655f 6f62 6a29 0a20 2020 2020 2020  ime_obj).       
+00003400: 2064 6174 655f 7573 203d 2044 6174 6574   date_us = Datet
+00003410: 696d 6543 6f6e 7665 7274 6572 2e74 6f5f  imeConverter.to_
+00003420: 6d69 6372 6f73 6563 6f6e 6473 2864 6174  microseconds(dat
+00003430: 6574 696d 655f 6f62 6a29 0a20 2020 2020  etime_obj).     
+00003440: 2020 2023 2043 6f6e 7665 7274 696e 6720     # Converting 
+00003450: 746f 206e 616e 6f73 6563 6f6e 6473 206a  to nanoseconds j
+00003460: 7573 7473 2061 6464 7320 7468 7265 6520  usts adds three 
+00003470: 7472 6169 6c69 6e67 207a 6572 6f73 2061  trailing zeros a
+00003480: 7320 6461 7465 7469 6d65 206f 626a 6563  s datetime objec
+00003490: 7420 646f 6573 6e27 7420 6861 7665 206e  t doesn't have n
+000034a0: 616e 6f73 6563 6f6e 6473 2e0a 2020 2020  anoseconds..    
+000034b0: 2020 2020 6461 7465 5f6e 7320 3d20 4461      date_ns = Da
+000034c0: 7465 7469 6d65 436f 6e76 6572 7465 722e  tetimeConverter.
+000034d0: 746f 5f6e 616e 6f73 6563 6f6e 6473 2864  to_nanoseconds(d
+000034e0: 6174 6574 696d 655f 6f62 6a29 0a20 2020  atetime_obj).   
+000034f0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00003500: 5b32 2e32 5d20 4461 7465 7469 6d65 5374  [2.2] DatetimeSt
+00003510: 7269 6e67 436f 6e76 6572 7465 720a 2020  ringConverter.  
+00003520: 2020 2020 2020 2320 4461 7465 7469 6d65        # Datetime
+00003530: 5374 7269 6e67 436f 6e76 6572 7465 7220  StringConverter 
+00003540: 7461 6b65 7320 7374 7269 6e67 2069 6e20  takes string in 
+00003550: 2279 7979 792d 4d4d 2d64 6454 4848 3a6d  "yyyy-MM-ddTHH:m
+00003560: 6d3a 7373 5b2e 5353 5353 5353 5353 535d  m:ss[.SSSSSSSSS]
+00003570: 5a22 2066 6f72 6d61 742e 0a20 2020 2020  Z" format..     
+00003580: 2020 200a 2020 2020 2020 2020 6461 7465     .        date
+00003590: 5f73 7472 696e 6720 3d20 2232 3032 332d  _string = "2023-
+000035a0: 3031 2d30 3554 3134 3a33 383a 3235 2e30  01-05T14:38:25.0
+000035b0: 3031 3436 5a22 0a20 2020 2020 2020 200a  0146Z".        .
+000035c0: 2020 2020 2020 2020 2320 5765 2068 6176          # We hav
+000035d0: 6520 7361 6d65 206d 6574 686f 6473 2061  e same methods a
+000035e0: 7320 696e 2044 6174 6574 696d 6543 6f6e  s in DatetimeCon
+000035f0: 7665 7274 6572 0a20 2020 2020 2020 2064  verter.        d
+00003600: 6174 655f 6d73 5f66 726f 6d5f 7374 7269  ate_ms_from_stri
+00003610: 6e67 203d 2044 6174 6574 696d 6553 7472  ng = DatetimeStr
+00003620: 696e 6743 6f6e 7665 7274 6572 2e74 6f5f  ingConverter.to_
+00003630: 6d69 6c6c 6973 6563 6f6e 6473 2864 6174  milliseconds(dat
+00003640: 655f 7374 7269 6e67 290a 2020 2020 2020  e_string).      
+00003650: 2020 6461 7465 5f75 735f 6672 6f6d 5f73    date_us_from_s
+00003660: 7472 696e 6720 3d20 4461 7465 7469 6d65  tring = Datetime
+00003670: 5374 7269 6e67 436f 6e76 6572 7465 722e  StringConverter.
+00003680: 746f 5f6d 6963 726f 7365 636f 6e64 7328  to_microseconds(
+00003690: 6461 7465 5f73 7472 696e 6729 0a20 2020  date_string).   
+000036a0: 2020 2020 2064 6174 655f 6e73 5f66 726f       date_ns_fro
+000036b0: 6d5f 7374 7269 6e67 203d 2044 6174 6574  m_string = Datet
+000036c0: 696d 6553 7472 696e 6743 6f6e 7665 7274  imeStringConvert
+000036d0: 6572 2e74 6f5f 6e61 6e6f 7365 636f 6e64  er.to_nanosecond
+000036e0: 7328 6461 7465 5f73 7472 696e 6729 0a20  s(date_string). 
+000036f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003700: 2320 5765 2063 616e 2061 6c73 6f20 6765  # We can also ge
+00003710: 7420 6461 7465 7469 6d65 206f 626a 6563  t datetime objec
+00003720: 7420 6672 6f6d 2073 7472 696e 670a 2020  t from string.  
+00003730: 2020 2020 2020 6461 7465 7469 6d65 5f66        datetime_f
+00003740: 726f 6d5f 7374 7269 6e67 203d 2044 6174  rom_string = Dat
+00003750: 6574 696d 6553 7472 696e 6743 6f6e 7665  etimeStringConve
+00003760: 7274 6572 2e74 6f5f 6461 7465 7469 6d65  rter.to_datetime
+00003770: 2864 6174 655f 7374 7269 6e67 290a 2020  (date_string).  
+00003780: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00003790: 205b 322e 335d 2050 726f 746f 6275 6654   [2.3] ProtobufT
+000037a0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
+000037b0: 720a 2020 2020 2020 2020 2320 5072 6f74  r.        # Prot
+000037c0: 6f62 7566 2074 696d 6573 7461 6d70 7320  obuf timestamps 
+000037d0: 6d75 7374 2062 6520 696e 2066 6f72 6d20  must be in form 
+000037e0: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
+000037f0: 7365 636f 6e64 732c 2022 6e61 6e6f 223a  seconds, "nano":
+00003800: 206e 616e 6f73 6563 6f6e 6473 7d0a 2020   nanoseconds}.  
+00003810: 2020 2020 2020 0a20 2020 2020 2020 2070        .        p
+00003820: 726f 746f 6275 665f 7469 6d65 7374 616d  rotobuf_timestam
+00003830: 7020 3d20 7b22 6570 6f63 6853 6563 6f6e  p = {"epochSecon
+00003840: 6422 3a20 3136 3732 3932 3935 3035 2c20  d": 1672929505, 
+00003850: 226e 616e 6f22 3a20 315f 3436 305f 3030  "nano": 1_460_00
+00003860: 307d 0a20 2020 2020 2020 200a 2020 2020  0}.        .    
+00003870: 2020 2020 6461 7465 5f6d 735f 6672 6f6d      date_ms_from
+00003880: 5f74 696d 6573 7461 6d70 203d 2050 726f  _timestamp = Pro
+00003890: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
+000038a0: 6e76 6572 7465 722e 746f 5f6d 696c 6c69  nverter.to_milli
+000038b0: 7365 636f 6e64 7328 7072 6f74 6f62 7566  seconds(protobuf
+000038c0: 5f74 696d 6573 7461 6d70 290a 2020 2020  _timestamp).    
+000038d0: 2020 2020 6461 7465 5f75 735f 6672 6f6d      date_us_from
+000038e0: 5f74 696d 6573 7461 6d70 203d 2050 726f  _timestamp = Pro
+000038f0: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
+00003900: 6e76 6572 7465 722e 746f 5f6d 6963 726f  nverter.to_micro
+00003910: 7365 636f 6e64 7328 7072 6f74 6f62 7566  seconds(protobuf
+00003920: 5f74 696d 6573 7461 6d70 290a 2020 2020  _timestamp).    
+00003930: 2020 2020 6461 7465 5f6e 735f 6672 6f6d      date_ns_from
+00003940: 5f74 696d 6573 7461 6d70 203d 2050 726f  _timestamp = Pro
+00003950: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
+00003960: 6e76 6572 7465 722e 746f 5f6e 616e 6f73  nverter.to_nanos
+00003970: 6563 6f6e 6473 2870 726f 746f 6275 665f  econds(protobuf_
+00003980: 7469 6d65 7374 616d 7029 0a20 2020 2020  timestamp).     
+00003990: 2020 2064 6174 6574 696d 655f 6672 6f6d     datetime_from
+000039a0: 5f74 696d 6573 7461 6d70 203d 2050 726f  _timestamp = Pro
+000039b0: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
+000039c0: 6e76 6572 7465 722e 746f 5f64 6174 6574  nverter.to_datet
+000039d0: 696d 6528 7072 6f74 6f62 7566 5f74 696d  ime(protobuf_tim
+000039e0: 6573 7461 6d70 290a 2020 2020 2020 2020  estamp).        
+000039f0: 0a20 2020 2020 2020 2023 205b 335d 2057  .        # [3] W
+00003a00: 6f72 6b69 6e67 2077 6974 6820 4576 656e  orking with Even
+00003a10: 7454 7265 6520 616e 6420 4576 656e 7454  tTree and EventT
+00003a20: 7265 6543 6f6c 6c65 6374 696f 6e2e 0a20  reeCollection.. 
+00003a30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003a40: 2320 5b33 2e31 5d20 4275 696c 6420 6120  # [3.1] Build a 
+00003a50: 6375 7374 6f6d 2045 7665 6e74 5472 6565  custom EventTree
+00003a60: 0a20 2020 2020 2020 2023 2054 6f20 6372  .        # To cr
+00003a70: 6561 7465 2061 6e20 4576 656e 7454 7265  eate an EventTre
+00003a80: 6520 6f62 6a65 6374 2079 6f75 206e 6565  e object you nee
+00003a90: 6420 746f 2070 726f 7669 6465 206e 616d  d to provide nam
+00003aa0: 652c 2069 6420 616e 6420 6461 7461 206f  e, id and data o
+00003ab0: 6620 7468 6520 726f 6f74 2065 7665 6e74  f the root event
+00003ac0: 2e0a 2020 2020 2020 2020 7472 6565 203d  ..        tree =
+00003ad0: 2045 7665 6e74 5472 6565 2865 7665 6e74   EventTree(event
+00003ae0: 5f6e 616d 653d 2272 6f6f 7420 6576 656e  _name="root even
+00003af0: 7422 2c20 6576 656e 745f 6964 3d22 726f  t", event_id="ro
+00003b00: 6f74 5f69 6422 2c20 6461 7461 3d7b 2264  ot_id", data={"d
+00003b10: 6174 6122 3a20 5b31 2c20 322c 2033 2c20  ata": [1, 2, 3, 
+00003b20: 342c 2035 5d7d 290a 2020 2020 2020 2020  4, 5]}).        
+00003b30: 0a20 2020 2020 2020 2023 2054 6f20 6164  .        # To ad
+00003b40: 6420 6e65 7720 6e6f 6465 2075 7365 2061  d new node use a
+00003b50: 7070 656e 645f 6576 656e 742e 2070 6172  ppend_event. par
+00003b60: 656e 745f 6964 2069 7320 6e65 6365 7373  ent_id is necess
+00003b70: 6172 792c 2064 6174 6120 6973 206f 7074  ary, data is opt
+00003b80: 696f 6e61 6c2e 0a20 2020 2020 2020 2074  ional..        t
+00003b90: 7265 652e 6170 7065 6e64 5f65 7665 6e74  ree.append_event
+00003ba0: 2865 7665 6e74 5f6e 616d 653d 2241 222c  (event_name="A",
+00003bb0: 2065 7665 6e74 5f69 643d 2241 5f69 6422   event_id="A_id"
+00003bc0: 2c20 6461 7461 3d4e 6f6e 652c 2070 6172  , data=None, par
+00003bd0: 656e 745f 6964 3d22 726f 6f74 5f69 6422  ent_id="root_id"
+00003be0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00003bf0: 2020 2023 205b 332e 335d 2042 7569 6c64     # [3.3] Build
+00003c00: 696e 6720 7468 6520 4576 656e 7454 7265  ing the EventTre
+00003c10: 6543 6f6c 6c65 6374 696f 6e2e 0a20 2020  eCollection..   
+00003c20: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00003c30: 4966 2079 6f75 2064 6f6e 2774 2073 7065  If you don't spe
+00003c40: 6369 6679 2064 6174 615f 736f 7572 6365  cify data_source
+00003c50: 2066 6f72 2074 6865 2064 7269 7665 7220   for the driver 
+00003c60: 7468 656e 2069 7420 776f 6e27 7420 7265  then it won't re
+00003c70: 636f 7665 7220 6465 7461 6368 6564 2065  cover detached e
+00003c80: 7665 6e74 732e 0a20 2020 2020 2020 2064  vents..        d
+00003c90: 7269 7665 723a 2049 4554 4344 7269 7665  river: IETCDrive
+00003ca0: 7220 2023 2059 6f75 2073 686f 756c 6420  r  # You should 
+00003cb0: 696e 6974 2045 5443 4472 6976 6572 206f  init ETCDriver o
+00003cc0: 626a 6563 742e 2045 2e67 2e20 6672 6f6d  bject. E.g. from
+00003cd0: 204c 7744 5020 6d6f 6475 6c65 206f 7220   LwDP module or 
+00003ce0: 796f 7572 2063 7573 746f 6d20 636c 6173  your custom clas
+00003cf0: 732e 0a20 2020 2020 2020 2065 7463 203d  s..        etc =
+00003d00: 2045 7665 6e74 5472 6565 436f 6c6c 6563   EventTreeCollec
+00003d10: 7469 6f6e 2864 7269 7665 7229 0a20 2020  tion(driver).   
+00003d20: 2020 2020 2065 7463 2e62 7569 6c64 2865       etc.build(e
+00003d30: 7665 6e74 7329 0a20 2020 2020 2020 200a  vents).        .
+00003d40: 2020 2020 2020 2020 2320 4465 7461 6368          # Detach
+00003d50: 6564 2065 7665 6e74 7320 6973 6e27 7420  ed events isn't 
+00003d60: 656d 7074 792e 0a20 2020 2020 2020 2061  empty..        a
+00003d70: 7373 6572 7420 6574 632e 6765 745f 6465  ssert etc.get_de
+00003d80: 7461 6368 6564 5f65 7665 6e74 7328 290a  tached_events().
+00003d90: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003da0: 2065 7463 203d 2045 7665 6e74 5472 6565   etc = EventTree
+00003db0: 436f 6c6c 6563 7469 6f6e 2864 7269 7665  Collection(drive
+00003dc0: 7229 0a20 2020 2020 2020 2023 2044 6574  r).        # Det
+00003dd0: 6163 6865 6420 6576 656e 7473 2061 7265  ached events are
+00003de0: 2065 6d70 7479 2062 6563 6175 7365 2074   empty because t
+00003df0: 6865 7920 7765 7265 2072 6563 6f76 6572  hey were recover
+00003e00: 6564 2e0a 2020 2020 2020 2020 6173 7365  ed..        asse
+00003e10: 7274 206e 6f74 2065 7463 2e67 6574 5f64  rt not etc.get_d
+00003e20: 6574 6163 6865 645f 6576 656e 7473 2829  etached_events()
+00003e30: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00003e40: 2020 2320 5468 6520 636f 6c6c 6563 7469    # The collecti
+00003e50: 6f6e 2068 6173 2045 7665 6e74 5472 6565  on has EventTree
+00003e60: 7320 6561 6368 2077 6974 6820 6120 7472  s each with a tr
+00003e70: 6565 206f 6620 6576 656e 7473 2e0a 2020  ee of events..  
+00003e80: 2020 2020 2020 2320 5573 696e 6720 436f        # Using Co
+00003e90: 6c6c 6563 7469 6f6e 2061 6e64 2045 7665  llection and Eve
+00003ea0: 6e74 5472 6565 732c 2079 6f75 2063 616e  ntTrees, you can
+00003eb0: 2077 6f72 6b20 666c 6578 6962 6c79 2077   work flexibly w
+00003ec0: 6974 6820 6576 656e 7473 2e0a 2020 2020  ith events..    
 00003ed0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-00003ee0: 332e 332e 325d 2047 6574 2072 6f6f 7473  3.3.2] Get roots
-00003ef0: 2069 6473 206f 6620 616c 6c20 7472 6565   ids of all tree
-00003f00: 732e 0a20 2020 2020 2020 2072 6f6f 7473  s..        roots
-00003f10: 3a20 4c69 7374 5b73 7472 5d20 3d20 6574  : List[str] = et
-00003f20: 632e 6765 745f 726f 6f74 735f 6964 7328  c.get_roots_ids(
-00003f30: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00003f40: 2020 2023 205b 332e 332e 335d 2046 696e     # [3.3.3] Fin
-00003f50: 6420 616e 2065 7665 6e74 2069 6e20 616c  d an event in al
-00003f60: 6c20 7472 6565 732e 0a20 2020 2020 2020  l trees..       
-00003f70: 2066 696e 645f 6576 656e 743a 204f 7074   find_event: Opt
-00003f80: 696f 6e61 6c5b 6469 6374 5d20 3d20 6574  ional[dict] = et
-00003f90: 632e 6669 6e64 286c 616d 6264 6120 6576  c.find(lambda ev
-00003fa0: 656e 743a 2022 5365 6e64 206d 6573 7361  ent: "Send messa
-00003fb0: 6765 2220 696e 2065 7665 6e74 5b22 6576  ge" in event["ev
-00003fc0: 656e 7454 7970 6522 5d29 0a20 2020 2020  entType"]).     
-00003fd0: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
-00003fe0: 2e33 2e34 5d20 4669 6e64 2061 6c6c 2065  .3.4] Find all e
-00003ff0: 7665 6e74 7320 696e 2061 6c6c 2074 7265  vents in all tre
-00004000: 6573 2e20 5468 6572 6520 6973 2061 6c73  es. There is als
-00004010: 6f20 6974 6572 6162 6c65 2076 6572 7369  o iterable versi
-00004020: 6f6e 2027 6669 6e64 616c 6c5f 6974 6572  on 'findall_iter
-00004030: 272e 0a20 2020 2020 2020 2066 696e 645f  '..        find_
-00004040: 6576 656e 7473 3a20 4c69 7374 5b64 6963  events: List[dic
-00004050: 745d 203d 2065 7463 2e66 696e 6461 6c6c  t] = etc.findall
-00004060: 286c 616d 6264 6120 6576 656e 743a 2065  (lambda event: e
-00004070: 7665 6e74 5b22 7375 6363 6573 7366 756c  vent["successful
-00004080: 225d 2069 7320 5472 7565 290a 2020 2020  "] is True).    
-00004090: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-000040a0: 332e 332e 355d 2046 696e 6420 616e 2061  3.3.5] Find an a
-000040b0: 6e63 6573 746f 7220 6f66 2074 6865 2065  ncestor of the e
-000040c0: 7665 6e74 2e0a 2020 2020 2020 2020 616e  vent..        an
-000040d0: 6365 7374 6f72 3a20 4f70 7469 6f6e 616c  cestor: Optional
-000040e0: 5b64 6963 745d 203d 2065 7463 2e66 696e  [dict] = etc.fin
-000040f0: 645f 616e 6365 7374 6f72 280a 2020 2020  d_ancestor(.    
-00004100: 2020 2020 2020 2020 2238 6262 6533 3731          "8bbe371
-00004110: 372d 6366 3539 2d31 3165 622d 6133 6637  7-cf59-11eb-a3f7
-00004120: 2d30 3934 6639 3034 6333 6136 3222 2c20  -094f904c3a62", 
-00004130: 6669 6c74 6572 3d6c 616d 6264 6120 6576  filter=lambda ev
-00004140: 656e 743a 2022 526f 6f74 4576 656e 7422  ent: "RootEvent"
-00004150: 2069 6e20 6576 656e 745b 2265 7665 6e74   in event["event
-00004160: 4e61 6d65 225d 0a20 2020 2020 2020 2029  Name"].        )
-00004170: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004180: 2020 2320 5b33 2e33 2e36 5d20 4765 7420    # [3.3.6] Get 
-00004190: 6368 696c 6472 656e 206f 6620 7468 6520  children of the 
-000041a0: 6576 656e 742e 2054 6865 7265 2069 7320  event. There is 
-000041b0: 616c 736f 2069 7465 7261 626c 6520 7665  also iterable ve
-000041c0: 7273 696f 6e20 2767 6574 5f63 6869 6c64  rsion 'get_child
-000041d0: 7265 6e5f 6974 6572 272e 0a20 2020 2020  ren_iter'..     
-000041e0: 2020 2063 6869 6c64 7265 6e3a 2054 7570     children: Tup
-000041f0: 6c65 5b64 6963 745d 203d 2065 7463 2e67  le[dict] = etc.g
-00004200: 6574 5f63 6869 6c64 7265 6e28 2238 3134  et_children("814
-00004210: 3432 3265 312d 3963 3638 2d31 3165 622d  422e1-9c68-11eb-
-00004220: 3835 3938 2d36 3931 6562 6437 6634 3133  8598-691ebd7f413
-00004230: 6422 290a 2020 2020 2020 2020 0a20 2020  d").        .   
-00004240: 2020 2020 2023 205b 332e 332e 375d 2047       # [3.3.7] G
-00004250: 6574 2073 7562 7472 6565 2066 6f72 2073  et subtree for s
-00004260: 7065 6369 6669 6564 2065 7665 6e74 2e0a  pecified event..
-00004270: 2020 2020 2020 2020 7375 6274 7265 653a          subtree:
-00004280: 2045 7665 6e74 5472 6565 203d 2065 7463   EventTree = etc
-00004290: 2e67 6574 5f73 7562 7472 6565 2822 3865  .get_subtree("8e
-000042a0: 3233 3737 3464 2d63 6635 392d 3131 6562  23774d-cf59-11eb
-000042b0: 2d61 3665 332d 3535 6266 6462 3262 3366  -a6e3-55bfdb2b3f
-000042c0: 3231 2229 0a20 2020 2020 2020 200a 2020  21").        .  
-000042d0: 2020 2020 2020 2320 5b33 2e33 2e38 5d20        # [3.3.8] 
-000042e0: 4765 7420 6675 6c6c 2070 6174 6820 746f  Get full path to
-000042f0: 2074 6865 2065 7665 6e74 2e0a 2020 2020   the event..    
-00004300: 2020 2020 2320 4c6f 6f6b 7320 6c69 6b65      # Looks like
-00004310: 205b 616e 6365 7374 6f72 5f72 6f6f 742c   [ancestor_root,
-00004320: 2061 6e63 6573 746f 725f 6c65 7665 6c31   ancestor_level1
-00004330: 2c20 616e 6365 7374 6f72 5f6c 6576 656c  , ancestor_level
-00004340: 322c 2065 7665 6e74 5d0a 2020 2020 2020  2, event].      
-00004350: 2020 6576 656e 745f 7061 7468 3a20 4c69    event_path: Li
-00004360: 7374 5b64 6963 745d 203d 2065 7463 2e67  st[dict] = etc.g
-00004370: 6574 5f66 756c 6c5f 7061 7468 2822 3865  et_full_path("8e
-00004380: 3235 3234 6661 2d63 6635 392d 3131 6562  2524fa-cf59-11eb
-00004390: 2d61 3366 372d 3039 3466 3930 3463 3361  -a3f7-094f904c3a
-000043a0: 3632 2229 0a20 2020 2020 2020 200a 2020  62").        .  
-000043b0: 2020 2020 2020 2320 5b33 2e33 2e39 5d20        # [3.3.9] 
-000043c0: 4765 7420 7061 7265 6e74 206f 6620 7468  Get parent of th
-000043d0: 6520 6576 656e 742e 0a20 2020 2020 2020  e event..       
-000043e0: 2070 6172 656e 7420 3d20 6574 632e 6765   parent = etc.ge
-000043f0: 745f 7061 7265 6e74 2822 3865 3235 3234  t_parent("8e2524
-00004400: 6661 2d63 6635 392d 3131 6562 2d61 3366  fa-cf59-11eb-a3f
-00004410: 372d 3039 3466 3930 3463 3361 3632 2229  7-094f904c3a62")
-00004420: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004430: 2020 2320 5b33 2e33 2e31 305d 2041 7070    # [3.3.10] App
-00004440: 656e 6420 6e65 7720 6576 656e 7420 746f  end new event to
-00004450: 2074 6865 2063 6f6c 6c65 6374 696f 6e2e   the collection.
-00004460: 0a20 2020 2020 2020 2065 7463 2e61 7070  .        etc.app
-00004470: 656e 645f 6576 656e 7428 0a20 2020 2020  end_event(.     
-00004480: 2020 2020 2020 2065 7665 6e74 3d7b 0a20         event={. 
-00004490: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000044a0: 6576 656e 7449 6422 3a20 2261 3230 6635  eventId": "a20f5
-000044b0: 6566 342d 6333 6665 2d62 6231 302d 6132  ef4-c3fe-bb10-a2
-000044c0: 3963 2d64 6433 6437 3834 3930 3965 6222  9c-dd3d784909eb"
-000044d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000044e0: 2020 2270 6172 656e 7445 7665 6e74 4964    "parentEventId
-000044f0: 223a 2022 3865 3235 3234 6661 2d63 6635  ": "8e2524fa-cf5
-00004500: 392d 3131 6562 2d61 3366 372d 3039 3466  9-11eb-a3f7-094f
-00004510: 3930 3463 3361 3632 222c 0a20 2020 2020  904c3a62",.     
-00004520: 2020 2020 2020 2020 2020 2022 6576 656e             "even
-00004530: 744e 616d 6522 3a20 2253 7475 6245 7665  tName": "StubEve
-00004540: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
-00004550: 207d 0a20 2020 2020 2020 2029 0a20 2020   }.        ).   
-00004560: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-00004570: 5b33 2e33 2e31 315d 2053 686f 7720 7468  [3.3.11] Show th
-00004580: 6520 656e 7469 7265 2063 6f6c 6c65 6374  e entire collect
-00004590: 696f 6e2e 0a20 2020 2020 2020 2065 7463  ion..        etc
-000045a0: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
-000045b0: 0a20 2020 2020 2020 2023 205b 332e 345d  .        # [3.4]
-000045c0: 2057 6f72 6b69 6e67 2077 6974 6820 7468   Working with th
-000045d0: 6520 4576 656e 7454 7265 652e 0a20 2020  e EventTree..   
-000045e0: 2020 2020 2023 2045 7665 6e74 5472 6565       # EventTree
-000045f0: 2068 6173 2074 6865 2073 616d 6520 6d65   has the same me
-00004600: 7468 6f64 7320 6173 2045 7665 6e74 5472  thods as EventTr
-00004610: 6565 436f 6c6c 6563 7469 6f6e 2c20 6275  eeCollection, bu
-00004620: 7420 6f6e 6c79 2066 6f72 2069 7473 206f  t only for its o
-00004630: 776e 2074 7265 652e 0a20 2020 2020 2020  wn tree..       
-00004640: 200a 2020 2020 2020 2020 2320 5b33 2e34   .        # [3.4
-00004650: 2e31 5d20 4765 7420 636f 6c6c 6563 7469  .1] Get collecti
-00004660: 6f6e 2074 7265 6573 2e0a 2020 2020 2020  on trees..      
-00004670: 2020 7472 6565 733a 204c 6973 745b 4576    trees: List[Ev
-00004680: 656e 7454 7265 655d 203d 2065 7463 2e67  entTree] = etc.g
-00004690: 6574 5f74 7265 6573 2829 0a20 2020 2020  et_trees().     
-000046a0: 2020 2074 7265 653a 2045 7665 6e74 5472     tree: EventTr
-000046b0: 6565 203d 2074 7265 6573 5b30 5d0a 2020  ee = trees[0].  
-000046c0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000046d0: 2042 7574 2045 7665 6e74 5472 6565 2070   But EventTree p
-000046e0: 726f 7669 6465 7320 6120 776f 726b 2077  rovides a work w
-000046f0: 6974 6820 7468 6520 7472 6565 2c20 6275  ith the tree, bu
-00004700: 7420 646f 6573 206e 6f74 206d 6f64 6966  t does not modif
-00004710: 7920 6974 2e0a 2020 2020 2020 2020 2320  y it..        # 
-00004720: 4966 2079 6f75 2077 616e 7420 746f 206d  If you want to m
-00004730: 6f64 6966 7920 7468 6520 7472 6565 2c20  odify the tree, 
-00004740: 7573 6520 4576 656e 7454 7265 6543 6f6c  use EventTreeCol
-00004750: 6c65 6374 696f 6e73 2e0a 2020 2020 2020  lections..      
-00004760: 2020 0a20 2020 2020 2020 2023 205b 332e    .        # [3.
-00004770: 355d 2057 6f72 6b69 6e67 2077 6974 6820  5] Working with 
-00004780: 5061 7265 6e74 6c65 7373 5472 6565 2e0a  ParentlessTree..
-00004790: 2020 2020 2020 2020 2320 5061 7265 6e74          # Parent
-000047a0: 6c65 7373 5472 6565 2069 7320 4576 656e  lessTree is Even
-000047b0: 7454 7265 6520 7768 6963 6820 6861 7320  tTree which has 
-000047c0: 6465 7461 6368 6564 2065 7665 6e74 7320  detached events 
-000047d0: 7769 7468 2073 7475 6273 2e0a 2020 2020  with stubs..    
-000047e0: 2020 2020 7061 7265 6e74 6c65 7373 5f74      parentless_t
-000047f0: 7265 6573 3a20 4c69 7374 5b45 7665 6e74  rees: List[Event
-00004800: 5472 6565 5d20 3d20 6574 632e 6765 745f  Tree] = etc.get_
-00004810: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
-00004820: 2829 0a20 2020 2020 2020 200a 2020 2020  ().        .    
-00004830: 2020 2020 2320 5b33 2e36 5d20 576f 726b      # [3.6] Work
-00004840: 696e 6720 7769 7468 2050 6172 656e 7445  ing with ParentE
-00004850: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
-00004860: 6f6e 2e0a 2020 2020 2020 2020 2320 5061  on..        # Pa
-00004870: 7265 6e74 4576 656e 7454 7265 6543 6f6c  rentEventTreeCol
-00004880: 6c65 6374 696f 6e20 6973 2061 2074 7265  lection is a tre
-00004890: 6520 636f 6c6c 6563 7469 6f6e 206c 696b  e collection lik
-000048a0: 6520 4576 656e 7454 7265 6543 6f6c 6c65  e EventTreeColle
-000048b0: 6374 696f 6e2c 0a20 2020 2020 2020 2023  ction,.        #
-000048c0: 2062 7574 2069 7420 6861 7320 6f6e 6c79   but it has only
-000048d0: 2065 7665 6e74 7320 7468 6174 2068 6176   events that hav
-000048e0: 6520 7265 6665 7265 6e63 6573 2e0a 2020  e references..  
-000048f0: 2020 2020 2020 6461 7461 5f73 6f75 7263        data_sourc
-00004900: 653a 2049 4461 7461 536f 7572 6365 2020  e: IDataSource  
-00004910: 2320 596f 7520 7368 6f75 6c64 2069 6e69  # You should ini
-00004920: 7420 4461 7461 536f 7572 6365 206f 626a  t DataSource obj
-00004930: 6563 742e 2045 2e67 2e20 6672 6f6d 204c  ect. E.g. from L
-00004940: 7744 5020 6d6f 6475 6c65 2e0a 2020 2020  wDP module..    
-00004950: 2020 2020 2320 4554 4344 7269 7665 7220      # ETCDriver 
-00004960: 6865 7265 2069 7320 6120 7374 7562 2c20  here is a stub, 
-00004970: 6163 7475 616c 6c79 2074 6865 206c 6962  actually the lib
-00004980: 2064 6f6e 2774 2068 6176 6520 7375 6368   don't have such
-00004990: 2063 6c61 7373 2e0a 2020 2020 2020 2020   class..        
-000049a0: 2320 596f 7520 6361 6e20 7461 6b65 2069  # You can take i
-000049b0: 7420 696e 204c 7744 5020 6d6f 6475 6c65  t in LwDP module
-000049c0: 206f 7220 6372 6561 7465 2079 6f75 7273   or create yours
-000049d0: 656c 6620 636c 6173 7320 6966 2079 6f75  elf class if you
-000049e0: 2068 6176 6520 736f 6d65 2073 7065 6369   have some speci
-000049f0: 616c 2065 7665 6e74 7320 7374 7275 6374  al events struct
-00004a00: 7572 652e 0a20 2020 2020 2020 2064 7269  ure..        dri
-00004a10: 7665 7220 3d20 4554 4344 7269 7665 7228  ver = ETCDriver(
-00004a20: 6461 7461 5f73 6f75 7263 653d 6461 7461  data_source=data
-00004a30: 5f73 6f75 7263 6529 0a20 2020 2020 2020  _source).       
-00004a40: 2065 7463 203d 2050 6172 656e 7445 7665   etc = ParentEve
-00004a50: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
-00004a60: 2864 7269 7665 7229 0a20 2020 2020 2020  (driver).       
-00004a70: 2065 7463 2e62 7569 6c64 2865 7665 6e74   etc.build(event
-00004a80: 7329 0a20 2020 2020 2020 200a 2020 2020  s).        .    
-00004a90: 2020 2020 6574 632e 7368 6f77 2829 0a20      etc.show(). 
-00004aa0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00004ab0: 2020 203c 212d 2d20 656e 6420 6765 745f     <!-- end get_
-00004ac0: 7374 6172 7465 645f 6578 616d 706c 652e  started_example.
-00004ad0: 7079 202d 2d3e 0a20 2020 2020 2020 200a  py -->.        .
-00004ae0: 2020 2020 2020 2020 2323 2032 2e33 2e20          ## 2.3. 
-00004af0: 5368 6f72 7420 7468 656f 7279 0a20 2020  Short theory.   
-00004b00: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
-00004b10: 6520 6c69 6272 6172 7920 7072 6f76 6964  e library provid
-00004b20: 6573 2074 6f6f 6c73 2066 6f72 2068 616e  es tools for han
-00004b30: 646c 696e 6720 7374 7265 616d 2064 6174  dling stream dat
-00004b40: 612e 2057 6861 7427 7320 6120 7374 7265  a. What's a stre
-00004b50: 616d 3f20 4974 2773 2061 2073 6571 7565  am? It's a seque
-00004b60: 6e63 6520 6f66 2065 6c65 6d65 6e74 7320  nce of elements 
-00004b70: 6672 6f6d 2061 2073 6f75 7263 6520 7468  from a source th
-00004b80: 6174 0a20 2020 2020 2020 2073 7570 706f  at.        suppo
-00004b90: 7274 7320 6167 6772 6567 6174 6520 6f70  rts aggregate op
-00004ba0: 6572 6174 696f 6e73 2e0a 2020 2020 2020  erations..      
-00004bb0: 2020 0a20 2020 2020 2020 2023 2323 2054    .        ### T
-00004bc0: 6572 6d73 0a20 2020 2020 2020 200a 2020  erms.        .  
-00004bd0: 2020 2020 2020 2d20 2a2a 4461 7461 206f        - **Data o
-00004be0: 626a 6563 742a 2a3a 2041 6e20 696e 7374  bject**: An inst
-00004bf0: 616e 6365 206f 6620 6044 6174 6160 2063  ance of `Data` c
-00004c00: 6c61 7373 2077 6869 6368 2069 7320 7772  lass which is wr
-00004c10: 6170 7065 7220 756e 6465 7220 7374 7265  apper under stre
-00004c20: 616d 2e0a 2020 2020 2020 2020 2d20 2a2a  am..        - **
-00004c30: 5365 7175 656e 6365 206f 6620 656c 656d  Sequence of elem
-00004c40: 656e 7473 2a2a 3a0a 2020 2020 2020 2020  ents**:.        
-00004c50: 2020 4120 5f44 6174 6120 6f62 6a65 6374    A _Data object
-00004c60: 5f20 7072 6f76 6964 6573 2061 6e20 696e  _ provides an in
-00004c70: 7465 7266 6163 6520 746f 2061 2073 6571  terface to a seq
-00004c80: 7565 6e63 6564 2073 6574 206f 6620 7661  uenced set of va
-00004c90: 6c75 6573 206f 6620 6120 7370 6563 6966  lues of a specif
-00004ca0: 6963 2065 6c65 6d65 6e74 2074 7970 652e  ic element type.
-00004cb0: 2053 7472 6561 6d20 696e 7369 6465 2074   Stream inside t
-00004cc0: 6865 205f 4461 7461 0a20 2020 2020 2020  he _Data.       
-00004cd0: 2020 206f 626a 6563 745f 202a 2a64 6f6e     object_ **don
-00004ce0: 1974 2061 6374 7561 6c6c 7920 7374 6f72  .t actually stor
-00004cf0: 652a 2a20 656c 656d 656e 7473 3b20 7468  e** elements; th
-00004d00: 6579 2061 7265 2063 6f6d 7075 7465 6420  ey are computed 
-00004d10: 6f6e 2064 656d 616e 642e 0a20 2020 2020  on demand..     
-00004d20: 2020 202d 202a 2a64 6174 6120 736f 7572     - **data sour
-00004d30: 6365 2a2a 2028 6578 6163 746c 7920 696e  ce** (exactly in
-00004d40: 2073 6d61 6c6c 206c 6574 7465 7273 293a   small letters):
-00004d50: 0a20 2020 2020 2020 2020 2041 6e79 2073  .          Any s
-00004d60: 6f75 7263 6520 6f66 2064 6174 612e 2045  ource of data. E
-00004d70: 2e67 2e20 5b4c 6967 6874 7765 6967 6874  .g. [Lightweight
-00004d80: 2044 6174 6120 5072 6f76 6964 6572 5d28   Data Provider](
-00004d90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00004da0: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d6c  om/th2-net/th2-l
-00004db0: 772d 6461 7461 2d70 726f 7669 6465 7229  w-data-provider)
-00004dc0: 2c20 636f 6c6c 6563 7469 6f6e 732c 0a20  , collections,. 
-00004dd0: 2020 2020 2020 2020 2061 7272 6179 732c           arrays,
-00004de0: 206f 7220 492f 4f20 7265 736f 7572 6365   or I/O resource
-00004df0: 732e 0a20 2020 2020 2020 202d 202a 2a44  s..        - **D
-00004e00: 6174 6153 6f75 7263 652a 2a3a 0a20 2020  ataSource**:.   
-00004e10: 2020 2020 2020 2041 2063 6c61 7373 2074         A class t
-00004e20: 6861 7420 6973 2061 6e20 696e 7465 726d  hat is an interm
-00004e30: 6564 6961 7465 206c 696e 6b20 6265 7477  ediate link betw
-00004e40: 6565 6e20 7468 6520 536f 7572 6365 4150  een the SourceAP
-00004e50: 4920 616e 6420 436f 6d6d 616e 6473 2e0a  I and Commands..
-00004e60: 2020 2020 2020 2020 2d20 2a2a 536f 7572          - **Sour
-00004e70: 6365 4150 492a 2a3a 0a20 2020 2020 2020  ceAPI**:.       
-00004e80: 2020 2045 6163 6820 736f 7572 6365 2068     Each source h
-00004e90: 6173 2069 7473 206f 776e 2041 5049 2074  as its own API t
-00004ea0: 6f20 7265 7472 6965 7665 2064 6174 612e  o retrieve data.
-00004eb0: 2053 6f75 7263 6541 5049 2069 7320 6120   SourceAPI is a 
-00004ec0: 636c 6173 7320 7468 6174 2070 726f 7669  class that provi
-00004ed0: 6465 2041 5049 2066 6f72 2073 6f6d 6520  de API for some 
-00004ee0: 6461 7461 2073 6f75 7263 652e 0a20 2020  data source..   
-00004ef0: 2020 2020 202d 202a 2a43 6f6d 6d61 6e64       - **Command
-00004f00: 732a 2a3a 0a20 2020 2020 2020 2020 2043  s**:.          C
-00004f10: 6c61 7373 6573 2074 6861 7420 7072 6f76  lasses that prov
-00004f20: 6964 6520 7573 6572 2d66 7269 656e 646c  ide user-friendl
-00004f30: 7920 696e 7465 7266 6163 6573 2066 6f72  y interfaces for
-00004f40: 2067 6574 7469 6e67 2073 6f6d 6520 6461   getting some da
-00004f50: 7461 2066 726f 6d20 4461 7461 536f 7572  ta from DataSour
-00004f60: 6365 2e20 436f 6d6d 616e 6473 2075 7365  ce. Commands use
-00004f70: 205f 536f 7572 6365 4150 495f 2074 6f0a   _SourceAPI_ to.
-00004f80: 2020 2020 2020 2020 2020 6163 6869 6576            achiev
-00004f90: 6520 6974 2e0a 2020 2020 2020 2020 2d20  e it..        - 
-00004fa0: 2a2a 4164 6170 7465 7273 2a2a 3a0a 2020  **Adapters**:.  
-00004fb0: 2020 2020 2020 2020 4974 2773 2073 696d          It's sim
-00004fc0: 696c 6172 2074 6f20 6675 6e63 7469 6f6e  ilar to function
-00004fd0: 2066 6f72 2060 4461 7461 2e6d 6170 6020   for `Data.map` 
-00004fe0: 6d65 7468 6f64 2e20 4164 6f70 7461 626c  method. Adoptabl
-00004ff0: 6520 636f 6d6d 616e 6473 2075 7365 6420  e commands used 
-00005000: 6974 2074 6f20 7570 6461 7465 2074 6865  it to update the
-00005010: 2064 6174 6120 7374 7265 616d 2e0a 2020   data stream..  
-00005020: 2020 2020 2020 2d20 2a2a 4167 6772 6567        - **Aggreg
-00005030: 6174 6520 6f70 6572 6174 696f 6e73 2a2a  ate operations**
-00005040: 3a0a 2020 2020 2020 2020 2020 436f 6d6d  :.          Comm
-00005050: 6f6e 206f 7065 7261 7469 6f6e 7320 7375  on operations su
-00005060: 6368 2061 7320 6669 6c74 6572 2c20 6d61  ch as filter, ma
-00005070: 702c 206c 696d 6974 2061 6e64 2073 6f20  p, limit and so 
-00005080: 6f6e 2e0a 2020 2020 2020 2020 2d20 2a2a  on..        - **
-00005090: 576f 726b 666c 6f77 2a2a 3a20 416e 206f  Workflow**: An o
-000050a0: 7264 6572 6564 2073 6574 206f 6620 5f41  rdered set of _A
-000050b0: 6767 7265 6761 7465 206f 7065 7261 7469  ggregate operati
-000050c0: 6f6e 735f 2e0a 2020 2020 2020 2020 0a20  ons_..        . 
-000050d0: 2020 2020 2020 2023 2323 2043 6f6e 6365         ### Conce
-000050e0: 7074 0a20 2020 2020 2020 200a 2020 2020  pt.        .    
-000050f0: 2020 2020 5468 6520 6c69 6272 6172 7920      The library 
-00005100: 6465 7363 7269 6265 7320 7468 6520 6869  describes the hi
-00005110: 6768 2d6c 6576 656c 2069 6e74 6572 6661  gh-level interfa
-00005120: 6365 7320 6049 536f 7572 6365 4150 4960  ces `ISourceAPI`
-00005130: 2c20 6049 4461 7461 536f 7572 6365 602c  , `IDataSource`,
-00005140: 2060 4943 6f6d 6d61 6e64 602c 2060 4941   `ICommand`, `IA
-00005150: 6461 7074 6572 602e 0a20 2020 2020 2020  dapter`..       
-00005160: 200a 2020 2020 2020 2020 416e 7920 6461   .        Any da
-00005170: 7461 2073 6f75 7263 6520 6d75 7374 2062  ta source must b
-00005180: 6520 6465 7363 7269 6265 6420 6279 2074  e described by t
-00005190: 6865 2060 4944 6174 6153 6f75 7263 6560  he `IDataSource`
-000051a0: 2061 6273 7472 6163 7420 636c 6173 732e   abstract class.
-000051b0: 2054 6865 7365 2063 616e 2062 6520 5f46   These can be _F
-000051c0: 696c 6544 6174 6153 6f75 7263 655f 2c20  ileDataSource_, 
-000051d0: 0a20 2020 2020 2020 205f 4353 5644 6174  .        _CSVDat
-000051e0: 6153 6f75 7263 655f 2c20 5f44 4244 6174  aSource_, _DBDat
-000051f0: 6153 6f75 7263 655f 2061 6e64 206f 7468  aSource_ and oth
-00005200: 6572 2e0a 2020 2020 2020 2020 0a20 2020  er..        .   
-00005210: 2020 2020 2055 7375 616c 6c79 2c20 6461       Usually, da
-00005220: 7461 2073 6f75 7263 6573 2068 6176 6520  ta sources have 
-00005230: 736f 6d65 206b 696e 6420 6f66 2041 5049  some kind of API
-00005240: 2e20 4461 7461 6261 7365 7320 2d20 7072  . Databases - pr
-00005250: 6f76 6964 6520 5351 4c20 6c61 6e67 7561  ovide SQL langua
-00005260: 6765 2c20 7768 656e 2077 6f72 6b69 6e67  ge, when working
-00005270: 2077 6974 6820 6120 6669 6c65 2c20 796f   with a file, yo
-00005280: 7520 6361 6e20 7265 6164 0a20 2020 2020  u can read.     
-00005290: 2020 206c 696e 6520 6279 206c 696e 652c     line by line,
-000052a0: 2065 7463 2e20 5468 6973 2041 5049 2069   etc. This API i
-000052b0: 7320 6465 7363 7269 6265 6420 6279 2074  s described by t
-000052c0: 6865 2060 4953 6f75 7263 6541 5049 6020  he `ISourceAPI` 
-000052d0: 636c 6173 732e 2042 6563 6175 7365 2064  class. Because d
-000052e0: 6966 6665 7265 6e74 2076 6572 7369 6f6e  ifferent version
-000052f0: 7320 6f66 2074 6865 2073 616d 6520 6461  s of the same da
-00005300: 7461 2073 6f75 7263 650a 2020 2020 2020  ta source.      
-00005310: 2020 6d61 7920 6861 7665 2064 6966 6665    may have diffe
-00005320: 7265 6e74 2041 5049 2c20 6974 2069 7320  rent API, it is 
-00005330: 6265 7474 6572 2074 6f20 6372 6561 7465  better to create
-00005340: 2061 2063 6c61 7373 2066 6f72 2065 6163   a class for eac
-00005350: 6820 7665 7273 696f 6e2e 0a20 2020 2020  h version..     
-00005360: 2020 200a 2020 2020 2020 2020 4765 6e65     .        Gene
-00005370: 7261 6c6c 792c 2064 6174 6120 736f 7572  rally, data sour
-00005380: 6365 2041 5049 7320 6172 6520 6869 6464  ce APIs are hidd
-00005390: 656e 2062 6568 696e 6420 636f 6e76 656e  en behind conven
-000053a0: 6965 6e74 2069 6e74 6572 6661 6365 732e  ient interfaces.
-000053b0: 2054 6865 2072 6f6c 6520 6f66 2074 6865   The role of the
-000053c0: 7365 2069 6e74 6572 6661 6365 7320 6973  se interfaces is
-000053d0: 2070 6c61 7965 640a 2020 2020 2020 2020   played.        
-000053e0: 6279 2060 4943 6f6d 6d61 6e64 6020 636c  by `ICommand` cl
-000053f0: 6173 7365 732e 0a20 2020 2020 2020 200a  asses..        .
-00005400: 2020 2020 2020 2020 6049 4164 6170 7465          `IAdapte
-00005410: 7260 2063 6c61 7373 6573 2074 7261 6e73  r` classes trans
-00005420: 666f 726d 2064 6174 6120 7374 7265 616d  form data stream
-00005430: 206c 696b 6520 6675 6e63 7469 6f6e 7320   like functions 
-00005440: 666f 7220 6044 6174 612e 6d61 7060 206d  for `Data.map` m
-00005450: 6574 686f 642e 2045 7373 656e 7469 616c  ethod. Essential
-00005460: 6c79 2069 7427 7320 7468 6520 7361 6d65  ly it's the same
-00005470: 2074 6869 6e67 2062 7574 206d 6f72 650a   thing but more.
-00005480: 2020 2020 2020 2020 666c 6578 6962 6c65          flexible
-00005490: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000054a0: 2020 2046 6f72 2065 7861 6d70 6c65 2c20     For example, 
-000054b0: 4c77 4450 2044 6174 6153 6f75 7263 6528  LwDP DataSource(
-000054c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000054d0: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d64  om/th2-net/th2-d
-000054e0: 732d 736f 7572 6365 2d6c 7764 7029 2075  s-source-lwdp) u
-000054f0: 7365 7320 7468 6573 6520 6162 7374 7261  ses these abstra
-00005500: 6374 2063 6c61 7373 6573 2074 6f20 6275  ct classes to bu
-00005510: 696c 6420 6974 7320 696d 706c 656d 656e  ild its implemen
-00005520: 7461 7469 6f6e 2e59 6f75 2063 616e 2065  tation.You can e
-00005530: 6173 696c 7920 6372 6561 7465 2079 6f75  asily create you
-00005540: 7220 6f77 6e20 756e 6971 7565 2063 6f6d  r own unique com
-00005550: 6d61 6e64 7320 666f 7220 5f4c 7744 5020  mands for _LwDP 
-00005560: 4461 7461 536f 7572 6365 5f2c 2061 7320  DataSource_, as 
-00005570: 7765 6c6c 2061 7320 656e 7469 7265 0a20  well as entire. 
-00005580: 2020 2020 2020 205f 4461 7461 536f 7572         _DataSour
-00005590: 6365 5f20 636c 6173 7365 732e 205b 4865  ce_ classes. [He
-000055a0: 7265 2069 7320 6120 646f 6375 6d65 6e74  re is a document
-000055b0: 6174 696f 6e5d 2864 6f63 756d 656e 7461  ation](documenta
-000055c0: 7469 6f6e 2f64 6174 6173 6f75 7263 652e  tion/datasource.
-000055d0: 6d64 2920 6f6e 2068 6f77 2074 6f20 696d  md) on how to im
-000055e0: 706c 656d 656e 7420 7468 6573 6520 696e  plement these in
-000055f0: 7465 7266 6163 6573 2e0a 2020 2020 2020  terfaces..      
-00005600: 2020 0a20 2020 2020 2020 2021 5b44 6174    .        ![Dat
-00005610: 6120 7374 7265 616d 2070 6970 656c 696e  a stream pipelin
-00005620: 655d 2864 6f63 756d 656e 7461 7469 6f6e  e](documentation
-00005630: 2f69 6d67 2f63 6f6e 6365 7074 2e70 6e67  /img/concept.png
-00005640: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00005650: 2020 2023 2323 2053 7472 6561 6d20 6f70     ### Stream op
-00005660: 6572 6174 696f 6e73 0a20 2020 2020 2020  erations.       
-00005670: 200a 2020 2020 2020 2020 4675 7274 6865   .        Furthe
-00005680: 726d 6f72 652c 2073 7472 6561 6d20 6f70  rmore, stream op
-00005690: 6572 6174 696f 6e73 2068 6176 6520 7477  erations have tw
-000056a0: 6f20 6675 6e64 616d 656e 7461 6c20 6368  o fundamental ch
-000056b0: 6172 6163 7465 7269 7374 6963 7320 7468  aracteristics th
-000056c0: 6174 206d 616b 6520 7468 656d 2076 6572  at make them ver
-000056d0: 7920 6469 6666 6572 656e 7420 6672 6f6d  y different from
-000056e0: 2063 6f6c 6c65 6374 696f 6e0a 2020 2020   collection.    
-000056f0: 2020 2020 6f70 6572 6174 696f 6e73 3a20      operations: 
-00005700: 5f50 6970 656c 696e 696e 675f 2061 6e64  _Pipelining_ and
-00005710: 205f 496e 7465 726e 616c 2069 7465 7261   _Internal itera
-00005720: 7469 6f6e 5f2e 0a20 2020 2020 2020 200a  tion_..        .
-00005730: 2020 2020 2020 2020 2323 2323 2050 6970          #### Pip
-00005740: 656c 696e 696e 670a 2020 2020 2020 2020  elining.        
-00005750: 0a20 2020 2020 2020 204d 616e 7920 7374  .        Many st
-00005760: 7265 616d 206f 7065 7261 7469 6f6e 7320  ream operations 
-00005770: 7265 7475 726e 2061 2073 7472 6561 6d20  return a stream 
-00005780: 7468 656d 7365 6c76 6573 2e20 5468 6973  themselves. This
-00005790: 2061 6c6c 6f77 7320 6f70 6572 6174 696f   allows operatio
-000057a0: 6e73 2074 6f20 6265 2063 6861 696e 6564  ns to be chained
-000057b0: 2074 6f20 666f 726d 2061 206c 6172 6765   to form a large
-000057c0: 7220 7069 7065 6c69 6e65 2e0a 2020 2020  r pipeline..    
-000057d0: 2020 2020 0a20 2020 2020 2020 2021 5b44      .        ![D
-000057e0: 6174 6120 7374 7265 616d 2070 6970 656c  ata stream pipel
-000057f0: 696e 655d 2864 6f63 756d 656e 7461 7469  ine](documentati
-00005800: 6f6e 2f69 6d67 2f64 6174 615f 7374 7265  on/img/data_stre
-00005810: 616d 5f70 6970 656c 696e 652e 706e 6729  am_pipeline.png)
-00005820: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00005830: 2020 2323 2323 2049 6e74 6572 6e61 6c20    #### Internal 
-00005840: 6974 6572 6174 696f 6e0a 2020 2020 2020  iteration.      
-00005850: 2020 0a20 2020 2020 2020 2049 6e20 636f    .        In co
-00005860: 6e74 7261 7374 2074 6f20 636f 6c6c 6563  ntrast to collec
-00005870: 7469 6f6e 732c 2077 6869 6368 2061 7265  tions, which are
-00005880: 2069 7465 7261 7465 6420 6578 706c 6963   iterated explic
-00005890: 6974 6c79 2028 6578 7465 726e 616c 2069  itly (external i
-000058a0: 7465 7261 7469 6f6e 292c 2073 7472 6561  teration), strea
-000058b0: 6d20 6f70 6572 6174 696f 6e73 2064 6f20  m operations do 
-000058c0: 7468 6520 6974 6572 6174 696f 6e0a 2020  the iteration.  
-000058d0: 2020 2020 2020 6265 6869 6e64 2074 6865        behind the
-000058e0: 2073 6365 6e65 7320 666f 7220 796f 752e   scenes for you.
-000058f0: 204e 6f74 652c 2069 7420 646f 6573 6e27   Note, it doesn'
-00005900: 7420 6d65 616e 2079 6f75 2063 616e 6e6f  t mean you canno
-00005910: 7420 6974 6572 6174 6520 7468 6520 5f44  t iterate the _D
-00005920: 6174 6120 6f62 6a65 6374 5f2e 0a20 2020  ata object_..   
-00005930: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00005940: 2320 4461 7461 2063 6163 6869 6e67 0a20  # Data caching. 
-00005950: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00005960: 5468 6520 5f44 6174 6120 6f62 6a65 6374  The _Data object
-00005970: 5f20 7072 6f76 6964 6573 2074 6865 2061  _ provides the a
-00005980: 6269 6c69 7479 2074 6f20 7573 6520 7468  bility to use th
-00005990: 6520 6361 6368 652e 2054 6865 2063 6163  e cache. The cac
-000059a0: 6865 2077 6f72 6b73 2066 6f72 2065 6163  he works for eac
-000059b0: 6820 5f44 6174 6120 6f62 6a65 6374 5f2c  h _Data object_,
-000059c0: 2074 6861 7420 6973 2c20 796f 7520 6368   that is, you ch
-000059d0: 6f6f 7365 0a20 2020 2020 2020 2077 6869  oose.        whi
-000059e0: 6368 205f 4461 7461 206f 626a 6563 745f  ch _Data object_
-000059f0: 2079 6f75 2077 616e 7420 746f 2073 6176   you want to sav
-00005a00: 652e 2054 6865 205f 4461 7461 206f 626a  e. The _Data obj
-00005a10: 6563 745f 2063 6163 6865 2069 7320 7361  ect_ cache is sa
-00005a20: 7665 6420 6166 7465 7220 7468 6520 6669  ved after the fi
-00005a30: 7273 7420 6974 6572 6174 696f 6e2c 2062  rst iteration, b
-00005a40: 7574 2074 6865 2069 7465 7261 7469 6f6e  ut the iteration
-00005a50: 0a20 2020 2020 2020 2073 6f75 7263 6520  .        source 
-00005a60: 6d61 7920 6265 2064 6966 6665 7265 6e74  may be different
-00005a70: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00005a80: 2020 2049 6620 796f 7520 646f 6e27 7420     If you don't 
-00005a90: 7573 6520 7468 6520 6361 6368 652c 2079  use the cache, y
-00005aa0: 6f75 7220 736f 7572 6365 2077 696c 6c20  our source will 
-00005ab0: 6265 2074 6865 2064 6174 6120 736f 7572  be the data sour
-00005ac0: 6365 2079 6f75 2068 6176 6520 696e 2074  ce you have in t
-00005ad0: 6865 205f 4461 7461 204f 626a 6563 745f  he _Data Object_
-00005ae0: 2e20 4275 7420 6966 2079 6f75 2075 7365  . But if you use
-00005af0: 2074 6865 2063 6163 6865 2c0a 2020 2020   the cache,.    
-00005b00: 2020 2020 796f 7572 2073 6f75 7263 6520      your source 
-00005b10: 6361 6e20 6265 2074 6865 2064 6174 6120  can be the data 
-00005b20: 736f 7572 6365 2c20 7468 6520 7061 7265  source, the pare
-00005b30: 6e74 2063 6163 6865 2c20 6f72 206f 776e  nt cache, or own
-00005b40: 2063 6163 6865 3a0a 2020 2020 2020 2020   cache:.        
-00005b50: 0a20 2020 2020 2020 202a 2054 6865 2064  .        * The d
-00005b60: 6174 6120 736f 7572 6365 3a0a 2020 2020  ata source:.    
-00005b70: 2020 2020 2020 4966 2074 6865 205f 4461        If the _Da
-00005b80: 7461 204f 626a 6563 745f 2064 6f65 736e  ta Object_ doesn
-00005b90: 2774 2068 6176 6520 6120 7061 7265 6e74  't have a parent
-00005ba0: 2063 6163 6865 2061 6e64 2069 7473 2063   cache and its c
-00005bb0: 6163 6865 2e0a 2020 2020 2020 2020 2a20  ache..        * 
-00005bc0: 5468 6520 7061 7265 6e74 2063 6163 6865  The parent cache
-00005bd0: 3a0a 2020 2020 2020 2020 2020 4966 2074  :.          If t
-00005be0: 6865 205f 4461 7461 204f 626a 6563 745f  he _Data Object_
-00005bf0: 2068 6173 2061 2070 6172 656e 7420 6361   has a parent ca
-00005c00: 6368 652e 2049 7420 646f 6573 6e27 7420  che. It doesn't 
-00005c10: 6d61 7474 6572 2077 6861 7420 706f 7369  matter what posi
-00005c20: 7469 6f6e 2074 6865 2070 6172 656e 7420  tion the parent 
-00005c30: 6361 6368 6520 6861 7320 696e 2069 6e68  cache has in inh
-00005c40: 6572 6974 616e 6365 2e0a 2020 2020 2020  eritance..      
-00005c50: 2020 2020 5f44 6174 6120 4f62 6a65 6374      _Data Object
-00005c60: 5f20 756e 6465 7273 7461 6e64 7320 7768  _ understands wh
-00005c70: 6f73 6520 6361 6368 6520 6974 2069 7320  ose cache it is 
-00005c80: 616e 6420 6578 6563 7574 6573 2074 6865  and executes the
-00005c90: 2070 6172 7420 6f66 2074 6865 2077 6f72   part of the wor
-00005ca0: 6b66 6c6f 7720 7468 6174 2077 6173 206e  kflow that was n
-00005cb0: 6f74 2065 7865 6375 7465 642e 0a20 2020  ot executed..   
-00005cc0: 2020 2020 202a 2054 6865 206f 776e 2063       * The own c
-00005cd0: 6163 6865 3a0a 2020 2020 2020 2020 2020  ache:.          
-00005ce0: 4966 2069 7420 6973 206e 6f74 2074 6865  If it is not the
-00005cf0: 2066 6972 7374 2069 7465 7261 7469 6f6e   first iteration
-00005d00: 206f 6620 7468 6973 2044 6174 6120 6f62   of this Data ob
-00005d10: 6a65 6374 2e0a 2020 2020 2020 2020 0a20  ject..        . 
-00005d20: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
-00005d30: 2074 6865 2063 6163 6865 2073 7461 7465   the cache state
-00005d40: 206f 6620 7468 6520 4461 7461 206f 626a   of the Data obj
-00005d50: 6563 7420 6973 206e 6f74 2069 6e68 6572  ect is not inher
-00005d60: 6974 6564 2e0a 2020 2020 2020 2020 0a20  ited..        . 
-00005d70: 2020 2020 2020 2023 2323 2320 466f 7263         #### Forc
-00005d80: 6564 2063 6163 6869 6e67 0a20 2020 2020  ed caching.     
-00005d90: 2020 2059 6f75 2063 616e 2074 656c 6c20     You can tell 
-00005da0: 4453 2074 6f20 6361 6368 6520 6461 7461  DS to cache data
-00005db0: 2074 6f20 7370 6563 6966 6963 2063 6163   to specific cac
-00005dc0: 6865 2066 696c 652c 2077 6869 6368 2077  he file, which w
-00005dd0: 6f6e 2774 2062 6520 6465 6c65 7465 6420  on't be deleted 
-00005de0: 6166 7465 7220 7363 7269 7074 2065 6e64  after script end
-00005df0: 2e0a 2020 2020 2020 2020 596f 7520 6361  ..        You ca
-00005e00: 6e20 7365 6520 6578 616d 706c 6520 696e  n see example in
-00005e10: 2031 2e31 3220 7365 6374 696f 6e20 6f66   1.12 section of
-00005e20: 205b 6765 745f 7374 6172 7465 645f 6578   [get_started_ex
-00005e30: 616d 706c 655d 2865 7861 6d70 6c65 732f  ample](examples/
-00005e40: 6765 745f 7374 6172 7465 645f 6578 616d  get_started_exam
-00005e50: 706c 652e 7079 292e 0a20 2020 2020 2020  ple.py)..       
-00005e60: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
-00005e70: 2020 2023 2323 2045 7665 6e74 5472 6565     ### EventTree
-00005e80: 2061 6e64 2063 6f6c 6c65 6374 696f 6e73   and collections
-00005e90: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00005ea0: 2020 2323 2323 2045 7665 6e74 5472 6565    #### EventTree
-00005eb0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00005ec0: 2020 6045 7665 6e74 5472 6565 6020 6973    `EventTree` is
-00005ed0: 2061 2074 7265 652d 6261 7365 6420 6461   a tree-based da
-00005ee0: 7461 2073 7472 7563 7475 7265 206f 6620  ta structure of 
-00005ef0: 6576 656e 7473 2e20 4974 2061 6c6c 6f77  events. It allow
-00005f00: 7320 796f 7520 6765 7420 6368 696c 6472  s you get childr
-00005f10: 656e 2061 6e64 2070 6172 656e 7473 206f  en and parents o
-00005f20: 6620 6576 656e 742c 200a 2020 2020 2020  f event, .      
-00005f30: 2020 6469 7370 6c61 7920 7472 6565 2c20    display tree, 
-00005f40: 6765 7420 6675 6c6c 2070 6174 6820 746f  get full path to
-00005f50: 2065 7665 6e74 2065 7463 2e0a 2020 2020   event etc..    
-00005f60: 2020 2020 0a20 2020 2020 2020 2044 6574      .        Det
-00005f70: 6169 6c73 3a0a 2020 2020 2020 2020 0a20  ails:.        . 
-00005f80: 2020 2020 2020 202a 2060 4576 656e 7454         * `EventT
-00005f90: 7265 6560 2063 6f6e 7461 696e 7320 616c  ree` contains al
-00005fa0: 6c20 6576 656e 7473 2069 6e20 6d65 6d6f  l events in memo
-00005fb0: 7279 2e0a 2020 2020 2020 2020 2a20 5472  ry..        * Tr
-00005fc0: 6565 2068 6173 2073 6f6d 6520 696d 706f  ee has some impo
-00005fd0: 7274 616e 7420 7465 726d 733a 0a20 2020  rtant terms:.   
-00005fe0: 2020 2020 2020 2020 2031 2e20 5f41 6e63           1. _Anc
-00005ff0: 6573 746f 725f 2069 7320 616e 7920 7265  estor_ is any re
-00006000: 6c61 7469 7665 206f 6620 7468 6520 6576  lative of the ev
-00006010: 656e 7420 7570 2074 6865 2074 7265 6520  ent up the tree 
-00006020: 2867 7261 6e64 7061 7265 6e74 2c20 7061  (grandparent, pa
-00006030: 7265 6e74 2065 7463 2e29 2e0a 2020 2020  rent etc.)..    
-00006040: 2020 2020 2020 2020 322e 205f 5061 7265          2. _Pare
-00006050: 6e74 5f20 6973 206f 6e6c 7920 7468 6520  nt_ is only the 
-00006060: 6669 7273 7420 7265 6c61 7469 7665 206f  first relative o
-00006070: 6620 7468 6520 6576 656e 7420 7570 2074  f the event up t
-00006080: 6865 2074 7265 652e 0a20 2020 2020 2020  he tree..       
-00006090: 2020 2020 2033 2e20 5f43 6869 6c64 5f20       3. _Child_ 
-000060a0: 6973 2074 6865 2066 6972 7374 2072 656c  is the first rel
-000060b0: 6174 6976 6520 6f66 2074 6865 2065 7665  ative of the eve
-000060c0: 6e74 2064 6f77 6e20 7468 6520 7472 6565  nt down the tree
-000060d0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000060e0: 2020 2054 616b 6520 6120 6c6f 6f6b 2061     Take a look a
-000060f0: 7420 7468 6520 666f 6c6c 6f77 696e 6720  t the following 
-00006100: 4854 4d4c 2074 7265 6520 746f 2075 6e64  HTML tree to und
-00006110: 6572 7374 616e 6420 7468 656d 2e0a 2020  erstand them..  
-00006120: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00006130: 2020 6060 600a 2020 2020 2020 2020 2020    ```.          
-00006140: 2020 3c62 6f64 793e 203c 212d 2d20 616e    <body> <!-- an
-00006150: 6365 7374 6f72 2028 6772 616e 6470 6172  cestor (grandpar
-00006160: 656e 7429 2c20 6275 7420 6e6f 7420 7061  ent), but not pa
-00006170: 7265 6e74 202d 2d3e 0a20 2020 2020 2020  rent -->.       
-00006180: 2020 2020 2020 2020 203c 6469 763e 203c           <div> <
-00006190: 212d 2d20 7061 7265 6e74 2026 2061 6e63  !-- parent & anc
-000061a0: 6573 746f 7220 2d2d 3e0a 2020 2020 2020  estor -->.      
-000061b0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000061c0: 3e48 656c 6c6f 2c20 776f 726c 6421 3c2f  >Hello, world!</
-000061d0: 703e 203c 212d 2d20 6368 696c 6420 2d2d  p> <!-- child --
-000061e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000061f0: 2020 2020 2020 3c70 3e47 6f6f 6462 7965        <p>Goodbye
-00006200: 213c 2f70 3e20 3c21 2d2d 2073 6962 6c69  !</p> <!-- sibli
-00006210: 6e67 202d 2d3e 0a20 2020 2020 2020 2020  ng -->.         
-00006220: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00006230: 2020 2020 2020 2020 2020 3c2f 626f 6479            </body
-00006240: 3e0a 2020 2020 2020 2020 2020 2060 6060  >.           ```
-00006250: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006260: 2020 2323 2323 2043 6f6c 6c65 6374 696f    #### Collectio
-00006270: 6e73 0a20 2020 2020 2020 200a 2020 2020  ns.        .    
-00006280: 2020 2020 2a2a 4576 656e 7454 7265 6543      **EventTreeC
-00006290: 6f6c 6c65 6374 696f 6e2a 2a20 6973 2061  ollection** is a
-000062a0: 2063 6f6c 6c65 6374 696f 6e20 6f66 2045   collection of E
-000062b0: 7665 6e74 5472 6565 732e 2054 6865 2063  ventTrees. The c
-000062c0: 6f6c 6c65 6374 696f 6e20 6275 696c 6473  ollection builds
-000062d0: 2061 2066 6577 205f 4576 656e 7454 7265   a few _EventTre
-000062e0: 655f 2062 7920 7061 7373 6564 205f 4461  e_ by passed _Da
-000062f0: 7461 0a20 2020 2020 2020 206f 626a 6563  ta.        objec
-00006300: 745f 2e20 416c 7468 6f75 6768 2079 6f75  t_. Although you
-00006310: 2063 616e 2063 6861 6e67 6520 7468 6520   can change the 
-00006320: 7472 6565 2064 6972 6563 746c 792c 2069  tree directly, i
-00006330: 7427 7320 6265 7474 6572 2074 6f20 646f  t's better to do
-00006340: 2069 7420 7468 726f 7567 6820 636f 6c6c   it through coll
-00006350: 6563 7469 6f6e 7320 6265 6361 7573 6520  ections because 
-00006360: 7468 6579 2061 7265 2061 7761 7265 206f  they are aware o
-00006370: 660a 2020 2020 2020 2020 6064 6574 6163  f.        `detac
-00006380: 6865 645f 6576 656e 7473 6020 616e 6420  hed_events` and 
-00006390: 6361 6e20 736f 6c76 6520 736f 6d65 2065  can solve some e
-000063a0: 7665 6e74 7320 6465 7065 6e64 656e 6369  vents dependenci
-000063b0: 6573 2e20 5468 6520 636f 6c6c 6563 7469  es. The collecti
-000063c0: 6f6e 2068 6173 2073 696d 696c 6172 2066  on has similar f
-000063d0: 6561 7475 7265 7320 6c69 6b65 2061 2073  eatures like a s
-000063e0: 696e 676c 6520 5f45 7665 6e74 5472 6565  ingle _EventTree
-000063f0: 5f0a 2020 2020 2020 2020 6275 7420 6170  _.        but ap
-00006400: 706c 7969 6e67 2074 6865 6d20 666f 7220  plying them for 
-00006410: 616c 6c20 5f45 7665 6e74 5472 6565 735f  all _EventTrees_
-00006420: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00006430: 2020 202a 2a50 6172 656e 7445 7665 6e74     **ParentEvent
-00006440: 5472 6565 436f 6c6c 6563 7469 6f6e 2a2a  TreeCollection**
-00006450: 2069 7320 6120 636f 6c6c 6563 7469 6f6e   is a collection
-00006460: 2073 696d 696c 6172 2074 6f20 5f45 7665   similar to _Eve
-00006470: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
-00006480: 5f20 6275 7420 636f 6e74 6169 6e69 6e67  _ but containing
-00006490: 206f 6e6c 7920 7061 7265 6e74 2065 7665   only parent eve
-000064a0: 6e74 7320 7468 6174 0a20 2020 2020 2020  nts that.       
-000064b0: 2061 7265 2072 6566 6572 656e 6365 6420   are referenced 
-000064c0: 696e 2074 6865 2064 6174 6120 7374 7265  in the data stre
-000064d0: 616d 2e20 5468 6520 636f 6c6c 6563 7469  am. The collecti
-000064e0: 6f6e 2068 6173 2066 6561 7475 7265 7320  on has features 
-000064f0: 7369 6d69 6c61 7220 746f 205f 4576 656e  similar to _Even
-00006500: 7454 7265 6543 6f6c 6c65 6374 696f 6e5f  tTreeCollection_
-00006510: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00006520: 2020 2044 6574 6169 6c73 3a0a 2020 2020     Details:.    
-00006530: 2020 2020 0a20 2020 2020 2020 202a 2054      .        * T
-00006540: 6f20 7573 6520 4554 2063 6f6c 6c65 6374  o use ET collect
-00006550: 696f 6e73 2079 6f75 206e 6565 6420 746f  ions you need to
-00006560: 2069 6e69 7469 616c 697a 6520 7468 656d   initialize them
-00006570: 2062 7920 5f45 5443 4472 6976 6572 5f2e   by _ETCDriver_.
-00006580: 2044 6174 6120 736f 7572 6365 7320 7573   Data sources us
-00006590: 7561 6c6c 7920 7072 6f76 6964 6520 7468  ually provide th
-000065a0: 656d 2e0a 2020 2020 2020 2020 2020 596f  em..          Yo
-000065b0: 7520 6361 6e20 6372 6561 7465 2069 7420  u can create it 
-000065c0: 6279 2079 6f75 7273 656c 6620 6465 7065  by yourself depe
-000065d0: 6e64 696e 6720 6f6e 2079 6f75 7220 6461  nding on your da
-000065e0: 7461 2073 7472 7563 7475 7265 2e20 200a  ta structure.  .
-000065f0: 2020 2020 2020 2020 2a20 5468 6520 636f          * The co
-00006600: 6c6c 6563 7469 6f6e 2068 6173 2061 2066  llection has a f
-00006610: 6561 7475 7265 2074 6f20 7265 636f 7665  eature to recove
-00006620: 7220 6576 656e 7473 2e20 416c 6c20 6576  r events. All ev
-00006630: 656e 7473 2074 6861 7420 6172 6520 6e6f  ents that are no
-00006640: 7420 696e 2074 6865 2072 6563 6569 7665  t in the receive
-00006650: 6420 6461 7461 2073 7472 6561 6d2c 2062  d data stream, b
-00006660: 7574 2077 6869 6368 2061 7265 0a20 2020  ut which are.   
-00006670: 2020 2020 2020 2072 6566 6572 656e 6365         reference
-00006680: 6420 7769 6c6c 2062 6520 6c6f 6164 6564  d will be loaded
-00006690: 2066 726f 6d20 7468 6520 6461 7461 2073   from the data s
-000066a0: 6f75 7263 652e 0a20 2020 2020 2020 202a  ource..        *
-000066b0: 2059 6f75 2063 616e 2074 616b 6520 6064   You can take `d
-000066c0: 6574 6163 6865 645f 6576 656e 7473 6020  etached_events` 
-000066d0: 746f 2073 6565 2077 6869 6368 2065 7665  to see which eve
-000066e0: 6e74 7320 6172 6520 6d69 7373 696e 672e  nts are missing.
-000066f0: 0a20 2020 2020 2020 202a 2049 6620 796f  .        * If yo
-00006700: 7520 7761 6e74 2c20 796f 7520 6361 6e20  u want, you can 
-00006710: 6275 696c 6420 7061 7265 6e74 6c65 7373  build parentless
-00006720: 2074 7265 6573 2077 6865 7265 2074 6865   trees where the
-00006730: 206d 6973 7369 6e67 2065 7665 6e74 7320   missing events 
-00006740: 6172 6520 7374 7562 6265 6420 696e 7374  are stubbed inst
-00006750: 6561 642e 204a 7573 740a 2020 2020 2020  ead. Just.      
-00006760: 2020 2020 7573 6520 6067 6574 5f70 6172      use `get_par
-00006770: 656e 746c 6573 735f 7472 6565 7328 2960  entless_trees()`
-00006780: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00006790: 2020 2052 6571 7569 7265 6d65 6e74 733a     Requirements:
-000067a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000067b0: 2020 312e 2045 7665 6e74 7320 7072 6f76    1. Events prov
-000067c0: 6964 6564 2074 6f20 4554 4320 6861 7665  ided to ETC have
-000067d0: 2074 6f20 6861 7665 2060 6576 656e 745f   to have `event_
-000067e0: 6e61 6d65 602c 2060 6576 656e 745f 6964  name`, `event_id
-000067f0: 602c 2060 7061 7265 6e74 5f65 7665 6e74  `, `parent_event
-00006800: 5f69 6460 2066 6965 6c64 732e 2054 6865  _id` fields. The
-00006810: 7920 0a20 2020 2020 2020 2063 616e 2068  y .        can h
-00006820: 6176 6520 616e 6f74 6865 7220 6e61 6d65  ave another name
-00006830: 7320 2869 7420 7265 736f 6c76 6573 2069  s (it resolves i
-00006840: 6e20 7468 6520 6472 6976 6572 292e 0a20  n the driver).. 
-00006850: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006860: 2323 2323 2048 696e 7473 0a20 2020 2020  #### Hints.     
-00006870: 2020 200a 2020 2020 2020 2020 2a20 5265     .        * Re
-00006880: 6d6f 7665 2061 6c6c 2075 6e6e 6563 6573  move all unneces
-00006890: 7361 7279 2066 6965 6c64 7320 6672 6f6d  sary fields from
-000068a0: 2065 7665 6e74 7320 6265 666f 7265 2070   events before p
-000068b0: 6173 7369 6e67 2074 6f20 6120 5f63 6f6c  assing to a _col
-000068c0: 6c65 6374 696f 6e5f 2074 6f20 7265 6475  lection_ to redu
-000068d0: 6365 206d 656d 6f72 7920 7573 6167 652e  ce memory usage.
-000068e0: 0a20 2020 2020 2020 202a 2055 7365 2060  .        * Use `
-000068f0: 7368 6f77 2829 6020 6d65 7468 6f64 2074  show()` method t
-00006900: 6f20 7072 696e 7420 7468 6520 7472 6565  o print the tree
-00006910: 2069 6e20 7472 6565 2d6c 696b 6520 7669   in tree-like vi
-00006920: 6577 2e0a 2020 2020 2020 2020 2a20 4e6f  ew..        * No
-00006930: 7465 2074 6861 7420 7468 6520 6067 6574  te that the `get
-00006940: 5f78 6020 6d65 7468 6f64 7320 7769 6c6c  _x` methods will
-00006950: 2072 6169 7365 2061 6e20 6578 6365 7074   raise an except
-00006960: 696f 6e20 6966 2079 6f75 2070 6173 7320  ion if you pass 
-00006970: 616e 2075 6e6b 6e6f 776e 2065 7665 6e74  an unknown event
-00006980: 2069 642c 2075 6e6c 696b 6520 7468 6520   id, unlike the 
-00006990: 6066 696e 645f 7860 206d 6574 686f 6473  `find_x` methods
-000069a0: 2028 0a20 2020 2020 2020 2020 2074 6865   (.          the
-000069b0: 7920 7265 7475 726e 204e 6f6e 6529 2e0a  y return None)..
-000069c0: 2020 2020 2020 2020 2a20 4966 2079 6f75          * If you
-000069d0: 2077 616e 7420 746f 206b 6e6f 7720 7468   want to know th
-000069e0: 6174 2073 7065 6369 6669 6564 2065 7665  at specified eve
-000069f0: 6e74 2065 7869 7374 732c 2075 7365 2074  nt exists, use t
-00006a00: 6865 2070 7974 686f 6e20 6069 6e60 206b  he python `in` k
-00006a10: 6579 776f 7264 2028 652e 672e 2060 2765  eyword (e.g. `'e
-00006a20: 7665 6e74 2d69 6427 2069 6e20 6576 656e  vent-id' in even
-00006a30: 7473 5f74 7265 6560 292e 0a20 2020 2020  ts_tree`)..     
-00006a40: 2020 202a 2055 7365 2074 6865 2070 7974     * Use the pyt
-00006a50: 686f 6e20 606c 656e 6020 6b65 7977 6f72  hon `len` keywor
-00006a60: 6420 746f 2067 6574 2065 7665 6e74 7320  d to get events 
-00006a70: 6e75 6d62 6572 2069 6e20 7468 6520 7472  number in the tr
-00006a80: 6565 2e0a 2020 2020 2020 2020 0a20 2020  ee..        .   
-00006a90: 2020 2020 2023 2323 2046 6965 6c64 7352       ### FieldsR
-00006aa0: 6573 6f6c 7665 720a 2020 2020 2020 2020  esolver.        
-00006ab0: 5468 6520 6964 6561 206f 6620 7573 696e  The idea of usin
-00006ac0: 6720 7265 736f 6c76 6572 733a 2020 0a20  g resolvers:  . 
-00006ad0: 2020 2020 2020 2049 7420 736f 6c76 6573         It solves
-00006ae0: 2074 6865 2070 726f 626c 656d 206f 6620   the problem of 
-00006af0: 6861 7669 6e67 2061 2066 6577 2044 6174  having a few Dat
-00006b00: 6153 6f75 7263 6573 2077 6974 6820 7468  aSources with th
-00006b10: 6520 7361 6d65 2064 6174 612c 200a 2020  e same data, .  
-00006b20: 2020 2020 2020 6275 7420 7769 7468 2064        but with d
-00006b30: 6966 6665 7265 6e74 2077 6179 7320 746f  ifferent ways to
-00006b40: 2067 6574 2069 742e 0a20 2020 2020 2020   get it..       
-00006b50: 200a 2020 2020 2020 2020 5468 6573 6520   .        These 
-00006b60: 636c 6173 7365 7320 7072 6f76 6964 6520  classes provide 
-00006b70: 796f 7520 6765 7474 6572 206d 6574 686f  you getter metho
-00006b80: 6473 2e20 0a20 2020 2020 2020 2055 7369  ds. .        Usi
-00006b90: 6e67 2074 6865 7365 2063 6c61 7373 6573  ng these classes
-00006ba0: 2061 6c6c 6f77 7320 796f 7520 746f 2066   allows you to f
-00006bb0: 7265 656c 7920 7377 6974 6368 2062 6574  reely switch bet
-00006bc0: 7765 656e 2064 6966 6665 7265 6e74 2064  ween different d
-00006bd0: 6174 6120 0a20 2020 2020 2020 2066 6f72  ata .        for
-00006be0: 6d61 7473 2061 6e64 2064 6f6e 2774 2063  mats and don't c
-00006bf0: 6861 6e67 6520 796f 7572 2063 6f64 652e  hange your code.
-00006c00: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
-00006c10: 2020 2052 6573 6f6c 7665 7273 2073 6f6c     Resolvers sol
-00006c20: 7665 2074 6865 2070 726f 626c 656d 206f  ve the problem o
-00006c30: 6620 6461 7461 2d66 6f72 6d61 7420 6d69  f data-format mi
-00006c40: 6772 6174 696f 6e2e 2020 0a20 2020 2020  gration.  .     
-00006c50: 2020 202d 2066 6965 6c64 7320 706c 6163     - fields plac
-00006c60: 6520 6361 6e20 6265 2063 6861 6e67 6564  e can be changed
-00006c70: 0a20 2020 2020 2020 202d 2066 6965 6c64  .        - field
-00006c80: 7320 6e61 6d65 7320 6361 6e20 6265 2063  s names can be c
-00006c90: 6861 6e67 6564 0a20 2020 2020 2020 200a  hanged.        .
-00006ca0: 2020 2020 2020 2020 5265 736f 6c76 6572          Resolver
-00006cb0: 7320 6361 6e20 776f 726b 206f 6e6c 7920  s can work only 
-00006cc0: 7769 7468 206f 6e65 2065 7665 6e74 2f6d  with one event/m
-00006cd0: 6573 7361 6765 2e20 0a20 2020 2020 2020  essage. .       
-00006ce0: 2049 7420 6d65 616e 732c 2069 6620 796f   It means, if yo
-00006cf0: 7572 206d 6573 7361 6765 2068 6173 2073  ur message has s
-00006d00: 7562 2d6d 6573 7361 6765 7320 6974 2077  ub-messages it w
-00006d10: 6f6e 2774 2077 6f72 6b2c 2062 6563 6175  on't work, becau
-00006d20: 7365 2072 6573 6f6c 7665 7220 7769 6c6c  se resolver will
-00006d30: 206e 6f74 200a 2020 2020 2020 2020 6b6e   not .        kn
-00006d40: 6f77 2077 6974 6820 7768 6963 6820 7375  ow with which su
-00006d50: 622d 6d65 7373 6167 6520 7368 6f75 6c64  b-message should
-00006d60: 2069 7420 776f 726b 2e20 0a20 2020 2020   it work. .     
-00006d70: 2020 200a 2020 2020 2020 2020 496d 706c     .        Impl
-00006d80: 656d 656e 7461 7469 6f6e 2061 6476 6963  ementation advic
-00006d90: 653a 0a20 2020 2020 2020 2031 2e20 7261  e:.        1. ra
-00006da0: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
-00006db0: 6564 4572 726f 7220 2d2d 2069 6620 796f  edError -- if yo
-00006dc0: 7572 2049 6d70 6c65 6d65 6e74 6174 696f  ur Implementatio
-00006dd0: 6e20 646f 6573 6e27 7420 7375 7070 6f72  n doesn't suppor
-00006de0: 7420 7468 6973 2067 6574 7465 722e 0a20  t this getter.. 
-00006df0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006e00: 5065 7266 6f72 6d61 6e63 6520 696d 7061  Performance impa
-00006e10: 6374 3a0a 2020 2020 2020 2020 2d20 4974  ct:.        - It
-00006e20: 2061 2062 6974 2073 6c6f 7765 7220 7468   a bit slower th
-00006e30: 616e 2075 7369 6e67 206e 616b 6564 2066  an using naked f
-00006e40: 6965 6c64 2061 6363 6573 7320 6064 6963  ield access `dic
-00006e50: 745b 276b 6579 275d 602e 200a 2020 2020  t['key']`. .    
-00006e60: 2020 2020 0a20 2020 2020 2020 2023 2320      .        ## 
-00006e70: 322e 342e 204c 696e 6b73 0a20 2020 2020  2.4. Links.     
-00006e80: 2020 200a 2020 2020 2020 2020 2d20 5b52     .        - [R
-00006e90: 6570 6f72 7420 4461 7461 2050 726f 7669  eport Data Provi
-00006ea0: 6465 725d 2868 7474 7073 3a2f 2f67 6974  der](https://git
-00006eb0: 6875 622e 636f 6d2f 7468 322d 6e65 742f  hub.com/th2-net/
-00006ec0: 7468 322d 7270 742d 6461 7461 2d70 726f  th2-rpt-data-pro
-00006ed0: 7669 6465 7229 0a20 2020 2020 2020 202d  vider).        -
-00006ee0: 205b 5468 3220 4461 7461 2053 6572 7669   [Th2 Data Servi
-00006ef0: 6365 7320 5574 696c 735d 2868 7474 7073  ces Utils](https
-00006f00: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
-00006f10: 322d 6e65 742f 7468 322d 6461 7461 2d73  2-net/th2-data-s
-00006f20: 6572 7669 6365 732d 7574 696c 7329 0a20  ervices-utils). 
-00006f30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006f40: 2320 332e 2042 6573 7420 7072 6163 7469  # 3. Best practi
-00006f50: 6365 730a 2020 2020 2020 2020 4465 7065  ces.        Depe
-00006f60: 6e64 696e 6720 6f6e 2068 6f77 2079 6f75  nding on how you
-00006f70: 2077 6f72 6b20 7769 7468 2060 4461 7461   work with `Data
-00006f80: 206f 626a 6563 7460 2c20 6974 2063 616e   object`, it can
-00006f90: 2062 6520 736c 6f77 206f 6620 6661 7374   be slow of fast
-00006fa0: 2e20 200a 2020 2020 2020 2020 4173 2077  .  .        As w
-00006fb0: 6974 6820 6120 7265 6c61 7469 6f6e 616c  ith a relational
-00006fc0: 2064 6174 6162 6173 652c 2079 6f75 2063   database, you c
-00006fd0: 616e 2077 7269 7465 2061 2071 7565 7279  an write a query
-00006fe0: 2074 6861 7420 7769 6c6c 2072 6574 7572   that will retur
-00006ff0: 6e20 6461 7461 2073 6c6f 776c 7920 6f72  n data slowly or
-00007000: 2071 7569 636b 6c79 2c20 0a20 2020 2020   quickly, .     
-00007010: 2020 2074 6865 2073 616d 6520 7768 656e     the same when
-00007020: 2077 6f72 6b69 6e67 2077 6974 6820 6120   working with a 
-00007030: 6044 6174 6120 6f62 6a65 6374 602e 0a20  `Data object`.. 
-00007040: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007050: 466f 6c6c 6f77 2074 6865 2072 756c 6573  Follow the rules
-00007060: 2074 6f20 6d61 6b65 2079 6f75 7220 776f   to make your wo
-00007070: 726b 2077 6974 6820 4461 7461 206f 626a  rk with Data obj
-00007080: 6563 7420 6661 7374 3a0a 2020 2020 2020  ect fast:.      
-00007090: 2020 312e 2055 7365 2060 4461 7461 2e75    1. Use `Data.u
-000070a0: 7365 5f63 6163 6865 2829 6020 6966 2079  se_cache()` if y
-000070b0: 6f75 2069 7465 7261 7465 2064 6174 6120  ou iterate data 
-000070c0: 6d6f 7265 2074 6861 6e20 6f6e 6520 7469  more than one ti
-000070d0: 6d65 2e0a 2020 2020 2020 2020 322e 2054  me..        2. T
-000070e0: 7279 2074 6f20 646f 6e27 7420 6974 6572  ry to don't iter
-000070f0: 6174 6520 6f6e 6520 6044 6174 6120 6f62  ate one `Data ob
-00007100: 6a65 6374 6020 696e 7369 6465 2074 6865  ject` inside the
-00007110: 206f 7468 6572 206f 6e65 2e20 200a 2020   other one.  .  
-00007120: 2020 2020 2020 2020 2049 6620 796f 7520           If you 
-00007130: 7368 6f75 6c64 2074 6f20 646f 2069 742c  should to do it,
-00007140: 2075 7365 2073 686f 7274 2060 4461 7461   use short `Data
-00007150: 206f 626a 6563 7460 2066 6972 7374 2061   object` first a
-00007160: 6e64 206c 6f6e 6720 6044 6174 6120 6f62  nd long `Data ob
-00007170: 6a65 6374 6020 696e 7369 6465 2074 6865  ject` inside the
-00007180: 206c 6f6f 702e 2020 0a20 2020 2020 2020   loop.  .       
-00007190: 2020 2020 4974 276c 6c20 616c 6c6f 7720      It'll allow 
-000071a0: 796f 7520 6f70 656e 2074 6865 2063 6163  you open the cac
-000071b0: 6865 2066 696c 6520 6f72 2063 7265 6174  he file or creat
-000071c0: 6520 6120 7265 7175 6573 7420 746f 2060  e a request to `
-000071d0: 4461 7461 2073 6f75 7263 6560 206c 6573  Data source` les
-000071e0: 7320 6e75 6d62 6572 206f 6620 7469 6d65  s number of time
-000071f0: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
-00007200: 2020 2020 2320 342e 204f 6666 6963 6961      # 4. Officia
-00007210: 6c20 4461 7461 536f 7572 6365 2069 6d70  l DataSource imp
-00007220: 6c65 6d65 6e74 6174 696f 6e73 0a20 2020  lementations.   
-00007230: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-00007240: 5b4c 6967 6874 7765 6967 6874 2044 6174  [Lightweight Dat
-00007250: 6120 5072 6f76 6964 6572 2044 6174 6120  a Provider Data 
-00007260: 536f 7572 6365 5d28 6874 7470 733a 2f2f  Source](https://
-00007270: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
-00007280: 6574 2f74 6832 2d64 732d 736f 7572 6365  et/th2-ds-source
-00007290: 2d6c 7764 7029 0a20 2020 2020 2020 200a  -lwdp).        .
-000072a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000072b0: 2023 2035 2e20 4150 490a 2020 2020 2020   # 5. API.      
-000072c0: 2020 0a20 2020 2020 2020 2049 6620 796f    .        If yo
-000072d0: 7520 6172 6520 6c6f 6f6b 696e 6720 666f  u are looking fo
-000072e0: 7220 636c 6173 7365 7320 6465 7363 7269  r classes descri
-000072f0: 7074 696f 6e20 7365 6520 7468 6520 5b41  ption see the [A
-00007300: 5049 2044 6f63 756d 656e 7461 7469 6f6e  PI Documentation
-00007310: 5d28 646f 6375 6d65 6e74 6174 696f 6e2f  ](documentation/
-00007320: 6170 692f 696e 6465 782e 6d64 292e 0a20  api/index.md).. 
-00007330: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007340: 2320 362e 2045 7861 6d70 6c65 730a 2020  # 6. Examples.  
-00007350: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
-00007360: 205b 6765 745f 7374 6172 7465 645f 6578   [get_started_ex
-00007370: 616d 706c 652e 7079 5d28 6578 616d 706c  ample.py](exampl
-00007380: 6573 2f67 6574 5f73 7461 7274 6564 5f65  es/get_started_e
-00007390: 7861 6d70 6c65 2e70 7929 0a20 2020 2020  xample.py).     
-000073a0: 2020 200a 506c 6174 666f 726d 3a20 554e     .Platform: UN
-000073b0: 4b4e 4f57 4e0a 5265 7175 6972 6573 2d50  KNOWN.Requires-P
-000073c0: 7974 686f 6e3a 203e 3d33 2e37 0a44 6573  ython: >=3.7.Des
-000073d0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-000073e0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-000073f0: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
-00007400: 7472 613a 2072 6470 0a50 726f 7669 6465  tra: rdp.Provide
-00007410: 732d 4578 7472 613a 2072 6470 350a 5072  s-Extra: rdp5.Pr
-00007420: 6f76 6964 6573 2d45 7874 7261 3a20 7264  ovides-Extra: rd
-00007430: 7036 0a50 726f 7669 6465 732d 4578 7472  p6.Provides-Extr
-00007440: 613a 206c 7764 700a 5072 6f76 6964 6573  a: lwdp.Provides
-00007450: 2d45 7874 7261 3a20 6c77 6470 310a 5072  -Extra: lwdp1.Pr
-00007460: 6f76 6964 6573 2d45 7874 7261 3a20 6c77  ovides-Extra: lw
-00007470: 6470 320a 5072 6f76 6964 6573 2d45 7874  dp2.Provides-Ext
-00007480: 7261 3a20 6c77 6470 2d64 6576 0a50 726f  ra: lwdp-dev.Pro
-00007490: 7669 6465 732d 4578 7472 613a 2075 7469  vides-Extra: uti
-000074a0: 6c73 2d72 7074 2d76 6965 7765 720a 5072  ls-rpt-viewer.Pr
-000074b0: 6f76 6964 6573 2d45 7874 7261 3a20 7574  ovides-Extra: ut
-000074c0: 696c 732d 7270 742d 7669 6577 6572 350a  ils-rpt-viewer5.
-000074d0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000074e0: 7574 696c 732d 6164 7661 6e63 6564 0a    utils-advanced.
+00003ee0: 332e 332e 315d 2047 6574 206c 6561 7665  3.3.1] Get leave
+00003ef0: 7320 6f66 2061 6c6c 2074 7265 6573 2e0a  s of all trees..
+00003f00: 2020 2020 2020 2020 6c65 6176 6573 3a20          leaves: 
+00003f10: 5475 706c 655b 6469 6374 5d20 3d20 6574  Tuple[dict] = et
+00003f20: 632e 6765 745f 6c65 6176 6573 2829 0a20  c.get_leaves(). 
+00003f30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003f40: 2320 5b33 2e33 2e32 5d20 4765 7420 726f  # [3.3.2] Get ro
+00003f50: 6f74 7320 6964 7320 6f66 2061 6c6c 2074  ots ids of all t
+00003f60: 7265 6573 2e0a 2020 2020 2020 2020 726f  rees..        ro
+00003f70: 6f74 733a 204c 6973 745b 7374 725d 203d  ots: List[str] =
+00003f80: 2065 7463 2e67 6574 5f72 6f6f 7473 5f69   etc.get_roots_i
+00003f90: 6473 2829 0a20 2020 2020 2020 200a 2020  ds().        .  
+00003fa0: 2020 2020 2020 2320 5b33 2e33 2e33 5d20        # [3.3.3] 
+00003fb0: 4669 6e64 2061 6e20 6576 656e 7420 696e  Find an event in
+00003fc0: 2061 6c6c 2074 7265 6573 2e0a 2020 2020   all trees..    
+00003fd0: 2020 2020 6669 6e64 5f65 7665 6e74 3a20      find_event: 
+00003fe0: 4f70 7469 6f6e 616c 5b64 6963 745d 203d  Optional[dict] =
+00003ff0: 2065 7463 2e66 696e 6428 6c61 6d62 6461   etc.find(lambda
+00004000: 2065 7665 6e74 3a20 2253 656e 6420 6d65   event: "Send me
+00004010: 7373 6167 6522 2069 6e20 6576 656e 745b  ssage" in event[
+00004020: 2265 7665 6e74 5479 7065 225d 290a 2020  "eventType"]).  
+00004030: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00004040: 205b 332e 332e 345d 2046 696e 6420 616c   [3.3.4] Find al
+00004050: 6c20 6576 656e 7473 2069 6e20 616c 6c20  l events in all 
+00004060: 7472 6565 732e 2054 6865 7265 2069 7320  trees. There is 
+00004070: 616c 736f 2069 7465 7261 626c 6520 7665  also iterable ve
+00004080: 7273 696f 6e20 2766 696e 6461 6c6c 5f69  rsion 'findall_i
+00004090: 7465 7227 2e0a 2020 2020 2020 2020 6669  ter'..        fi
+000040a0: 6e64 5f65 7665 6e74 733a 204c 6973 745b  nd_events: List[
+000040b0: 6469 6374 5d20 3d20 6574 632e 6669 6e64  dict] = etc.find
+000040c0: 616c 6c28 6c61 6d62 6461 2065 7665 6e74  all(lambda event
+000040d0: 3a20 6576 656e 745b 2273 7563 6365 7373  : event["success
+000040e0: 6675 6c22 5d20 6973 2054 7275 6529 0a20  ful"] is True). 
+000040f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00004100: 2320 5b33 2e33 2e35 5d20 4669 6e64 2061  # [3.3.5] Find a
+00004110: 6e20 616e 6365 7374 6f72 206f 6620 7468  n ancestor of th
+00004120: 6520 6576 656e 742e 0a20 2020 2020 2020  e event..       
+00004130: 2061 6e63 6573 746f 723a 204f 7074 696f   ancestor: Optio
+00004140: 6e61 6c5b 6469 6374 5d20 3d20 6574 632e  nal[dict] = etc.
+00004150: 6669 6e64 5f61 6e63 6573 746f 7228 0a20  find_ancestor(. 
+00004160: 2020 2020 2020 2020 2020 2022 3862 6265             "8bbe
+00004170: 3337 3137 2d63 6635 392d 3131 6562 2d61  3717-cf59-11eb-a
+00004180: 3366 372d 3039 3466 3930 3463 3361 3632  3f7-094f904c3a62
+00004190: 222c 2066 696c 7465 723d 6c61 6d62 6461  ", filter=lambda
+000041a0: 2065 7665 6e74 3a20 2252 6f6f 7445 7665   event: "RootEve
+000041b0: 6e74 2220 696e 2065 7665 6e74 5b22 6576  nt" in event["ev
+000041c0: 656e 744e 616d 6522 5d0a 2020 2020 2020  entName"].      
+000041d0: 2020 290a 2020 2020 2020 2020 0a20 2020    ).        .   
+000041e0: 2020 2020 2023 205b 332e 332e 365d 2047       # [3.3.6] G
+000041f0: 6574 2063 6869 6c64 7265 6e20 6f66 2074  et children of t
+00004200: 6865 2065 7665 6e74 2e20 5468 6572 6520  he event. There 
+00004210: 6973 2061 6c73 6f20 6974 6572 6162 6c65  is also iterable
+00004220: 2076 6572 7369 6f6e 2027 6765 745f 6368   version 'get_ch
+00004230: 696c 6472 656e 5f69 7465 7227 2e0a 2020  ildren_iter'..  
+00004240: 2020 2020 2020 6368 696c 6472 656e 3a20        children: 
+00004250: 5475 706c 655b 6469 6374 5d20 3d20 6574  Tuple[dict] = et
+00004260: 632e 6765 745f 6368 696c 6472 656e 2822  c.get_children("
+00004270: 3831 3434 3232 6531 2d39 6336 382d 3131  814422e1-9c68-11
+00004280: 6562 2d38 3539 382d 3639 3165 6264 3766  eb-8598-691ebd7f
+00004290: 3431 3364 2229 0a20 2020 2020 2020 200a  413d").        .
+000042a0: 2020 2020 2020 2020 2320 5b33 2e33 2e37          # [3.3.7
+000042b0: 5d20 4765 7420 7375 6274 7265 6520 666f  ] Get subtree fo
+000042c0: 7220 7370 6563 6966 6965 6420 6576 656e  r specified even
+000042d0: 742e 0a20 2020 2020 2020 2073 7562 7472  t..        subtr
+000042e0: 6565 3a20 4576 656e 7454 7265 6520 3d20  ee: EventTree = 
+000042f0: 6574 632e 6765 745f 7375 6274 7265 6528  etc.get_subtree(
+00004300: 2238 6532 3337 3734 642d 6366 3539 2d31  "8e23774d-cf59-1
+00004310: 3165 622d 6136 6533 2d35 3562 6664 6232  1eb-a6e3-55bfdb2
+00004320: 6233 6632 3122 290a 2020 2020 2020 2020  b3f21").        
+00004330: 0a20 2020 2020 2020 2023 205b 332e 332e  .        # [3.3.
+00004340: 385d 2047 6574 2066 756c 6c20 7061 7468  8] Get full path
+00004350: 2074 6f20 7468 6520 6576 656e 742e 0a20   to the event.. 
+00004360: 2020 2020 2020 2023 204c 6f6f 6b73 206c         # Looks l
+00004370: 696b 6520 5b61 6e63 6573 746f 725f 726f  ike [ancestor_ro
+00004380: 6f74 2c20 616e 6365 7374 6f72 5f6c 6576  ot, ancestor_lev
+00004390: 656c 312c 2061 6e63 6573 746f 725f 6c65  el1, ancestor_le
+000043a0: 7665 6c32 2c20 6576 656e 745d 0a20 2020  vel2, event].   
+000043b0: 2020 2020 2065 7665 6e74 5f70 6174 683a       event_path:
+000043c0: 204c 6973 745b 6469 6374 5d20 3d20 6574   List[dict] = et
+000043d0: 632e 6765 745f 6675 6c6c 5f70 6174 6828  c.get_full_path(
+000043e0: 2238 6532 3532 3466 612d 6366 3539 2d31  "8e2524fa-cf59-1
+000043f0: 3165 622d 6133 6637 2d30 3934 6639 3034  1eb-a3f7-094f904
+00004400: 6333 6136 3222 290a 2020 2020 2020 2020  c3a62").        
+00004410: 0a20 2020 2020 2020 2023 205b 332e 332e  .        # [3.3.
+00004420: 395d 2047 6574 2070 6172 656e 7420 6f66  9] Get parent of
+00004430: 2074 6865 2065 7665 6e74 2e0a 2020 2020   the event..    
+00004440: 2020 2020 7061 7265 6e74 203d 2065 7463      parent = etc
+00004450: 2e67 6574 5f70 6172 656e 7428 2238 6532  .get_parent("8e2
+00004460: 3532 3466 612d 6366 3539 2d31 3165 622d  524fa-cf59-11eb-
+00004470: 6133 6637 2d30 3934 6639 3034 6333 6136  a3f7-094f904c3a6
+00004480: 3222 290a 2020 2020 2020 2020 0a20 2020  2").        .   
+00004490: 2020 2020 2023 205b 332e 332e 3130 5d20       # [3.3.10] 
+000044a0: 4170 7065 6e64 206e 6577 2065 7665 6e74  Append new event
+000044b0: 2074 6f20 7468 6520 636f 6c6c 6563 7469   to the collecti
+000044c0: 6f6e 2e0a 2020 2020 2020 2020 6574 632e  on..        etc.
+000044d0: 6170 7065 6e64 5f65 7665 6e74 280a 2020  append_event(.  
+000044e0: 2020 2020 2020 2020 2020 6576 656e 743d            event=
+000044f0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00004500: 2020 2265 7665 6e74 4964 223a 2022 6132    "eventId": "a2
+00004510: 3066 3565 6634 2d63 3366 652d 6262 3130  0f5ef4-c3fe-bb10
+00004520: 2d61 3239 632d 6464 3364 3738 3439 3039  -a29c-dd3d784909
+00004530: 6562 222c 0a20 2020 2020 2020 2020 2020  eb",.           
+00004540: 2020 2020 2022 7061 7265 6e74 4576 656e       "parentEven
+00004550: 7449 6422 3a20 2238 6532 3532 3466 612d  tId": "8e2524fa-
+00004560: 6366 3539 2d31 3165 622d 6133 6637 2d30  cf59-11eb-a3f7-0
+00004570: 3934 6639 3034 6333 6136 3222 2c0a 2020  94f904c3a62",.  
+00004580: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00004590: 7665 6e74 4e61 6d65 223a 2022 5374 7562  ventName": "Stub
+000045a0: 4576 656e 7422 2c0a 2020 2020 2020 2020  Event",.        
+000045b0: 2020 2020 7d0a 2020 2020 2020 2020 290a      }.        ).
+000045c0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000045d0: 2023 205b 332e 332e 3131 5d20 5368 6f77   # [3.3.11] Show
+000045e0: 2074 6865 2065 6e74 6972 6520 636f 6c6c   the entire coll
+000045f0: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
+00004600: 6574 632e 7368 6f77 2829 0a20 2020 2020  etc.show().     
+00004610: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
+00004620: 2e34 5d20 576f 726b 696e 6720 7769 7468  .4] Working with
+00004630: 2074 6865 2045 7665 6e74 5472 6565 2e0a   the EventTree..
+00004640: 2020 2020 2020 2020 2320 4576 656e 7454          # EventT
+00004650: 7265 6520 6861 7320 7468 6520 7361 6d65  ree has the same
+00004660: 206d 6574 686f 6473 2061 7320 4576 656e   methods as Even
+00004670: 7454 7265 6543 6f6c 6c65 6374 696f 6e2c  tTreeCollection,
+00004680: 2062 7574 206f 6e6c 7920 666f 7220 6974   but only for it
+00004690: 7320 6f77 6e20 7472 6565 2e0a 2020 2020  s own tree..    
+000046a0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
+000046b0: 332e 342e 315d 2047 6574 2063 6f6c 6c65  3.4.1] Get colle
+000046c0: 6374 696f 6e20 7472 6565 732e 0a20 2020  ction trees..   
+000046d0: 2020 2020 2074 7265 6573 3a20 4c69 7374       trees: List
+000046e0: 5b45 7665 6e74 5472 6565 5d20 3d20 6574  [EventTree] = et
+000046f0: 632e 6765 745f 7472 6565 7328 290a 2020  c.get_trees().  
+00004700: 2020 2020 2020 7472 6565 3a20 4576 656e        tree: Even
+00004710: 7454 7265 6520 3d20 7472 6565 735b 305d  tTree = trees[0]
+00004720: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00004730: 2020 2320 4275 7420 4576 656e 7454 7265    # But EventTre
+00004740: 6520 7072 6f76 6964 6573 2061 2077 6f72  e provides a wor
+00004750: 6b20 7769 7468 2074 6865 2074 7265 652c  k with the tree,
+00004760: 2062 7574 2064 6f65 7320 6e6f 7420 6d6f   but does not mo
+00004770: 6469 6679 2069 742e 0a20 2020 2020 2020  dify it..       
+00004780: 2023 2049 6620 796f 7520 7761 6e74 2074   # If you want t
+00004790: 6f20 6d6f 6469 6679 2074 6865 2074 7265  o modify the tre
+000047a0: 652c 2075 7365 2045 7665 6e74 5472 6565  e, use EventTree
+000047b0: 436f 6c6c 6563 7469 6f6e 732e 0a20 2020  Collections..   
+000047c0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+000047d0: 5b33 2e35 5d20 576f 726b 696e 6720 7769  [3.5] Working wi
+000047e0: 7468 2050 6172 656e 746c 6573 7354 7265  th ParentlessTre
+000047f0: 652e 0a20 2020 2020 2020 2023 2050 6172  e..        # Par
+00004800: 656e 746c 6573 7354 7265 6520 6973 2045  entlessTree is E
+00004810: 7665 6e74 5472 6565 2077 6869 6368 2068  ventTree which h
+00004820: 6173 2064 6574 6163 6865 6420 6576 656e  as detached even
+00004830: 7473 2077 6974 6820 7374 7562 732e 0a20  ts with stubs.. 
+00004840: 2020 2020 2020 2070 6172 656e 746c 6573         parentles
+00004850: 735f 7472 6565 733a 204c 6973 745b 4576  s_trees: List[Ev
+00004860: 656e 7454 7265 655d 203d 2065 7463 2e67  entTree] = etc.g
+00004870: 6574 5f70 6172 656e 746c 6573 735f 7472  et_parentless_tr
+00004880: 6565 7328 290a 2020 2020 2020 2020 0a20  ees().        . 
+00004890: 2020 2020 2020 2023 205b 332e 365d 2057         # [3.6] W
+000048a0: 6f72 6b69 6e67 2077 6974 6820 5061 7265  orking with Pare
+000048b0: 6e74 4576 656e 7454 7265 6543 6f6c 6c65  ntEventTreeColle
+000048c0: 6374 696f 6e2e 0a20 2020 2020 2020 2023  ction..        #
+000048d0: 2050 6172 656e 7445 7665 6e74 5472 6565   ParentEventTree
+000048e0: 436f 6c6c 6563 7469 6f6e 2069 7320 6120  Collection is a 
+000048f0: 7472 6565 2063 6f6c 6c65 6374 696f 6e20  tree collection 
+00004900: 6c69 6b65 2045 7665 6e74 5472 6565 436f  like EventTreeCo
+00004910: 6c6c 6563 7469 6f6e 2c0a 2020 2020 2020  llection,.      
+00004920: 2020 2320 6275 7420 6974 2068 6173 206f    # but it has o
+00004930: 6e6c 7920 6576 656e 7473 2074 6861 7420  nly events that 
+00004940: 6861 7665 2072 6566 6572 656e 6365 732e  have references.
+00004950: 0a20 2020 2020 2020 2064 6174 615f 736f  .        data_so
+00004960: 7572 6365 3a20 4944 6174 6153 6f75 7263  urce: IDataSourc
+00004970: 6520 2023 2059 6f75 2073 686f 756c 6420  e  # You should 
+00004980: 696e 6974 2044 6174 6153 6f75 7263 6520  init DataSource 
+00004990: 6f62 6a65 6374 2e20 452e 672e 2066 726f  object. E.g. fro
+000049a0: 6d20 4c77 4450 206d 6f64 756c 652e 0a20  m LwDP module.. 
+000049b0: 2020 2020 2020 2023 2045 5443 4472 6976         # ETCDriv
+000049c0: 6572 2068 6572 6520 6973 2061 2073 7475  er here is a stu
+000049d0: 622c 2061 6374 7561 6c6c 7920 7468 6520  b, actually the 
+000049e0: 6c69 6220 646f 6e27 7420 6861 7665 2073  lib don't have s
+000049f0: 7563 6820 636c 6173 732e 0a20 2020 2020  uch class..     
+00004a00: 2020 2023 2059 6f75 2063 616e 2074 616b     # You can tak
+00004a10: 6520 6974 2069 6e20 4c77 4450 206d 6f64  e it in LwDP mod
+00004a20: 756c 6520 6f72 2063 7265 6174 6520 796f  ule or create yo
+00004a30: 7572 7365 6c66 2063 6c61 7373 2069 6620  urself class if 
+00004a40: 796f 7520 6861 7665 2073 6f6d 6520 7370  you have some sp
+00004a50: 6563 6961 6c20 6576 656e 7473 2073 7472  ecial events str
+00004a60: 7563 7475 7265 2e0a 2020 2020 2020 2020  ucture..        
+00004a70: 6472 6976 6572 203d 2045 5443 4472 6976  driver = ETCDriv
+00004a80: 6572 2864 6174 615f 736f 7572 6365 3d64  er(data_source=d
+00004a90: 6174 615f 736f 7572 6365 290a 2020 2020  ata_source).    
+00004aa0: 2020 2020 6574 6320 3d20 5061 7265 6e74      etc = Parent
+00004ab0: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
+00004ac0: 696f 6e28 6472 6976 6572 290a 2020 2020  ion(driver).    
+00004ad0: 2020 2020 6574 632e 6275 696c 6428 6576      etc.build(ev
+00004ae0: 656e 7473 290a 2020 2020 2020 2020 0a20  ents).        . 
+00004af0: 2020 2020 2020 2065 7463 2e73 686f 7728         etc.show(
+00004b00: 290a 2020 2020 2020 2020 6060 600a 2020  ).        ```.  
+00004b10: 2020 2020 2020 3c21 2d2d 2065 6e64 2067        <!-- end g
+00004b20: 6574 5f73 7461 7274 6564 5f65 7861 6d70  et_started_examp
+00004b30: 6c65 2e70 7920 2d2d 3e0a 2020 2020 2020  le.py -->.      
+00004b40: 2020 0a20 2020 2020 2020 2023 2320 322e    .        ## 2.
+00004b50: 332e 2053 686f 7274 2074 6865 6f72 790a  3. Short theory.
+00004b60: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004b70: 2054 6865 206c 6962 7261 7279 2070 726f   The library pro
+00004b80: 7669 6465 7320 746f 6f6c 7320 666f 7220  vides tools for 
+00004b90: 6861 6e64 6c69 6e67 2073 7472 6561 6d20  handling stream 
+00004ba0: 6461 7461 2e20 5768 6174 2773 2061 2073  data. What's a s
+00004bb0: 7472 6561 6d3f 2049 7427 7320 6120 7365  tream? It's a se
+00004bc0: 7175 656e 6365 206f 6620 656c 656d 656e  quence of elemen
+00004bd0: 7473 2066 726f 6d20 6120 736f 7572 6365  ts from a source
+00004be0: 2074 6861 740a 2020 2020 2020 2020 7375   that.        su
+00004bf0: 7070 6f72 7473 2061 6767 7265 6761 7465  pports aggregate
+00004c00: 206f 7065 7261 7469 6f6e 732e 0a20 2020   operations..   
+00004c10: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
+00004c20: 2320 5465 726d 730a 2020 2020 2020 2020  # Terms.        
+00004c30: 0a20 2020 2020 2020 202d 202a 2a44 6174  .        - **Dat
+00004c40: 6120 6f62 6a65 6374 2a2a 3a20 416e 2069  a object**: An i
+00004c50: 6e73 7461 6e63 6520 6f66 2060 4461 7461  nstance of `Data
+00004c60: 6020 636c 6173 7320 7768 6963 6820 6973  ` class which is
+00004c70: 2077 7261 7070 6572 2075 6e64 6572 2073   wrapper under s
+00004c80: 7472 6561 6d2e 0a20 2020 2020 2020 202d  tream..        -
+00004c90: 202a 2a53 6571 7565 6e63 6520 6f66 2065   **Sequence of e
+00004ca0: 6c65 6d65 6e74 732a 2a3a 0a20 2020 2020  lements**:.     
+00004cb0: 2020 2020 2041 205f 4461 7461 206f 626a       A _Data obj
+00004cc0: 6563 745f 2070 726f 7669 6465 7320 616e  ect_ provides an
+00004cd0: 2069 6e74 6572 6661 6365 2074 6f20 6120   interface to a 
+00004ce0: 7365 7175 656e 6365 6420 7365 7420 6f66  sequenced set of
+00004cf0: 2076 616c 7565 7320 6f66 2061 2073 7065   values of a spe
+00004d00: 6369 6669 6320 656c 656d 656e 7420 7479  cific element ty
+00004d10: 7065 2e20 5374 7265 616d 2069 6e73 6964  pe. Stream insid
+00004d20: 6520 7468 6520 5f44 6174 610a 2020 2020  e the _Data.    
+00004d30: 2020 2020 2020 6f62 6a65 6374 5f20 2a2a        object_ **
+00004d40: 646f 6e19 7420 6163 7475 616c 6c79 2073  don.t actually s
+00004d50: 746f 7265 2a2a 2065 6c65 6d65 6e74 733b  tore** elements;
+00004d60: 2074 6865 7920 6172 6520 636f 6d70 7574   they are comput
+00004d70: 6564 206f 6e20 6465 6d61 6e64 2e0a 2020  ed on demand..  
+00004d80: 2020 2020 2020 2d20 2a2a 6461 7461 2073        - **data s
+00004d90: 6f75 7263 652a 2a20 2865 7861 6374 6c79  ource** (exactly
+00004da0: 2069 6e20 736d 616c 6c20 6c65 7474 6572   in small letter
+00004db0: 7329 3a0a 2020 2020 2020 2020 2020 416e  s):.          An
+00004dc0: 7920 736f 7572 6365 206f 6620 6461 7461  y source of data
+00004dd0: 2e20 452e 672e 205b 4c69 6768 7477 6569  . E.g. [Lightwei
+00004de0: 6768 7420 4461 7461 2050 726f 7669 6465  ght Data Provide
+00004df0: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
+00004e00: 622e 636f 6d2f 7468 322d 6e65 742f 7468  b.com/th2-net/th
+00004e10: 322d 6c77 2d64 6174 612d 7072 6f76 6964  2-lw-data-provid
+00004e20: 6572 292c 2063 6f6c 6c65 6374 696f 6e73  er), collections
+00004e30: 2c0a 2020 2020 2020 2020 2020 6172 7261  ,.          arra
+00004e40: 7973 2c20 6f72 2049 2f4f 2072 6573 6f75  ys, or I/O resou
+00004e50: 7263 6573 2e0a 2020 2020 2020 2020 2d20  rces..        - 
+00004e60: 2a2a 4461 7461 536f 7572 6365 2a2a 3a0a  **DataSource**:.
+00004e70: 2020 2020 2020 2020 2020 4120 636c 6173            A clas
+00004e80: 7320 7468 6174 2069 7320 616e 2069 6e74  s that is an int
+00004e90: 6572 6d65 6469 6174 6520 6c69 6e6b 2062  ermediate link b
+00004ea0: 6574 7765 656e 2074 6865 2053 6f75 7263  etween the Sourc
+00004eb0: 6541 5049 2061 6e64 2043 6f6d 6d61 6e64  eAPI and Command
+00004ec0: 732e 0a20 2020 2020 2020 202d 202a 2a53  s..        - **S
+00004ed0: 6f75 7263 6541 5049 2a2a 3a0a 2020 2020  ourceAPI**:.    
+00004ee0: 2020 2020 2020 4561 6368 2073 6f75 7263        Each sourc
+00004ef0: 6520 6861 7320 6974 7320 6f77 6e20 4150  e has its own AP
+00004f00: 4920 746f 2072 6574 7269 6576 6520 6461  I to retrieve da
+00004f10: 7461 2e20 536f 7572 6365 4150 4920 6973  ta. SourceAPI is
+00004f20: 2061 2063 6c61 7373 2074 6861 7420 7072   a class that pr
+00004f30: 6f76 6964 6520 4150 4920 666f 7220 736f  ovide API for so
+00004f40: 6d65 2064 6174 6120 736f 7572 6365 2e0a  me data source..
+00004f50: 2020 2020 2020 2020 2d20 2a2a 436f 6d6d          - **Comm
+00004f60: 616e 6473 2a2a 3a0a 2020 2020 2020 2020  ands**:.        
+00004f70: 2020 436c 6173 7365 7320 7468 6174 2070    Classes that p
+00004f80: 726f 7669 6465 2075 7365 722d 6672 6965  rovide user-frie
+00004f90: 6e64 6c79 2069 6e74 6572 6661 6365 7320  ndly interfaces 
+00004fa0: 666f 7220 6765 7474 696e 6720 736f 6d65  for getting some
+00004fb0: 2064 6174 6120 6672 6f6d 2044 6174 6153   data from DataS
+00004fc0: 6f75 7263 652e 2043 6f6d 6d61 6e64 7320  ource. Commands 
+00004fd0: 7573 6520 5f53 6f75 7263 6541 5049 5f20  use _SourceAPI_ 
+00004fe0: 746f 0a20 2020 2020 2020 2020 2061 6368  to.          ach
+00004ff0: 6965 7665 2069 742e 0a20 2020 2020 2020  ieve it..       
+00005000: 202d 202a 2a41 6461 7074 6572 732a 2a3a   - **Adapters**:
+00005010: 0a20 2020 2020 2020 2020 2049 7427 7320  .          It's 
+00005020: 7369 6d69 6c61 7220 746f 2066 756e 6374  similar to funct
+00005030: 696f 6e20 666f 7220 6044 6174 612e 6d61  ion for `Data.ma
+00005040: 7060 206d 6574 686f 642e 2041 646f 7074  p` method. Adopt
+00005050: 6162 6c65 2063 6f6d 6d61 6e64 7320 7573  able commands us
+00005060: 6564 2069 7420 746f 2075 7064 6174 6520  ed it to update 
+00005070: 7468 6520 6461 7461 2073 7472 6561 6d2e  the data stream.
+00005080: 0a20 2020 2020 2020 202d 202a 2a41 6767  .        - **Agg
+00005090: 7265 6761 7465 206f 7065 7261 7469 6f6e  regate operation
+000050a0: 732a 2a3a 0a20 2020 2020 2020 2020 2043  s**:.          C
+000050b0: 6f6d 6d6f 6e20 6f70 6572 6174 696f 6e73  ommon operations
+000050c0: 2073 7563 6820 6173 2066 696c 7465 722c   such as filter,
+000050d0: 206d 6170 2c20 6c69 6d69 7420 616e 6420   map, limit and 
+000050e0: 736f 206f 6e2e 0a20 2020 2020 2020 202d  so on..        -
+000050f0: 202a 2a57 6f72 6b66 6c6f 772a 2a3a 2041   **Workflow**: A
+00005100: 6e20 6f72 6465 7265 6420 7365 7420 6f66  n ordered set of
+00005110: 205f 4167 6772 6567 6174 6520 6f70 6572   _Aggregate oper
+00005120: 6174 696f 6e73 5f2e 0a20 2020 2020 2020  ations_..       
+00005130: 200a 2020 2020 2020 2020 2323 2320 436f   .        ### Co
+00005140: 6e63 6570 740a 2020 2020 2020 2020 0a20  ncept.        . 
+00005150: 2020 2020 2020 2054 6865 206c 6962 7261         The libra
+00005160: 7279 2064 6573 6372 6962 6573 2074 6865  ry describes the
+00005170: 2068 6967 682d 6c65 7665 6c20 696e 7465   high-level inte
+00005180: 7266 6163 6573 2060 4953 6f75 7263 6541  rfaces `ISourceA
+00005190: 5049 602c 2060 4944 6174 6153 6f75 7263  PI`, `IDataSourc
+000051a0: 6560 2c20 6049 436f 6d6d 616e 6460 2c20  e`, `ICommand`, 
+000051b0: 6049 4164 6170 7465 7260 2e0a 2020 2020  `IAdapter`..    
+000051c0: 2020 2020 0a20 2020 2020 2020 2041 6e79      .        Any
+000051d0: 2064 6174 6120 736f 7572 6365 206d 7573   data source mus
+000051e0: 7420 6265 2064 6573 6372 6962 6564 2062  t be described b
+000051f0: 7920 7468 6520 6049 4461 7461 536f 7572  y the `IDataSour
+00005200: 6365 6020 6162 7374 7261 6374 2063 6c61  ce` abstract cla
+00005210: 7373 2e20 5468 6573 6520 6361 6e20 6265  ss. These can be
+00005220: 205f 4669 6c65 4461 7461 536f 7572 6365   _FileDataSource
+00005230: 5f2c 200a 2020 2020 2020 2020 5f43 5356  _, .        _CSV
+00005240: 4461 7461 536f 7572 6365 5f2c 205f 4442  DataSource_, _DB
+00005250: 4461 7461 536f 7572 6365 5f20 616e 6420  DataSource_ and 
+00005260: 6f74 6865 722e 0a20 2020 2020 2020 200a  other..        .
+00005270: 2020 2020 2020 2020 5573 7561 6c6c 792c          Usually,
+00005280: 2064 6174 6120 736f 7572 6365 7320 6861   data sources ha
+00005290: 7665 2073 6f6d 6520 6b69 6e64 206f 6620  ve some kind of 
+000052a0: 4150 492e 2044 6174 6162 6173 6573 202d  API. Databases -
+000052b0: 2070 726f 7669 6465 2053 514c 206c 616e   provide SQL lan
+000052c0: 6775 6167 652c 2077 6865 6e20 776f 726b  guage, when work
+000052d0: 696e 6720 7769 7468 2061 2066 696c 652c  ing with a file,
+000052e0: 2079 6f75 2063 616e 2072 6561 640a 2020   you can read.  
+000052f0: 2020 2020 2020 6c69 6e65 2062 7920 6c69        line by li
+00005300: 6e65 2c20 6574 632e 2054 6869 7320 4150  ne, etc. This AP
+00005310: 4920 6973 2064 6573 6372 6962 6564 2062  I is described b
+00005320: 7920 7468 6520 6049 536f 7572 6365 4150  y the `ISourceAP
+00005330: 4960 2063 6c61 7373 2e20 4265 6361 7573  I` class. Becaus
+00005340: 6520 6469 6666 6572 656e 7420 7665 7273  e different vers
+00005350: 696f 6e73 206f 6620 7468 6520 7361 6d65  ions of the same
+00005360: 2064 6174 6120 736f 7572 6365 0a20 2020   data source.   
+00005370: 2020 2020 206d 6179 2068 6176 6520 6469       may have di
+00005380: 6666 6572 656e 7420 4150 492c 2069 7420  fferent API, it 
+00005390: 6973 2062 6574 7465 7220 746f 2063 7265  is better to cre
+000053a0: 6174 6520 6120 636c 6173 7320 666f 7220  ate a class for 
+000053b0: 6561 6368 2076 6572 7369 6f6e 2e0a 2020  each version..  
+000053c0: 2020 2020 2020 0a20 2020 2020 2020 2047        .        G
+000053d0: 656e 6572 616c 6c79 2c20 6461 7461 2073  enerally, data s
+000053e0: 6f75 7263 6520 4150 4973 2061 7265 2068  ource APIs are h
+000053f0: 6964 6465 6e20 6265 6869 6e64 2063 6f6e  idden behind con
+00005400: 7665 6e69 656e 7420 696e 7465 7266 6163  venient interfac
+00005410: 6573 2e20 5468 6520 726f 6c65 206f 6620  es. The role of 
+00005420: 7468 6573 6520 696e 7465 7266 6163 6573  these interfaces
+00005430: 2069 7320 706c 6179 6564 0a20 2020 2020   is played.     
+00005440: 2020 2062 7920 6049 436f 6d6d 616e 6460     by `ICommand`
+00005450: 2063 6c61 7373 6573 2e0a 2020 2020 2020   classes..      
+00005460: 2020 0a20 2020 2020 2020 2060 4941 6461    .        `IAda
+00005470: 7074 6572 6020 636c 6173 7365 7320 7472  pter` classes tr
+00005480: 616e 7366 6f72 6d20 6461 7461 2073 7472  ansform data str
+00005490: 6561 6d20 6c69 6b65 2066 756e 6374 696f  eam like functio
+000054a0: 6e73 2066 6f72 2060 4461 7461 2e6d 6170  ns for `Data.map
+000054b0: 6020 6d65 7468 6f64 2e20 4573 7365 6e74  ` method. Essent
+000054c0: 6961 6c6c 7920 6974 2773 2074 6865 2073  ially it's the s
+000054d0: 616d 6520 7468 696e 6720 6275 7420 6d6f  ame thing but mo
+000054e0: 7265 0a20 2020 2020 2020 2066 6c65 7869  re.        flexi
+000054f0: 626c 652e 0a20 2020 2020 2020 200a 2020  ble..        .  
+00005500: 2020 2020 2020 466f 7220 6578 616d 706c        For exampl
+00005510: 652c 204c 7744 5020 4461 7461 536f 7572  e, LwDP DataSour
+00005520: 6365 2868 7474 7073 3a2f 2f67 6974 6875  ce(https://githu
+00005530: 622e 636f 6d2f 7468 322d 6e65 742f 7468  b.com/th2-net/th
+00005540: 322d 6473 2d73 6f75 7263 652d 6c77 6470  2-ds-source-lwdp
+00005550: 2920 7573 6573 2074 6865 7365 2061 6273  ) uses these abs
+00005560: 7472 6163 7420 636c 6173 7365 7320 746f  tract classes to
+00005570: 2062 7569 6c64 2069 7473 2069 6d70 6c65   build its imple
+00005580: 6d65 6e74 6174 696f 6e2e 596f 7520 6361  mentation.You ca
+00005590: 6e20 6561 7369 6c79 2063 7265 6174 6520  n easily create 
+000055a0: 796f 7572 206f 776e 2075 6e69 7175 6520  your own unique 
+000055b0: 636f 6d6d 616e 6473 2066 6f72 205f 4c77  commands for _Lw
+000055c0: 4450 2044 6174 6153 6f75 7263 655f 2c20  DP DataSource_, 
+000055d0: 6173 2077 656c 6c20 6173 2065 6e74 6972  as well as entir
+000055e0: 650a 2020 2020 2020 2020 5f44 6174 6153  e.        _DataS
+000055f0: 6f75 7263 655f 2063 6c61 7373 6573 2e20  ource_ classes. 
+00005600: 5b48 6572 6520 6973 2061 2064 6f63 756d  [Here is a docum
+00005610: 656e 7461 7469 6f6e 5d28 646f 6375 6d65  entation](docume
+00005620: 6e74 6174 696f 6e2f 6461 7461 736f 7572  ntation/datasour
+00005630: 6365 2e6d 6429 206f 6e20 686f 7720 746f  ce.md) on how to
+00005640: 2069 6d70 6c65 6d65 6e74 2074 6865 7365   implement these
+00005650: 2069 6e74 6572 6661 6365 732e 0a20 2020   interfaces..   
+00005660: 2020 2020 200a 2020 2020 2020 2020 215b       .        ![
+00005670: 4461 7461 2073 7472 6561 6d20 7069 7065  Data stream pipe
+00005680: 6c69 6e65 5d28 646f 6375 6d65 6e74 6174  line](documentat
+00005690: 696f 6e2f 696d 672f 636f 6e63 6570 742e  ion/img/concept.
+000056a0: 706e 6729 0a20 2020 2020 2020 200a 2020  png).        .  
+000056b0: 2020 2020 2020 2323 2320 5374 7265 616d        ### Stream
+000056c0: 206f 7065 7261 7469 6f6e 730a 2020 2020   operations.    
+000056d0: 2020 2020 0a20 2020 2020 2020 2046 7572      .        Fur
+000056e0: 7468 6572 6d6f 7265 2c20 7374 7265 616d  thermore, stream
+000056f0: 206f 7065 7261 7469 6f6e 7320 6861 7665   operations have
+00005700: 2074 776f 2066 756e 6461 6d65 6e74 616c   two fundamental
+00005710: 2063 6861 7261 6374 6572 6973 7469 6373   characteristics
+00005720: 2074 6861 7420 6d61 6b65 2074 6865 6d20   that make them 
+00005730: 7665 7279 2064 6966 6665 7265 6e74 2066  very different f
+00005740: 726f 6d20 636f 6c6c 6563 7469 6f6e 0a20  rom collection. 
+00005750: 2020 2020 2020 206f 7065 7261 7469 6f6e         operation
+00005760: 733a 205f 5069 7065 6c69 6e69 6e67 5f20  s: _Pipelining_ 
+00005770: 616e 6420 5f49 6e74 6572 6e61 6c20 6974  and _Internal it
+00005780: 6572 6174 696f 6e5f 2e0a 2020 2020 2020  eration_..      
+00005790: 2020 0a20 2020 2020 2020 2023 2323 2320    .        #### 
+000057a0: 5069 7065 6c69 6e69 6e67 0a20 2020 2020  Pipelining.     
+000057b0: 2020 200a 2020 2020 2020 2020 4d61 6e79     .        Many
+000057c0: 2073 7472 6561 6d20 6f70 6572 6174 696f   stream operatio
+000057d0: 6e73 2072 6574 7572 6e20 6120 7374 7265  ns return a stre
+000057e0: 616d 2074 6865 6d73 656c 7665 732e 2054  am themselves. T
+000057f0: 6869 7320 616c 6c6f 7773 206f 7065 7261  his allows opera
+00005800: 7469 6f6e 7320 746f 2062 6520 6368 6169  tions to be chai
+00005810: 6e65 6420 746f 2066 6f72 6d20 6120 6c61  ned to form a la
+00005820: 7267 6572 2070 6970 656c 696e 652e 0a20  rger pipeline.. 
+00005830: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005840: 215b 4461 7461 2073 7472 6561 6d20 7069  ![Data stream pi
+00005850: 7065 6c69 6e65 5d28 646f 6375 6d65 6e74  peline](document
+00005860: 6174 696f 6e2f 696d 672f 6461 7461 5f73  ation/img/data_s
+00005870: 7472 6561 6d5f 7069 7065 6c69 6e65 2e70  tream_pipeline.p
+00005880: 6e67 290a 2020 2020 2020 2020 0a20 2020  ng).        .   
+00005890: 2020 2020 2023 2323 2320 496e 7465 726e       #### Intern
+000058a0: 616c 2069 7465 7261 7469 6f6e 0a20 2020  al iteration.   
+000058b0: 2020 2020 200a 2020 2020 2020 2020 496e       .        In
+000058c0: 2063 6f6e 7472 6173 7420 746f 2063 6f6c   contrast to col
+000058d0: 6c65 6374 696f 6e73 2c20 7768 6963 6820  lections, which 
+000058e0: 6172 6520 6974 6572 6174 6564 2065 7870  are iterated exp
+000058f0: 6c69 6369 746c 7920 2865 7874 6572 6e61  licitly (externa
+00005900: 6c20 6974 6572 6174 696f 6e29 2c20 7374  l iteration), st
+00005910: 7265 616d 206f 7065 7261 7469 6f6e 7320  ream operations 
+00005920: 646f 2074 6865 2069 7465 7261 7469 6f6e  do the iteration
+00005930: 0a20 2020 2020 2020 2062 6568 696e 6420  .        behind 
+00005940: 7468 6520 7363 656e 6573 2066 6f72 2079  the scenes for y
+00005950: 6f75 2e20 4e6f 7465 2c20 6974 2064 6f65  ou. Note, it doe
+00005960: 736e 2774 206d 6561 6e20 796f 7520 6361  sn't mean you ca
+00005970: 6e6e 6f74 2069 7465 7261 7465 2074 6865  nnot iterate the
+00005980: 205f 4461 7461 206f 626a 6563 745f 2e0a   _Data object_..
+00005990: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000059a0: 2023 2323 2044 6174 6120 6361 6368 696e   ### Data cachin
+000059b0: 670a 2020 2020 2020 2020 0a20 2020 2020  g.        .     
+000059c0: 2020 2054 6865 205f 4461 7461 206f 626a     The _Data obj
+000059d0: 6563 745f 2070 726f 7669 6465 7320 7468  ect_ provides th
+000059e0: 6520 6162 696c 6974 7920 746f 2075 7365  e ability to use
+000059f0: 2074 6865 2063 6163 6865 2e20 5468 6520   the cache. The 
+00005a00: 6361 6368 6520 776f 726b 7320 666f 7220  cache works for 
+00005a10: 6561 6368 205f 4461 7461 206f 626a 6563  each _Data objec
+00005a20: 745f 2c20 7468 6174 2069 732c 2079 6f75  t_, that is, you
+00005a30: 2063 686f 6f73 650a 2020 2020 2020 2020   choose.        
+00005a40: 7768 6963 6820 5f44 6174 6120 6f62 6a65  which _Data obje
+00005a50: 6374 5f20 796f 7520 7761 6e74 2074 6f20  ct_ you want to 
+00005a60: 7361 7665 2e20 5468 6520 5f44 6174 6120  save. The _Data 
+00005a70: 6f62 6a65 6374 5f20 6361 6368 6520 6973  object_ cache is
+00005a80: 2073 6176 6564 2061 6674 6572 2074 6865   saved after the
+00005a90: 2066 6972 7374 2069 7465 7261 7469 6f6e   first iteration
+00005aa0: 2c20 6275 7420 7468 6520 6974 6572 6174  , but the iterat
+00005ab0: 696f 6e0a 2020 2020 2020 2020 736f 7572  ion.        sour
+00005ac0: 6365 206d 6179 2062 6520 6469 6666 6572  ce may be differ
+00005ad0: 656e 742e 0a20 2020 2020 2020 200a 2020  ent..        .  
+00005ae0: 2020 2020 2020 4966 2079 6f75 2064 6f6e        If you don
+00005af0: 2774 2075 7365 2074 6865 2063 6163 6865  't use the cache
+00005b00: 2c20 796f 7572 2073 6f75 7263 6520 7769  , your source wi
+00005b10: 6c6c 2062 6520 7468 6520 6461 7461 2073  ll be the data s
+00005b20: 6f75 7263 6520 796f 7520 6861 7665 2069  ource you have i
+00005b30: 6e20 7468 6520 5f44 6174 6120 4f62 6a65  n the _Data Obje
+00005b40: 6374 5f2e 2042 7574 2069 6620 796f 7520  ct_. But if you 
+00005b50: 7573 6520 7468 6520 6361 6368 652c 0a20  use the cache,. 
+00005b60: 2020 2020 2020 2079 6f75 7220 736f 7572         your sour
+00005b70: 6365 2063 616e 2062 6520 7468 6520 6461  ce can be the da
+00005b80: 7461 2073 6f75 7263 652c 2074 6865 2070  ta source, the p
+00005b90: 6172 656e 7420 6361 6368 652c 206f 7220  arent cache, or 
+00005ba0: 6f77 6e20 6361 6368 653a 0a20 2020 2020  own cache:.     
+00005bb0: 2020 200a 2020 2020 2020 2020 2a20 5468     .        * Th
+00005bc0: 6520 6461 7461 2073 6f75 7263 653a 0a20  e data source:. 
+00005bd0: 2020 2020 2020 2020 2049 6620 7468 6520           If the 
+00005be0: 5f44 6174 6120 4f62 6a65 6374 5f20 646f  _Data Object_ do
+00005bf0: 6573 6e27 7420 6861 7665 2061 2070 6172  esn't have a par
+00005c00: 656e 7420 6361 6368 6520 616e 6420 6974  ent cache and it
+00005c10: 7320 6361 6368 652e 0a20 2020 2020 2020  s cache..       
+00005c20: 202a 2054 6865 2070 6172 656e 7420 6361   * The parent ca
+00005c30: 6368 653a 0a20 2020 2020 2020 2020 2049  che:.          I
+00005c40: 6620 7468 6520 5f44 6174 6120 4f62 6a65  f the _Data Obje
+00005c50: 6374 5f20 6861 7320 6120 7061 7265 6e74  ct_ has a parent
+00005c60: 2063 6163 6865 2e20 4974 2064 6f65 736e   cache. It doesn
+00005c70: 2774 206d 6174 7465 7220 7768 6174 2070  't matter what p
+00005c80: 6f73 6974 696f 6e20 7468 6520 7061 7265  osition the pare
+00005c90: 6e74 2063 6163 6865 2068 6173 2069 6e20  nt cache has in 
+00005ca0: 696e 6865 7269 7461 6e63 652e 0a20 2020  inheritance..   
+00005cb0: 2020 2020 2020 205f 4461 7461 204f 626a         _Data Obj
+00005cc0: 6563 745f 2075 6e64 6572 7374 616e 6473  ect_ understands
+00005cd0: 2077 686f 7365 2063 6163 6865 2069 7420   whose cache it 
+00005ce0: 6973 2061 6e64 2065 7865 6375 7465 7320  is and executes 
+00005cf0: 7468 6520 7061 7274 206f 6620 7468 6520  the part of the 
+00005d00: 776f 726b 666c 6f77 2074 6861 7420 7761  workflow that wa
+00005d10: 7320 6e6f 7420 6578 6563 7574 6564 2e0a  s not executed..
+00005d20: 2020 2020 2020 2020 2a20 5468 6520 6f77          * The ow
+00005d30: 6e20 6361 6368 653a 0a20 2020 2020 2020  n cache:.       
+00005d40: 2020 2049 6620 6974 2069 7320 6e6f 7420     If it is not 
+00005d50: 7468 6520 6669 7273 7420 6974 6572 6174  the first iterat
+00005d60: 696f 6e20 6f66 2074 6869 7320 4461 7461  ion of this Data
+00005d70: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
+00005d80: 200a 2020 2020 2020 2020 4e6f 7465 2074   .        Note t
+00005d90: 6861 7420 7468 6520 6361 6368 6520 7374  hat the cache st
+00005da0: 6174 6520 6f66 2074 6865 2044 6174 6120  ate of the Data 
+00005db0: 6f62 6a65 6374 2069 7320 6e6f 7420 696e  object is not in
+00005dc0: 6865 7269 7465 642e 0a20 2020 2020 2020  herited..       
+00005dd0: 200a 2020 2020 2020 2020 2323 2323 2046   .        #### F
+00005de0: 6f72 6365 6420 6361 6368 696e 670a 2020  orced caching.  
+00005df0: 2020 2020 2020 596f 7520 6361 6e20 7465        You can te
+00005e00: 6c6c 2044 5320 746f 2063 6163 6865 2064  ll DS to cache d
+00005e10: 6174 6120 746f 2073 7065 6369 6669 6320  ata to specific 
+00005e20: 6361 6368 6520 6669 6c65 2c20 7768 6963  cache file, whic
+00005e30: 6820 776f 6e27 7420 6265 2064 656c 6574  h won't be delet
+00005e40: 6564 2061 6674 6572 2073 6372 6970 7420  ed after script 
+00005e50: 656e 642e 0a20 2020 2020 2020 2059 6f75  end..        You
+00005e60: 2063 616e 2073 6565 2065 7861 6d70 6c65   can see example
+00005e70: 2069 6e20 312e 3132 2073 6563 7469 6f6e   in 1.12 section
+00005e80: 206f 6620 5b67 6574 5f73 7461 7274 6564   of [get_started
+00005e90: 5f65 7861 6d70 6c65 5d28 6578 616d 706c  _example](exampl
+00005ea0: 6573 2f67 6574 5f73 7461 7274 6564 5f65  es/get_started_e
+00005eb0: 7861 6d70 6c65 2e70 7929 2e0a 2020 2020  xample.py)..    
+00005ec0: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
+00005ed0: 2020 2020 2020 2323 2320 4576 656e 7454        ### EventT
+00005ee0: 7265 6520 616e 6420 636f 6c6c 6563 7469  ree and collecti
+00005ef0: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
+00005f00: 2020 2020 2023 2323 2320 4576 656e 7454       #### EventT
+00005f10: 7265 650a 2020 2020 2020 2020 0a20 2020  ree.        .   
+00005f20: 2020 2020 2060 4576 656e 7454 7265 6560       `EventTree`
+00005f30: 2069 7320 6120 7472 6565 2d62 6173 6564   is a tree-based
+00005f40: 2064 6174 6120 7374 7275 6374 7572 6520   data structure 
+00005f50: 6f66 2065 7665 6e74 732e 2049 7420 616c  of events. It al
+00005f60: 6c6f 7773 2079 6f75 2067 6574 2063 6869  lows you get chi
+00005f70: 6c64 7265 6e20 616e 6420 7061 7265 6e74  ldren and parent
+00005f80: 7320 6f66 2065 7665 6e74 2c20 0a20 2020  s of event, .   
+00005f90: 2020 2020 2064 6973 706c 6179 2074 7265       display tre
+00005fa0: 652c 2067 6574 2066 756c 6c20 7061 7468  e, get full path
+00005fb0: 2074 6f20 6576 656e 7420 6574 632e 0a20   to event etc.. 
+00005fc0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005fd0: 4465 7461 696c 733a 0a20 2020 2020 2020  Details:.       
+00005fe0: 200a 2020 2020 2020 2020 2a20 6045 7665   .        * `Eve
+00005ff0: 6e74 5472 6565 6020 636f 6e74 6169 6e73  ntTree` contains
+00006000: 2061 6c6c 2065 7665 6e74 7320 696e 206d   all events in m
+00006010: 656d 6f72 792e 0a20 2020 2020 2020 202a  emory..        *
+00006020: 2054 7265 6520 6861 7320 736f 6d65 2069   Tree has some i
+00006030: 6d70 6f72 7461 6e74 2074 6572 6d73 3a0a  mportant terms:.
+00006040: 2020 2020 2020 2020 2020 2020 312e 205f              1. _
+00006050: 416e 6365 7374 6f72 5f20 6973 2061 6e79  Ancestor_ is any
+00006060: 2072 656c 6174 6976 6520 6f66 2074 6865   relative of the
+00006070: 2065 7665 6e74 2075 7020 7468 6520 7472   event up the tr
+00006080: 6565 2028 6772 616e 6470 6172 656e 742c  ee (grandparent,
+00006090: 2070 6172 656e 7420 6574 632e 292e 0a20   parent etc.).. 
+000060a0: 2020 2020 2020 2020 2020 2032 2e20 5f50             2. _P
+000060b0: 6172 656e 745f 2069 7320 6f6e 6c79 2074  arent_ is only t
+000060c0: 6865 2066 6972 7374 2072 656c 6174 6976  he first relativ
+000060d0: 6520 6f66 2074 6865 2065 7665 6e74 2075  e of the event u
+000060e0: 7020 7468 6520 7472 6565 2e0a 2020 2020  p the tree..    
+000060f0: 2020 2020 2020 2020 332e 205f 4368 696c          3. _Chil
+00006100: 645f 2069 7320 7468 6520 6669 7273 7420  d_ is the first 
+00006110: 7265 6c61 7469 7665 206f 6620 7468 6520  relative of the 
+00006120: 6576 656e 7420 646f 776e 2074 6865 2074  event down the t
+00006130: 7265 652e 0a20 2020 2020 2020 200a 2020  ree..        .  
+00006140: 2020 2020 2020 5461 6b65 2061 206c 6f6f        Take a loo
+00006150: 6b20 6174 2074 6865 2066 6f6c 6c6f 7769  k at the followi
+00006160: 6e67 2048 544d 4c20 7472 6565 2074 6f20  ng HTML tree to 
+00006170: 756e 6465 7273 7461 6e64 2074 6865 6d2e  understand them.
+00006180: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00006190: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+000061a0: 2020 2020 203c 626f 6479 3e20 3c21 2d2d       <body> <!--
+000061b0: 2061 6e63 6573 746f 7220 2867 7261 6e64   ancestor (grand
+000061c0: 7061 7265 6e74 292c 2062 7574 206e 6f74  parent), but not
+000061d0: 2070 6172 656e 7420 2d2d 3e0a 2020 2020   parent -->.    
+000061e0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000061f0: 3e20 3c21 2d2d 2070 6172 656e 7420 2620  > <!-- parent & 
+00006200: 616e 6365 7374 6f72 202d 2d3e 0a20 2020  ancestor -->.   
+00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006220: 203c 703e 4865 6c6c 6f2c 2077 6f72 6c64   <p>Hello, world
+00006230: 213c 2f70 3e20 3c21 2d2d 2063 6869 6c64  !</p> <!-- child
+00006240: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
+00006250: 2020 2020 2020 2020 203c 703e 476f 6f64           <p>Good
+00006260: 6279 6521 3c2f 703e 203c 212d 2d20 7369  bye!</p> <!-- si
+00006270: 626c 696e 6720 2d2d 3e0a 2020 2020 2020  bling -->.      
+00006280: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00006290: 0a20 2020 2020 2020 2020 2020 203c 2f62  .            </b
+000062a0: 6f64 793e 0a20 2020 2020 2020 2020 2020  ody>.           
+000062b0: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
+000062c0: 2020 2020 2023 2323 2320 436f 6c6c 6563       #### Collec
+000062d0: 7469 6f6e 730a 2020 2020 2020 2020 0a20  tions.        . 
+000062e0: 2020 2020 2020 202a 2a45 7665 6e74 5472         **EventTr
+000062f0: 6565 436f 6c6c 6563 7469 6f6e 2a2a 2069  eeCollection** i
+00006300: 7320 6120 636f 6c6c 6563 7469 6f6e 206f  s a collection o
+00006310: 6620 4576 656e 7454 7265 6573 2e20 5468  f EventTrees. Th
+00006320: 6520 636f 6c6c 6563 7469 6f6e 2062 7569  e collection bui
+00006330: 6c64 7320 6120 6665 7720 5f45 7665 6e74  lds a few _Event
+00006340: 5472 6565 5f20 6279 2070 6173 7365 6420  Tree_ by passed 
+00006350: 5f44 6174 610a 2020 2020 2020 2020 6f62  _Data.        ob
+00006360: 6a65 6374 5f2e 2041 6c74 686f 7567 6820  ject_. Although 
+00006370: 796f 7520 6361 6e20 6368 616e 6765 2074  you can change t
+00006380: 6865 2074 7265 6520 6469 7265 6374 6c79  he tree directly
+00006390: 2c20 6974 2773 2062 6574 7465 7220 746f  , it's better to
+000063a0: 2064 6f20 6974 2074 6872 6f75 6768 2063   do it through c
+000063b0: 6f6c 6c65 6374 696f 6e73 2062 6563 6175  ollections becau
+000063c0: 7365 2074 6865 7920 6172 6520 6177 6172  se they are awar
+000063d0: 6520 6f66 0a20 2020 2020 2020 2060 6465  e of.        `de
+000063e0: 7461 6368 6564 5f65 7665 6e74 7360 2061  tached_events` a
+000063f0: 6e64 2063 616e 2073 6f6c 7665 2073 6f6d  nd can solve som
+00006400: 6520 6576 656e 7473 2064 6570 656e 6465  e events depende
+00006410: 6e63 6965 732e 2054 6865 2063 6f6c 6c65  ncies. The colle
+00006420: 6374 696f 6e20 6861 7320 7369 6d69 6c61  ction has simila
+00006430: 7220 6665 6174 7572 6573 206c 696b 6520  r features like 
+00006440: 6120 7369 6e67 6c65 205f 4576 656e 7454  a single _EventT
+00006450: 7265 655f 0a20 2020 2020 2020 2062 7574  ree_.        but
+00006460: 2061 7070 6c79 696e 6720 7468 656d 2066   applying them f
+00006470: 6f72 2061 6c6c 205f 4576 656e 7454 7265  or all _EventTre
+00006480: 6573 5f2e 0a20 2020 2020 2020 200a 2020  es_..        .  
+00006490: 2020 2020 2020 2a2a 5061 7265 6e74 4576        **ParentEv
+000064a0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+000064b0: 6e2a 2a20 6973 2061 2063 6f6c 6c65 6374  n** is a collect
+000064c0: 696f 6e20 7369 6d69 6c61 7220 746f 205f  ion similar to _
+000064d0: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
+000064e0: 696f 6e5f 2062 7574 2063 6f6e 7461 696e  ion_ but contain
+000064f0: 696e 6720 6f6e 6c79 2070 6172 656e 7420  ing only parent 
+00006500: 6576 656e 7473 2074 6861 740a 2020 2020  events that.    
+00006510: 2020 2020 6172 6520 7265 6665 7265 6e63      are referenc
+00006520: 6564 2069 6e20 7468 6520 6461 7461 2073  ed in the data s
+00006530: 7472 6561 6d2e 2054 6865 2063 6f6c 6c65  tream. The colle
+00006540: 6374 696f 6e20 6861 7320 6665 6174 7572  ction has featur
+00006550: 6573 2073 696d 696c 6172 2074 6f20 5f45  es similar to _E
+00006560: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
+00006570: 6f6e 5f2e 0a20 2020 2020 2020 200a 2020  on_..        .  
+00006580: 2020 2020 2020 4465 7461 696c 733a 0a20        Details:. 
+00006590: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000065a0: 2a20 546f 2075 7365 2045 5420 636f 6c6c  * To use ET coll
+000065b0: 6563 7469 6f6e 7320 796f 7520 6e65 6564  ections you need
+000065c0: 2074 6f20 696e 6974 6961 6c69 7a65 2074   to initialize t
+000065d0: 6865 6d20 6279 205f 4554 4344 7269 7665  hem by _ETCDrive
+000065e0: 725f 2e20 4461 7461 2073 6f75 7263 6573  r_. Data sources
+000065f0: 2075 7375 616c 6c79 2070 726f 7669 6465   usually provide
+00006600: 2074 6865 6d2e 0a20 2020 2020 2020 2020   them..         
+00006610: 2059 6f75 2063 616e 2063 7265 6174 6520   You can create 
+00006620: 6974 2062 7920 796f 7572 7365 6c66 2064  it by yourself d
+00006630: 6570 656e 6469 6e67 206f 6e20 796f 7572  epending on your
+00006640: 2064 6174 6120 7374 7275 6374 7572 652e   data structure.
+00006650: 2020 0a20 2020 2020 2020 202a 2054 6865    .        * The
+00006660: 2063 6f6c 6c65 6374 696f 6e20 6861 7320   collection has 
+00006670: 6120 6665 6174 7572 6520 746f 2072 6563  a feature to rec
+00006680: 6f76 6572 2065 7665 6e74 732e 2041 6c6c  over events. All
+00006690: 2065 7665 6e74 7320 7468 6174 2061 7265   events that are
+000066a0: 206e 6f74 2069 6e20 7468 6520 7265 6365   not in the rece
+000066b0: 6976 6564 2064 6174 6120 7374 7265 616d  ived data stream
+000066c0: 2c20 6275 7420 7768 6963 6820 6172 650a  , but which are.
+000066d0: 2020 2020 2020 2020 2020 7265 6665 7265            refere
+000066e0: 6e63 6564 2077 696c 6c20 6265 206c 6f61  nced will be loa
+000066f0: 6465 6420 6672 6f6d 2074 6865 2064 6174  ded from the dat
+00006700: 6120 736f 7572 6365 2e0a 2020 2020 2020  a source..      
+00006710: 2020 2a20 596f 7520 6361 6e20 7461 6b65    * You can take
+00006720: 2060 6465 7461 6368 6564 5f65 7665 6e74   `detached_event
+00006730: 7360 2074 6f20 7365 6520 7768 6963 6820  s` to see which 
+00006740: 6576 656e 7473 2061 7265 206d 6973 7369  events are missi
+00006750: 6e67 2e0a 2020 2020 2020 2020 2a20 4966  ng..        * If
+00006760: 2079 6f75 2077 616e 742c 2079 6f75 2063   you want, you c
+00006770: 616e 2062 7569 6c64 2070 6172 656e 746c  an build parentl
+00006780: 6573 7320 7472 6565 7320 7768 6572 6520  ess trees where 
+00006790: 7468 6520 6d69 7373 696e 6720 6576 656e  the missing even
+000067a0: 7473 2061 7265 2073 7475 6262 6564 2069  ts are stubbed i
+000067b0: 6e73 7465 6164 2e20 4a75 7374 0a20 2020  nstead. Just.   
+000067c0: 2020 2020 2020 2075 7365 2060 6765 745f         use `get_
+000067d0: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
+000067e0: 2829 602e 0a20 2020 2020 2020 200a 2020  ()`..        .  
+000067f0: 2020 2020 2020 5265 7175 6972 656d 656e        Requiremen
+00006800: 7473 3a0a 2020 2020 2020 2020 0a20 2020  ts:.        .   
+00006810: 2020 2020 2031 2e20 4576 656e 7473 2070       1. Events p
+00006820: 726f 7669 6465 6420 746f 2045 5443 2068  rovided to ETC h
+00006830: 6176 6520 746f 2068 6176 6520 6065 7665  ave to have `eve
+00006840: 6e74 5f6e 616d 6560 2c20 6065 7665 6e74  nt_name`, `event
+00006850: 5f69 6460 2c20 6070 6172 656e 745f 6576  _id`, `parent_ev
+00006860: 656e 745f 6964 6020 6669 656c 6473 2e20  ent_id` fields. 
+00006870: 5468 6579 200a 2020 2020 2020 2020 6361  They .        ca
+00006880: 6e20 6861 7665 2061 6e6f 7468 6572 206e  n have another n
+00006890: 616d 6573 2028 6974 2072 6573 6f6c 7665  ames (it resolve
+000068a0: 7320 696e 2074 6865 2064 7269 7665 7229  s in the driver)
+000068b0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+000068c0: 2020 2023 2323 2320 4869 6e74 730a 2020     #### Hints.  
+000068d0: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
+000068e0: 2052 656d 6f76 6520 616c 6c20 756e 6e65   Remove all unne
+000068f0: 6365 7373 6172 7920 6669 656c 6473 2066  cessary fields f
+00006900: 726f 6d20 6576 656e 7473 2062 6566 6f72  rom events befor
+00006910: 6520 7061 7373 696e 6720 746f 2061 205f  e passing to a _
+00006920: 636f 6c6c 6563 7469 6f6e 5f20 746f 2072  collection_ to r
+00006930: 6564 7563 6520 6d65 6d6f 7279 2075 7361  educe memory usa
+00006940: 6765 2e0a 2020 2020 2020 2020 2a20 5573  ge..        * Us
+00006950: 6520 6073 686f 7728 2960 206d 6574 686f  e `show()` metho
+00006960: 6420 746f 2070 7269 6e74 2074 6865 2074  d to print the t
+00006970: 7265 6520 696e 2074 7265 652d 6c69 6b65  ree in tree-like
+00006980: 2076 6965 772e 0a20 2020 2020 2020 202a   view..        *
+00006990: 204e 6f74 6520 7468 6174 2074 6865 2060   Note that the `
+000069a0: 6765 745f 7860 206d 6574 686f 6473 2077  get_x` methods w
+000069b0: 696c 6c20 7261 6973 6520 616e 2065 7863  ill raise an exc
+000069c0: 6570 7469 6f6e 2069 6620 796f 7520 7061  eption if you pa
+000069d0: 7373 2061 6e20 756e 6b6e 6f77 6e20 6576  ss an unknown ev
+000069e0: 656e 7420 6964 2c20 756e 6c69 6b65 2074  ent id, unlike t
+000069f0: 6865 2060 6669 6e64 5f78 6020 6d65 7468  he `find_x` meth
+00006a00: 6f64 7320 280a 2020 2020 2020 2020 2020  ods (.          
+00006a10: 7468 6579 2072 6574 7572 6e20 4e6f 6e65  they return None
+00006a20: 292e 0a20 2020 2020 2020 202a 2049 6620  )..        * If 
+00006a30: 796f 7520 7761 6e74 2074 6f20 6b6e 6f77  you want to know
+00006a40: 2074 6861 7420 7370 6563 6966 6965 6420   that specified 
+00006a50: 6576 656e 7420 6578 6973 7473 2c20 7573  event exists, us
+00006a60: 6520 7468 6520 7079 7468 6f6e 2060 696e  e the python `in
+00006a70: 6020 6b65 7977 6f72 6420 2865 2e67 2e20  ` keyword (e.g. 
+00006a80: 6027 6576 656e 742d 6964 2720 696e 2065  `'event-id' in e
+00006a90: 7665 6e74 735f 7472 6565 6029 2e0a 2020  vents_tree`)..  
+00006aa0: 2020 2020 2020 2a20 5573 6520 7468 6520        * Use the 
+00006ab0: 7079 7468 6f6e 2060 6c65 6e60 206b 6579  python `len` key
+00006ac0: 776f 7264 2074 6f20 6765 7420 6576 656e  word to get even
+00006ad0: 7473 206e 756d 6265 7220 696e 2074 6865  ts number in the
+00006ae0: 2074 7265 652e 0a20 2020 2020 2020 200a   tree..        .
+00006af0: 2020 2020 2020 2020 2323 2320 4669 656c          ### Fiel
+00006b00: 6473 5265 736f 6c76 6572 0a20 2020 2020  dsResolver.     
+00006b10: 2020 2054 6865 2069 6465 6120 6f66 2075     The idea of u
+00006b20: 7369 6e67 2072 6573 6f6c 7665 7273 3a20  sing resolvers: 
+00006b30: 200a 2020 2020 2020 2020 4974 2073 6f6c   .        It sol
+00006b40: 7665 7320 7468 6520 7072 6f62 6c65 6d20  ves the problem 
+00006b50: 6f66 2068 6176 696e 6720 6120 6665 7720  of having a few 
+00006b60: 4461 7461 536f 7572 6365 7320 7769 7468  DataSources with
+00006b70: 2074 6865 2073 616d 6520 6461 7461 2c20   the same data, 
+00006b80: 0a20 2020 2020 2020 2062 7574 2077 6974  .        but wit
+00006b90: 6820 6469 6666 6572 656e 7420 7761 7973  h different ways
+00006ba0: 2074 6f20 6765 7420 6974 2e0a 2020 2020   to get it..    
+00006bb0: 2020 2020 0a20 2020 2020 2020 2054 6865      .        The
+00006bc0: 7365 2063 6c61 7373 6573 2070 726f 7669  se classes provi
+00006bd0: 6465 2079 6f75 2067 6574 7465 7220 6d65  de you getter me
+00006be0: 7468 6f64 732e 200a 2020 2020 2020 2020  thods. .        
+00006bf0: 5573 696e 6720 7468 6573 6520 636c 6173  Using these clas
+00006c00: 7365 7320 616c 6c6f 7773 2079 6f75 2074  ses allows you t
+00006c10: 6f20 6672 6565 6c79 2073 7769 7463 6820  o freely switch 
+00006c20: 6265 7477 6565 6e20 6469 6666 6572 656e  between differen
+00006c30: 7420 6461 7461 200a 2020 2020 2020 2020  t data .        
+00006c40: 666f 726d 6174 7320 616e 6420 646f 6e27  formats and don'
+00006c50: 7420 6368 616e 6765 2079 6f75 7220 636f  t change your co
+00006c60: 6465 2e20 0a20 2020 2020 2020 200a 2020  de. .        .  
+00006c70: 2020 2020 2020 5265 736f 6c76 6572 7320        Resolvers 
+00006c80: 736f 6c76 6520 7468 6520 7072 6f62 6c65  solve the proble
+00006c90: 6d20 6f66 2064 6174 612d 666f 726d 6174  m of data-format
+00006ca0: 206d 6967 7261 7469 6f6e 2e20 200a 2020   migration.  .  
+00006cb0: 2020 2020 2020 2d20 6669 656c 6473 2070        - fields p
+00006cc0: 6c61 6365 2063 616e 2062 6520 6368 616e  lace can be chan
+00006cd0: 6765 640a 2020 2020 2020 2020 2d20 6669  ged.        - fi
+00006ce0: 656c 6473 206e 616d 6573 2063 616e 2062  elds names can b
+00006cf0: 6520 6368 616e 6765 640a 2020 2020 2020  e changed.      
+00006d00: 2020 0a20 2020 2020 2020 2052 6573 6f6c    .        Resol
+00006d10: 7665 7273 2063 616e 2077 6f72 6b20 6f6e  vers can work on
+00006d20: 6c79 2077 6974 6820 6f6e 6520 6576 656e  ly with one even
+00006d30: 742f 6d65 7373 6167 652e 200a 2020 2020  t/message. .    
+00006d40: 2020 2020 4974 206d 6561 6e73 2c20 6966      It means, if
+00006d50: 2079 6f75 7220 6d65 7373 6167 6520 6861   your message ha
+00006d60: 7320 7375 622d 6d65 7373 6167 6573 2069  s sub-messages i
+00006d70: 7420 776f 6e27 7420 776f 726b 2c20 6265  t won't work, be
+00006d80: 6361 7573 6520 7265 736f 6c76 6572 2077  cause resolver w
+00006d90: 696c 6c20 6e6f 7420 0a20 2020 2020 2020  ill not .       
+00006da0: 206b 6e6f 7720 7769 7468 2077 6869 6368   know with which
+00006db0: 2073 7562 2d6d 6573 7361 6765 2073 686f   sub-message sho
+00006dc0: 756c 6420 6974 2077 6f72 6b2e 200a 2020  uld it work. .  
+00006dd0: 2020 2020 2020 0a20 2020 2020 2020 2049        .        I
+00006de0: 6d70 6c65 6d65 6e74 6174 696f 6e20 6164  mplementation ad
+00006df0: 7669 6365 3a0a 2020 2020 2020 2020 312e  vice:.        1.
+00006e00: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+00006e10: 656e 7465 6445 7272 6f72 202d 2d20 6966  entedError -- if
+00006e20: 2079 6f75 7220 496d 706c 656d 656e 7461   your Implementa
+00006e30: 7469 6f6e 2064 6f65 736e 2774 2073 7570  tion doesn't sup
+00006e40: 706f 7274 2074 6869 7320 6765 7474 6572  port this getter
+00006e50: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00006e60: 2020 2050 6572 666f 726d 616e 6365 2069     Performance i
+00006e70: 6d70 6163 743a 0a20 2020 2020 2020 202d  mpact:.        -
+00006e80: 2049 7420 6120 6269 7420 736c 6f77 6572   It a bit slower
+00006e90: 2074 6861 6e20 7573 696e 6720 6e61 6b65   than using nake
+00006ea0: 6420 6669 656c 6420 6163 6365 7373 2060  d field access `
+00006eb0: 6469 6374 5b27 6b65 7927 5d60 2e20 0a20  dict['key']`. . 
+00006ec0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00006ed0: 2323 2032 2e34 2e20 4c69 6e6b 730a 2020  ## 2.4. Links.  
+00006ee0: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00006ef0: 205b 5265 706f 7274 2044 6174 6120 5072   [Report Data Pr
+00006f00: 6f76 6964 6572 5d28 6874 7470 733a 2f2f  ovider](https://
+00006f10: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
+00006f20: 6574 2f74 6832 2d72 7074 2d64 6174 612d  et/th2-rpt-data-
+00006f30: 7072 6f76 6964 6572 290a 2020 2020 2020  provider).      
+00006f40: 2020 2d20 5b54 6832 2044 6174 6120 5365    - [Th2 Data Se
+00006f50: 7276 6963 6573 2055 7469 6c73 5d28 6874  rvices Utils](ht
+00006f60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00006f70: 2f74 6832 2d6e 6574 2f74 6832 2d64 6174  /th2-net/th2-dat
+00006f80: 612d 7365 7276 6963 6573 2d75 7469 6c73  a-services-utils
+00006f90: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00006fa0: 2020 2023 2033 2e20 4265 7374 2070 7261     # 3. Best pra
+00006fb0: 6374 6963 6573 0a20 2020 2020 2020 2044  ctices.        D
+00006fc0: 6570 656e 6469 6e67 206f 6e20 686f 7720  epending on how 
+00006fd0: 796f 7520 776f 726b 2077 6974 6820 6044  you work with `D
+00006fe0: 6174 6120 6f62 6a65 6374 602c 2069 7420  ata object`, it 
+00006ff0: 6361 6e20 6265 2073 6c6f 7720 6f66 2066  can be slow of f
+00007000: 6173 742e 2020 0a20 2020 2020 2020 2041  ast.  .        A
+00007010: 7320 7769 7468 2061 2072 656c 6174 696f  s with a relatio
+00007020: 6e61 6c20 6461 7461 6261 7365 2c20 796f  nal database, yo
+00007030: 7520 6361 6e20 7772 6974 6520 6120 7175  u can write a qu
+00007040: 6572 7920 7468 6174 2077 696c 6c20 7265  ery that will re
+00007050: 7475 726e 2064 6174 6120 736c 6f77 6c79  turn data slowly
+00007060: 206f 7220 7175 6963 6b6c 792c 200a 2020   or quickly, .  
+00007070: 2020 2020 2020 7468 6520 7361 6d65 2077        the same w
+00007080: 6865 6e20 776f 726b 696e 6720 7769 7468  hen working with
+00007090: 2061 2060 4461 7461 206f 626a 6563 7460   a `Data object`
+000070a0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+000070b0: 2020 2046 6f6c 6c6f 7720 7468 6520 7275     Follow the ru
+000070c0: 6c65 7320 746f 206d 616b 6520 796f 7572  les to make your
+000070d0: 2077 6f72 6b20 7769 7468 2044 6174 6120   work with Data 
+000070e0: 6f62 6a65 6374 2066 6173 743a 0a20 2020  object fast:.   
+000070f0: 2020 2020 2031 2e20 5573 6520 6044 6174       1. Use `Dat
+00007100: 612e 7573 655f 6361 6368 6528 2960 2069  a.use_cache()` i
+00007110: 6620 796f 7520 6974 6572 6174 6520 6461  f you iterate da
+00007120: 7461 206d 6f72 6520 7468 616e 206f 6e65  ta more than one
+00007130: 2074 696d 652e 0a20 2020 2020 2020 2032   time..        2
+00007140: 2e20 5472 7920 746f 2064 6f6e 2774 2069  . Try to don't i
+00007150: 7465 7261 7465 206f 6e65 2060 4461 7461  terate one `Data
+00007160: 206f 626a 6563 7460 2069 6e73 6964 6520   object` inside 
+00007170: 7468 6520 6f74 6865 7220 6f6e 652e 2020  the other one.  
+00007180: 0a20 2020 2020 2020 2020 2020 4966 2079  .           If y
+00007190: 6f75 2073 686f 756c 6420 746f 2064 6f20  ou should to do 
+000071a0: 6974 2c20 7573 6520 7368 6f72 7420 6044  it, use short `D
+000071b0: 6174 6120 6f62 6a65 6374 6020 6669 7273  ata object` firs
+000071c0: 7420 616e 6420 6c6f 6e67 2060 4461 7461  t and long `Data
+000071d0: 206f 626a 6563 7460 2069 6e73 6964 6520   object` inside 
+000071e0: 7468 6520 6c6f 6f70 2e20 200a 2020 2020  the loop.  .    
+000071f0: 2020 2020 2020 2049 7427 6c6c 2061 6c6c         It'll all
+00007200: 6f77 2079 6f75 206f 7065 6e20 7468 6520  ow you open the 
+00007210: 6361 6368 6520 6669 6c65 206f 7220 6372  cache file or cr
+00007220: 6561 7465 2061 2072 6571 7565 7374 2074  eate a request t
+00007230: 6f20 6044 6174 6120 736f 7572 6365 6020  o `Data source` 
+00007240: 6c65 7373 206e 756d 6265 7220 6f66 2074  less number of t
+00007250: 696d 6573 2e0a 2020 2020 2020 2020 0a20  imes..        . 
+00007260: 2020 2020 2020 2023 2034 2e20 4f66 6669         # 4. Offi
+00007270: 6369 616c 2044 6174 6153 6f75 7263 6520  cial DataSource 
+00007280: 696d 706c 656d 656e 7461 7469 6f6e 730a  implementations.
+00007290: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000072a0: 202d 205b 4c69 6768 7477 6569 6768 7420   - [Lightweight 
+000072b0: 4461 7461 2050 726f 7669 6465 7220 4461  Data Provider Da
+000072c0: 7461 2053 6f75 7263 655d 2868 7474 7073  ta Source](https
+000072d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
+000072e0: 322d 6e65 742f 7468 322d 6473 2d73 6f75  2-net/th2-ds-sou
+000072f0: 7263 652d 6c77 6470 290a 2020 2020 2020  rce-lwdp).      
+00007300: 2020 0a20 2020 2020 2020 200a 2020 2020    .        .    
+00007310: 2020 2020 2320 352e 2041 5049 0a20 2020      # 5. API.   
+00007320: 2020 2020 200a 2020 2020 2020 2020 4966       .        If
+00007330: 2079 6f75 2061 7265 206c 6f6f 6b69 6e67   you are looking
+00007340: 2066 6f72 2063 6c61 7373 6573 2064 6573   for classes des
+00007350: 6372 6970 7469 6f6e 2073 6565 2074 6865  cription see the
+00007360: 205b 4150 4920 446f 6375 6d65 6e74 6174   [API Documentat
+00007370: 696f 6e5d 2864 6f63 756d 656e 7461 7469  ion](documentati
+00007380: 6f6e 2f61 7069 2f69 6e64 6578 2e6d 6429  on/api/index.md)
+00007390: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+000073a0: 2020 2023 2036 2e20 4578 616d 706c 6573     # 6. Examples
+000073b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000073c0: 2020 2d20 5b67 6574 5f73 7461 7274 6564    - [get_started
+000073d0: 5f65 7861 6d70 6c65 2e70 795d 2865 7861  _example.py](exa
+000073e0: 6d70 6c65 732f 6765 745f 7374 6172 7465  mples/get_starte
+000073f0: 645f 6578 616d 706c 652e 7079 290a 2020  d_example.py).  
+00007400: 2020 2020 2020 0a50 6c61 7466 6f72 6d3a        .Platform:
+00007410: 2055 4e4b 4e4f 574e 0a52 6571 7569 7265   UNKNOWN.Require
+00007420: 732d 5079 7468 6f6e 3a20 3e3d 332e 370a  s-Python: >=3.7.
+00007430: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+00007440: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+00007450: 6172 6b64 6f77 6e0a 5072 6f76 6964 6573  arkdown.Provides
+00007460: 2d45 7874 7261 3a20 7264 700a 5072 6f76  -Extra: rdp.Prov
+00007470: 6964 6573 2d45 7874 7261 3a20 7264 7035  ides-Extra: rdp5
+00007480: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00007490: 2072 6470 360a 5072 6f76 6964 6573 2d45   rdp6.Provides-E
+000074a0: 7874 7261 3a20 6c77 6470 0a50 726f 7669  xtra: lwdp.Provi
+000074b0: 6465 732d 4578 7472 613a 206c 7764 7031  des-Extra: lwdp1
+000074c0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+000074d0: 206c 7764 7032 0a50 726f 7669 6465 732d   lwdp2.Provides-
+000074e0: 4578 7472 613a 206c 7764 702d 6465 760a  Extra: lwdp-dev.
+000074f0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00007500: 7574 696c 732d 7270 742d 7669 6577 6572  utils-rpt-viewer
+00007510: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00007520: 2075 7469 6c73 2d72 7074 2d76 6965 7765   utils-rpt-viewe
+00007530: 7235 0a50 726f 7669 6465 732d 4578 7472  r5.Provides-Extr
+00007540: 613a 2075 7469 6c73 2d61 6476 616e 6365  a: utils-advance
+00007550: 640a                                     d.
```

### Comparing `th2_data_services-2.0.0.dev5738217622/README.md` & `th2_data_services-2.0.0.dev5738245039/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,1479 +58,1484 @@
 00000390: 7472 6565 2d61 6e64 2d63 6f6c 6c65 6374  tree-and-collect
 000003a0: 696f 6e73 290a 2020 2020 2020 2020 202a  ions).         *
 000003b0: 205b 4576 656e 7454 7265 655d 2823 6576   [EventTree](#ev
 000003c0: 656e 7474 7265 6529 0a20 2020 2020 2020  enttree).       
 000003d0: 2020 2a20 5b43 6f6c 6c65 6374 696f 6e73    * [Collections
 000003e0: 5d28 2363 6f6c 6c65 6374 696f 6e73 290a  ](#collections).
 000003f0: 2020 2020 2020 2020 202a 205b 4869 6e74           * [Hint
-00000400: 735d 2823 6869 6e74 7329 0a20 2020 2a20  s](#hints).   * 
-00000410: 5b32 2e34 2e20 4c69 6e6b 735d 2823 3234  [2.4. Links](#24
-00000420: 2d6c 696e 6b73 290a 2a20 5b33 2e20 4f66  -links).* [3. Of
-00000430: 6669 6369 616c 2044 6174 6153 6f75 7263  ficial DataSourc
-00000440: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
-00000450: 735d 2823 332d 6f66 6669 6369 616c 2d64  s](#3-official-d
-00000460: 6174 6173 6f75 7263 652d 696d 706c 656d  atasource-implem
-00000470: 656e 7461 7469 6f6e 7329 0a2a 205b 342e  entations).* [4.
-00000480: 2041 5049 5d28 2334 2d61 7069 290a 2a20   API](#4-api).* 
-00000490: 5b35 2e20 4578 616d 706c 6573 5d28 2335  [5. Examples](#5
-000004a0: 2d65 7861 6d70 6c65 7329 0a3c 212d 2d74  -examples).<!--t
-000004b0: 652d 2d3e 0a0a 2320 312e 2049 6e74 726f  e-->..# 1. Intro
-000004c0: 6475 6374 696f 6e0a 0a54 6869 7320 7265  duction..This re
-000004d0: 706f 7369 746f 7279 2069 7320 6120 6c69  pository is a li
-000004e0: 6272 6172 7920 666f 7220 6372 6561 7469  brary for creati
-000004f0: 6e67 2074 6832 2d64 6174 612d 7365 7276  ng th2-data-serv
-00000500: 6963 6573 2061 7070 6c69 6361 7469 6f6e  ices application
-00000510: 732e 0a44 6174 6120 5365 7276 6963 6573  s..Data Services
-00000520: 2061 6c6c 6f77 7320 796f 7520 746f 206d   allows you to m
-00000530: 616e 6970 756c 6174 6520 7468 6520 7374  anipulate the st
-00000540: 7265 616d 2064 6174 6120 7072 6f63 6573  ream data proces
-00000550: 7369 6e67 2077 6f72 6b66 6c6f 7720 7573  sing workflow us
-00000560: 696e 6720 7069 7065 6c69 6e69 6e67 2e0a  ing pipelining..
-00000570: 0a54 6865 206c 6962 7261 7279 2773 2066  .The library's f
-00000580: 6561 7475 7265 733a 0a0a 2d20 5072 6f76  eatures:..- Prov
-00000590: 6964 6573 2063 6f72 6520 696e 7465 7266  ides core interf
-000005a0: 6163 6520 666f 7220 6465 7665 6c6f 7069  ace for developi
-000005b0: 6e67 2064 6174 6120 736f 7572 6365 2069  ng data source i
-000005c0: 6d70 6c65 6d65 6e74 6174 696f 6e73 0a2d  mplementations.-
-000005d0: 2057 6f72 6b20 7769 7468 2069 7465 7261   Work with itera
-000005e0: 626c 6520 6f62 6a65 6374 7320 286c 6973  ble objects (lis
-000005f0: 742c 2074 7570 6c65 2c20 6574 6320 696e  t, tuple, etc in
-00000600: 636c 7564 696e 6720 6669 6c65 7329 2076  cluding files) v
-00000610: 6961 205f 4461 7461 206f 626a 6563 745f  ia _Data object_
-00000620: 2075 7369 6e67 2069 7473 2066 6561 7475   using its featu
-00000630: 7265 730a 2d20 4d61 6e69 7075 6c61 7465  res.- Manipulate
-00000640: 2074 6865 2077 6f72 6b66 6c6f 7720 746f   the workflow to
-00000650: 206d 616b 6520 736f 6d65 2061 6e61 6c79   make some analy
-00000660: 7369 7320 6279 205f 4461 7461 206f 626a  sis by _Data obj
-00000670: 6563 745f 206d 6574 686f 6473 0a2d 2055  ect_ methods.- U
-00000680: 7365 2074 696d 6573 7461 6d70 2063 6f6e  se timestamp con
-00000690: 7665 7274 6572 2069 6d70 6c65 6d65 6e74  verter implement
-000006a0: 6174 696f 6e73 206f 7220 7573 6520 6261  ations or use ba
-000006b0: 7365 2063 6c61 7373 2074 6f20 6372 6561  se class to crea
-000006c0: 7465 2063 7573 746f 6d20 636f 6e76 6572  te custom conver
-000006d0: 7465 7273 0a2d 2042 7569 6c64 2045 7665  ters.- Build Eve
-000006e0: 6e74 2054 7265 6573 2028 4576 656e 7454  nt Trees (EventT
-000006f0: 7265 652c 2045 7665 6e74 5472 6565 436f  ree, EventTreeCo
-00000700: 6c6c 6563 7469 6f6e 2061 6e64 2050 6172  llection and Par
-00000710: 656e 7445 7665 6e74 5472 6565 436f 6c6c  entEventTreeColl
-00000720: 6563 7469 6f6e 2063 6c61 7373 6573 290a  ection classes).
-00000730: 0a57 6f72 6b66 6c6f 7720 6d61 6e69 7075  .Workflow manipu
-00000740: 6c61 7469 6f6e 2074 6f6f 6c73 2061 6c6c  lation tools all
-00000750: 6f77 7320 796f 753a 0a0a 2d20 4669 6c74  ows you:..- Filt
-00000760: 6572 696e 6720 7374 7265 616d 2064 6174  ering stream dat
-00000770: 6120 2860 4461 7461 2e66 696c 7465 7260  a (`Data.filter`
-00000780: 206d 6574 686f 6429 0a2d 2054 7261 6e73   method).- Trans
-00000790: 666f 726d 696e 6720 7374 7265 616d 2064  forming stream d
-000007a0: 6174 6120 2860 4461 7461 2e6d 6170 6020  ata (`Data.map` 
-000007b0: 6d65 7468 6f64 290a 2d20 4c69 6d69 7469  method).- Limiti
-000007c0: 6e67 2074 6865 206e 756d 6265 7220 6f66  ng the number of
-000007d0: 2070 726f 6365 7373 6564 2073 7472 6561   processed strea
-000007e0: 6d69 6e67 2064 6174 6120 2860 4461 7461  ming data (`Data
-000007f0: 2e6c 696d 6974 6020 6d65 7468 6f64 290a  .limit` method).
-00000800: 0a54 6865 7265 2069 7320 616c 736f 2061  .There is also a
-00000810: 6e6f 7468 6572 2070 6172 7420 6f66 205f  nother part of _
-00000820: 6461 7461 2073 6572 7669 6365 735f 0a0a  data services_..
-00000830: 2d20 5b74 6832 2d64 6174 612d 7365 7276  - [th2-data-serv
-00000840: 6963 6573 2d75 7469 6c73 5d28 6874 7470  ices-utils](http
-00000850: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00000860: 6832 2d6e 6574 2f74 6832 2d64 6174 612d  h2-net/th2-data-
-00000870: 7365 7276 6963 6573 2d75 7469 6c73 292e  services-utils).
-00000880: 2049 7427 7320 6120 7365 7420 6f66 2074   It's a set of t
-00000890: 6f6f 6c73 2074 6f20 7065 7266 6f72 6d20  ools to perform 
-000008a0: 7468 6520 6d6f 7374 0a20 2063 6f6d 6d6f  the most.  commo
-000008b0: 6e20 616e 616c 7973 6973 2074 6173 6b73  n analysis tasks
-000008c0: 2e0a 0a23 2032 2e20 4765 7474 696e 6720  ...# 2. Getting 
-000008d0: 7374 6172 7465 640a 0a23 2320 322e 312e  started..## 2.1.
-000008e0: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a23   Installation..#
-000008f0: 2323 2043 6f72 650a 0a2d 2046 726f 6d20  ## Core..- From 
-00000900: 5079 5049 2028 7069 7029 2020 200a 2020  PyPI (pip)   .  
-00000910: 5468 6973 2070 6163 6b61 6765 2063 616e  This package can
-00000920: 2062 6520 666f 756e 6420 6f6e 205b 5079   be found on [Py
-00000930: 5049 5d28 6874 7470 733a 2f2f 7079 7069  PI](https://pypi
-00000940: 2e6f 7267 2f70 726f 6a65 6374 2f74 6832  .org/project/th2
-00000950: 2d64 6174 612d 7365 7276 6963 6573 2f20  -data-services/ 
-00000960: 2274 6832 2d64 6174 612d 7365 7276 6963  "th2-data-servic
-00000970: 6573 2229 2e0a 2020 2020 6060 600a 2020  es")..    ```.  
-00000980: 2020 7069 7020 696e 7374 616c 6c20 7468    pip install th
-00000990: 322d 6461 7461 2d73 6572 7669 6365 730a  2-data-services.
-000009a0: 2020 2020 6060 600a 0a2d 2046 726f 6d20      ```..- From 
-000009b0: 536f 7572 6365 0a20 2020 2060 6060 0a20  Source.    ```. 
-000009c0: 2020 2067 6974 2063 6c6f 6e65 2068 7474     git clone htt
-000009d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000009e0: 7468 322d 6e65 742f 7468 322d 6461 7461  th2-net/th2-data
-000009f0: 2d73 6572 7669 6365 730a 2020 2020 7069  -services.    pi
-00000a00: 7020 696e 7374 616c 6c20 7468 322d 6461  p install th2-da
-00000a10: 7461 2d73 6572 7669 6365 732f 0a20 2020  ta-services/.   
-00000a20: 2060 6060 0a0a 2323 2320 4461 7461 2073   ```..### Data s
-00000a30: 6f75 7263 6573 2028 7072 6f76 6964 6572  ources (provider
-00000a40: 7329 0a0a 5369 6e63 6520 6076 312e 332e  s)..Since `v1.3.
-00000a50: 3060 2c20 7468 6520 6c69 6272 6172 7920  0`, the library 
-00000a60: 646f 6573 6e27 7420 7072 6f76 6964 6520  doesn't provide 
-00000a70: 6461 7461 2073 6f75 7263 6520 6465 7065  data source depe
-00000a80: 6e64 656e 6369 6573 2e0a 0a59 6f75 2073  ndencies...You s
-00000a90: 686f 756c 6420 7072 6f76 6964 6520 6974  hould provide it
-00000aa0: 206d 616e 7561 6c6c 7920 6475 7269 6e67   manually during
-00000ab0: 2069 6e73 7461 6c6c 6174 696f 6e2e 200a   installation. .
-00000ac0: 596f 7520 6a75 7374 206e 6565 6420 746f  You just need to
-00000ad0: 2061 6464 2073 7175 6172 6520 6272 6163   add square brac
-00000ae0: 6b65 7473 2061 6674 6572 206c 6962 7261  kets after libra
-00000af0: 7279 206e 616d 6520 616e 6420 7075 7420  ry name and put 
-00000b00: 6465 7065 6e64 656e 6379 206e 616d 652e  dependency name.
-00000b10: 0a0a 6060 600a 7069 7020 696e 7374 616c  ..```.pip instal
-00000b20: 6c20 7468 322d 6461 7461 2d73 6572 7669  l th2-data-servi
-00000b30: 6365 735b 6465 7065 6e64 656e 6379 5f6e  ces[dependency_n
-00000b40: 616d 655d 0a60 6060 0a0a 2a2a 4465 7065  ame].```..**Depe
-00000b50: 6e64 656e 6369 6573 206c 6973 742a 2a20  ndencies list** 
-00000b60: 0a0a 7c20 2064 6570 656e 6465 6e63 7920  ..|  dependency 
-00000b70: 6e61 6d65 2020 7c20 7072 6f76 6964 6572  name  | provider
-00000b80: 2076 6572 7369 6f6e 2020 2020 2020 2020   version        
-00000b90: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00000ba0: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
-00000bb0: 2d2d 2d3a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|-----------
-00000bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20  ------------|.| 
-00000be0: 2020 2020 2020 6c77 6470 2020 2020 2020        lwdp      
-00000bf0: 2020 7c20 6c61 7465 7374 2076 6572 7369    | latest versi
-00000c00: 6f6e 206f 6620 6c77 6470 2020 2020 2020  on of lwdp      
-00000c10: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-00000c20: 2020 2020 6c77 6470 3220 2020 2020 2020      lwdp2       
-00000c30: 7c20 6c61 7465 7374 2076 6572 7369 6f6e  | latest version
-00000c40: 206f 6620 6c77 6470 2076 3220 2020 2020   of lwdp v2     
-00000c50: 2020 2020 2020 2020 7c0a 7c20 7574 696c          |.| util
-00000c60: 732d 7270 742d 7669 6577 6572 2020 7c20  s-rpt-viewer  | 
-00000c70: 6c61 7465 7374 2076 6572 7369 6f6e 206f  latest version o
-00000c80: 6620 7574 696c 732d 7270 742d 7669 6577  f utils-rpt-view
-00000c90: 6572 2020 2020 7c0a 7c20 7574 696c 732d  er    |.| utils-
-00000ca0: 7270 742d 7669 6577 6572 3520 7c20 6c61  rpt-viewer5 | la
-00000cb0: 7465 7374 2076 6572 7369 6f6e 206f 6620  test version of 
-00000cc0: 7574 696c 732d 7270 742d 7669 6577 6572  utils-rpt-viewer
-00000cd0: 2076 3520 7c0a 7c20 2020 7574 696c 732d   v5 |.|   utils-
-00000ce0: 6164 7661 6e63 6564 2020 7c20 6c61 7465  advanced  | late
-00000cf0: 7374 2076 6572 7369 6f6e 206f 6620 6473  st version of ds
-00000d00: 2d75 7469 6c73 2020 2020 2020 2020 2020  -utils          
-00000d10: 2020 7c0a 0a2a 2a45 7861 6d70 6c65 2a2a    |..**Example**
-00000d20: 0a0a 6060 600a 7069 7020 696e 7374 616c  ..```.pip instal
-00000d30: 6c20 7468 322d 6461 7461 2d73 6572 7669  l th2-data-servi
-00000d40: 6365 735b 6c77 6470 315d 0a60 6060 0a0a  ces[lwdp1].```..
-00000d50: 2323 2032 2e32 2e20 4578 616d 706c 650a  ## 2.2. Example.
-00000d60: 0a41 2067 6f6f 642c 2073 686f 7274 2065  .A good, short e
-00000d70: 7861 6d70 6c65 2069 7320 776f 7274 6820  xample is worth 
-00000d80: 6120 7468 6f75 7361 6e64 2077 6f72 6473  a thousand words
-00000d90: 2e0a 0a54 6869 7320 6578 616d 706c 6520  ...This example 
-00000da0: 7368 6f77 7320 6261 7369 6320 7573 6167  shows basic usag
-00000db0: 6520 6f66 206c 6962 7261 7279 2773 2066  e of library's f
-00000dc0: 6561 7475 7265 732e 0a0a 5b54 6865 2066  eatures...[The f
-00000dd0: 6f6c 6c6f 7769 6e67 2065 7861 6d70 6c65  ollowing example
-00000de0: 2061 7320 6120 6669 6c65 5d28 6578 616d   as a file](exam
-00000df0: 706c 6573 2f67 6574 5f73 7461 7274 6564  ples/get_started
-00000e00: 5f65 7861 6d70 6c65 2e70 7929 2e0a 0a3c  _example.py)...<
-00000e10: 212d 2d20 7374 6172 7420 6765 745f 7374  !-- start get_st
-00000e20: 6172 7465 645f 6578 616d 706c 652e 7079  arted_example.py
-00000e30: 202d 2d3e 0a60 6060 7079 7468 6f6e 0a66   -->.```python.f
-00000e40: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-00000e50: 7420 5475 706c 652c 204c 6973 742c 204f  t Tuple, List, O
-00000e60: 7074 696f 6e61 6c2c 2047 656e 6572 6174  ptional, Generat
-00000e70: 6f72 0a66 726f 6d20 6461 7465 7469 6d65  or.from datetime
-00000e80: 2069 6d70 6f72 7420 6461 7465 7469 6d65   import datetime
-00000e90: 0a0a 6672 6f6d 2074 6832 5f64 6174 615f  ..from th2_data_
-00000ea0: 7365 7276 6963 6573 2e64 6174 6120 696d  services.data im
-00000eb0: 706f 7274 2044 6174 610a 6672 6f6d 2074  port Data.from t
-00000ec0: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
-00000ed0: 2e65 7665 6e74 5f74 7265 6520 696d 706f  .event_tree impo
-00000ee0: 7274 2045 7665 6e74 5472 6565 2c20 4576  rt EventTree, Ev
-00000ef0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00000f00: 6e2c 2050 6172 656e 7445 7665 6e74 5472  n, ParentEventTr
-00000f10: 6565 436f 6c6c 6563 7469 6f6e 2c20 4945  eeCollection, IE
-00000f20: 5443 4472 6976 6572 0a66 726f 6d20 7468  TCDriver.from th
-00000f30: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00000f40: 696e 7465 7266 6163 6573 2069 6d70 6f72  interfaces impor
-00000f50: 7420 4944 6174 6153 6f75 7263 650a 6672  t IDataSource.fr
-00000f60: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
-00000f70: 6963 6573 2e75 7469 6c73 2e63 6f6e 7665  ices.utils.conve
-00000f80: 7274 6572 7320 696d 706f 7274 2044 6174  rters import Dat
-00000f90: 6574 696d 6543 6f6e 7665 7274 6572 2c20  etimeConverter, 
-00000fa0: 4461 7465 7469 6d65 5374 7269 6e67 436f  DatetimeStringCo
-00000fb0: 6e76 6572 7465 722c 2050 726f 746f 6275  nverter, Protobu
-00000fc0: 6654 696d 6573 7461 6d70 436f 6e76 6572  fTimestampConver
-00000fd0: 7465 720a 0a23 205b 305d 204c 6962 2063  ter..# [0] Lib c
-00000fe0: 6f6e 6669 6775 7261 7469 6f6e 0a23 205b  onfiguration.# [
-00000ff0: 302e 315d 2049 6e74 6572 6163 7469 7665  0.1] Interactive
-00001000: 206f 7220 5363 7269 7074 206d 6f64 650a   or Script mode.
-00001010: 2320 4966 2079 6f75 2075 7365 2074 6865  # If you use the
-00001020: 206c 6962 2069 6e20 696e 7465 7261 6374   lib in interact
-00001030: 6976 6520 6d6f 6465 2028 6a75 7079 7465  ive mode (jupyte
-00001040: 722c 2069 7079 7468 6f6e 2920 6974 2773  r, ipython) it's
-00001050: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
-00001060: 7365 7420 7468 6520 7370 6563 6961 6c0a  set the special.
-00001070: 2320 676c 6f62 616c 2070 6172 616d 6574  # global paramet
-00001080: 6572 2074 6f20 5472 7565 2e20 4974 276c  er to True. It'l
-00001090: 6c20 6b65 6570 2063 6163 6865 2066 696c  l keep cache fil
-000010a0: 6573 2069 6620 736f 6d65 7468 696e 6720  es if something 
-000010b0: 7765 6e74 2077 726f 6e67 2e0a 6672 6f6d  went wrong..from
-000010c0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
-000010d0: 6573 2e63 6f6e 6669 6720 696d 706f 7274  es.config import
-000010e0: 206f 7074 696f 6e73 0a0a 6f70 7469 6f6e   options..option
-000010f0: 732e 494e 5445 5241 4354 4956 455f 4d4f  s.INTERACTIVE_MO
-00001100: 4445 203d 2054 7275 650a 0a23 2053 6f6d  DE = True..# Som
-00001110: 6520 6578 616d 706c 6520 6461 7461 0a65  e example data.e
-00001120: 7665 6e74 7320 3d20 4461 7461 280a 2020  vents = Data(.  
-00001130: 2020 5b0a 2020 2020 2020 2020 7b0a 2020    [.        {.  
-00001140: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00001150: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
-00001160: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
-00001170: 3031 3035 3133 3537 3035 3536 3038 3733  0105135705560873
-00001180: 3030 303a 6436 3165 3933 3061 2d38 6430  000:d61e930a-8d0
-00001190: 302d 3131 6564 2d61 6131 612d 6433 3461  0-11ed-aa1a-d34a
-000011a0: 3631 3535 3135 3264 5f31 222c 0a20 2020  6155152d_1",.   
-000011b0: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
-000011c0: 6422 3a20 4e6f 6e65 2c0a 2020 2020 2020  d": None,.      
-000011d0: 2020 2020 2020 2269 7342 6174 6368 6564        "isBatched
-000011e0: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
-000011f0: 2020 2020 2020 2265 7665 6e74 4e61 6d65        "eventName
-00001200: 223a 2022 5365 7420 6f66 2061 7574 6f2d  ": "Set of auto-
-00001210: 6765 6e65 7261 7465 6420 6576 656e 7473  generated events
-00001220: 2066 6f72 2064 7320 6c69 6220 7465 7374   for ds lib test
-00001230: 696e 6722 2c0a 2020 2020 2020 2020 2020  ing",.          
-00001240: 2020 2265 7665 6e74 5479 7065 223a 2022    "eventType": "
-00001250: 6473 2d6c 6962 2d74 6573 742d 6576 656e  ds-lib-test-even
-00001260: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00001270: 2265 6e64 5469 6d65 7374 616d 7022 3a20  "endTimestamp": 
-00001280: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
-00001290: 3136 3732 3932 3730 3235 2c20 226e 616e  1672927025, "nan
-000012a0: 6f22 3a20 3536 3137 3531 3030 307d 2c0a  o": 561751000},.
-000012b0: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-000012c0: 7274 5469 6d65 7374 616d 7022 3a20 7b22  rtTimestamp": {"
-000012d0: 6570 6f63 6853 6563 6f6e 6422 3a20 3136  epochSecond": 16
-000012e0: 3732 3932 3730 3235 2c20 226e 616e 6f22  72927025, "nano"
-000012f0: 3a20 3536 3038 3733 3030 307d 2c0a 2020  : 560873000},.  
-00001300: 2020 2020 2020 2020 2020 2270 6172 656e            "paren
-00001310: 7445 7665 6e74 4964 223a 204e 6f6e 652c  tEventId": None,
-00001320: 0a20 2020 2020 2020 2020 2020 2022 7375  .            "su
-00001330: 6363 6573 7366 756c 223a 2054 7275 652c  ccessful": True,
-00001340: 0a20 2020 2020 2020 2020 2020 2022 626f  .            "bo
-00001350: 6f6b 4964 223a 2022 6465 6d6f 5f62 6f6f  okId": "demo_boo
-00001360: 6b5f 3122 2c0a 2020 2020 2020 2020 2020  k_1",.          
-00001370: 2020 2273 636f 7065 223a 2022 7468 322d    "scope": "th2-
-00001380: 7363 6f70 6522 2c0a 2020 2020 2020 2020  scope",.        
-00001390: 2020 2020 2261 7474 6163 6865 644d 6573      "attachedMes
-000013a0: 7361 6765 4964 7322 3a20 5b5d 2c0a 2020  sageIds": [],.  
-000013b0: 2020 2020 2020 2020 2020 2262 6f64 7922            "body"
-000013c0: 3a20 5b5d 2c0a 2020 2020 2020 2020 7d2c  : [],.        },
-000013d0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-000013e0: 2020 2020 2020 2022 6576 656e 7449 6422         "eventId"
-000013f0: 3a20 2264 656d 6f5f 626f 6f6b 5f31 3a74  : "demo_book_1:t
-00001400: 6832 2d73 636f 7065 3a32 3032 3330 3130  h2-scope:2023010
-00001410: 3531 3335 3730 3535 3633 3532 3230 3030  5135705563522000
-00001420: 3a39 6164 6262 3365 302d 3566 3862 2d34  :9adbb3e0-5f8b-4
-00001430: 6332 382d 6132 6163 2d37 3336 3165 3866  c28-a2ac-7361e8f
-00001440: 6137 3034 633e 6465 6d6f 5f62 6f6f 6b5f  a704c>demo_book_
+00000400: 735d 2823 6869 6e74 7329 0a20 2020 2020  s](#hints).     
+00000410: 202a 205b 4669 656c 6473 5265 736f 6c76   * [FieldsResolv
+00000420: 6572 5d28 2366 6965 6c64 7372 6573 6f6c  er](#fieldsresol
+00000430: 7665 7229 0a20 2020 2a20 5b32 2e34 2e20  ver).   * [2.4. 
+00000440: 4c69 6e6b 735d 2823 3234 2d6c 696e 6b73  Links](#24-links
+00000450: 290a 2a20 5b33 2e20 4265 7374 2070 7261  ).* [3. Best pra
+00000460: 6374 6963 6573 5d28 2333 2d62 6573 742d  ctices](#3-best-
+00000470: 7072 6163 7469 6365 7329 0a2a 205b 342e  practices).* [4.
+00000480: 204f 6666 6963 6961 6c20 4461 7461 536f   Official DataSo
+00000490: 7572 6365 2069 6d70 6c65 6d65 6e74 6174  urce implementat
+000004a0: 696f 6e73 5d28 2334 2d6f 6666 6963 6961  ions](#4-officia
+000004b0: 6c2d 6461 7461 736f 7572 6365 2d69 6d70  l-datasource-imp
+000004c0: 6c65 6d65 6e74 6174 696f 6e73 290a 2a20  lementations).* 
+000004d0: 5b35 2e20 4150 495d 2823 352d 6170 6929  [5. API](#5-api)
+000004e0: 0a2a 205b 362e 2045 7861 6d70 6c65 735d  .* [6. Examples]
+000004f0: 2823 362d 6578 616d 706c 6573 290a 3c21  (#6-examples).<!
+00000500: 2d2d 7465 2d2d 3e0a 0a23 2031 2e20 496e  --te-->..# 1. In
+00000510: 7472 6f64 7563 7469 6f6e 0a0a 5468 6973  troduction..This
+00000520: 2072 6570 6f73 6974 6f72 7920 6973 2061   repository is a
+00000530: 206c 6962 7261 7279 2066 6f72 2063 7265   library for cre
+00000540: 6174 696e 6720 7468 322d 6461 7461 2d73  ating th2-data-s
+00000550: 6572 7669 6365 7320 6170 706c 6963 6174  ervices applicat
+00000560: 696f 6e73 2e0a 4461 7461 2053 6572 7669  ions..Data Servi
+00000570: 6365 7320 616c 6c6f 7773 2079 6f75 2074  ces allows you t
+00000580: 6f20 6d61 6e69 7075 6c61 7465 2074 6865  o manipulate the
+00000590: 2073 7472 6561 6d20 6461 7461 2070 726f   stream data pro
+000005a0: 6365 7373 696e 6720 776f 726b 666c 6f77  cessing workflow
+000005b0: 2075 7369 6e67 2070 6970 656c 696e 696e   using pipelinin
+000005c0: 672e 0a0a 5468 6520 6c69 6272 6172 7927  g...The library'
+000005d0: 7320 6665 6174 7572 6573 3a0a 0a2d 2050  s features:..- P
+000005e0: 726f 7669 6465 7320 636f 7265 2069 6e74  rovides core int
+000005f0: 6572 6661 6365 2066 6f72 2064 6576 656c  erface for devel
+00000600: 6f70 696e 6720 6461 7461 2073 6f75 7263  oping data sourc
+00000610: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+00000620: 730a 2d20 576f 726b 2077 6974 6820 6974  s.- Work with it
+00000630: 6572 6162 6c65 206f 626a 6563 7473 2028  erable objects (
+00000640: 6c69 7374 2c20 7475 706c 652c 2065 7463  list, tuple, etc
+00000650: 2069 6e63 6c75 6469 6e67 2066 696c 6573   including files
+00000660: 2920 7669 6120 5f44 6174 6120 6f62 6a65  ) via _Data obje
+00000670: 6374 5f20 7573 696e 6720 6974 7320 6665  ct_ using its fe
+00000680: 6174 7572 6573 0a2d 204d 616e 6970 756c  atures.- Manipul
+00000690: 6174 6520 7468 6520 776f 726b 666c 6f77  ate the workflow
+000006a0: 2074 6f20 6d61 6b65 2073 6f6d 6520 616e   to make some an
+000006b0: 616c 7973 6973 2062 7920 5f44 6174 6120  alysis by _Data 
+000006c0: 6f62 6a65 6374 5f20 6d65 7468 6f64 730a  object_ methods.
+000006d0: 2d20 5573 6520 7469 6d65 7374 616d 7020  - Use timestamp 
+000006e0: 636f 6e76 6572 7465 7220 696d 706c 656d  converter implem
+000006f0: 656e 7461 7469 6f6e 7320 6f72 2075 7365  entations or use
+00000700: 2062 6173 6520 636c 6173 7320 746f 2063   base class to c
+00000710: 7265 6174 6520 6375 7374 6f6d 2063 6f6e  reate custom con
+00000720: 7665 7274 6572 730a 2d20 4275 696c 6420  verters.- Build 
+00000730: 4576 656e 7420 5472 6565 7320 2845 7665  Event Trees (Eve
+00000740: 6e74 5472 6565 2c20 4576 656e 7454 7265  ntTree, EventTre
+00000750: 6543 6f6c 6c65 6374 696f 6e20 616e 6420  eCollection and 
+00000760: 5061 7265 6e74 4576 656e 7454 7265 6543  ParentEventTreeC
+00000770: 6f6c 6c65 6374 696f 6e20 636c 6173 7365  ollection classe
+00000780: 7329 0a0a 576f 726b 666c 6f77 206d 616e  s)..Workflow man
+00000790: 6970 756c 6174 696f 6e20 746f 6f6c 7320  ipulation tools 
+000007a0: 616c 6c6f 7773 2079 6f75 3a0a 0a2d 2046  allows you:..- F
+000007b0: 696c 7465 7269 6e67 2073 7472 6561 6d20  iltering stream 
+000007c0: 6461 7461 2028 6044 6174 612e 6669 6c74  data (`Data.filt
+000007d0: 6572 6020 6d65 7468 6f64 290a 2d20 5472  er` method).- Tr
+000007e0: 616e 7366 6f72 6d69 6e67 2073 7472 6561  ansforming strea
+000007f0: 6d20 6461 7461 2028 6044 6174 612e 6d61  m data (`Data.ma
+00000800: 7060 206d 6574 686f 6429 0a2d 204c 696d  p` method).- Lim
+00000810: 6974 696e 6720 7468 6520 6e75 6d62 6572  iting the number
+00000820: 206f 6620 7072 6f63 6573 7365 6420 7374   of processed st
+00000830: 7265 616d 696e 6720 6461 7461 2028 6044  reaming data (`D
+00000840: 6174 612e 6c69 6d69 7460 206d 6574 686f  ata.limit` metho
+00000850: 6429 0a0a 5468 6572 6520 6973 2061 6c73  d)..There is als
+00000860: 6f20 616e 6f74 6865 7220 7061 7274 206f  o another part o
+00000870: 6620 5f64 6174 6120 7365 7276 6963 6573  f _data services
+00000880: 5f0a 0a2d 205b 7468 322d 6461 7461 2d73  _..- [th2-data-s
+00000890: 6572 7669 6365 732d 7574 696c 735d 2868  ervices-utils](h
+000008a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000008b0: 6d2f 7468 322d 6e65 742f 7468 322d 6461  m/th2-net/th2-da
+000008c0: 7461 2d73 6572 7669 6365 732d 7574 696c  ta-services-util
+000008d0: 7329 2e20 4974 2773 2061 2073 6574 206f  s). It's a set o
+000008e0: 6620 746f 6f6c 7320 746f 2070 6572 666f  f tools to perfo
+000008f0: 726d 2074 6865 206d 6f73 740a 2020 636f  rm the most.  co
+00000900: 6d6d 6f6e 2061 6e61 6c79 7369 7320 7461  mmon analysis ta
+00000910: 736b 732e 0a0a 2320 322e 2047 6574 7469  sks...# 2. Getti
+00000920: 6e67 2073 7461 7274 6564 0a0a 2323 2032  ng started..## 2
+00000930: 2e31 2e20 496e 7374 616c 6c61 7469 6f6e  .1. Installation
+00000940: 0a0a 2323 2320 436f 7265 0a0a 2d20 4672  ..### Core..- Fr
+00000950: 6f6d 2050 7950 4920 2870 6970 2920 2020  om PyPI (pip)   
+00000960: 0a20 2054 6869 7320 7061 636b 6167 6520  .  This package 
+00000970: 6361 6e20 6265 2066 6f75 6e64 206f 6e20  can be found on 
+00000980: 5b50 7950 495d 2868 7474 7073 3a2f 2f70  [PyPI](https://p
+00000990: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+000009a0: 7468 322d 6461 7461 2d73 6572 7669 6365  th2-data-service
+000009b0: 732f 2022 7468 322d 6461 7461 2d73 6572  s/ "th2-data-ser
+000009c0: 7669 6365 7322 292e 0a20 2020 2060 6060  vices")..    ```
+000009d0: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+000009e0: 2074 6832 2d64 6174 612d 7365 7276 6963   th2-data-servic
+000009f0: 6573 0a20 2020 2060 6060 0a0a 2d20 4672  es.    ```..- Fr
+00000a00: 6f6d 2053 6f75 7263 650a 2020 2020 6060  om Source.    ``
+00000a10: 600a 2020 2020 6769 7420 636c 6f6e 6520  `.    git clone 
+00000a20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000a30: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d64  om/th2-net/th2-d
+00000a40: 6174 612d 7365 7276 6963 6573 0a20 2020  ata-services.   
+00000a50: 2070 6970 2069 6e73 7461 6c6c 2074 6832   pip install th2
+00000a60: 2d64 6174 612d 7365 7276 6963 6573 2f0a  -data-services/.
+00000a70: 2020 2020 6060 600a 0a23 2323 2044 6174      ```..### Dat
+00000a80: 6120 736f 7572 6365 7320 2870 726f 7669  a sources (provi
+00000a90: 6465 7273 290a 0a53 696e 6365 2060 7631  ders)..Since `v1
+00000aa0: 2e33 2e30 602c 2074 6865 206c 6962 7261  .3.0`, the libra
+00000ab0: 7279 2064 6f65 736e 2774 2070 726f 7669  ry doesn't provi
+00000ac0: 6465 2064 6174 6120 736f 7572 6365 2064  de data source d
+00000ad0: 6570 656e 6465 6e63 6965 732e 0a0a 596f  ependencies...Yo
+00000ae0: 7520 7368 6f75 6c64 2070 726f 7669 6465  u should provide
+00000af0: 2069 7420 6d61 6e75 616c 6c79 2064 7572   it manually dur
+00000b00: 696e 6720 696e 7374 616c 6c61 7469 6f6e  ing installation
+00000b10: 2e20 0a59 6f75 206a 7573 7420 6e65 6564  . .You just need
+00000b20: 2074 6f20 6164 6420 7371 7561 7265 2062   to add square b
+00000b30: 7261 636b 6574 7320 6166 7465 7220 6c69  rackets after li
+00000b40: 6272 6172 7920 6e61 6d65 2061 6e64 2070  brary name and p
+00000b50: 7574 2064 6570 656e 6465 6e63 7920 6e61  ut dependency na
+00000b60: 6d65 2e0a 0a60 6060 0a70 6970 2069 6e73  me...```.pip ins
+00000b70: 7461 6c6c 2074 6832 2d64 6174 612d 7365  tall th2-data-se
+00000b80: 7276 6963 6573 5b64 6570 656e 6465 6e63  rvices[dependenc
+00000b90: 795f 6e61 6d65 5d0a 6060 600a 0a2a 2a44  y_name].```..**D
+00000ba0: 6570 656e 6465 6e63 6965 7320 6c69 7374  ependencies list
+00000bb0: 2a2a 200a 0a7c 2020 6465 7065 6e64 656e  ** ..|  dependen
+00000bc0: 6379 206e 616d 6520 207c 2070 726f 7669  cy name  | provi
+00000bd0: 6465 7220 7665 7273 696f 6e20 2020 2020  der version     
+00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bf0: 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.|:-----------
+00000c00: 2d2d 2d2d 2d2d 3a7c 2d2d 2d2d 2d2d 2d2d  ------:|--------
+00000c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00000c30: 0a7c 2020 2020 2020 206c 7764 7020 2020  .|       lwdp   
+00000c40: 2020 2020 207c 206c 6174 6573 7420 7665       | latest ve
+00000c50: 7273 696f 6e20 6f66 206c 7764 7020 2020  rsion of lwdp   
+00000c60: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00000c70: 2020 2020 2020 206c 7764 7032 2020 2020         lwdp2    
+00000c80: 2020 207c 206c 6174 6573 7420 7665 7273     | latest vers
+00000c90: 696f 6e20 6f66 206c 7764 7020 7632 2020  ion of lwdp v2  
+00000ca0: 2020 2020 2020 2020 2020 207c 0a7c 2075             |.| u
+00000cb0: 7469 6c73 2d72 7074 2d76 6965 7765 7220  tils-rpt-viewer 
+00000cc0: 207c 206c 6174 6573 7420 7665 7273 696f   | latest versio
+00000cd0: 6e20 6f66 2075 7469 6c73 2d72 7074 2d76  n of utils-rpt-v
+00000ce0: 6965 7765 7220 2020 207c 0a7c 2075 7469  iewer    |.| uti
+00000cf0: 6c73 2d72 7074 2d76 6965 7765 7235 207c  ls-rpt-viewer5 |
+00000d00: 206c 6174 6573 7420 7665 7273 696f 6e20   latest version 
+00000d10: 6f66 2075 7469 6c73 2d72 7074 2d76 6965  of utils-rpt-vie
+00000d20: 7765 7220 7635 207c 0a7c 2020 2075 7469  wer v5 |.|   uti
+00000d30: 6c73 2d61 6476 616e 6365 6420 207c 206c  ls-advanced  | l
+00000d40: 6174 6573 7420 7665 7273 696f 6e20 6f66  atest version of
+00000d50: 2064 732d 7574 696c 7320 2020 2020 2020   ds-utils       
+00000d60: 2020 2020 207c 0a0a 2a2a 4578 616d 706c       |..**Exampl
+00000d70: 652a 2a0a 0a60 6060 0a70 6970 2069 6e73  e**..```.pip ins
+00000d80: 7461 6c6c 2074 6832 2d64 6174 612d 7365  tall th2-data-se
+00000d90: 7276 6963 6573 5b6c 7764 7031 5d0a 6060  rvices[lwdp1].``
+00000da0: 600a 0a23 2320 322e 322e 2045 7861 6d70  `..## 2.2. Examp
+00000db0: 6c65 0a0a 4120 676f 6f64 2c20 7368 6f72  le..A good, shor
+00000dc0: 7420 6578 616d 706c 6520 6973 2077 6f72  t example is wor
+00000dd0: 7468 2061 2074 686f 7573 616e 6420 776f  th a thousand wo
+00000de0: 7264 732e 0a0a 5468 6973 2065 7861 6d70  rds...This examp
+00000df0: 6c65 2073 686f 7773 2062 6173 6963 2075  le shows basic u
+00000e00: 7361 6765 206f 6620 6c69 6272 6172 7927  sage of library'
+00000e10: 7320 6665 6174 7572 6573 2e0a 0a5b 5468  s features...[Th
+00000e20: 6520 666f 6c6c 6f77 696e 6720 6578 616d  e following exam
+00000e30: 706c 6520 6173 2061 2066 696c 655d 2865  ple as a file](e
+00000e40: 7861 6d70 6c65 732f 6765 745f 7374 6172  xamples/get_star
+00000e50: 7465 645f 6578 616d 706c 652e 7079 292e  ted_example.py).
+00000e60: 0a0a 3c21 2d2d 2073 7461 7274 2067 6574  ..<!-- start get
+00000e70: 5f73 7461 7274 6564 5f65 7861 6d70 6c65  _started_example
+00000e80: 2e70 7920 2d2d 3e0a 6060 6070 7974 686f  .py -->.```pytho
+00000e90: 6e0a 6672 6f6d 2074 7970 696e 6720 696d  n.from typing im
+00000ea0: 706f 7274 2054 7570 6c65 2c20 4c69 7374  port Tuple, List
+00000eb0: 2c20 4f70 7469 6f6e 616c 2c20 4765 6e65  , Optional, Gene
+00000ec0: 7261 746f 720a 6672 6f6d 2064 6174 6574  rator.from datet
+00000ed0: 696d 6520 696d 706f 7274 2064 6174 6574  ime import datet
+00000ee0: 696d 650a 0a66 726f 6d20 7468 325f 6461  ime..from th2_da
+00000ef0: 7461 5f73 6572 7669 6365 732e 6461 7461  ta_services.data
+00000f00: 2069 6d70 6f72 7420 4461 7461 0a66 726f   import Data.fro
+00000f10: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
+00000f20: 6365 732e 6576 656e 745f 7472 6565 2069  ces.event_tree i
+00000f30: 6d70 6f72 7420 4576 656e 7454 7265 652c  mport EventTree,
+00000f40: 2045 7665 6e74 5472 6565 436f 6c6c 6563   EventTreeCollec
+00000f50: 7469 6f6e 2c20 5061 7265 6e74 4576 656e  tion, ParentEven
+00000f60: 7454 7265 6543 6f6c 6c65 6374 696f 6e2c  tTreeCollection,
+00000f70: 2049 4554 4344 7269 7665 720a 6672 6f6d   IETCDriver.from
+00000f80: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
+00000f90: 6573 2e69 6e74 6572 6661 6365 7320 696d  es.interfaces im
+00000fa0: 706f 7274 2049 4461 7461 536f 7572 6365  port IDataSource
+00000fb0: 0a66 726f 6d20 7468 325f 6461 7461 5f73  .from th2_data_s
+00000fc0: 6572 7669 6365 732e 7574 696c 732e 636f  ervices.utils.co
+00000fd0: 6e76 6572 7465 7273 2069 6d70 6f72 7420  nverters import 
+00000fe0: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
+00000ff0: 722c 2044 6174 6574 696d 6553 7472 696e  r, DatetimeStrin
+00001000: 6743 6f6e 7665 7274 6572 2c20 5072 6f74  gConverter, Prot
+00001010: 6f62 7566 5469 6d65 7374 616d 7043 6f6e  obufTimestampCon
+00001020: 7665 7274 6572 0a0a 2320 5b30 5d20 4c69  verter..# [0] Li
+00001030: 6220 636f 6e66 6967 7572 6174 696f 6e0a  b configuration.
+00001040: 2320 5b30 2e31 5d20 496e 7465 7261 6374  # [0.1] Interact
+00001050: 6976 6520 6f72 2053 6372 6970 7420 6d6f  ive or Script mo
+00001060: 6465 0a23 2049 6620 796f 7520 7573 6520  de.# If you use 
+00001070: 7468 6520 6c69 6220 696e 2069 6e74 6572  the lib in inter
+00001080: 6163 7469 7665 206d 6f64 6520 286a 7570  active mode (jup
+00001090: 7974 6572 2c20 6970 7974 686f 6e29 2069  yter, ipython) i
+000010a0: 7427 7320 7265 636f 6d6d 656e 6465 6420  t's recommended 
+000010b0: 746f 2073 6574 2074 6865 2073 7065 6369  to set the speci
+000010c0: 616c 0a23 2067 6c6f 6261 6c20 7061 7261  al.# global para
+000010d0: 6d65 7465 7220 746f 2054 7275 652e 2049  meter to True. I
+000010e0: 7427 6c6c 206b 6565 7020 6361 6368 6520  t'll keep cache 
+000010f0: 6669 6c65 7320 6966 2073 6f6d 6574 6869  files if somethi
+00001100: 6e67 2077 656e 7420 7772 6f6e 672e 0a66  ng went wrong..f
+00001110: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
+00001120: 7669 6365 732e 636f 6e66 6967 2069 6d70  vices.config imp
+00001130: 6f72 7420 6f70 7469 6f6e 730a 0a6f 7074  ort options..opt
+00001140: 696f 6e73 2e49 4e54 4552 4143 5449 5645  ions.INTERACTIVE
+00001150: 5f4d 4f44 4520 3d20 5472 7565 0a0a 2320  _MODE = True..# 
+00001160: 536f 6d65 2065 7861 6d70 6c65 2064 6174  Some example dat
+00001170: 610a 6576 656e 7473 203d 2044 6174 6128  a.events = Data(
+00001180: 0a20 2020 205b 0a20 2020 2020 2020 207b  .    [.        {
+00001190: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
+000011a0: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
+000011b0: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
+000011c0: 3032 3330 3130 3531 3335 3730 3535 3630  0230105135705560
+000011d0: 3837 3330 3030 3a64 3631 6539 3330 612d  873000:d61e930a-
+000011e0: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
+000011f0: 3334 6136 3135 3531 3532 645f 3122 2c0a  34a6155152d_1",.
+00001200: 2020 2020 2020 2020 2020 2020 2262 6174              "bat
+00001210: 6368 4964 223a 204e 6f6e 652c 0a20 2020  chId": None,.   
+00001220: 2020 2020 2020 2020 2022 6973 4261 7463           "isBatc
+00001230: 6865 6422 3a20 4661 6c73 652c 0a20 2020  hed": False,.   
+00001240: 2020 2020 2020 2020 2022 6576 656e 744e           "eventN
+00001250: 616d 6522 3a20 2253 6574 206f 6620 6175  ame": "Set of au
+00001260: 746f 2d67 656e 6572 6174 6564 2065 7665  to-generated eve
+00001270: 6e74 7320 666f 7220 6473 206c 6962 2074  nts for ds lib t
+00001280: 6573 7469 6e67 222c 0a20 2020 2020 2020  esting",.       
+00001290: 2020 2020 2022 6576 656e 7454 7970 6522       "eventType"
+000012a0: 3a20 2264 732d 6c69 622d 7465 7374 2d65  : "ds-lib-test-e
+000012b0: 7665 6e74 222c 0a20 2020 2020 2020 2020  vent",.         
+000012c0: 2020 2022 656e 6454 696d 6573 7461 6d70     "endTimestamp
+000012d0: 223a 207b 2265 706f 6368 5365 636f 6e64  ": {"epochSecond
+000012e0: 223a 2031 3637 3239 3237 3032 352c 2022  ": 1672927025, "
+000012f0: 6e61 6e6f 223a 2035 3631 3735 3130 3030  nano": 561751000
+00001300: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
+00001310: 7374 6172 7454 696d 6573 7461 6d70 223a  startTimestamp":
+00001320: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
+00001330: 2031 3637 3239 3237 3032 352c 2022 6e61   1672927025, "na
+00001340: 6e6f 223a 2035 3630 3837 3330 3030 7d2c  no": 560873000},
+00001350: 0a20 2020 2020 2020 2020 2020 2022 7061  .            "pa
+00001360: 7265 6e74 4576 656e 7449 6422 3a20 4e6f  rentEventId": No
+00001370: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00001380: 2273 7563 6365 7373 6675 6c22 3a20 5472  "successful": Tr
+00001390: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+000013a0: 2262 6f6f 6b49 6422 3a20 2264 656d 6f5f  "bookId": "demo_
+000013b0: 626f 6f6b 5f31 222c 0a20 2020 2020 2020  book_1",.       
+000013c0: 2020 2020 2022 7363 6f70 6522 3a20 2274       "scope": "t
+000013d0: 6832 2d73 636f 7065 222c 0a20 2020 2020  h2-scope",.     
+000013e0: 2020 2020 2020 2022 6174 7461 6368 6564         "attached
+000013f0: 4d65 7373 6167 6549 6473 223a 205b 5d2c  MessageIds": [],
+00001400: 0a20 2020 2020 2020 2020 2020 2022 626f  .            "bo
+00001410: 6479 223a 205b 5d2c 0a20 2020 2020 2020  dy": [],.       
+00001420: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+00001430: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00001440: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
 00001450: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
 00001460: 3031 3035 3133 3537 3035 3536 3335 3232  0105135705563522
-00001470: 3030 303a 6436 3165 3933 3061 2d38 6430  000:d61e930a-8d0
-00001480: 302d 3131 6564 2d61 6131 612d 6433 3461  0-11ed-aa1a-d34a
-00001490: 3631 3535 3135 3264 5f32 222c 0a20 2020  6155152d_2",.   
-000014a0: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
-000014b0: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
-000014c0: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
-000014d0: 3130 3531 3335 3730 3535 3633 3532 3230  1051357055635220
-000014e0: 3030 3a39 6164 6262 3365 302d 3566 3862  00:9adbb3e0-5f8b
-000014f0: 2d34 6332 382d 6132 6163 2d37 3336 3165  -4c28-a2ac-7361e
-00001500: 3866 6137 3034 6322 2c0a 2020 2020 2020  8fa704c",.      
-00001510: 2020 2020 2020 2269 7342 6174 6368 6564        "isBatched
-00001520: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
-00001530: 2020 2020 2022 6576 656e 744e 616d 6522       "eventName"
-00001540: 3a20 2250 6c61 696e 2065 7665 6e74 2031  : "Plain event 1
-00001550: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00001560: 6576 656e 7454 7970 6522 3a20 2264 732d  eventType": "ds-
-00001570: 6c69 622d 7465 7374 2d65 7665 6e74 222c  lib-test-event",
-00001580: 0a20 2020 2020 2020 2020 2020 2022 656e  .            "en
-00001590: 6454 696d 6573 7461 6d70 223a 207b 2265  dTimestamp": {"e
-000015a0: 706f 6368 5365 636f 6e64 223a 2031 3637  pochSecond": 167
-000015b0: 3239 3237 3032 352c 2022 6e61 6e6f 223a  2927025, "nano":
-000015c0: 2035 3633 3634 3030 3030 7d2c 0a20 2020   563640000},.   
-000015d0: 2020 2020 2020 2020 2022 7374 6172 7454           "startT
-000015e0: 696d 6573 7461 6d70 223a 207b 2265 706f  imestamp": {"epo
-000015f0: 6368 5365 636f 6e64 223a 2031 3637 3239  chSecond": 16729
-00001600: 3237 3032 352c 2022 6e61 6e6f 223a 2035  27025, "nano": 5
-00001610: 3633 3532 3230 3030 7d2c 0a20 2020 2020  63522000},.     
-00001620: 2020 2020 2020 2022 7061 7265 6e74 4576         "parentEv
-00001630: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
-00001640: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
-00001650: 3032 3330 3130 3531 3335 3730 3535 3630  0230105135705560
-00001660: 3837 3330 3030 3a64 3631 6539 3330 612d  873000:d61e930a-
-00001670: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
-00001680: 3334 6136 3135 3531 3532 645f 3122 2c0a  34a6155152d_1",.
-00001690: 2020 2020 2020 2020 2020 2020 2273 7563              "suc
-000016a0: 6365 7373 6675 6c22 3a20 5472 7565 2c0a  cessful": True,.
-000016b0: 2020 2020 2020 2020 2020 2020 2262 6f6f              "boo
-000016c0: 6b49 6422 3a20 2264 656d 6f5f 626f 6f6b  kId": "demo_book
-000016d0: 5f31 222c 0a20 2020 2020 2020 2020 2020  _1",.           
-000016e0: 2022 7363 6f70 6522 3a20 2274 6832 2d73   "scope": "th2-s
-000016f0: 636f 7065 222c 0a20 2020 2020 2020 2020  cope",.         
-00001700: 2020 2022 6174 7461 6368 6564 4d65 7373     "attachedMess
-00001710: 6167 6549 6473 223a 205b 5d2c 0a20 2020  ageIds": [],.   
-00001720: 2020 2020 2020 2020 2022 626f 6479 223a           "body":
-00001730: 207b 2274 7970 6522 3a20 226d 6573 7361   {"type": "messa
-00001740: 6765 222c 2022 6461 7461 223a 2022 6473  ge", "data": "ds
-00001750: 2d6c 6962 2074 6573 7420 626f 6479 227d  -lib test body"}
-00001760: 2c0a 2020 2020 2020 2020 7d2c 0a20 2020  ,.        },.   
-00001770: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00001780: 2020 2022 6576 656e 7449 6422 3a20 2264     "eventId": "d
-00001790: 656d 6f5f 626f 6f6b 5f31 3a74 6832 2d73  emo_book_1:th2-s
-000017a0: 636f 7065 3a32 3032 3330 3130 3531 3335  cope:20230105135
-000017b0: 3730 3535 3633 3532 3230 3030 3a39 6164  705563522000:9ad
-000017c0: 6262 3365 302d 3566 3862 2d34 6332 382d  bb3e0-5f8b-4c28-
-000017d0: 6132 6163 2d37 3336 3165 3866 6137 3034  a2ac-7361e8fa704
-000017e0: 633e 6465 6d6f 5f62 6f6f 6b5f 313a 7468  c>demo_book_1:th
+00001470: 3030 303a 3961 6462 6233 6530 2d35 6638  000:9adbb3e0-5f8
+00001480: 622d 3463 3238 2d61 3261 632d 3733 3631  b-4c28-a2ac-7361
+00001490: 6538 6661 3730 3463 3e64 656d 6f5f 626f  e8fa704c>demo_bo
+000014a0: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
+000014b0: 3032 3330 3130 3531 3335 3730 3535 3633  0230105135705563
+000014c0: 3532 3230 3030 3a64 3631 6539 3330 612d  522000:d61e930a-
+000014d0: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
+000014e0: 3334 6136 3135 3531 3532 645f 3222 2c0a  34a6155152d_2",.
+000014f0: 2020 2020 2020 2020 2020 2020 2262 6174              "bat
+00001500: 6368 4964 223a 2022 6465 6d6f 5f62 6f6f  chId": "demo_boo
+00001510: 6b5f 313a 7468 322d 7363 6f70 653a 3230  k_1:th2-scope:20
+00001520: 3233 3031 3035 3133 3537 3035 3536 3335  2301051357055635
+00001530: 3232 3030 303a 3961 6462 6233 6530 2d35  22000:9adbb3e0-5
+00001540: 6638 622d 3463 3238 2d61 3261 632d 3733  f8b-4c28-a2ac-73
+00001550: 3631 6538 6661 3730 3463 222c 0a20 2020  61e8fa704c",.   
+00001560: 2020 2020 2020 2020 2022 6973 4261 7463           "isBatc
+00001570: 6865 6422 3a20 5472 7565 2c0a 2020 2020  hed": True,.    
+00001580: 2020 2020 2020 2020 2265 7665 6e74 4e61          "eventNa
+00001590: 6d65 223a 2022 506c 6169 6e20 6576 656e  me": "Plain even
+000015a0: 7420 3122 2c0a 2020 2020 2020 2020 2020  t 1",.          
+000015b0: 2020 2265 7665 6e74 5479 7065 223a 2022    "eventType": "
+000015c0: 6473 2d6c 6962 2d74 6573 742d 6576 656e  ds-lib-test-even
+000015d0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+000015e0: 2265 6e64 5469 6d65 7374 616d 7022 3a20  "endTimestamp": 
+000015f0: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
+00001600: 3136 3732 3932 3730 3235 2c20 226e 616e  1672927025, "nan
+00001610: 6f22 3a20 3536 3336 3430 3030 307d 2c0a  o": 563640000},.
+00001620: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
+00001630: 7274 5469 6d65 7374 616d 7022 3a20 7b22  rtTimestamp": {"
+00001640: 6570 6f63 6853 6563 6f6e 6422 3a20 3136  epochSecond": 16
+00001650: 3732 3932 3730 3235 2c20 226e 616e 6f22  72927025, "nano"
+00001660: 3a20 3536 3335 3232 3030 307d 2c0a 2020  : 563522000},.  
+00001670: 2020 2020 2020 2020 2020 2270 6172 656e            "paren
+00001680: 7445 7665 6e74 4964 223a 2022 6465 6d6f  tEventId": "demo
+00001690: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
+000016a0: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
+000016b0: 3536 3038 3733 3030 303a 6436 3165 3933  560873000:d61e93
+000016c0: 3061 2d38 6430 302d 3131 6564 2d61 6131  0a-8d00-11ed-aa1
+000016d0: 612d 6433 3461 3631 3535 3135 3264 5f31  a-d34a6155152d_1
+000016e0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000016f0: 7375 6363 6573 7366 756c 223a 2054 7275  successful": Tru
+00001700: 652c 0a20 2020 2020 2020 2020 2020 2022  e,.            "
+00001710: 626f 6f6b 4964 223a 2022 6465 6d6f 5f62  bookId": "demo_b
+00001720: 6f6f 6b5f 3122 2c0a 2020 2020 2020 2020  ook_1",.        
+00001730: 2020 2020 2273 636f 7065 223a 2022 7468      "scope": "th
+00001740: 322d 7363 6f70 6522 2c0a 2020 2020 2020  2-scope",.      
+00001750: 2020 2020 2020 2261 7474 6163 6865 644d        "attachedM
+00001760: 6573 7361 6765 4964 7322 3a20 5b5d 2c0a  essageIds": [],.
+00001770: 2020 2020 2020 2020 2020 2020 2262 6f64              "bod
+00001780: 7922 3a20 7b22 7479 7065 223a 2022 6d65  y": {"type": "me
+00001790: 7373 6167 6522 2c20 2264 6174 6122 3a20  ssage", "data": 
+000017a0: 2264 732d 6c69 6220 7465 7374 2062 6f64  "ds-lib test bod
+000017b0: 7922 7d2c 0a20 2020 2020 2020 207d 2c0a  y"},.        },.
+000017c0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000017d0: 2020 2020 2020 2265 7665 6e74 4964 223a        "eventId":
+000017e0: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
 000017f0: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
-00001800: 3133 3537 3035 3536 3337 3537 3030 303a  135705563757000:
-00001810: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
-00001820: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
-00001830: 3135 3264 5f33 222c 0a20 2020 2020 2020  152d_3",.       
-00001840: 2020 2020 2022 6261 7463 6849 6422 3a20       "batchId": 
-00001850: 2264 656d 6f5f 626f 6f6b 5f31 3a74 6832  "demo_book_1:th2
-00001860: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
-00001870: 3335 3730 3535 3633 3532 3230 3030 3a39  35705563522000:9
-00001880: 6164 6262 3365 302d 3566 3862 2d34 6332  adbb3e0-5f8b-4c2
-00001890: 382d 6132 6163 2d37 3336 3165 3866 6137  8-a2ac-7361e8fa7
-000018a0: 3034 6322 2c0a 2020 2020 2020 2020 2020  04c",.          
-000018b0: 2020 2269 7342 6174 6368 6564 223a 2054    "isBatched": T
-000018c0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-000018d0: 2022 6576 656e 744e 616d 6522 3a20 2250   "eventName": "P
-000018e0: 6c61 696e 2065 7665 6e74 2032 222c 0a20  lain event 2",. 
-000018f0: 2020 2020 2020 2020 2020 2022 6576 656e             "even
-00001900: 7454 7970 6522 3a20 2264 732d 6c69 622d  tType": "ds-lib-
-00001910: 7465 7374 2d65 7665 6e74 222c 0a20 2020  test-event",.   
-00001920: 2020 2020 2020 2020 2022 656e 6454 696d           "endTim
-00001930: 6573 7461 6d70 223a 207b 2265 706f 6368  estamp": {"epoch
-00001940: 5365 636f 6e64 223a 2031 3637 3239 3237  Second": 1672927
-00001950: 3032 352c 2022 6e61 6e6f 223a 2035 3633  025, "nano": 563
-00001960: 3739 3130 3030 7d2c 0a20 2020 2020 2020  791000},.       
-00001970: 2020 2020 2022 7374 6172 7454 696d 6573       "startTimes
-00001980: 7461 6d70 223a 207b 2265 706f 6368 5365  tamp": {"epochSe
-00001990: 636f 6e64 223a 2031 3637 3239 3237 3032  cond": 167292702
-000019a0: 352c 2022 6e61 6e6f 223a 2035 3633 3735  5, "nano": 56375
-000019b0: 3730 3030 7d2c 0a20 2020 2020 2020 2020  7000},.         
-000019c0: 2020 2022 7061 7265 6e74 4576 656e 7449     "parentEventI
-000019d0: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
-000019e0: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
-000019f0: 3130 3531 3335 3730 3535 3630 3837 3330  1051357055608730
-00001a00: 3030 3a64 3631 6539 3330 612d 3864 3030  00:d61e930a-8d00
-00001a10: 2d31 3165 642d 6161 3161 2d64 3334 6136  -11ed-aa1a-d34a6
-00001a20: 3135 3531 3532 645f 3122 2c0a 2020 2020  155152d_1",.    
-00001a30: 2020 2020 2020 2020 2273 7563 6365 7373          "success
-00001a40: 6675 6c22 3a20 5472 7565 2c0a 2020 2020  ful": True,.    
-00001a50: 2020 2020 2020 2020 2262 6f6f 6b49 6422          "bookId"
-00001a60: 3a20 2264 656d 6f5f 626f 6f6b 5f31 222c  : "demo_book_1",
-00001a70: 0a20 2020 2020 2020 2020 2020 2022 7363  .            "sc
-00001a80: 6f70 6522 3a20 2274 6832 2d73 636f 7065  ope": "th2-scope
-00001a90: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00001aa0: 6174 7461 6368 6564 4d65 7373 6167 6549  attachedMessageI
-00001ab0: 6473 223a 205b 5d2c 0a20 2020 2020 2020  ds": [],.       
-00001ac0: 2020 2020 2022 626f 6479 223a 207b 2274       "body": {"t
-00001ad0: 7970 6522 3a20 226d 6573 7361 6765 222c  ype": "message",
-00001ae0: 2022 6461 7461 223a 2022 6473 2d6c 6962   "data": "ds-lib
-00001af0: 2074 6573 7420 626f 6479 227d 2c0a 2020   test body"},.  
-00001b00: 2020 2020 2020 7d2c 0a20 2020 205d 0a29        },.    ].)
-00001b10: 0a0a 2320 5b31 5d20 576f 726b 696e 6720  ..# [1] Working 
-00001b20: 7769 7468 2061 2044 6174 6120 6f62 6a65  with a Data obje
-00001b30: 6374 2e0a 2320 5b31 2e31 5d20 4669 6c74  ct..# [1.1] Filt
-00001b40: 6572 2e0a 6669 6c74 6572 6564 5f65 7665  er..filtered_eve
-00001b50: 6e74 733a 2044 6174 6120 3d20 6576 656e  nts: Data = even
-00001b60: 7473 2e66 696c 7465 7228 6c61 6d62 6461  ts.filter(lambda
-00001b70: 2065 3a20 655b 2262 6f64 7922 5d20 213d   e: e["body"] !=
-00001b80: 205b 5d29 2020 2320 4669 6c74 6572 2065   [])  # Filter e
-00001b90: 7665 6e74 7320 7769 7468 2065 6d70 7479  vents with empty
-00001ba0: 2062 6f64 792e 0a0a 0a23 205b 312e 325d   body....# [1.2]
-00001bb0: 204d 6170 2e0a 6465 6620 7472 616e 7366   Map..def transf
-00001bc0: 6f72 6d5f 6675 6e63 7469 6f6e 2872 6563  orm_function(rec
-00001bd0: 6f72 6429 3a0a 2020 2020 7265 7475 726e  ord):.    return
-00001be0: 207b 2265 7665 6e74 4e61 6d65 223a 2072   {"eventName": r
-00001bf0: 6563 6f72 645b 2265 7665 6e74 4e61 6d65  ecord["eventName
-00001c00: 225d 2c20 2273 7563 6365 7373 6675 6c22  "], "successful"
-00001c10: 3a20 7265 636f 7264 5b22 7375 6363 6573  : record["succes
-00001c20: 7366 756c 225d 7d0a 0a0a 6669 6c74 6572  sful"]}...filter
-00001c30: 6564 5f61 6e64 5f6d 6170 7065 645f 6576  ed_and_mapped_ev
-00001c40: 656e 7473 203d 2066 696c 7465 7265 645f  ents = filtered_
-00001c50: 6576 656e 7473 2e6d 6170 2874 7261 6e73  events.map(trans
-00001c60: 666f 726d 5f66 756e 6374 696f 6e29 0a0a  form_function)..
-00001c70: 2320 5b31 2e33 5d20 4461 7461 2070 6970  # [1.3] Data pip
-00001c80: 656c 696e 652e 0a23 2020 2020 2020 2049  eline..#       I
-00001c90: 6e73 7465 6164 206f 6620 646f 696e 6720  nstead of doing 
-00001ca0: 6461 7461 2074 7261 6e73 666f 726d 6174  data transformat
-00001cb0: 696f 6e73 2073 7465 7020 6279 2073 7465  ions step by ste
-00001cc0: 7020 796f 7520 6361 6e20 646f 2069 7420  p you can do it 
-00001cd0: 696e 206f 6e65 206c 696e 652e 0a66 696c  in one line..fil
-00001ce0: 7465 7265 645f 616e 645f 6d61 7070 6564  tered_and_mapped
-00001cf0: 5f65 7665 6e74 735f 6279 5f70 6970 656c  _events_by_pipel
-00001d00: 696e 6520 3d20 6576 656e 7473 2e66 696c  ine = events.fil
-00001d10: 7465 7228 6c61 6d62 6461 2065 3a20 655b  ter(lambda e: e[
-00001d20: 2262 6f64 7922 5d20 213d 205b 5d29 2e6d  "body"] != []).m
-00001d30: 6170 2874 7261 6e73 666f 726d 5f66 756e  ap(transform_fun
-00001d40: 6374 696f 6e29 0a23 2043 6f6e 7465 6e74  ction).# Content
-00001d50: 206f 6620 7468 6573 6520 7477 6f20 4461   of these two Da
-00001d60: 7461 206f 626a 6563 7473 2073 686f 756c  ta objects shoul
-00001d70: 6420 6265 2065 7175 616c 2e0a 6173 7365  d be equal..asse
-00001d80: 7274 206c 6973 7428 6669 6c74 6572 6564  rt list(filtered
-00001d90: 5f61 6e64 5f6d 6170 7065 645f 6576 656e  _and_mapped_even
-00001da0: 7473 2920 3d3d 206c 6973 7428 6669 6c74  ts) == list(filt
-00001db0: 6572 6564 5f61 6e64 5f6d 6170 7065 645f  ered_and_mapped_
-00001dc0: 6576 656e 7473 5f62 795f 7069 7065 6c69  events_by_pipeli
-00001dd0: 6e65 290a 0a23 205b 312e 345d 2053 6966  ne)..# [1.4] Sif
-00001de0: 742e 2053 6b69 7020 7468 6520 6669 7273  t. Skip the firs
-00001df0: 7420 6665 7720 6974 656d 7320 6f72 206c  t few items or l
-00001e00: 696d 6974 2074 6865 6d2e 0a64 6174 6120  imit them..data 
-00001e10: 3d20 4461 7461 285b 312c 2032 2c20 332c  = Data([1, 2, 3,
-00001e20: 2034 2c20 352c 2036 2c20 372c 2038 2c20   4, 5, 6, 7, 8, 
-00001e30: 392c 2031 302c 2031 312c 2031 322c 2031  9, 10, 11, 12, 1
-00001e40: 332c 2031 342c 2031 355d 290a 6974 656d  3, 14, 15]).item
-00001e50: 735f 6672 6f6d 5f31 315f 746f 5f65 6e64  s_from_11_to_end
-00001e60: 3a20 4765 6e65 7261 746f 7220 3d20 6461  : Generator = da
-00001e70: 7461 2e73 6966 7428 736b 6970 3d31 3029  ta.sift(skip=10)
-00001e80: 0a6f 6e6c 795f 6669 7273 745f 3130 5f69  .only_first_10_i
-00001e90: 7465 6d73 3a20 4765 6e65 7261 746f 7220  tems: Generator 
-00001ea0: 3d20 6461 7461 2e73 6966 7428 6c69 6d69  = data.sift(limi
-00001eb0: 743d 3130 290a 0a23 205b 312e 355d 2043  t=10)..# [1.5] C
-00001ec0: 6861 6e67 696e 6720 6361 6368 6520 7374  hanging cache st
-00001ed0: 6174 7573 2e0a 6576 656e 7473 2e75 7365  atus..events.use
-00001ee0: 5f63 6163 6865 2854 7275 6529 0a23 206f  _cache(True).# o
-00001ef0: 7220 6a75 7374 0a65 7665 6e74 732e 7573  r just.events.us
-00001f00: 655f 6361 6368 6528 2920 2023 2049 6620  e_cache()  # If 
-00001f10: 796f 7520 7761 6e74 2074 6f20 6163 7469  you want to acti
-00001f20: 7661 7465 2063 6163 6865 2e0a 2320 5b31  vate cache..# [1
-00001f30: 2e36 5d20 5761 6c6b 2074 6872 6f75 6768  .6] Walk through
-00001f40: 2064 6174 612e 0a66 6f72 2065 7665 6e74   data..for event
-00001f50: 2069 6e20 6576 656e 7473 3a0a 2020 2020   in events:.    
-00001f60: 2320 446f 2073 6f6d 6574 6869 6e67 2077  # Do something w
-00001f70: 6974 6820 6576 656e 7420 2865 7665 6e74  ith event (event
-00001f80: 2069 7320 6120 6469 6374 292e 0a20 2020   is a dict)..   
-00001f90: 2070 7269 6e74 2865 7665 6e74 290a 2320   print(event).# 
-00001fa0: 4166 7465 7220 6669 7273 7420 6974 6572  After first iter
-00001fb0: 6174 696f 6e20 7468 6520 6576 656e 7473  ation the events
-00001fc0: 2068 6173 2061 2063 6163 6865 2066 696c   has a cache fil
-00001fd0: 652e 0a23 204e 6f77 2074 6865 7920 7769  e..# Now they wi
-00001fe0: 6c6c 2062 6520 7573 6564 2069 6e20 7468  ll be used in th
-00001ff0: 6520 6361 6368 6520 696e 2074 6865 206e  e cache in the n
-00002000: 6578 7420 6974 6572 6174 696f 6e2e 0a0a  ext iteration...
-00002010: 2320 5b31 2e37 5d20 4765 7420 6e75 6d62  # [1.7] Get numb
-00002020: 6572 206f 6620 7468 6520 656c 656d 656e  er of the elemen
-00002030: 7473 2069 6e20 7468 6520 4461 7461 206f  ts in the Data o
-00002040: 626a 6563 742e 0a6e 756d 6265 725f 6f66  bject..number_of
-00002050: 5f65 7665 6e74 7320 3d20 6576 656e 7473  _events = events
-00002060: 2e6c 656e 0a0a 2320 5b31 2e38 5d20 4368  .len..# [1.8] Ch
-00002070: 6563 6b20 7468 6174 2044 6174 6120 6f62  eck that Data ob
-00002080: 6a65 6374 2069 736e 2774 2065 6d70 7479  ject isn't empty
-00002090: 2e0a 2320 5468 6520 6461 7461 2073 6f75  ..# The data sou
-000020a0: 7263 6520 7368 6f75 6c64 2062 6520 6e6f  rce should be no
-000020b0: 7420 656d 7074 792e 0a61 7373 6572 7420  t empty..assert 
-000020c0: 6576 656e 7473 2e69 735f 656d 7074 7920  events.is_empty 
-000020d0: 6973 2046 616c 7365 0a0a 2320 5b31 2e39  is False..# [1.9
-000020e0: 5d20 436f 6e76 6572 7420 4461 7461 206f  ] Convert Data o
-000020f0: 626a 6563 7420 746f 2074 6865 206c 6973  bject to the lis
-00002100: 7420 6f66 2065 6c65 6d65 6e74 7328 6576  t of elements(ev
-00002110: 656e 7473 206f 7220 6d65 7373 6167 6573  ents or messages
-00002120: 292e 0a23 2042 6520 6361 7265 6675 6c2c  )..# Be careful,
-00002130: 2074 6869 7320 6361 6e20 7461 6b65 2074   this can take t
-00002140: 6f6f 206d 7563 6820 6d65 6d6f 7279 2e0a  oo much memory..
-00002150: 6576 656e 7473 5f6c 6973 7420 3d20 6c69  events_list = li
-00002160: 7374 2865 7665 6e74 7329 0a0a 2320 5b31  st(events)..# [1
-00002170: 2e31 305d 2054 6865 2063 6163 6865 2069  .10] The cache i
-00002180: 6e68 6572 6974 616e 6365 2e0a 2320 4372  nheritance..# Cr
-00002190: 6561 7465 7320 6120 6e65 7720 4461 7461  eates a new Data
-000021a0: 206f 626a 6563 7420 7468 6174 2077 696c   object that wil
-000021b0: 6c20 7573 6520 6361 6368 6520 6672 6f6d  l use cache from
-000021c0: 2074 6865 2065 7665 6e74 7320 4461 7461   the events Data
-000021d0: 206f 626a 6563 742e 0a65 7665 6e74 735f   object..events_
-000021e0: 6669 6c74 6572 6564 3a20 4461 7461 203d  filtered: Data =
-000021f0: 2065 7665 6e74 732e 6669 6c74 6572 286c   events.filter(l
-00002200: 616d 6264 6120 7265 636f 7264 3a20 7265  ambda record: re
-00002210: 636f 7264 2e67 6574 2822 6261 7463 6849  cord.get("batchI
-00002220: 6422 2929 0a0a 2320 4e65 7720 4461 7461  d"))..# New Data
-00002230: 206f 626a 6563 7473 2064 6f6e 2774 2075   objects don't u
-00002240: 7365 2074 6865 6972 206f 776e 2063 6163  se their own cac
-00002250: 6865 2062 7920 6465 6661 756c 7420 6275  he by default bu
-00002260: 7420 7573 6520 7468 6520 6361 6368 6520  t use the cache 
-00002270: 6f66 2074 6865 2070 6172 656e 7420 4461  of the parent Da
-00002280: 7461 206f 626a 6563 742e 0a23 2055 7365  ta object..# Use
-00002290: 2075 7365 5f63 6163 6865 206d 6574 686f   use_cache metho
-000022a0: 6420 746f 2061 6374 6976 6174 6520 6361  d to activate ca
-000022b0: 6368 696e 672e 0a23 2041 6674 6572 2074  ching..# After t
-000022c0: 6861 742c 2074 6865 2044 6174 6120 6f62  hat, the Data ob
-000022d0: 6a65 6374 2077 696c 6c20 6372 6561 7465  ject will create
-000022e0: 2069 7473 206f 776e 2063 6163 6865 2066   its own cache f
-000022f0: 696c 652e 0a65 7665 6e74 735f 6669 6c74  ile..events_filt
-00002300: 6572 6564 2e75 7365 5f63 6163 6865 2829  ered.use_cache()
-00002310: 0a0a 6c69 7374 2865 7665 6e74 735f 6669  ..list(events_fi
-00002320: 6c74 6572 6564 2920 2023 204a 7573 7420  ltered)  # Just 
-00002330: 746f 2069 7465 7261 7465 2044 6174 6120  to iterate Data 
-00002340: 6f62 6a65 6374 2028 6361 6368 6520 6669  object (cache fi
-00002350: 6c65 2077 696c 6c20 6265 2063 7265 6174  le will be creat
-00002360: 6564 292e 0a0a 6669 6c74 6572 6564 5f65  ed)...filtered_e
-00002370: 7665 6e74 735f 7479 7065 7320 3d20 6576  vents_types = ev
-00002380: 656e 7473 5f66 696c 7465 7265 642e 6d61  ents_filtered.ma
-00002390: 7028 6c61 6d62 6461 2072 6563 6f72 643a  p(lambda record:
-000023a0: 207b 2265 7665 6e74 5479 7065 223a 2072   {"eventType": r
-000023b0: 6563 6f72 642e 6765 7428 2265 7665 6e74  ecord.get("event
-000023c0: 5479 7065 2229 7d29 0a0a 6576 656e 7473  Type")})..events
-000023d0: 5f77 6974 686f 7574 5f74 7970 6573 5f77  _without_types_w
-000023e0: 6974 685f 6261 7463 6820 3d20 6669 6c74  ith_batch = filt
-000023f0: 6572 6564 5f65 7665 6e74 735f 7479 7065  ered_events_type
-00002400: 732e 6669 6c74 6572 286c 616d 6264 6120  s.filter(lambda 
-00002410: 7265 636f 7264 3a20 6e6f 7420 7265 636f  record: not reco
-00002420: 7264 2e67 6574 2822 6576 656e 7454 7970  rd.get("eventTyp
-00002430: 6522 2929 0a65 7665 6e74 735f 7769 7468  e")).events_with
-00002440: 6f75 745f 7479 7065 735f 7769 7468 5f62  out_types_with_b
-00002450: 6174 6368 2e75 7365 5f63 6163 6865 2829  atch.use_cache()
-00002460: 0a0a 2320 5b31 2e31 315d 2044 6174 6120  ..# [1.11] Data 
-00002470: 6f62 6a65 6374 7320 6a6f 696e 696e 672e  objects joining.
-00002480: 0a23 2059 6f75 2068 6176 6520 7468 6520  .# You have the 
-00002490: 666f 6c6c 6f77 696e 6720 3320 4461 7461  following 3 Data
-000024a0: 206f 626a 6563 7473 2e0a 6431 203d 2044   objects..d1 = D
-000024b0: 6174 6128 5b31 2c20 322c 2033 5d29 0a64  ata([1, 2, 3]).d
-000024c0: 3220 3d20 4461 7461 285b 2261 222c 207b  2 = Data(["a", {
-000024d0: 2269 6422 3a20 3132 337d 2c20 2263 225d  "id": 123}, "c"]
-000024e0: 290a 6433 203d 2044 6174 6128 5b37 2c20  ).d3 = Data([7, 
-000024f0: 382c 2039 5d29 0a23 2059 6f75 2063 616e  8, 9]).# You can
-00002500: 206a 6f69 6e20 4461 7461 206f 626a 6563   join Data objec
-00002510: 7473 2069 6e20 666f 6c6c 6f77 696e 6720  ts in following 
-00002520: 7761 7973 2e0a 2320 506c 6561 7365 206e  ways..# Please n
-00002530: 6f74 652c 206e 6577 2044 6174 6120 6f62  ote, new Data ob
-00002540: 6a65 6374 2077 696c 6c20 6861 7665 2063  ject will have c
-00002550: 6163 6865 2073 7461 7475 7320 3d3d 2046  ache status == F
-00002560: 616c 7365 2e0a 6461 7461 5f76 6961 5f69  alse..data_via_i
-00002570: 6e69 7420 3d20 4461 7461 285b 6431 2c20  nit = Data([d1, 
-00002580: 6432 2c20 6433 5d29 0a64 6174 615f 7669  d2, d3]).data_vi
-00002590: 615f 6164 6420 3d20 6431 202b 2064 3220  a_add = d1 + d2 
-000025a0: 2b20 6433 0a64 6174 615f 7769 7468 5f6e  + d3.data_with_n
-000025b0: 6f6e 5f64 6174 615f 6f62 6a5f 7669 615f  on_data_obj_via_
-000025c0: 696e 6974 203d 2044 6174 6128 5b64 312c  init = Data([d1,
-000025d0: 205b 2261 222c 207b 2269 6422 3a20 3132   ["a", {"id": 12
-000025e0: 337d 2c20 2263 225d 2c20 6433 5d29 0a64  3}, "c"], d3]).d
-000025f0: 6174 615f 7769 7468 5f6e 6f6e 5f64 6174  ata_with_non_dat
-00002600: 615f 6f62 6a5f 7669 615f 6164 6420 3d20  a_obj_via_add = 
-00002610: 6431 202b 205b 2261 222c 207b 2269 6422  d1 + ["a", {"id"
-00002620: 3a20 3132 337d 2c20 2263 225d 202b 2064  : 123}, "c"] + d
-00002630: 330a 2320 596f 7520 6361 6e20 6a6f 696e  3.# You can join
-00002640: 2063 7572 7265 6e74 2044 6174 6120 6f62   current Data ob
-00002650: 6a65 6374 206f 6e20 706c 6163 6520 7573  ject on place us
-00002660: 696e 6720 2b3d 2e0a 2320 4974 2077 696c  ing +=..# It wil
-00002670: 6c20 6b65 6570 2063 6163 6865 2073 7461  l keep cache sta
-00002680: 7475 732e 0a64 3120 2b3d 2064 3320 2023  tus..d1 += d3  #
-00002690: 2064 3120 7769 6c6c 2062 6563 6f6d 6520   d1 will become 
-000026a0: 4461 7461 285b 312c 322c 332c 372c 382c  Data([1,2,3,7,8,
-000026b0: 395d 290a 0a23 205b 312e 3132 5d20 4275  9])..# [1.12] Bu
-000026c0: 696c 6420 616e 6420 7265 6164 2044 6174  ild and read Dat
-000026d0: 6120 6f62 6a65 6374 2063 6163 6865 2066  a object cache f
-000026e0: 696c 6573 2e0a 6576 656e 7473 2e62 7569  iles..events.bui
-000026f0: 6c64 5f63 6163 6865 2822 6361 6368 655f  ld_cache("cache_
-00002700: 6669 6c65 6e61 6d65 5f6f 725f 7061 7468  filename_or_path
-00002710: 2229 0a64 6174 615f 6f62 6a5f 6672 6f6d  ").data_obj_from
-00002720: 5f63 6163 6865 203d 2044 6174 612e 6672  _cache = Data.fr
-00002730: 6f6d 5f63 6163 6865 5f66 696c 6528 2263  om_cache_file("c
-00002740: 6163 6865 5f66 696c 656e 616d 655f 6f72  ache_filename_or
-00002750: 5f70 6174 6822 290a 0a23 205b 325d 2057  _path")..# [2] W
-00002760: 6f72 6b69 6e67 2077 6974 6820 636f 6e76  orking with conv
-00002770: 6572 7465 7273 2e0a 2320 5468 6572 6520  erters..# There 
-00002780: 6172 6520 6375 7272 656e 746c 7920 7468  are currently th
-00002790: 7265 6520 696d 706c 656d 656e 7461 7469  ree implementati
-000027a0: 6f6e 7320 6f66 2049 5469 6d65 7374 616d  ons of ITimestam
-000027b0: 7043 6f6e 7665 7274 6572 2063 6c61 7373  pConverter class
-000027c0: 3a20 4461 7465 7469 6d65 436f 6e76 6572  : DatetimeConver
-000027d0: 7465 2c20 4461 7465 7469 6d65 5374 7269  te, DatetimeStri
-000027e0: 6e67 436f 6e76 6572 7465 7220 616e 6420  ngConverter and 
-000027f0: 5072 6f74 6f62 7566 5469 6d65 7374 616d  ProtobufTimestam
-00002800: 7043 6f6e 7665 7274 6572 2e0a 2320 5468  pConverter..# Th
-00002810: 6579 2061 6c6c 2069 6d70 6c65 6d65 6e74  ey all implement
-00002820: 2073 616d 6520 6d65 7468 6f64 7320 6672   same methods fr
-00002830: 6f6d 2062 6173 6520 636c 6173 732e 0a23  om base class..#
-00002840: 204e 6f74 6520 7468 6174 2073 6f6d 6520   Note that some 
-00002850: 6163 6375 7261 6379 206d 6179 2062 6520  accuracy may be 
-00002860: 6c6f 7374 2064 7572 696e 6720 636f 6e76  lost during conv
-00002870: 6572 7369 6f6e 2e0a 2320 4966 2066 6f72  ersion..# If for
-00002880: 2065 7861 6d70 6c65 2079 6f75 2075 7365   example you use
-00002890: 2074 6f5f 6d69 6372 6f73 6563 6f6e 6473   to_microseconds
-000028a0: 206e 616e 6f73 6563 6f6e 6473 2077 696c   nanoseconds wil
-000028b0: 6c20 6265 2063 7574 206f 6666 2069 6e73  l be cut off ins
-000028c0: 7465 6164 206f 6620 726f 756e 6469 6e67  tead of rounding
-000028d0: 2e0a 0a23 205b 322e 315d 2044 6174 6574  ...# [2.1] Datet
-000028e0: 696d 6543 6f6e 7665 7274 6572 2e0a 2320  imeConverter..# 
-000028f0: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
-00002900: 7220 7461 6b65 7320 6461 7465 7469 6d65  r takes datetime
-00002910: 2e64 6174 6574 696d 6520 6f62 6a65 6374  .datetime object
-00002920: 2061 7320 696e 7075 742e 0a0a 6461 7465   as input...date
-00002930: 7469 6d65 5f6f 626a 203d 2064 6174 6574  time_obj = datet
-00002940: 696d 6528 7965 6172 3d32 3032 332c 206d  ime(year=2023, m
-00002950: 6f6e 7468 3d31 2c20 6461 793d 352c 2068  onth=1, day=5, h
-00002960: 6f75 723d 3134 2c20 6d69 6e75 7465 3d33  our=14, minute=3
-00002970: 382c 2073 6563 6f6e 643d 3235 2c20 6d69  8, second=25, mi
-00002980: 6372 6f73 6563 6f6e 643d 3134 3630 290a  crosecond=1460).
-00002990: 0a23 2049 7420 6861 7320 6d65 7468 6f64  .# It has method
-000029a0: 7320 7468 6174 2072 6574 7572 6e20 7468  s that return th
-000029b0: 6520 6461 7465 7469 6d65 2069 6e20 6469  e datetime in di
-000029c0: 6666 6572 656e 7420 666f 726d 6173 3a0a  fferent formas:.
-000029d0: 0a64 6174 655f 6d73 203d 2044 6174 6574  .date_ms = Datet
-000029e0: 696d 6543 6f6e 7665 7274 6572 2e74 6f5f  imeConverter.to_
-000029f0: 6d69 6c6c 6973 6563 6f6e 6473 2864 6174  milliseconds(dat
-00002a00: 6574 696d 655f 6f62 6a29 0a64 6174 655f  etime_obj).date_
-00002a10: 7573 203d 2044 6174 6574 696d 6543 6f6e  us = DatetimeCon
-00002a20: 7665 7274 6572 2e74 6f5f 6d69 6372 6f73  verter.to_micros
-00002a30: 6563 6f6e 6473 2864 6174 6574 696d 655f  econds(datetime_
-00002a40: 6f62 6a29 0a23 2043 6f6e 7665 7274 696e  obj).# Convertin
-00002a50: 6720 746f 206e 616e 6f73 6563 6f6e 6473  g to nanoseconds
-00002a60: 206a 7573 7473 2061 6464 7320 7468 7265   justs adds thre
-00002a70: 6520 7472 6169 6c69 6e67 207a 6572 6f73  e trailing zeros
-00002a80: 2061 7320 6461 7465 7469 6d65 206f 626a   as datetime obj
-00002a90: 6563 7420 646f 6573 6e27 7420 6861 7665  ect doesn't have
-00002aa0: 206e 616e 6f73 6563 6f6e 6473 2e0a 6461   nanoseconds..da
-00002ab0: 7465 5f6e 7320 3d20 4461 7465 7469 6d65  te_ns = Datetime
-00002ac0: 436f 6e76 6572 7465 722e 746f 5f6e 616e  Converter.to_nan
-00002ad0: 6f73 6563 6f6e 6473 2864 6174 6574 696d  oseconds(datetim
-00002ae0: 655f 6f62 6a29 0a0a 2320 5b32 2e32 5d20  e_obj)..# [2.2] 
-00002af0: 4461 7465 7469 6d65 5374 7269 6e67 436f  DatetimeStringCo
-00002b00: 6e76 6572 7465 720a 2320 4461 7465 7469  nverter.# Dateti
-00002b10: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
-00002b20: 7220 7461 6b65 7320 7374 7269 6e67 2069  r takes string i
-00002b30: 6e20 2279 7979 792d 4d4d 2d64 6454 4848  n "yyyy-MM-ddTHH
-00002b40: 3a6d 6d3a 7373 5b2e 5353 5353 5353 5353  :mm:ss[.SSSSSSSS
-00002b50: 535d 5a22 2066 6f72 6d61 742e 0a0a 6461  S]Z" format...da
-00002b60: 7465 5f73 7472 696e 6720 3d20 2232 3032  te_string = "202
-00002b70: 332d 3031 2d30 3554 3134 3a33 383a 3235  3-01-05T14:38:25
-00002b80: 2e30 3031 3436 5a22 0a0a 2320 5765 2068  .00146Z"..# We h
-00002b90: 6176 6520 7361 6d65 206d 6574 686f 6473  ave same methods
-00002ba0: 2061 7320 696e 2044 6174 6574 696d 6543   as in DatetimeC
-00002bb0: 6f6e 7665 7274 6572 0a64 6174 655f 6d73  onverter.date_ms
-00002bc0: 5f66 726f 6d5f 7374 7269 6e67 203d 2044  _from_string = D
-00002bd0: 6174 6574 696d 6553 7472 696e 6743 6f6e  atetimeStringCon
-00002be0: 7665 7274 6572 2e74 6f5f 6d69 6c6c 6973  verter.to_millis
-00002bf0: 6563 6f6e 6473 2864 6174 655f 7374 7269  econds(date_stri
-00002c00: 6e67 290a 6461 7465 5f75 735f 6672 6f6d  ng).date_us_from
-00002c10: 5f73 7472 696e 6720 3d20 4461 7465 7469  _string = Dateti
-00002c20: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
-00002c30: 722e 746f 5f6d 6963 726f 7365 636f 6e64  r.to_microsecond
-00002c40: 7328 6461 7465 5f73 7472 696e 6729 0a64  s(date_string).d
-00002c50: 6174 655f 6e73 5f66 726f 6d5f 7374 7269  ate_ns_from_stri
-00002c60: 6e67 203d 2044 6174 6574 696d 6553 7472  ng = DatetimeStr
-00002c70: 696e 6743 6f6e 7665 7274 6572 2e74 6f5f  ingConverter.to_
-00002c80: 6e61 6e6f 7365 636f 6e64 7328 6461 7465  nanoseconds(date
-00002c90: 5f73 7472 696e 6729 0a0a 2320 5765 2063  _string)..# We c
-00002ca0: 616e 2061 6c73 6f20 6765 7420 6461 7465  an also get date
-00002cb0: 7469 6d65 206f 626a 6563 7420 6672 6f6d  time object from
-00002cc0: 2073 7472 696e 670a 6461 7465 7469 6d65   string.datetime
-00002cd0: 5f66 726f 6d5f 7374 7269 6e67 203d 2044  _from_string = D
-00002ce0: 6174 6574 696d 6553 7472 696e 6743 6f6e  atetimeStringCon
-00002cf0: 7665 7274 6572 2e74 6f5f 6461 7465 7469  verter.to_dateti
-00002d00: 6d65 2864 6174 655f 7374 7269 6e67 290a  me(date_string).
-00002d10: 0a23 205b 322e 335d 2050 726f 746f 6275  .# [2.3] Protobu
-00002d20: 6654 696d 6573 7461 6d70 436f 6e76 6572  fTimestampConver
-00002d30: 7465 720a 2320 5072 6f74 6f62 7566 2074  ter.# Protobuf t
-00002d40: 696d 6573 7461 6d70 7320 6d75 7374 2062  imestamps must b
-00002d50: 6520 696e 2066 6f72 6d20 7b22 6570 6f63  e in form {"epoc
-00002d60: 6853 6563 6f6e 6422 3a20 7365 636f 6e64  hSecond": second
-00002d70: 732c 2022 6e61 6e6f 223a 206e 616e 6f73  s, "nano": nanos
-00002d80: 6563 6f6e 6473 7d0a 0a70 726f 746f 6275  econds}..protobu
-00002d90: 665f 7469 6d65 7374 616d 7020 3d20 7b22  f_timestamp = {"
-00002da0: 6570 6f63 6853 6563 6f6e 6422 3a20 3136  epochSecond": 16
-00002db0: 3732 3932 3935 3035 2c20 226e 616e 6f22  72929505, "nano"
-00002dc0: 3a20 315f 3436 305f 3030 307d 0a0a 6461  : 1_460_000}..da
-00002dd0: 7465 5f6d 735f 6672 6f6d 5f74 696d 6573  te_ms_from_times
-00002de0: 7461 6d70 203d 2050 726f 746f 6275 6654  tamp = ProtobufT
-00002df0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
-00002e00: 722e 746f 5f6d 696c 6c69 7365 636f 6e64  r.to_millisecond
-00002e10: 7328 7072 6f74 6f62 7566 5f74 696d 6573  s(protobuf_times
-00002e20: 7461 6d70 290a 6461 7465 5f75 735f 6672  tamp).date_us_fr
-00002e30: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
-00002e40: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
-00002e50: 436f 6e76 6572 7465 722e 746f 5f6d 6963  Converter.to_mic
-00002e60: 726f 7365 636f 6e64 7328 7072 6f74 6f62  roseconds(protob
-00002e70: 7566 5f74 696d 6573 7461 6d70 290a 6461  uf_timestamp).da
-00002e80: 7465 5f6e 735f 6672 6f6d 5f74 696d 6573  te_ns_from_times
-00002e90: 7461 6d70 203d 2050 726f 746f 6275 6654  tamp = ProtobufT
-00002ea0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
-00002eb0: 722e 746f 5f6e 616e 6f73 6563 6f6e 6473  r.to_nanoseconds
-00002ec0: 2870 726f 746f 6275 665f 7469 6d65 7374  (protobuf_timest
-00002ed0: 616d 7029 0a64 6174 6574 696d 655f 6672  amp).datetime_fr
-00002ee0: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
-00002ef0: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
-00002f00: 436f 6e76 6572 7465 722e 746f 5f64 6174  Converter.to_dat
-00002f10: 6574 696d 6528 7072 6f74 6f62 7566 5f74  etime(protobuf_t
-00002f20: 696d 6573 7461 6d70 290a 0a23 205b 335d  imestamp)..# [3]
-00002f30: 2057 6f72 6b69 6e67 2077 6974 6820 4576   Working with Ev
-00002f40: 656e 7454 7265 6520 616e 6420 4576 656e  entTree and Even
-00002f50: 7454 7265 6543 6f6c 6c65 6374 696f 6e2e  tTreeCollection.
-00002f60: 0a0a 2320 5b33 2e31 5d20 4275 696c 6420  ..# [3.1] Build 
-00002f70: 6120 6375 7374 6f6d 2045 7665 6e74 5472  a custom EventTr
-00002f80: 6565 0a23 2054 6f20 6372 6561 7465 2061  ee.# To create a
-00002f90: 6e20 4576 656e 7454 7265 6520 6f62 6a65  n EventTree obje
-00002fa0: 6374 2079 6f75 206e 6565 6420 746f 2070  ct you need to p
-00002fb0: 726f 7669 6465 206e 616d 652c 2069 6420  rovide name, id 
-00002fc0: 616e 6420 6461 7461 206f 6620 7468 6520  and data of the 
-00002fd0: 726f 6f74 2065 7665 6e74 2e0a 7472 6565  root event..tree
-00002fe0: 203d 2045 7665 6e74 5472 6565 2865 7665   = EventTree(eve
-00002ff0: 6e74 5f6e 616d 653d 2272 6f6f 7420 6576  nt_name="root ev
-00003000: 656e 7422 2c20 6576 656e 745f 6964 3d22  ent", event_id="
-00003010: 726f 6f74 5f69 6422 2c20 6461 7461 3d7b  root_id", data={
-00003020: 2264 6174 6122 3a20 5b31 2c20 322c 2033  "data": [1, 2, 3
-00003030: 2c20 342c 2035 5d7d 290a 0a23 2054 6f20  , 4, 5]})..# To 
-00003040: 6164 6420 6e65 7720 6e6f 6465 2075 7365  add new node use
-00003050: 2061 7070 656e 645f 6576 656e 742e 2070   append_event. p
-00003060: 6172 656e 745f 6964 2069 7320 6e65 6365  arent_id is nece
-00003070: 7373 6172 792c 2064 6174 6120 6973 206f  ssary, data is o
-00003080: 7074 696f 6e61 6c2e 0a74 7265 652e 6170  ptional..tree.ap
-00003090: 7065 6e64 5f65 7665 6e74 2865 7665 6e74  pend_event(event
-000030a0: 5f6e 616d 653d 2241 222c 2065 7665 6e74  _name="A", event
-000030b0: 5f69 643d 2241 5f69 6422 2c20 6461 7461  _id="A_id", data
-000030c0: 3d4e 6f6e 652c 2070 6172 656e 745f 6964  =None, parent_id
-000030d0: 3d22 726f 6f74 5f69 6422 290a 0a23 205b  ="root_id")..# [
-000030e0: 332e 335d 2042 7569 6c64 696e 6720 7468  3.3] Building th
-000030f0: 6520 4576 656e 7454 7265 6543 6f6c 6c65  e EventTreeColle
-00003100: 6374 696f 6e2e 0a0a 2320 4966 2079 6f75  ction...# If you
-00003110: 2064 6f6e 2774 2073 7065 6369 6679 2064   don't specify d
-00003120: 6174 615f 736f 7572 6365 2066 6f72 2074  ata_source for t
-00003130: 6865 2064 7269 7665 7220 7468 656e 2069  he driver then i
-00003140: 7420 776f 6e27 7420 7265 636f 7665 7220  t won't recover 
-00003150: 6465 7461 6368 6564 2065 7665 6e74 732e  detached events.
-00003160: 0a64 7269 7665 723a 2049 4554 4344 7269  .driver: IETCDri
-00003170: 7665 7220 2023 2059 6f75 2073 686f 756c  ver  # You shoul
-00003180: 6420 696e 6974 2045 5443 4472 6976 6572  d init ETCDriver
-00003190: 206f 626a 6563 742e 2045 2e67 2e20 6672   object. E.g. fr
-000031a0: 6f6d 204c 7744 5020 6d6f 6475 6c65 206f  om LwDP module o
-000031b0: 7220 796f 7572 2063 7573 746f 6d20 636c  r your custom cl
-000031c0: 6173 732e 0a65 7463 203d 2045 7665 6e74  ass..etc = Event
-000031d0: 5472 6565 436f 6c6c 6563 7469 6f6e 2864  TreeCollection(d
-000031e0: 7269 7665 7229 0a65 7463 2e62 7569 6c64  river).etc.build
-000031f0: 2865 7665 6e74 7329 0a0a 2320 4465 7461  (events)..# Deta
-00003200: 6368 6564 2065 7665 6e74 7320 6973 6e27  ched events isn'
-00003210: 7420 656d 7074 792e 0a61 7373 6572 7420  t empty..assert 
-00003220: 6574 632e 6765 745f 6465 7461 6368 6564  etc.get_detached
-00003230: 5f65 7665 6e74 7328 290a 0a65 7463 203d  _events()..etc =
-00003240: 2045 7665 6e74 5472 6565 436f 6c6c 6563   EventTreeCollec
-00003250: 7469 6f6e 2864 7269 7665 7229 0a23 2044  tion(driver).# D
-00003260: 6574 6163 6865 6420 6576 656e 7473 2061  etached events a
-00003270: 7265 2065 6d70 7479 2062 6563 6175 7365  re empty because
-00003280: 2074 6865 7920 7765 7265 2072 6563 6f76   they were recov
-00003290: 6572 6564 2e0a 6173 7365 7274 206e 6f74  ered..assert not
-000032a0: 2065 7463 2e67 6574 5f64 6574 6163 6865   etc.get_detache
-000032b0: 645f 6576 656e 7473 2829 0a0a 2320 5468  d_events()..# Th
-000032c0: 6520 636f 6c6c 6563 7469 6f6e 2068 6173  e collection has
-000032d0: 2045 7665 6e74 5472 6565 7320 6561 6368   EventTrees each
-000032e0: 2077 6974 6820 6120 7472 6565 206f 6620   with a tree of 
-000032f0: 6576 656e 7473 2e0a 2320 5573 696e 6720  events..# Using 
-00003300: 436f 6c6c 6563 7469 6f6e 2061 6e64 2045  Collection and E
-00003310: 7665 6e74 5472 6565 732c 2079 6f75 2063  ventTrees, you c
-00003320: 616e 2077 6f72 6b20 666c 6578 6962 6c79  an work flexibly
-00003330: 2077 6974 6820 6576 656e 7473 2e0a 0a23   with events...#
-00003340: 205b 332e 332e 315d 2047 6574 206c 6561   [3.3.1] Get lea
-00003350: 7665 7320 6f66 2061 6c6c 2074 7265 6573  ves of all trees
-00003360: 2e0a 6c65 6176 6573 3a20 5475 706c 655b  ..leaves: Tuple[
-00003370: 6469 6374 5d20 3d20 6574 632e 6765 745f  dict] = etc.get_
-00003380: 6c65 6176 6573 2829 0a0a 2320 5b33 2e33  leaves()..# [3.3
-00003390: 2e32 5d20 4765 7420 726f 6f74 7320 6964  .2] Get roots id
-000033a0: 7320 6f66 2061 6c6c 2074 7265 6573 2e0a  s of all trees..
-000033b0: 726f 6f74 733a 204c 6973 745b 7374 725d  roots: List[str]
-000033c0: 203d 2065 7463 2e67 6574 5f72 6f6f 7473   = etc.get_roots
-000033d0: 5f69 6473 2829 0a0a 2320 5b33 2e33 2e33  _ids()..# [3.3.3
-000033e0: 5d20 4669 6e64 2061 6e20 6576 656e 7420  ] Find an event 
-000033f0: 696e 2061 6c6c 2074 7265 6573 2e0a 6669  in all trees..fi
-00003400: 6e64 5f65 7665 6e74 3a20 4f70 7469 6f6e  nd_event: Option
-00003410: 616c 5b64 6963 745d 203d 2065 7463 2e66  al[dict] = etc.f
-00003420: 696e 6428 6c61 6d62 6461 2065 7665 6e74  ind(lambda event
-00003430: 3a20 2253 656e 6420 6d65 7373 6167 6522  : "Send message"
-00003440: 2069 6e20 6576 656e 745b 2265 7665 6e74   in event["event
-00003450: 5479 7065 225d 290a 0a23 205b 332e 332e  Type"])..# [3.3.
-00003460: 345d 2046 696e 6420 616c 6c20 6576 656e  4] Find all even
-00003470: 7473 2069 6e20 616c 6c20 7472 6565 732e  ts in all trees.
-00003480: 2054 6865 7265 2069 7320 616c 736f 2069   There is also i
-00003490: 7465 7261 626c 6520 7665 7273 696f 6e20  terable version 
-000034a0: 2766 696e 6461 6c6c 5f69 7465 7227 2e0a  'findall_iter'..
-000034b0: 6669 6e64 5f65 7665 6e74 733a 204c 6973  find_events: Lis
-000034c0: 745b 6469 6374 5d20 3d20 6574 632e 6669  t[dict] = etc.fi
-000034d0: 6e64 616c 6c28 6c61 6d62 6461 2065 7665  ndall(lambda eve
-000034e0: 6e74 3a20 6576 656e 745b 2273 7563 6365  nt: event["succe
-000034f0: 7373 6675 6c22 5d20 6973 2054 7275 6529  ssful"] is True)
-00003500: 0a0a 2320 5b33 2e33 2e35 5d20 4669 6e64  ..# [3.3.5] Find
-00003510: 2061 6e20 616e 6365 7374 6f72 206f 6620   an ancestor of 
-00003520: 7468 6520 6576 656e 742e 0a61 6e63 6573  the event..ances
-00003530: 746f 723a 204f 7074 696f 6e61 6c5b 6469  tor: Optional[di
-00003540: 6374 5d20 3d20 6574 632e 6669 6e64 5f61  ct] = etc.find_a
-00003550: 6e63 6573 746f 7228 0a20 2020 2022 3862  ncestor(.    "8b
-00003560: 6265 3337 3137 2d63 6635 392d 3131 6562  be3717-cf59-11eb
-00003570: 2d61 3366 372d 3039 3466 3930 3463 3361  -a3f7-094f904c3a
-00003580: 3632 222c 2066 696c 7465 723d 6c61 6d62  62", filter=lamb
-00003590: 6461 2065 7665 6e74 3a20 2252 6f6f 7445  da event: "RootE
-000035a0: 7665 6e74 2220 696e 2065 7665 6e74 5b22  vent" in event["
-000035b0: 6576 656e 744e 616d 6522 5d0a 290a 0a23  eventName"].)..#
-000035c0: 205b 332e 332e 365d 2047 6574 2063 6869   [3.3.6] Get chi
-000035d0: 6c64 7265 6e20 6f66 2074 6865 2065 7665  ldren of the eve
-000035e0: 6e74 2e20 5468 6572 6520 6973 2061 6c73  nt. There is als
-000035f0: 6f20 6974 6572 6162 6c65 2076 6572 7369  o iterable versi
-00003600: 6f6e 2027 6765 745f 6368 696c 6472 656e  on 'get_children
-00003610: 5f69 7465 7227 2e0a 6368 696c 6472 656e  _iter'..children
-00003620: 3a20 5475 706c 655b 6469 6374 5d20 3d20  : Tuple[dict] = 
-00003630: 6574 632e 6765 745f 6368 696c 6472 656e  etc.get_children
-00003640: 2822 3831 3434 3232 6531 2d39 6336 382d  ("814422e1-9c68-
-00003650: 3131 6562 2d38 3539 382d 3639 3165 6264  11eb-8598-691ebd
-00003660: 3766 3431 3364 2229 0a0a 2320 5b33 2e33  7f413d")..# [3.3
-00003670: 2e37 5d20 4765 7420 7375 6274 7265 6520  .7] Get subtree 
-00003680: 666f 7220 7370 6563 6966 6965 6420 6576  for specified ev
-00003690: 656e 742e 0a73 7562 7472 6565 3a20 4576  ent..subtree: Ev
-000036a0: 656e 7454 7265 6520 3d20 6574 632e 6765  entTree = etc.ge
-000036b0: 745f 7375 6274 7265 6528 2238 6532 3337  t_subtree("8e237
-000036c0: 3734 642d 6366 3539 2d31 3165 622d 6136  74d-cf59-11eb-a6
-000036d0: 6533 2d35 3562 6664 6232 6233 6632 3122  e3-55bfdb2b3f21"
-000036e0: 290a 0a23 205b 332e 332e 385d 2047 6574  )..# [3.3.8] Get
-000036f0: 2066 756c 6c20 7061 7468 2074 6f20 7468   full path to th
-00003700: 6520 6576 656e 742e 0a23 204c 6f6f 6b73  e event..# Looks
-00003710: 206c 696b 6520 5b61 6e63 6573 746f 725f   like [ancestor_
-00003720: 726f 6f74 2c20 616e 6365 7374 6f72 5f6c  root, ancestor_l
-00003730: 6576 656c 312c 2061 6e63 6573 746f 725f  evel1, ancestor_
-00003740: 6c65 7665 6c32 2c20 6576 656e 745d 0a65  level2, event].e
-00003750: 7665 6e74 5f70 6174 683a 204c 6973 745b  vent_path: List[
-00003760: 6469 6374 5d20 3d20 6574 632e 6765 745f  dict] = etc.get_
-00003770: 6675 6c6c 5f70 6174 6828 2238 6532 3532  full_path("8e252
-00003780: 3466 612d 6366 3539 2d31 3165 622d 6133  4fa-cf59-11eb-a3
-00003790: 6637 2d30 3934 6639 3034 6333 6136 3222  f7-094f904c3a62"
-000037a0: 290a 0a23 205b 332e 332e 395d 2047 6574  )..# [3.3.9] Get
-000037b0: 2070 6172 656e 7420 6f66 2074 6865 2065   parent of the e
-000037c0: 7665 6e74 2e0a 7061 7265 6e74 203d 2065  vent..parent = e
-000037d0: 7463 2e67 6574 5f70 6172 656e 7428 2238  tc.get_parent("8
-000037e0: 6532 3532 3466 612d 6366 3539 2d31 3165  e2524fa-cf59-11e
-000037f0: 622d 6133 6637 2d30 3934 6639 3034 6333  b-a3f7-094f904c3
-00003800: 6136 3222 290a 0a23 205b 332e 332e 3130  a62")..# [3.3.10
-00003810: 5d20 4170 7065 6e64 206e 6577 2065 7665  ] Append new eve
-00003820: 6e74 2074 6f20 7468 6520 636f 6c6c 6563  nt to the collec
-00003830: 7469 6f6e 2e0a 6574 632e 6170 7065 6e64  tion..etc.append
-00003840: 5f65 7665 6e74 280a 2020 2020 6576 656e  _event(.    even
-00003850: 743d 7b0a 2020 2020 2020 2020 2265 7665  t={.        "eve
-00003860: 6e74 4964 223a 2022 6132 3066 3565 6634  ntId": "a20f5ef4
-00003870: 2d63 3366 652d 6262 3130 2d61 3239 632d  -c3fe-bb10-a29c-
-00003880: 6464 3364 3738 3439 3039 6562 222c 0a20  dd3d784909eb",. 
-00003890: 2020 2020 2020 2022 7061 7265 6e74 4576         "parentEv
-000038a0: 656e 7449 6422 3a20 2238 6532 3532 3466  entId": "8e2524f
-000038b0: 612d 6366 3539 2d31 3165 622d 6133 6637  a-cf59-11eb-a3f7
-000038c0: 2d30 3934 6639 3034 6333 6136 3222 2c0a  -094f904c3a62",.
-000038d0: 2020 2020 2020 2020 2265 7665 6e74 4e61          "eventNa
-000038e0: 6d65 223a 2022 5374 7562 4576 656e 7422  me": "StubEvent"
-000038f0: 2c0a 2020 2020 7d0a 290a 0a23 205b 332e  ,.    }.)..# [3.
-00003900: 332e 3131 5d20 5368 6f77 2074 6865 2065  3.11] Show the e
-00003910: 6e74 6972 6520 636f 6c6c 6563 7469 6f6e  ntire collection
-00003920: 2e0a 6574 632e 7368 6f77 2829 0a0a 2320  ..etc.show()..# 
-00003930: 5b33 2e34 5d20 576f 726b 696e 6720 7769  [3.4] Working wi
-00003940: 7468 2074 6865 2045 7665 6e74 5472 6565  th the EventTree
-00003950: 2e0a 2320 4576 656e 7454 7265 6520 6861  ..# EventTree ha
-00003960: 7320 7468 6520 7361 6d65 206d 6574 686f  s the same metho
-00003970: 6473 2061 7320 4576 656e 7454 7265 6543  ds as EventTreeC
-00003980: 6f6c 6c65 6374 696f 6e2c 2062 7574 206f  ollection, but o
-00003990: 6e6c 7920 666f 7220 6974 7320 6f77 6e20  nly for its own 
-000039a0: 7472 6565 2e0a 0a23 205b 332e 342e 315d  tree...# [3.4.1]
-000039b0: 2047 6574 2063 6f6c 6c65 6374 696f 6e20   Get collection 
-000039c0: 7472 6565 732e 0a74 7265 6573 3a20 4c69  trees..trees: Li
-000039d0: 7374 5b45 7665 6e74 5472 6565 5d20 3d20  st[EventTree] = 
-000039e0: 6574 632e 6765 745f 7472 6565 7328 290a  etc.get_trees().
-000039f0: 7472 6565 3a20 4576 656e 7454 7265 6520  tree: EventTree 
-00003a00: 3d20 7472 6565 735b 305d 0a0a 2320 4275  = trees[0]..# Bu
-00003a10: 7420 4576 656e 7454 7265 6520 7072 6f76  t EventTree prov
-00003a20: 6964 6573 2061 2077 6f72 6b20 7769 7468  ides a work with
-00003a30: 2074 6865 2074 7265 652c 2062 7574 2064   the tree, but d
-00003a40: 6f65 7320 6e6f 7420 6d6f 6469 6679 2069  oes not modify i
-00003a50: 742e 0a23 2049 6620 796f 7520 7761 6e74  t..# If you want
-00003a60: 2074 6f20 6d6f 6469 6679 2074 6865 2074   to modify the t
-00003a70: 7265 652c 2075 7365 2045 7665 6e74 5472  ree, use EventTr
-00003a80: 6565 436f 6c6c 6563 7469 6f6e 732e 0a0a  eeCollections...
-00003a90: 2320 5b33 2e35 5d20 576f 726b 696e 6720  # [3.5] Working 
-00003aa0: 7769 7468 2050 6172 656e 746c 6573 7354  with ParentlessT
-00003ab0: 7265 652e 0a23 2050 6172 656e 746c 6573  ree..# Parentles
-00003ac0: 7354 7265 6520 6973 2045 7665 6e74 5472  sTree is EventTr
-00003ad0: 6565 2077 6869 6368 2068 6173 2064 6574  ee which has det
-00003ae0: 6163 6865 6420 6576 656e 7473 2077 6974  ached events wit
-00003af0: 6820 7374 7562 732e 0a70 6172 656e 746c  h stubs..parentl
-00003b00: 6573 735f 7472 6565 733a 204c 6973 745b  ess_trees: List[
-00003b10: 4576 656e 7454 7265 655d 203d 2065 7463  EventTree] = etc
-00003b20: 2e67 6574 5f70 6172 656e 746c 6573 735f  .get_parentless_
-00003b30: 7472 6565 7328 290a 0a23 205b 332e 365d  trees()..# [3.6]
-00003b40: 2057 6f72 6b69 6e67 2077 6974 6820 5061   Working with Pa
-00003b50: 7265 6e74 4576 656e 7454 7265 6543 6f6c  rentEventTreeCol
-00003b60: 6c65 6374 696f 6e2e 0a23 2050 6172 656e  lection..# Paren
-00003b70: 7445 7665 6e74 5472 6565 436f 6c6c 6563  tEventTreeCollec
-00003b80: 7469 6f6e 2069 7320 6120 7472 6565 2063  tion is a tree c
-00003b90: 6f6c 6c65 6374 696f 6e20 6c69 6b65 2045  ollection like E
-00003ba0: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
-00003bb0: 6f6e 2c0a 2320 6275 7420 6974 2068 6173  on,.# but it has
-00003bc0: 206f 6e6c 7920 6576 656e 7473 2074 6861   only events tha
-00003bd0: 7420 6861 7665 2072 6566 6572 656e 6365  t have reference
-00003be0: 732e 0a64 6174 615f 736f 7572 6365 3a20  s..data_source: 
-00003bf0: 4944 6174 6153 6f75 7263 6520 2023 2059  IDataSource  # Y
-00003c00: 6f75 2073 686f 756c 6420 696e 6974 2044  ou should init D
-00003c10: 6174 6153 6f75 7263 6520 6f62 6a65 6374  ataSource object
-00003c20: 2e20 452e 672e 2066 726f 6d20 4c77 4450  . E.g. from LwDP
-00003c30: 206d 6f64 756c 652e 0a23 2045 5443 4472   module..# ETCDr
-00003c40: 6976 6572 2068 6572 6520 6973 2061 2073  iver here is a s
-00003c50: 7475 622c 2061 6374 7561 6c6c 7920 7468  tub, actually th
-00003c60: 6520 6c69 6220 646f 6e27 7420 6861 7665  e lib don't have
-00003c70: 2073 7563 6820 636c 6173 732e 0a23 2059   such class..# Y
-00003c80: 6f75 2063 616e 2074 616b 6520 6974 2069  ou can take it i
-00003c90: 6e20 4c77 4450 206d 6f64 756c 6520 6f72  n LwDP module or
-00003ca0: 2063 7265 6174 6520 796f 7572 7365 6c66   create yourself
-00003cb0: 2063 6c61 7373 2069 6620 796f 7520 6861   class if you ha
-00003cc0: 7665 2073 6f6d 6520 7370 6563 6961 6c20  ve some special 
-00003cd0: 6576 656e 7473 2073 7472 7563 7475 7265  events structure
-00003ce0: 2e0a 6472 6976 6572 203d 2045 5443 4472  ..driver = ETCDr
-00003cf0: 6976 6572 2864 6174 615f 736f 7572 6365  iver(data_source
-00003d00: 3d64 6174 615f 736f 7572 6365 290a 6574  =data_source).et
-00003d10: 6320 3d20 5061 7265 6e74 4576 656e 7454  c = ParentEventT
-00003d20: 7265 6543 6f6c 6c65 6374 696f 6e28 6472  reeCollection(dr
-00003d30: 6976 6572 290a 6574 632e 6275 696c 6428  iver).etc.build(
-00003d40: 6576 656e 7473 290a 0a65 7463 2e73 686f  events)..etc.sho
-00003d50: 7728 290a 6060 600a 3c21 2d2d 2065 6e64  w().```.<!-- end
-00003d60: 2067 6574 5f73 7461 7274 6564 5f65 7861   get_started_exa
-00003d70: 6d70 6c65 2e70 7920 2d2d 3e0a 0a23 2320  mple.py -->..## 
-00003d80: 322e 332e 2053 686f 7274 2074 6865 6f72  2.3. Short theor
-00003d90: 790a 0a54 6865 206c 6962 7261 7279 2070  y..The library p
-00003da0: 726f 7669 6465 7320 746f 6f6c 7320 666f  rovides tools fo
-00003db0: 7220 6861 6e64 6c69 6e67 2073 7472 6561  r handling strea
-00003dc0: 6d20 6461 7461 2e20 5768 6174 2773 2061  m data. What's a
-00003dd0: 2073 7472 6561 6d3f 2049 7427 7320 6120   stream? It's a 
-00003de0: 7365 7175 656e 6365 206f 6620 656c 656d  sequence of elem
-00003df0: 656e 7473 2066 726f 6d20 6120 736f 7572  ents from a sour
-00003e00: 6365 2074 6861 740a 7375 7070 6f72 7473  ce that.supports
-00003e10: 2061 6767 7265 6761 7465 206f 7065 7261   aggregate opera
-00003e20: 7469 6f6e 732e 0a0a 2323 2320 5465 726d  tions...### Term
-00003e30: 730a 0a2d 202a 2a44 6174 6120 6f62 6a65  s..- **Data obje
-00003e40: 6374 2a2a 3a20 416e 2069 6e73 7461 6e63  ct**: An instanc
-00003e50: 6520 6f66 2060 4461 7461 6020 636c 6173  e of `Data` clas
-00003e60: 7320 7768 6963 6820 6973 2077 7261 7070  s which is wrapp
-00003e70: 6572 2075 6e64 6572 2073 7472 6561 6d2e  er under stream.
-00003e80: 0a2d 202a 2a53 6571 7565 6e63 6520 6f66  .- **Sequence of
-00003e90: 2065 6c65 6d65 6e74 732a 2a3a 0a20 2041   elements**:.  A
-00003ea0: 205f 4461 7461 206f 626a 6563 745f 2070   _Data object_ p
-00003eb0: 726f 7669 6465 7320 616e 2069 6e74 6572  rovides an inter
-00003ec0: 6661 6365 2074 6f20 6120 7365 7175 656e  face to a sequen
-00003ed0: 6365 6420 7365 7420 6f66 2076 616c 7565  ced set of value
-00003ee0: 7320 6f66 2061 2073 7065 6369 6669 6320  s of a specific 
-00003ef0: 656c 656d 656e 7420 7479 7065 2e20 5374  element type. St
-00003f00: 7265 616d 2069 6e73 6964 6520 7468 6520  ream inside the 
-00003f10: 5f44 6174 610a 2020 6f62 6a65 6374 5f20  _Data.  object_ 
-00003f20: 2a2a 646f 6e19 7420 6163 7475 616c 6c79  **don.t actually
-00003f30: 2073 746f 7265 2a2a 2065 6c65 6d65 6e74   store** element
-00003f40: 733b 2074 6865 7920 6172 6520 636f 6d70  s; they are comp
-00003f50: 7574 6564 206f 6e20 6465 6d61 6e64 2e0a  uted on demand..
-00003f60: 2d20 2a2a 6461 7461 2073 6f75 7263 652a  - **data source*
-00003f70: 2a20 2865 7861 6374 6c79 2069 6e20 736d  * (exactly in sm
-00003f80: 616c 6c20 6c65 7474 6572 7329 3a0a 2020  all letters):.  
-00003f90: 416e 7920 736f 7572 6365 206f 6620 6461  Any source of da
-00003fa0: 7461 2e20 452e 672e 205b 4c69 6768 7477  ta. E.g. [Lightw
-00003fb0: 6569 6768 7420 4461 7461 2050 726f 7669  eight Data Provi
-00003fc0: 6465 725d 2868 7474 7073 3a2f 2f67 6974  der](https://git
-00003fd0: 6875 622e 636f 6d2f 7468 322d 6e65 742f  hub.com/th2-net/
-00003fe0: 7468 322d 6c77 2d64 6174 612d 7072 6f76  th2-lw-data-prov
-00003ff0: 6964 6572 292c 2063 6f6c 6c65 6374 696f  ider), collectio
-00004000: 6e73 2c0a 2020 6172 7261 7973 2c20 6f72  ns,.  arrays, or
-00004010: 2049 2f4f 2072 6573 6f75 7263 6573 2e0a   I/O resources..
-00004020: 2d20 2a2a 4461 7461 536f 7572 6365 2a2a  - **DataSource**
-00004030: 3a0a 2020 4120 636c 6173 7320 7468 6174  :.  A class that
-00004040: 2069 7320 616e 2069 6e74 6572 6d65 6469   is an intermedi
-00004050: 6174 6520 6c69 6e6b 2062 6574 7765 656e  ate link between
-00004060: 2074 6865 2053 6f75 7263 6541 5049 2061   the SourceAPI a
-00004070: 6e64 2043 6f6d 6d61 6e64 732e 0a2d 202a  nd Commands..- *
-00004080: 2a53 6f75 7263 6541 5049 2a2a 3a0a 2020  *SourceAPI**:.  
-00004090: 4561 6368 2073 6f75 7263 6520 6861 7320  Each source has 
-000040a0: 6974 7320 6f77 6e20 4150 4920 746f 2072  its own API to r
-000040b0: 6574 7269 6576 6520 6461 7461 2e20 536f  etrieve data. So
-000040c0: 7572 6365 4150 4920 6973 2061 2063 6c61  urceAPI is a cla
-000040d0: 7373 2074 6861 7420 7072 6f76 6964 6520  ss that provide 
-000040e0: 4150 4920 666f 7220 736f 6d65 2064 6174  API for some dat
-000040f0: 6120 736f 7572 6365 2e0a 2d20 2a2a 436f  a source..- **Co
-00004100: 6d6d 616e 6473 2a2a 3a0a 2020 436c 6173  mmands**:.  Clas
-00004110: 7365 7320 7468 6174 2070 726f 7669 6465  ses that provide
-00004120: 2075 7365 722d 6672 6965 6e64 6c79 2069   user-friendly i
-00004130: 6e74 6572 6661 6365 7320 666f 7220 6765  nterfaces for ge
-00004140: 7474 696e 6720 736f 6d65 2064 6174 6120  tting some data 
-00004150: 6672 6f6d 2044 6174 6153 6f75 7263 652e  from DataSource.
-00004160: 2043 6f6d 6d61 6e64 7320 7573 6520 5f53   Commands use _S
-00004170: 6f75 7263 6541 5049 5f20 746f 0a20 2061  ourceAPI_ to.  a
-00004180: 6368 6965 7665 2069 742e 0a2d 202a 2a41  chieve it..- **A
-00004190: 6461 7074 6572 732a 2a3a 0a20 2049 7427  dapters**:.  It'
-000041a0: 7320 7369 6d69 6c61 7220 746f 2066 756e  s similar to fun
-000041b0: 6374 696f 6e20 666f 7220 6044 6174 612e  ction for `Data.
-000041c0: 6d61 7060 206d 6574 686f 642e 2041 646f  map` method. Ado
-000041d0: 7074 6162 6c65 2063 6f6d 6d61 6e64 7320  ptable commands 
-000041e0: 7573 6564 2069 7420 746f 2075 7064 6174  used it to updat
-000041f0: 6520 7468 6520 6461 7461 2073 7472 6561  e the data strea
-00004200: 6d2e 0a2d 202a 2a41 6767 7265 6761 7465  m..- **Aggregate
-00004210: 206f 7065 7261 7469 6f6e 732a 2a3a 0a20   operations**:. 
-00004220: 2043 6f6d 6d6f 6e20 6f70 6572 6174 696f   Common operatio
-00004230: 6e73 2073 7563 6820 6173 2066 696c 7465  ns such as filte
-00004240: 722c 206d 6170 2c20 6c69 6d69 7420 616e  r, map, limit an
-00004250: 6420 736f 206f 6e2e 0a2d 202a 2a57 6f72  d so on..- **Wor
-00004260: 6b66 6c6f 772a 2a3a 2041 6e20 6f72 6465  kflow**: An orde
-00004270: 7265 6420 7365 7420 6f66 205f 4167 6772  red set of _Aggr
-00004280: 6567 6174 6520 6f70 6572 6174 696f 6e73  egate operations
-00004290: 5f2e 0a0a 2323 2320 436f 6e63 6570 740a  _...### Concept.
-000042a0: 0a54 6865 206c 6962 7261 7279 2064 6573  .The library des
-000042b0: 6372 6962 6573 2074 6865 2068 6967 682d  cribes the high-
-000042c0: 6c65 7665 6c20 696e 7465 7266 6163 6573  level interfaces
-000042d0: 2060 4953 6f75 7263 6541 5049 602c 2060   `ISourceAPI`, `
-000042e0: 4944 6174 6153 6f75 7263 6560 2c20 6049  IDataSource`, `I
-000042f0: 436f 6d6d 616e 6460 2c20 6049 4164 6170  Command`, `IAdap
-00004300: 7465 7260 2e0a 0a41 6e79 2064 6174 6120  ter`...Any data 
-00004310: 736f 7572 6365 206d 7573 7420 6265 2064  source must be d
-00004320: 6573 6372 6962 6564 2062 7920 7468 6520  escribed by the 
-00004330: 6049 4461 7461 536f 7572 6365 6020 6162  `IDataSource` ab
-00004340: 7374 7261 6374 2063 6c61 7373 2e20 5468  stract class. Th
-00004350: 6573 6520 6361 6e20 6265 205f 4669 6c65  ese can be _File
-00004360: 4461 7461 536f 7572 6365 5f2c 200a 5f43  DataSource_, ._C
-00004370: 5356 4461 7461 536f 7572 6365 5f2c 205f  SVDataSource_, _
-00004380: 4442 4461 7461 536f 7572 6365 5f20 616e  DBDataSource_ an
-00004390: 6420 6f74 6865 722e 0a0a 5573 7561 6c6c  d other...Usuall
-000043a0: 792c 2064 6174 6120 736f 7572 6365 7320  y, data sources 
-000043b0: 6861 7665 2073 6f6d 6520 6b69 6e64 206f  have some kind o
-000043c0: 6620 4150 492e 2044 6174 6162 6173 6573  f API. Databases
-000043d0: 202d 2070 726f 7669 6465 2053 514c 206c   - provide SQL l
-000043e0: 616e 6775 6167 652c 2077 6865 6e20 776f  anguage, when wo
-000043f0: 726b 696e 6720 7769 7468 2061 2066 696c  rking with a fil
-00004400: 652c 2079 6f75 2063 616e 2072 6561 640a  e, you can read.
-00004410: 6c69 6e65 2062 7920 6c69 6e65 2c20 6574  line by line, et
-00004420: 632e 2054 6869 7320 4150 4920 6973 2064  c. This API is d
-00004430: 6573 6372 6962 6564 2062 7920 7468 6520  escribed by the 
-00004440: 6049 536f 7572 6365 4150 4960 2063 6c61  `ISourceAPI` cla
-00004450: 7373 2e20 4265 6361 7573 6520 6469 6666  ss. Because diff
-00004460: 6572 656e 7420 7665 7273 696f 6e73 206f  erent versions o
-00004470: 6620 7468 6520 7361 6d65 2064 6174 6120  f the same data 
-00004480: 736f 7572 6365 0a6d 6179 2068 6176 6520  source.may have 
-00004490: 6469 6666 6572 656e 7420 4150 492c 2069  different API, i
-000044a0: 7420 6973 2062 6574 7465 7220 746f 2063  t is better to c
-000044b0: 7265 6174 6520 6120 636c 6173 7320 666f  reate a class fo
-000044c0: 7220 6561 6368 2076 6572 7369 6f6e 2e0a  r each version..
-000044d0: 0a47 656e 6572 616c 6c79 2c20 6461 7461  .Generally, data
-000044e0: 2073 6f75 7263 6520 4150 4973 2061 7265   source APIs are
-000044f0: 2068 6964 6465 6e20 6265 6869 6e64 2063   hidden behind c
-00004500: 6f6e 7665 6e69 656e 7420 696e 7465 7266  onvenient interf
-00004510: 6163 6573 2e20 5468 6520 726f 6c65 206f  aces. The role o
-00004520: 6620 7468 6573 6520 696e 7465 7266 6163  f these interfac
-00004530: 6573 2069 7320 706c 6179 6564 0a62 7920  es is played.by 
-00004540: 6049 436f 6d6d 616e 6460 2063 6c61 7373  `ICommand` class
-00004550: 6573 2e0a 0a60 4941 6461 7074 6572 6020  es...`IAdapter` 
-00004560: 636c 6173 7365 7320 7472 616e 7366 6f72  classes transfor
-00004570: 6d20 6461 7461 2073 7472 6561 6d20 6c69  m data stream li
-00004580: 6b65 2066 756e 6374 696f 6e73 2066 6f72  ke functions for
-00004590: 2060 4461 7461 2e6d 6170 6020 6d65 7468   `Data.map` meth
-000045a0: 6f64 2e20 4573 7365 6e74 6961 6c6c 7920  od. Essentially 
-000045b0: 6974 2773 2074 6865 2073 616d 6520 7468  it's the same th
-000045c0: 696e 6720 6275 7420 6d6f 7265 0a66 6c65  ing but more.fle
-000045d0: 7869 626c 652e 0a0a 466f 7220 6578 616d  xible...For exam
-000045e0: 706c 652c 204c 7744 5020 4461 7461 536f  ple, LwDP DataSo
-000045f0: 7572 6365 2868 7474 7073 3a2f 2f67 6974  urce(https://git
-00004600: 6875 622e 636f 6d2f 7468 322d 6e65 742f  hub.com/th2-net/
-00004610: 7468 322d 6473 2d73 6f75 7263 652d 6c77  th2-ds-source-lw
-00004620: 6470 2920 7573 6573 2074 6865 7365 2061  dp) uses these a
-00004630: 6273 7472 6163 7420 636c 6173 7365 7320  bstract classes 
-00004640: 746f 2062 7569 6c64 2069 7473 2069 6d70  to build its imp
-00004650: 6c65 6d65 6e74 6174 696f 6e2e 596f 7520  lementation.You 
-00004660: 6361 6e20 6561 7369 6c79 2063 7265 6174  can easily creat
-00004670: 6520 796f 7572 206f 776e 2075 6e69 7175  e your own uniqu
-00004680: 6520 636f 6d6d 616e 6473 2066 6f72 205f  e commands for _
-00004690: 4c77 4450 2044 6174 6153 6f75 7263 655f  LwDP DataSource_
-000046a0: 2c20 6173 2077 656c 6c20 6173 2065 6e74  , as well as ent
-000046b0: 6972 650a 5f44 6174 6153 6f75 7263 655f  ire._DataSource_
-000046c0: 2063 6c61 7373 6573 2e20 5b48 6572 6520   classes. [Here 
-000046d0: 6973 2061 2064 6f63 756d 656e 7461 7469  is a documentati
-000046e0: 6f6e 5d28 646f 6375 6d65 6e74 6174 696f  on](documentatio
-000046f0: 6e2f 6461 7461 736f 7572 6365 2e6d 6429  n/datasource.md)
-00004700: 206f 6e20 686f 7720 746f 2069 6d70 6c65   on how to imple
-00004710: 6d65 6e74 2074 6865 7365 2069 6e74 6572  ment these inter
-00004720: 6661 6365 732e 0a0a 215b 4461 7461 2073  faces...![Data s
-00004730: 7472 6561 6d20 7069 7065 6c69 6e65 5d28  tream pipeline](
-00004740: 646f 6375 6d65 6e74 6174 696f 6e2f 696d  documentation/im
-00004750: 672f 636f 6e63 6570 742e 706e 6729 0a0a  g/concept.png)..
-00004760: 2323 2320 5374 7265 616d 206f 7065 7261  ### Stream opera
-00004770: 7469 6f6e 730a 0a46 7572 7468 6572 6d6f  tions..Furthermo
-00004780: 7265 2c20 7374 7265 616d 206f 7065 7261  re, stream opera
-00004790: 7469 6f6e 7320 6861 7665 2074 776f 2066  tions have two f
-000047a0: 756e 6461 6d65 6e74 616c 2063 6861 7261  undamental chara
-000047b0: 6374 6572 6973 7469 6373 2074 6861 7420  cteristics that 
-000047c0: 6d61 6b65 2074 6865 6d20 7665 7279 2064  make them very d
-000047d0: 6966 6665 7265 6e74 2066 726f 6d20 636f  ifferent from co
-000047e0: 6c6c 6563 7469 6f6e 0a6f 7065 7261 7469  llection.operati
-000047f0: 6f6e 733a 205f 5069 7065 6c69 6e69 6e67  ons: _Pipelining
-00004800: 5f20 616e 6420 5f49 6e74 6572 6e61 6c20  _ and _Internal 
-00004810: 6974 6572 6174 696f 6e5f 2e0a 0a23 2323  iteration_...###
-00004820: 2320 5069 7065 6c69 6e69 6e67 0a0a 4d61  # Pipelining..Ma
-00004830: 6e79 2073 7472 6561 6d20 6f70 6572 6174  ny stream operat
-00004840: 696f 6e73 2072 6574 7572 6e20 6120 7374  ions return a st
-00004850: 7265 616d 2074 6865 6d73 656c 7665 732e  ream themselves.
-00004860: 2054 6869 7320 616c 6c6f 7773 206f 7065   This allows ope
-00004870: 7261 7469 6f6e 7320 746f 2062 6520 6368  rations to be ch
-00004880: 6169 6e65 6420 746f 2066 6f72 6d20 6120  ained to form a 
-00004890: 6c61 7267 6572 2070 6970 656c 696e 652e  larger pipeline.
-000048a0: 0a0a 215b 4461 7461 2073 7472 6561 6d20  ..![Data stream 
-000048b0: 7069 7065 6c69 6e65 5d28 646f 6375 6d65  pipeline](docume
-000048c0: 6e74 6174 696f 6e2f 696d 672f 6461 7461  ntation/img/data
-000048d0: 5f73 7472 6561 6d5f 7069 7065 6c69 6e65  _stream_pipeline
-000048e0: 2e70 6e67 290a 0a23 2323 2320 496e 7465  .png)..#### Inte
-000048f0: 726e 616c 2069 7465 7261 7469 6f6e 0a0a  rnal iteration..
-00004900: 496e 2063 6f6e 7472 6173 7420 746f 2063  In contrast to c
-00004910: 6f6c 6c65 6374 696f 6e73 2c20 7768 6963  ollections, whic
-00004920: 6820 6172 6520 6974 6572 6174 6564 2065  h are iterated e
-00004930: 7870 6c69 6369 746c 7920 2865 7874 6572  xplicitly (exter
-00004940: 6e61 6c20 6974 6572 6174 696f 6e29 2c20  nal iteration), 
-00004950: 7374 7265 616d 206f 7065 7261 7469 6f6e  stream operation
-00004960: 7320 646f 2074 6865 2069 7465 7261 7469  s do the iterati
-00004970: 6f6e 0a62 6568 696e 6420 7468 6520 7363  on.behind the sc
-00004980: 656e 6573 2066 6f72 2079 6f75 2e20 4e6f  enes for you. No
-00004990: 7465 2c20 6974 2064 6f65 736e 2774 206d  te, it doesn't m
-000049a0: 6561 6e20 796f 7520 6361 6e6e 6f74 2069  ean you cannot i
-000049b0: 7465 7261 7465 2074 6865 205f 4461 7461  terate the _Data
-000049c0: 206f 626a 6563 745f 2e0a 0a23 2323 2044   object_...### D
-000049d0: 6174 6120 6361 6368 696e 670a 0a54 6865  ata caching..The
-000049e0: 205f 4461 7461 206f 626a 6563 745f 2070   _Data object_ p
-000049f0: 726f 7669 6465 7320 7468 6520 6162 696c  rovides the abil
-00004a00: 6974 7920 746f 2075 7365 2074 6865 2063  ity to use the c
-00004a10: 6163 6865 2e20 5468 6520 6361 6368 6520  ache. The cache 
-00004a20: 776f 726b 7320 666f 7220 6561 6368 205f  works for each _
-00004a30: 4461 7461 206f 626a 6563 745f 2c20 7468  Data object_, th
-00004a40: 6174 2069 732c 2079 6f75 2063 686f 6f73  at is, you choos
-00004a50: 650a 7768 6963 6820 5f44 6174 6120 6f62  e.which _Data ob
-00004a60: 6a65 6374 5f20 796f 7520 7761 6e74 2074  ject_ you want t
-00004a70: 6f20 7361 7665 2e20 5468 6520 5f44 6174  o save. The _Dat
-00004a80: 6120 6f62 6a65 6374 5f20 6361 6368 6520  a object_ cache 
-00004a90: 6973 2073 6176 6564 2061 6674 6572 2074  is saved after t
-00004aa0: 6865 2066 6972 7374 2069 7465 7261 7469  he first iterati
-00004ab0: 6f6e 2c20 6275 7420 7468 6520 6974 6572  on, but the iter
-00004ac0: 6174 696f 6e0a 736f 7572 6365 206d 6179  ation.source may
-00004ad0: 2062 6520 6469 6666 6572 656e 742e 0a0a   be different...
-00004ae0: 4966 2079 6f75 2064 6f6e 2774 2075 7365  If you don't use
-00004af0: 2074 6865 2063 6163 6865 2c20 796f 7572   the cache, your
-00004b00: 2073 6f75 7263 6520 7769 6c6c 2062 6520   source will be 
-00004b10: 7468 6520 6461 7461 2073 6f75 7263 6520  the data source 
-00004b20: 796f 7520 6861 7665 2069 6e20 7468 6520  you have in the 
-00004b30: 5f44 6174 6120 4f62 6a65 6374 5f2e 2042  _Data Object_. B
-00004b40: 7574 2069 6620 796f 7520 7573 6520 7468  ut if you use th
-00004b50: 6520 6361 6368 652c 0a79 6f75 7220 736f  e cache,.your so
-00004b60: 7572 6365 2063 616e 2062 6520 7468 6520  urce can be the 
-00004b70: 6461 7461 2073 6f75 7263 652c 2074 6865  data source, the
-00004b80: 2070 6172 656e 7420 6361 6368 652c 206f   parent cache, o
-00004b90: 7220 6f77 6e20 6361 6368 653a 0a0a 2a20  r own cache:..* 
-00004ba0: 5468 6520 6461 7461 2073 6f75 7263 653a  The data source:
-00004bb0: 0a20 2049 6620 7468 6520 5f44 6174 6120  .  If the _Data 
-00004bc0: 4f62 6a65 6374 5f20 646f 6573 6e27 7420  Object_ doesn't 
-00004bd0: 6861 7665 2061 2070 6172 656e 7420 6361  have a parent ca
-00004be0: 6368 6520 616e 6420 6974 7320 6361 6368  che and its cach
-00004bf0: 652e 0a2a 2054 6865 2070 6172 656e 7420  e..* The parent 
-00004c00: 6361 6368 653a 0a20 2049 6620 7468 6520  cache:.  If the 
-00004c10: 5f44 6174 6120 4f62 6a65 6374 5f20 6861  _Data Object_ ha
-00004c20: 7320 6120 7061 7265 6e74 2063 6163 6865  s a parent cache
-00004c30: 2e20 4974 2064 6f65 736e 2774 206d 6174  . It doesn't mat
-00004c40: 7465 7220 7768 6174 2070 6f73 6974 696f  ter what positio
-00004c50: 6e20 7468 6520 7061 7265 6e74 2063 6163  n the parent cac
-00004c60: 6865 2068 6173 2069 6e20 696e 6865 7269  he has in inheri
-00004c70: 7461 6e63 652e 0a20 205f 4461 7461 204f  tance..  _Data O
-00004c80: 626a 6563 745f 2075 6e64 6572 7374 616e  bject_ understan
-00004c90: 6473 2077 686f 7365 2063 6163 6865 2069  ds whose cache i
-00004ca0: 7420 6973 2061 6e64 2065 7865 6375 7465  t is and execute
-00004cb0: 7320 7468 6520 7061 7274 206f 6620 7468  s the part of th
-00004cc0: 6520 776f 726b 666c 6f77 2074 6861 7420  e workflow that 
-00004cd0: 7761 7320 6e6f 7420 6578 6563 7574 6564  was not executed
-00004ce0: 2e0a 2a20 5468 6520 6f77 6e20 6361 6368  ..* The own cach
-00004cf0: 653a 0a20 2049 6620 6974 2069 7320 6e6f  e:.  If it is no
-00004d00: 7420 7468 6520 6669 7273 7420 6974 6572  t the first iter
-00004d10: 6174 696f 6e20 6f66 2074 6869 7320 4461  ation of this Da
-00004d20: 7461 206f 626a 6563 742e 0a0a 4e6f 7465  ta object...Note
-00004d30: 2074 6861 7420 7468 6520 6361 6368 6520   that the cache 
-00004d40: 7374 6174 6520 6f66 2074 6865 2044 6174  state of the Dat
-00004d50: 6120 6f62 6a65 6374 2069 7320 6e6f 7420  a object is not 
-00004d60: 696e 6865 7269 7465 642e 0a0a 2323 2323  inherited...####
-00004d70: 2046 6f72 6365 6420 6361 6368 696e 670a   Forced caching.
-00004d80: 596f 7520 6361 6e20 7465 6c6c 2044 5320  You can tell DS 
-00004d90: 746f 2063 6163 6865 2064 6174 6120 746f  to cache data to
-00004da0: 2073 7065 6369 6669 6320 6361 6368 6520   specific cache 
-00004db0: 6669 6c65 2c20 7768 6963 6820 776f 6e27  file, which won'
-00004dc0: 7420 6265 2064 656c 6574 6564 2061 6674  t be deleted aft
-00004dd0: 6572 2073 6372 6970 7420 656e 642e 0a59  er script end..Y
-00004de0: 6f75 2063 616e 2073 6565 2065 7861 6d70  ou can see examp
-00004df0: 6c65 2069 6e20 312e 3132 2073 6563 7469  le in 1.12 secti
-00004e00: 6f6e 206f 6620 5b67 6574 5f73 7461 7274  on of [get_start
-00004e10: 6564 5f65 7861 6d70 6c65 5d28 6578 616d  ed_example](exam
-00004e20: 706c 6573 2f67 6574 5f73 7461 7274 6564  ples/get_started
-00004e30: 5f65 7861 6d70 6c65 2e70 7929 2e0a 0a0a  _example.py)....
-00004e40: 2323 2320 4576 656e 7454 7265 6520 616e  ### EventTree an
-00004e50: 6420 636f 6c6c 6563 7469 6f6e 730a 0a23  d collections..#
-00004e60: 2323 2320 4576 656e 7454 7265 650a 0a60  ### EventTree..`
-00004e70: 4576 656e 7454 7265 6560 2069 7320 6120  EventTree` is a 
-00004e80: 7472 6565 2d62 6173 6564 2064 6174 6120  tree-based data 
-00004e90: 7374 7275 6374 7572 6520 6f66 2065 7665  structure of eve
-00004ea0: 6e74 732e 2049 7420 616c 6c6f 7773 2079  nts. It allows y
-00004eb0: 6f75 2067 6574 2063 6869 6c64 7265 6e20  ou get children 
-00004ec0: 616e 6420 7061 7265 6e74 7320 6f66 2065  and parents of e
-00004ed0: 7665 6e74 2c20 0a64 6973 706c 6179 2074  vent, .display t
-00004ee0: 7265 652c 2067 6574 2066 756c 6c20 7061  ree, get full pa
-00004ef0: 7468 2074 6f20 6576 656e 7420 6574 632e  th to event etc.
-00004f00: 0a0a 4465 7461 696c 733a 0a0a 2a20 6045  ..Details:..* `E
-00004f10: 7665 6e74 5472 6565 6020 636f 6e74 6169  ventTree` contai
-00004f20: 6e73 2061 6c6c 2065 7665 6e74 7320 696e  ns all events in
-00004f30: 206d 656d 6f72 792e 0a2a 2054 7265 6520   memory..* Tree 
-00004f40: 6861 7320 736f 6d65 2069 6d70 6f72 7461  has some importa
-00004f50: 6e74 2074 6572 6d73 3a0a 2020 2020 312e  nt terms:.    1.
-00004f60: 205f 416e 6365 7374 6f72 5f20 6973 2061   _Ancestor_ is a
-00004f70: 6e79 2072 656c 6174 6976 6520 6f66 2074  ny relative of t
-00004f80: 6865 2065 7665 6e74 2075 7020 7468 6520  he event up the 
-00004f90: 7472 6565 2028 6772 616e 6470 6172 656e  tree (grandparen
-00004fa0: 742c 2070 6172 656e 7420 6574 632e 292e  t, parent etc.).
-00004fb0: 0a20 2020 2032 2e20 5f50 6172 656e 745f  .    2. _Parent_
-00004fc0: 2069 7320 6f6e 6c79 2074 6865 2066 6972   is only the fir
-00004fd0: 7374 2072 656c 6174 6976 6520 6f66 2074  st relative of t
-00004fe0: 6865 2065 7665 6e74 2075 7020 7468 6520  he event up the 
-00004ff0: 7472 6565 2e0a 2020 2020 332e 205f 4368  tree..    3. _Ch
-00005000: 696c 645f 2069 7320 7468 6520 6669 7273  ild_ is the firs
-00005010: 7420 7265 6c61 7469 7665 206f 6620 7468  t relative of th
-00005020: 6520 6576 656e 7420 646f 776e 2074 6865  e event down the
-00005030: 2074 7265 652e 0a0a 5461 6b65 2061 206c   tree...Take a l
-00005040: 6f6f 6b20 6174 2074 6865 2066 6f6c 6c6f  ook at the follo
-00005050: 7769 6e67 2048 544d 4c20 7472 6565 2074  wing HTML tree t
-00005060: 6f20 756e 6465 7273 7461 6e64 2074 6865  o understand the
-00005070: 6d2e 0a0a 2020 2060 6060 0a20 2020 203c  m...   ```.    <
-00005080: 626f 6479 3e20 3c21 2d2d 2061 6e63 6573  body> <!-- ances
-00005090: 746f 7220 2867 7261 6e64 7061 7265 6e74  tor (grandparent
-000050a0: 292c 2062 7574 206e 6f74 2070 6172 656e  ), but not paren
-000050b0: 7420 2d2d 3e0a 2020 2020 2020 2020 3c64  t -->.        <d
-000050c0: 6976 3e20 3c21 2d2d 2070 6172 656e 7420  iv> <!-- parent 
-000050d0: 2620 616e 6365 7374 6f72 202d 2d3e 0a20  & ancestor -->. 
-000050e0: 2020 2020 2020 2020 2020 203c 703e 4865             <p>He
-000050f0: 6c6c 6f2c 2077 6f72 6c64 213c 2f70 3e20  llo, world!</p> 
-00005100: 3c21 2d2d 2063 6869 6c64 202d 2d3e 0a20  <!-- child -->. 
-00005110: 2020 2020 2020 2020 2020 203c 703e 476f             <p>Go
-00005120: 6f64 6279 6521 3c2f 703e 203c 212d 2d20  odbye!</p> <!-- 
-00005130: 7369 626c 696e 6720 2d2d 3e0a 2020 2020  sibling -->.    
-00005140: 2020 2020 3c2f 6469 763e 0a20 2020 203c      </div>.    <
-00005150: 2f62 6f64 793e 0a20 2020 6060 600a 0a23  /body>.   ```..#
-00005160: 2323 2320 436f 6c6c 6563 7469 6f6e 730a  ### Collections.
-00005170: 0a2a 2a45 7665 6e74 5472 6565 436f 6c6c  .**EventTreeColl
-00005180: 6563 7469 6f6e 2a2a 2069 7320 6120 636f  ection** is a co
-00005190: 6c6c 6563 7469 6f6e 206f 6620 4576 656e  llection of Even
-000051a0: 7454 7265 6573 2e20 5468 6520 636f 6c6c  tTrees. The coll
-000051b0: 6563 7469 6f6e 2062 7569 6c64 7320 6120  ection builds a 
-000051c0: 6665 7720 5f45 7665 6e74 5472 6565 5f20  few _EventTree_ 
-000051d0: 6279 2070 6173 7365 6420 5f44 6174 610a  by passed _Data.
-000051e0: 6f62 6a65 6374 5f2e 2041 6c74 686f 7567  object_. Althoug
-000051f0: 6820 796f 7520 6361 6e20 6368 616e 6765  h you can change
-00005200: 2074 6865 2074 7265 6520 6469 7265 6374   the tree direct
-00005210: 6c79 2c20 6974 2773 2062 6574 7465 7220  ly, it's better 
-00005220: 746f 2064 6f20 6974 2074 6872 6f75 6768  to do it through
-00005230: 2063 6f6c 6c65 6374 696f 6e73 2062 6563   collections bec
-00005240: 6175 7365 2074 6865 7920 6172 6520 6177  ause they are aw
-00005250: 6172 6520 6f66 0a60 6465 7461 6368 6564  are of.`detached
-00005260: 5f65 7665 6e74 7360 2061 6e64 2063 616e  _events` and can
-00005270: 2073 6f6c 7665 2073 6f6d 6520 6576 656e   solve some even
-00005280: 7473 2064 6570 656e 6465 6e63 6965 732e  ts dependencies.
-00005290: 2054 6865 2063 6f6c 6c65 6374 696f 6e20   The collection 
-000052a0: 6861 7320 7369 6d69 6c61 7220 6665 6174  has similar feat
-000052b0: 7572 6573 206c 696b 6520 6120 7369 6e67  ures like a sing
-000052c0: 6c65 205f 4576 656e 7454 7265 655f 0a62  le _EventTree_.b
-000052d0: 7574 2061 7070 6c79 696e 6720 7468 656d  ut applying them
-000052e0: 2066 6f72 2061 6c6c 205f 4576 656e 7454   for all _EventT
-000052f0: 7265 6573 5f2e 0a0a 2a2a 5061 7265 6e74  rees_...**Parent
-00005300: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
-00005310: 696f 6e2a 2a20 6973 2061 2063 6f6c 6c65  ion** is a colle
-00005320: 6374 696f 6e20 7369 6d69 6c61 7220 746f  ction similar to
-00005330: 205f 4576 656e 7454 7265 6543 6f6c 6c65   _EventTreeColle
-00005340: 6374 696f 6e5f 2062 7574 2063 6f6e 7461  ction_ but conta
-00005350: 696e 696e 6720 6f6e 6c79 2070 6172 656e  ining only paren
-00005360: 7420 6576 656e 7473 2074 6861 740a 6172  t events that.ar
-00005370: 6520 7265 6665 7265 6e63 6564 2069 6e20  e referenced in 
-00005380: 7468 6520 6461 7461 2073 7472 6561 6d2e  the data stream.
-00005390: 2054 6865 2063 6f6c 6c65 6374 696f 6e20   The collection 
-000053a0: 6861 7320 6665 6174 7572 6573 2073 696d  has features sim
-000053b0: 696c 6172 2074 6f20 5f45 7665 6e74 5472  ilar to _EventTr
-000053c0: 6565 436f 6c6c 6563 7469 6f6e 5f2e 0a0a  eeCollection_...
-000053d0: 4465 7461 696c 733a 0a0a 2a20 546f 2075  Details:..* To u
-000053e0: 7365 2045 5420 636f 6c6c 6563 7469 6f6e  se ET collection
-000053f0: 7320 796f 7520 6e65 6564 2074 6f20 696e  s you need to in
-00005400: 6974 6961 6c69 7a65 2074 6865 6d20 6279  itialize them by
-00005410: 205f 4554 4344 7269 7665 725f 2e20 4461   _ETCDriver_. Da
-00005420: 7461 2073 6f75 7263 6573 2075 7375 616c  ta sources usual
-00005430: 6c79 2070 726f 7669 6465 2074 6865 6d2e  ly provide them.
-00005440: 0a20 2059 6f75 2063 616e 2063 7265 6174  .  You can creat
-00005450: 6520 6974 2062 7920 796f 7572 7365 6c66  e it by yourself
-00005460: 2064 6570 656e 6469 6e67 206f 6e20 796f   depending on yo
-00005470: 7572 2064 6174 6120 7374 7275 6374 7572  ur data structur
-00005480: 652e 2020 0a2a 2054 6865 2063 6f6c 6c65  e.  .* The colle
-00005490: 6374 696f 6e20 6861 7320 6120 6665 6174  ction has a feat
-000054a0: 7572 6520 746f 2072 6563 6f76 6572 2065  ure to recover e
-000054b0: 7665 6e74 732e 2041 6c6c 2065 7665 6e74  vents. All event
-000054c0: 7320 7468 6174 2061 7265 206e 6f74 2069  s that are not i
-000054d0: 6e20 7468 6520 7265 6365 6976 6564 2064  n the received d
-000054e0: 6174 6120 7374 7265 616d 2c20 6275 7420  ata stream, but 
-000054f0: 7768 6963 6820 6172 650a 2020 7265 6665  which are.  refe
-00005500: 7265 6e63 6564 2077 696c 6c20 6265 206c  renced will be l
-00005510: 6f61 6465 6420 6672 6f6d 2074 6865 2064  oaded from the d
-00005520: 6174 6120 736f 7572 6365 2e0a 2a20 596f  ata source..* Yo
-00005530: 7520 6361 6e20 7461 6b65 2060 6465 7461  u can take `deta
-00005540: 6368 6564 5f65 7665 6e74 7360 2074 6f20  ched_events` to 
-00005550: 7365 6520 7768 6963 6820 6576 656e 7473  see which events
-00005560: 2061 7265 206d 6973 7369 6e67 2e0a 2a20   are missing..* 
-00005570: 4966 2079 6f75 2077 616e 742c 2079 6f75  If you want, you
-00005580: 2063 616e 2062 7569 6c64 2070 6172 656e   can build paren
-00005590: 746c 6573 7320 7472 6565 7320 7768 6572  tless trees wher
-000055a0: 6520 7468 6520 6d69 7373 696e 6720 6576  e the missing ev
-000055b0: 656e 7473 2061 7265 2073 7475 6262 6564  ents are stubbed
-000055c0: 2069 6e73 7465 6164 2e20 4a75 7374 0a20   instead. Just. 
-000055d0: 2075 7365 2060 6765 745f 7061 7265 6e74   use `get_parent
-000055e0: 6c65 7373 5f74 7265 6573 2829 602e 0a0a  less_trees()`...
-000055f0: 5265 7175 6972 656d 656e 7473 3a0a 0a31  Requirements:..1
-00005600: 2e20 4576 656e 7473 2070 726f 7669 6465  . Events provide
-00005610: 6420 746f 2045 5443 2068 6176 6520 746f  d to ETC have to
-00005620: 2068 6176 6520 6065 7665 6e74 5f6e 616d   have `event_nam
-00005630: 6560 2c20 6065 7665 6e74 5f69 6460 2c20  e`, `event_id`, 
-00005640: 6070 6172 656e 745f 6576 656e 745f 6964  `parent_event_id
-00005650: 6020 6669 656c 6473 2e20 5468 6579 200a  ` fields. They .
-00005660: 6361 6e20 6861 7665 2061 6e6f 7468 6572  can have another
-00005670: 206e 616d 6573 2028 6974 2072 6573 6f6c   names (it resol
-00005680: 7665 7320 696e 2074 6865 2064 7269 7665  ves in the drive
-00005690: 7229 2e0a 0a23 2323 2320 4869 6e74 730a  r)...#### Hints.
-000056a0: 0a2a 2052 656d 6f76 6520 616c 6c20 756e  .* Remove all un
-000056b0: 6e65 6365 7373 6172 7920 6669 656c 6473  necessary fields
-000056c0: 2066 726f 6d20 6576 656e 7473 2062 6566   from events bef
-000056d0: 6f72 6520 7061 7373 696e 6720 746f 2061  ore passing to a
-000056e0: 205f 636f 6c6c 6563 7469 6f6e 5f20 746f   _collection_ to
-000056f0: 2072 6564 7563 6520 6d65 6d6f 7279 2075   reduce memory u
-00005700: 7361 6765 2e0a 2a20 5573 6520 6073 686f  sage..* Use `sho
-00005710: 7728 2960 206d 6574 686f 6420 746f 2070  w()` method to p
-00005720: 7269 6e74 2074 6865 2074 7265 6520 696e  rint the tree in
-00005730: 2074 7265 652d 6c69 6b65 2076 6965 772e   tree-like view.
-00005740: 0a2a 204e 6f74 6520 7468 6174 2074 6865  .* Note that the
-00005750: 2060 6765 745f 7860 206d 6574 686f 6473   `get_x` methods
-00005760: 2077 696c 6c20 7261 6973 6520 616e 2065   will raise an e
-00005770: 7863 6570 7469 6f6e 2069 6620 796f 7520  xception if you 
-00005780: 7061 7373 2061 6e20 756e 6b6e 6f77 6e20  pass an unknown 
-00005790: 6576 656e 7420 6964 2c20 756e 6c69 6b65  event id, unlike
-000057a0: 2074 6865 2060 6669 6e64 5f78 6020 6d65   the `find_x` me
-000057b0: 7468 6f64 7320 280a 2020 7468 6579 2072  thods (.  they r
-000057c0: 6574 7572 6e20 4e6f 6e65 292e 0a2a 2049  eturn None)..* I
-000057d0: 6620 796f 7520 7761 6e74 2074 6f20 6b6e  f you want to kn
-000057e0: 6f77 2074 6861 7420 7370 6563 6966 6965  ow that specifie
-000057f0: 6420 6576 656e 7420 6578 6973 7473 2c20  d event exists, 
-00005800: 7573 6520 7468 6520 7079 7468 6f6e 2060  use the python `
-00005810: 696e 6020 6b65 7977 6f72 6420 2865 2e67  in` keyword (e.g
-00005820: 2e20 6027 6576 656e 742d 6964 2720 696e  . `'event-id' in
-00005830: 2065 7665 6e74 735f 7472 6565 6029 2e0a   events_tree`)..
-00005840: 2a20 5573 6520 7468 6520 7079 7468 6f6e  * Use the python
-00005850: 2060 6c65 6e60 206b 6579 776f 7264 2074   `len` keyword t
-00005860: 6f20 6765 7420 6576 656e 7473 206e 756d  o get events num
-00005870: 6265 7220 696e 2074 6865 2074 7265 652e  ber in the tree.
-00005880: 0a0a 2323 2320 4669 656c 6473 5265 736f  ..### FieldsReso
-00005890: 6c76 6572 0a54 6865 2069 6465 6120 6f66  lver.The idea of
-000058a0: 2075 7369 6e67 2072 6573 6f6c 7665 7273   using resolvers
-000058b0: 3a20 200a 4974 2073 6f6c 7665 7320 7468  :  .It solves th
-000058c0: 6520 7072 6f62 6c65 6d20 6f66 2068 6176  e problem of hav
-000058d0: 696e 6720 6120 6665 7720 4461 7461 536f  ing a few DataSo
-000058e0: 7572 6365 7320 7769 7468 2074 6865 2073  urces with the s
-000058f0: 616d 6520 6461 7461 2c20 0a62 7574 2077  ame data, .but w
-00005900: 6974 6820 6469 6666 6572 656e 7420 7761  ith different wa
-00005910: 7973 2074 6f20 6765 7420 6974 2e0a 0a54  ys to get it...T
-00005920: 6865 7365 2063 6c61 7373 6573 2070 726f  hese classes pro
-00005930: 7669 6465 2079 6f75 2067 6574 7465 7220  vide you getter 
-00005940: 6d65 7468 6f64 732e 200a 5573 696e 6720  methods. .Using 
-00005950: 7468 6573 6520 636c 6173 7365 7320 616c  these classes al
-00005960: 6c6f 7773 2079 6f75 2074 6f20 6672 6565  lows you to free
-00005970: 6c79 2073 7769 7463 6820 6265 7477 6565  ly switch betwee
-00005980: 6e20 6469 6666 6572 656e 7420 6461 7461  n different data
-00005990: 200a 666f 726d 6174 7320 616e 6420 646f   .formats and do
-000059a0: 6e27 7420 6368 616e 6765 2079 6f75 7220  n't change your 
-000059b0: 636f 6465 2e20 0a0a 5265 736f 6c76 6572  code. ..Resolver
-000059c0: 7320 736f 6c76 6520 7468 6520 7072 6f62  s solve the prob
-000059d0: 6c65 6d20 6f66 2064 6174 612d 666f 726d  lem of data-form
-000059e0: 6174 206d 6967 7261 7469 6f6e 2e20 200a  at migration.  .
-000059f0: 2d20 6669 656c 6473 2070 6c61 6365 2063  - fields place c
-00005a00: 616e 2062 6520 6368 616e 6765 640a 2d20  an be changed.- 
-00005a10: 6669 656c 6473 206e 616d 6573 2063 616e  fields names can
-00005a20: 2062 6520 6368 616e 6765 640a 0a52 6573   be changed..Res
-00005a30: 6f6c 7665 7273 2063 616e 2077 6f72 6b20  olvers can work 
-00005a40: 6f6e 6c79 2077 6974 6820 6f6e 6520 6576  only with one ev
-00005a50: 656e 742f 6d65 7373 6167 652e 200a 4974  ent/message. .It
-00005a60: 206d 6561 6e73 2c20 6966 2079 6f75 7220   means, if your 
-00005a70: 6d65 7373 6167 6520 6861 7320 7375 622d  message has sub-
-00005a80: 6d65 7373 6167 6573 2069 7420 776f 6e27  messages it won'
-00005a90: 7420 776f 726b 2c20 6265 6361 7573 6520  t work, because 
-00005aa0: 7265 736f 6c76 6572 2077 696c 6c20 6e6f  resolver will no
-00005ab0: 7420 0a6b 6e6f 7720 7769 7468 2077 6869  t .know with whi
-00005ac0: 6368 2073 7562 2d6d 6573 7361 6765 2073  ch sub-message s
-00005ad0: 686f 756c 6420 6974 2077 6f72 6b2e 200a  hould it work. .
-00005ae0: 0a49 6d70 6c65 6d65 6e74 6174 696f 6e20  .Implementation 
-00005af0: 6164 7669 6365 3a0a 312e 2072 6169 7365  advice:.1. raise
-00005b00: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
-00005b10: 7272 6f72 202d 2d20 6966 2079 6f75 7220  rror -- if your 
-00005b20: 496d 706c 656d 656e 7461 7469 6f6e 2064  Implementation d
-00005b30: 6f65 736e 2774 2073 7570 706f 7274 2074  oesn't support t
-00005b40: 6869 7320 6765 7474 6572 2e0a 0a50 6572  his getter...Per
-00005b50: 666f 726d 616e 6365 2069 6d70 6163 743a  formance impact:
-00005b60: 0a2d 2049 7420 6120 6269 7420 736c 6f77  .- It a bit slow
-00005b70: 6572 2074 6861 6e20 7573 696e 6720 6e61  er than using na
-00005b80: 6b65 6420 6669 656c 6420 6163 6365 7373  ked field access
-00005b90: 2060 6469 6374 5b27 6b65 7927 5d60 2e20   `dict['key']`. 
-00005ba0: 0a0a 2323 2032 2e34 2e20 4c69 6e6b 730a  ..## 2.4. Links.
-00005bb0: 0a2d 205b 5265 706f 7274 2044 6174 6120  .- [Report Data 
-00005bc0: 5072 6f76 6964 6572 5d28 6874 7470 733a  Provider](https:
-00005bd0: 2f2f 6769 7468 7562 2e63 6f6d 2f74 6832  //github.com/th2
-00005be0: 2d6e 6574 2f74 6832 2d72 7074 2d64 6174  -net/th2-rpt-dat
-00005bf0: 612d 7072 6f76 6964 6572 290a 2d20 5b54  a-provider).- [T
-00005c00: 6832 2044 6174 6120 5365 7276 6963 6573  h2 Data Services
-00005c10: 2055 7469 6c73 5d28 6874 7470 733a 2f2f   Utils](https://
-00005c20: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
-00005c30: 6574 2f74 6832 2d64 6174 612d 7365 7276  et/th2-data-serv
-00005c40: 6963 6573 2d75 7469 6c73 290a 0a23 2033  ices-utils)..# 3
-00005c50: 2e20 4265 7374 2070 7261 6374 6963 6573  . Best practices
-00005c60: 0a44 6570 656e 6469 6e67 206f 6e20 686f  .Depending on ho
-00005c70: 7720 796f 7520 776f 726b 2077 6974 6820  w you work with 
-00005c80: 6044 6174 6120 6f62 6a65 6374 602c 2069  `Data object`, i
-00005c90: 7420 6361 6e20 6265 2073 6c6f 7720 6f66  t can be slow of
-00005ca0: 2066 6173 742e 2020 0a41 7320 7769 7468   fast.  .As with
-00005cb0: 2061 2072 656c 6174 696f 6e61 6c20 6461   a relational da
-00005cc0: 7461 6261 7365 2c20 796f 7520 6361 6e20  tabase, you can 
-00005cd0: 7772 6974 6520 6120 7175 6572 7920 7468  write a query th
-00005ce0: 6174 2077 696c 6c20 7265 7475 726e 2064  at will return d
-00005cf0: 6174 6120 736c 6f77 6c79 206f 7220 7175  ata slowly or qu
-00005d00: 6963 6b6c 792c 200a 7468 6520 7361 6d65  ickly, .the same
-00005d10: 2077 6865 6e20 776f 726b 696e 6720 7769   when working wi
-00005d20: 7468 2061 2060 4461 7461 206f 626a 6563  th a `Data objec
-00005d30: 7460 2e0a 0a46 6f6c 6c6f 7720 7468 6520  t`...Follow the 
-00005d40: 7275 6c65 7320 746f 206d 616b 6520 796f  rules to make yo
-00005d50: 7572 2077 6f72 6b20 7769 7468 2044 6174  ur work with Dat
-00005d60: 6120 6f62 6a65 6374 2066 6173 743a 0a31  a object fast:.1
-00005d70: 2e20 5573 6520 6044 6174 612e 7573 655f  . Use `Data.use_
-00005d80: 6361 6368 6528 2960 2069 6620 796f 7520  cache()` if you 
-00005d90: 6974 6572 6174 6520 6461 7461 206d 6f72  iterate data mor
-00005da0: 6520 7468 616e 206f 6e65 2074 696d 652e  e than one time.
-00005db0: 0a32 2e20 5472 7920 746f 2064 6f6e 2774  .2. Try to don't
-00005dc0: 2069 7465 7261 7465 206f 6e65 2060 4461   iterate one `Da
-00005dd0: 7461 206f 626a 6563 7460 2069 6e73 6964  ta object` insid
-00005de0: 6520 7468 6520 6f74 6865 7220 6f6e 652e  e the other one.
-00005df0: 2020 0a20 2020 4966 2079 6f75 2073 686f    .   If you sho
-00005e00: 756c 6420 746f 2064 6f20 6974 2c20 7573  uld to do it, us
-00005e10: 6520 7368 6f72 7420 6044 6174 6120 6f62  e short `Data ob
-00005e20: 6a65 6374 6020 6669 7273 7420 616e 6420  ject` first and 
-00005e30: 6c6f 6e67 2060 4461 7461 206f 626a 6563  long `Data objec
-00005e40: 7460 2069 6e73 6964 6520 7468 6520 6c6f  t` inside the lo
-00005e50: 6f70 2e20 200a 2020 2049 7427 6c6c 2061  op.  .   It'll a
-00005e60: 6c6c 6f77 2079 6f75 206f 7065 6e20 7468  llow you open th
-00005e70: 6520 6361 6368 6520 6669 6c65 206f 7220  e cache file or 
-00005e80: 6372 6561 7465 2061 2072 6571 7565 7374  create a request
-00005e90: 2074 6f20 6044 6174 6120 736f 7572 6365   to `Data source
-00005ea0: 6020 6c65 7373 206e 756d 6265 7220 6f66  ` less number of
-00005eb0: 2074 696d 6573 2e0a 0a23 2034 2e20 4f66   times...# 4. Of
-00005ec0: 6669 6369 616c 2044 6174 6153 6f75 7263  ficial DataSourc
-00005ed0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
-00005ee0: 730a 0a2d 205b 4c69 6768 7477 6569 6768  s..- [Lightweigh
-00005ef0: 7420 4461 7461 2050 726f 7669 6465 7220  t Data Provider 
-00005f00: 4461 7461 2053 6f75 7263 655d 2868 7474  Data Source](htt
-00005f10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00005f20: 7468 322d 6e65 742f 7468 322d 6473 2d73  th2-net/th2-ds-s
-00005f30: 6f75 7263 652d 6c77 6470 290a 0a0a 2320  ource-lwdp)...# 
-00005f40: 352e 2041 5049 0a0a 4966 2079 6f75 2061  5. API..If you a
-00005f50: 7265 206c 6f6f 6b69 6e67 2066 6f72 2063  re looking for c
-00005f60: 6c61 7373 6573 2064 6573 6372 6970 7469  lasses descripti
-00005f70: 6f6e 2073 6565 2074 6865 205b 4150 4920  on see the [API 
-00005f80: 446f 6375 6d65 6e74 6174 696f 6e5d 2864  Documentation](d
-00005f90: 6f63 756d 656e 7461 7469 6f6e 2f61 7069  ocumentation/api
-00005fa0: 2f69 6e64 6578 2e6d 6429 2e0a 0a23 2036  /index.md)...# 6
-00005fb0: 2e20 4578 616d 706c 6573 0a0a 2d20 5b67  . Examples..- [g
-00005fc0: 6574 5f73 7461 7274 6564 5f65 7861 6d70  et_started_examp
-00005fd0: 6c65 2e70 795d 2865 7861 6d70 6c65 732f  le.py](examples/
-00005fe0: 6765 745f 7374 6172 7465 645f 6578 616d  get_started_exam
-00005ff0: 706c 652e 7079 290a                      ple.py).
+00001800: 3133 3537 3035 3536 3335 3232 3030 303a  135705563522000:
+00001810: 3961 6462 6233 6530 2d35 6638 622d 3463  9adbb3e0-5f8b-4c
+00001820: 3238 2d61 3261 632d 3733 3631 6538 6661  28-a2ac-7361e8fa
+00001830: 3730 3463 3e64 656d 6f5f 626f 6f6b 5f31  704c>demo_book_1
+00001840: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
+00001850: 3130 3531 3335 3730 3535 3633 3735 3730  1051357055637570
+00001860: 3030 3a64 3631 6539 3330 612d 3864 3030  00:d61e930a-8d00
+00001870: 2d31 3165 642d 6161 3161 2d64 3334 6136  -11ed-aa1a-d34a6
+00001880: 3135 3531 3532 645f 3322 2c0a 2020 2020  155152d_3",.    
+00001890: 2020 2020 2020 2020 2262 6174 6368 4964          "batchId
+000018a0: 223a 2022 6465 6d6f 5f62 6f6f 6b5f 313a  ": "demo_book_1:
+000018b0: 7468 322d 7363 6f70 653a 3230 3233 3031  th2-scope:202301
+000018c0: 3035 3133 3537 3035 3536 3335 3232 3030  0513570556352200
+000018d0: 303a 3961 6462 6233 6530 2d35 6638 622d  0:9adbb3e0-5f8b-
+000018e0: 3463 3238 2d61 3261 632d 3733 3631 6538  4c28-a2ac-7361e8
+000018f0: 6661 3730 3463 222c 0a20 2020 2020 2020  fa704c",.       
+00001900: 2020 2020 2022 6973 4261 7463 6865 6422       "isBatched"
+00001910: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
+00001920: 2020 2020 2265 7665 6e74 4e61 6d65 223a      "eventName":
+00001930: 2022 506c 6169 6e20 6576 656e 7420 3222   "Plain event 2"
+00001940: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
+00001950: 7665 6e74 5479 7065 223a 2022 6473 2d6c  ventType": "ds-l
+00001960: 6962 2d74 6573 742d 6576 656e 7422 2c0a  ib-test-event",.
+00001970: 2020 2020 2020 2020 2020 2020 2265 6e64              "end
+00001980: 5469 6d65 7374 616d 7022 3a20 7b22 6570  Timestamp": {"ep
+00001990: 6f63 6853 6563 6f6e 6422 3a20 3136 3732  ochSecond": 1672
+000019a0: 3932 3730 3235 2c20 226e 616e 6f22 3a20  927025, "nano": 
+000019b0: 3536 3337 3931 3030 307d 2c0a 2020 2020  563791000},.    
+000019c0: 2020 2020 2020 2020 2273 7461 7274 5469          "startTi
+000019d0: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
+000019e0: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
+000019f0: 3730 3235 2c20 226e 616e 6f22 3a20 3536  7025, "nano": 56
+00001a00: 3337 3537 3030 307d 2c0a 2020 2020 2020  3757000},.      
+00001a10: 2020 2020 2020 2270 6172 656e 7445 7665        "parentEve
+00001a20: 6e74 4964 223a 2022 6465 6d6f 5f62 6f6f  ntId": "demo_boo
+00001a30: 6b5f 313a 7468 322d 7363 6f70 653a 3230  k_1:th2-scope:20
+00001a40: 3233 3031 3035 3133 3537 3035 3536 3038  2301051357055608
+00001a50: 3733 3030 303a 6436 3165 3933 3061 2d38  73000:d61e930a-8
+00001a60: 6430 302d 3131 6564 2d61 6131 612d 6433  d00-11ed-aa1a-d3
+00001a70: 3461 3631 3535 3135 3264 5f31 222c 0a20  4a6155152d_1",. 
+00001a80: 2020 2020 2020 2020 2020 2022 7375 6363             "succ
+00001a90: 6573 7366 756c 223a 2054 7275 652c 0a20  essful": True,. 
+00001aa0: 2020 2020 2020 2020 2020 2022 626f 6f6b             "book
+00001ab0: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
+00001ac0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
+00001ad0: 2273 636f 7065 223a 2022 7468 322d 7363  "scope": "th2-sc
+00001ae0: 6f70 6522 2c0a 2020 2020 2020 2020 2020  ope",.          
+00001af0: 2020 2261 7474 6163 6865 644d 6573 7361    "attachedMessa
+00001b00: 6765 4964 7322 3a20 5b5d 2c0a 2020 2020  geIds": [],.    
+00001b10: 2020 2020 2020 2020 2262 6f64 7922 3a20          "body": 
+00001b20: 7b22 7479 7065 223a 2022 6d65 7373 6167  {"type": "messag
+00001b30: 6522 2c20 2264 6174 6122 3a20 2264 732d  e", "data": "ds-
+00001b40: 6c69 6220 7465 7374 2062 6f64 7922 7d2c  lib test body"},
+00001b50: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00001b60: 5d0a 290a 0a23 205b 315d 2057 6f72 6b69  ].)..# [1] Worki
+00001b70: 6e67 2077 6974 6820 6120 4461 7461 206f  ng with a Data o
+00001b80: 626a 6563 742e 0a23 205b 312e 315d 2046  bject..# [1.1] F
+00001b90: 696c 7465 722e 0a66 696c 7465 7265 645f  ilter..filtered_
+00001ba0: 6576 656e 7473 3a20 4461 7461 203d 2065  events: Data = e
+00001bb0: 7665 6e74 732e 6669 6c74 6572 286c 616d  vents.filter(lam
+00001bc0: 6264 6120 653a 2065 5b22 626f 6479 225d  bda e: e["body"]
+00001bd0: 2021 3d20 5b5d 2920 2023 2046 696c 7465   != [])  # Filte
+00001be0: 7220 6576 656e 7473 2077 6974 6820 656d  r events with em
+00001bf0: 7074 7920 626f 6479 2e0a 0a0a 2320 5b31  pty body....# [1
+00001c00: 2e32 5d20 4d61 702e 0a64 6566 2074 7261  .2] Map..def tra
+00001c10: 6e73 666f 726d 5f66 756e 6374 696f 6e28  nsform_function(
+00001c20: 7265 636f 7264 293a 0a20 2020 2072 6574  record):.    ret
+00001c30: 7572 6e20 7b22 6576 656e 744e 616d 6522  urn {"eventName"
+00001c40: 3a20 7265 636f 7264 5b22 6576 656e 744e  : record["eventN
+00001c50: 616d 6522 5d2c 2022 7375 6363 6573 7366  ame"], "successf
+00001c60: 756c 223a 2072 6563 6f72 645b 2273 7563  ul": record["suc
+00001c70: 6365 7373 6675 6c22 5d7d 0a0a 0a66 696c  cessful"]}...fil
+00001c80: 7465 7265 645f 616e 645f 6d61 7070 6564  tered_and_mapped
+00001c90: 5f65 7665 6e74 7320 3d20 6669 6c74 6572  _events = filter
+00001ca0: 6564 5f65 7665 6e74 732e 6d61 7028 7472  ed_events.map(tr
+00001cb0: 616e 7366 6f72 6d5f 6675 6e63 7469 6f6e  ansform_function
+00001cc0: 290a 0a23 205b 312e 335d 2044 6174 6120  )..# [1.3] Data 
+00001cd0: 7069 7065 6c69 6e65 2e0a 2320 2020 2020  pipeline..#     
+00001ce0: 2020 496e 7374 6561 6420 6f66 2064 6f69    Instead of doi
+00001cf0: 6e67 2064 6174 6120 7472 616e 7366 6f72  ng data transfor
+00001d00: 6d61 7469 6f6e 7320 7374 6570 2062 7920  mations step by 
+00001d10: 7374 6570 2079 6f75 2063 616e 2064 6f20  step you can do 
+00001d20: 6974 2069 6e20 6f6e 6520 6c69 6e65 2e0a  it in one line..
+00001d30: 6669 6c74 6572 6564 5f61 6e64 5f6d 6170  filtered_and_map
+00001d40: 7065 645f 6576 656e 7473 5f62 795f 7069  ped_events_by_pi
+00001d50: 7065 6c69 6e65 203d 2065 7665 6e74 732e  peline = events.
+00001d60: 6669 6c74 6572 286c 616d 6264 6120 653a  filter(lambda e:
+00001d70: 2065 5b22 626f 6479 225d 2021 3d20 5b5d   e["body"] != []
+00001d80: 292e 6d61 7028 7472 616e 7366 6f72 6d5f  ).map(transform_
+00001d90: 6675 6e63 7469 6f6e 290a 2320 436f 6e74  function).# Cont
+00001da0: 656e 7420 6f66 2074 6865 7365 2074 776f  ent of these two
+00001db0: 2044 6174 6120 6f62 6a65 6374 7320 7368   Data objects sh
+00001dc0: 6f75 6c64 2062 6520 6571 7561 6c2e 0a61  ould be equal..a
+00001dd0: 7373 6572 7420 6c69 7374 2866 696c 7465  ssert list(filte
+00001de0: 7265 645f 616e 645f 6d61 7070 6564 5f65  red_and_mapped_e
+00001df0: 7665 6e74 7329 203d 3d20 6c69 7374 2866  vents) == list(f
+00001e00: 696c 7465 7265 645f 616e 645f 6d61 7070  iltered_and_mapp
+00001e10: 6564 5f65 7665 6e74 735f 6279 5f70 6970  ed_events_by_pip
+00001e20: 656c 696e 6529 0a0a 2320 5b31 2e34 5d20  eline)..# [1.4] 
+00001e30: 5369 6674 2e20 536b 6970 2074 6865 2066  Sift. Skip the f
+00001e40: 6972 7374 2066 6577 2069 7465 6d73 206f  irst few items o
+00001e50: 7220 6c69 6d69 7420 7468 656d 2e0a 6461  r limit them..da
+00001e60: 7461 203d 2044 6174 6128 5b31 2c20 322c  ta = Data([1, 2,
+00001e70: 2033 2c20 342c 2035 2c20 362c 2037 2c20   3, 4, 5, 6, 7, 
+00001e80: 382c 2039 2c20 3130 2c20 3131 2c20 3132  8, 9, 10, 11, 12
+00001e90: 2c20 3133 2c20 3134 2c20 3135 5d29 0a69  , 13, 14, 15]).i
+00001ea0: 7465 6d73 5f66 726f 6d5f 3131 5f74 6f5f  tems_from_11_to_
+00001eb0: 656e 643a 2047 656e 6572 6174 6f72 203d  end: Generator =
+00001ec0: 2064 6174 612e 7369 6674 2873 6b69 703d   data.sift(skip=
+00001ed0: 3130 290a 6f6e 6c79 5f66 6972 7374 5f31  10).only_first_1
+00001ee0: 305f 6974 656d 733a 2047 656e 6572 6174  0_items: Generat
+00001ef0: 6f72 203d 2064 6174 612e 7369 6674 286c  or = data.sift(l
+00001f00: 696d 6974 3d31 3029 0a0a 2320 5b31 2e35  imit=10)..# [1.5
+00001f10: 5d20 4368 616e 6769 6e67 2063 6163 6865  ] Changing cache
+00001f20: 2073 7461 7475 732e 0a65 7665 6e74 732e   status..events.
+00001f30: 7573 655f 6361 6368 6528 5472 7565 290a  use_cache(True).
+00001f40: 2320 6f72 206a 7573 740a 6576 656e 7473  # or just.events
+00001f50: 2e75 7365 5f63 6163 6865 2829 2020 2320  .use_cache()  # 
+00001f60: 4966 2079 6f75 2077 616e 7420 746f 2061  If you want to a
+00001f70: 6374 6976 6174 6520 6361 6368 652e 0a23  ctivate cache..#
+00001f80: 205b 312e 365d 2057 616c 6b20 7468 726f   [1.6] Walk thro
+00001f90: 7567 6820 6461 7461 2e0a 666f 7220 6576  ugh data..for ev
+00001fa0: 656e 7420 696e 2065 7665 6e74 733a 0a20  ent in events:. 
+00001fb0: 2020 2023 2044 6f20 736f 6d65 7468 696e     # Do somethin
+00001fc0: 6720 7769 7468 2065 7665 6e74 2028 6576  g with event (ev
+00001fd0: 656e 7420 6973 2061 2064 6963 7429 2e0a  ent is a dict)..
+00001fe0: 2020 2020 7072 696e 7428 6576 656e 7429      print(event)
+00001ff0: 0a23 2041 6674 6572 2066 6972 7374 2069  .# After first i
+00002000: 7465 7261 7469 6f6e 2074 6865 2065 7665  teration the eve
+00002010: 6e74 7320 6861 7320 6120 6361 6368 6520  nts has a cache 
+00002020: 6669 6c65 2e0a 2320 4e6f 7720 7468 6579  file..# Now they
+00002030: 2077 696c 6c20 6265 2075 7365 6420 696e   will be used in
+00002040: 2074 6865 2063 6163 6865 2069 6e20 7468   the cache in th
+00002050: 6520 6e65 7874 2069 7465 7261 7469 6f6e  e next iteration
+00002060: 2e0a 0a23 205b 312e 375d 2047 6574 206e  ...# [1.7] Get n
+00002070: 756d 6265 7220 6f66 2074 6865 2065 6c65  umber of the ele
+00002080: 6d65 6e74 7320 696e 2074 6865 2044 6174  ments in the Dat
+00002090: 6120 6f62 6a65 6374 2e0a 6e75 6d62 6572  a object..number
+000020a0: 5f6f 665f 6576 656e 7473 203d 2065 7665  _of_events = eve
+000020b0: 6e74 732e 6c65 6e0a 0a23 205b 312e 385d  nts.len..# [1.8]
+000020c0: 2043 6865 636b 2074 6861 7420 4461 7461   Check that Data
+000020d0: 206f 626a 6563 7420 6973 6e27 7420 656d   object isn't em
+000020e0: 7074 792e 0a23 2054 6865 2064 6174 6120  pty..# The data 
+000020f0: 736f 7572 6365 2073 686f 756c 6420 6265  source should be
+00002100: 206e 6f74 2065 6d70 7479 2e0a 6173 7365   not empty..asse
+00002110: 7274 2065 7665 6e74 732e 6973 5f65 6d70  rt events.is_emp
+00002120: 7479 2069 7320 4661 6c73 650a 0a23 205b  ty is False..# [
+00002130: 312e 395d 2043 6f6e 7665 7274 2044 6174  1.9] Convert Dat
+00002140: 6120 6f62 6a65 6374 2074 6f20 7468 6520  a object to the 
+00002150: 6c69 7374 206f 6620 656c 656d 656e 7473  list of elements
+00002160: 2865 7665 6e74 7320 6f72 206d 6573 7361  (events or messa
+00002170: 6765 7329 2e0a 2320 4265 2063 6172 6566  ges)..# Be caref
+00002180: 756c 2c20 7468 6973 2063 616e 2074 616b  ul, this can tak
+00002190: 6520 746f 6f20 6d75 6368 206d 656d 6f72  e too much memor
+000021a0: 792e 0a65 7665 6e74 735f 6c69 7374 203d  y..events_list =
+000021b0: 206c 6973 7428 6576 656e 7473 290a 0a23   list(events)..#
+000021c0: 205b 312e 3130 5d20 5468 6520 6361 6368   [1.10] The cach
+000021d0: 6520 696e 6865 7269 7461 6e63 652e 0a23  e inheritance..#
+000021e0: 2043 7265 6174 6573 2061 206e 6577 2044   Creates a new D
+000021f0: 6174 6120 6f62 6a65 6374 2074 6861 7420  ata object that 
+00002200: 7769 6c6c 2075 7365 2063 6163 6865 2066  will use cache f
+00002210: 726f 6d20 7468 6520 6576 656e 7473 2044  rom the events D
+00002220: 6174 6120 6f62 6a65 6374 2e0a 6576 656e  ata object..even
+00002230: 7473 5f66 696c 7465 7265 643a 2044 6174  ts_filtered: Dat
+00002240: 6120 3d20 6576 656e 7473 2e66 696c 7465  a = events.filte
+00002250: 7228 6c61 6d62 6461 2072 6563 6f72 643a  r(lambda record:
+00002260: 2072 6563 6f72 642e 6765 7428 2262 6174   record.get("bat
+00002270: 6368 4964 2229 290a 0a23 204e 6577 2044  chId"))..# New D
+00002280: 6174 6120 6f62 6a65 6374 7320 646f 6e27  ata objects don'
+00002290: 7420 7573 6520 7468 6569 7220 6f77 6e20  t use their own 
+000022a0: 6361 6368 6520 6279 2064 6566 6175 6c74  cache by default
+000022b0: 2062 7574 2075 7365 2074 6865 2063 6163   but use the cac
+000022c0: 6865 206f 6620 7468 6520 7061 7265 6e74  he of the parent
+000022d0: 2044 6174 6120 6f62 6a65 6374 2e0a 2320   Data object..# 
+000022e0: 5573 6520 7573 655f 6361 6368 6520 6d65  Use use_cache me
+000022f0: 7468 6f64 2074 6f20 6163 7469 7661 7465  thod to activate
+00002300: 2063 6163 6869 6e67 2e0a 2320 4166 7465   caching..# Afte
+00002310: 7220 7468 6174 2c20 7468 6520 4461 7461  r that, the Data
+00002320: 206f 626a 6563 7420 7769 6c6c 2063 7265   object will cre
+00002330: 6174 6520 6974 7320 6f77 6e20 6361 6368  ate its own cach
+00002340: 6520 6669 6c65 2e0a 6576 656e 7473 5f66  e file..events_f
+00002350: 696c 7465 7265 642e 7573 655f 6361 6368  iltered.use_cach
+00002360: 6528 290a 0a6c 6973 7428 6576 656e 7473  e()..list(events
+00002370: 5f66 696c 7465 7265 6429 2020 2320 4a75  _filtered)  # Ju
+00002380: 7374 2074 6f20 6974 6572 6174 6520 4461  st to iterate Da
+00002390: 7461 206f 626a 6563 7420 2863 6163 6865  ta object (cache
+000023a0: 2066 696c 6520 7769 6c6c 2062 6520 6372   file will be cr
+000023b0: 6561 7465 6429 2e0a 0a66 696c 7465 7265  eated)...filtere
+000023c0: 645f 6576 656e 7473 5f74 7970 6573 203d  d_events_types =
+000023d0: 2065 7665 6e74 735f 6669 6c74 6572 6564   events_filtered
+000023e0: 2e6d 6170 286c 616d 6264 6120 7265 636f  .map(lambda reco
+000023f0: 7264 3a20 7b22 6576 656e 7454 7970 6522  rd: {"eventType"
+00002400: 3a20 7265 636f 7264 2e67 6574 2822 6576  : record.get("ev
+00002410: 656e 7454 7970 6522 297d 290a 0a65 7665  entType")})..eve
+00002420: 6e74 735f 7769 7468 6f75 745f 7479 7065  nts_without_type
+00002430: 735f 7769 7468 5f62 6174 6368 203d 2066  s_with_batch = f
+00002440: 696c 7465 7265 645f 6576 656e 7473 5f74  iltered_events_t
+00002450: 7970 6573 2e66 696c 7465 7228 6c61 6d62  ypes.filter(lamb
+00002460: 6461 2072 6563 6f72 643a 206e 6f74 2072  da record: not r
+00002470: 6563 6f72 642e 6765 7428 2265 7665 6e74  ecord.get("event
+00002480: 5479 7065 2229 290a 6576 656e 7473 5f77  Type")).events_w
+00002490: 6974 686f 7574 5f74 7970 6573 5f77 6974  ithout_types_wit
+000024a0: 685f 6261 7463 682e 7573 655f 6361 6368  h_batch.use_cach
+000024b0: 6528 290a 0a23 205b 312e 3131 5d20 4461  e()..# [1.11] Da
+000024c0: 7461 206f 626a 6563 7473 206a 6f69 6e69  ta objects joini
+000024d0: 6e67 2e0a 2320 596f 7520 6861 7665 2074  ng..# You have t
+000024e0: 6865 2066 6f6c 6c6f 7769 6e67 2033 2044  he following 3 D
+000024f0: 6174 6120 6f62 6a65 6374 732e 0a64 3120  ata objects..d1 
+00002500: 3d20 4461 7461 285b 312c 2032 2c20 335d  = Data([1, 2, 3]
+00002510: 290a 6432 203d 2044 6174 6128 5b22 6122  ).d2 = Data(["a"
+00002520: 2c20 7b22 6964 223a 2031 3233 7d2c 2022  , {"id": 123}, "
+00002530: 6322 5d29 0a64 3320 3d20 4461 7461 285b  c"]).d3 = Data([
+00002540: 372c 2038 2c20 395d 290a 2320 596f 7520  7, 8, 9]).# You 
+00002550: 6361 6e20 6a6f 696e 2044 6174 6120 6f62  can join Data ob
+00002560: 6a65 6374 7320 696e 2066 6f6c 6c6f 7769  jects in followi
+00002570: 6e67 2077 6179 732e 0a23 2050 6c65 6173  ng ways..# Pleas
+00002580: 6520 6e6f 7465 2c20 6e65 7720 4461 7461  e note, new Data
+00002590: 206f 626a 6563 7420 7769 6c6c 2068 6176   object will hav
+000025a0: 6520 6361 6368 6520 7374 6174 7573 203d  e cache status =
+000025b0: 3d20 4661 6c73 652e 0a64 6174 615f 7669  = False..data_vi
+000025c0: 615f 696e 6974 203d 2044 6174 6128 5b64  a_init = Data([d
+000025d0: 312c 2064 322c 2064 335d 290a 6461 7461  1, d2, d3]).data
+000025e0: 5f76 6961 5f61 6464 203d 2064 3120 2b20  _via_add = d1 + 
+000025f0: 6432 202b 2064 330a 6461 7461 5f77 6974  d2 + d3.data_wit
+00002600: 685f 6e6f 6e5f 6461 7461 5f6f 626a 5f76  h_non_data_obj_v
+00002610: 6961 5f69 6e69 7420 3d20 4461 7461 285b  ia_init = Data([
+00002620: 6431 2c20 5b22 6122 2c20 7b22 6964 223a  d1, ["a", {"id":
+00002630: 2031 3233 7d2c 2022 6322 5d2c 2064 335d   123}, "c"], d3]
+00002640: 290a 6461 7461 5f77 6974 685f 6e6f 6e5f  ).data_with_non_
+00002650: 6461 7461 5f6f 626a 5f76 6961 5f61 6464  data_obj_via_add
+00002660: 203d 2064 3120 2b20 5b22 6122 2c20 7b22   = d1 + ["a", {"
+00002670: 6964 223a 2031 3233 7d2c 2022 6322 5d20  id": 123}, "c"] 
+00002680: 2b20 6433 0a23 2059 6f75 2063 616e 206a  + d3.# You can j
+00002690: 6f69 6e20 6375 7272 656e 7420 4461 7461  oin current Data
+000026a0: 206f 626a 6563 7420 6f6e 2070 6c61 6365   object on place
+000026b0: 2075 7369 6e67 202b 3d2e 0a23 2049 7420   using +=..# It 
+000026c0: 7769 6c6c 206b 6565 7020 6361 6368 6520  will keep cache 
+000026d0: 7374 6174 7573 2e0a 6431 202b 3d20 6433  status..d1 += d3
+000026e0: 2020 2320 6431 2077 696c 6c20 6265 636f    # d1 will beco
+000026f0: 6d65 2044 6174 6128 5b31 2c32 2c33 2c37  me Data([1,2,3,7
+00002700: 2c38 2c39 5d29 0a0a 2320 5b31 2e31 325d  ,8,9])..# [1.12]
+00002710: 2042 7569 6c64 2061 6e64 2072 6561 6420   Build and read 
+00002720: 4461 7461 206f 626a 6563 7420 6361 6368  Data object cach
+00002730: 6520 6669 6c65 732e 0a65 7665 6e74 732e  e files..events.
+00002740: 6275 696c 645f 6361 6368 6528 2263 6163  build_cache("cac
+00002750: 6865 5f66 696c 656e 616d 655f 6f72 5f70  he_filename_or_p
+00002760: 6174 6822 290a 6461 7461 5f6f 626a 5f66  ath").data_obj_f
+00002770: 726f 6d5f 6361 6368 6520 3d20 4461 7461  rom_cache = Data
+00002780: 2e66 726f 6d5f 6361 6368 655f 6669 6c65  .from_cache_file
+00002790: 2822 6361 6368 655f 6669 6c65 6e61 6d65  ("cache_filename
+000027a0: 5f6f 725f 7061 7468 2229 0a0a 2320 5b32  _or_path")..# [2
+000027b0: 5d20 576f 726b 696e 6720 7769 7468 2063  ] Working with c
+000027c0: 6f6e 7665 7274 6572 732e 0a23 2054 6865  onverters..# The
+000027d0: 7265 2061 7265 2063 7572 7265 6e74 6c79  re are currently
+000027e0: 2074 6872 6565 2069 6d70 6c65 6d65 6e74   three implement
+000027f0: 6174 696f 6e73 206f 6620 4954 696d 6573  ations of ITimes
+00002800: 7461 6d70 436f 6e76 6572 7465 7220 636c  tampConverter cl
+00002810: 6173 733a 2044 6174 6574 696d 6543 6f6e  ass: DatetimeCon
+00002820: 7665 7274 652c 2044 6174 6574 696d 6553  verte, DatetimeS
+00002830: 7472 696e 6743 6f6e 7665 7274 6572 2061  tringConverter a
+00002840: 6e64 2050 726f 746f 6275 6654 696d 6573  nd ProtobufTimes
+00002850: 7461 6d70 436f 6e76 6572 7465 722e 0a23  tampConverter..#
+00002860: 2054 6865 7920 616c 6c20 696d 706c 656d   They all implem
+00002870: 656e 7420 7361 6d65 206d 6574 686f 6473  ent same methods
+00002880: 2066 726f 6d20 6261 7365 2063 6c61 7373   from base class
+00002890: 2e0a 2320 4e6f 7465 2074 6861 7420 736f  ..# Note that so
+000028a0: 6d65 2061 6363 7572 6163 7920 6d61 7920  me accuracy may 
+000028b0: 6265 206c 6f73 7420 6475 7269 6e67 2063  be lost during c
+000028c0: 6f6e 7665 7273 696f 6e2e 0a23 2049 6620  onversion..# If 
+000028d0: 666f 7220 6578 616d 706c 6520 796f 7520  for example you 
+000028e0: 7573 6520 746f 5f6d 6963 726f 7365 636f  use to_microseco
+000028f0: 6e64 7320 6e61 6e6f 7365 636f 6e64 7320  nds nanoseconds 
+00002900: 7769 6c6c 2062 6520 6375 7420 6f66 6620  will be cut off 
+00002910: 696e 7374 6561 6420 6f66 2072 6f75 6e64  instead of round
+00002920: 696e 672e 0a0a 2320 5b32 2e31 5d20 4461  ing...# [2.1] Da
+00002930: 7465 7469 6d65 436f 6e76 6572 7465 722e  tetimeConverter.
+00002940: 0a23 2044 6174 6574 696d 6543 6f6e 7665  .# DatetimeConve
+00002950: 7274 6572 2074 616b 6573 2064 6174 6574  rter takes datet
+00002960: 696d 652e 6461 7465 7469 6d65 206f 626a  ime.datetime obj
+00002970: 6563 7420 6173 2069 6e70 7574 2e0a 0a64  ect as input...d
+00002980: 6174 6574 696d 655f 6f62 6a20 3d20 6461  atetime_obj = da
+00002990: 7465 7469 6d65 2879 6561 723d 3230 3233  tetime(year=2023
+000029a0: 2c20 6d6f 6e74 683d 312c 2064 6179 3d35  , month=1, day=5
+000029b0: 2c20 686f 7572 3d31 342c 206d 696e 7574  , hour=14, minut
+000029c0: 653d 3338 2c20 7365 636f 6e64 3d32 352c  e=38, second=25,
+000029d0: 206d 6963 726f 7365 636f 6e64 3d31 3436   microsecond=146
+000029e0: 3029 0a0a 2320 4974 2068 6173 206d 6574  0)..# It has met
+000029f0: 686f 6473 2074 6861 7420 7265 7475 726e  hods that return
+00002a00: 2074 6865 2064 6174 6574 696d 6520 696e   the datetime in
+00002a10: 2064 6966 6665 7265 6e74 2066 6f72 6d61   different forma
+00002a20: 733a 0a0a 6461 7465 5f6d 7320 3d20 4461  s:..date_ms = Da
+00002a30: 7465 7469 6d65 436f 6e76 6572 7465 722e  tetimeConverter.
+00002a40: 746f 5f6d 696c 6c69 7365 636f 6e64 7328  to_milliseconds(
+00002a50: 6461 7465 7469 6d65 5f6f 626a 290a 6461  datetime_obj).da
+00002a60: 7465 5f75 7320 3d20 4461 7465 7469 6d65  te_us = Datetime
+00002a70: 436f 6e76 6572 7465 722e 746f 5f6d 6963  Converter.to_mic
+00002a80: 726f 7365 636f 6e64 7328 6461 7465 7469  roseconds(dateti
+00002a90: 6d65 5f6f 626a 290a 2320 436f 6e76 6572  me_obj).# Conver
+00002aa0: 7469 6e67 2074 6f20 6e61 6e6f 7365 636f  ting to nanoseco
+00002ab0: 6e64 7320 6a75 7374 7320 6164 6473 2074  nds justs adds t
+00002ac0: 6872 6565 2074 7261 696c 696e 6720 7a65  hree trailing ze
+00002ad0: 726f 7320 6173 2064 6174 6574 696d 6520  ros as datetime 
+00002ae0: 6f62 6a65 6374 2064 6f65 736e 2774 2068  object doesn't h
+00002af0: 6176 6520 6e61 6e6f 7365 636f 6e64 732e  ave nanoseconds.
+00002b00: 0a64 6174 655f 6e73 203d 2044 6174 6574  .date_ns = Datet
+00002b10: 696d 6543 6f6e 7665 7274 6572 2e74 6f5f  imeConverter.to_
+00002b20: 6e61 6e6f 7365 636f 6e64 7328 6461 7465  nanoseconds(date
+00002b30: 7469 6d65 5f6f 626a 290a 0a23 205b 322e  time_obj)..# [2.
+00002b40: 325d 2044 6174 6574 696d 6553 7472 696e  2] DatetimeStrin
+00002b50: 6743 6f6e 7665 7274 6572 0a23 2044 6174  gConverter.# Dat
+00002b60: 6574 696d 6553 7472 696e 6743 6f6e 7665  etimeStringConve
+00002b70: 7274 6572 2074 616b 6573 2073 7472 696e  rter takes strin
+00002b80: 6720 696e 2022 7979 7979 2d4d 4d2d 6464  g in "yyyy-MM-dd
+00002b90: 5448 483a 6d6d 3a73 735b 2e53 5353 5353  THH:mm:ss[.SSSSS
+00002ba0: 5353 5353 5d5a 2220 666f 726d 6174 2e0a  SSSS]Z" format..
+00002bb0: 0a64 6174 655f 7374 7269 6e67 203d 2022  .date_string = "
+00002bc0: 3230 3233 2d30 312d 3035 5431 343a 3338  2023-01-05T14:38
+00002bd0: 3a32 352e 3030 3134 365a 220a 0a23 2057  :25.00146Z"..# W
+00002be0: 6520 6861 7665 2073 616d 6520 6d65 7468  e have same meth
+00002bf0: 6f64 7320 6173 2069 6e20 4461 7465 7469  ods as in Dateti
+00002c00: 6d65 436f 6e76 6572 7465 720a 6461 7465  meConverter.date
+00002c10: 5f6d 735f 6672 6f6d 5f73 7472 696e 6720  _ms_from_string 
+00002c20: 3d20 4461 7465 7469 6d65 5374 7269 6e67  = DatetimeString
+00002c30: 436f 6e76 6572 7465 722e 746f 5f6d 696c  Converter.to_mil
+00002c40: 6c69 7365 636f 6e64 7328 6461 7465 5f73  liseconds(date_s
+00002c50: 7472 696e 6729 0a64 6174 655f 7573 5f66  tring).date_us_f
+00002c60: 726f 6d5f 7374 7269 6e67 203d 2044 6174  rom_string = Dat
+00002c70: 6574 696d 6553 7472 696e 6743 6f6e 7665  etimeStringConve
+00002c80: 7274 6572 2e74 6f5f 6d69 6372 6f73 6563  rter.to_microsec
+00002c90: 6f6e 6473 2864 6174 655f 7374 7269 6e67  onds(date_string
+00002ca0: 290a 6461 7465 5f6e 735f 6672 6f6d 5f73  ).date_ns_from_s
+00002cb0: 7472 696e 6720 3d20 4461 7465 7469 6d65  tring = Datetime
+00002cc0: 5374 7269 6e67 436f 6e76 6572 7465 722e  StringConverter.
+00002cd0: 746f 5f6e 616e 6f73 6563 6f6e 6473 2864  to_nanoseconds(d
+00002ce0: 6174 655f 7374 7269 6e67 290a 0a23 2057  ate_string)..# W
+00002cf0: 6520 6361 6e20 616c 736f 2067 6574 2064  e can also get d
+00002d00: 6174 6574 696d 6520 6f62 6a65 6374 2066  atetime object f
+00002d10: 726f 6d20 7374 7269 6e67 0a64 6174 6574  rom string.datet
+00002d20: 696d 655f 6672 6f6d 5f73 7472 696e 6720  ime_from_string 
+00002d30: 3d20 4461 7465 7469 6d65 5374 7269 6e67  = DatetimeString
+00002d40: 436f 6e76 6572 7465 722e 746f 5f64 6174  Converter.to_dat
+00002d50: 6574 696d 6528 6461 7465 5f73 7472 696e  etime(date_strin
+00002d60: 6729 0a0a 2320 5b32 2e33 5d20 5072 6f74  g)..# [2.3] Prot
+00002d70: 6f62 7566 5469 6d65 7374 616d 7043 6f6e  obufTimestampCon
+00002d80: 7665 7274 6572 0a23 2050 726f 746f 6275  verter.# Protobu
+00002d90: 6620 7469 6d65 7374 616d 7073 206d 7573  f timestamps mus
+00002da0: 7420 6265 2069 6e20 666f 726d 207b 2265  t be in form {"e
+00002db0: 706f 6368 5365 636f 6e64 223a 2073 6563  pochSecond": sec
+00002dc0: 6f6e 6473 2c20 226e 616e 6f22 3a20 6e61  onds, "nano": na
+00002dd0: 6e6f 7365 636f 6e64 737d 0a0a 7072 6f74  noseconds}..prot
+00002de0: 6f62 7566 5f74 696d 6573 7461 6d70 203d  obuf_timestamp =
+00002df0: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
+00002e00: 2031 3637 3239 3239 3530 352c 2022 6e61   1672929505, "na
+00002e10: 6e6f 223a 2031 5f34 3630 5f30 3030 7d0a  no": 1_460_000}.
+00002e20: 0a64 6174 655f 6d73 5f66 726f 6d5f 7469  .date_ms_from_ti
+00002e30: 6d65 7374 616d 7020 3d20 5072 6f74 6f62  mestamp = Protob
+00002e40: 7566 5469 6d65 7374 616d 7043 6f6e 7665  ufTimestampConve
+00002e50: 7274 6572 2e74 6f5f 6d69 6c6c 6973 6563  rter.to_millisec
+00002e60: 6f6e 6473 2870 726f 746f 6275 665f 7469  onds(protobuf_ti
+00002e70: 6d65 7374 616d 7029 0a64 6174 655f 7573  mestamp).date_us
+00002e80: 5f66 726f 6d5f 7469 6d65 7374 616d 7020  _from_timestamp 
+00002e90: 3d20 5072 6f74 6f62 7566 5469 6d65 7374  = ProtobufTimest
+00002ea0: 616d 7043 6f6e 7665 7274 6572 2e74 6f5f  ampConverter.to_
+00002eb0: 6d69 6372 6f73 6563 6f6e 6473 2870 726f  microseconds(pro
+00002ec0: 746f 6275 665f 7469 6d65 7374 616d 7029  tobuf_timestamp)
+00002ed0: 0a64 6174 655f 6e73 5f66 726f 6d5f 7469  .date_ns_from_ti
+00002ee0: 6d65 7374 616d 7020 3d20 5072 6f74 6f62  mestamp = Protob
+00002ef0: 7566 5469 6d65 7374 616d 7043 6f6e 7665  ufTimestampConve
+00002f00: 7274 6572 2e74 6f5f 6e61 6e6f 7365 636f  rter.to_nanoseco
+00002f10: 6e64 7328 7072 6f74 6f62 7566 5f74 696d  nds(protobuf_tim
+00002f20: 6573 7461 6d70 290a 6461 7465 7469 6d65  estamp).datetime
+00002f30: 5f66 726f 6d5f 7469 6d65 7374 616d 7020  _from_timestamp 
+00002f40: 3d20 5072 6f74 6f62 7566 5469 6d65 7374  = ProtobufTimest
+00002f50: 616d 7043 6f6e 7665 7274 6572 2e74 6f5f  ampConverter.to_
+00002f60: 6461 7465 7469 6d65 2870 726f 746f 6275  datetime(protobu
+00002f70: 665f 7469 6d65 7374 616d 7029 0a0a 2320  f_timestamp)..# 
+00002f80: 5b33 5d20 576f 726b 696e 6720 7769 7468  [3] Working with
+00002f90: 2045 7665 6e74 5472 6565 2061 6e64 2045   EventTree and E
+00002fa0: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
+00002fb0: 6f6e 2e0a 0a23 205b 332e 315d 2042 7569  on...# [3.1] Bui
+00002fc0: 6c64 2061 2063 7573 746f 6d20 4576 656e  ld a custom Even
+00002fd0: 7454 7265 650a 2320 546f 2063 7265 6174  tTree.# To creat
+00002fe0: 6520 616e 2045 7665 6e74 5472 6565 206f  e an EventTree o
+00002ff0: 626a 6563 7420 796f 7520 6e65 6564 2074  bject you need t
+00003000: 6f20 7072 6f76 6964 6520 6e61 6d65 2c20  o provide name, 
+00003010: 6964 2061 6e64 2064 6174 6120 6f66 2074  id and data of t
+00003020: 6865 2072 6f6f 7420 6576 656e 742e 0a74  he root event..t
+00003030: 7265 6520 3d20 4576 656e 7454 7265 6528  ree = EventTree(
+00003040: 6576 656e 745f 6e61 6d65 3d22 726f 6f74  event_name="root
+00003050: 2065 7665 6e74 222c 2065 7665 6e74 5f69   event", event_i
+00003060: 643d 2272 6f6f 745f 6964 222c 2064 6174  d="root_id", dat
+00003070: 613d 7b22 6461 7461 223a 205b 312c 2032  a={"data": [1, 2
+00003080: 2c20 332c 2034 2c20 355d 7d29 0a0a 2320  , 3, 4, 5]})..# 
+00003090: 546f 2061 6464 206e 6577 206e 6f64 6520  To add new node 
+000030a0: 7573 6520 6170 7065 6e64 5f65 7665 6e74  use append_event
+000030b0: 2e20 7061 7265 6e74 5f69 6420 6973 206e  . parent_id is n
+000030c0: 6563 6573 7361 7279 2c20 6461 7461 2069  ecessary, data i
+000030d0: 7320 6f70 7469 6f6e 616c 2e0a 7472 6565  s optional..tree
+000030e0: 2e61 7070 656e 645f 6576 656e 7428 6576  .append_event(ev
+000030f0: 656e 745f 6e61 6d65 3d22 4122 2c20 6576  ent_name="A", ev
+00003100: 656e 745f 6964 3d22 415f 6964 222c 2064  ent_id="A_id", d
+00003110: 6174 613d 4e6f 6e65 2c20 7061 7265 6e74  ata=None, parent
+00003120: 5f69 643d 2272 6f6f 745f 6964 2229 0a0a  _id="root_id")..
+00003130: 2320 5b33 2e33 5d20 4275 696c 6469 6e67  # [3.3] Building
+00003140: 2074 6865 2045 7665 6e74 5472 6565 436f   the EventTreeCo
+00003150: 6c6c 6563 7469 6f6e 2e0a 0a23 2049 6620  llection...# If 
+00003160: 796f 7520 646f 6e27 7420 7370 6563 6966  you don't specif
+00003170: 7920 6461 7461 5f73 6f75 7263 6520 666f  y data_source fo
+00003180: 7220 7468 6520 6472 6976 6572 2074 6865  r the driver the
+00003190: 6e20 6974 2077 6f6e 2774 2072 6563 6f76  n it won't recov
+000031a0: 6572 2064 6574 6163 6865 6420 6576 656e  er detached even
+000031b0: 7473 2e0a 6472 6976 6572 3a20 4945 5443  ts..driver: IETC
+000031c0: 4472 6976 6572 2020 2320 596f 7520 7368  Driver  # You sh
+000031d0: 6f75 6c64 2069 6e69 7420 4554 4344 7269  ould init ETCDri
+000031e0: 7665 7220 6f62 6a65 6374 2e20 452e 672e  ver object. E.g.
+000031f0: 2066 726f 6d20 4c77 4450 206d 6f64 756c   from LwDP modul
+00003200: 6520 6f72 2079 6f75 7220 6375 7374 6f6d  e or your custom
+00003210: 2063 6c61 7373 2e0a 6574 6320 3d20 4576   class..etc = Ev
+00003220: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+00003230: 6e28 6472 6976 6572 290a 6574 632e 6275  n(driver).etc.bu
+00003240: 696c 6428 6576 656e 7473 290a 0a23 2044  ild(events)..# D
+00003250: 6574 6163 6865 6420 6576 656e 7473 2069  etached events i
+00003260: 736e 2774 2065 6d70 7479 2e0a 6173 7365  sn't empty..asse
+00003270: 7274 2065 7463 2e67 6574 5f64 6574 6163  rt etc.get_detac
+00003280: 6865 645f 6576 656e 7473 2829 0a0a 6574  hed_events()..et
+00003290: 6320 3d20 4576 656e 7454 7265 6543 6f6c  c = EventTreeCol
+000032a0: 6c65 6374 696f 6e28 6472 6976 6572 290a  lection(driver).
+000032b0: 2320 4465 7461 6368 6564 2065 7665 6e74  # Detached event
+000032c0: 7320 6172 6520 656d 7074 7920 6265 6361  s are empty beca
+000032d0: 7573 6520 7468 6579 2077 6572 6520 7265  use they were re
+000032e0: 636f 7665 7265 642e 0a61 7373 6572 7420  covered..assert 
+000032f0: 6e6f 7420 6574 632e 6765 745f 6465 7461  not etc.get_deta
+00003300: 6368 6564 5f65 7665 6e74 7328 290a 0a23  ched_events()..#
+00003310: 2054 6865 2063 6f6c 6c65 6374 696f 6e20   The collection 
+00003320: 6861 7320 4576 656e 7454 7265 6573 2065  has EventTrees e
+00003330: 6163 6820 7769 7468 2061 2074 7265 6520  ach with a tree 
+00003340: 6f66 2065 7665 6e74 732e 0a23 2055 7369  of events..# Usi
+00003350: 6e67 2043 6f6c 6c65 6374 696f 6e20 616e  ng Collection an
+00003360: 6420 4576 656e 7454 7265 6573 2c20 796f  d EventTrees, yo
+00003370: 7520 6361 6e20 776f 726b 2066 6c65 7869  u can work flexi
+00003380: 626c 7920 7769 7468 2065 7665 6e74 732e  bly with events.
+00003390: 0a0a 2320 5b33 2e33 2e31 5d20 4765 7420  ..# [3.3.1] Get 
+000033a0: 6c65 6176 6573 206f 6620 616c 6c20 7472  leaves of all tr
+000033b0: 6565 732e 0a6c 6561 7665 733a 2054 7570  ees..leaves: Tup
+000033c0: 6c65 5b64 6963 745d 203d 2065 7463 2e67  le[dict] = etc.g
+000033d0: 6574 5f6c 6561 7665 7328 290a 0a23 205b  et_leaves()..# [
+000033e0: 332e 332e 325d 2047 6574 2072 6f6f 7473  3.3.2] Get roots
+000033f0: 2069 6473 206f 6620 616c 6c20 7472 6565   ids of all tree
+00003400: 732e 0a72 6f6f 7473 3a20 4c69 7374 5b73  s..roots: List[s
+00003410: 7472 5d20 3d20 6574 632e 6765 745f 726f  tr] = etc.get_ro
+00003420: 6f74 735f 6964 7328 290a 0a23 205b 332e  ots_ids()..# [3.
+00003430: 332e 335d 2046 696e 6420 616e 2065 7665  3.3] Find an eve
+00003440: 6e74 2069 6e20 616c 6c20 7472 6565 732e  nt in all trees.
+00003450: 0a66 696e 645f 6576 656e 743a 204f 7074  .find_event: Opt
+00003460: 696f 6e61 6c5b 6469 6374 5d20 3d20 6574  ional[dict] = et
+00003470: 632e 6669 6e64 286c 616d 6264 6120 6576  c.find(lambda ev
+00003480: 656e 743a 2022 5365 6e64 206d 6573 7361  ent: "Send messa
+00003490: 6765 2220 696e 2065 7665 6e74 5b22 6576  ge" in event["ev
+000034a0: 656e 7454 7970 6522 5d29 0a0a 2320 5b33  entType"])..# [3
+000034b0: 2e33 2e34 5d20 4669 6e64 2061 6c6c 2065  .3.4] Find all e
+000034c0: 7665 6e74 7320 696e 2061 6c6c 2074 7265  vents in all tre
+000034d0: 6573 2e20 5468 6572 6520 6973 2061 6c73  es. There is als
+000034e0: 6f20 6974 6572 6162 6c65 2076 6572 7369  o iterable versi
+000034f0: 6f6e 2027 6669 6e64 616c 6c5f 6974 6572  on 'findall_iter
+00003500: 272e 0a66 696e 645f 6576 656e 7473 3a20  '..find_events: 
+00003510: 4c69 7374 5b64 6963 745d 203d 2065 7463  List[dict] = etc
+00003520: 2e66 696e 6461 6c6c 286c 616d 6264 6120  .findall(lambda 
+00003530: 6576 656e 743a 2065 7665 6e74 5b22 7375  event: event["su
+00003540: 6363 6573 7366 756c 225d 2069 7320 5472  ccessful"] is Tr
+00003550: 7565 290a 0a23 205b 332e 332e 355d 2046  ue)..# [3.3.5] F
+00003560: 696e 6420 616e 2061 6e63 6573 746f 7220  ind an ancestor 
+00003570: 6f66 2074 6865 2065 7665 6e74 2e0a 616e  of the event..an
+00003580: 6365 7374 6f72 3a20 4f70 7469 6f6e 616c  cestor: Optional
+00003590: 5b64 6963 745d 203d 2065 7463 2e66 696e  [dict] = etc.fin
+000035a0: 645f 616e 6365 7374 6f72 280a 2020 2020  d_ancestor(.    
+000035b0: 2238 6262 6533 3731 372d 6366 3539 2d31  "8bbe3717-cf59-1
+000035c0: 3165 622d 6133 6637 2d30 3934 6639 3034  1eb-a3f7-094f904
+000035d0: 6333 6136 3222 2c20 6669 6c74 6572 3d6c  c3a62", filter=l
+000035e0: 616d 6264 6120 6576 656e 743a 2022 526f  ambda event: "Ro
+000035f0: 6f74 4576 656e 7422 2069 6e20 6576 656e  otEvent" in even
+00003600: 745b 2265 7665 6e74 4e61 6d65 225d 0a29  t["eventName"].)
+00003610: 0a0a 2320 5b33 2e33 2e36 5d20 4765 7420  ..# [3.3.6] Get 
+00003620: 6368 696c 6472 656e 206f 6620 7468 6520  children of the 
+00003630: 6576 656e 742e 2054 6865 7265 2069 7320  event. There is 
+00003640: 616c 736f 2069 7465 7261 626c 6520 7665  also iterable ve
+00003650: 7273 696f 6e20 2767 6574 5f63 6869 6c64  rsion 'get_child
+00003660: 7265 6e5f 6974 6572 272e 0a63 6869 6c64  ren_iter'..child
+00003670: 7265 6e3a 2054 7570 6c65 5b64 6963 745d  ren: Tuple[dict]
+00003680: 203d 2065 7463 2e67 6574 5f63 6869 6c64   = etc.get_child
+00003690: 7265 6e28 2238 3134 3432 3265 312d 3963  ren("814422e1-9c
+000036a0: 3638 2d31 3165 622d 3835 3938 2d36 3931  68-11eb-8598-691
+000036b0: 6562 6437 6634 3133 6422 290a 0a23 205b  ebd7f413d")..# [
+000036c0: 332e 332e 375d 2047 6574 2073 7562 7472  3.3.7] Get subtr
+000036d0: 6565 2066 6f72 2073 7065 6369 6669 6564  ee for specified
+000036e0: 2065 7665 6e74 2e0a 7375 6274 7265 653a   event..subtree:
+000036f0: 2045 7665 6e74 5472 6565 203d 2065 7463   EventTree = etc
+00003700: 2e67 6574 5f73 7562 7472 6565 2822 3865  .get_subtree("8e
+00003710: 3233 3737 3464 2d63 6635 392d 3131 6562  23774d-cf59-11eb
+00003720: 2d61 3665 332d 3535 6266 6462 3262 3366  -a6e3-55bfdb2b3f
+00003730: 3231 2229 0a0a 2320 5b33 2e33 2e38 5d20  21")..# [3.3.8] 
+00003740: 4765 7420 6675 6c6c 2070 6174 6820 746f  Get full path to
+00003750: 2074 6865 2065 7665 6e74 2e0a 2320 4c6f   the event..# Lo
+00003760: 6f6b 7320 6c69 6b65 205b 616e 6365 7374  oks like [ancest
+00003770: 6f72 5f72 6f6f 742c 2061 6e63 6573 746f  or_root, ancesto
+00003780: 725f 6c65 7665 6c31 2c20 616e 6365 7374  r_level1, ancest
+00003790: 6f72 5f6c 6576 656c 322c 2065 7665 6e74  or_level2, event
+000037a0: 5d0a 6576 656e 745f 7061 7468 3a20 4c69  ].event_path: Li
+000037b0: 7374 5b64 6963 745d 203d 2065 7463 2e67  st[dict] = etc.g
+000037c0: 6574 5f66 756c 6c5f 7061 7468 2822 3865  et_full_path("8e
+000037d0: 3235 3234 6661 2d63 6635 392d 3131 6562  2524fa-cf59-11eb
+000037e0: 2d61 3366 372d 3039 3466 3930 3463 3361  -a3f7-094f904c3a
+000037f0: 3632 2229 0a0a 2320 5b33 2e33 2e39 5d20  62")..# [3.3.9] 
+00003800: 4765 7420 7061 7265 6e74 206f 6620 7468  Get parent of th
+00003810: 6520 6576 656e 742e 0a70 6172 656e 7420  e event..parent 
+00003820: 3d20 6574 632e 6765 745f 7061 7265 6e74  = etc.get_parent
+00003830: 2822 3865 3235 3234 6661 2d63 6635 392d  ("8e2524fa-cf59-
+00003840: 3131 6562 2d61 3366 372d 3039 3466 3930  11eb-a3f7-094f90
+00003850: 3463 3361 3632 2229 0a0a 2320 5b33 2e33  4c3a62")..# [3.3
+00003860: 2e31 305d 2041 7070 656e 6420 6e65 7720  .10] Append new 
+00003870: 6576 656e 7420 746f 2074 6865 2063 6f6c  event to the col
+00003880: 6c65 6374 696f 6e2e 0a65 7463 2e61 7070  lection..etc.app
+00003890: 656e 645f 6576 656e 7428 0a20 2020 2065  end_event(.    e
+000038a0: 7665 6e74 3d7b 0a20 2020 2020 2020 2022  vent={.        "
+000038b0: 6576 656e 7449 6422 3a20 2261 3230 6635  eventId": "a20f5
+000038c0: 6566 342d 6333 6665 2d62 6231 302d 6132  ef4-c3fe-bb10-a2
+000038d0: 3963 2d64 6433 6437 3834 3930 3965 6222  9c-dd3d784909eb"
+000038e0: 2c0a 2020 2020 2020 2020 2270 6172 656e  ,.        "paren
+000038f0: 7445 7665 6e74 4964 223a 2022 3865 3235  tEventId": "8e25
+00003900: 3234 6661 2d63 6635 392d 3131 6562 2d61  24fa-cf59-11eb-a
+00003910: 3366 372d 3039 3466 3930 3463 3361 3632  3f7-094f904c3a62
+00003920: 222c 0a20 2020 2020 2020 2022 6576 656e  ",.        "even
+00003930: 744e 616d 6522 3a20 2253 7475 6245 7665  tName": "StubEve
+00003940: 6e74 222c 0a20 2020 207d 0a29 0a0a 2320  nt",.    }.)..# 
+00003950: 5b33 2e33 2e31 315d 2053 686f 7720 7468  [3.3.11] Show th
+00003960: 6520 656e 7469 7265 2063 6f6c 6c65 6374  e entire collect
+00003970: 696f 6e2e 0a65 7463 2e73 686f 7728 290a  ion..etc.show().
+00003980: 0a23 205b 332e 345d 2057 6f72 6b69 6e67  .# [3.4] Working
+00003990: 2077 6974 6820 7468 6520 4576 656e 7454   with the EventT
+000039a0: 7265 652e 0a23 2045 7665 6e74 5472 6565  ree..# EventTree
+000039b0: 2068 6173 2074 6865 2073 616d 6520 6d65   has the same me
+000039c0: 7468 6f64 7320 6173 2045 7665 6e74 5472  thods as EventTr
+000039d0: 6565 436f 6c6c 6563 7469 6f6e 2c20 6275  eeCollection, bu
+000039e0: 7420 6f6e 6c79 2066 6f72 2069 7473 206f  t only for its o
+000039f0: 776e 2074 7265 652e 0a0a 2320 5b33 2e34  wn tree...# [3.4
+00003a00: 2e31 5d20 4765 7420 636f 6c6c 6563 7469  .1] Get collecti
+00003a10: 6f6e 2074 7265 6573 2e0a 7472 6565 733a  on trees..trees:
+00003a20: 204c 6973 745b 4576 656e 7454 7265 655d   List[EventTree]
+00003a30: 203d 2065 7463 2e67 6574 5f74 7265 6573   = etc.get_trees
+00003a40: 2829 0a74 7265 653a 2045 7665 6e74 5472  ().tree: EventTr
+00003a50: 6565 203d 2074 7265 6573 5b30 5d0a 0a23  ee = trees[0]..#
+00003a60: 2042 7574 2045 7665 6e74 5472 6565 2070   But EventTree p
+00003a70: 726f 7669 6465 7320 6120 776f 726b 2077  rovides a work w
+00003a80: 6974 6820 7468 6520 7472 6565 2c20 6275  ith the tree, bu
+00003a90: 7420 646f 6573 206e 6f74 206d 6f64 6966  t does not modif
+00003aa0: 7920 6974 2e0a 2320 4966 2079 6f75 2077  y it..# If you w
+00003ab0: 616e 7420 746f 206d 6f64 6966 7920 7468  ant to modify th
+00003ac0: 6520 7472 6565 2c20 7573 6520 4576 656e  e tree, use Even
+00003ad0: 7454 7265 6543 6f6c 6c65 6374 696f 6e73  tTreeCollections
+00003ae0: 2e0a 0a23 205b 332e 355d 2057 6f72 6b69  ...# [3.5] Worki
+00003af0: 6e67 2077 6974 6820 5061 7265 6e74 6c65  ng with Parentle
+00003b00: 7373 5472 6565 2e0a 2320 5061 7265 6e74  ssTree..# Parent
+00003b10: 6c65 7373 5472 6565 2069 7320 4576 656e  lessTree is Even
+00003b20: 7454 7265 6520 7768 6963 6820 6861 7320  tTree which has 
+00003b30: 6465 7461 6368 6564 2065 7665 6e74 7320  detached events 
+00003b40: 7769 7468 2073 7475 6273 2e0a 7061 7265  with stubs..pare
+00003b50: 6e74 6c65 7373 5f74 7265 6573 3a20 4c69  ntless_trees: Li
+00003b60: 7374 5b45 7665 6e74 5472 6565 5d20 3d20  st[EventTree] = 
+00003b70: 6574 632e 6765 745f 7061 7265 6e74 6c65  etc.get_parentle
+00003b80: 7373 5f74 7265 6573 2829 0a0a 2320 5b33  ss_trees()..# [3
+00003b90: 2e36 5d20 576f 726b 696e 6720 7769 7468  .6] Working with
+00003ba0: 2050 6172 656e 7445 7665 6e74 5472 6565   ParentEventTree
+00003bb0: 436f 6c6c 6563 7469 6f6e 2e0a 2320 5061  Collection..# Pa
+00003bc0: 7265 6e74 4576 656e 7454 7265 6543 6f6c  rentEventTreeCol
+00003bd0: 6c65 6374 696f 6e20 6973 2061 2074 7265  lection is a tre
+00003be0: 6520 636f 6c6c 6563 7469 6f6e 206c 696b  e collection lik
+00003bf0: 6520 4576 656e 7454 7265 6543 6f6c 6c65  e EventTreeColle
+00003c00: 6374 696f 6e2c 0a23 2062 7574 2069 7420  ction,.# but it 
+00003c10: 6861 7320 6f6e 6c79 2065 7665 6e74 7320  has only events 
+00003c20: 7468 6174 2068 6176 6520 7265 6665 7265  that have refere
+00003c30: 6e63 6573 2e0a 6461 7461 5f73 6f75 7263  nces..data_sourc
+00003c40: 653a 2049 4461 7461 536f 7572 6365 2020  e: IDataSource  
+00003c50: 2320 596f 7520 7368 6f75 6c64 2069 6e69  # You should ini
+00003c60: 7420 4461 7461 536f 7572 6365 206f 626a  t DataSource obj
+00003c70: 6563 742e 2045 2e67 2e20 6672 6f6d 204c  ect. E.g. from L
+00003c80: 7744 5020 6d6f 6475 6c65 2e0a 2320 4554  wDP module..# ET
+00003c90: 4344 7269 7665 7220 6865 7265 2069 7320  CDriver here is 
+00003ca0: 6120 7374 7562 2c20 6163 7475 616c 6c79  a stub, actually
+00003cb0: 2074 6865 206c 6962 2064 6f6e 2774 2068   the lib don't h
+00003cc0: 6176 6520 7375 6368 2063 6c61 7373 2e0a  ave such class..
+00003cd0: 2320 596f 7520 6361 6e20 7461 6b65 2069  # You can take i
+00003ce0: 7420 696e 204c 7744 5020 6d6f 6475 6c65  t in LwDP module
+00003cf0: 206f 7220 6372 6561 7465 2079 6f75 7273   or create yours
+00003d00: 656c 6620 636c 6173 7320 6966 2079 6f75  elf class if you
+00003d10: 2068 6176 6520 736f 6d65 2073 7065 6369   have some speci
+00003d20: 616c 2065 7665 6e74 7320 7374 7275 6374  al events struct
+00003d30: 7572 652e 0a64 7269 7665 7220 3d20 4554  ure..driver = ET
+00003d40: 4344 7269 7665 7228 6461 7461 5f73 6f75  CDriver(data_sou
+00003d50: 7263 653d 6461 7461 5f73 6f75 7263 6529  rce=data_source)
+00003d60: 0a65 7463 203d 2050 6172 656e 7445 7665  .etc = ParentEve
+00003d70: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
+00003d80: 2864 7269 7665 7229 0a65 7463 2e62 7569  (driver).etc.bui
+00003d90: 6c64 2865 7665 6e74 7329 0a0a 6574 632e  ld(events)..etc.
+00003da0: 7368 6f77 2829 0a60 6060 0a3c 212d 2d20  show().```.<!-- 
+00003db0: 656e 6420 6765 745f 7374 6172 7465 645f  end get_started_
+00003dc0: 6578 616d 706c 652e 7079 202d 2d3e 0a0a  example.py -->..
+00003dd0: 2323 2032 2e33 2e20 5368 6f72 7420 7468  ## 2.3. Short th
+00003de0: 656f 7279 0a0a 5468 6520 6c69 6272 6172  eory..The librar
+00003df0: 7920 7072 6f76 6964 6573 2074 6f6f 6c73  y provides tools
+00003e00: 2066 6f72 2068 616e 646c 696e 6720 7374   for handling st
+00003e10: 7265 616d 2064 6174 612e 2057 6861 7427  ream data. What'
+00003e20: 7320 6120 7374 7265 616d 3f20 4974 2773  s a stream? It's
+00003e30: 2061 2073 6571 7565 6e63 6520 6f66 2065   a sequence of e
+00003e40: 6c65 6d65 6e74 7320 6672 6f6d 2061 2073  lements from a s
+00003e50: 6f75 7263 6520 7468 6174 0a73 7570 706f  ource that.suppo
+00003e60: 7274 7320 6167 6772 6567 6174 6520 6f70  rts aggregate op
+00003e70: 6572 6174 696f 6e73 2e0a 0a23 2323 2054  erations...### T
+00003e80: 6572 6d73 0a0a 2d20 2a2a 4461 7461 206f  erms..- **Data o
+00003e90: 626a 6563 742a 2a3a 2041 6e20 696e 7374  bject**: An inst
+00003ea0: 616e 6365 206f 6620 6044 6174 6160 2063  ance of `Data` c
+00003eb0: 6c61 7373 2077 6869 6368 2069 7320 7772  lass which is wr
+00003ec0: 6170 7065 7220 756e 6465 7220 7374 7265  apper under stre
+00003ed0: 616d 2e0a 2d20 2a2a 5365 7175 656e 6365  am..- **Sequence
+00003ee0: 206f 6620 656c 656d 656e 7473 2a2a 3a0a   of elements**:.
+00003ef0: 2020 4120 5f44 6174 6120 6f62 6a65 6374    A _Data object
+00003f00: 5f20 7072 6f76 6964 6573 2061 6e20 696e  _ provides an in
+00003f10: 7465 7266 6163 6520 746f 2061 2073 6571  terface to a seq
+00003f20: 7565 6e63 6564 2073 6574 206f 6620 7661  uenced set of va
+00003f30: 6c75 6573 206f 6620 6120 7370 6563 6966  lues of a specif
+00003f40: 6963 2065 6c65 6d65 6e74 2074 7970 652e  ic element type.
+00003f50: 2053 7472 6561 6d20 696e 7369 6465 2074   Stream inside t
+00003f60: 6865 205f 4461 7461 0a20 206f 626a 6563  he _Data.  objec
+00003f70: 745f 202a 2a64 6f6e 1974 2061 6374 7561  t_ **don.t actua
+00003f80: 6c6c 7920 7374 6f72 652a 2a20 656c 656d  lly store** elem
+00003f90: 656e 7473 3b20 7468 6579 2061 7265 2063  ents; they are c
+00003fa0: 6f6d 7075 7465 6420 6f6e 2064 656d 616e  omputed on deman
+00003fb0: 642e 0a2d 202a 2a64 6174 6120 736f 7572  d..- **data sour
+00003fc0: 6365 2a2a 2028 6578 6163 746c 7920 696e  ce** (exactly in
+00003fd0: 2073 6d61 6c6c 206c 6574 7465 7273 293a   small letters):
+00003fe0: 0a20 2041 6e79 2073 6f75 7263 6520 6f66  .  Any source of
+00003ff0: 2064 6174 612e 2045 2e67 2e20 5b4c 6967   data. E.g. [Lig
+00004000: 6874 7765 6967 6874 2044 6174 6120 5072  htweight Data Pr
+00004010: 6f76 6964 6572 5d28 6874 7470 733a 2f2f  ovider](https://
+00004020: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
+00004030: 6574 2f74 6832 2d6c 772d 6461 7461 2d70  et/th2-lw-data-p
+00004040: 726f 7669 6465 7229 2c20 636f 6c6c 6563  rovider), collec
+00004050: 7469 6f6e 732c 0a20 2061 7272 6179 732c  tions,.  arrays,
+00004060: 206f 7220 492f 4f20 7265 736f 7572 6365   or I/O resource
+00004070: 732e 0a2d 202a 2a44 6174 6153 6f75 7263  s..- **DataSourc
+00004080: 652a 2a3a 0a20 2041 2063 6c61 7373 2074  e**:.  A class t
+00004090: 6861 7420 6973 2061 6e20 696e 7465 726d  hat is an interm
+000040a0: 6564 6961 7465 206c 696e 6b20 6265 7477  ediate link betw
+000040b0: 6565 6e20 7468 6520 536f 7572 6365 4150  een the SourceAP
+000040c0: 4920 616e 6420 436f 6d6d 616e 6473 2e0a  I and Commands..
+000040d0: 2d20 2a2a 536f 7572 6365 4150 492a 2a3a  - **SourceAPI**:
+000040e0: 0a20 2045 6163 6820 736f 7572 6365 2068  .  Each source h
+000040f0: 6173 2069 7473 206f 776e 2041 5049 2074  as its own API t
+00004100: 6f20 7265 7472 6965 7665 2064 6174 612e  o retrieve data.
+00004110: 2053 6f75 7263 6541 5049 2069 7320 6120   SourceAPI is a 
+00004120: 636c 6173 7320 7468 6174 2070 726f 7669  class that provi
+00004130: 6465 2041 5049 2066 6f72 2073 6f6d 6520  de API for some 
+00004140: 6461 7461 2073 6f75 7263 652e 0a2d 202a  data source..- *
+00004150: 2a43 6f6d 6d61 6e64 732a 2a3a 0a20 2043  *Commands**:.  C
+00004160: 6c61 7373 6573 2074 6861 7420 7072 6f76  lasses that prov
+00004170: 6964 6520 7573 6572 2d66 7269 656e 646c  ide user-friendl
+00004180: 7920 696e 7465 7266 6163 6573 2066 6f72  y interfaces for
+00004190: 2067 6574 7469 6e67 2073 6f6d 6520 6461   getting some da
+000041a0: 7461 2066 726f 6d20 4461 7461 536f 7572  ta from DataSour
+000041b0: 6365 2e20 436f 6d6d 616e 6473 2075 7365  ce. Commands use
+000041c0: 205f 536f 7572 6365 4150 495f 2074 6f0a   _SourceAPI_ to.
+000041d0: 2020 6163 6869 6576 6520 6974 2e0a 2d20    achieve it..- 
+000041e0: 2a2a 4164 6170 7465 7273 2a2a 3a0a 2020  **Adapters**:.  
+000041f0: 4974 2773 2073 696d 696c 6172 2074 6f20  It's similar to 
+00004200: 6675 6e63 7469 6f6e 2066 6f72 2060 4461  function for `Da
+00004210: 7461 2e6d 6170 6020 6d65 7468 6f64 2e20  ta.map` method. 
+00004220: 4164 6f70 7461 626c 6520 636f 6d6d 616e  Adoptable comman
+00004230: 6473 2075 7365 6420 6974 2074 6f20 7570  ds used it to up
+00004240: 6461 7465 2074 6865 2064 6174 6120 7374  date the data st
+00004250: 7265 616d 2e0a 2d20 2a2a 4167 6772 6567  ream..- **Aggreg
+00004260: 6174 6520 6f70 6572 6174 696f 6e73 2a2a  ate operations**
+00004270: 3a0a 2020 436f 6d6d 6f6e 206f 7065 7261  :.  Common opera
+00004280: 7469 6f6e 7320 7375 6368 2061 7320 6669  tions such as fi
+00004290: 6c74 6572 2c20 6d61 702c 206c 696d 6974  lter, map, limit
+000042a0: 2061 6e64 2073 6f20 6f6e 2e0a 2d20 2a2a   and so on..- **
+000042b0: 576f 726b 666c 6f77 2a2a 3a20 416e 206f  Workflow**: An o
+000042c0: 7264 6572 6564 2073 6574 206f 6620 5f41  rdered set of _A
+000042d0: 6767 7265 6761 7465 206f 7065 7261 7469  ggregate operati
+000042e0: 6f6e 735f 2e0a 0a23 2323 2043 6f6e 6365  ons_...### Conce
+000042f0: 7074 0a0a 5468 6520 6c69 6272 6172 7920  pt..The library 
+00004300: 6465 7363 7269 6265 7320 7468 6520 6869  describes the hi
+00004310: 6768 2d6c 6576 656c 2069 6e74 6572 6661  gh-level interfa
+00004320: 6365 7320 6049 536f 7572 6365 4150 4960  ces `ISourceAPI`
+00004330: 2c20 6049 4461 7461 536f 7572 6365 602c  , `IDataSource`,
+00004340: 2060 4943 6f6d 6d61 6e64 602c 2060 4941   `ICommand`, `IA
+00004350: 6461 7074 6572 602e 0a0a 416e 7920 6461  dapter`...Any da
+00004360: 7461 2073 6f75 7263 6520 6d75 7374 2062  ta source must b
+00004370: 6520 6465 7363 7269 6265 6420 6279 2074  e described by t
+00004380: 6865 2060 4944 6174 6153 6f75 7263 6560  he `IDataSource`
+00004390: 2061 6273 7472 6163 7420 636c 6173 732e   abstract class.
+000043a0: 2054 6865 7365 2063 616e 2062 6520 5f46   These can be _F
+000043b0: 696c 6544 6174 6153 6f75 7263 655f 2c20  ileDataSource_, 
+000043c0: 0a5f 4353 5644 6174 6153 6f75 7263 655f  ._CSVDataSource_
+000043d0: 2c20 5f44 4244 6174 6153 6f75 7263 655f  , _DBDataSource_
+000043e0: 2061 6e64 206f 7468 6572 2e0a 0a55 7375   and other...Usu
+000043f0: 616c 6c79 2c20 6461 7461 2073 6f75 7263  ally, data sourc
+00004400: 6573 2068 6176 6520 736f 6d65 206b 696e  es have some kin
+00004410: 6420 6f66 2041 5049 2e20 4461 7461 6261  d of API. Databa
+00004420: 7365 7320 2d20 7072 6f76 6964 6520 5351  ses - provide SQ
+00004430: 4c20 6c61 6e67 7561 6765 2c20 7768 656e  L language, when
+00004440: 2077 6f72 6b69 6e67 2077 6974 6820 6120   working with a 
+00004450: 6669 6c65 2c20 796f 7520 6361 6e20 7265  file, you can re
+00004460: 6164 0a6c 696e 6520 6279 206c 696e 652c  ad.line by line,
+00004470: 2065 7463 2e20 5468 6973 2041 5049 2069   etc. This API i
+00004480: 7320 6465 7363 7269 6265 6420 6279 2074  s described by t
+00004490: 6865 2060 4953 6f75 7263 6541 5049 6020  he `ISourceAPI` 
+000044a0: 636c 6173 732e 2042 6563 6175 7365 2064  class. Because d
+000044b0: 6966 6665 7265 6e74 2076 6572 7369 6f6e  ifferent version
+000044c0: 7320 6f66 2074 6865 2073 616d 6520 6461  s of the same da
+000044d0: 7461 2073 6f75 7263 650a 6d61 7920 6861  ta source.may ha
+000044e0: 7665 2064 6966 6665 7265 6e74 2041 5049  ve different API
+000044f0: 2c20 6974 2069 7320 6265 7474 6572 2074  , it is better t
+00004500: 6f20 6372 6561 7465 2061 2063 6c61 7373  o create a class
+00004510: 2066 6f72 2065 6163 6820 7665 7273 696f   for each versio
+00004520: 6e2e 0a0a 4765 6e65 7261 6c6c 792c 2064  n...Generally, d
+00004530: 6174 6120 736f 7572 6365 2041 5049 7320  ata source APIs 
+00004540: 6172 6520 6869 6464 656e 2062 6568 696e  are hidden behin
+00004550: 6420 636f 6e76 656e 6965 6e74 2069 6e74  d convenient int
+00004560: 6572 6661 6365 732e 2054 6865 2072 6f6c  erfaces. The rol
+00004570: 6520 6f66 2074 6865 7365 2069 6e74 6572  e of these inter
+00004580: 6661 6365 7320 6973 2070 6c61 7965 640a  faces is played.
+00004590: 6279 2060 4943 6f6d 6d61 6e64 6020 636c  by `ICommand` cl
+000045a0: 6173 7365 732e 0a0a 6049 4164 6170 7465  asses...`IAdapte
+000045b0: 7260 2063 6c61 7373 6573 2074 7261 6e73  r` classes trans
+000045c0: 666f 726d 2064 6174 6120 7374 7265 616d  form data stream
+000045d0: 206c 696b 6520 6675 6e63 7469 6f6e 7320   like functions 
+000045e0: 666f 7220 6044 6174 612e 6d61 7060 206d  for `Data.map` m
+000045f0: 6574 686f 642e 2045 7373 656e 7469 616c  ethod. Essential
+00004600: 6c79 2069 7427 7320 7468 6520 7361 6d65  ly it's the same
+00004610: 2074 6869 6e67 2062 7574 206d 6f72 650a   thing but more.
+00004620: 666c 6578 6962 6c65 2e0a 0a46 6f72 2065  flexible...For e
+00004630: 7861 6d70 6c65 2c20 4c77 4450 2044 6174  xample, LwDP Dat
+00004640: 6153 6f75 7263 6528 6874 7470 733a 2f2f  aSource(https://
+00004650: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
+00004660: 6574 2f74 6832 2d64 732d 736f 7572 6365  et/th2-ds-source
+00004670: 2d6c 7764 7029 2075 7365 7320 7468 6573  -lwdp) uses thes
+00004680: 6520 6162 7374 7261 6374 2063 6c61 7373  e abstract class
+00004690: 6573 2074 6f20 6275 696c 6420 6974 7320  es to build its 
+000046a0: 696d 706c 656d 656e 7461 7469 6f6e 2e59  implementation.Y
+000046b0: 6f75 2063 616e 2065 6173 696c 7920 6372  ou can easily cr
+000046c0: 6561 7465 2079 6f75 7220 6f77 6e20 756e  eate your own un
+000046d0: 6971 7565 2063 6f6d 6d61 6e64 7320 666f  ique commands fo
+000046e0: 7220 5f4c 7744 5020 4461 7461 536f 7572  r _LwDP DataSour
+000046f0: 6365 5f2c 2061 7320 7765 6c6c 2061 7320  ce_, as well as 
+00004700: 656e 7469 7265 0a5f 4461 7461 536f 7572  entire._DataSour
+00004710: 6365 5f20 636c 6173 7365 732e 205b 4865  ce_ classes. [He
+00004720: 7265 2069 7320 6120 646f 6375 6d65 6e74  re is a document
+00004730: 6174 696f 6e5d 2864 6f63 756d 656e 7461  ation](documenta
+00004740: 7469 6f6e 2f64 6174 6173 6f75 7263 652e  tion/datasource.
+00004750: 6d64 2920 6f6e 2068 6f77 2074 6f20 696d  md) on how to im
+00004760: 706c 656d 656e 7420 7468 6573 6520 696e  plement these in
+00004770: 7465 7266 6163 6573 2e0a 0a21 5b44 6174  terfaces...![Dat
+00004780: 6120 7374 7265 616d 2070 6970 656c 696e  a stream pipelin
+00004790: 655d 2864 6f63 756d 656e 7461 7469 6f6e  e](documentation
+000047a0: 2f69 6d67 2f63 6f6e 6365 7074 2e70 6e67  /img/concept.png
+000047b0: 290a 0a23 2323 2053 7472 6561 6d20 6f70  )..### Stream op
+000047c0: 6572 6174 696f 6e73 0a0a 4675 7274 6865  erations..Furthe
+000047d0: 726d 6f72 652c 2073 7472 6561 6d20 6f70  rmore, stream op
+000047e0: 6572 6174 696f 6e73 2068 6176 6520 7477  erations have tw
+000047f0: 6f20 6675 6e64 616d 656e 7461 6c20 6368  o fundamental ch
+00004800: 6172 6163 7465 7269 7374 6963 7320 7468  aracteristics th
+00004810: 6174 206d 616b 6520 7468 656d 2076 6572  at make them ver
+00004820: 7920 6469 6666 6572 656e 7420 6672 6f6d  y different from
+00004830: 2063 6f6c 6c65 6374 696f 6e0a 6f70 6572   collection.oper
+00004840: 6174 696f 6e73 3a20 5f50 6970 656c 696e  ations: _Pipelin
+00004850: 696e 675f 2061 6e64 205f 496e 7465 726e  ing_ and _Intern
+00004860: 616c 2069 7465 7261 7469 6f6e 5f2e 0a0a  al iteration_...
+00004870: 2323 2323 2050 6970 656c 696e 696e 670a  #### Pipelining.
+00004880: 0a4d 616e 7920 7374 7265 616d 206f 7065  .Many stream ope
+00004890: 7261 7469 6f6e 7320 7265 7475 726e 2061  rations return a
+000048a0: 2073 7472 6561 6d20 7468 656d 7365 6c76   stream themselv
+000048b0: 6573 2e20 5468 6973 2061 6c6c 6f77 7320  es. This allows 
+000048c0: 6f70 6572 6174 696f 6e73 2074 6f20 6265  operations to be
+000048d0: 2063 6861 696e 6564 2074 6f20 666f 726d   chained to form
+000048e0: 2061 206c 6172 6765 7220 7069 7065 6c69   a larger pipeli
+000048f0: 6e65 2e0a 0a21 5b44 6174 6120 7374 7265  ne...![Data stre
+00004900: 616d 2070 6970 656c 696e 655d 2864 6f63  am pipeline](doc
+00004910: 756d 656e 7461 7469 6f6e 2f69 6d67 2f64  umentation/img/d
+00004920: 6174 615f 7374 7265 616d 5f70 6970 656c  ata_stream_pipel
+00004930: 696e 652e 706e 6729 0a0a 2323 2323 2049  ine.png)..#### I
+00004940: 6e74 6572 6e61 6c20 6974 6572 6174 696f  nternal iteratio
+00004950: 6e0a 0a49 6e20 636f 6e74 7261 7374 2074  n..In contrast t
+00004960: 6f20 636f 6c6c 6563 7469 6f6e 732c 2077  o collections, w
+00004970: 6869 6368 2061 7265 2069 7465 7261 7465  hich are iterate
+00004980: 6420 6578 706c 6963 6974 6c79 2028 6578  d explicitly (ex
+00004990: 7465 726e 616c 2069 7465 7261 7469 6f6e  ternal iteration
+000049a0: 292c 2073 7472 6561 6d20 6f70 6572 6174  ), stream operat
+000049b0: 696f 6e73 2064 6f20 7468 6520 6974 6572  ions do the iter
+000049c0: 6174 696f 6e0a 6265 6869 6e64 2074 6865  ation.behind the
+000049d0: 2073 6365 6e65 7320 666f 7220 796f 752e   scenes for you.
+000049e0: 204e 6f74 652c 2069 7420 646f 6573 6e27   Note, it doesn'
+000049f0: 7420 6d65 616e 2079 6f75 2063 616e 6e6f  t mean you canno
+00004a00: 7420 6974 6572 6174 6520 7468 6520 5f44  t iterate the _D
+00004a10: 6174 6120 6f62 6a65 6374 5f2e 0a0a 2323  ata object_...##
+00004a20: 2320 4461 7461 2063 6163 6869 6e67 0a0a  # Data caching..
+00004a30: 5468 6520 5f44 6174 6120 6f62 6a65 6374  The _Data object
+00004a40: 5f20 7072 6f76 6964 6573 2074 6865 2061  _ provides the a
+00004a50: 6269 6c69 7479 2074 6f20 7573 6520 7468  bility to use th
+00004a60: 6520 6361 6368 652e 2054 6865 2063 6163  e cache. The cac
+00004a70: 6865 2077 6f72 6b73 2066 6f72 2065 6163  he works for eac
+00004a80: 6820 5f44 6174 6120 6f62 6a65 6374 5f2c  h _Data object_,
+00004a90: 2074 6861 7420 6973 2c20 796f 7520 6368   that is, you ch
+00004aa0: 6f6f 7365 0a77 6869 6368 205f 4461 7461  oose.which _Data
+00004ab0: 206f 626a 6563 745f 2079 6f75 2077 616e   object_ you wan
+00004ac0: 7420 746f 2073 6176 652e 2054 6865 205f  t to save. The _
+00004ad0: 4461 7461 206f 626a 6563 745f 2063 6163  Data object_ cac
+00004ae0: 6865 2069 7320 7361 7665 6420 6166 7465  he is saved afte
+00004af0: 7220 7468 6520 6669 7273 7420 6974 6572  r the first iter
+00004b00: 6174 696f 6e2c 2062 7574 2074 6865 2069  ation, but the i
+00004b10: 7465 7261 7469 6f6e 0a73 6f75 7263 6520  teration.source 
+00004b20: 6d61 7920 6265 2064 6966 6665 7265 6e74  may be different
+00004b30: 2e0a 0a49 6620 796f 7520 646f 6e27 7420  ...If you don't 
+00004b40: 7573 6520 7468 6520 6361 6368 652c 2079  use the cache, y
+00004b50: 6f75 7220 736f 7572 6365 2077 696c 6c20  our source will 
+00004b60: 6265 2074 6865 2064 6174 6120 736f 7572  be the data sour
+00004b70: 6365 2079 6f75 2068 6176 6520 696e 2074  ce you have in t
+00004b80: 6865 205f 4461 7461 204f 626a 6563 745f  he _Data Object_
+00004b90: 2e20 4275 7420 6966 2079 6f75 2075 7365  . But if you use
+00004ba0: 2074 6865 2063 6163 6865 2c0a 796f 7572   the cache,.your
+00004bb0: 2073 6f75 7263 6520 6361 6e20 6265 2074   source can be t
+00004bc0: 6865 2064 6174 6120 736f 7572 6365 2c20  he data source, 
+00004bd0: 7468 6520 7061 7265 6e74 2063 6163 6865  the parent cache
+00004be0: 2c20 6f72 206f 776e 2063 6163 6865 3a0a  , or own cache:.
+00004bf0: 0a2a 2054 6865 2064 6174 6120 736f 7572  .* The data sour
+00004c00: 6365 3a0a 2020 4966 2074 6865 205f 4461  ce:.  If the _Da
+00004c10: 7461 204f 626a 6563 745f 2064 6f65 736e  ta Object_ doesn
+00004c20: 2774 2068 6176 6520 6120 7061 7265 6e74  't have a parent
+00004c30: 2063 6163 6865 2061 6e64 2069 7473 2063   cache and its c
+00004c40: 6163 6865 2e0a 2a20 5468 6520 7061 7265  ache..* The pare
+00004c50: 6e74 2063 6163 6865 3a0a 2020 4966 2074  nt cache:.  If t
+00004c60: 6865 205f 4461 7461 204f 626a 6563 745f  he _Data Object_
+00004c70: 2068 6173 2061 2070 6172 656e 7420 6361   has a parent ca
+00004c80: 6368 652e 2049 7420 646f 6573 6e27 7420  che. It doesn't 
+00004c90: 6d61 7474 6572 2077 6861 7420 706f 7369  matter what posi
+00004ca0: 7469 6f6e 2074 6865 2070 6172 656e 7420  tion the parent 
+00004cb0: 6361 6368 6520 6861 7320 696e 2069 6e68  cache has in inh
+00004cc0: 6572 6974 616e 6365 2e0a 2020 5f44 6174  eritance..  _Dat
+00004cd0: 6120 4f62 6a65 6374 5f20 756e 6465 7273  a Object_ unders
+00004ce0: 7461 6e64 7320 7768 6f73 6520 6361 6368  tands whose cach
+00004cf0: 6520 6974 2069 7320 616e 6420 6578 6563  e it is and exec
+00004d00: 7574 6573 2074 6865 2070 6172 7420 6f66  utes the part of
+00004d10: 2074 6865 2077 6f72 6b66 6c6f 7720 7468   the workflow th
+00004d20: 6174 2077 6173 206e 6f74 2065 7865 6375  at was not execu
+00004d30: 7465 642e 0a2a 2054 6865 206f 776e 2063  ted..* The own c
+00004d40: 6163 6865 3a0a 2020 4966 2069 7420 6973  ache:.  If it is
+00004d50: 206e 6f74 2074 6865 2066 6972 7374 2069   not the first i
+00004d60: 7465 7261 7469 6f6e 206f 6620 7468 6973  teration of this
+00004d70: 2044 6174 6120 6f62 6a65 6374 2e0a 0a4e   Data object...N
+00004d80: 6f74 6520 7468 6174 2074 6865 2063 6163  ote that the cac
+00004d90: 6865 2073 7461 7465 206f 6620 7468 6520  he state of the 
+00004da0: 4461 7461 206f 626a 6563 7420 6973 206e  Data object is n
+00004db0: 6f74 2069 6e68 6572 6974 6564 2e0a 0a23  ot inherited...#
+00004dc0: 2323 2320 466f 7263 6564 2063 6163 6869  ### Forced cachi
+00004dd0: 6e67 0a59 6f75 2063 616e 2074 656c 6c20  ng.You can tell 
+00004de0: 4453 2074 6f20 6361 6368 6520 6461 7461  DS to cache data
+00004df0: 2074 6f20 7370 6563 6966 6963 2063 6163   to specific cac
+00004e00: 6865 2066 696c 652c 2077 6869 6368 2077  he file, which w
+00004e10: 6f6e 2774 2062 6520 6465 6c65 7465 6420  on't be deleted 
+00004e20: 6166 7465 7220 7363 7269 7074 2065 6e64  after script end
+00004e30: 2e0a 596f 7520 6361 6e20 7365 6520 6578  ..You can see ex
+00004e40: 616d 706c 6520 696e 2031 2e31 3220 7365  ample in 1.12 se
+00004e50: 6374 696f 6e20 6f66 205b 6765 745f 7374  ction of [get_st
+00004e60: 6172 7465 645f 6578 616d 706c 655d 2865  arted_example](e
+00004e70: 7861 6d70 6c65 732f 6765 745f 7374 6172  xamples/get_star
+00004e80: 7465 645f 6578 616d 706c 652e 7079 292e  ted_example.py).
+00004e90: 0a0a 0a23 2323 2045 7665 6e74 5472 6565  ...### EventTree
+00004ea0: 2061 6e64 2063 6f6c 6c65 6374 696f 6e73   and collections
+00004eb0: 0a0a 2323 2323 2045 7665 6e74 5472 6565  ..#### EventTree
+00004ec0: 0a0a 6045 7665 6e74 5472 6565 6020 6973  ..`EventTree` is
+00004ed0: 2061 2074 7265 652d 6261 7365 6420 6461   a tree-based da
+00004ee0: 7461 2073 7472 7563 7475 7265 206f 6620  ta structure of 
+00004ef0: 6576 656e 7473 2e20 4974 2061 6c6c 6f77  events. It allow
+00004f00: 7320 796f 7520 6765 7420 6368 696c 6472  s you get childr
+00004f10: 656e 2061 6e64 2070 6172 656e 7473 206f  en and parents o
+00004f20: 6620 6576 656e 742c 200a 6469 7370 6c61  f event, .displa
+00004f30: 7920 7472 6565 2c20 6765 7420 6675 6c6c  y tree, get full
+00004f40: 2070 6174 6820 746f 2065 7665 6e74 2065   path to event e
+00004f50: 7463 2e0a 0a44 6574 6169 6c73 3a0a 0a2a  tc...Details:..*
+00004f60: 2060 4576 656e 7454 7265 6560 2063 6f6e   `EventTree` con
+00004f70: 7461 696e 7320 616c 6c20 6576 656e 7473  tains all events
+00004f80: 2069 6e20 6d65 6d6f 7279 2e0a 2a20 5472   in memory..* Tr
+00004f90: 6565 2068 6173 2073 6f6d 6520 696d 706f  ee has some impo
+00004fa0: 7274 616e 7420 7465 726d 733a 0a20 2020  rtant terms:.   
+00004fb0: 2031 2e20 5f41 6e63 6573 746f 725f 2069   1. _Ancestor_ i
+00004fc0: 7320 616e 7920 7265 6c61 7469 7665 206f  s any relative o
+00004fd0: 6620 7468 6520 6576 656e 7420 7570 2074  f the event up t
+00004fe0: 6865 2074 7265 6520 2867 7261 6e64 7061  he tree (grandpa
+00004ff0: 7265 6e74 2c20 7061 7265 6e74 2065 7463  rent, parent etc
+00005000: 2e29 2e0a 2020 2020 322e 205f 5061 7265  .)..    2. _Pare
+00005010: 6e74 5f20 6973 206f 6e6c 7920 7468 6520  nt_ is only the 
+00005020: 6669 7273 7420 7265 6c61 7469 7665 206f  first relative o
+00005030: 6620 7468 6520 6576 656e 7420 7570 2074  f the event up t
+00005040: 6865 2074 7265 652e 0a20 2020 2033 2e20  he tree..    3. 
+00005050: 5f43 6869 6c64 5f20 6973 2074 6865 2066  _Child_ is the f
+00005060: 6972 7374 2072 656c 6174 6976 6520 6f66  irst relative of
+00005070: 2074 6865 2065 7665 6e74 2064 6f77 6e20   the event down 
+00005080: 7468 6520 7472 6565 2e0a 0a54 616b 6520  the tree...Take 
+00005090: 6120 6c6f 6f6b 2061 7420 7468 6520 666f  a look at the fo
+000050a0: 6c6c 6f77 696e 6720 4854 4d4c 2074 7265  llowing HTML tre
+000050b0: 6520 746f 2075 6e64 6572 7374 616e 6420  e to understand 
+000050c0: 7468 656d 2e0a 0a20 2020 6060 600a 2020  them...   ```.  
+000050d0: 2020 3c62 6f64 793e 203c 212d 2d20 616e    <body> <!-- an
+000050e0: 6365 7374 6f72 2028 6772 616e 6470 6172  cestor (grandpar
+000050f0: 656e 7429 2c20 6275 7420 6e6f 7420 7061  ent), but not pa
+00005100: 7265 6e74 202d 2d3e 0a20 2020 2020 2020  rent -->.       
+00005110: 203c 6469 763e 203c 212d 2d20 7061 7265   <div> <!-- pare
+00005120: 6e74 2026 2061 6e63 6573 746f 7220 2d2d  nt & ancestor --
+00005130: 3e0a 2020 2020 2020 2020 2020 2020 3c70  >.            <p
+00005140: 3e48 656c 6c6f 2c20 776f 726c 6421 3c2f  >Hello, world!</
+00005150: 703e 203c 212d 2d20 6368 696c 6420 2d2d  p> <!-- child --
+00005160: 3e0a 2020 2020 2020 2020 2020 2020 3c70  >.            <p
+00005170: 3e47 6f6f 6462 7965 213c 2f70 3e20 3c21  >Goodbye!</p> <!
+00005180: 2d2d 2073 6962 6c69 6e67 202d 2d3e 0a20  -- sibling -->. 
+00005190: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+000051a0: 2020 3c2f 626f 6479 3e0a 2020 2060 6060    </body>.   ```
+000051b0: 0a0a 2323 2323 2043 6f6c 6c65 6374 696f  ..#### Collectio
+000051c0: 6e73 0a0a 2a2a 4576 656e 7454 7265 6543  ns..**EventTreeC
+000051d0: 6f6c 6c65 6374 696f 6e2a 2a20 6973 2061  ollection** is a
+000051e0: 2063 6f6c 6c65 6374 696f 6e20 6f66 2045   collection of E
+000051f0: 7665 6e74 5472 6565 732e 2054 6865 2063  ventTrees. The c
+00005200: 6f6c 6c65 6374 696f 6e20 6275 696c 6473  ollection builds
+00005210: 2061 2066 6577 205f 4576 656e 7454 7265   a few _EventTre
+00005220: 655f 2062 7920 7061 7373 6564 205f 4461  e_ by passed _Da
+00005230: 7461 0a6f 626a 6563 745f 2e20 416c 7468  ta.object_. Alth
+00005240: 6f75 6768 2079 6f75 2063 616e 2063 6861  ough you can cha
+00005250: 6e67 6520 7468 6520 7472 6565 2064 6972  nge the tree dir
+00005260: 6563 746c 792c 2069 7427 7320 6265 7474  ectly, it's bett
+00005270: 6572 2074 6f20 646f 2069 7420 7468 726f  er to do it thro
+00005280: 7567 6820 636f 6c6c 6563 7469 6f6e 7320  ugh collections 
+00005290: 6265 6361 7573 6520 7468 6579 2061 7265  because they are
+000052a0: 2061 7761 7265 206f 660a 6064 6574 6163   aware of.`detac
+000052b0: 6865 645f 6576 656e 7473 6020 616e 6420  hed_events` and 
+000052c0: 6361 6e20 736f 6c76 6520 736f 6d65 2065  can solve some e
+000052d0: 7665 6e74 7320 6465 7065 6e64 656e 6369  vents dependenci
+000052e0: 6573 2e20 5468 6520 636f 6c6c 6563 7469  es. The collecti
+000052f0: 6f6e 2068 6173 2073 696d 696c 6172 2066  on has similar f
+00005300: 6561 7475 7265 7320 6c69 6b65 2061 2073  eatures like a s
+00005310: 696e 676c 6520 5f45 7665 6e74 5472 6565  ingle _EventTree
+00005320: 5f0a 6275 7420 6170 706c 7969 6e67 2074  _.but applying t
+00005330: 6865 6d20 666f 7220 616c 6c20 5f45 7665  hem for all _Eve
+00005340: 6e74 5472 6565 735f 2e0a 0a2a 2a50 6172  ntTrees_...**Par
+00005350: 656e 7445 7665 6e74 5472 6565 436f 6c6c  entEventTreeColl
+00005360: 6563 7469 6f6e 2a2a 2069 7320 6120 636f  ection** is a co
+00005370: 6c6c 6563 7469 6f6e 2073 696d 696c 6172  llection similar
+00005380: 2074 6f20 5f45 7665 6e74 5472 6565 436f   to _EventTreeCo
+00005390: 6c6c 6563 7469 6f6e 5f20 6275 7420 636f  llection_ but co
+000053a0: 6e74 6169 6e69 6e67 206f 6e6c 7920 7061  ntaining only pa
+000053b0: 7265 6e74 2065 7665 6e74 7320 7468 6174  rent events that
+000053c0: 0a61 7265 2072 6566 6572 656e 6365 6420  .are referenced 
+000053d0: 696e 2074 6865 2064 6174 6120 7374 7265  in the data stre
+000053e0: 616d 2e20 5468 6520 636f 6c6c 6563 7469  am. The collecti
+000053f0: 6f6e 2068 6173 2066 6561 7475 7265 7320  on has features 
+00005400: 7369 6d69 6c61 7220 746f 205f 4576 656e  similar to _Even
+00005410: 7454 7265 6543 6f6c 6c65 6374 696f 6e5f  tTreeCollection_
+00005420: 2e0a 0a44 6574 6169 6c73 3a0a 0a2a 2054  ...Details:..* T
+00005430: 6f20 7573 6520 4554 2063 6f6c 6c65 6374  o use ET collect
+00005440: 696f 6e73 2079 6f75 206e 6565 6420 746f  ions you need to
+00005450: 2069 6e69 7469 616c 697a 6520 7468 656d   initialize them
+00005460: 2062 7920 5f45 5443 4472 6976 6572 5f2e   by _ETCDriver_.
+00005470: 2044 6174 6120 736f 7572 6365 7320 7573   Data sources us
+00005480: 7561 6c6c 7920 7072 6f76 6964 6520 7468  ually provide th
+00005490: 656d 2e0a 2020 596f 7520 6361 6e20 6372  em..  You can cr
+000054a0: 6561 7465 2069 7420 6279 2079 6f75 7273  eate it by yours
+000054b0: 656c 6620 6465 7065 6e64 696e 6720 6f6e  elf depending on
+000054c0: 2079 6f75 7220 6461 7461 2073 7472 7563   your data struc
+000054d0: 7475 7265 2e20 200a 2a20 5468 6520 636f  ture.  .* The co
+000054e0: 6c6c 6563 7469 6f6e 2068 6173 2061 2066  llection has a f
+000054f0: 6561 7475 7265 2074 6f20 7265 636f 7665  eature to recove
+00005500: 7220 6576 656e 7473 2e20 416c 6c20 6576  r events. All ev
+00005510: 656e 7473 2074 6861 7420 6172 6520 6e6f  ents that are no
+00005520: 7420 696e 2074 6865 2072 6563 6569 7665  t in the receive
+00005530: 6420 6461 7461 2073 7472 6561 6d2c 2062  d data stream, b
+00005540: 7574 2077 6869 6368 2061 7265 0a20 2072  ut which are.  r
+00005550: 6566 6572 656e 6365 6420 7769 6c6c 2062  eferenced will b
+00005560: 6520 6c6f 6164 6564 2066 726f 6d20 7468  e loaded from th
+00005570: 6520 6461 7461 2073 6f75 7263 652e 0a2a  e data source..*
+00005580: 2059 6f75 2063 616e 2074 616b 6520 6064   You can take `d
+00005590: 6574 6163 6865 645f 6576 656e 7473 6020  etached_events` 
+000055a0: 746f 2073 6565 2077 6869 6368 2065 7665  to see which eve
+000055b0: 6e74 7320 6172 6520 6d69 7373 696e 672e  nts are missing.
+000055c0: 0a2a 2049 6620 796f 7520 7761 6e74 2c20  .* If you want, 
+000055d0: 796f 7520 6361 6e20 6275 696c 6420 7061  you can build pa
+000055e0: 7265 6e74 6c65 7373 2074 7265 6573 2077  rentless trees w
+000055f0: 6865 7265 2074 6865 206d 6973 7369 6e67  here the missing
+00005600: 2065 7665 6e74 7320 6172 6520 7374 7562   events are stub
+00005610: 6265 6420 696e 7374 6561 642e 204a 7573  bed instead. Jus
+00005620: 740a 2020 7573 6520 6067 6574 5f70 6172  t.  use `get_par
+00005630: 656e 746c 6573 735f 7472 6565 7328 2960  entless_trees()`
+00005640: 2e0a 0a52 6571 7569 7265 6d65 6e74 733a  ...Requirements:
+00005650: 0a0a 312e 2045 7665 6e74 7320 7072 6f76  ..1. Events prov
+00005660: 6964 6564 2074 6f20 4554 4320 6861 7665  ided to ETC have
+00005670: 2074 6f20 6861 7665 2060 6576 656e 745f   to have `event_
+00005680: 6e61 6d65 602c 2060 6576 656e 745f 6964  name`, `event_id
+00005690: 602c 2060 7061 7265 6e74 5f65 7665 6e74  `, `parent_event
+000056a0: 5f69 6460 2066 6965 6c64 732e 2054 6865  _id` fields. The
+000056b0: 7920 0a63 616e 2068 6176 6520 616e 6f74  y .can have anot
+000056c0: 6865 7220 6e61 6d65 7320 2869 7420 7265  her names (it re
+000056d0: 736f 6c76 6573 2069 6e20 7468 6520 6472  solves in the dr
+000056e0: 6976 6572 292e 0a0a 2323 2323 2048 696e  iver)...#### Hin
+000056f0: 7473 0a0a 2a20 5265 6d6f 7665 2061 6c6c  ts..* Remove all
+00005700: 2075 6e6e 6563 6573 7361 7279 2066 6965   unnecessary fie
+00005710: 6c64 7320 6672 6f6d 2065 7665 6e74 7320  lds from events 
+00005720: 6265 666f 7265 2070 6173 7369 6e67 2074  before passing t
+00005730: 6f20 6120 5f63 6f6c 6c65 6374 696f 6e5f  o a _collection_
+00005740: 2074 6f20 7265 6475 6365 206d 656d 6f72   to reduce memor
+00005750: 7920 7573 6167 652e 0a2a 2055 7365 2060  y usage..* Use `
+00005760: 7368 6f77 2829 6020 6d65 7468 6f64 2074  show()` method t
+00005770: 6f20 7072 696e 7420 7468 6520 7472 6565  o print the tree
+00005780: 2069 6e20 7472 6565 2d6c 696b 6520 7669   in tree-like vi
+00005790: 6577 2e0a 2a20 4e6f 7465 2074 6861 7420  ew..* Note that 
+000057a0: 7468 6520 6067 6574 5f78 6020 6d65 7468  the `get_x` meth
+000057b0: 6f64 7320 7769 6c6c 2072 6169 7365 2061  ods will raise a
+000057c0: 6e20 6578 6365 7074 696f 6e20 6966 2079  n exception if y
+000057d0: 6f75 2070 6173 7320 616e 2075 6e6b 6e6f  ou pass an unkno
+000057e0: 776e 2065 7665 6e74 2069 642c 2075 6e6c  wn event id, unl
+000057f0: 696b 6520 7468 6520 6066 696e 645f 7860  ike the `find_x`
+00005800: 206d 6574 686f 6473 2028 0a20 2074 6865   methods (.  the
+00005810: 7920 7265 7475 726e 204e 6f6e 6529 2e0a  y return None)..
+00005820: 2a20 4966 2079 6f75 2077 616e 7420 746f  * If you want to
+00005830: 206b 6e6f 7720 7468 6174 2073 7065 6369   know that speci
+00005840: 6669 6564 2065 7665 6e74 2065 7869 7374  fied event exist
+00005850: 732c 2075 7365 2074 6865 2070 7974 686f  s, use the pytho
+00005860: 6e20 6069 6e60 206b 6579 776f 7264 2028  n `in` keyword (
+00005870: 652e 672e 2060 2765 7665 6e74 2d69 6427  e.g. `'event-id'
+00005880: 2069 6e20 6576 656e 7473 5f74 7265 6560   in events_tree`
+00005890: 292e 0a2a 2055 7365 2074 6865 2070 7974  )..* Use the pyt
+000058a0: 686f 6e20 606c 656e 6020 6b65 7977 6f72  hon `len` keywor
+000058b0: 6420 746f 2067 6574 2065 7665 6e74 7320  d to get events 
+000058c0: 6e75 6d62 6572 2069 6e20 7468 6520 7472  number in the tr
+000058d0: 6565 2e0a 0a23 2323 2046 6965 6c64 7352  ee...### FieldsR
+000058e0: 6573 6f6c 7665 720a 5468 6520 6964 6561  esolver.The idea
+000058f0: 206f 6620 7573 696e 6720 7265 736f 6c76   of using resolv
+00005900: 6572 733a 2020 0a49 7420 736f 6c76 6573  ers:  .It solves
+00005910: 2074 6865 2070 726f 626c 656d 206f 6620   the problem of 
+00005920: 6861 7669 6e67 2061 2066 6577 2044 6174  having a few Dat
+00005930: 6153 6f75 7263 6573 2077 6974 6820 7468  aSources with th
+00005940: 6520 7361 6d65 2064 6174 612c 200a 6275  e same data, .bu
+00005950: 7420 7769 7468 2064 6966 6665 7265 6e74  t with different
+00005960: 2077 6179 7320 746f 2067 6574 2069 742e   ways to get it.
+00005970: 0a0a 5468 6573 6520 636c 6173 7365 7320  ..These classes 
+00005980: 7072 6f76 6964 6520 796f 7520 6765 7474  provide you gett
+00005990: 6572 206d 6574 686f 6473 2e20 0a55 7369  er methods. .Usi
+000059a0: 6e67 2074 6865 7365 2063 6c61 7373 6573  ng these classes
+000059b0: 2061 6c6c 6f77 7320 796f 7520 746f 2066   allows you to f
+000059c0: 7265 656c 7920 7377 6974 6368 2062 6574  reely switch bet
+000059d0: 7765 656e 2064 6966 6665 7265 6e74 2064  ween different d
+000059e0: 6174 6120 0a66 6f72 6d61 7473 2061 6e64  ata .formats and
+000059f0: 2064 6f6e 2774 2063 6861 6e67 6520 796f   don't change yo
+00005a00: 7572 2063 6f64 652e 200a 0a52 6573 6f6c  ur code. ..Resol
+00005a10: 7665 7273 2073 6f6c 7665 2074 6865 2070  vers solve the p
+00005a20: 726f 626c 656d 206f 6620 6461 7461 2d66  roblem of data-f
+00005a30: 6f72 6d61 7420 6d69 6772 6174 696f 6e2e  ormat migration.
+00005a40: 2020 0a2d 2066 6965 6c64 7320 706c 6163    .- fields plac
+00005a50: 6520 6361 6e20 6265 2063 6861 6e67 6564  e can be changed
+00005a60: 0a2d 2066 6965 6c64 7320 6e61 6d65 7320  .- fields names 
+00005a70: 6361 6e20 6265 2063 6861 6e67 6564 0a0a  can be changed..
+00005a80: 5265 736f 6c76 6572 7320 6361 6e20 776f  Resolvers can wo
+00005a90: 726b 206f 6e6c 7920 7769 7468 206f 6e65  rk only with one
+00005aa0: 2065 7665 6e74 2f6d 6573 7361 6765 2e20   event/message. 
+00005ab0: 0a49 7420 6d65 616e 732c 2069 6620 796f  .It means, if yo
+00005ac0: 7572 206d 6573 7361 6765 2068 6173 2073  ur message has s
+00005ad0: 7562 2d6d 6573 7361 6765 7320 6974 2077  ub-messages it w
+00005ae0: 6f6e 2774 2077 6f72 6b2c 2062 6563 6175  on't work, becau
+00005af0: 7365 2072 6573 6f6c 7665 7220 7769 6c6c  se resolver will
+00005b00: 206e 6f74 200a 6b6e 6f77 2077 6974 6820   not .know with 
+00005b10: 7768 6963 6820 7375 622d 6d65 7373 6167  which sub-messag
+00005b20: 6520 7368 6f75 6c64 2069 7420 776f 726b  e should it work
+00005b30: 2e20 0a0a 496d 706c 656d 656e 7461 7469  . ..Implementati
+00005b40: 6f6e 2061 6476 6963 653a 0a31 2e20 7261  on advice:.1. ra
+00005b50: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+00005b60: 6564 4572 726f 7220 2d2d 2069 6620 796f  edError -- if yo
+00005b70: 7572 2049 6d70 6c65 6d65 6e74 6174 696f  ur Implementatio
+00005b80: 6e20 646f 6573 6e27 7420 7375 7070 6f72  n doesn't suppor
+00005b90: 7420 7468 6973 2067 6574 7465 722e 0a0a  t this getter...
+00005ba0: 5065 7266 6f72 6d61 6e63 6520 696d 7061  Performance impa
+00005bb0: 6374 3a0a 2d20 4974 2061 2062 6974 2073  ct:.- It a bit s
+00005bc0: 6c6f 7765 7220 7468 616e 2075 7369 6e67  lower than using
+00005bd0: 206e 616b 6564 2066 6965 6c64 2061 6363   naked field acc
+00005be0: 6573 7320 6064 6963 745b 276b 6579 275d  ess `dict['key']
+00005bf0: 602e 200a 0a23 2320 322e 342e 204c 696e  `. ..## 2.4. Lin
+00005c00: 6b73 0a0a 2d20 5b52 6570 6f72 7420 4461  ks..- [Report Da
+00005c10: 7461 2050 726f 7669 6465 725d 2868 7474  ta Provider](htt
+00005c20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00005c30: 7468 322d 6e65 742f 7468 322d 7270 742d  th2-net/th2-rpt-
+00005c40: 6461 7461 2d70 726f 7669 6465 7229 0a2d  data-provider).-
+00005c50: 205b 5468 3220 4461 7461 2053 6572 7669   [Th2 Data Servi
+00005c60: 6365 7320 5574 696c 735d 2868 7474 7073  ces Utils](https
+00005c70: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
+00005c80: 322d 6e65 742f 7468 322d 6461 7461 2d73  2-net/th2-data-s
+00005c90: 6572 7669 6365 732d 7574 696c 7329 0a0a  ervices-utils)..
+00005ca0: 2320 332e 2042 6573 7420 7072 6163 7469  # 3. Best practi
+00005cb0: 6365 730a 4465 7065 6e64 696e 6720 6f6e  ces.Depending on
+00005cc0: 2068 6f77 2079 6f75 2077 6f72 6b20 7769   how you work wi
+00005cd0: 7468 2060 4461 7461 206f 626a 6563 7460  th `Data object`
+00005ce0: 2c20 6974 2063 616e 2062 6520 736c 6f77  , it can be slow
+00005cf0: 206f 6620 6661 7374 2e20 200a 4173 2077   of fast.  .As w
+00005d00: 6974 6820 6120 7265 6c61 7469 6f6e 616c  ith a relational
+00005d10: 2064 6174 6162 6173 652c 2079 6f75 2063   database, you c
+00005d20: 616e 2077 7269 7465 2061 2071 7565 7279  an write a query
+00005d30: 2074 6861 7420 7769 6c6c 2072 6574 7572   that will retur
+00005d40: 6e20 6461 7461 2073 6c6f 776c 7920 6f72  n data slowly or
+00005d50: 2071 7569 636b 6c79 2c20 0a74 6865 2073   quickly, .the s
+00005d60: 616d 6520 7768 656e 2077 6f72 6b69 6e67  ame when working
+00005d70: 2077 6974 6820 6120 6044 6174 6120 6f62   with a `Data ob
+00005d80: 6a65 6374 602e 0a0a 466f 6c6c 6f77 2074  ject`...Follow t
+00005d90: 6865 2072 756c 6573 2074 6f20 6d61 6b65  he rules to make
+00005da0: 2079 6f75 7220 776f 726b 2077 6974 6820   your work with 
+00005db0: 4461 7461 206f 626a 6563 7420 6661 7374  Data object fast
+00005dc0: 3a0a 312e 2055 7365 2060 4461 7461 2e75  :.1. Use `Data.u
+00005dd0: 7365 5f63 6163 6865 2829 6020 6966 2079  se_cache()` if y
+00005de0: 6f75 2069 7465 7261 7465 2064 6174 6120  ou iterate data 
+00005df0: 6d6f 7265 2074 6861 6e20 6f6e 6520 7469  more than one ti
+00005e00: 6d65 2e0a 322e 2054 7279 2074 6f20 646f  me..2. Try to do
+00005e10: 6e27 7420 6974 6572 6174 6520 6f6e 6520  n't iterate one 
+00005e20: 6044 6174 6120 6f62 6a65 6374 6020 696e  `Data object` in
+00005e30: 7369 6465 2074 6865 206f 7468 6572 206f  side the other o
+00005e40: 6e65 2e20 200a 2020 2049 6620 796f 7520  ne.  .   If you 
+00005e50: 7368 6f75 6c64 2074 6f20 646f 2069 742c  should to do it,
+00005e60: 2075 7365 2073 686f 7274 2060 4461 7461   use short `Data
+00005e70: 206f 626a 6563 7460 2066 6972 7374 2061   object` first a
+00005e80: 6e64 206c 6f6e 6720 6044 6174 6120 6f62  nd long `Data ob
+00005e90: 6a65 6374 6020 696e 7369 6465 2074 6865  ject` inside the
+00005ea0: 206c 6f6f 702e 2020 0a20 2020 4974 276c   loop.  .   It'l
+00005eb0: 6c20 616c 6c6f 7720 796f 7520 6f70 656e  l allow you open
+00005ec0: 2074 6865 2063 6163 6865 2066 696c 6520   the cache file 
+00005ed0: 6f72 2063 7265 6174 6520 6120 7265 7175  or create a requ
+00005ee0: 6573 7420 746f 2060 4461 7461 2073 6f75  est to `Data sou
+00005ef0: 7263 6560 206c 6573 7320 6e75 6d62 6572  rce` less number
+00005f00: 206f 6620 7469 6d65 732e 0a0a 2320 342e   of times...# 4.
+00005f10: 204f 6666 6963 6961 6c20 4461 7461 536f   Official DataSo
+00005f20: 7572 6365 2069 6d70 6c65 6d65 6e74 6174  urce implementat
+00005f30: 696f 6e73 0a0a 2d20 5b4c 6967 6874 7765  ions..- [Lightwe
+00005f40: 6967 6874 2044 6174 6120 5072 6f76 6964  ight Data Provid
+00005f50: 6572 2044 6174 6120 536f 7572 6365 5d28  er Data Source](
+00005f60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00005f70: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d64  om/th2-net/th2-d
+00005f80: 732d 736f 7572 6365 2d6c 7764 7029 0a0a  s-source-lwdp)..
+00005f90: 0a23 2035 2e20 4150 490a 0a49 6620 796f  .# 5. API..If yo
+00005fa0: 7520 6172 6520 6c6f 6f6b 696e 6720 666f  u are looking fo
+00005fb0: 7220 636c 6173 7365 7320 6465 7363 7269  r classes descri
+00005fc0: 7074 696f 6e20 7365 6520 7468 6520 5b41  ption see the [A
+00005fd0: 5049 2044 6f63 756d 656e 7461 7469 6f6e  PI Documentation
+00005fe0: 5d28 646f 6375 6d65 6e74 6174 696f 6e2f  ](documentation/
+00005ff0: 6170 692f 696e 6465 782e 6d64 292e 0a0a  api/index.md)...
+00006000: 2320 362e 2045 7861 6d70 6c65 730a 0a2d  # 6. Examples..-
+00006010: 205b 6765 745f 7374 6172 7465 645f 6578   [get_started_ex
+00006020: 616d 706c 652e 7079 5d28 6578 616d 706c  ample.py](exampl
+00006030: 6573 2f67 6574 5f73 7461 7274 6564 5f65  es/get_started_e
+00006040: 7861 6d70 6c65 2e70 7929 0a              xample.py).
```

### Comparing `th2_data_services-2.0.0.dev5738217622/setup.py` & `th2_data_services-2.0.0.dev5738245039/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/data.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev5738245039/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev5738245039/th2_data_services.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3537 3338 3231 3736 3232 0a53 756d 6d61  5738217622.Summa
+00000040: 3537 3338 3234 3530 3339 0a53 756d 6d61  5738245039.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
@@ -89,1783 +89,1790 @@
 00000580: 6e74 5472 6565 5d28 2365 7665 6e74 7472  ntTree](#eventtr
 00000590: 6565 290a 2020 2020 2020 2020 2020 2020  ee).            
 000005a0: 2020 2020 202a 205b 436f 6c6c 6563 7469       * [Collecti
 000005b0: 6f6e 735d 2823 636f 6c6c 6563 7469 6f6e  ons](#collection
 000005c0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
 000005d0: 2020 2020 2a20 5b48 696e 7473 5d28 2368      * [Hints](#h
 000005e0: 696e 7473 290a 2020 2020 2020 2020 2020  ints).          
-000005f0: 202a 205b 322e 342e 204c 696e 6b73 5d28   * [2.4. Links](
-00000600: 2332 342d 6c69 6e6b 7329 0a20 2020 2020  #24-links).     
-00000610: 2020 202a 205b 332e 204f 6666 6963 6961     * [3. Officia
-00000620: 6c20 4461 7461 536f 7572 6365 2069 6d70  l DataSource imp
-00000630: 6c65 6d65 6e74 6174 696f 6e73 5d28 2333  lementations](#3
-00000640: 2d6f 6666 6963 6961 6c2d 6461 7461 736f  -official-dataso
-00000650: 7572 6365 2d69 6d70 6c65 6d65 6e74 6174  urce-implementat
-00000660: 696f 6e73 290a 2020 2020 2020 2020 2a20  ions).        * 
-00000670: 5b34 2e20 4150 495d 2823 342d 6170 6929  [4. API](#4-api)
-00000680: 0a20 2020 2020 2020 202a 205b 352e 2045  .        * [5. E
-00000690: 7861 6d70 6c65 735d 2823 352d 6578 616d  xamples](#5-exam
-000006a0: 706c 6573 290a 2020 2020 2020 2020 3c21  ples).        <!
-000006b0: 2d2d 7465 2d2d 3e0a 2020 2020 2020 2020  --te-->.        
-000006c0: 0a20 2020 2020 2020 2023 2031 2e20 496e  .        # 1. In
-000006d0: 7472 6f64 7563 7469 6f6e 0a20 2020 2020  troduction.     
-000006e0: 2020 200a 2020 2020 2020 2020 5468 6973     .        This
-000006f0: 2072 6570 6f73 6974 6f72 7920 6973 2061   repository is a
-00000700: 206c 6962 7261 7279 2066 6f72 2063 7265   library for cre
-00000710: 6174 696e 6720 7468 322d 6461 7461 2d73  ating th2-data-s
-00000720: 6572 7669 6365 7320 6170 706c 6963 6174  ervices applicat
-00000730: 696f 6e73 2e0a 2020 2020 2020 2020 4461  ions..        Da
-00000740: 7461 2053 6572 7669 6365 7320 616c 6c6f  ta Services allo
-00000750: 7773 2079 6f75 2074 6f20 6d61 6e69 7075  ws you to manipu
-00000760: 6c61 7465 2074 6865 2073 7472 6561 6d20  late the stream 
-00000770: 6461 7461 2070 726f 6365 7373 696e 6720  data processing 
-00000780: 776f 726b 666c 6f77 2075 7369 6e67 2070  workflow using p
-00000790: 6970 656c 696e 696e 672e 0a20 2020 2020  ipelining..     
-000007a0: 2020 200a 2020 2020 2020 2020 5468 6520     .        The 
-000007b0: 6c69 6272 6172 7927 7320 6665 6174 7572  library's featur
-000007c0: 6573 3a0a 2020 2020 2020 2020 0a20 2020  es:.        .   
-000007d0: 2020 2020 202d 2050 726f 7669 6465 7320       - Provides 
-000007e0: 636f 7265 2069 6e74 6572 6661 6365 2066  core interface f
-000007f0: 6f72 2064 6576 656c 6f70 696e 6720 6461  or developing da
-00000800: 7461 2073 6f75 7263 6520 696d 706c 656d  ta source implem
-00000810: 656e 7461 7469 6f6e 730a 2020 2020 2020  entations.      
-00000820: 2020 2d20 576f 726b 2077 6974 6820 6974    - Work with it
-00000830: 6572 6162 6c65 206f 626a 6563 7473 2028  erable objects (
-00000840: 6c69 7374 2c20 7475 706c 652c 2065 7463  list, tuple, etc
-00000850: 2069 6e63 6c75 6469 6e67 2066 696c 6573   including files
-00000860: 2920 7669 6120 5f44 6174 6120 6f62 6a65  ) via _Data obje
-00000870: 6374 5f20 7573 696e 6720 6974 7320 6665  ct_ using its fe
-00000880: 6174 7572 6573 0a20 2020 2020 2020 202d  atures.        -
-00000890: 204d 616e 6970 756c 6174 6520 7468 6520   Manipulate the 
-000008a0: 776f 726b 666c 6f77 2074 6f20 6d61 6b65  workflow to make
-000008b0: 2073 6f6d 6520 616e 616c 7973 6973 2062   some analysis b
-000008c0: 7920 5f44 6174 6120 6f62 6a65 6374 5f20  y _Data object_ 
-000008d0: 6d65 7468 6f64 730a 2020 2020 2020 2020  methods.        
-000008e0: 2d20 5573 6520 7469 6d65 7374 616d 7020  - Use timestamp 
-000008f0: 636f 6e76 6572 7465 7220 696d 706c 656d  converter implem
-00000900: 656e 7461 7469 6f6e 7320 6f72 2075 7365  entations or use
-00000910: 2062 6173 6520 636c 6173 7320 746f 2063   base class to c
-00000920: 7265 6174 6520 6375 7374 6f6d 2063 6f6e  reate custom con
-00000930: 7665 7274 6572 730a 2020 2020 2020 2020  verters.        
-00000940: 2d20 4275 696c 6420 4576 656e 7420 5472  - Build Event Tr
-00000950: 6565 7320 2845 7665 6e74 5472 6565 2c20  ees (EventTree, 
-00000960: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
-00000970: 696f 6e20 616e 6420 5061 7265 6e74 4576  ion and ParentEv
-00000980: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00000990: 6e20 636c 6173 7365 7329 0a20 2020 2020  n classes).     
-000009a0: 2020 200a 2020 2020 2020 2020 576f 726b     .        Work
-000009b0: 666c 6f77 206d 616e 6970 756c 6174 696f  flow manipulatio
-000009c0: 6e20 746f 6f6c 7320 616c 6c6f 7773 2079  n tools allows y
-000009d0: 6f75 3a0a 2020 2020 2020 2020 0a20 2020  ou:.        .   
-000009e0: 2020 2020 202d 2046 696c 7465 7269 6e67       - Filtering
-000009f0: 2073 7472 6561 6d20 6461 7461 2028 6044   stream data (`D
-00000a00: 6174 612e 6669 6c74 6572 6020 6d65 7468  ata.filter` meth
-00000a10: 6f64 290a 2020 2020 2020 2020 2d20 5472  od).        - Tr
-00000a20: 616e 7366 6f72 6d69 6e67 2073 7472 6561  ansforming strea
-00000a30: 6d20 6461 7461 2028 6044 6174 612e 6d61  m data (`Data.ma
-00000a40: 7060 206d 6574 686f 6429 0a20 2020 2020  p` method).     
-00000a50: 2020 202d 204c 696d 6974 696e 6720 7468     - Limiting th
-00000a60: 6520 6e75 6d62 6572 206f 6620 7072 6f63  e number of proc
-00000a70: 6573 7365 6420 7374 7265 616d 696e 6720  essed streaming 
-00000a80: 6461 7461 2028 6044 6174 612e 6c69 6d69  data (`Data.limi
-00000a90: 7460 206d 6574 686f 6429 0a20 2020 2020  t` method).     
-00000aa0: 2020 200a 2020 2020 2020 2020 5468 6572     .        Ther
-00000ab0: 6520 6973 2061 6c73 6f20 616e 6f74 6865  e is also anothe
-00000ac0: 7220 7061 7274 206f 6620 5f64 6174 6120  r part of _data 
-00000ad0: 7365 7276 6963 6573 5f0a 2020 2020 2020  services_.      
-00000ae0: 2020 0a20 2020 2020 2020 202d 205b 7468    .        - [th
-00000af0: 322d 6461 7461 2d73 6572 7669 6365 732d  2-data-services-
-00000b00: 7574 696c 735d 2868 7474 7073 3a2f 2f67  utils](https://g
-00000b10: 6974 6875 622e 636f 6d2f 7468 322d 6e65  ithub.com/th2-ne
-00000b20: 742f 7468 322d 6461 7461 2d73 6572 7669  t/th2-data-servi
-00000b30: 6365 732d 7574 696c 7329 2e20 4974 2773  ces-utils). It's
-00000b40: 2061 2073 6574 206f 6620 746f 6f6c 7320   a set of tools 
-00000b50: 746f 2070 6572 666f 726d 2074 6865 206d  to perform the m
-00000b60: 6f73 740a 2020 2020 2020 2020 2020 636f  ost.          co
-00000b70: 6d6d 6f6e 2061 6e61 6c79 7369 7320 7461  mmon analysis ta
-00000b80: 736b 732e 0a20 2020 2020 2020 200a 2020  sks..        .  
-00000b90: 2020 2020 2020 2320 322e 2047 6574 7469        # 2. Getti
-00000ba0: 6e67 2073 7461 7274 6564 0a20 2020 2020  ng started.     
-00000bb0: 2020 200a 2020 2020 2020 2020 2323 2032     .        ## 2
-00000bc0: 2e31 2e20 496e 7374 616c 6c61 7469 6f6e  .1. Installation
-00000bd0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000be0: 2020 2323 2320 436f 7265 0a20 2020 2020    ### Core.     
-00000bf0: 2020 200a 2020 2020 2020 2020 2d20 4672     .        - Fr
-00000c00: 6f6d 2050 7950 4920 2870 6970 2920 2020  om PyPI (pip)   
-00000c10: 0a20 2020 2020 2020 2020 2054 6869 7320  .          This 
-00000c20: 7061 636b 6167 6520 6361 6e20 6265 2066  package can be f
-00000c30: 6f75 6e64 206f 6e20 5b50 7950 495d 2868  ound on [PyPI](h
-00000c40: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000c50: 7072 6f6a 6563 742f 7468 322d 6461 7461  project/th2-data
-00000c60: 2d73 6572 7669 6365 732f 2022 7468 322d  -services/ "th2-
-00000c70: 6461 7461 2d73 6572 7669 6365 7322 292e  data-services").
-00000c80: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
-00000c90: 0a20 2020 2020 2020 2020 2020 2070 6970  .            pip
-00000ca0: 2069 6e73 7461 6c6c 2074 6832 2d64 6174   install th2-dat
-00000cb0: 612d 7365 7276 6963 6573 0a20 2020 2020  a-services.     
-00000cc0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00000cd0: 2020 200a 2020 2020 2020 2020 2d20 4672     .        - Fr
-00000ce0: 6f6d 2053 6f75 7263 650a 2020 2020 2020  om Source.      
-00000cf0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00000d00: 2020 2020 2020 6769 7420 636c 6f6e 6520        git clone 
-00000d10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000d20: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d64  om/th2-net/th2-d
-00000d30: 6174 612d 7365 7276 6963 6573 0a20 2020  ata-services.   
-00000d40: 2020 2020 2020 2020 2070 6970 2069 6e73           pip ins
-00000d50: 7461 6c6c 2074 6832 2d64 6174 612d 7365  tall th2-data-se
-00000d60: 7276 6963 6573 2f0a 2020 2020 2020 2020  rvices/.        
-00000d70: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00000d80: 0a20 2020 2020 2020 2023 2323 2044 6174  .        ### Dat
-00000d90: 6120 736f 7572 6365 7320 2870 726f 7669  a sources (provi
-00000da0: 6465 7273 290a 2020 2020 2020 2020 0a20  ders).        . 
-00000db0: 2020 2020 2020 2053 696e 6365 2060 7631         Since `v1
-00000dc0: 2e33 2e30 602c 2074 6865 206c 6962 7261  .3.0`, the libra
-00000dd0: 7279 2064 6f65 736e 2774 2070 726f 7669  ry doesn't provi
-00000de0: 6465 2064 6174 6120 736f 7572 6365 2064  de data source d
-00000df0: 6570 656e 6465 6e63 6965 732e 0a20 2020  ependencies..   
-00000e00: 2020 2020 200a 2020 2020 2020 2020 596f       .        Yo
-00000e10: 7520 7368 6f75 6c64 2070 726f 7669 6465  u should provide
-00000e20: 2069 7420 6d61 6e75 616c 6c79 2064 7572   it manually dur
-00000e30: 696e 6720 696e 7374 616c 6c61 7469 6f6e  ing installation
-00000e40: 2e20 0a20 2020 2020 2020 2059 6f75 206a  . .        You j
-00000e50: 7573 7420 6e65 6564 2074 6f20 6164 6420  ust need to add 
-00000e60: 7371 7561 7265 2062 7261 636b 6574 7320  square brackets 
-00000e70: 6166 7465 7220 6c69 6272 6172 7920 6e61  after library na
-00000e80: 6d65 2061 6e64 2070 7574 2064 6570 656e  me and put depen
-00000e90: 6465 6e63 7920 6e61 6d65 2e0a 2020 2020  dency name..    
-00000ea0: 2020 2020 0a20 2020 2020 2020 2060 6060      .        ```
-00000eb0: 0a20 2020 2020 2020 2070 6970 2069 6e73  .        pip ins
-00000ec0: 7461 6c6c 2074 6832 2d64 6174 612d 7365  tall th2-data-se
-00000ed0: 7276 6963 6573 5b64 6570 656e 6465 6e63  rvices[dependenc
-00000ee0: 795f 6e61 6d65 5d0a 2020 2020 2020 2020  y_name].        
-00000ef0: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
-00000f00: 2020 2020 202a 2a44 6570 656e 6465 6e63       **Dependenc
-00000f10: 6965 7320 6c69 7374 2a2a 200a 2020 2020  ies list** .    
-00000f20: 2020 2020 0a20 2020 2020 2020 207c 2020      .        |  
-00000f30: 6465 7065 6e64 656e 6379 206e 616d 6520  dependency name 
-00000f40: 207c 2070 726f 7669 6465 7220 7665 7273   | provider vers
-00000f50: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
-00000f60: 2020 2020 2020 2020 207c 0a20 2020 2020           |.     
-00000f70: 2020 207c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d     |:-----------
-00000f80: 2d2d 2d2d 2d2d 3a7c 2d2d 2d2d 2d2d 2d2d  ------:|--------
-00000f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-00000fb0: 0a20 2020 2020 2020 207c 2020 2020 2020  .        |      
-00000fc0: 206c 7764 7020 2020 2020 2020 207c 206c   lwdp        | l
-00000fd0: 6174 6573 7420 7665 7273 696f 6e20 6f66  atest version of
-00000fe0: 206c 7764 7020 2020 2020 2020 2020 2020   lwdp           
-00000ff0: 2020 2020 207c 0a20 2020 2020 2020 207c       |.        |
-00001000: 2020 2020 2020 206c 7764 7032 2020 2020         lwdp2    
-00001010: 2020 207c 206c 6174 6573 7420 7665 7273     | latest vers
-00001020: 696f 6e20 6f66 206c 7764 7020 7632 2020  ion of lwdp v2  
-00001030: 2020 2020 2020 2020 2020 207c 0a20 2020             |.   
-00001040: 2020 2020 207c 2075 7469 6c73 2d72 7074       | utils-rpt
-00001050: 2d76 6965 7765 7220 207c 206c 6174 6573  -viewer  | lates
-00001060: 7420 7665 7273 696f 6e20 6f66 2075 7469  t version of uti
-00001070: 6c73 2d72 7074 2d76 6965 7765 7220 2020  ls-rpt-viewer   
-00001080: 207c 0a20 2020 2020 2020 207c 2075 7469   |.        | uti
-00001090: 6c73 2d72 7074 2d76 6965 7765 7235 207c  ls-rpt-viewer5 |
-000010a0: 206c 6174 6573 7420 7665 7273 696f 6e20   latest version 
-000010b0: 6f66 2075 7469 6c73 2d72 7074 2d76 6965  of utils-rpt-vie
-000010c0: 7765 7220 7635 207c 0a20 2020 2020 2020  wer v5 |.       
-000010d0: 207c 2020 2075 7469 6c73 2d61 6476 616e   |   utils-advan
-000010e0: 6365 6420 207c 206c 6174 6573 7420 7665  ced  | latest ve
-000010f0: 7273 696f 6e20 6f66 2064 732d 7574 696c  rsion of ds-util
-00001100: 7320 2020 2020 2020 2020 2020 207c 0a20  s            |. 
-00001110: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001120: 2a2a 4578 616d 706c 652a 2a0a 2020 2020  **Example**.    
-00001130: 2020 2020 0a20 2020 2020 2020 2060 6060      .        ```
-00001140: 0a20 2020 2020 2020 2070 6970 2069 6e73  .        pip ins
-00001150: 7461 6c6c 2074 6832 2d64 6174 612d 7365  tall th2-data-se
-00001160: 7276 6963 6573 5b6c 7764 7031 5d0a 2020  rvices[lwdp1].  
-00001170: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00001180: 2020 0a20 2020 2020 2020 2023 2320 322e    .        ## 2.
-00001190: 322e 2045 7861 6d70 6c65 0a20 2020 2020  2. Example.     
-000011a0: 2020 200a 2020 2020 2020 2020 4120 676f     .        A go
-000011b0: 6f64 2c20 7368 6f72 7420 6578 616d 706c  od, short exampl
-000011c0: 6520 6973 2077 6f72 7468 2061 2074 686f  e is worth a tho
-000011d0: 7573 616e 6420 776f 7264 732e 0a20 2020  usand words..   
-000011e0: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
-000011f0: 6973 2065 7861 6d70 6c65 2073 686f 7773  is example shows
-00001200: 2062 6173 6963 2075 7361 6765 206f 6620   basic usage of 
-00001210: 6c69 6272 6172 7927 7320 6665 6174 7572  library's featur
-00001220: 6573 2e0a 2020 2020 2020 2020 0a20 2020  es..        .   
-00001230: 2020 2020 205b 5468 6520 666f 6c6c 6f77       [The follow
-00001240: 696e 6720 6578 616d 706c 6520 6173 2061  ing example as a
-00001250: 2066 696c 655d 2865 7861 6d70 6c65 732f   file](examples/
-00001260: 6765 745f 7374 6172 7465 645f 6578 616d  get_started_exam
-00001270: 706c 652e 7079 292e 0a20 2020 2020 2020  ple.py)..       
-00001280: 200a 2020 2020 2020 2020 3c21 2d2d 2073   .        <!-- s
-00001290: 7461 7274 2067 6574 5f73 7461 7274 6564  tart get_started
-000012a0: 5f65 7861 6d70 6c65 2e70 7920 2d2d 3e0a  _example.py -->.
-000012b0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-000012c0: 6e0a 2020 2020 2020 2020 6672 6f6d 2074  n.        from t
-000012d0: 7970 696e 6720 696d 706f 7274 2054 7570  yping import Tup
-000012e0: 6c65 2c20 4c69 7374 2c20 4f70 7469 6f6e  le, List, Option
-000012f0: 616c 2c20 4765 6e65 7261 746f 720a 2020  al, Generator.  
-00001300: 2020 2020 2020 6672 6f6d 2064 6174 6574        from datet
-00001310: 696d 6520 696d 706f 7274 2064 6174 6574  ime import datet
-00001320: 696d 650a 2020 2020 2020 2020 0a20 2020  ime.        .   
-00001330: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
-00001340: 7461 5f73 6572 7669 6365 732e 6461 7461  ta_services.data
-00001350: 2069 6d70 6f72 7420 4461 7461 0a20 2020   import Data.   
-00001360: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
-00001370: 7461 5f73 6572 7669 6365 732e 6576 656e  ta_services.even
-00001380: 745f 7472 6565 2069 6d70 6f72 7420 4576  t_tree import Ev
-00001390: 656e 7454 7265 652c 2045 7665 6e74 5472  entTree, EventTr
-000013a0: 6565 436f 6c6c 6563 7469 6f6e 2c20 5061  eeCollection, Pa
-000013b0: 7265 6e74 4576 656e 7454 7265 6543 6f6c  rentEventTreeCol
-000013c0: 6c65 6374 696f 6e2c 2049 4554 4344 7269  lection, IETCDri
-000013d0: 7665 720a 2020 2020 2020 2020 6672 6f6d  ver.        from
-000013e0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
-000013f0: 6573 2e69 6e74 6572 6661 6365 7320 696d  es.interfaces im
-00001400: 706f 7274 2049 4461 7461 536f 7572 6365  port IDataSource
-00001410: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
-00001420: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00001430: 7574 696c 732e 636f 6e76 6572 7465 7273  utils.converters
-00001440: 2069 6d70 6f72 7420 4461 7465 7469 6d65   import Datetime
-00001450: 436f 6e76 6572 7465 722c 2044 6174 6574  Converter, Datet
-00001460: 696d 6553 7472 696e 6743 6f6e 7665 7274  imeStringConvert
-00001470: 6572 2c20 5072 6f74 6f62 7566 5469 6d65  er, ProtobufTime
-00001480: 7374 616d 7043 6f6e 7665 7274 6572 0a20  stampConverter. 
-00001490: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000014a0: 2320 5b30 5d20 4c69 6220 636f 6e66 6967  # [0] Lib config
-000014b0: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
-000014c0: 2320 5b30 2e31 5d20 496e 7465 7261 6374  # [0.1] Interact
-000014d0: 6976 6520 6f72 2053 6372 6970 7420 6d6f  ive or Script mo
-000014e0: 6465 0a20 2020 2020 2020 2023 2049 6620  de.        # If 
-000014f0: 796f 7520 7573 6520 7468 6520 6c69 6220  you use the lib 
-00001500: 696e 2069 6e74 6572 6163 7469 7665 206d  in interactive m
-00001510: 6f64 6520 286a 7570 7974 6572 2c20 6970  ode (jupyter, ip
-00001520: 7974 686f 6e29 2069 7427 7320 7265 636f  ython) it's reco
-00001530: 6d6d 656e 6465 6420 746f 2073 6574 2074  mmended to set t
-00001540: 6865 2073 7065 6369 616c 0a20 2020 2020  he special.     
-00001550: 2020 2023 2067 6c6f 6261 6c20 7061 7261     # global para
-00001560: 6d65 7465 7220 746f 2054 7275 652e 2049  meter to True. I
-00001570: 7427 6c6c 206b 6565 7020 6361 6368 6520  t'll keep cache 
-00001580: 6669 6c65 7320 6966 2073 6f6d 6574 6869  files if somethi
-00001590: 6e67 2077 656e 7420 7772 6f6e 672e 0a20  ng went wrong.. 
-000015a0: 2020 2020 2020 2066 726f 6d20 7468 325f         from th2_
-000015b0: 6461 7461 5f73 6572 7669 6365 732e 636f  data_services.co
-000015c0: 6e66 6967 2069 6d70 6f72 7420 6f70 7469  nfig import opti
-000015d0: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
-000015e0: 2020 2020 206f 7074 696f 6e73 2e49 4e54       options.INT
-000015f0: 4552 4143 5449 5645 5f4d 4f44 4520 3d20  ERACTIVE_MODE = 
-00001600: 5472 7565 0a20 2020 2020 2020 200a 2020  True.        .  
-00001610: 2020 2020 2020 2320 536f 6d65 2065 7861        # Some exa
-00001620: 6d70 6c65 2064 6174 610a 2020 2020 2020  mple data.      
-00001630: 2020 6576 656e 7473 203d 2044 6174 6128    events = Data(
-00001640: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
-00001650: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00001660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001670: 2020 2020 2022 6576 656e 7449 6422 3a20       "eventId": 
-00001680: 2264 656d 6f5f 626f 6f6b 5f31 3a74 6832  "demo_book_1:th2
-00001690: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
-000016a0: 3335 3730 3535 3630 3837 3330 3030 3a64  35705560873000:d
-000016b0: 3631 6539 3330 612d 3864 3030 2d31 3165  61e930a-8d00-11e
-000016c0: 642d 6161 3161 2d64 3334 6136 3135 3531  d-aa1a-d34a61551
-000016d0: 3532 645f 3122 2c0a 2020 2020 2020 2020  52d_1",.        
-000016e0: 2020 2020 2020 2020 2020 2020 2262 6174              "bat
-000016f0: 6368 4964 223a 204e 6f6e 652c 0a20 2020  chId": None,.   
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2022 6973 4261 7463 6865 6422 3a20 4661   "isBatched": Fa
-00001720: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-00001730: 2020 2020 2020 2020 2022 6576 656e 744e           "eventN
-00001740: 616d 6522 3a20 2253 6574 206f 6620 6175  ame": "Set of au
-00001750: 746f 2d67 656e 6572 6174 6564 2065 7665  to-generated eve
-00001760: 6e74 7320 666f 7220 6473 206c 6962 2074  nts for ds lib t
-00001770: 6573 7469 6e67 222c 0a20 2020 2020 2020  esting",.       
-00001780: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
-00001790: 656e 7454 7970 6522 3a20 2264 732d 6c69  entType": "ds-li
-000017a0: 622d 7465 7374 2d65 7665 6e74 222c 0a20  b-test-event",. 
-000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017c0: 2020 2022 656e 6454 696d 6573 7461 6d70     "endTimestamp
-000017d0: 223a 207b 2265 706f 6368 5365 636f 6e64  ": {"epochSecond
-000017e0: 223a 2031 3637 3239 3237 3032 352c 2022  ": 1672927025, "
-000017f0: 6e61 6e6f 223a 2035 3631 3735 3130 3030  nano": 561751000
-00001800: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00001810: 2020 2020 2020 2022 7374 6172 7454 696d         "startTim
-00001820: 6573 7461 6d70 223a 207b 2265 706f 6368  estamp": {"epoch
-00001830: 5365 636f 6e64 223a 2031 3637 3239 3237  Second": 1672927
-00001840: 3032 352c 2022 6e61 6e6f 223a 2035 3630  025, "nano": 560
-00001850: 3837 3330 3030 7d2c 0a20 2020 2020 2020  873000},.       
-00001860: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
-00001870: 7265 6e74 4576 656e 7449 6422 3a20 4e6f  rentEventId": No
-00001880: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00001890: 2020 2020 2020 2020 2273 7563 6365 7373          "success
-000018a0: 6675 6c22 3a20 5472 7565 2c0a 2020 2020  ful": True,.    
-000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018c0: 2262 6f6f 6b49 6422 3a20 2264 656d 6f5f  "bookId": "demo_
-000018d0: 626f 6f6b 5f31 222c 0a20 2020 2020 2020  book_1",.       
-000018e0: 2020 2020 2020 2020 2020 2020 2022 7363               "sc
-000018f0: 6f70 6522 3a20 2274 6832 2d73 636f 7065  ope": "th2-scope
-00001900: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001910: 2020 2020 2020 2022 6174 7461 6368 6564         "attached
-00001920: 4d65 7373 6167 6549 6473 223a 205b 5d2c  MessageIds": [],
-00001930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001940: 2020 2020 2022 626f 6479 223a 205b 5d2c       "body": [],
-00001950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001960: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00001970: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00001980: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00001990: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
-000019a0: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
-000019b0: 3031 3035 3133 3537 3035 3536 3335 3232  0105135705563522
-000019c0: 3030 303a 3961 6462 6233 6530 2d35 6638  000:9adbb3e0-5f8
-000019d0: 622d 3463 3238 2d61 3261 632d 3733 3631  b-4c28-a2ac-7361
-000019e0: 6538 6661 3730 3463 3e64 656d 6f5f 626f  e8fa704c>demo_bo
-000019f0: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
-00001a00: 3032 3330 3130 3531 3335 3730 3535 3633  0230105135705563
-00001a10: 3532 3230 3030 3a64 3631 6539 3330 612d  522000:d61e930a-
-00001a20: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
-00001a30: 3334 6136 3135 3531 3532 645f 3222 2c0a  34a6155152d_2",.
-00001a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a50: 2020 2020 2262 6174 6368 4964 223a 2022      "batchId": "
-00001a60: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
-00001a70: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
-00001a80: 3537 3035 3536 3335 3232 3030 303a 3961  5705563522000:9a
-00001a90: 6462 6233 6530 2d35 6638 622d 3463 3238  dbb3e0-5f8b-4c28
-00001aa0: 2d61 3261 632d 3733 3631 6538 6661 3730  -a2ac-7361e8fa70
-00001ab0: 3463 222c 0a20 2020 2020 2020 2020 2020  4c",.           
-00001ac0: 2020 2020 2020 2020 2022 6973 4261 7463           "isBatc
-00001ad0: 6865 6422 3a20 5472 7565 2c0a 2020 2020  hed": True,.    
-00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001af0: 2265 7665 6e74 4e61 6d65 223a 2022 506c  "eventName": "Pl
-00001b00: 6169 6e20 6576 656e 7420 3122 2c0a 2020  ain event 1",.  
-00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b20: 2020 2265 7665 6e74 5479 7065 223a 2022    "eventType": "
-00001b30: 6473 2d6c 6962 2d74 6573 742d 6576 656e  ds-lib-test-even
-00001b40: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00001b50: 2020 2020 2020 2020 2265 6e64 5469 6d65          "endTime
-00001b60: 7374 616d 7022 3a20 7b22 6570 6f63 6853  stamp": {"epochS
-00001b70: 6563 6f6e 6422 3a20 3136 3732 3932 3730  econd": 16729270
-00001b80: 3235 2c20 226e 616e 6f22 3a20 3536 3336  25, "nano": 5636
-00001b90: 3430 3030 307d 2c0a 2020 2020 2020 2020  40000},.        
-00001ba0: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-00001bb0: 7274 5469 6d65 7374 616d 7022 3a20 7b22  rtTimestamp": {"
-00001bc0: 6570 6f63 6853 6563 6f6e 6422 3a20 3136  epochSecond": 16
-00001bd0: 3732 3932 3730 3235 2c20 226e 616e 6f22  72927025, "nano"
-00001be0: 3a20 3536 3335 3232 3030 307d 2c0a 2020  : 563522000},.  
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c00: 2020 2270 6172 656e 7445 7665 6e74 4964    "parentEventId
-00001c10: 223a 2022 6465 6d6f 5f62 6f6f 6b5f 313a  ": "demo_book_1:
-00001c20: 7468 322d 7363 6f70 653a 3230 3233 3031  th2-scope:202301
-00001c30: 3035 3133 3537 3035 3536 3038 3733 3030  0513570556087300
-00001c40: 303a 6436 3165 3933 3061 2d38 6430 302d  0:d61e930a-8d00-
-00001c50: 3131 6564 2d61 6131 612d 6433 3461 3631  11ed-aa1a-d34a61
-00001c60: 3535 3135 3264 5f31 222c 0a20 2020 2020  55152d_1",.     
-00001c70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001c80: 7375 6363 6573 7366 756c 223a 2054 7275  successful": Tru
-00001c90: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001ca0: 2020 2020 2020 2022 626f 6f6b 4964 223a         "bookId":
-00001cb0: 2022 6465 6d6f 5f62 6f6f 6b5f 3122 2c0a   "demo_book_1",.
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cd0: 2020 2020 2273 636f 7065 223a 2022 7468      "scope": "th
-00001ce0: 322d 7363 6f70 6522 2c0a 2020 2020 2020  2-scope",.      
-00001cf0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00001d00: 7474 6163 6865 644d 6573 7361 6765 4964  ttachedMessageId
-00001d10: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
-00001d20: 2020 2020 2020 2020 2020 2020 2262 6f64              "bod
-00001d30: 7922 3a20 7b22 7479 7065 223a 2022 6d65  y": {"type": "me
-00001d40: 7373 6167 6522 2c20 2264 6174 6122 3a20  ssage", "data": 
-00001d50: 2264 732d 6c69 6220 7465 7374 2062 6f64  "ds-lib test bod
-00001d60: 7922 7d2c 0a20 2020 2020 2020 2020 2020  y"},.           
-00001d70: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00001d80: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00001da0: 7665 6e74 4964 223a 2022 6465 6d6f 5f62  ventId": "demo_b
-00001db0: 6f6f 6b5f 313a 7468 322d 7363 6f70 653a  ook_1:th2-scope:
-00001dc0: 3230 3233 3031 3035 3133 3537 3035 3536  2023010513570556
-00001dd0: 3335 3232 3030 303a 3961 6462 6233 6530  3522000:9adbb3e0
-00001de0: 2d35 6638 622d 3463 3238 2d61 3261 632d  -5f8b-4c28-a2ac-
-00001df0: 3733 3631 6538 6661 3730 3463 3e64 656d  7361e8fa704c>dem
-00001e00: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
-00001e10: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
-00001e20: 3535 3633 3735 3730 3030 3a64 3631 6539  5563757000:d61e9
-00001e30: 3330 612d 3864 3030 2d31 3165 642d 6161  30a-8d00-11ed-aa
-00001e40: 3161 2d64 3334 6136 3135 3531 3532 645f  1a-d34a6155152d_
-00001e50: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
-00001e60: 2020 2020 2020 2020 2262 6174 6368 4964          "batchId
-00001e70: 223a 2022 6465 6d6f 5f62 6f6f 6b5f 313a  ": "demo_book_1:
-00001e80: 7468 322d 7363 6f70 653a 3230 3233 3031  th2-scope:202301
-00001e90: 3035 3133 3537 3035 3536 3335 3232 3030  0513570556352200
-00001ea0: 303a 3961 6462 6233 6530 2d35 6638 622d  0:9adbb3e0-5f8b-
-00001eb0: 3463 3238 2d61 3261 632d 3733 3631 6538  4c28-a2ac-7361e8
-00001ec0: 6661 3730 3463 222c 0a20 2020 2020 2020  fa704c",.       
-00001ed0: 2020 2020 2020 2020 2020 2020 2022 6973               "is
-00001ee0: 4261 7463 6865 6422 3a20 5472 7565 2c0a  Batched": True,.
-00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f00: 2020 2020 2265 7665 6e74 4e61 6d65 223a      "eventName":
-00001f10: 2022 506c 6169 6e20 6576 656e 7420 3222   "Plain event 2"
-00001f20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001f30: 2020 2020 2020 2265 7665 6e74 5479 7065        "eventType
-00001f40: 223a 2022 6473 2d6c 6962 2d74 6573 742d  ": "ds-lib-test-
-00001f50: 6576 656e 7422 2c0a 2020 2020 2020 2020  event",.        
-00001f60: 2020 2020 2020 2020 2020 2020 2265 6e64              "end
-00001f70: 5469 6d65 7374 616d 7022 3a20 7b22 6570  Timestamp": {"ep
-00001f80: 6f63 6853 6563 6f6e 6422 3a20 3136 3732  ochSecond": 1672
-00001f90: 3932 3730 3235 2c20 226e 616e 6f22 3a20  927025, "nano": 
-00001fa0: 3536 3337 3931 3030 307d 2c0a 2020 2020  563791000},.    
-00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fc0: 2273 7461 7274 5469 6d65 7374 616d 7022  "startTimestamp"
-00001fd0: 3a20 7b22 6570 6f63 6853 6563 6f6e 6422  : {"epochSecond"
-00001fe0: 3a20 3136 3732 3932 3730 3235 2c20 226e  : 1672927025, "n
-00001ff0: 616e 6f22 3a20 3536 3337 3537 3030 307d  ano": 563757000}
-00002000: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002010: 2020 2020 2020 2270 6172 656e 7445 7665        "parentEve
-00002020: 6e74 4964 223a 2022 6465 6d6f 5f62 6f6f  ntId": "demo_boo
-00002030: 6b5f 313a 7468 322d 7363 6f70 653a 3230  k_1:th2-scope:20
-00002040: 3233 3031 3035 3133 3537 3035 3536 3038  2301051357055608
-00002050: 3733 3030 303a 6436 3165 3933 3061 2d38  73000:d61e930a-8
-00002060: 6430 302d 3131 6564 2d61 6131 612d 6433  d00-11ed-aa1a-d3
-00002070: 3461 3631 3535 3135 3264 5f31 222c 0a20  4a6155152d_1",. 
-00002080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002090: 2020 2022 7375 6363 6573 7366 756c 223a     "successful":
-000020a0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-000020b0: 2020 2020 2020 2020 2020 2022 626f 6f6b             "book
-000020c0: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
-000020d0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-000020e0: 2020 2020 2020 2020 2273 636f 7065 223a          "scope":
-000020f0: 2022 7468 322d 7363 6f70 6522 2c0a 2020   "th2-scope",.  
-00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002110: 2020 2261 7474 6163 6865 644d 6573 7361    "attachedMessa
-00002120: 6765 4964 7322 3a20 5b5d 2c0a 2020 2020  geIds": [],.    
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2262 6f64 7922 3a20 7b22 7479 7065 223a  "body": {"type":
-00002150: 2022 6d65 7373 6167 6522 2c20 2264 6174   "message", "dat
-00002160: 6122 3a20 2264 732d 6c69 6220 7465 7374  a": "ds-lib test
-00002170: 2062 6f64 7922 7d2c 0a20 2020 2020 2020   body"},.       
-00002180: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00002190: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-000021a0: 2020 290a 2020 2020 2020 2020 0a20 2020    ).        .   
-000021b0: 2020 2020 2023 205b 315d 2057 6f72 6b69       # [1] Worki
-000021c0: 6e67 2077 6974 6820 6120 4461 7461 206f  ng with a Data o
-000021d0: 626a 6563 742e 0a20 2020 2020 2020 2023  bject..        #
-000021e0: 205b 312e 315d 2046 696c 7465 722e 0a20   [1.1] Filter.. 
-000021f0: 2020 2020 2020 2066 696c 7465 7265 645f         filtered_
-00002200: 6576 656e 7473 3a20 4461 7461 203d 2065  events: Data = e
-00002210: 7665 6e74 732e 6669 6c74 6572 286c 616d  vents.filter(lam
-00002220: 6264 6120 653a 2065 5b22 626f 6479 225d  bda e: e["body"]
-00002230: 2021 3d20 5b5d 2920 2023 2046 696c 7465   != [])  # Filte
-00002240: 7220 6576 656e 7473 2077 6974 6820 656d  r events with em
-00002250: 7074 7920 626f 6479 2e0a 2020 2020 2020  pty body..      
-00002260: 2020 0a20 2020 2020 2020 200a 2020 2020    .        .    
-00002270: 2020 2020 2320 5b31 2e32 5d20 4d61 702e      # [1.2] Map.
-00002280: 0a20 2020 2020 2020 2064 6566 2074 7261  .        def tra
-00002290: 6e73 666f 726d 5f66 756e 6374 696f 6e28  nsform_function(
-000022a0: 7265 636f 7264 293a 0a20 2020 2020 2020  record):.       
-000022b0: 2020 2020 2072 6574 7572 6e20 7b22 6576       return {"ev
-000022c0: 656e 744e 616d 6522 3a20 7265 636f 7264  entName": record
-000022d0: 5b22 6576 656e 744e 616d 6522 5d2c 2022  ["eventName"], "
-000022e0: 7375 6363 6573 7366 756c 223a 2072 6563  successful": rec
-000022f0: 6f72 645b 2273 7563 6365 7373 6675 6c22  ord["successful"
-00002300: 5d7d 0a20 2020 2020 2020 200a 2020 2020  ]}.        .    
-00002310: 2020 2020 0a20 2020 2020 2020 2066 696c      .        fil
-00002320: 7465 7265 645f 616e 645f 6d61 7070 6564  tered_and_mapped
-00002330: 5f65 7665 6e74 7320 3d20 6669 6c74 6572  _events = filter
-00002340: 6564 5f65 7665 6e74 732e 6d61 7028 7472  ed_events.map(tr
-00002350: 616e 7366 6f72 6d5f 6675 6e63 7469 6f6e  ansform_function
-00002360: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00002370: 2020 2023 205b 312e 335d 2044 6174 6120     # [1.3] Data 
-00002380: 7069 7065 6c69 6e65 2e0a 2020 2020 2020  pipeline..      
-00002390: 2020 2320 2020 2020 2020 496e 7374 6561    #       Instea
-000023a0: 6420 6f66 2064 6f69 6e67 2064 6174 6120  d of doing data 
-000023b0: 7472 616e 7366 6f72 6d61 7469 6f6e 7320  transformations 
-000023c0: 7374 6570 2062 7920 7374 6570 2079 6f75  step by step you
-000023d0: 2063 616e 2064 6f20 6974 2069 6e20 6f6e   can do it in on
-000023e0: 6520 6c69 6e65 2e0a 2020 2020 2020 2020  e line..        
-000023f0: 6669 6c74 6572 6564 5f61 6e64 5f6d 6170  filtered_and_map
-00002400: 7065 645f 6576 656e 7473 5f62 795f 7069  ped_events_by_pi
-00002410: 7065 6c69 6e65 203d 2065 7665 6e74 732e  peline = events.
-00002420: 6669 6c74 6572 286c 616d 6264 6120 653a  filter(lambda e:
-00002430: 2065 5b22 626f 6479 225d 2021 3d20 5b5d   e["body"] != []
-00002440: 292e 6d61 7028 7472 616e 7366 6f72 6d5f  ).map(transform_
-00002450: 6675 6e63 7469 6f6e 290a 2020 2020 2020  function).      
-00002460: 2020 2320 436f 6e74 656e 7420 6f66 2074    # Content of t
-00002470: 6865 7365 2074 776f 2044 6174 6120 6f62  hese two Data ob
-00002480: 6a65 6374 7320 7368 6f75 6c64 2062 6520  jects should be 
-00002490: 6571 7561 6c2e 0a20 2020 2020 2020 2061  equal..        a
-000024a0: 7373 6572 7420 6c69 7374 2866 696c 7465  ssert list(filte
-000024b0: 7265 645f 616e 645f 6d61 7070 6564 5f65  red_and_mapped_e
-000024c0: 7665 6e74 7329 203d 3d20 6c69 7374 2866  vents) == list(f
-000024d0: 696c 7465 7265 645f 616e 645f 6d61 7070  iltered_and_mapp
-000024e0: 6564 5f65 7665 6e74 735f 6279 5f70 6970  ed_events_by_pip
-000024f0: 656c 696e 6529 0a20 2020 2020 2020 200a  eline).        .
-00002500: 2020 2020 2020 2020 2320 5b31 2e34 5d20          # [1.4] 
-00002510: 5369 6674 2e20 536b 6970 2074 6865 2066  Sift. Skip the f
-00002520: 6972 7374 2066 6577 2069 7465 6d73 206f  irst few items o
-00002530: 7220 6c69 6d69 7420 7468 656d 2e0a 2020  r limit them..  
-00002540: 2020 2020 2020 6461 7461 203d 2044 6174        data = Dat
-00002550: 6128 5b31 2c20 322c 2033 2c20 342c 2035  a([1, 2, 3, 4, 5
-00002560: 2c20 362c 2037 2c20 382c 2039 2c20 3130  , 6, 7, 8, 9, 10
-00002570: 2c20 3131 2c20 3132 2c20 3133 2c20 3134  , 11, 12, 13, 14
-00002580: 2c20 3135 5d29 0a20 2020 2020 2020 2069  , 15]).        i
-00002590: 7465 6d73 5f66 726f 6d5f 3131 5f74 6f5f  tems_from_11_to_
-000025a0: 656e 643a 2047 656e 6572 6174 6f72 203d  end: Generator =
-000025b0: 2064 6174 612e 7369 6674 2873 6b69 703d   data.sift(skip=
-000025c0: 3130 290a 2020 2020 2020 2020 6f6e 6c79  10).        only
-000025d0: 5f66 6972 7374 5f31 305f 6974 656d 733a  _first_10_items:
-000025e0: 2047 656e 6572 6174 6f72 203d 2064 6174   Generator = dat
-000025f0: 612e 7369 6674 286c 696d 6974 3d31 3029  a.sift(limit=10)
-00002600: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002610: 2020 2320 5b31 2e35 5d20 4368 616e 6769    # [1.5] Changi
-00002620: 6e67 2063 6163 6865 2073 7461 7475 732e  ng cache status.
-00002630: 0a20 2020 2020 2020 2065 7665 6e74 732e  .        events.
-00002640: 7573 655f 6361 6368 6528 5472 7565 290a  use_cache(True).
-00002650: 2020 2020 2020 2020 2320 6f72 206a 7573          # or jus
-00002660: 740a 2020 2020 2020 2020 6576 656e 7473  t.        events
-00002670: 2e75 7365 5f63 6163 6865 2829 2020 2320  .use_cache()  # 
-00002680: 4966 2079 6f75 2077 616e 7420 746f 2061  If you want to a
-00002690: 6374 6976 6174 6520 6361 6368 652e 0a20  ctivate cache.. 
-000026a0: 2020 2020 2020 2023 205b 312e 365d 2057         # [1.6] W
-000026b0: 616c 6b20 7468 726f 7567 6820 6461 7461  alk through data
-000026c0: 2e0a 2020 2020 2020 2020 666f 7220 6576  ..        for ev
-000026d0: 656e 7420 696e 2065 7665 6e74 733a 0a20  ent in events:. 
-000026e0: 2020 2020 2020 2020 2020 2023 2044 6f20             # Do 
-000026f0: 736f 6d65 7468 696e 6720 7769 7468 2065  something with e
-00002700: 7665 6e74 2028 6576 656e 7420 6973 2061  vent (event is a
-00002710: 2064 6963 7429 2e0a 2020 2020 2020 2020   dict)..        
-00002720: 2020 2020 7072 696e 7428 6576 656e 7429      print(event)
-00002730: 0a20 2020 2020 2020 2023 2041 6674 6572  .        # After
-00002740: 2066 6972 7374 2069 7465 7261 7469 6f6e   first iteration
-00002750: 2074 6865 2065 7665 6e74 7320 6861 7320   the events has 
-00002760: 6120 6361 6368 6520 6669 6c65 2e0a 2020  a cache file..  
-00002770: 2020 2020 2020 2320 4e6f 7720 7468 6579        # Now they
-00002780: 2077 696c 6c20 6265 2075 7365 6420 696e   will be used in
-00002790: 2074 6865 2063 6163 6865 2069 6e20 7468   the cache in th
-000027a0: 6520 6e65 7874 2069 7465 7261 7469 6f6e  e next iteration
-000027b0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000027c0: 2020 2023 205b 312e 375d 2047 6574 206e     # [1.7] Get n
-000027d0: 756d 6265 7220 6f66 2074 6865 2065 6c65  umber of the ele
-000027e0: 6d65 6e74 7320 696e 2074 6865 2044 6174  ments in the Dat
-000027f0: 6120 6f62 6a65 6374 2e0a 2020 2020 2020  a object..      
-00002800: 2020 6e75 6d62 6572 5f6f 665f 6576 656e    number_of_even
-00002810: 7473 203d 2065 7665 6e74 732e 6c65 6e0a  ts = events.len.
-00002820: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002830: 2023 205b 312e 385d 2043 6865 636b 2074   # [1.8] Check t
-00002840: 6861 7420 4461 7461 206f 626a 6563 7420  hat Data object 
-00002850: 6973 6e27 7420 656d 7074 792e 0a20 2020  isn't empty..   
-00002860: 2020 2020 2023 2054 6865 2064 6174 6120       # The data 
-00002870: 736f 7572 6365 2073 686f 756c 6420 6265  source should be
-00002880: 206e 6f74 2065 6d70 7479 2e0a 2020 2020   not empty..    
-00002890: 2020 2020 6173 7365 7274 2065 7665 6e74      assert event
-000028a0: 732e 6973 5f65 6d70 7479 2069 7320 4661  s.is_empty is Fa
-000028b0: 6c73 650a 2020 2020 2020 2020 0a20 2020  lse.        .   
-000028c0: 2020 2020 2023 205b 312e 395d 2043 6f6e       # [1.9] Con
-000028d0: 7665 7274 2044 6174 6120 6f62 6a65 6374  vert Data object
-000028e0: 2074 6f20 7468 6520 6c69 7374 206f 6620   to the list of 
-000028f0: 656c 656d 656e 7473 2865 7665 6e74 7320  elements(events 
-00002900: 6f72 206d 6573 7361 6765 7329 2e0a 2020  or messages)..  
-00002910: 2020 2020 2020 2320 4265 2063 6172 6566        # Be caref
-00002920: 756c 2c20 7468 6973 2063 616e 2074 616b  ul, this can tak
-00002930: 6520 746f 6f20 6d75 6368 206d 656d 6f72  e too much memor
-00002940: 792e 0a20 2020 2020 2020 2065 7665 6e74  y..        event
-00002950: 735f 6c69 7374 203d 206c 6973 7428 6576  s_list = list(ev
-00002960: 656e 7473 290a 2020 2020 2020 2020 0a20  ents).        . 
-00002970: 2020 2020 2020 2023 205b 312e 3130 5d20         # [1.10] 
-00002980: 5468 6520 6361 6368 6520 696e 6865 7269  The cache inheri
-00002990: 7461 6e63 652e 0a20 2020 2020 2020 2023  tance..        #
-000029a0: 2043 7265 6174 6573 2061 206e 6577 2044   Creates a new D
-000029b0: 6174 6120 6f62 6a65 6374 2074 6861 7420  ata object that 
-000029c0: 7769 6c6c 2075 7365 2063 6163 6865 2066  will use cache f
-000029d0: 726f 6d20 7468 6520 6576 656e 7473 2044  rom the events D
-000029e0: 6174 6120 6f62 6a65 6374 2e0a 2020 2020  ata object..    
-000029f0: 2020 2020 6576 656e 7473 5f66 696c 7465      events_filte
-00002a00: 7265 643a 2044 6174 6120 3d20 6576 656e  red: Data = even
-00002a10: 7473 2e66 696c 7465 7228 6c61 6d62 6461  ts.filter(lambda
-00002a20: 2072 6563 6f72 643a 2072 6563 6f72 642e   record: record.
-00002a30: 6765 7428 2262 6174 6368 4964 2229 290a  get("batchId")).
-00002a40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002a50: 2023 204e 6577 2044 6174 6120 6f62 6a65   # New Data obje
-00002a60: 6374 7320 646f 6e27 7420 7573 6520 7468  cts don't use th
-00002a70: 6569 7220 6f77 6e20 6361 6368 6520 6279  eir own cache by
-00002a80: 2064 6566 6175 6c74 2062 7574 2075 7365   default but use
-00002a90: 2074 6865 2063 6163 6865 206f 6620 7468   the cache of th
-00002aa0: 6520 7061 7265 6e74 2044 6174 6120 6f62  e parent Data ob
-00002ab0: 6a65 6374 2e0a 2020 2020 2020 2020 2320  ject..        # 
-00002ac0: 5573 6520 7573 655f 6361 6368 6520 6d65  Use use_cache me
-00002ad0: 7468 6f64 2074 6f20 6163 7469 7661 7465  thod to activate
-00002ae0: 2063 6163 6869 6e67 2e0a 2020 2020 2020   caching..      
-00002af0: 2020 2320 4166 7465 7220 7468 6174 2c20    # After that, 
-00002b00: 7468 6520 4461 7461 206f 626a 6563 7420  the Data object 
-00002b10: 7769 6c6c 2063 7265 6174 6520 6974 7320  will create its 
-00002b20: 6f77 6e20 6361 6368 6520 6669 6c65 2e0a  own cache file..
-00002b30: 2020 2020 2020 2020 6576 656e 7473 5f66          events_f
-00002b40: 696c 7465 7265 642e 7573 655f 6361 6368  iltered.use_cach
-00002b50: 6528 290a 2020 2020 2020 2020 0a20 2020  e().        .   
-00002b60: 2020 2020 206c 6973 7428 6576 656e 7473       list(events
-00002b70: 5f66 696c 7465 7265 6429 2020 2320 4a75  _filtered)  # Ju
-00002b80: 7374 2074 6f20 6974 6572 6174 6520 4461  st to iterate Da
-00002b90: 7461 206f 626a 6563 7420 2863 6163 6865  ta object (cache
-00002ba0: 2066 696c 6520 7769 6c6c 2062 6520 6372   file will be cr
-00002bb0: 6561 7465 6429 2e0a 2020 2020 2020 2020  eated)..        
-00002bc0: 0a20 2020 2020 2020 2066 696c 7465 7265  .        filtere
-00002bd0: 645f 6576 656e 7473 5f74 7970 6573 203d  d_events_types =
-00002be0: 2065 7665 6e74 735f 6669 6c74 6572 6564   events_filtered
-00002bf0: 2e6d 6170 286c 616d 6264 6120 7265 636f  .map(lambda reco
-00002c00: 7264 3a20 7b22 6576 656e 7454 7970 6522  rd: {"eventType"
-00002c10: 3a20 7265 636f 7264 2e67 6574 2822 6576  : record.get("ev
-00002c20: 656e 7454 7970 6522 297d 290a 2020 2020  entType")}).    
-00002c30: 2020 2020 0a20 2020 2020 2020 2065 7665      .        eve
-00002c40: 6e74 735f 7769 7468 6f75 745f 7479 7065  nts_without_type
-00002c50: 735f 7769 7468 5f62 6174 6368 203d 2066  s_with_batch = f
-00002c60: 696c 7465 7265 645f 6576 656e 7473 5f74  iltered_events_t
-00002c70: 7970 6573 2e66 696c 7465 7228 6c61 6d62  ypes.filter(lamb
-00002c80: 6461 2072 6563 6f72 643a 206e 6f74 2072  da record: not r
-00002c90: 6563 6f72 642e 6765 7428 2265 7665 6e74  ecord.get("event
-00002ca0: 5479 7065 2229 290a 2020 2020 2020 2020  Type")).        
-00002cb0: 6576 656e 7473 5f77 6974 686f 7574 5f74  events_without_t
-00002cc0: 7970 6573 5f77 6974 685f 6261 7463 682e  ypes_with_batch.
-00002cd0: 7573 655f 6361 6368 6528 290a 2020 2020  use_cache().    
-00002ce0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-00002cf0: 312e 3131 5d20 4461 7461 206f 626a 6563  1.11] Data objec
-00002d00: 7473 206a 6f69 6e69 6e67 2e0a 2020 2020  ts joining..    
-00002d10: 2020 2020 2320 596f 7520 6861 7665 2074      # You have t
-00002d20: 6865 2066 6f6c 6c6f 7769 6e67 2033 2044  he following 3 D
-00002d30: 6174 6120 6f62 6a65 6374 732e 0a20 2020  ata objects..   
-00002d40: 2020 2020 2064 3120 3d20 4461 7461 285b       d1 = Data([
-00002d50: 312c 2032 2c20 335d 290a 2020 2020 2020  1, 2, 3]).      
-00002d60: 2020 6432 203d 2044 6174 6128 5b22 6122    d2 = Data(["a"
-00002d70: 2c20 7b22 6964 223a 2031 3233 7d2c 2022  , {"id": 123}, "
-00002d80: 6322 5d29 0a20 2020 2020 2020 2064 3320  c"]).        d3 
-00002d90: 3d20 4461 7461 285b 372c 2038 2c20 395d  = Data([7, 8, 9]
-00002da0: 290a 2020 2020 2020 2020 2320 596f 7520  ).        # You 
-00002db0: 6361 6e20 6a6f 696e 2044 6174 6120 6f62  can join Data ob
-00002dc0: 6a65 6374 7320 696e 2066 6f6c 6c6f 7769  jects in followi
-00002dd0: 6e67 2077 6179 732e 0a20 2020 2020 2020  ng ways..       
-00002de0: 2023 2050 6c65 6173 6520 6e6f 7465 2c20   # Please note, 
-00002df0: 6e65 7720 4461 7461 206f 626a 6563 7420  new Data object 
-00002e00: 7769 6c6c 2068 6176 6520 6361 6368 6520  will have cache 
-00002e10: 7374 6174 7573 203d 3d20 4661 6c73 652e  status == False.
-00002e20: 0a20 2020 2020 2020 2064 6174 615f 7669  .        data_vi
-00002e30: 615f 696e 6974 203d 2044 6174 6128 5b64  a_init = Data([d
-00002e40: 312c 2064 322c 2064 335d 290a 2020 2020  1, d2, d3]).    
-00002e50: 2020 2020 6461 7461 5f76 6961 5f61 6464      data_via_add
-00002e60: 203d 2064 3120 2b20 6432 202b 2064 330a   = d1 + d2 + d3.
-00002e70: 2020 2020 2020 2020 6461 7461 5f77 6974          data_wit
-00002e80: 685f 6e6f 6e5f 6461 7461 5f6f 626a 5f76  h_non_data_obj_v
-00002e90: 6961 5f69 6e69 7420 3d20 4461 7461 285b  ia_init = Data([
-00002ea0: 6431 2c20 5b22 6122 2c20 7b22 6964 223a  d1, ["a", {"id":
-00002eb0: 2031 3233 7d2c 2022 6322 5d2c 2064 335d   123}, "c"], d3]
-00002ec0: 290a 2020 2020 2020 2020 6461 7461 5f77  ).        data_w
-00002ed0: 6974 685f 6e6f 6e5f 6461 7461 5f6f 626a  ith_non_data_obj
-00002ee0: 5f76 6961 5f61 6464 203d 2064 3120 2b20  _via_add = d1 + 
-00002ef0: 5b22 6122 2c20 7b22 6964 223a 2031 3233  ["a", {"id": 123
-00002f00: 7d2c 2022 6322 5d20 2b20 6433 0a20 2020  }, "c"] + d3.   
-00002f10: 2020 2020 2023 2059 6f75 2063 616e 206a       # You can j
-00002f20: 6f69 6e20 6375 7272 656e 7420 4461 7461  oin current Data
-00002f30: 206f 626a 6563 7420 6f6e 2070 6c61 6365   object on place
-00002f40: 2075 7369 6e67 202b 3d2e 0a20 2020 2020   using +=..     
-00002f50: 2020 2023 2049 7420 7769 6c6c 206b 6565     # It will kee
-00002f60: 7020 6361 6368 6520 7374 6174 7573 2e0a  p cache status..
-00002f70: 2020 2020 2020 2020 6431 202b 3d20 6433          d1 += d3
-00002f80: 2020 2320 6431 2077 696c 6c20 6265 636f    # d1 will beco
-00002f90: 6d65 2044 6174 6128 5b31 2c32 2c33 2c37  me Data([1,2,3,7
-00002fa0: 2c38 2c39 5d29 0a20 2020 2020 2020 200a  ,8,9]).        .
-00002fb0: 2020 2020 2020 2020 2320 5b31 2e31 325d          # [1.12]
-00002fc0: 2042 7569 6c64 2061 6e64 2072 6561 6420   Build and read 
-00002fd0: 4461 7461 206f 626a 6563 7420 6361 6368  Data object cach
-00002fe0: 6520 6669 6c65 732e 0a20 2020 2020 2020  e files..       
-00002ff0: 2065 7665 6e74 732e 6275 696c 645f 6361   events.build_ca
-00003000: 6368 6528 2263 6163 6865 5f66 696c 656e  che("cache_filen
-00003010: 616d 655f 6f72 5f70 6174 6822 290a 2020  ame_or_path").  
-00003020: 2020 2020 2020 6461 7461 5f6f 626a 5f66        data_obj_f
-00003030: 726f 6d5f 6361 6368 6520 3d20 4461 7461  rom_cache = Data
-00003040: 2e66 726f 6d5f 6361 6368 655f 6669 6c65  .from_cache_file
-00003050: 2822 6361 6368 655f 6669 6c65 6e61 6d65  ("cache_filename
-00003060: 5f6f 725f 7061 7468 2229 0a20 2020 2020  _or_path").     
-00003070: 2020 200a 2020 2020 2020 2020 2320 5b32     .        # [2
-00003080: 5d20 576f 726b 696e 6720 7769 7468 2063  ] Working with c
-00003090: 6f6e 7665 7274 6572 732e 0a20 2020 2020  onverters..     
-000030a0: 2020 2023 2054 6865 7265 2061 7265 2063     # There are c
-000030b0: 7572 7265 6e74 6c79 2074 6872 6565 2069  urrently three i
-000030c0: 6d70 6c65 6d65 6e74 6174 696f 6e73 206f  mplementations o
-000030d0: 6620 4954 696d 6573 7461 6d70 436f 6e76  f ITimestampConv
-000030e0: 6572 7465 7220 636c 6173 733a 2044 6174  erter class: Dat
-000030f0: 6574 696d 6543 6f6e 7665 7274 652c 2044  etimeConverte, D
-00003100: 6174 6574 696d 6553 7472 696e 6743 6f6e  atetimeStringCon
-00003110: 7665 7274 6572 2061 6e64 2050 726f 746f  verter and Proto
-00003120: 6275 6654 696d 6573 7461 6d70 436f 6e76  bufTimestampConv
-00003130: 6572 7465 722e 0a20 2020 2020 2020 2023  erter..        #
-00003140: 2054 6865 7920 616c 6c20 696d 706c 656d   They all implem
-00003150: 656e 7420 7361 6d65 206d 6574 686f 6473  ent same methods
-00003160: 2066 726f 6d20 6261 7365 2063 6c61 7373   from base class
-00003170: 2e0a 2020 2020 2020 2020 2320 4e6f 7465  ..        # Note
-00003180: 2074 6861 7420 736f 6d65 2061 6363 7572   that some accur
-00003190: 6163 7920 6d61 7920 6265 206c 6f73 7420  acy may be lost 
-000031a0: 6475 7269 6e67 2063 6f6e 7665 7273 696f  during conversio
-000031b0: 6e2e 0a20 2020 2020 2020 2023 2049 6620  n..        # If 
-000031c0: 666f 7220 6578 616d 706c 6520 796f 7520  for example you 
-000031d0: 7573 6520 746f 5f6d 6963 726f 7365 636f  use to_microseco
-000031e0: 6e64 7320 6e61 6e6f 7365 636f 6e64 7320  nds nanoseconds 
-000031f0: 7769 6c6c 2062 6520 6375 7420 6f66 6620  will be cut off 
-00003200: 696e 7374 6561 6420 6f66 2072 6f75 6e64  instead of round
-00003210: 696e 672e 0a20 2020 2020 2020 200a 2020  ing..        .  
-00003220: 2020 2020 2020 2320 5b32 2e31 5d20 4461        # [2.1] Da
-00003230: 7465 7469 6d65 436f 6e76 6572 7465 722e  tetimeConverter.
-00003240: 0a20 2020 2020 2020 2023 2044 6174 6574  .        # Datet
-00003250: 696d 6543 6f6e 7665 7274 6572 2074 616b  imeConverter tak
-00003260: 6573 2064 6174 6574 696d 652e 6461 7465  es datetime.date
-00003270: 7469 6d65 206f 626a 6563 7420 6173 2069  time object as i
-00003280: 6e70 7574 2e0a 2020 2020 2020 2020 0a20  nput..        . 
-00003290: 2020 2020 2020 2064 6174 6574 696d 655f         datetime_
-000032a0: 6f62 6a20 3d20 6461 7465 7469 6d65 2879  obj = datetime(y
-000032b0: 6561 723d 3230 3233 2c20 6d6f 6e74 683d  ear=2023, month=
-000032c0: 312c 2064 6179 3d35 2c20 686f 7572 3d31  1, day=5, hour=1
-000032d0: 342c 206d 696e 7574 653d 3338 2c20 7365  4, minute=38, se
-000032e0: 636f 6e64 3d32 352c 206d 6963 726f 7365  cond=25, microse
-000032f0: 636f 6e64 3d31 3436 3029 0a20 2020 2020  cond=1460).     
-00003300: 2020 200a 2020 2020 2020 2020 2320 4974     .        # It
-00003310: 2068 6173 206d 6574 686f 6473 2074 6861   has methods tha
-00003320: 7420 7265 7475 726e 2074 6865 2064 6174  t return the dat
-00003330: 6574 696d 6520 696e 2064 6966 6665 7265  etime in differe
-00003340: 6e74 2066 6f72 6d61 733a 0a20 2020 2020  nt formas:.     
-00003350: 2020 200a 2020 2020 2020 2020 6461 7465     .        date
-00003360: 5f6d 7320 3d20 4461 7465 7469 6d65 436f  _ms = DatetimeCo
-00003370: 6e76 6572 7465 722e 746f 5f6d 696c 6c69  nverter.to_milli
-00003380: 7365 636f 6e64 7328 6461 7465 7469 6d65  seconds(datetime
-00003390: 5f6f 626a 290a 2020 2020 2020 2020 6461  _obj).        da
-000033a0: 7465 5f75 7320 3d20 4461 7465 7469 6d65  te_us = Datetime
-000033b0: 436f 6e76 6572 7465 722e 746f 5f6d 6963  Converter.to_mic
-000033c0: 726f 7365 636f 6e64 7328 6461 7465 7469  roseconds(dateti
-000033d0: 6d65 5f6f 626a 290a 2020 2020 2020 2020  me_obj).        
-000033e0: 2320 436f 6e76 6572 7469 6e67 2074 6f20  # Converting to 
-000033f0: 6e61 6e6f 7365 636f 6e64 7320 6a75 7374  nanoseconds just
-00003400: 7320 6164 6473 2074 6872 6565 2074 7261  s adds three tra
-00003410: 696c 696e 6720 7a65 726f 7320 6173 2064  iling zeros as d
-00003420: 6174 6574 696d 6520 6f62 6a65 6374 2064  atetime object d
-00003430: 6f65 736e 2774 2068 6176 6520 6e61 6e6f  oesn't have nano
-00003440: 7365 636f 6e64 732e 0a20 2020 2020 2020  seconds..       
-00003450: 2064 6174 655f 6e73 203d 2044 6174 6574   date_ns = Datet
-00003460: 696d 6543 6f6e 7665 7274 6572 2e74 6f5f  imeConverter.to_
-00003470: 6e61 6e6f 7365 636f 6e64 7328 6461 7465  nanoseconds(date
-00003480: 7469 6d65 5f6f 626a 290a 2020 2020 2020  time_obj).      
-00003490: 2020 0a20 2020 2020 2020 2023 205b 322e    .        # [2.
-000034a0: 325d 2044 6174 6574 696d 6553 7472 696e  2] DatetimeStrin
-000034b0: 6743 6f6e 7665 7274 6572 0a20 2020 2020  gConverter.     
-000034c0: 2020 2023 2044 6174 6574 696d 6553 7472     # DatetimeStr
-000034d0: 696e 6743 6f6e 7665 7274 6572 2074 616b  ingConverter tak
-000034e0: 6573 2073 7472 696e 6720 696e 2022 7979  es string in "yy
-000034f0: 7979 2d4d 4d2d 6464 5448 483a 6d6d 3a73  yy-MM-ddTHH:mm:s
-00003500: 735b 2e53 5353 5353 5353 5353 5d5a 2220  s[.SSSSSSSSS]Z" 
-00003510: 666f 726d 6174 2e0a 2020 2020 2020 2020  format..        
-00003520: 0a20 2020 2020 2020 2064 6174 655f 7374  .        date_st
-00003530: 7269 6e67 203d 2022 3230 3233 2d30 312d  ring = "2023-01-
-00003540: 3035 5431 343a 3338 3a32 352e 3030 3134  05T14:38:25.0014
-00003550: 365a 220a 2020 2020 2020 2020 0a20 2020  6Z".        .   
-00003560: 2020 2020 2023 2057 6520 6861 7665 2073       # We have s
-00003570: 616d 6520 6d65 7468 6f64 7320 6173 2069  ame methods as i
-00003580: 6e20 4461 7465 7469 6d65 436f 6e76 6572  n DatetimeConver
-00003590: 7465 720a 2020 2020 2020 2020 6461 7465  ter.        date
-000035a0: 5f6d 735f 6672 6f6d 5f73 7472 696e 6720  _ms_from_string 
-000035b0: 3d20 4461 7465 7469 6d65 5374 7269 6e67  = DatetimeString
-000035c0: 436f 6e76 6572 7465 722e 746f 5f6d 696c  Converter.to_mil
-000035d0: 6c69 7365 636f 6e64 7328 6461 7465 5f73  liseconds(date_s
-000035e0: 7472 696e 6729 0a20 2020 2020 2020 2064  tring).        d
-000035f0: 6174 655f 7573 5f66 726f 6d5f 7374 7269  ate_us_from_stri
-00003600: 6e67 203d 2044 6174 6574 696d 6553 7472  ng = DatetimeStr
-00003610: 696e 6743 6f6e 7665 7274 6572 2e74 6f5f  ingConverter.to_
-00003620: 6d69 6372 6f73 6563 6f6e 6473 2864 6174  microseconds(dat
-00003630: 655f 7374 7269 6e67 290a 2020 2020 2020  e_string).      
-00003640: 2020 6461 7465 5f6e 735f 6672 6f6d 5f73    date_ns_from_s
-00003650: 7472 696e 6720 3d20 4461 7465 7469 6d65  tring = Datetime
-00003660: 5374 7269 6e67 436f 6e76 6572 7465 722e  StringConverter.
-00003670: 746f 5f6e 616e 6f73 6563 6f6e 6473 2864  to_nanoseconds(d
-00003680: 6174 655f 7374 7269 6e67 290a 2020 2020  ate_string).    
-00003690: 2020 2020 0a20 2020 2020 2020 2023 2057      .        # W
-000036a0: 6520 6361 6e20 616c 736f 2067 6574 2064  e can also get d
-000036b0: 6174 6574 696d 6520 6f62 6a65 6374 2066  atetime object f
-000036c0: 726f 6d20 7374 7269 6e67 0a20 2020 2020  rom string.     
-000036d0: 2020 2064 6174 6574 696d 655f 6672 6f6d     datetime_from
-000036e0: 5f73 7472 696e 6720 3d20 4461 7465 7469  _string = Dateti
-000036f0: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
-00003700: 722e 746f 5f64 6174 6574 696d 6528 6461  r.to_datetime(da
-00003710: 7465 5f73 7472 696e 6729 0a20 2020 2020  te_string).     
-00003720: 2020 200a 2020 2020 2020 2020 2320 5b32     .        # [2
-00003730: 2e33 5d20 5072 6f74 6f62 7566 5469 6d65  .3] ProtobufTime
-00003740: 7374 616d 7043 6f6e 7665 7274 6572 0a20  stampConverter. 
-00003750: 2020 2020 2020 2023 2050 726f 746f 6275         # Protobu
-00003760: 6620 7469 6d65 7374 616d 7073 206d 7573  f timestamps mus
-00003770: 7420 6265 2069 6e20 666f 726d 207b 2265  t be in form {"e
-00003780: 706f 6368 5365 636f 6e64 223a 2073 6563  pochSecond": sec
-00003790: 6f6e 6473 2c20 226e 616e 6f22 3a20 6e61  onds, "nano": na
-000037a0: 6e6f 7365 636f 6e64 737d 0a20 2020 2020  noseconds}.     
-000037b0: 2020 200a 2020 2020 2020 2020 7072 6f74     .        prot
-000037c0: 6f62 7566 5f74 696d 6573 7461 6d70 203d  obuf_timestamp =
-000037d0: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
-000037e0: 2031 3637 3239 3239 3530 352c 2022 6e61   1672929505, "na
-000037f0: 6e6f 223a 2031 5f34 3630 5f30 3030 7d0a  no": 1_460_000}.
-00003800: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00003810: 2064 6174 655f 6d73 5f66 726f 6d5f 7469   date_ms_from_ti
-00003820: 6d65 7374 616d 7020 3d20 5072 6f74 6f62  mestamp = Protob
-00003830: 7566 5469 6d65 7374 616d 7043 6f6e 7665  ufTimestampConve
-00003840: 7274 6572 2e74 6f5f 6d69 6c6c 6973 6563  rter.to_millisec
-00003850: 6f6e 6473 2870 726f 746f 6275 665f 7469  onds(protobuf_ti
-00003860: 6d65 7374 616d 7029 0a20 2020 2020 2020  mestamp).       
-00003870: 2064 6174 655f 7573 5f66 726f 6d5f 7469   date_us_from_ti
-00003880: 6d65 7374 616d 7020 3d20 5072 6f74 6f62  mestamp = Protob
-00003890: 7566 5469 6d65 7374 616d 7043 6f6e 7665  ufTimestampConve
-000038a0: 7274 6572 2e74 6f5f 6d69 6372 6f73 6563  rter.to_microsec
-000038b0: 6f6e 6473 2870 726f 746f 6275 665f 7469  onds(protobuf_ti
-000038c0: 6d65 7374 616d 7029 0a20 2020 2020 2020  mestamp).       
-000038d0: 2064 6174 655f 6e73 5f66 726f 6d5f 7469   date_ns_from_ti
-000038e0: 6d65 7374 616d 7020 3d20 5072 6f74 6f62  mestamp = Protob
-000038f0: 7566 5469 6d65 7374 616d 7043 6f6e 7665  ufTimestampConve
-00003900: 7274 6572 2e74 6f5f 6e61 6e6f 7365 636f  rter.to_nanoseco
-00003910: 6e64 7328 7072 6f74 6f62 7566 5f74 696d  nds(protobuf_tim
-00003920: 6573 7461 6d70 290a 2020 2020 2020 2020  estamp).        
-00003930: 6461 7465 7469 6d65 5f66 726f 6d5f 7469  datetime_from_ti
-00003940: 6d65 7374 616d 7020 3d20 5072 6f74 6f62  mestamp = Protob
-00003950: 7566 5469 6d65 7374 616d 7043 6f6e 7665  ufTimestampConve
-00003960: 7274 6572 2e74 6f5f 6461 7465 7469 6d65  rter.to_datetime
-00003970: 2870 726f 746f 6275 665f 7469 6d65 7374  (protobuf_timest
-00003980: 616d 7029 0a20 2020 2020 2020 200a 2020  amp).        .  
-00003990: 2020 2020 2020 2320 5b33 5d20 576f 726b        # [3] Work
-000039a0: 696e 6720 7769 7468 2045 7665 6e74 5472  ing with EventTr
-000039b0: 6565 2061 6e64 2045 7665 6e74 5472 6565  ee and EventTree
-000039c0: 436f 6c6c 6563 7469 6f6e 2e0a 2020 2020  Collection..    
-000039d0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-000039e0: 332e 315d 2042 7569 6c64 2061 2063 7573  3.1] Build a cus
-000039f0: 746f 6d20 4576 656e 7454 7265 650a 2020  tom EventTree.  
-00003a00: 2020 2020 2020 2320 546f 2063 7265 6174        # To creat
-00003a10: 6520 616e 2045 7665 6e74 5472 6565 206f  e an EventTree o
-00003a20: 626a 6563 7420 796f 7520 6e65 6564 2074  bject you need t
-00003a30: 6f20 7072 6f76 6964 6520 6e61 6d65 2c20  o provide name, 
-00003a40: 6964 2061 6e64 2064 6174 6120 6f66 2074  id and data of t
-00003a50: 6865 2072 6f6f 7420 6576 656e 742e 0a20  he root event.. 
-00003a60: 2020 2020 2020 2074 7265 6520 3d20 4576         tree = Ev
-00003a70: 656e 7454 7265 6528 6576 656e 745f 6e61  entTree(event_na
-00003a80: 6d65 3d22 726f 6f74 2065 7665 6e74 222c  me="root event",
-00003a90: 2065 7665 6e74 5f69 643d 2272 6f6f 745f   event_id="root_
-00003aa0: 6964 222c 2064 6174 613d 7b22 6461 7461  id", data={"data
-00003ab0: 223a 205b 312c 2032 2c20 332c 2034 2c20  ": [1, 2, 3, 4, 
-00003ac0: 355d 7d29 0a20 2020 2020 2020 200a 2020  5]}).        .  
-00003ad0: 2020 2020 2020 2320 546f 2061 6464 206e        # To add n
-00003ae0: 6577 206e 6f64 6520 7573 6520 6170 7065  ew node use appe
-00003af0: 6e64 5f65 7665 6e74 2e20 7061 7265 6e74  nd_event. parent
-00003b00: 5f69 6420 6973 206e 6563 6573 7361 7279  _id is necessary
-00003b10: 2c20 6461 7461 2069 7320 6f70 7469 6f6e  , data is option
-00003b20: 616c 2e0a 2020 2020 2020 2020 7472 6565  al..        tree
-00003b30: 2e61 7070 656e 645f 6576 656e 7428 6576  .append_event(ev
-00003b40: 656e 745f 6e61 6d65 3d22 4122 2c20 6576  ent_name="A", ev
-00003b50: 656e 745f 6964 3d22 415f 6964 222c 2064  ent_id="A_id", d
-00003b60: 6174 613d 4e6f 6e65 2c20 7061 7265 6e74  ata=None, parent
-00003b70: 5f69 643d 2272 6f6f 745f 6964 2229 0a20  _id="root_id"). 
-00003b80: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003b90: 2320 5b33 2e33 5d20 4275 696c 6469 6e67  # [3.3] Building
-00003ba0: 2074 6865 2045 7665 6e74 5472 6565 436f   the EventTreeCo
-00003bb0: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
-00003bc0: 2020 0a20 2020 2020 2020 2023 2049 6620    .        # If 
-00003bd0: 796f 7520 646f 6e27 7420 7370 6563 6966  you don't specif
-00003be0: 7920 6461 7461 5f73 6f75 7263 6520 666f  y data_source fo
-00003bf0: 7220 7468 6520 6472 6976 6572 2074 6865  r the driver the
-00003c00: 6e20 6974 2077 6f6e 2774 2072 6563 6f76  n it won't recov
-00003c10: 6572 2064 6574 6163 6865 6420 6576 656e  er detached even
-00003c20: 7473 2e0a 2020 2020 2020 2020 6472 6976  ts..        driv
-00003c30: 6572 3a20 4945 5443 4472 6976 6572 2020  er: IETCDriver  
-00003c40: 2320 596f 7520 7368 6f75 6c64 2069 6e69  # You should ini
-00003c50: 7420 4554 4344 7269 7665 7220 6f62 6a65  t ETCDriver obje
-00003c60: 6374 2e20 452e 672e 2066 726f 6d20 4c77  ct. E.g. from Lw
-00003c70: 4450 206d 6f64 756c 6520 6f72 2079 6f75  DP module or you
-00003c80: 7220 6375 7374 6f6d 2063 6c61 7373 2e0a  r custom class..
-00003c90: 2020 2020 2020 2020 6574 6320 3d20 4576          etc = Ev
-00003ca0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00003cb0: 6e28 6472 6976 6572 290a 2020 2020 2020  n(driver).      
-00003cc0: 2020 6574 632e 6275 696c 6428 6576 656e    etc.build(even
-00003cd0: 7473 290a 2020 2020 2020 2020 0a20 2020  ts).        .   
-00003ce0: 2020 2020 2023 2044 6574 6163 6865 6420       # Detached 
-00003cf0: 6576 656e 7473 2069 736e 2774 2065 6d70  events isn't emp
-00003d00: 7479 2e0a 2020 2020 2020 2020 6173 7365  ty..        asse
-00003d10: 7274 2065 7463 2e67 6574 5f64 6574 6163  rt etc.get_detac
-00003d20: 6865 645f 6576 656e 7473 2829 0a20 2020  hed_events().   
-00003d30: 2020 2020 200a 2020 2020 2020 2020 6574       .        et
-00003d40: 6320 3d20 4576 656e 7454 7265 6543 6f6c  c = EventTreeCol
-00003d50: 6c65 6374 696f 6e28 6472 6976 6572 290a  lection(driver).
-00003d60: 2020 2020 2020 2020 2320 4465 7461 6368          # Detach
-00003d70: 6564 2065 7665 6e74 7320 6172 6520 656d  ed events are em
-00003d80: 7074 7920 6265 6361 7573 6520 7468 6579  pty because they
-00003d90: 2077 6572 6520 7265 636f 7665 7265 642e   were recovered.
-00003da0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00003db0: 6e6f 7420 6574 632e 6765 745f 6465 7461  not etc.get_deta
-00003dc0: 6368 6564 5f65 7665 6e74 7328 290a 2020  ched_events().  
-00003dd0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00003de0: 2054 6865 2063 6f6c 6c65 6374 696f 6e20   The collection 
-00003df0: 6861 7320 4576 656e 7454 7265 6573 2065  has EventTrees e
-00003e00: 6163 6820 7769 7468 2061 2074 7265 6520  ach with a tree 
-00003e10: 6f66 2065 7665 6e74 732e 0a20 2020 2020  of events..     
-00003e20: 2020 2023 2055 7369 6e67 2043 6f6c 6c65     # Using Colle
-00003e30: 6374 696f 6e20 616e 6420 4576 656e 7454  ction and EventT
-00003e40: 7265 6573 2c20 796f 7520 6361 6e20 776f  rees, you can wo
-00003e50: 726b 2066 6c65 7869 626c 7920 7769 7468  rk flexibly with
-00003e60: 2065 7665 6e74 732e 0a20 2020 2020 2020   events..       
-00003e70: 200a 2020 2020 2020 2020 2320 5b33 2e33   .        # [3.3
-00003e80: 2e31 5d20 4765 7420 6c65 6176 6573 206f  .1] Get leaves o
-00003e90: 6620 616c 6c20 7472 6565 732e 0a20 2020  f all trees..   
-00003ea0: 2020 2020 206c 6561 7665 733a 2054 7570       leaves: Tup
-00003eb0: 6c65 5b64 6963 745d 203d 2065 7463 2e67  le[dict] = etc.g
-00003ec0: 6574 5f6c 6561 7665 7328 290a 2020 2020  et_leaves().    
+000005f0: 2020 2020 2a20 5b46 6965 6c64 7352 6573      * [FieldsRes
+00000600: 6f6c 7665 725d 2823 6669 656c 6473 7265  olver](#fieldsre
+00000610: 736f 6c76 6572 290a 2020 2020 2020 2020  solver).        
+00000620: 2020 202a 205b 322e 342e 204c 696e 6b73     * [2.4. Links
+00000630: 5d28 2332 342d 6c69 6e6b 7329 0a20 2020  ](#24-links).   
+00000640: 2020 2020 202a 205b 332e 2042 6573 7420       * [3. Best 
+00000650: 7072 6163 7469 6365 735d 2823 332d 6265  practices](#3-be
+00000660: 7374 2d70 7261 6374 6963 6573 290a 2020  st-practices).  
+00000670: 2020 2020 2020 2a20 5b34 2e20 4f66 6669        * [4. Offi
+00000680: 6369 616c 2044 6174 6153 6f75 7263 6520  cial DataSource 
+00000690: 696d 706c 656d 656e 7461 7469 6f6e 735d  implementations]
+000006a0: 2823 342d 6f66 6669 6369 616c 2d64 6174  (#4-official-dat
+000006b0: 6173 6f75 7263 652d 696d 706c 656d 656e  asource-implemen
+000006c0: 7461 7469 6f6e 7329 0a20 2020 2020 2020  tations).       
+000006d0: 202a 205b 352e 2041 5049 5d28 2335 2d61   * [5. API](#5-a
+000006e0: 7069 290a 2020 2020 2020 2020 2a20 5b36  pi).        * [6
+000006f0: 2e20 4578 616d 706c 6573 5d28 2336 2d65  . Examples](#6-e
+00000700: 7861 6d70 6c65 7329 0a20 2020 2020 2020  xamples).       
+00000710: 203c 212d 2d74 652d 2d3e 0a20 2020 2020   <!--te-->.     
+00000720: 2020 200a 2020 2020 2020 2020 2320 312e     .        # 1.
+00000730: 2049 6e74 726f 6475 6374 696f 6e0a 2020   Introduction.  
+00000740: 2020 2020 2020 0a20 2020 2020 2020 2054        .        T
+00000750: 6869 7320 7265 706f 7369 746f 7279 2069  his repository i
+00000760: 7320 6120 6c69 6272 6172 7920 666f 7220  s a library for 
+00000770: 6372 6561 7469 6e67 2074 6832 2d64 6174  creating th2-dat
+00000780: 612d 7365 7276 6963 6573 2061 7070 6c69  a-services appli
+00000790: 6361 7469 6f6e 732e 0a20 2020 2020 2020  cations..       
+000007a0: 2044 6174 6120 5365 7276 6963 6573 2061   Data Services a
+000007b0: 6c6c 6f77 7320 796f 7520 746f 206d 616e  llows you to man
+000007c0: 6970 756c 6174 6520 7468 6520 7374 7265  ipulate the stre
+000007d0: 616d 2064 6174 6120 7072 6f63 6573 7369  am data processi
+000007e0: 6e67 2077 6f72 6b66 6c6f 7720 7573 696e  ng workflow usin
+000007f0: 6720 7069 7065 6c69 6e69 6e67 2e0a 2020  g pipelining..  
+00000800: 2020 2020 2020 0a20 2020 2020 2020 2054        .        T
+00000810: 6865 206c 6962 7261 7279 2773 2066 6561  he library's fea
+00000820: 7475 7265 733a 0a20 2020 2020 2020 200a  tures:.        .
+00000830: 2020 2020 2020 2020 2d20 5072 6f76 6964          - Provid
+00000840: 6573 2063 6f72 6520 696e 7465 7266 6163  es core interfac
+00000850: 6520 666f 7220 6465 7665 6c6f 7069 6e67  e for developing
+00000860: 2064 6174 6120 736f 7572 6365 2069 6d70   data source imp
+00000870: 6c65 6d65 6e74 6174 696f 6e73 0a20 2020  lementations.   
+00000880: 2020 2020 202d 2057 6f72 6b20 7769 7468       - Work with
+00000890: 2069 7465 7261 626c 6520 6f62 6a65 6374   iterable object
+000008a0: 7320 286c 6973 742c 2074 7570 6c65 2c20  s (list, tuple, 
+000008b0: 6574 6320 696e 636c 7564 696e 6720 6669  etc including fi
+000008c0: 6c65 7329 2076 6961 205f 4461 7461 206f  les) via _Data o
+000008d0: 626a 6563 745f 2075 7369 6e67 2069 7473  bject_ using its
+000008e0: 2066 6561 7475 7265 730a 2020 2020 2020   features.      
+000008f0: 2020 2d20 4d61 6e69 7075 6c61 7465 2074    - Manipulate t
+00000900: 6865 2077 6f72 6b66 6c6f 7720 746f 206d  he workflow to m
+00000910: 616b 6520 736f 6d65 2061 6e61 6c79 7369  ake some analysi
+00000920: 7320 6279 205f 4461 7461 206f 626a 6563  s by _Data objec
+00000930: 745f 206d 6574 686f 6473 0a20 2020 2020  t_ methods.     
+00000940: 2020 202d 2055 7365 2074 696d 6573 7461     - Use timesta
+00000950: 6d70 2063 6f6e 7665 7274 6572 2069 6d70  mp converter imp
+00000960: 6c65 6d65 6e74 6174 696f 6e73 206f 7220  lementations or 
+00000970: 7573 6520 6261 7365 2063 6c61 7373 2074  use base class t
+00000980: 6f20 6372 6561 7465 2063 7573 746f 6d20  o create custom 
+00000990: 636f 6e76 6572 7465 7273 0a20 2020 2020  converters.     
+000009a0: 2020 202d 2042 7569 6c64 2045 7665 6e74     - Build Event
+000009b0: 2054 7265 6573 2028 4576 656e 7454 7265   Trees (EventTre
+000009c0: 652c 2045 7665 6e74 5472 6565 436f 6c6c  e, EventTreeColl
+000009d0: 6563 7469 6f6e 2061 6e64 2050 6172 656e  ection and Paren
+000009e0: 7445 7665 6e74 5472 6565 436f 6c6c 6563  tEventTreeCollec
+000009f0: 7469 6f6e 2063 6c61 7373 6573 290a 2020  tion classes).  
+00000a00: 2020 2020 2020 0a20 2020 2020 2020 2057        .        W
+00000a10: 6f72 6b66 6c6f 7720 6d61 6e69 7075 6c61  orkflow manipula
+00000a20: 7469 6f6e 2074 6f6f 6c73 2061 6c6c 6f77  tion tools allow
+00000a30: 7320 796f 753a 0a20 2020 2020 2020 200a  s you:.        .
+00000a40: 2020 2020 2020 2020 2d20 4669 6c74 6572          - Filter
+00000a50: 696e 6720 7374 7265 616d 2064 6174 6120  ing stream data 
+00000a60: 2860 4461 7461 2e66 696c 7465 7260 206d  (`Data.filter` m
+00000a70: 6574 686f 6429 0a20 2020 2020 2020 202d  ethod).        -
+00000a80: 2054 7261 6e73 666f 726d 696e 6720 7374   Transforming st
+00000a90: 7265 616d 2064 6174 6120 2860 4461 7461  ream data (`Data
+00000aa0: 2e6d 6170 6020 6d65 7468 6f64 290a 2020  .map` method).  
+00000ab0: 2020 2020 2020 2d20 4c69 6d69 7469 6e67        - Limiting
+00000ac0: 2074 6865 206e 756d 6265 7220 6f66 2070   the number of p
+00000ad0: 726f 6365 7373 6564 2073 7472 6561 6d69  rocessed streami
+00000ae0: 6e67 2064 6174 6120 2860 4461 7461 2e6c  ng data (`Data.l
+00000af0: 696d 6974 6020 6d65 7468 6f64 290a 2020  imit` method).  
+00000b00: 2020 2020 2020 0a20 2020 2020 2020 2054        .        T
+00000b10: 6865 7265 2069 7320 616c 736f 2061 6e6f  here is also ano
+00000b20: 7468 6572 2070 6172 7420 6f66 205f 6461  ther part of _da
+00000b30: 7461 2073 6572 7669 6365 735f 0a20 2020  ta services_.   
+00000b40: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+00000b50: 5b74 6832 2d64 6174 612d 7365 7276 6963  [th2-data-servic
+00000b60: 6573 2d75 7469 6c73 5d28 6874 7470 733a  es-utils](https:
+00000b70: 2f2f 6769 7468 7562 2e63 6f6d 2f74 6832  //github.com/th2
+00000b80: 2d6e 6574 2f74 6832 2d64 6174 612d 7365  -net/th2-data-se
+00000b90: 7276 6963 6573 2d75 7469 6c73 292e 2049  rvices-utils). I
+00000ba0: 7427 7320 6120 7365 7420 6f66 2074 6f6f  t's a set of too
+00000bb0: 6c73 2074 6f20 7065 7266 6f72 6d20 7468  ls to perform th
+00000bc0: 6520 6d6f 7374 0a20 2020 2020 2020 2020  e most.         
+00000bd0: 2063 6f6d 6d6f 6e20 616e 616c 7973 6973   common analysis
+00000be0: 2074 6173 6b73 2e0a 2020 2020 2020 2020   tasks..        
+00000bf0: 0a20 2020 2020 2020 2023 2032 2e20 4765  .        # 2. Ge
+00000c00: 7474 696e 6720 7374 6172 7465 640a 2020  tting started.  
+00000c10: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00000c20: 2320 322e 312e 2049 6e73 7461 6c6c 6174  # 2.1. Installat
+00000c30: 696f 6e0a 2020 2020 2020 2020 0a20 2020  ion.        .   
+00000c40: 2020 2020 2023 2323 2043 6f72 650a 2020       ### Core.  
+00000c50: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00000c60: 2046 726f 6d20 5079 5049 2028 7069 7029   From PyPI (pip)
+00000c70: 2020 200a 2020 2020 2020 2020 2020 5468     .          Th
+00000c80: 6973 2070 6163 6b61 6765 2063 616e 2062  is package can b
+00000c90: 6520 666f 756e 6420 6f6e 205b 5079 5049  e found on [PyPI
+00000ca0: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+00000cb0: 7267 2f70 726f 6a65 6374 2f74 6832 2d64  rg/project/th2-d
+00000cc0: 6174 612d 7365 7276 6963 6573 2f20 2274  ata-services/ "t
+00000cd0: 6832 2d64 6174 612d 7365 7276 6963 6573  h2-data-services
+00000ce0: 2229 2e0a 2020 2020 2020 2020 2020 2020  ")..            
+00000cf0: 6060 600a 2020 2020 2020 2020 2020 2020  ```.            
+00000d00: 7069 7020 696e 7374 616c 6c20 7468 322d  pip install th2-
+00000d10: 6461 7461 2d73 6572 7669 6365 730a 2020  data-services.  
+00000d20: 2020 2020 2020 2020 2020 6060 600a 2020            ```.  
+00000d30: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00000d40: 2046 726f 6d20 536f 7572 6365 0a20 2020   From Source.   
+00000d50: 2020 2020 2020 2020 2060 6060 0a20 2020           ```.   
+00000d60: 2020 2020 2020 2020 2067 6974 2063 6c6f           git clo
+00000d70: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
+00000d80: 622e 636f 6d2f 7468 322d 6e65 742f 7468  b.com/th2-net/th
+00000d90: 322d 6461 7461 2d73 6572 7669 6365 730a  2-data-services.
+00000da0: 2020 2020 2020 2020 2020 2020 7069 7020              pip 
+00000db0: 696e 7374 616c 6c20 7468 322d 6461 7461  install th2-data
+00000dc0: 2d73 6572 7669 6365 732f 0a20 2020 2020  -services/.     
+00000dd0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00000de0: 2020 200a 2020 2020 2020 2020 2323 2320     .        ### 
+00000df0: 4461 7461 2073 6f75 7263 6573 2028 7072  Data sources (pr
+00000e00: 6f76 6964 6572 7329 0a20 2020 2020 2020  oviders).       
+00000e10: 200a 2020 2020 2020 2020 5369 6e63 6520   .        Since 
+00000e20: 6076 312e 332e 3060 2c20 7468 6520 6c69  `v1.3.0`, the li
+00000e30: 6272 6172 7920 646f 6573 6e27 7420 7072  brary doesn't pr
+00000e40: 6f76 6964 6520 6461 7461 2073 6f75 7263  ovide data sourc
+00000e50: 6520 6465 7065 6e64 656e 6369 6573 2e0a  e dependencies..
+00000e60: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000e70: 2059 6f75 2073 686f 756c 6420 7072 6f76   You should prov
+00000e80: 6964 6520 6974 206d 616e 7561 6c6c 7920  ide it manually 
+00000e90: 6475 7269 6e67 2069 6e73 7461 6c6c 6174  during installat
+00000ea0: 696f 6e2e 200a 2020 2020 2020 2020 596f  ion. .        Yo
+00000eb0: 7520 6a75 7374 206e 6565 6420 746f 2061  u just need to a
+00000ec0: 6464 2073 7175 6172 6520 6272 6163 6b65  dd square bracke
+00000ed0: 7473 2061 6674 6572 206c 6962 7261 7279  ts after library
+00000ee0: 206e 616d 6520 616e 6420 7075 7420 6465   name and put de
+00000ef0: 7065 6e64 656e 6379 206e 616d 652e 0a20  pendency name.. 
+00000f00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000f10: 6060 600a 2020 2020 2020 2020 7069 7020  ```.        pip 
+00000f20: 696e 7374 616c 6c20 7468 322d 6461 7461  install th2-data
+00000f30: 2d73 6572 7669 6365 735b 6465 7065 6e64  -services[depend
+00000f40: 656e 6379 5f6e 616d 655d 0a20 2020 2020  ency_name].     
+00000f50: 2020 2060 6060 0a20 2020 2020 2020 200a     ```.        .
+00000f60: 2020 2020 2020 2020 2a2a 4465 7065 6e64          **Depend
+00000f70: 656e 6369 6573 206c 6973 742a 2a20 0a20  encies list** . 
+00000f80: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000f90: 7c20 2064 6570 656e 6465 6e63 7920 6e61  |  dependency na
+00000fa0: 6d65 2020 7c20 7072 6f76 6964 6572 2076  me  | provider v
+00000fb0: 6572 7369 6f6e 2020 2020 2020 2020 2020  ersion          
+00000fc0: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
+00000fd0: 2020 2020 2020 7c3a 2d2d 2d2d 2d2d 2d2d        |:--------
+00000fe0: 2d2d 2d2d 2d2d 2d2d 2d3a 7c2d 2d2d 2d2d  ---------:|-----
+00000ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001010: 2d2d 7c0a 2020 2020 2020 2020 7c20 2020  --|.        |   
+00001020: 2020 2020 6c77 6470 2020 2020 2020 2020      lwdp        
+00001030: 7c20 6c61 7465 7374 2076 6572 7369 6f6e  | latest version
+00001040: 206f 6620 6c77 6470 2020 2020 2020 2020   of lwdp        
+00001050: 2020 2020 2020 2020 7c0a 2020 2020 2020          |.      
+00001060: 2020 7c20 2020 2020 2020 6c77 6470 3220    |       lwdp2 
+00001070: 2020 2020 2020 7c20 6c61 7465 7374 2076        | latest v
+00001080: 6572 7369 6f6e 206f 6620 6c77 6470 2076  ersion of lwdp v
+00001090: 3220 2020 2020 2020 2020 2020 2020 7c0a  2             |.
+000010a0: 2020 2020 2020 2020 7c20 7574 696c 732d          | utils-
+000010b0: 7270 742d 7669 6577 6572 2020 7c20 6c61  rpt-viewer  | la
+000010c0: 7465 7374 2076 6572 7369 6f6e 206f 6620  test version of 
+000010d0: 7574 696c 732d 7270 742d 7669 6577 6572  utils-rpt-viewer
+000010e0: 2020 2020 7c0a 2020 2020 2020 2020 7c20      |.        | 
+000010f0: 7574 696c 732d 7270 742d 7669 6577 6572  utils-rpt-viewer
+00001100: 3520 7c20 6c61 7465 7374 2076 6572 7369  5 | latest versi
+00001110: 6f6e 206f 6620 7574 696c 732d 7270 742d  on of utils-rpt-
+00001120: 7669 6577 6572 2076 3520 7c0a 2020 2020  viewer v5 |.    
+00001130: 2020 2020 7c20 2020 7574 696c 732d 6164      |   utils-ad
+00001140: 7661 6e63 6564 2020 7c20 6c61 7465 7374  vanced  | latest
+00001150: 2076 6572 7369 6f6e 206f 6620 6473 2d75   version of ds-u
+00001160: 7469 6c73 2020 2020 2020 2020 2020 2020  tils            
+00001170: 7c0a 2020 2020 2020 2020 0a20 2020 2020  |.        .     
+00001180: 2020 202a 2a45 7861 6d70 6c65 2a2a 0a20     **Example**. 
+00001190: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000011a0: 6060 600a 2020 2020 2020 2020 7069 7020  ```.        pip 
+000011b0: 696e 7374 616c 6c20 7468 322d 6461 7461  install th2-data
+000011c0: 2d73 6572 7669 6365 735b 6c77 6470 315d  -services[lwdp1]
+000011d0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+000011e0: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
+000011f0: 2032 2e32 2e20 4578 616d 706c 650a 2020   2.2. Example.  
+00001200: 2020 2020 2020 0a20 2020 2020 2020 2041        .        A
+00001210: 2067 6f6f 642c 2073 686f 7274 2065 7861   good, short exa
+00001220: 6d70 6c65 2069 7320 776f 7274 6820 6120  mple is worth a 
+00001230: 7468 6f75 7361 6e64 2077 6f72 6473 2e0a  thousand words..
+00001240: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001250: 2054 6869 7320 6578 616d 706c 6520 7368   This example sh
+00001260: 6f77 7320 6261 7369 6320 7573 6167 6520  ows basic usage 
+00001270: 6f66 206c 6962 7261 7279 2773 2066 6561  of library's fea
+00001280: 7475 7265 732e 0a20 2020 2020 2020 200a  tures..        .
+00001290: 2020 2020 2020 2020 5b54 6865 2066 6f6c          [The fol
+000012a0: 6c6f 7769 6e67 2065 7861 6d70 6c65 2061  lowing example a
+000012b0: 7320 6120 6669 6c65 5d28 6578 616d 706c  s a file](exampl
+000012c0: 6573 2f67 6574 5f73 7461 7274 6564 5f65  es/get_started_e
+000012d0: 7861 6d70 6c65 2e70 7929 2e0a 2020 2020  xample.py)..    
+000012e0: 2020 2020 0a20 2020 2020 2020 203c 212d      .        <!-
+000012f0: 2d20 7374 6172 7420 6765 745f 7374 6172  - start get_star
+00001300: 7465 645f 6578 616d 706c 652e 7079 202d  ted_example.py -
+00001310: 2d3e 0a20 2020 2020 2020 2060 6060 7079  ->.        ```py
+00001320: 7468 6f6e 0a20 2020 2020 2020 2066 726f  thon.        fro
+00001330: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00001340: 5475 706c 652c 204c 6973 742c 204f 7074  Tuple, List, Opt
+00001350: 696f 6e61 6c2c 2047 656e 6572 6174 6f72  ional, Generator
+00001360: 0a20 2020 2020 2020 2066 726f 6d20 6461  .        from da
+00001370: 7465 7469 6d65 2069 6d70 6f72 7420 6461  tetime import da
+00001380: 7465 7469 6d65 0a20 2020 2020 2020 200a  tetime.        .
+00001390: 2020 2020 2020 2020 6672 6f6d 2074 6832          from th2
+000013a0: 5f64 6174 615f 7365 7276 6963 6573 2e64  _data_services.d
+000013b0: 6174 6120 696d 706f 7274 2044 6174 610a  ata import Data.
+000013c0: 2020 2020 2020 2020 6672 6f6d 2074 6832          from th2
+000013d0: 5f64 6174 615f 7365 7276 6963 6573 2e65  _data_services.e
+000013e0: 7665 6e74 5f74 7265 6520 696d 706f 7274  vent_tree import
+000013f0: 2045 7665 6e74 5472 6565 2c20 4576 656e   EventTree, Even
+00001400: 7454 7265 6543 6f6c 6c65 6374 696f 6e2c  tTreeCollection,
+00001410: 2050 6172 656e 7445 7665 6e74 5472 6565   ParentEventTree
+00001420: 436f 6c6c 6563 7469 6f6e 2c20 4945 5443  Collection, IETC
+00001430: 4472 6976 6572 0a20 2020 2020 2020 2066  Driver.        f
+00001440: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
+00001450: 7669 6365 732e 696e 7465 7266 6163 6573  vices.interfaces
+00001460: 2069 6d70 6f72 7420 4944 6174 6153 6f75   import IDataSou
+00001470: 7263 650a 2020 2020 2020 2020 6672 6f6d  rce.        from
+00001480: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
+00001490: 6573 2e75 7469 6c73 2e63 6f6e 7665 7274  es.utils.convert
+000014a0: 6572 7320 696d 706f 7274 2044 6174 6574  ers import Datet
+000014b0: 696d 6543 6f6e 7665 7274 6572 2c20 4461  imeConverter, Da
+000014c0: 7465 7469 6d65 5374 7269 6e67 436f 6e76  tetimeStringConv
+000014d0: 6572 7465 722c 2050 726f 746f 6275 6654  erter, ProtobufT
+000014e0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
+000014f0: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
+00001500: 2020 2023 205b 305d 204c 6962 2063 6f6e     # [0] Lib con
+00001510: 6669 6775 7261 7469 6f6e 0a20 2020 2020  figuration.     
+00001520: 2020 2023 205b 302e 315d 2049 6e74 6572     # [0.1] Inter
+00001530: 6163 7469 7665 206f 7220 5363 7269 7074  active or Script
+00001540: 206d 6f64 650a 2020 2020 2020 2020 2320   mode.        # 
+00001550: 4966 2079 6f75 2075 7365 2074 6865 206c  If you use the l
+00001560: 6962 2069 6e20 696e 7465 7261 6374 6976  ib in interactiv
+00001570: 6520 6d6f 6465 2028 6a75 7079 7465 722c  e mode (jupyter,
+00001580: 2069 7079 7468 6f6e 2920 6974 2773 2072   ipython) it's r
+00001590: 6563 6f6d 6d65 6e64 6564 2074 6f20 7365  ecommended to se
+000015a0: 7420 7468 6520 7370 6563 6961 6c0a 2020  t the special.  
+000015b0: 2020 2020 2020 2320 676c 6f62 616c 2070        # global p
+000015c0: 6172 616d 6574 6572 2074 6f20 5472 7565  arameter to True
+000015d0: 2e20 4974 276c 6c20 6b65 6570 2063 6163  . It'll keep cac
+000015e0: 6865 2066 696c 6573 2069 6620 736f 6d65  he files if some
+000015f0: 7468 696e 6720 7765 6e74 2077 726f 6e67  thing went wrong
+00001600: 2e0a 2020 2020 2020 2020 6672 6f6d 2074  ..        from t
+00001610: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
+00001620: 2e63 6f6e 6669 6720 696d 706f 7274 206f  .config import o
+00001630: 7074 696f 6e73 0a20 2020 2020 2020 200a  ptions.        .
+00001640: 2020 2020 2020 2020 6f70 7469 6f6e 732e          options.
+00001650: 494e 5445 5241 4354 4956 455f 4d4f 4445  INTERACTIVE_MODE
+00001660: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+00001670: 0a20 2020 2020 2020 2023 2053 6f6d 6520  .        # Some 
+00001680: 6578 616d 706c 6520 6461 7461 0a20 2020  example data.   
+00001690: 2020 2020 2065 7665 6e74 7320 3d20 4461       events = Da
+000016a0: 7461 280a 2020 2020 2020 2020 2020 2020  ta(.            
+000016b0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+000016c0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+000016d0: 2020 2020 2020 2020 2265 7665 6e74 4964          "eventId
+000016e0: 223a 2022 6465 6d6f 5f62 6f6f 6b5f 313a  ": "demo_book_1:
+000016f0: 7468 322d 7363 6f70 653a 3230 3233 3031  th2-scope:202301
+00001700: 3035 3133 3537 3035 3536 3038 3733 3030  0513570556087300
+00001710: 303a 6436 3165 3933 3061 2d38 6430 302d  0:d61e930a-8d00-
+00001720: 3131 6564 2d61 6131 612d 6433 3461 3631  11ed-aa1a-d34a61
+00001730: 3535 3135 3264 5f31 222c 0a20 2020 2020  55152d_1",.     
+00001740: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001750: 6261 7463 6849 6422 3a20 4e6f 6e65 2c0a  batchId": None,.
+00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001770: 2020 2020 2269 7342 6174 6368 6564 223a      "isBatched":
+00001780: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+00001790: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+000017a0: 6e74 4e61 6d65 223a 2022 5365 7420 6f66  ntName": "Set of
+000017b0: 2061 7574 6f2d 6765 6e65 7261 7465 6420   auto-generated 
+000017c0: 6576 656e 7473 2066 6f72 2064 7320 6c69  events for ds li
+000017d0: 6220 7465 7374 696e 6722 2c0a 2020 2020  b testing",.    
+000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017f0: 2265 7665 6e74 5479 7065 223a 2022 6473  "eventType": "ds
+00001800: 2d6c 6962 2d74 6573 742d 6576 656e 7422  -lib-test-event"
+00001810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001820: 2020 2020 2020 2265 6e64 5469 6d65 7374        "endTimest
+00001830: 616d 7022 3a20 7b22 6570 6f63 6853 6563  amp": {"epochSec
+00001840: 6f6e 6422 3a20 3136 3732 3932 3730 3235  ond": 1672927025
+00001850: 2c20 226e 616e 6f22 3a20 3536 3137 3531  , "nano": 561751
+00001860: 3030 307d 2c0a 2020 2020 2020 2020 2020  000},.          
+00001870: 2020 2020 2020 2020 2020 2273 7461 7274            "start
+00001880: 5469 6d65 7374 616d 7022 3a20 7b22 6570  Timestamp": {"ep
+00001890: 6f63 6853 6563 6f6e 6422 3a20 3136 3732  ochSecond": 1672
+000018a0: 3932 3730 3235 2c20 226e 616e 6f22 3a20  927025, "nano": 
+000018b0: 3536 3038 3733 3030 307d 2c0a 2020 2020  560873000},.    
+000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018d0: 2270 6172 656e 7445 7665 6e74 4964 223a  "parentEventId":
+000018e0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+000018f0: 2020 2020 2020 2020 2020 2022 7375 6363             "succ
+00001900: 6573 7366 756c 223a 2054 7275 652c 0a20  essful": True,. 
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2020 2022 626f 6f6b 4964 223a 2022 6465     "bookId": "de
+00001930: 6d6f 5f62 6f6f 6b5f 3122 2c0a 2020 2020  mo_book_1",.    
+00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001950: 2273 636f 7065 223a 2022 7468 322d 7363  "scope": "th2-sc
+00001960: 6f70 6522 2c0a 2020 2020 2020 2020 2020  ope",.          
+00001970: 2020 2020 2020 2020 2020 2261 7474 6163            "attac
+00001980: 6865 644d 6573 7361 6765 4964 7322 3a20  hedMessageIds": 
+00001990: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+000019a0: 2020 2020 2020 2020 2262 6f64 7922 3a20          "body": 
+000019b0: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+000019c0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+000019d0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000019e0: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
+000019f0: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
+00001a00: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
+00001a10: 3032 3330 3130 3531 3335 3730 3535 3633  0230105135705563
+00001a20: 3532 3230 3030 3a39 6164 6262 3365 302d  522000:9adbb3e0-
+00001a30: 3566 3862 2d34 6332 382d 6132 6163 2d37  5f8b-4c28-a2ac-7
+00001a40: 3336 3165 3866 6137 3034 633e 6465 6d6f  361e8fa704c>demo
+00001a50: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
+00001a60: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
+00001a70: 3536 3335 3232 3030 303a 6436 3165 3933  563522000:d61e93
+00001a80: 3061 2d38 6430 302d 3131 6564 2d61 6131  0a-8d00-11ed-aa1
+00001a90: 612d 6433 3461 3631 3535 3135 3264 5f32  a-d34a6155152d_2
+00001aa0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001ab0: 2020 2020 2020 2022 6261 7463 6849 6422         "batchId"
+00001ac0: 3a20 2264 656d 6f5f 626f 6f6b 5f31 3a74  : "demo_book_1:t
+00001ad0: 6832 2d73 636f 7065 3a32 3032 3330 3130  h2-scope:2023010
+00001ae0: 3531 3335 3730 3535 3633 3532 3230 3030  5135705563522000
+00001af0: 3a39 6164 6262 3365 302d 3566 3862 2d34  :9adbb3e0-5f8b-4
+00001b00: 6332 382d 6132 6163 2d37 3336 3165 3866  c28-a2ac-7361e8f
+00001b10: 6137 3034 6322 2c0a 2020 2020 2020 2020  a704c",.        
+00001b20: 2020 2020 2020 2020 2020 2020 2269 7342              "isB
+00001b30: 6174 6368 6564 223a 2054 7275 652c 0a20  atched": True,. 
+00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b50: 2020 2022 6576 656e 744e 616d 6522 3a20     "eventName": 
+00001b60: 2250 6c61 696e 2065 7665 6e74 2031 222c  "Plain event 1",
+00001b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b80: 2020 2020 2022 6576 656e 7454 7970 6522       "eventType"
+00001b90: 3a20 2264 732d 6c69 622d 7465 7374 2d65  : "ds-lib-test-e
+00001ba0: 7665 6e74 222c 0a20 2020 2020 2020 2020  vent",.         
+00001bb0: 2020 2020 2020 2020 2020 2022 656e 6454             "endT
+00001bc0: 696d 6573 7461 6d70 223a 207b 2265 706f  imestamp": {"epo
+00001bd0: 6368 5365 636f 6e64 223a 2031 3637 3239  chSecond": 16729
+00001be0: 3237 3032 352c 2022 6e61 6e6f 223a 2035  27025, "nano": 5
+00001bf0: 3633 3634 3030 3030 7d2c 0a20 2020 2020  63640000},.     
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001c10: 7374 6172 7454 696d 6573 7461 6d70 223a  startTimestamp":
+00001c20: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
+00001c30: 2031 3637 3239 3237 3032 352c 2022 6e61   1672927025, "na
+00001c40: 6e6f 223a 2035 3633 3532 3230 3030 7d2c  no": 563522000},
+00001c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c60: 2020 2020 2022 7061 7265 6e74 4576 656e       "parentEven
+00001c70: 7449 6422 3a20 2264 656d 6f5f 626f 6f6b  tId": "demo_book
+00001c80: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+00001c90: 3330 3130 3531 3335 3730 3535 3630 3837  3010513570556087
+00001ca0: 3330 3030 3a64 3631 6539 3330 612d 3864  3000:d61e930a-8d
+00001cb0: 3030 2d31 3165 642d 6161 3161 2d64 3334  00-11ed-aa1a-d34
+00001cc0: 6136 3135 3531 3532 645f 3122 2c0a 2020  a6155152d_1",.  
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 2273 7563 6365 7373 6675 6c22 3a20    "successful": 
+00001cf0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00001d00: 2020 2020 2020 2020 2020 2262 6f6f 6b49            "bookI
+00001d10: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
+00001d20: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001d30: 2020 2020 2020 2022 7363 6f70 6522 3a20         "scope": 
+00001d40: 2274 6832 2d73 636f 7065 222c 0a20 2020  "th2-scope",.   
+00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d60: 2022 6174 7461 6368 6564 4d65 7373 6167   "attachedMessag
+00001d70: 6549 6473 223a 205b 5d2c 0a20 2020 2020  eIds": [],.     
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001d90: 626f 6479 223a 207b 2274 7970 6522 3a20  body": {"type": 
+00001da0: 226d 6573 7361 6765 222c 2022 6461 7461  "message", "data
+00001db0: 223a 2022 6473 2d6c 6962 2074 6573 7420  ": "ds-lib test 
+00001dc0: 626f 6479 227d 2c0a 2020 2020 2020 2020  body"},.        
+00001dd0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001de0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e00: 2022 6576 656e 7449 6422 3a20 2264 656d   "eventId": "dem
+00001e10: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
+00001e20: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
+00001e30: 3535 3633 3532 3230 3030 3a39 6164 6262  5563522000:9adbb
+00001e40: 3365 302d 3566 3862 2d34 6332 382d 6132  3e0-5f8b-4c28-a2
+00001e50: 6163 2d37 3336 3165 3866 6137 3034 633e  ac-7361e8fa704c>
+00001e60: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
+00001e70: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
+00001e80: 3537 3035 3536 3337 3537 3030 303a 6436  5705563757000:d6
+00001e90: 3165 3933 3061 2d38 6430 302d 3131 6564  1e930a-8d00-11ed
+00001ea0: 2d61 6131 612d 6433 3461 3631 3535 3135  -aa1a-d34a615515
+00001eb0: 3264 5f33 222c 0a20 2020 2020 2020 2020  2d_3",.         
+00001ec0: 2020 2020 2020 2020 2020 2022 6261 7463             "batc
+00001ed0: 6849 6422 3a20 2264 656d 6f5f 626f 6f6b  hId": "demo_book
+00001ee0: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+00001ef0: 3330 3130 3531 3335 3730 3535 3633 3532  3010513570556352
+00001f00: 3230 3030 3a39 6164 6262 3365 302d 3566  2000:9adbb3e0-5f
+00001f10: 3862 2d34 6332 382d 6132 6163 2d37 3336  8b-4c28-a2ac-736
+00001f20: 3165 3866 6137 3034 6322 2c0a 2020 2020  1e8fa704c",.    
+00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f40: 2269 7342 6174 6368 6564 223a 2054 7275  "isBatched": Tru
+00001f50: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00001f60: 2020 2020 2020 2022 6576 656e 744e 616d         "eventNam
+00001f70: 6522 3a20 2250 6c61 696e 2065 7665 6e74  e": "Plain event
+00001f80: 2032 222c 0a20 2020 2020 2020 2020 2020   2",.           
+00001f90: 2020 2020 2020 2020 2022 6576 656e 7454           "eventT
+00001fa0: 7970 6522 3a20 2264 732d 6c69 622d 7465  ype": "ds-lib-te
+00001fb0: 7374 2d65 7665 6e74 222c 0a20 2020 2020  st-event",.     
+00001fc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001fd0: 656e 6454 696d 6573 7461 6d70 223a 207b  endTimestamp": {
+00001fe0: 2265 706f 6368 5365 636f 6e64 223a 2031  "epochSecond": 1
+00001ff0: 3637 3239 3237 3032 352c 2022 6e61 6e6f  672927025, "nano
+00002000: 223a 2035 3633 3739 3130 3030 7d2c 0a20  ": 563791000},. 
+00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002020: 2020 2022 7374 6172 7454 696d 6573 7461     "startTimesta
+00002030: 6d70 223a 207b 2265 706f 6368 5365 636f  mp": {"epochSeco
+00002040: 6e64 223a 2031 3637 3239 3237 3032 352c  nd": 1672927025,
+00002050: 2022 6e61 6e6f 223a 2035 3633 3735 3730   "nano": 5637570
+00002060: 3030 7d2c 0a20 2020 2020 2020 2020 2020  00},.           
+00002070: 2020 2020 2020 2020 2022 7061 7265 6e74           "parent
+00002080: 4576 656e 7449 6422 3a20 2264 656d 6f5f  EventId": "demo_
+00002090: 626f 6f6b 5f31 3a74 6832 2d73 636f 7065  book_1:th2-scope
+000020a0: 3a32 3032 3330 3130 3531 3335 3730 3535  :202301051357055
+000020b0: 3630 3837 3330 3030 3a64 3631 6539 3330  60873000:d61e930
+000020c0: 612d 3864 3030 2d31 3165 642d 6161 3161  a-8d00-11ed-aa1a
+000020d0: 2d64 3334 6136 3135 3531 3532 645f 3122  -d34a6155152d_1"
+000020e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000020f0: 2020 2020 2020 2273 7563 6365 7373 6675        "successfu
+00002100: 6c22 3a20 5472 7565 2c0a 2020 2020 2020  l": True,.      
+00002110: 2020 2020 2020 2020 2020 2020 2020 2262                "b
+00002120: 6f6f 6b49 6422 3a20 2264 656d 6f5f 626f  ookId": "demo_bo
+00002130: 6f6b 5f31 222c 0a20 2020 2020 2020 2020  ok_1",.         
+00002140: 2020 2020 2020 2020 2020 2022 7363 6f70             "scop
+00002150: 6522 3a20 2274 6832 2d73 636f 7065 222c  e": "th2-scope",
+00002160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002170: 2020 2020 2022 6174 7461 6368 6564 4d65       "attachedMe
+00002180: 7373 6167 6549 6473 223a 205b 5d2c 0a20  ssageIds": [],. 
+00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021a0: 2020 2022 626f 6479 223a 207b 2274 7970     "body": {"typ
+000021b0: 6522 3a20 226d 6573 7361 6765 222c 2022  e": "message", "
+000021c0: 6461 7461 223a 2022 6473 2d6c 6962 2074  data": "ds-lib t
+000021d0: 6573 7420 626f 6479 227d 2c0a 2020 2020  est body"},.    
+000021e0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000021f0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00002200: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
+00002210: 2020 2020 2020 2020 2320 5b31 5d20 576f          # [1] Wo
+00002220: 726b 696e 6720 7769 7468 2061 2044 6174  rking with a Dat
+00002230: 6120 6f62 6a65 6374 2e0a 2020 2020 2020  a object..      
+00002240: 2020 2320 5b31 2e31 5d20 4669 6c74 6572    # [1.1] Filter
+00002250: 2e0a 2020 2020 2020 2020 6669 6c74 6572  ..        filter
+00002260: 6564 5f65 7665 6e74 733a 2044 6174 6120  ed_events: Data 
+00002270: 3d20 6576 656e 7473 2e66 696c 7465 7228  = events.filter(
+00002280: 6c61 6d62 6461 2065 3a20 655b 2262 6f64  lambda e: e["bod
+00002290: 7922 5d20 213d 205b 5d29 2020 2320 4669  y"] != [])  # Fi
+000022a0: 6c74 6572 2065 7665 6e74 7320 7769 7468  lter events with
+000022b0: 2065 6d70 7479 2062 6f64 792e 0a20 2020   empty body..   
+000022c0: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
+000022d0: 2020 2020 2020 2023 205b 312e 325d 204d         # [1.2] M
+000022e0: 6170 2e0a 2020 2020 2020 2020 6465 6620  ap..        def 
+000022f0: 7472 616e 7366 6f72 6d5f 6675 6e63 7469  transform_functi
+00002300: 6f6e 2872 6563 6f72 6429 3a0a 2020 2020  on(record):.    
+00002310: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+00002320: 2265 7665 6e74 4e61 6d65 223a 2072 6563  "eventName": rec
+00002330: 6f72 645b 2265 7665 6e74 4e61 6d65 225d  ord["eventName"]
+00002340: 2c20 2273 7563 6365 7373 6675 6c22 3a20  , "successful": 
+00002350: 7265 636f 7264 5b22 7375 6363 6573 7366  record["successf
+00002360: 756c 225d 7d0a 2020 2020 2020 2020 0a20  ul"]}.        . 
+00002370: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002380: 6669 6c74 6572 6564 5f61 6e64 5f6d 6170  filtered_and_map
+00002390: 7065 645f 6576 656e 7473 203d 2066 696c  ped_events = fil
+000023a0: 7465 7265 645f 6576 656e 7473 2e6d 6170  tered_events.map
+000023b0: 2874 7261 6e73 666f 726d 5f66 756e 6374  (transform_funct
+000023c0: 696f 6e29 0a20 2020 2020 2020 200a 2020  ion).        .  
+000023d0: 2020 2020 2020 2320 5b31 2e33 5d20 4461        # [1.3] Da
+000023e0: 7461 2070 6970 656c 696e 652e 0a20 2020  ta pipeline..   
+000023f0: 2020 2020 2023 2020 2020 2020 2049 6e73       #       Ins
+00002400: 7465 6164 206f 6620 646f 696e 6720 6461  tead of doing da
+00002410: 7461 2074 7261 6e73 666f 726d 6174 696f  ta transformatio
+00002420: 6e73 2073 7465 7020 6279 2073 7465 7020  ns step by step 
+00002430: 796f 7520 6361 6e20 646f 2069 7420 696e  you can do it in
+00002440: 206f 6e65 206c 696e 652e 0a20 2020 2020   one line..     
+00002450: 2020 2066 696c 7465 7265 645f 616e 645f     filtered_and_
+00002460: 6d61 7070 6564 5f65 7665 6e74 735f 6279  mapped_events_by
+00002470: 5f70 6970 656c 696e 6520 3d20 6576 656e  _pipeline = even
+00002480: 7473 2e66 696c 7465 7228 6c61 6d62 6461  ts.filter(lambda
+00002490: 2065 3a20 655b 2262 6f64 7922 5d20 213d   e: e["body"] !=
+000024a0: 205b 5d29 2e6d 6170 2874 7261 6e73 666f   []).map(transfo
+000024b0: 726d 5f66 756e 6374 696f 6e29 0a20 2020  rm_function).   
+000024c0: 2020 2020 2023 2043 6f6e 7465 6e74 206f       # Content o
+000024d0: 6620 7468 6573 6520 7477 6f20 4461 7461  f these two Data
+000024e0: 206f 626a 6563 7473 2073 686f 756c 6420   objects should 
+000024f0: 6265 2065 7175 616c 2e0a 2020 2020 2020  be equal..      
+00002500: 2020 6173 7365 7274 206c 6973 7428 6669    assert list(fi
+00002510: 6c74 6572 6564 5f61 6e64 5f6d 6170 7065  ltered_and_mappe
+00002520: 645f 6576 656e 7473 2920 3d3d 206c 6973  d_events) == lis
+00002530: 7428 6669 6c74 6572 6564 5f61 6e64 5f6d  t(filtered_and_m
+00002540: 6170 7065 645f 6576 656e 7473 5f62 795f  apped_events_by_
+00002550: 7069 7065 6c69 6e65 290a 2020 2020 2020  pipeline).      
+00002560: 2020 0a20 2020 2020 2020 2023 205b 312e    .        # [1.
+00002570: 345d 2053 6966 742e 2053 6b69 7020 7468  4] Sift. Skip th
+00002580: 6520 6669 7273 7420 6665 7720 6974 656d  e first few item
+00002590: 7320 6f72 206c 696d 6974 2074 6865 6d2e  s or limit them.
+000025a0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+000025b0: 4461 7461 285b 312c 2032 2c20 332c 2034  Data([1, 2, 3, 4
+000025c0: 2c20 352c 2036 2c20 372c 2038 2c20 392c  , 5, 6, 7, 8, 9,
+000025d0: 2031 302c 2031 312c 2031 322c 2031 332c   10, 11, 12, 13,
+000025e0: 2031 342c 2031 355d 290a 2020 2020 2020   14, 15]).      
+000025f0: 2020 6974 656d 735f 6672 6f6d 5f31 315f    items_from_11_
+00002600: 746f 5f65 6e64 3a20 4765 6e65 7261 746f  to_end: Generato
+00002610: 7220 3d20 6461 7461 2e73 6966 7428 736b  r = data.sift(sk
+00002620: 6970 3d31 3029 0a20 2020 2020 2020 206f  ip=10).        o
+00002630: 6e6c 795f 6669 7273 745f 3130 5f69 7465  nly_first_10_ite
+00002640: 6d73 3a20 4765 6e65 7261 746f 7220 3d20  ms: Generator = 
+00002650: 6461 7461 2e73 6966 7428 6c69 6d69 743d  data.sift(limit=
+00002660: 3130 290a 2020 2020 2020 2020 0a20 2020  10).        .   
+00002670: 2020 2020 2023 205b 312e 355d 2043 6861       # [1.5] Cha
+00002680: 6e67 696e 6720 6361 6368 6520 7374 6174  nging cache stat
+00002690: 7573 2e0a 2020 2020 2020 2020 6576 656e  us..        even
+000026a0: 7473 2e75 7365 5f63 6163 6865 2854 7275  ts.use_cache(Tru
+000026b0: 6529 0a20 2020 2020 2020 2023 206f 7220  e).        # or 
+000026c0: 6a75 7374 0a20 2020 2020 2020 2065 7665  just.        eve
+000026d0: 6e74 732e 7573 655f 6361 6368 6528 2920  nts.use_cache() 
+000026e0: 2023 2049 6620 796f 7520 7761 6e74 2074   # If you want t
+000026f0: 6f20 6163 7469 7661 7465 2063 6163 6865  o activate cache
+00002700: 2e0a 2020 2020 2020 2020 2320 5b31 2e36  ..        # [1.6
+00002710: 5d20 5761 6c6b 2074 6872 6f75 6768 2064  ] Walk through d
+00002720: 6174 612e 0a20 2020 2020 2020 2066 6f72  ata..        for
+00002730: 2065 7665 6e74 2069 6e20 6576 656e 7473   event in events
+00002740: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00002750: 446f 2073 6f6d 6574 6869 6e67 2077 6974  Do something wit
+00002760: 6820 6576 656e 7420 2865 7665 6e74 2069  h event (event i
+00002770: 7320 6120 6469 6374 292e 0a20 2020 2020  s a dict)..     
+00002780: 2020 2020 2020 2070 7269 6e74 2865 7665         print(eve
+00002790: 6e74 290a 2020 2020 2020 2020 2320 4166  nt).        # Af
+000027a0: 7465 7220 6669 7273 7420 6974 6572 6174  ter first iterat
+000027b0: 696f 6e20 7468 6520 6576 656e 7473 2068  ion the events h
+000027c0: 6173 2061 2063 6163 6865 2066 696c 652e  as a cache file.
+000027d0: 0a20 2020 2020 2020 2023 204e 6f77 2074  .        # Now t
+000027e0: 6865 7920 7769 6c6c 2062 6520 7573 6564  hey will be used
+000027f0: 2069 6e20 7468 6520 6361 6368 6520 696e   in the cache in
+00002800: 2074 6865 206e 6578 7420 6974 6572 6174   the next iterat
+00002810: 696f 6e2e 0a20 2020 2020 2020 200a 2020  ion..        .  
+00002820: 2020 2020 2020 2320 5b31 2e37 5d20 4765        # [1.7] Ge
+00002830: 7420 6e75 6d62 6572 206f 6620 7468 6520  t number of the 
+00002840: 656c 656d 656e 7473 2069 6e20 7468 6520  elements in the 
+00002850: 4461 7461 206f 626a 6563 742e 0a20 2020  Data object..   
+00002860: 2020 2020 206e 756d 6265 725f 6f66 5f65       number_of_e
+00002870: 7665 6e74 7320 3d20 6576 656e 7473 2e6c  vents = events.l
+00002880: 656e 0a20 2020 2020 2020 200a 2020 2020  en.        .    
+00002890: 2020 2020 2320 5b31 2e38 5d20 4368 6563      # [1.8] Chec
+000028a0: 6b20 7468 6174 2044 6174 6120 6f62 6a65  k that Data obje
+000028b0: 6374 2069 736e 2774 2065 6d70 7479 2e0a  ct isn't empty..
+000028c0: 2020 2020 2020 2020 2320 5468 6520 6461          # The da
+000028d0: 7461 2073 6f75 7263 6520 7368 6f75 6c64  ta source should
+000028e0: 2062 6520 6e6f 7420 656d 7074 792e 0a20   be not empty.. 
+000028f0: 2020 2020 2020 2061 7373 6572 7420 6576         assert ev
+00002900: 656e 7473 2e69 735f 656d 7074 7920 6973  ents.is_empty is
+00002910: 2046 616c 7365 0a20 2020 2020 2020 200a   False.        .
+00002920: 2020 2020 2020 2020 2320 5b31 2e39 5d20          # [1.9] 
+00002930: 436f 6e76 6572 7420 4461 7461 206f 626a  Convert Data obj
+00002940: 6563 7420 746f 2074 6865 206c 6973 7420  ect to the list 
+00002950: 6f66 2065 6c65 6d65 6e74 7328 6576 656e  of elements(even
+00002960: 7473 206f 7220 6d65 7373 6167 6573 292e  ts or messages).
+00002970: 0a20 2020 2020 2020 2023 2042 6520 6361  .        # Be ca
+00002980: 7265 6675 6c2c 2074 6869 7320 6361 6e20  reful, this can 
+00002990: 7461 6b65 2074 6f6f 206d 7563 6820 6d65  take too much me
+000029a0: 6d6f 7279 2e0a 2020 2020 2020 2020 6576  mory..        ev
+000029b0: 656e 7473 5f6c 6973 7420 3d20 6c69 7374  ents_list = list
+000029c0: 2865 7665 6e74 7329 0a20 2020 2020 2020  (events).       
+000029d0: 200a 2020 2020 2020 2020 2320 5b31 2e31   .        # [1.1
+000029e0: 305d 2054 6865 2063 6163 6865 2069 6e68  0] The cache inh
+000029f0: 6572 6974 616e 6365 2e0a 2020 2020 2020  eritance..      
+00002a00: 2020 2320 4372 6561 7465 7320 6120 6e65    # Creates a ne
+00002a10: 7720 4461 7461 206f 626a 6563 7420 7468  w Data object th
+00002a20: 6174 2077 696c 6c20 7573 6520 6361 6368  at will use cach
+00002a30: 6520 6672 6f6d 2074 6865 2065 7665 6e74  e from the event
+00002a40: 7320 4461 7461 206f 626a 6563 742e 0a20  s Data object.. 
+00002a50: 2020 2020 2020 2065 7665 6e74 735f 6669         events_fi
+00002a60: 6c74 6572 6564 3a20 4461 7461 203d 2065  ltered: Data = e
+00002a70: 7665 6e74 732e 6669 6c74 6572 286c 616d  vents.filter(lam
+00002a80: 6264 6120 7265 636f 7264 3a20 7265 636f  bda record: reco
+00002a90: 7264 2e67 6574 2822 6261 7463 6849 6422  rd.get("batchId"
+00002aa0: 2929 0a20 2020 2020 2020 200a 2020 2020  )).        .    
+00002ab0: 2020 2020 2320 4e65 7720 4461 7461 206f      # New Data o
+00002ac0: 626a 6563 7473 2064 6f6e 2774 2075 7365  bjects don't use
+00002ad0: 2074 6865 6972 206f 776e 2063 6163 6865   their own cache
+00002ae0: 2062 7920 6465 6661 756c 7420 6275 7420   by default but 
+00002af0: 7573 6520 7468 6520 6361 6368 6520 6f66  use the cache of
+00002b00: 2074 6865 2070 6172 656e 7420 4461 7461   the parent Data
+00002b10: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
+00002b20: 2023 2055 7365 2075 7365 5f63 6163 6865   # Use use_cache
+00002b30: 206d 6574 686f 6420 746f 2061 6374 6976   method to activ
+00002b40: 6174 6520 6361 6368 696e 672e 0a20 2020  ate caching..   
+00002b50: 2020 2020 2023 2041 6674 6572 2074 6861       # After tha
+00002b60: 742c 2074 6865 2044 6174 6120 6f62 6a65  t, the Data obje
+00002b70: 6374 2077 696c 6c20 6372 6561 7465 2069  ct will create i
+00002b80: 7473 206f 776e 2063 6163 6865 2066 696c  ts own cache fil
+00002b90: 652e 0a20 2020 2020 2020 2065 7665 6e74  e..        event
+00002ba0: 735f 6669 6c74 6572 6564 2e75 7365 5f63  s_filtered.use_c
+00002bb0: 6163 6865 2829 0a20 2020 2020 2020 200a  ache().        .
+00002bc0: 2020 2020 2020 2020 6c69 7374 2865 7665          list(eve
+00002bd0: 6e74 735f 6669 6c74 6572 6564 2920 2023  nts_filtered)  #
+00002be0: 204a 7573 7420 746f 2069 7465 7261 7465   Just to iterate
+00002bf0: 2044 6174 6120 6f62 6a65 6374 2028 6361   Data object (ca
+00002c00: 6368 6520 6669 6c65 2077 696c 6c20 6265  che file will be
+00002c10: 2063 7265 6174 6564 292e 0a20 2020 2020   created)..     
+00002c20: 2020 200a 2020 2020 2020 2020 6669 6c74     .        filt
+00002c30: 6572 6564 5f65 7665 6e74 735f 7479 7065  ered_events_type
+00002c40: 7320 3d20 6576 656e 7473 5f66 696c 7465  s = events_filte
+00002c50: 7265 642e 6d61 7028 6c61 6d62 6461 2072  red.map(lambda r
+00002c60: 6563 6f72 643a 207b 2265 7665 6e74 5479  ecord: {"eventTy
+00002c70: 7065 223a 2072 6563 6f72 642e 6765 7428  pe": record.get(
+00002c80: 2265 7665 6e74 5479 7065 2229 7d29 0a20  "eventType")}). 
+00002c90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002ca0: 6576 656e 7473 5f77 6974 686f 7574 5f74  events_without_t
+00002cb0: 7970 6573 5f77 6974 685f 6261 7463 6820  ypes_with_batch 
+00002cc0: 3d20 6669 6c74 6572 6564 5f65 7665 6e74  = filtered_event
+00002cd0: 735f 7479 7065 732e 6669 6c74 6572 286c  s_types.filter(l
+00002ce0: 616d 6264 6120 7265 636f 7264 3a20 6e6f  ambda record: no
+00002cf0: 7420 7265 636f 7264 2e67 6574 2822 6576  t record.get("ev
+00002d00: 656e 7454 7970 6522 2929 0a20 2020 2020  entType")).     
+00002d10: 2020 2065 7665 6e74 735f 7769 7468 6f75     events_withou
+00002d20: 745f 7479 7065 735f 7769 7468 5f62 6174  t_types_with_bat
+00002d30: 6368 2e75 7365 5f63 6163 6865 2829 0a20  ch.use_cache(). 
+00002d40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002d50: 2320 5b31 2e31 315d 2044 6174 6120 6f62  # [1.11] Data ob
+00002d60: 6a65 6374 7320 6a6f 696e 696e 672e 0a20  jects joining.. 
+00002d70: 2020 2020 2020 2023 2059 6f75 2068 6176         # You hav
+00002d80: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00002d90: 3320 4461 7461 206f 626a 6563 7473 2e0a  3 Data objects..
+00002da0: 2020 2020 2020 2020 6431 203d 2044 6174          d1 = Dat
+00002db0: 6128 5b31 2c20 322c 2033 5d29 0a20 2020  a([1, 2, 3]).   
+00002dc0: 2020 2020 2064 3220 3d20 4461 7461 285b       d2 = Data([
+00002dd0: 2261 222c 207b 2269 6422 3a20 3132 337d  "a", {"id": 123}
+00002de0: 2c20 2263 225d 290a 2020 2020 2020 2020  , "c"]).        
+00002df0: 6433 203d 2044 6174 6128 5b37 2c20 382c  d3 = Data([7, 8,
+00002e00: 2039 5d29 0a20 2020 2020 2020 2023 2059   9]).        # Y
+00002e10: 6f75 2063 616e 206a 6f69 6e20 4461 7461  ou can join Data
+00002e20: 206f 626a 6563 7473 2069 6e20 666f 6c6c   objects in foll
+00002e30: 6f77 696e 6720 7761 7973 2e0a 2020 2020  owing ways..    
+00002e40: 2020 2020 2320 506c 6561 7365 206e 6f74      # Please not
+00002e50: 652c 206e 6577 2044 6174 6120 6f62 6a65  e, new Data obje
+00002e60: 6374 2077 696c 6c20 6861 7665 2063 6163  ct will have cac
+00002e70: 6865 2073 7461 7475 7320 3d3d 2046 616c  he status == Fal
+00002e80: 7365 2e0a 2020 2020 2020 2020 6461 7461  se..        data
+00002e90: 5f76 6961 5f69 6e69 7420 3d20 4461 7461  _via_init = Data
+00002ea0: 285b 6431 2c20 6432 2c20 6433 5d29 0a20  ([d1, d2, d3]). 
+00002eb0: 2020 2020 2020 2064 6174 615f 7669 615f         data_via_
+00002ec0: 6164 6420 3d20 6431 202b 2064 3220 2b20  add = d1 + d2 + 
+00002ed0: 6433 0a20 2020 2020 2020 2064 6174 615f  d3.        data_
+00002ee0: 7769 7468 5f6e 6f6e 5f64 6174 615f 6f62  with_non_data_ob
+00002ef0: 6a5f 7669 615f 696e 6974 203d 2044 6174  j_via_init = Dat
+00002f00: 6128 5b64 312c 205b 2261 222c 207b 2269  a([d1, ["a", {"i
+00002f10: 6422 3a20 3132 337d 2c20 2263 225d 2c20  d": 123}, "c"], 
+00002f20: 6433 5d29 0a20 2020 2020 2020 2064 6174  d3]).        dat
+00002f30: 615f 7769 7468 5f6e 6f6e 5f64 6174 615f  a_with_non_data_
+00002f40: 6f62 6a5f 7669 615f 6164 6420 3d20 6431  obj_via_add = d1
+00002f50: 202b 205b 2261 222c 207b 2269 6422 3a20   + ["a", {"id": 
+00002f60: 3132 337d 2c20 2263 225d 202b 2064 330a  123}, "c"] + d3.
+00002f70: 2020 2020 2020 2020 2320 596f 7520 6361          # You ca
+00002f80: 6e20 6a6f 696e 2063 7572 7265 6e74 2044  n join current D
+00002f90: 6174 6120 6f62 6a65 6374 206f 6e20 706c  ata object on pl
+00002fa0: 6163 6520 7573 696e 6720 2b3d 2e0a 2020  ace using +=..  
+00002fb0: 2020 2020 2020 2320 4974 2077 696c 6c20        # It will 
+00002fc0: 6b65 6570 2063 6163 6865 2073 7461 7475  keep cache statu
+00002fd0: 732e 0a20 2020 2020 2020 2064 3120 2b3d  s..        d1 +=
+00002fe0: 2064 3320 2023 2064 3120 7769 6c6c 2062   d3  # d1 will b
+00002ff0: 6563 6f6d 6520 4461 7461 285b 312c 322c  ecome Data([1,2,
+00003000: 332c 372c 382c 395d 290a 2020 2020 2020  3,7,8,9]).      
+00003010: 2020 0a20 2020 2020 2020 2023 205b 312e    .        # [1.
+00003020: 3132 5d20 4275 696c 6420 616e 6420 7265  12] Build and re
+00003030: 6164 2044 6174 6120 6f62 6a65 6374 2063  ad Data object c
+00003040: 6163 6865 2066 696c 6573 2e0a 2020 2020  ache files..    
+00003050: 2020 2020 6576 656e 7473 2e62 7569 6c64      events.build
+00003060: 5f63 6163 6865 2822 6361 6368 655f 6669  _cache("cache_fi
+00003070: 6c65 6e61 6d65 5f6f 725f 7061 7468 2229  lename_or_path")
+00003080: 0a20 2020 2020 2020 2064 6174 615f 6f62  .        data_ob
+00003090: 6a5f 6672 6f6d 5f63 6163 6865 203d 2044  j_from_cache = D
+000030a0: 6174 612e 6672 6f6d 5f63 6163 6865 5f66  ata.from_cache_f
+000030b0: 696c 6528 2263 6163 6865 5f66 696c 656e  ile("cache_filen
+000030c0: 616d 655f 6f72 5f70 6174 6822 290a 2020  ame_or_path").  
+000030d0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+000030e0: 205b 325d 2057 6f72 6b69 6e67 2077 6974   [2] Working wit
+000030f0: 6820 636f 6e76 6572 7465 7273 2e0a 2020  h converters..  
+00003100: 2020 2020 2020 2320 5468 6572 6520 6172        # There ar
+00003110: 6520 6375 7272 656e 746c 7920 7468 7265  e currently thre
+00003120: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+00003130: 7320 6f66 2049 5469 6d65 7374 616d 7043  s of ITimestampC
+00003140: 6f6e 7665 7274 6572 2063 6c61 7373 3a20  onverter class: 
+00003150: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
+00003160: 2c20 4461 7465 7469 6d65 5374 7269 6e67  , DatetimeString
+00003170: 436f 6e76 6572 7465 7220 616e 6420 5072  Converter and Pr
+00003180: 6f74 6f62 7566 5469 6d65 7374 616d 7043  otobufTimestampC
+00003190: 6f6e 7665 7274 6572 2e0a 2020 2020 2020  onverter..      
+000031a0: 2020 2320 5468 6579 2061 6c6c 2069 6d70    # They all imp
+000031b0: 6c65 6d65 6e74 2073 616d 6520 6d65 7468  lement same meth
+000031c0: 6f64 7320 6672 6f6d 2062 6173 6520 636c  ods from base cl
+000031d0: 6173 732e 0a20 2020 2020 2020 2023 204e  ass..        # N
+000031e0: 6f74 6520 7468 6174 2073 6f6d 6520 6163  ote that some ac
+000031f0: 6375 7261 6379 206d 6179 2062 6520 6c6f  curacy may be lo
+00003200: 7374 2064 7572 696e 6720 636f 6e76 6572  st during conver
+00003210: 7369 6f6e 2e0a 2020 2020 2020 2020 2320  sion..        # 
+00003220: 4966 2066 6f72 2065 7861 6d70 6c65 2079  If for example y
+00003230: 6f75 2075 7365 2074 6f5f 6d69 6372 6f73  ou use to_micros
+00003240: 6563 6f6e 6473 206e 616e 6f73 6563 6f6e  econds nanosecon
+00003250: 6473 2077 696c 6c20 6265 2063 7574 206f  ds will be cut o
+00003260: 6666 2069 6e73 7465 6164 206f 6620 726f  ff instead of ro
+00003270: 756e 6469 6e67 2e0a 2020 2020 2020 2020  unding..        
+00003280: 0a20 2020 2020 2020 2023 205b 322e 315d  .        # [2.1]
+00003290: 2044 6174 6574 696d 6543 6f6e 7665 7274   DatetimeConvert
+000032a0: 6572 2e0a 2020 2020 2020 2020 2320 4461  er..        # Da
+000032b0: 7465 7469 6d65 436f 6e76 6572 7465 7220  tetimeConverter 
+000032c0: 7461 6b65 7320 6461 7465 7469 6d65 2e64  takes datetime.d
+000032d0: 6174 6574 696d 6520 6f62 6a65 6374 2061  atetime object a
+000032e0: 7320 696e 7075 742e 0a20 2020 2020 2020  s input..       
+000032f0: 200a 2020 2020 2020 2020 6461 7465 7469   .        dateti
+00003300: 6d65 5f6f 626a 203d 2064 6174 6574 696d  me_obj = datetim
+00003310: 6528 7965 6172 3d32 3032 332c 206d 6f6e  e(year=2023, mon
+00003320: 7468 3d31 2c20 6461 793d 352c 2068 6f75  th=1, day=5, hou
+00003330: 723d 3134 2c20 6d69 6e75 7465 3d33 382c  r=14, minute=38,
+00003340: 2073 6563 6f6e 643d 3235 2c20 6d69 6372   second=25, micr
+00003350: 6f73 6563 6f6e 643d 3134 3630 290a 2020  osecond=1460).  
+00003360: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00003370: 2049 7420 6861 7320 6d65 7468 6f64 7320   It has methods 
+00003380: 7468 6174 2072 6574 7572 6e20 7468 6520  that return the 
+00003390: 6461 7465 7469 6d65 2069 6e20 6469 6666  datetime in diff
+000033a0: 6572 656e 7420 666f 726d 6173 3a0a 2020  erent formas:.  
+000033b0: 2020 2020 2020 0a20 2020 2020 2020 2064        .        d
+000033c0: 6174 655f 6d73 203d 2044 6174 6574 696d  ate_ms = Datetim
+000033d0: 6543 6f6e 7665 7274 6572 2e74 6f5f 6d69  eConverter.to_mi
+000033e0: 6c6c 6973 6563 6f6e 6473 2864 6174 6574  lliseconds(datet
+000033f0: 696d 655f 6f62 6a29 0a20 2020 2020 2020  ime_obj).       
+00003400: 2064 6174 655f 7573 203d 2044 6174 6574   date_us = Datet
+00003410: 696d 6543 6f6e 7665 7274 6572 2e74 6f5f  imeConverter.to_
+00003420: 6d69 6372 6f73 6563 6f6e 6473 2864 6174  microseconds(dat
+00003430: 6574 696d 655f 6f62 6a29 0a20 2020 2020  etime_obj).     
+00003440: 2020 2023 2043 6f6e 7665 7274 696e 6720     # Converting 
+00003450: 746f 206e 616e 6f73 6563 6f6e 6473 206a  to nanoseconds j
+00003460: 7573 7473 2061 6464 7320 7468 7265 6520  usts adds three 
+00003470: 7472 6169 6c69 6e67 207a 6572 6f73 2061  trailing zeros a
+00003480: 7320 6461 7465 7469 6d65 206f 626a 6563  s datetime objec
+00003490: 7420 646f 6573 6e27 7420 6861 7665 206e  t doesn't have n
+000034a0: 616e 6f73 6563 6f6e 6473 2e0a 2020 2020  anoseconds..    
+000034b0: 2020 2020 6461 7465 5f6e 7320 3d20 4461      date_ns = Da
+000034c0: 7465 7469 6d65 436f 6e76 6572 7465 722e  tetimeConverter.
+000034d0: 746f 5f6e 616e 6f73 6563 6f6e 6473 2864  to_nanoseconds(d
+000034e0: 6174 6574 696d 655f 6f62 6a29 0a20 2020  atetime_obj).   
+000034f0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00003500: 5b32 2e32 5d20 4461 7465 7469 6d65 5374  [2.2] DatetimeSt
+00003510: 7269 6e67 436f 6e76 6572 7465 720a 2020  ringConverter.  
+00003520: 2020 2020 2020 2320 4461 7465 7469 6d65        # Datetime
+00003530: 5374 7269 6e67 436f 6e76 6572 7465 7220  StringConverter 
+00003540: 7461 6b65 7320 7374 7269 6e67 2069 6e20  takes string in 
+00003550: 2279 7979 792d 4d4d 2d64 6454 4848 3a6d  "yyyy-MM-ddTHH:m
+00003560: 6d3a 7373 5b2e 5353 5353 5353 5353 535d  m:ss[.SSSSSSSSS]
+00003570: 5a22 2066 6f72 6d61 742e 0a20 2020 2020  Z" format..     
+00003580: 2020 200a 2020 2020 2020 2020 6461 7465     .        date
+00003590: 5f73 7472 696e 6720 3d20 2232 3032 332d  _string = "2023-
+000035a0: 3031 2d30 3554 3134 3a33 383a 3235 2e30  01-05T14:38:25.0
+000035b0: 3031 3436 5a22 0a20 2020 2020 2020 200a  0146Z".        .
+000035c0: 2020 2020 2020 2020 2320 5765 2068 6176          # We hav
+000035d0: 6520 7361 6d65 206d 6574 686f 6473 2061  e same methods a
+000035e0: 7320 696e 2044 6174 6574 696d 6543 6f6e  s in DatetimeCon
+000035f0: 7665 7274 6572 0a20 2020 2020 2020 2064  verter.        d
+00003600: 6174 655f 6d73 5f66 726f 6d5f 7374 7269  ate_ms_from_stri
+00003610: 6e67 203d 2044 6174 6574 696d 6553 7472  ng = DatetimeStr
+00003620: 696e 6743 6f6e 7665 7274 6572 2e74 6f5f  ingConverter.to_
+00003630: 6d69 6c6c 6973 6563 6f6e 6473 2864 6174  milliseconds(dat
+00003640: 655f 7374 7269 6e67 290a 2020 2020 2020  e_string).      
+00003650: 2020 6461 7465 5f75 735f 6672 6f6d 5f73    date_us_from_s
+00003660: 7472 696e 6720 3d20 4461 7465 7469 6d65  tring = Datetime
+00003670: 5374 7269 6e67 436f 6e76 6572 7465 722e  StringConverter.
+00003680: 746f 5f6d 6963 726f 7365 636f 6e64 7328  to_microseconds(
+00003690: 6461 7465 5f73 7472 696e 6729 0a20 2020  date_string).   
+000036a0: 2020 2020 2064 6174 655f 6e73 5f66 726f       date_ns_fro
+000036b0: 6d5f 7374 7269 6e67 203d 2044 6174 6574  m_string = Datet
+000036c0: 696d 6553 7472 696e 6743 6f6e 7665 7274  imeStringConvert
+000036d0: 6572 2e74 6f5f 6e61 6e6f 7365 636f 6e64  er.to_nanosecond
+000036e0: 7328 6461 7465 5f73 7472 696e 6729 0a20  s(date_string). 
+000036f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003700: 2320 5765 2063 616e 2061 6c73 6f20 6765  # We can also ge
+00003710: 7420 6461 7465 7469 6d65 206f 626a 6563  t datetime objec
+00003720: 7420 6672 6f6d 2073 7472 696e 670a 2020  t from string.  
+00003730: 2020 2020 2020 6461 7465 7469 6d65 5f66        datetime_f
+00003740: 726f 6d5f 7374 7269 6e67 203d 2044 6174  rom_string = Dat
+00003750: 6574 696d 6553 7472 696e 6743 6f6e 7665  etimeStringConve
+00003760: 7274 6572 2e74 6f5f 6461 7465 7469 6d65  rter.to_datetime
+00003770: 2864 6174 655f 7374 7269 6e67 290a 2020  (date_string).  
+00003780: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00003790: 205b 322e 335d 2050 726f 746f 6275 6654   [2.3] ProtobufT
+000037a0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
+000037b0: 720a 2020 2020 2020 2020 2320 5072 6f74  r.        # Prot
+000037c0: 6f62 7566 2074 696d 6573 7461 6d70 7320  obuf timestamps 
+000037d0: 6d75 7374 2062 6520 696e 2066 6f72 6d20  must be in form 
+000037e0: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
+000037f0: 7365 636f 6e64 732c 2022 6e61 6e6f 223a  seconds, "nano":
+00003800: 206e 616e 6f73 6563 6f6e 6473 7d0a 2020   nanoseconds}.  
+00003810: 2020 2020 2020 0a20 2020 2020 2020 2070        .        p
+00003820: 726f 746f 6275 665f 7469 6d65 7374 616d  rotobuf_timestam
+00003830: 7020 3d20 7b22 6570 6f63 6853 6563 6f6e  p = {"epochSecon
+00003840: 6422 3a20 3136 3732 3932 3935 3035 2c20  d": 1672929505, 
+00003850: 226e 616e 6f22 3a20 315f 3436 305f 3030  "nano": 1_460_00
+00003860: 307d 0a20 2020 2020 2020 200a 2020 2020  0}.        .    
+00003870: 2020 2020 6461 7465 5f6d 735f 6672 6f6d      date_ms_from
+00003880: 5f74 696d 6573 7461 6d70 203d 2050 726f  _timestamp = Pro
+00003890: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
+000038a0: 6e76 6572 7465 722e 746f 5f6d 696c 6c69  nverter.to_milli
+000038b0: 7365 636f 6e64 7328 7072 6f74 6f62 7566  seconds(protobuf
+000038c0: 5f74 696d 6573 7461 6d70 290a 2020 2020  _timestamp).    
+000038d0: 2020 2020 6461 7465 5f75 735f 6672 6f6d      date_us_from
+000038e0: 5f74 696d 6573 7461 6d70 203d 2050 726f  _timestamp = Pro
+000038f0: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
+00003900: 6e76 6572 7465 722e 746f 5f6d 6963 726f  nverter.to_micro
+00003910: 7365 636f 6e64 7328 7072 6f74 6f62 7566  seconds(protobuf
+00003920: 5f74 696d 6573 7461 6d70 290a 2020 2020  _timestamp).    
+00003930: 2020 2020 6461 7465 5f6e 735f 6672 6f6d      date_ns_from
+00003940: 5f74 696d 6573 7461 6d70 203d 2050 726f  _timestamp = Pro
+00003950: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
+00003960: 6e76 6572 7465 722e 746f 5f6e 616e 6f73  nverter.to_nanos
+00003970: 6563 6f6e 6473 2870 726f 746f 6275 665f  econds(protobuf_
+00003980: 7469 6d65 7374 616d 7029 0a20 2020 2020  timestamp).     
+00003990: 2020 2064 6174 6574 696d 655f 6672 6f6d     datetime_from
+000039a0: 5f74 696d 6573 7461 6d70 203d 2050 726f  _timestamp = Pro
+000039b0: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
+000039c0: 6e76 6572 7465 722e 746f 5f64 6174 6574  nverter.to_datet
+000039d0: 696d 6528 7072 6f74 6f62 7566 5f74 696d  ime(protobuf_tim
+000039e0: 6573 7461 6d70 290a 2020 2020 2020 2020  estamp).        
+000039f0: 0a20 2020 2020 2020 2023 205b 335d 2057  .        # [3] W
+00003a00: 6f72 6b69 6e67 2077 6974 6820 4576 656e  orking with Even
+00003a10: 7454 7265 6520 616e 6420 4576 656e 7454  tTree and EventT
+00003a20: 7265 6543 6f6c 6c65 6374 696f 6e2e 0a20  reeCollection.. 
+00003a30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003a40: 2320 5b33 2e31 5d20 4275 696c 6420 6120  # [3.1] Build a 
+00003a50: 6375 7374 6f6d 2045 7665 6e74 5472 6565  custom EventTree
+00003a60: 0a20 2020 2020 2020 2023 2054 6f20 6372  .        # To cr
+00003a70: 6561 7465 2061 6e20 4576 656e 7454 7265  eate an EventTre
+00003a80: 6520 6f62 6a65 6374 2079 6f75 206e 6565  e object you nee
+00003a90: 6420 746f 2070 726f 7669 6465 206e 616d  d to provide nam
+00003aa0: 652c 2069 6420 616e 6420 6461 7461 206f  e, id and data o
+00003ab0: 6620 7468 6520 726f 6f74 2065 7665 6e74  f the root event
+00003ac0: 2e0a 2020 2020 2020 2020 7472 6565 203d  ..        tree =
+00003ad0: 2045 7665 6e74 5472 6565 2865 7665 6e74   EventTree(event
+00003ae0: 5f6e 616d 653d 2272 6f6f 7420 6576 656e  _name="root even
+00003af0: 7422 2c20 6576 656e 745f 6964 3d22 726f  t", event_id="ro
+00003b00: 6f74 5f69 6422 2c20 6461 7461 3d7b 2264  ot_id", data={"d
+00003b10: 6174 6122 3a20 5b31 2c20 322c 2033 2c20  ata": [1, 2, 3, 
+00003b20: 342c 2035 5d7d 290a 2020 2020 2020 2020  4, 5]}).        
+00003b30: 0a20 2020 2020 2020 2023 2054 6f20 6164  .        # To ad
+00003b40: 6420 6e65 7720 6e6f 6465 2075 7365 2061  d new node use a
+00003b50: 7070 656e 645f 6576 656e 742e 2070 6172  ppend_event. par
+00003b60: 656e 745f 6964 2069 7320 6e65 6365 7373  ent_id is necess
+00003b70: 6172 792c 2064 6174 6120 6973 206f 7074  ary, data is opt
+00003b80: 696f 6e61 6c2e 0a20 2020 2020 2020 2074  ional..        t
+00003b90: 7265 652e 6170 7065 6e64 5f65 7665 6e74  ree.append_event
+00003ba0: 2865 7665 6e74 5f6e 616d 653d 2241 222c  (event_name="A",
+00003bb0: 2065 7665 6e74 5f69 643d 2241 5f69 6422   event_id="A_id"
+00003bc0: 2c20 6461 7461 3d4e 6f6e 652c 2070 6172  , data=None, par
+00003bd0: 656e 745f 6964 3d22 726f 6f74 5f69 6422  ent_id="root_id"
+00003be0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00003bf0: 2020 2023 205b 332e 335d 2042 7569 6c64     # [3.3] Build
+00003c00: 696e 6720 7468 6520 4576 656e 7454 7265  ing the EventTre
+00003c10: 6543 6f6c 6c65 6374 696f 6e2e 0a20 2020  eCollection..   
+00003c20: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00003c30: 4966 2079 6f75 2064 6f6e 2774 2073 7065  If you don't spe
+00003c40: 6369 6679 2064 6174 615f 736f 7572 6365  cify data_source
+00003c50: 2066 6f72 2074 6865 2064 7269 7665 7220   for the driver 
+00003c60: 7468 656e 2069 7420 776f 6e27 7420 7265  then it won't re
+00003c70: 636f 7665 7220 6465 7461 6368 6564 2065  cover detached e
+00003c80: 7665 6e74 732e 0a20 2020 2020 2020 2064  vents..        d
+00003c90: 7269 7665 723a 2049 4554 4344 7269 7665  river: IETCDrive
+00003ca0: 7220 2023 2059 6f75 2073 686f 756c 6420  r  # You should 
+00003cb0: 696e 6974 2045 5443 4472 6976 6572 206f  init ETCDriver o
+00003cc0: 626a 6563 742e 2045 2e67 2e20 6672 6f6d  bject. E.g. from
+00003cd0: 204c 7744 5020 6d6f 6475 6c65 206f 7220   LwDP module or 
+00003ce0: 796f 7572 2063 7573 746f 6d20 636c 6173  your custom clas
+00003cf0: 732e 0a20 2020 2020 2020 2065 7463 203d  s..        etc =
+00003d00: 2045 7665 6e74 5472 6565 436f 6c6c 6563   EventTreeCollec
+00003d10: 7469 6f6e 2864 7269 7665 7229 0a20 2020  tion(driver).   
+00003d20: 2020 2020 2065 7463 2e62 7569 6c64 2865       etc.build(e
+00003d30: 7665 6e74 7329 0a20 2020 2020 2020 200a  vents).        .
+00003d40: 2020 2020 2020 2020 2320 4465 7461 6368          # Detach
+00003d50: 6564 2065 7665 6e74 7320 6973 6e27 7420  ed events isn't 
+00003d60: 656d 7074 792e 0a20 2020 2020 2020 2061  empty..        a
+00003d70: 7373 6572 7420 6574 632e 6765 745f 6465  ssert etc.get_de
+00003d80: 7461 6368 6564 5f65 7665 6e74 7328 290a  tached_events().
+00003d90: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003da0: 2065 7463 203d 2045 7665 6e74 5472 6565   etc = EventTree
+00003db0: 436f 6c6c 6563 7469 6f6e 2864 7269 7665  Collection(drive
+00003dc0: 7229 0a20 2020 2020 2020 2023 2044 6574  r).        # Det
+00003dd0: 6163 6865 6420 6576 656e 7473 2061 7265  ached events are
+00003de0: 2065 6d70 7479 2062 6563 6175 7365 2074   empty because t
+00003df0: 6865 7920 7765 7265 2072 6563 6f76 6572  hey were recover
+00003e00: 6564 2e0a 2020 2020 2020 2020 6173 7365  ed..        asse
+00003e10: 7274 206e 6f74 2065 7463 2e67 6574 5f64  rt not etc.get_d
+00003e20: 6574 6163 6865 645f 6576 656e 7473 2829  etached_events()
+00003e30: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00003e40: 2020 2320 5468 6520 636f 6c6c 6563 7469    # The collecti
+00003e50: 6f6e 2068 6173 2045 7665 6e74 5472 6565  on has EventTree
+00003e60: 7320 6561 6368 2077 6974 6820 6120 7472  s each with a tr
+00003e70: 6565 206f 6620 6576 656e 7473 2e0a 2020  ee of events..  
+00003e80: 2020 2020 2020 2320 5573 696e 6720 436f        # Using Co
+00003e90: 6c6c 6563 7469 6f6e 2061 6e64 2045 7665  llection and Eve
+00003ea0: 6e74 5472 6565 732c 2079 6f75 2063 616e  ntTrees, you can
+00003eb0: 2077 6f72 6b20 666c 6578 6962 6c79 2077   work flexibly w
+00003ec0: 6974 6820 6576 656e 7473 2e0a 2020 2020  ith events..    
 00003ed0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-00003ee0: 332e 332e 325d 2047 6574 2072 6f6f 7473  3.3.2] Get roots
-00003ef0: 2069 6473 206f 6620 616c 6c20 7472 6565   ids of all tree
-00003f00: 732e 0a20 2020 2020 2020 2072 6f6f 7473  s..        roots
-00003f10: 3a20 4c69 7374 5b73 7472 5d20 3d20 6574  : List[str] = et
-00003f20: 632e 6765 745f 726f 6f74 735f 6964 7328  c.get_roots_ids(
-00003f30: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00003f40: 2020 2023 205b 332e 332e 335d 2046 696e     # [3.3.3] Fin
-00003f50: 6420 616e 2065 7665 6e74 2069 6e20 616c  d an event in al
-00003f60: 6c20 7472 6565 732e 0a20 2020 2020 2020  l trees..       
-00003f70: 2066 696e 645f 6576 656e 743a 204f 7074   find_event: Opt
-00003f80: 696f 6e61 6c5b 6469 6374 5d20 3d20 6574  ional[dict] = et
-00003f90: 632e 6669 6e64 286c 616d 6264 6120 6576  c.find(lambda ev
-00003fa0: 656e 743a 2022 5365 6e64 206d 6573 7361  ent: "Send messa
-00003fb0: 6765 2220 696e 2065 7665 6e74 5b22 6576  ge" in event["ev
-00003fc0: 656e 7454 7970 6522 5d29 0a20 2020 2020  entType"]).     
-00003fd0: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
-00003fe0: 2e33 2e34 5d20 4669 6e64 2061 6c6c 2065  .3.4] Find all e
-00003ff0: 7665 6e74 7320 696e 2061 6c6c 2074 7265  vents in all tre
-00004000: 6573 2e20 5468 6572 6520 6973 2061 6c73  es. There is als
-00004010: 6f20 6974 6572 6162 6c65 2076 6572 7369  o iterable versi
-00004020: 6f6e 2027 6669 6e64 616c 6c5f 6974 6572  on 'findall_iter
-00004030: 272e 0a20 2020 2020 2020 2066 696e 645f  '..        find_
-00004040: 6576 656e 7473 3a20 4c69 7374 5b64 6963  events: List[dic
-00004050: 745d 203d 2065 7463 2e66 696e 6461 6c6c  t] = etc.findall
-00004060: 286c 616d 6264 6120 6576 656e 743a 2065  (lambda event: e
-00004070: 7665 6e74 5b22 7375 6363 6573 7366 756c  vent["successful
-00004080: 225d 2069 7320 5472 7565 290a 2020 2020  "] is True).    
-00004090: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-000040a0: 332e 332e 355d 2046 696e 6420 616e 2061  3.3.5] Find an a
-000040b0: 6e63 6573 746f 7220 6f66 2074 6865 2065  ncestor of the e
-000040c0: 7665 6e74 2e0a 2020 2020 2020 2020 616e  vent..        an
-000040d0: 6365 7374 6f72 3a20 4f70 7469 6f6e 616c  cestor: Optional
-000040e0: 5b64 6963 745d 203d 2065 7463 2e66 696e  [dict] = etc.fin
-000040f0: 645f 616e 6365 7374 6f72 280a 2020 2020  d_ancestor(.    
-00004100: 2020 2020 2020 2020 2238 6262 6533 3731          "8bbe371
-00004110: 372d 6366 3539 2d31 3165 622d 6133 6637  7-cf59-11eb-a3f7
-00004120: 2d30 3934 6639 3034 6333 6136 3222 2c20  -094f904c3a62", 
-00004130: 6669 6c74 6572 3d6c 616d 6264 6120 6576  filter=lambda ev
-00004140: 656e 743a 2022 526f 6f74 4576 656e 7422  ent: "RootEvent"
-00004150: 2069 6e20 6576 656e 745b 2265 7665 6e74   in event["event
-00004160: 4e61 6d65 225d 0a20 2020 2020 2020 2029  Name"].        )
-00004170: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004180: 2020 2320 5b33 2e33 2e36 5d20 4765 7420    # [3.3.6] Get 
-00004190: 6368 696c 6472 656e 206f 6620 7468 6520  children of the 
-000041a0: 6576 656e 742e 2054 6865 7265 2069 7320  event. There is 
-000041b0: 616c 736f 2069 7465 7261 626c 6520 7665  also iterable ve
-000041c0: 7273 696f 6e20 2767 6574 5f63 6869 6c64  rsion 'get_child
-000041d0: 7265 6e5f 6974 6572 272e 0a20 2020 2020  ren_iter'..     
-000041e0: 2020 2063 6869 6c64 7265 6e3a 2054 7570     children: Tup
-000041f0: 6c65 5b64 6963 745d 203d 2065 7463 2e67  le[dict] = etc.g
-00004200: 6574 5f63 6869 6c64 7265 6e28 2238 3134  et_children("814
-00004210: 3432 3265 312d 3963 3638 2d31 3165 622d  422e1-9c68-11eb-
-00004220: 3835 3938 2d36 3931 6562 6437 6634 3133  8598-691ebd7f413
-00004230: 6422 290a 2020 2020 2020 2020 0a20 2020  d").        .   
-00004240: 2020 2020 2023 205b 332e 332e 375d 2047       # [3.3.7] G
-00004250: 6574 2073 7562 7472 6565 2066 6f72 2073  et subtree for s
-00004260: 7065 6369 6669 6564 2065 7665 6e74 2e0a  pecified event..
-00004270: 2020 2020 2020 2020 7375 6274 7265 653a          subtree:
-00004280: 2045 7665 6e74 5472 6565 203d 2065 7463   EventTree = etc
-00004290: 2e67 6574 5f73 7562 7472 6565 2822 3865  .get_subtree("8e
-000042a0: 3233 3737 3464 2d63 6635 392d 3131 6562  23774d-cf59-11eb
-000042b0: 2d61 3665 332d 3535 6266 6462 3262 3366  -a6e3-55bfdb2b3f
-000042c0: 3231 2229 0a20 2020 2020 2020 200a 2020  21").        .  
-000042d0: 2020 2020 2020 2320 5b33 2e33 2e38 5d20        # [3.3.8] 
-000042e0: 4765 7420 6675 6c6c 2070 6174 6820 746f  Get full path to
-000042f0: 2074 6865 2065 7665 6e74 2e0a 2020 2020   the event..    
-00004300: 2020 2020 2320 4c6f 6f6b 7320 6c69 6b65      # Looks like
-00004310: 205b 616e 6365 7374 6f72 5f72 6f6f 742c   [ancestor_root,
-00004320: 2061 6e63 6573 746f 725f 6c65 7665 6c31   ancestor_level1
-00004330: 2c20 616e 6365 7374 6f72 5f6c 6576 656c  , ancestor_level
-00004340: 322c 2065 7665 6e74 5d0a 2020 2020 2020  2, event].      
-00004350: 2020 6576 656e 745f 7061 7468 3a20 4c69    event_path: Li
-00004360: 7374 5b64 6963 745d 203d 2065 7463 2e67  st[dict] = etc.g
-00004370: 6574 5f66 756c 6c5f 7061 7468 2822 3865  et_full_path("8e
-00004380: 3235 3234 6661 2d63 6635 392d 3131 6562  2524fa-cf59-11eb
-00004390: 2d61 3366 372d 3039 3466 3930 3463 3361  -a3f7-094f904c3a
-000043a0: 3632 2229 0a20 2020 2020 2020 200a 2020  62").        .  
-000043b0: 2020 2020 2020 2320 5b33 2e33 2e39 5d20        # [3.3.9] 
-000043c0: 4765 7420 7061 7265 6e74 206f 6620 7468  Get parent of th
-000043d0: 6520 6576 656e 742e 0a20 2020 2020 2020  e event..       
-000043e0: 2070 6172 656e 7420 3d20 6574 632e 6765   parent = etc.ge
-000043f0: 745f 7061 7265 6e74 2822 3865 3235 3234  t_parent("8e2524
-00004400: 6661 2d63 6635 392d 3131 6562 2d61 3366  fa-cf59-11eb-a3f
-00004410: 372d 3039 3466 3930 3463 3361 3632 2229  7-094f904c3a62")
-00004420: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004430: 2020 2320 5b33 2e33 2e31 305d 2041 7070    # [3.3.10] App
-00004440: 656e 6420 6e65 7720 6576 656e 7420 746f  end new event to
-00004450: 2074 6865 2063 6f6c 6c65 6374 696f 6e2e   the collection.
-00004460: 0a20 2020 2020 2020 2065 7463 2e61 7070  .        etc.app
-00004470: 656e 645f 6576 656e 7428 0a20 2020 2020  end_event(.     
-00004480: 2020 2020 2020 2065 7665 6e74 3d7b 0a20         event={. 
-00004490: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000044a0: 6576 656e 7449 6422 3a20 2261 3230 6635  eventId": "a20f5
-000044b0: 6566 342d 6333 6665 2d62 6231 302d 6132  ef4-c3fe-bb10-a2
-000044c0: 3963 2d64 6433 6437 3834 3930 3965 6222  9c-dd3d784909eb"
-000044d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000044e0: 2020 2270 6172 656e 7445 7665 6e74 4964    "parentEventId
-000044f0: 223a 2022 3865 3235 3234 6661 2d63 6635  ": "8e2524fa-cf5
-00004500: 392d 3131 6562 2d61 3366 372d 3039 3466  9-11eb-a3f7-094f
-00004510: 3930 3463 3361 3632 222c 0a20 2020 2020  904c3a62",.     
-00004520: 2020 2020 2020 2020 2020 2022 6576 656e             "even
-00004530: 744e 616d 6522 3a20 2253 7475 6245 7665  tName": "StubEve
-00004540: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
-00004550: 207d 0a20 2020 2020 2020 2029 0a20 2020   }.        ).   
-00004560: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-00004570: 5b33 2e33 2e31 315d 2053 686f 7720 7468  [3.3.11] Show th
-00004580: 6520 656e 7469 7265 2063 6f6c 6c65 6374  e entire collect
-00004590: 696f 6e2e 0a20 2020 2020 2020 2065 7463  ion..        etc
-000045a0: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
-000045b0: 0a20 2020 2020 2020 2023 205b 332e 345d  .        # [3.4]
-000045c0: 2057 6f72 6b69 6e67 2077 6974 6820 7468   Working with th
-000045d0: 6520 4576 656e 7454 7265 652e 0a20 2020  e EventTree..   
-000045e0: 2020 2020 2023 2045 7665 6e74 5472 6565       # EventTree
-000045f0: 2068 6173 2074 6865 2073 616d 6520 6d65   has the same me
-00004600: 7468 6f64 7320 6173 2045 7665 6e74 5472  thods as EventTr
-00004610: 6565 436f 6c6c 6563 7469 6f6e 2c20 6275  eeCollection, bu
-00004620: 7420 6f6e 6c79 2066 6f72 2069 7473 206f  t only for its o
-00004630: 776e 2074 7265 652e 0a20 2020 2020 2020  wn tree..       
-00004640: 200a 2020 2020 2020 2020 2320 5b33 2e34   .        # [3.4
-00004650: 2e31 5d20 4765 7420 636f 6c6c 6563 7469  .1] Get collecti
-00004660: 6f6e 2074 7265 6573 2e0a 2020 2020 2020  on trees..      
-00004670: 2020 7472 6565 733a 204c 6973 745b 4576    trees: List[Ev
-00004680: 656e 7454 7265 655d 203d 2065 7463 2e67  entTree] = etc.g
-00004690: 6574 5f74 7265 6573 2829 0a20 2020 2020  et_trees().     
-000046a0: 2020 2074 7265 653a 2045 7665 6e74 5472     tree: EventTr
-000046b0: 6565 203d 2074 7265 6573 5b30 5d0a 2020  ee = trees[0].  
-000046c0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000046d0: 2042 7574 2045 7665 6e74 5472 6565 2070   But EventTree p
-000046e0: 726f 7669 6465 7320 6120 776f 726b 2077  rovides a work w
-000046f0: 6974 6820 7468 6520 7472 6565 2c20 6275  ith the tree, bu
-00004700: 7420 646f 6573 206e 6f74 206d 6f64 6966  t does not modif
-00004710: 7920 6974 2e0a 2020 2020 2020 2020 2320  y it..        # 
-00004720: 4966 2079 6f75 2077 616e 7420 746f 206d  If you want to m
-00004730: 6f64 6966 7920 7468 6520 7472 6565 2c20  odify the tree, 
-00004740: 7573 6520 4576 656e 7454 7265 6543 6f6c  use EventTreeCol
-00004750: 6c65 6374 696f 6e73 2e0a 2020 2020 2020  lections..      
-00004760: 2020 0a20 2020 2020 2020 2023 205b 332e    .        # [3.
-00004770: 355d 2057 6f72 6b69 6e67 2077 6974 6820  5] Working with 
-00004780: 5061 7265 6e74 6c65 7373 5472 6565 2e0a  ParentlessTree..
-00004790: 2020 2020 2020 2020 2320 5061 7265 6e74          # Parent
-000047a0: 6c65 7373 5472 6565 2069 7320 4576 656e  lessTree is Even
-000047b0: 7454 7265 6520 7768 6963 6820 6861 7320  tTree which has 
-000047c0: 6465 7461 6368 6564 2065 7665 6e74 7320  detached events 
-000047d0: 7769 7468 2073 7475 6273 2e0a 2020 2020  with stubs..    
-000047e0: 2020 2020 7061 7265 6e74 6c65 7373 5f74      parentless_t
-000047f0: 7265 6573 3a20 4c69 7374 5b45 7665 6e74  rees: List[Event
-00004800: 5472 6565 5d20 3d20 6574 632e 6765 745f  Tree] = etc.get_
-00004810: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
-00004820: 2829 0a20 2020 2020 2020 200a 2020 2020  ().        .    
-00004830: 2020 2020 2320 5b33 2e36 5d20 576f 726b      # [3.6] Work
-00004840: 696e 6720 7769 7468 2050 6172 656e 7445  ing with ParentE
-00004850: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
-00004860: 6f6e 2e0a 2020 2020 2020 2020 2320 5061  on..        # Pa
-00004870: 7265 6e74 4576 656e 7454 7265 6543 6f6c  rentEventTreeCol
-00004880: 6c65 6374 696f 6e20 6973 2061 2074 7265  lection is a tre
-00004890: 6520 636f 6c6c 6563 7469 6f6e 206c 696b  e collection lik
-000048a0: 6520 4576 656e 7454 7265 6543 6f6c 6c65  e EventTreeColle
-000048b0: 6374 696f 6e2c 0a20 2020 2020 2020 2023  ction,.        #
-000048c0: 2062 7574 2069 7420 6861 7320 6f6e 6c79   but it has only
-000048d0: 2065 7665 6e74 7320 7468 6174 2068 6176   events that hav
-000048e0: 6520 7265 6665 7265 6e63 6573 2e0a 2020  e references..  
-000048f0: 2020 2020 2020 6461 7461 5f73 6f75 7263        data_sourc
-00004900: 653a 2049 4461 7461 536f 7572 6365 2020  e: IDataSource  
-00004910: 2320 596f 7520 7368 6f75 6c64 2069 6e69  # You should ini
-00004920: 7420 4461 7461 536f 7572 6365 206f 626a  t DataSource obj
-00004930: 6563 742e 2045 2e67 2e20 6672 6f6d 204c  ect. E.g. from L
-00004940: 7744 5020 6d6f 6475 6c65 2e0a 2020 2020  wDP module..    
-00004950: 2020 2020 2320 4554 4344 7269 7665 7220      # ETCDriver 
-00004960: 6865 7265 2069 7320 6120 7374 7562 2c20  here is a stub, 
-00004970: 6163 7475 616c 6c79 2074 6865 206c 6962  actually the lib
-00004980: 2064 6f6e 2774 2068 6176 6520 7375 6368   don't have such
-00004990: 2063 6c61 7373 2e0a 2020 2020 2020 2020   class..        
-000049a0: 2320 596f 7520 6361 6e20 7461 6b65 2069  # You can take i
-000049b0: 7420 696e 204c 7744 5020 6d6f 6475 6c65  t in LwDP module
-000049c0: 206f 7220 6372 6561 7465 2079 6f75 7273   or create yours
-000049d0: 656c 6620 636c 6173 7320 6966 2079 6f75  elf class if you
-000049e0: 2068 6176 6520 736f 6d65 2073 7065 6369   have some speci
-000049f0: 616c 2065 7665 6e74 7320 7374 7275 6374  al events struct
-00004a00: 7572 652e 0a20 2020 2020 2020 2064 7269  ure..        dri
-00004a10: 7665 7220 3d20 4554 4344 7269 7665 7228  ver = ETCDriver(
-00004a20: 6461 7461 5f73 6f75 7263 653d 6461 7461  data_source=data
-00004a30: 5f73 6f75 7263 6529 0a20 2020 2020 2020  _source).       
-00004a40: 2065 7463 203d 2050 6172 656e 7445 7665   etc = ParentEve
-00004a50: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
-00004a60: 2864 7269 7665 7229 0a20 2020 2020 2020  (driver).       
-00004a70: 2065 7463 2e62 7569 6c64 2865 7665 6e74   etc.build(event
-00004a80: 7329 0a20 2020 2020 2020 200a 2020 2020  s).        .    
-00004a90: 2020 2020 6574 632e 7368 6f77 2829 0a20      etc.show(). 
-00004aa0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00004ab0: 2020 203c 212d 2d20 656e 6420 6765 745f     <!-- end get_
-00004ac0: 7374 6172 7465 645f 6578 616d 706c 652e  started_example.
-00004ad0: 7079 202d 2d3e 0a20 2020 2020 2020 200a  py -->.        .
-00004ae0: 2020 2020 2020 2020 2323 2032 2e33 2e20          ## 2.3. 
-00004af0: 5368 6f72 7420 7468 656f 7279 0a20 2020  Short theory.   
-00004b00: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
-00004b10: 6520 6c69 6272 6172 7920 7072 6f76 6964  e library provid
-00004b20: 6573 2074 6f6f 6c73 2066 6f72 2068 616e  es tools for han
-00004b30: 646c 696e 6720 7374 7265 616d 2064 6174  dling stream dat
-00004b40: 612e 2057 6861 7427 7320 6120 7374 7265  a. What's a stre
-00004b50: 616d 3f20 4974 2773 2061 2073 6571 7565  am? It's a seque
-00004b60: 6e63 6520 6f66 2065 6c65 6d65 6e74 7320  nce of elements 
-00004b70: 6672 6f6d 2061 2073 6f75 7263 6520 7468  from a source th
-00004b80: 6174 0a20 2020 2020 2020 2073 7570 706f  at.        suppo
-00004b90: 7274 7320 6167 6772 6567 6174 6520 6f70  rts aggregate op
-00004ba0: 6572 6174 696f 6e73 2e0a 2020 2020 2020  erations..      
-00004bb0: 2020 0a20 2020 2020 2020 2023 2323 2054    .        ### T
-00004bc0: 6572 6d73 0a20 2020 2020 2020 200a 2020  erms.        .  
-00004bd0: 2020 2020 2020 2d20 2a2a 4461 7461 206f        - **Data o
-00004be0: 626a 6563 742a 2a3a 2041 6e20 696e 7374  bject**: An inst
-00004bf0: 616e 6365 206f 6620 6044 6174 6160 2063  ance of `Data` c
-00004c00: 6c61 7373 2077 6869 6368 2069 7320 7772  lass which is wr
-00004c10: 6170 7065 7220 756e 6465 7220 7374 7265  apper under stre
-00004c20: 616d 2e0a 2020 2020 2020 2020 2d20 2a2a  am..        - **
-00004c30: 5365 7175 656e 6365 206f 6620 656c 656d  Sequence of elem
-00004c40: 656e 7473 2a2a 3a0a 2020 2020 2020 2020  ents**:.        
-00004c50: 2020 4120 5f44 6174 6120 6f62 6a65 6374    A _Data object
-00004c60: 5f20 7072 6f76 6964 6573 2061 6e20 696e  _ provides an in
-00004c70: 7465 7266 6163 6520 746f 2061 2073 6571  terface to a seq
-00004c80: 7565 6e63 6564 2073 6574 206f 6620 7661  uenced set of va
-00004c90: 6c75 6573 206f 6620 6120 7370 6563 6966  lues of a specif
-00004ca0: 6963 2065 6c65 6d65 6e74 2074 7970 652e  ic element type.
-00004cb0: 2053 7472 6561 6d20 696e 7369 6465 2074   Stream inside t
-00004cc0: 6865 205f 4461 7461 0a20 2020 2020 2020  he _Data.       
-00004cd0: 2020 206f 626a 6563 745f 202a 2a64 6f6e     object_ **don
-00004ce0: 1974 2061 6374 7561 6c6c 7920 7374 6f72  .t actually stor
-00004cf0: 652a 2a20 656c 656d 656e 7473 3b20 7468  e** elements; th
-00004d00: 6579 2061 7265 2063 6f6d 7075 7465 6420  ey are computed 
-00004d10: 6f6e 2064 656d 616e 642e 0a20 2020 2020  on demand..     
-00004d20: 2020 202d 202a 2a64 6174 6120 736f 7572     - **data sour
-00004d30: 6365 2a2a 2028 6578 6163 746c 7920 696e  ce** (exactly in
-00004d40: 2073 6d61 6c6c 206c 6574 7465 7273 293a   small letters):
-00004d50: 0a20 2020 2020 2020 2020 2041 6e79 2073  .          Any s
-00004d60: 6f75 7263 6520 6f66 2064 6174 612e 2045  ource of data. E
-00004d70: 2e67 2e20 5b4c 6967 6874 7765 6967 6874  .g. [Lightweight
-00004d80: 2044 6174 6120 5072 6f76 6964 6572 5d28   Data Provider](
-00004d90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00004da0: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d6c  om/th2-net/th2-l
-00004db0: 772d 6461 7461 2d70 726f 7669 6465 7229  w-data-provider)
-00004dc0: 2c20 636f 6c6c 6563 7469 6f6e 732c 0a20  , collections,. 
-00004dd0: 2020 2020 2020 2020 2061 7272 6179 732c           arrays,
-00004de0: 206f 7220 492f 4f20 7265 736f 7572 6365   or I/O resource
-00004df0: 732e 0a20 2020 2020 2020 202d 202a 2a44  s..        - **D
-00004e00: 6174 6153 6f75 7263 652a 2a3a 0a20 2020  ataSource**:.   
-00004e10: 2020 2020 2020 2041 2063 6c61 7373 2074         A class t
-00004e20: 6861 7420 6973 2061 6e20 696e 7465 726d  hat is an interm
-00004e30: 6564 6961 7465 206c 696e 6b20 6265 7477  ediate link betw
-00004e40: 6565 6e20 7468 6520 536f 7572 6365 4150  een the SourceAP
-00004e50: 4920 616e 6420 436f 6d6d 616e 6473 2e0a  I and Commands..
-00004e60: 2020 2020 2020 2020 2d20 2a2a 536f 7572          - **Sour
-00004e70: 6365 4150 492a 2a3a 0a20 2020 2020 2020  ceAPI**:.       
-00004e80: 2020 2045 6163 6820 736f 7572 6365 2068     Each source h
-00004e90: 6173 2069 7473 206f 776e 2041 5049 2074  as its own API t
-00004ea0: 6f20 7265 7472 6965 7665 2064 6174 612e  o retrieve data.
-00004eb0: 2053 6f75 7263 6541 5049 2069 7320 6120   SourceAPI is a 
-00004ec0: 636c 6173 7320 7468 6174 2070 726f 7669  class that provi
-00004ed0: 6465 2041 5049 2066 6f72 2073 6f6d 6520  de API for some 
-00004ee0: 6461 7461 2073 6f75 7263 652e 0a20 2020  data source..   
-00004ef0: 2020 2020 202d 202a 2a43 6f6d 6d61 6e64       - **Command
-00004f00: 732a 2a3a 0a20 2020 2020 2020 2020 2043  s**:.          C
-00004f10: 6c61 7373 6573 2074 6861 7420 7072 6f76  lasses that prov
-00004f20: 6964 6520 7573 6572 2d66 7269 656e 646c  ide user-friendl
-00004f30: 7920 696e 7465 7266 6163 6573 2066 6f72  y interfaces for
-00004f40: 2067 6574 7469 6e67 2073 6f6d 6520 6461   getting some da
-00004f50: 7461 2066 726f 6d20 4461 7461 536f 7572  ta from DataSour
-00004f60: 6365 2e20 436f 6d6d 616e 6473 2075 7365  ce. Commands use
-00004f70: 205f 536f 7572 6365 4150 495f 2074 6f0a   _SourceAPI_ to.
-00004f80: 2020 2020 2020 2020 2020 6163 6869 6576            achiev
-00004f90: 6520 6974 2e0a 2020 2020 2020 2020 2d20  e it..        - 
-00004fa0: 2a2a 4164 6170 7465 7273 2a2a 3a0a 2020  **Adapters**:.  
-00004fb0: 2020 2020 2020 2020 4974 2773 2073 696d          It's sim
-00004fc0: 696c 6172 2074 6f20 6675 6e63 7469 6f6e  ilar to function
-00004fd0: 2066 6f72 2060 4461 7461 2e6d 6170 6020   for `Data.map` 
-00004fe0: 6d65 7468 6f64 2e20 4164 6f70 7461 626c  method. Adoptabl
-00004ff0: 6520 636f 6d6d 616e 6473 2075 7365 6420  e commands used 
-00005000: 6974 2074 6f20 7570 6461 7465 2074 6865  it to update the
-00005010: 2064 6174 6120 7374 7265 616d 2e0a 2020   data stream..  
-00005020: 2020 2020 2020 2d20 2a2a 4167 6772 6567        - **Aggreg
-00005030: 6174 6520 6f70 6572 6174 696f 6e73 2a2a  ate operations**
-00005040: 3a0a 2020 2020 2020 2020 2020 436f 6d6d  :.          Comm
-00005050: 6f6e 206f 7065 7261 7469 6f6e 7320 7375  on operations su
-00005060: 6368 2061 7320 6669 6c74 6572 2c20 6d61  ch as filter, ma
-00005070: 702c 206c 696d 6974 2061 6e64 2073 6f20  p, limit and so 
-00005080: 6f6e 2e0a 2020 2020 2020 2020 2d20 2a2a  on..        - **
-00005090: 576f 726b 666c 6f77 2a2a 3a20 416e 206f  Workflow**: An o
-000050a0: 7264 6572 6564 2073 6574 206f 6620 5f41  rdered set of _A
-000050b0: 6767 7265 6761 7465 206f 7065 7261 7469  ggregate operati
-000050c0: 6f6e 735f 2e0a 2020 2020 2020 2020 0a20  ons_..        . 
-000050d0: 2020 2020 2020 2023 2323 2043 6f6e 6365         ### Conce
-000050e0: 7074 0a20 2020 2020 2020 200a 2020 2020  pt.        .    
-000050f0: 2020 2020 5468 6520 6c69 6272 6172 7920      The library 
-00005100: 6465 7363 7269 6265 7320 7468 6520 6869  describes the hi
-00005110: 6768 2d6c 6576 656c 2069 6e74 6572 6661  gh-level interfa
-00005120: 6365 7320 6049 536f 7572 6365 4150 4960  ces `ISourceAPI`
-00005130: 2c20 6049 4461 7461 536f 7572 6365 602c  , `IDataSource`,
-00005140: 2060 4943 6f6d 6d61 6e64 602c 2060 4941   `ICommand`, `IA
-00005150: 6461 7074 6572 602e 0a20 2020 2020 2020  dapter`..       
-00005160: 200a 2020 2020 2020 2020 416e 7920 6461   .        Any da
-00005170: 7461 2073 6f75 7263 6520 6d75 7374 2062  ta source must b
-00005180: 6520 6465 7363 7269 6265 6420 6279 2074  e described by t
-00005190: 6865 2060 4944 6174 6153 6f75 7263 6560  he `IDataSource`
-000051a0: 2061 6273 7472 6163 7420 636c 6173 732e   abstract class.
-000051b0: 2054 6865 7365 2063 616e 2062 6520 5f46   These can be _F
-000051c0: 696c 6544 6174 6153 6f75 7263 655f 2c20  ileDataSource_, 
-000051d0: 0a20 2020 2020 2020 205f 4353 5644 6174  .        _CSVDat
-000051e0: 6153 6f75 7263 655f 2c20 5f44 4244 6174  aSource_, _DBDat
-000051f0: 6153 6f75 7263 655f 2061 6e64 206f 7468  aSource_ and oth
-00005200: 6572 2e0a 2020 2020 2020 2020 0a20 2020  er..        .   
-00005210: 2020 2020 2055 7375 616c 6c79 2c20 6461       Usually, da
-00005220: 7461 2073 6f75 7263 6573 2068 6176 6520  ta sources have 
-00005230: 736f 6d65 206b 696e 6420 6f66 2041 5049  some kind of API
-00005240: 2e20 4461 7461 6261 7365 7320 2d20 7072  . Databases - pr
-00005250: 6f76 6964 6520 5351 4c20 6c61 6e67 7561  ovide SQL langua
-00005260: 6765 2c20 7768 656e 2077 6f72 6b69 6e67  ge, when working
-00005270: 2077 6974 6820 6120 6669 6c65 2c20 796f   with a file, yo
-00005280: 7520 6361 6e20 7265 6164 0a20 2020 2020  u can read.     
-00005290: 2020 206c 696e 6520 6279 206c 696e 652c     line by line,
-000052a0: 2065 7463 2e20 5468 6973 2041 5049 2069   etc. This API i
-000052b0: 7320 6465 7363 7269 6265 6420 6279 2074  s described by t
-000052c0: 6865 2060 4953 6f75 7263 6541 5049 6020  he `ISourceAPI` 
-000052d0: 636c 6173 732e 2042 6563 6175 7365 2064  class. Because d
-000052e0: 6966 6665 7265 6e74 2076 6572 7369 6f6e  ifferent version
-000052f0: 7320 6f66 2074 6865 2073 616d 6520 6461  s of the same da
-00005300: 7461 2073 6f75 7263 650a 2020 2020 2020  ta source.      
-00005310: 2020 6d61 7920 6861 7665 2064 6966 6665    may have diffe
-00005320: 7265 6e74 2041 5049 2c20 6974 2069 7320  rent API, it is 
-00005330: 6265 7474 6572 2074 6f20 6372 6561 7465  better to create
-00005340: 2061 2063 6c61 7373 2066 6f72 2065 6163   a class for eac
-00005350: 6820 7665 7273 696f 6e2e 0a20 2020 2020  h version..     
-00005360: 2020 200a 2020 2020 2020 2020 4765 6e65     .        Gene
-00005370: 7261 6c6c 792c 2064 6174 6120 736f 7572  rally, data sour
-00005380: 6365 2041 5049 7320 6172 6520 6869 6464  ce APIs are hidd
-00005390: 656e 2062 6568 696e 6420 636f 6e76 656e  en behind conven
-000053a0: 6965 6e74 2069 6e74 6572 6661 6365 732e  ient interfaces.
-000053b0: 2054 6865 2072 6f6c 6520 6f66 2074 6865   The role of the
-000053c0: 7365 2069 6e74 6572 6661 6365 7320 6973  se interfaces is
-000053d0: 2070 6c61 7965 640a 2020 2020 2020 2020   played.        
-000053e0: 6279 2060 4943 6f6d 6d61 6e64 6020 636c  by `ICommand` cl
-000053f0: 6173 7365 732e 0a20 2020 2020 2020 200a  asses..        .
-00005400: 2020 2020 2020 2020 6049 4164 6170 7465          `IAdapte
-00005410: 7260 2063 6c61 7373 6573 2074 7261 6e73  r` classes trans
-00005420: 666f 726d 2064 6174 6120 7374 7265 616d  form data stream
-00005430: 206c 696b 6520 6675 6e63 7469 6f6e 7320   like functions 
-00005440: 666f 7220 6044 6174 612e 6d61 7060 206d  for `Data.map` m
-00005450: 6574 686f 642e 2045 7373 656e 7469 616c  ethod. Essential
-00005460: 6c79 2069 7427 7320 7468 6520 7361 6d65  ly it's the same
-00005470: 2074 6869 6e67 2062 7574 206d 6f72 650a   thing but more.
-00005480: 2020 2020 2020 2020 666c 6578 6962 6c65          flexible
-00005490: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000054a0: 2020 2046 6f72 2065 7861 6d70 6c65 2c20     For example, 
-000054b0: 4c77 4450 2044 6174 6153 6f75 7263 6528  LwDP DataSource(
-000054c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000054d0: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d64  om/th2-net/th2-d
-000054e0: 732d 736f 7572 6365 2d6c 7764 7029 2075  s-source-lwdp) u
-000054f0: 7365 7320 7468 6573 6520 6162 7374 7261  ses these abstra
-00005500: 6374 2063 6c61 7373 6573 2074 6f20 6275  ct classes to bu
-00005510: 696c 6420 6974 7320 696d 706c 656d 656e  ild its implemen
-00005520: 7461 7469 6f6e 2e59 6f75 2063 616e 2065  tation.You can e
-00005530: 6173 696c 7920 6372 6561 7465 2079 6f75  asily create you
-00005540: 7220 6f77 6e20 756e 6971 7565 2063 6f6d  r own unique com
-00005550: 6d61 6e64 7320 666f 7220 5f4c 7744 5020  mands for _LwDP 
-00005560: 4461 7461 536f 7572 6365 5f2c 2061 7320  DataSource_, as 
-00005570: 7765 6c6c 2061 7320 656e 7469 7265 0a20  well as entire. 
-00005580: 2020 2020 2020 205f 4461 7461 536f 7572         _DataSour
-00005590: 6365 5f20 636c 6173 7365 732e 205b 4865  ce_ classes. [He
-000055a0: 7265 2069 7320 6120 646f 6375 6d65 6e74  re is a document
-000055b0: 6174 696f 6e5d 2864 6f63 756d 656e 7461  ation](documenta
-000055c0: 7469 6f6e 2f64 6174 6173 6f75 7263 652e  tion/datasource.
-000055d0: 6d64 2920 6f6e 2068 6f77 2074 6f20 696d  md) on how to im
-000055e0: 706c 656d 656e 7420 7468 6573 6520 696e  plement these in
-000055f0: 7465 7266 6163 6573 2e0a 2020 2020 2020  terfaces..      
-00005600: 2020 0a20 2020 2020 2020 2021 5b44 6174    .        ![Dat
-00005610: 6120 7374 7265 616d 2070 6970 656c 696e  a stream pipelin
-00005620: 655d 2864 6f63 756d 656e 7461 7469 6f6e  e](documentation
-00005630: 2f69 6d67 2f63 6f6e 6365 7074 2e70 6e67  /img/concept.png
-00005640: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00005650: 2020 2023 2323 2053 7472 6561 6d20 6f70     ### Stream op
-00005660: 6572 6174 696f 6e73 0a20 2020 2020 2020  erations.       
-00005670: 200a 2020 2020 2020 2020 4675 7274 6865   .        Furthe
-00005680: 726d 6f72 652c 2073 7472 6561 6d20 6f70  rmore, stream op
-00005690: 6572 6174 696f 6e73 2068 6176 6520 7477  erations have tw
-000056a0: 6f20 6675 6e64 616d 656e 7461 6c20 6368  o fundamental ch
-000056b0: 6172 6163 7465 7269 7374 6963 7320 7468  aracteristics th
-000056c0: 6174 206d 616b 6520 7468 656d 2076 6572  at make them ver
-000056d0: 7920 6469 6666 6572 656e 7420 6672 6f6d  y different from
-000056e0: 2063 6f6c 6c65 6374 696f 6e0a 2020 2020   collection.    
-000056f0: 2020 2020 6f70 6572 6174 696f 6e73 3a20      operations: 
-00005700: 5f50 6970 656c 696e 696e 675f 2061 6e64  _Pipelining_ and
-00005710: 205f 496e 7465 726e 616c 2069 7465 7261   _Internal itera
-00005720: 7469 6f6e 5f2e 0a20 2020 2020 2020 200a  tion_..        .
-00005730: 2020 2020 2020 2020 2323 2323 2050 6970          #### Pip
-00005740: 656c 696e 696e 670a 2020 2020 2020 2020  elining.        
-00005750: 0a20 2020 2020 2020 204d 616e 7920 7374  .        Many st
-00005760: 7265 616d 206f 7065 7261 7469 6f6e 7320  ream operations 
-00005770: 7265 7475 726e 2061 2073 7472 6561 6d20  return a stream 
-00005780: 7468 656d 7365 6c76 6573 2e20 5468 6973  themselves. This
-00005790: 2061 6c6c 6f77 7320 6f70 6572 6174 696f   allows operatio
-000057a0: 6e73 2074 6f20 6265 2063 6861 696e 6564  ns to be chained
-000057b0: 2074 6f20 666f 726d 2061 206c 6172 6765   to form a large
-000057c0: 7220 7069 7065 6c69 6e65 2e0a 2020 2020  r pipeline..    
-000057d0: 2020 2020 0a20 2020 2020 2020 2021 5b44      .        ![D
-000057e0: 6174 6120 7374 7265 616d 2070 6970 656c  ata stream pipel
-000057f0: 696e 655d 2864 6f63 756d 656e 7461 7469  ine](documentati
-00005800: 6f6e 2f69 6d67 2f64 6174 615f 7374 7265  on/img/data_stre
-00005810: 616d 5f70 6970 656c 696e 652e 706e 6729  am_pipeline.png)
-00005820: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00005830: 2020 2323 2323 2049 6e74 6572 6e61 6c20    #### Internal 
-00005840: 6974 6572 6174 696f 6e0a 2020 2020 2020  iteration.      
-00005850: 2020 0a20 2020 2020 2020 2049 6e20 636f    .        In co
-00005860: 6e74 7261 7374 2074 6f20 636f 6c6c 6563  ntrast to collec
-00005870: 7469 6f6e 732c 2077 6869 6368 2061 7265  tions, which are
-00005880: 2069 7465 7261 7465 6420 6578 706c 6963   iterated explic
-00005890: 6974 6c79 2028 6578 7465 726e 616c 2069  itly (external i
-000058a0: 7465 7261 7469 6f6e 292c 2073 7472 6561  teration), strea
-000058b0: 6d20 6f70 6572 6174 696f 6e73 2064 6f20  m operations do 
-000058c0: 7468 6520 6974 6572 6174 696f 6e0a 2020  the iteration.  
-000058d0: 2020 2020 2020 6265 6869 6e64 2074 6865        behind the
-000058e0: 2073 6365 6e65 7320 666f 7220 796f 752e   scenes for you.
-000058f0: 204e 6f74 652c 2069 7420 646f 6573 6e27   Note, it doesn'
-00005900: 7420 6d65 616e 2079 6f75 2063 616e 6e6f  t mean you canno
-00005910: 7420 6974 6572 6174 6520 7468 6520 5f44  t iterate the _D
-00005920: 6174 6120 6f62 6a65 6374 5f2e 0a20 2020  ata object_..   
-00005930: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00005940: 2320 4461 7461 2063 6163 6869 6e67 0a20  # Data caching. 
-00005950: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00005960: 5468 6520 5f44 6174 6120 6f62 6a65 6374  The _Data object
-00005970: 5f20 7072 6f76 6964 6573 2074 6865 2061  _ provides the a
-00005980: 6269 6c69 7479 2074 6f20 7573 6520 7468  bility to use th
-00005990: 6520 6361 6368 652e 2054 6865 2063 6163  e cache. The cac
-000059a0: 6865 2077 6f72 6b73 2066 6f72 2065 6163  he works for eac
-000059b0: 6820 5f44 6174 6120 6f62 6a65 6374 5f2c  h _Data object_,
-000059c0: 2074 6861 7420 6973 2c20 796f 7520 6368   that is, you ch
-000059d0: 6f6f 7365 0a20 2020 2020 2020 2077 6869  oose.        whi
-000059e0: 6368 205f 4461 7461 206f 626a 6563 745f  ch _Data object_
-000059f0: 2079 6f75 2077 616e 7420 746f 2073 6176   you want to sav
-00005a00: 652e 2054 6865 205f 4461 7461 206f 626a  e. The _Data obj
-00005a10: 6563 745f 2063 6163 6865 2069 7320 7361  ect_ cache is sa
-00005a20: 7665 6420 6166 7465 7220 7468 6520 6669  ved after the fi
-00005a30: 7273 7420 6974 6572 6174 696f 6e2c 2062  rst iteration, b
-00005a40: 7574 2074 6865 2069 7465 7261 7469 6f6e  ut the iteration
-00005a50: 0a20 2020 2020 2020 2073 6f75 7263 6520  .        source 
-00005a60: 6d61 7920 6265 2064 6966 6665 7265 6e74  may be different
-00005a70: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00005a80: 2020 2049 6620 796f 7520 646f 6e27 7420     If you don't 
-00005a90: 7573 6520 7468 6520 6361 6368 652c 2079  use the cache, y
-00005aa0: 6f75 7220 736f 7572 6365 2077 696c 6c20  our source will 
-00005ab0: 6265 2074 6865 2064 6174 6120 736f 7572  be the data sour
-00005ac0: 6365 2079 6f75 2068 6176 6520 696e 2074  ce you have in t
-00005ad0: 6865 205f 4461 7461 204f 626a 6563 745f  he _Data Object_
-00005ae0: 2e20 4275 7420 6966 2079 6f75 2075 7365  . But if you use
-00005af0: 2074 6865 2063 6163 6865 2c0a 2020 2020   the cache,.    
-00005b00: 2020 2020 796f 7572 2073 6f75 7263 6520      your source 
-00005b10: 6361 6e20 6265 2074 6865 2064 6174 6120  can be the data 
-00005b20: 736f 7572 6365 2c20 7468 6520 7061 7265  source, the pare
-00005b30: 6e74 2063 6163 6865 2c20 6f72 206f 776e  nt cache, or own
-00005b40: 2063 6163 6865 3a0a 2020 2020 2020 2020   cache:.        
-00005b50: 0a20 2020 2020 2020 202a 2054 6865 2064  .        * The d
-00005b60: 6174 6120 736f 7572 6365 3a0a 2020 2020  ata source:.    
-00005b70: 2020 2020 2020 4966 2074 6865 205f 4461        If the _Da
-00005b80: 7461 204f 626a 6563 745f 2064 6f65 736e  ta Object_ doesn
-00005b90: 2774 2068 6176 6520 6120 7061 7265 6e74  't have a parent
-00005ba0: 2063 6163 6865 2061 6e64 2069 7473 2063   cache and its c
-00005bb0: 6163 6865 2e0a 2020 2020 2020 2020 2a20  ache..        * 
-00005bc0: 5468 6520 7061 7265 6e74 2063 6163 6865  The parent cache
-00005bd0: 3a0a 2020 2020 2020 2020 2020 4966 2074  :.          If t
-00005be0: 6865 205f 4461 7461 204f 626a 6563 745f  he _Data Object_
-00005bf0: 2068 6173 2061 2070 6172 656e 7420 6361   has a parent ca
-00005c00: 6368 652e 2049 7420 646f 6573 6e27 7420  che. It doesn't 
-00005c10: 6d61 7474 6572 2077 6861 7420 706f 7369  matter what posi
-00005c20: 7469 6f6e 2074 6865 2070 6172 656e 7420  tion the parent 
-00005c30: 6361 6368 6520 6861 7320 696e 2069 6e68  cache has in inh
-00005c40: 6572 6974 616e 6365 2e0a 2020 2020 2020  eritance..      
-00005c50: 2020 2020 5f44 6174 6120 4f62 6a65 6374      _Data Object
-00005c60: 5f20 756e 6465 7273 7461 6e64 7320 7768  _ understands wh
-00005c70: 6f73 6520 6361 6368 6520 6974 2069 7320  ose cache it is 
-00005c80: 616e 6420 6578 6563 7574 6573 2074 6865  and executes the
-00005c90: 2070 6172 7420 6f66 2074 6865 2077 6f72   part of the wor
-00005ca0: 6b66 6c6f 7720 7468 6174 2077 6173 206e  kflow that was n
-00005cb0: 6f74 2065 7865 6375 7465 642e 0a20 2020  ot executed..   
-00005cc0: 2020 2020 202a 2054 6865 206f 776e 2063       * The own c
-00005cd0: 6163 6865 3a0a 2020 2020 2020 2020 2020  ache:.          
-00005ce0: 4966 2069 7420 6973 206e 6f74 2074 6865  If it is not the
-00005cf0: 2066 6972 7374 2069 7465 7261 7469 6f6e   first iteration
-00005d00: 206f 6620 7468 6973 2044 6174 6120 6f62   of this Data ob
-00005d10: 6a65 6374 2e0a 2020 2020 2020 2020 0a20  ject..        . 
-00005d20: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
-00005d30: 2074 6865 2063 6163 6865 2073 7461 7465   the cache state
-00005d40: 206f 6620 7468 6520 4461 7461 206f 626a   of the Data obj
-00005d50: 6563 7420 6973 206e 6f74 2069 6e68 6572  ect is not inher
-00005d60: 6974 6564 2e0a 2020 2020 2020 2020 0a20  ited..        . 
-00005d70: 2020 2020 2020 2023 2323 2320 466f 7263         #### Forc
-00005d80: 6564 2063 6163 6869 6e67 0a20 2020 2020  ed caching.     
-00005d90: 2020 2059 6f75 2063 616e 2074 656c 6c20     You can tell 
-00005da0: 4453 2074 6f20 6361 6368 6520 6461 7461  DS to cache data
-00005db0: 2074 6f20 7370 6563 6966 6963 2063 6163   to specific cac
-00005dc0: 6865 2066 696c 652c 2077 6869 6368 2077  he file, which w
-00005dd0: 6f6e 2774 2062 6520 6465 6c65 7465 6420  on't be deleted 
-00005de0: 6166 7465 7220 7363 7269 7074 2065 6e64  after script end
-00005df0: 2e0a 2020 2020 2020 2020 596f 7520 6361  ..        You ca
-00005e00: 6e20 7365 6520 6578 616d 706c 6520 696e  n see example in
-00005e10: 2031 2e31 3220 7365 6374 696f 6e20 6f66   1.12 section of
-00005e20: 205b 6765 745f 7374 6172 7465 645f 6578   [get_started_ex
-00005e30: 616d 706c 655d 2865 7861 6d70 6c65 732f  ample](examples/
-00005e40: 6765 745f 7374 6172 7465 645f 6578 616d  get_started_exam
-00005e50: 706c 652e 7079 292e 0a20 2020 2020 2020  ple.py)..       
-00005e60: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
-00005e70: 2020 2023 2323 2045 7665 6e74 5472 6565     ### EventTree
-00005e80: 2061 6e64 2063 6f6c 6c65 6374 696f 6e73   and collections
-00005e90: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00005ea0: 2020 2323 2323 2045 7665 6e74 5472 6565    #### EventTree
-00005eb0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00005ec0: 2020 6045 7665 6e74 5472 6565 6020 6973    `EventTree` is
-00005ed0: 2061 2074 7265 652d 6261 7365 6420 6461   a tree-based da
-00005ee0: 7461 2073 7472 7563 7475 7265 206f 6620  ta structure of 
-00005ef0: 6576 656e 7473 2e20 4974 2061 6c6c 6f77  events. It allow
-00005f00: 7320 796f 7520 6765 7420 6368 696c 6472  s you get childr
-00005f10: 656e 2061 6e64 2070 6172 656e 7473 206f  en and parents o
-00005f20: 6620 6576 656e 742c 200a 2020 2020 2020  f event, .      
-00005f30: 2020 6469 7370 6c61 7920 7472 6565 2c20    display tree, 
-00005f40: 6765 7420 6675 6c6c 2070 6174 6820 746f  get full path to
-00005f50: 2065 7665 6e74 2065 7463 2e0a 2020 2020   event etc..    
-00005f60: 2020 2020 0a20 2020 2020 2020 2044 6574      .        Det
-00005f70: 6169 6c73 3a0a 2020 2020 2020 2020 0a20  ails:.        . 
-00005f80: 2020 2020 2020 202a 2060 4576 656e 7454         * `EventT
-00005f90: 7265 6560 2063 6f6e 7461 696e 7320 616c  ree` contains al
-00005fa0: 6c20 6576 656e 7473 2069 6e20 6d65 6d6f  l events in memo
-00005fb0: 7279 2e0a 2020 2020 2020 2020 2a20 5472  ry..        * Tr
-00005fc0: 6565 2068 6173 2073 6f6d 6520 696d 706f  ee has some impo
-00005fd0: 7274 616e 7420 7465 726d 733a 0a20 2020  rtant terms:.   
-00005fe0: 2020 2020 2020 2020 2031 2e20 5f41 6e63           1. _Anc
-00005ff0: 6573 746f 725f 2069 7320 616e 7920 7265  estor_ is any re
-00006000: 6c61 7469 7665 206f 6620 7468 6520 6576  lative of the ev
-00006010: 656e 7420 7570 2074 6865 2074 7265 6520  ent up the tree 
-00006020: 2867 7261 6e64 7061 7265 6e74 2c20 7061  (grandparent, pa
-00006030: 7265 6e74 2065 7463 2e29 2e0a 2020 2020  rent etc.)..    
-00006040: 2020 2020 2020 2020 322e 205f 5061 7265          2. _Pare
-00006050: 6e74 5f20 6973 206f 6e6c 7920 7468 6520  nt_ is only the 
-00006060: 6669 7273 7420 7265 6c61 7469 7665 206f  first relative o
-00006070: 6620 7468 6520 6576 656e 7420 7570 2074  f the event up t
-00006080: 6865 2074 7265 652e 0a20 2020 2020 2020  he tree..       
-00006090: 2020 2020 2033 2e20 5f43 6869 6c64 5f20       3. _Child_ 
-000060a0: 6973 2074 6865 2066 6972 7374 2072 656c  is the first rel
-000060b0: 6174 6976 6520 6f66 2074 6865 2065 7665  ative of the eve
-000060c0: 6e74 2064 6f77 6e20 7468 6520 7472 6565  nt down the tree
-000060d0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000060e0: 2020 2054 616b 6520 6120 6c6f 6f6b 2061     Take a look a
-000060f0: 7420 7468 6520 666f 6c6c 6f77 696e 6720  t the following 
-00006100: 4854 4d4c 2074 7265 6520 746f 2075 6e64  HTML tree to und
-00006110: 6572 7374 616e 6420 7468 656d 2e0a 2020  erstand them..  
-00006120: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00006130: 2020 6060 600a 2020 2020 2020 2020 2020    ```.          
-00006140: 2020 3c62 6f64 793e 203c 212d 2d20 616e    <body> <!-- an
-00006150: 6365 7374 6f72 2028 6772 616e 6470 6172  cestor (grandpar
-00006160: 656e 7429 2c20 6275 7420 6e6f 7420 7061  ent), but not pa
-00006170: 7265 6e74 202d 2d3e 0a20 2020 2020 2020  rent -->.       
-00006180: 2020 2020 2020 2020 203c 6469 763e 203c           <div> <
-00006190: 212d 2d20 7061 7265 6e74 2026 2061 6e63  !-- parent & anc
-000061a0: 6573 746f 7220 2d2d 3e0a 2020 2020 2020  estor -->.      
-000061b0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000061c0: 3e48 656c 6c6f 2c20 776f 726c 6421 3c2f  >Hello, world!</
-000061d0: 703e 203c 212d 2d20 6368 696c 6420 2d2d  p> <!-- child --
-000061e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000061f0: 2020 2020 2020 3c70 3e47 6f6f 6462 7965        <p>Goodbye
-00006200: 213c 2f70 3e20 3c21 2d2d 2073 6962 6c69  !</p> <!-- sibli
-00006210: 6e67 202d 2d3e 0a20 2020 2020 2020 2020  ng -->.         
-00006220: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00006230: 2020 2020 2020 2020 2020 3c2f 626f 6479            </body
-00006240: 3e0a 2020 2020 2020 2020 2020 2060 6060  >.           ```
-00006250: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006260: 2020 2323 2323 2043 6f6c 6c65 6374 696f    #### Collectio
-00006270: 6e73 0a20 2020 2020 2020 200a 2020 2020  ns.        .    
-00006280: 2020 2020 2a2a 4576 656e 7454 7265 6543      **EventTreeC
-00006290: 6f6c 6c65 6374 696f 6e2a 2a20 6973 2061  ollection** is a
-000062a0: 2063 6f6c 6c65 6374 696f 6e20 6f66 2045   collection of E
-000062b0: 7665 6e74 5472 6565 732e 2054 6865 2063  ventTrees. The c
-000062c0: 6f6c 6c65 6374 696f 6e20 6275 696c 6473  ollection builds
-000062d0: 2061 2066 6577 205f 4576 656e 7454 7265   a few _EventTre
-000062e0: 655f 2062 7920 7061 7373 6564 205f 4461  e_ by passed _Da
-000062f0: 7461 0a20 2020 2020 2020 206f 626a 6563  ta.        objec
-00006300: 745f 2e20 416c 7468 6f75 6768 2079 6f75  t_. Although you
-00006310: 2063 616e 2063 6861 6e67 6520 7468 6520   can change the 
-00006320: 7472 6565 2064 6972 6563 746c 792c 2069  tree directly, i
-00006330: 7427 7320 6265 7474 6572 2074 6f20 646f  t's better to do
-00006340: 2069 7420 7468 726f 7567 6820 636f 6c6c   it through coll
-00006350: 6563 7469 6f6e 7320 6265 6361 7573 6520  ections because 
-00006360: 7468 6579 2061 7265 2061 7761 7265 206f  they are aware o
-00006370: 660a 2020 2020 2020 2020 6064 6574 6163  f.        `detac
-00006380: 6865 645f 6576 656e 7473 6020 616e 6420  hed_events` and 
-00006390: 6361 6e20 736f 6c76 6520 736f 6d65 2065  can solve some e
-000063a0: 7665 6e74 7320 6465 7065 6e64 656e 6369  vents dependenci
-000063b0: 6573 2e20 5468 6520 636f 6c6c 6563 7469  es. The collecti
-000063c0: 6f6e 2068 6173 2073 696d 696c 6172 2066  on has similar f
-000063d0: 6561 7475 7265 7320 6c69 6b65 2061 2073  eatures like a s
-000063e0: 696e 676c 6520 5f45 7665 6e74 5472 6565  ingle _EventTree
-000063f0: 5f0a 2020 2020 2020 2020 6275 7420 6170  _.        but ap
-00006400: 706c 7969 6e67 2074 6865 6d20 666f 7220  plying them for 
-00006410: 616c 6c20 5f45 7665 6e74 5472 6565 735f  all _EventTrees_
-00006420: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00006430: 2020 202a 2a50 6172 656e 7445 7665 6e74     **ParentEvent
-00006440: 5472 6565 436f 6c6c 6563 7469 6f6e 2a2a  TreeCollection**
-00006450: 2069 7320 6120 636f 6c6c 6563 7469 6f6e   is a collection
-00006460: 2073 696d 696c 6172 2074 6f20 5f45 7665   similar to _Eve
-00006470: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
-00006480: 5f20 6275 7420 636f 6e74 6169 6e69 6e67  _ but containing
-00006490: 206f 6e6c 7920 7061 7265 6e74 2065 7665   only parent eve
-000064a0: 6e74 7320 7468 6174 0a20 2020 2020 2020  nts that.       
-000064b0: 2061 7265 2072 6566 6572 656e 6365 6420   are referenced 
-000064c0: 696e 2074 6865 2064 6174 6120 7374 7265  in the data stre
-000064d0: 616d 2e20 5468 6520 636f 6c6c 6563 7469  am. The collecti
-000064e0: 6f6e 2068 6173 2066 6561 7475 7265 7320  on has features 
-000064f0: 7369 6d69 6c61 7220 746f 205f 4576 656e  similar to _Even
-00006500: 7454 7265 6543 6f6c 6c65 6374 696f 6e5f  tTreeCollection_
-00006510: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00006520: 2020 2044 6574 6169 6c73 3a0a 2020 2020     Details:.    
-00006530: 2020 2020 0a20 2020 2020 2020 202a 2054      .        * T
-00006540: 6f20 7573 6520 4554 2063 6f6c 6c65 6374  o use ET collect
-00006550: 696f 6e73 2079 6f75 206e 6565 6420 746f  ions you need to
-00006560: 2069 6e69 7469 616c 697a 6520 7468 656d   initialize them
-00006570: 2062 7920 5f45 5443 4472 6976 6572 5f2e   by _ETCDriver_.
-00006580: 2044 6174 6120 736f 7572 6365 7320 7573   Data sources us
-00006590: 7561 6c6c 7920 7072 6f76 6964 6520 7468  ually provide th
-000065a0: 656d 2e0a 2020 2020 2020 2020 2020 596f  em..          Yo
-000065b0: 7520 6361 6e20 6372 6561 7465 2069 7420  u can create it 
-000065c0: 6279 2079 6f75 7273 656c 6620 6465 7065  by yourself depe
-000065d0: 6e64 696e 6720 6f6e 2079 6f75 7220 6461  nding on your da
-000065e0: 7461 2073 7472 7563 7475 7265 2e20 200a  ta structure.  .
-000065f0: 2020 2020 2020 2020 2a20 5468 6520 636f          * The co
-00006600: 6c6c 6563 7469 6f6e 2068 6173 2061 2066  llection has a f
-00006610: 6561 7475 7265 2074 6f20 7265 636f 7665  eature to recove
-00006620: 7220 6576 656e 7473 2e20 416c 6c20 6576  r events. All ev
-00006630: 656e 7473 2074 6861 7420 6172 6520 6e6f  ents that are no
-00006640: 7420 696e 2074 6865 2072 6563 6569 7665  t in the receive
-00006650: 6420 6461 7461 2073 7472 6561 6d2c 2062  d data stream, b
-00006660: 7574 2077 6869 6368 2061 7265 0a20 2020  ut which are.   
-00006670: 2020 2020 2020 2072 6566 6572 656e 6365         reference
-00006680: 6420 7769 6c6c 2062 6520 6c6f 6164 6564  d will be loaded
-00006690: 2066 726f 6d20 7468 6520 6461 7461 2073   from the data s
-000066a0: 6f75 7263 652e 0a20 2020 2020 2020 202a  ource..        *
-000066b0: 2059 6f75 2063 616e 2074 616b 6520 6064   You can take `d
-000066c0: 6574 6163 6865 645f 6576 656e 7473 6020  etached_events` 
-000066d0: 746f 2073 6565 2077 6869 6368 2065 7665  to see which eve
-000066e0: 6e74 7320 6172 6520 6d69 7373 696e 672e  nts are missing.
-000066f0: 0a20 2020 2020 2020 202a 2049 6620 796f  .        * If yo
-00006700: 7520 7761 6e74 2c20 796f 7520 6361 6e20  u want, you can 
-00006710: 6275 696c 6420 7061 7265 6e74 6c65 7373  build parentless
-00006720: 2074 7265 6573 2077 6865 7265 2074 6865   trees where the
-00006730: 206d 6973 7369 6e67 2065 7665 6e74 7320   missing events 
-00006740: 6172 6520 7374 7562 6265 6420 696e 7374  are stubbed inst
-00006750: 6561 642e 204a 7573 740a 2020 2020 2020  ead. Just.      
-00006760: 2020 2020 7573 6520 6067 6574 5f70 6172      use `get_par
-00006770: 656e 746c 6573 735f 7472 6565 7328 2960  entless_trees()`
-00006780: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00006790: 2020 2052 6571 7569 7265 6d65 6e74 733a     Requirements:
-000067a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000067b0: 2020 312e 2045 7665 6e74 7320 7072 6f76    1. Events prov
-000067c0: 6964 6564 2074 6f20 4554 4320 6861 7665  ided to ETC have
-000067d0: 2074 6f20 6861 7665 2060 6576 656e 745f   to have `event_
-000067e0: 6e61 6d65 602c 2060 6576 656e 745f 6964  name`, `event_id
-000067f0: 602c 2060 7061 7265 6e74 5f65 7665 6e74  `, `parent_event
-00006800: 5f69 6460 2066 6965 6c64 732e 2054 6865  _id` fields. The
-00006810: 7920 0a20 2020 2020 2020 2063 616e 2068  y .        can h
-00006820: 6176 6520 616e 6f74 6865 7220 6e61 6d65  ave another name
-00006830: 7320 2869 7420 7265 736f 6c76 6573 2069  s (it resolves i
-00006840: 6e20 7468 6520 6472 6976 6572 292e 0a20  n the driver).. 
-00006850: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006860: 2323 2323 2048 696e 7473 0a20 2020 2020  #### Hints.     
-00006870: 2020 200a 2020 2020 2020 2020 2a20 5265     .        * Re
-00006880: 6d6f 7665 2061 6c6c 2075 6e6e 6563 6573  move all unneces
-00006890: 7361 7279 2066 6965 6c64 7320 6672 6f6d  sary fields from
-000068a0: 2065 7665 6e74 7320 6265 666f 7265 2070   events before p
-000068b0: 6173 7369 6e67 2074 6f20 6120 5f63 6f6c  assing to a _col
-000068c0: 6c65 6374 696f 6e5f 2074 6f20 7265 6475  lection_ to redu
-000068d0: 6365 206d 656d 6f72 7920 7573 6167 652e  ce memory usage.
-000068e0: 0a20 2020 2020 2020 202a 2055 7365 2060  .        * Use `
-000068f0: 7368 6f77 2829 6020 6d65 7468 6f64 2074  show()` method t
-00006900: 6f20 7072 696e 7420 7468 6520 7472 6565  o print the tree
-00006910: 2069 6e20 7472 6565 2d6c 696b 6520 7669   in tree-like vi
-00006920: 6577 2e0a 2020 2020 2020 2020 2a20 4e6f  ew..        * No
-00006930: 7465 2074 6861 7420 7468 6520 6067 6574  te that the `get
-00006940: 5f78 6020 6d65 7468 6f64 7320 7769 6c6c  _x` methods will
-00006950: 2072 6169 7365 2061 6e20 6578 6365 7074   raise an except
-00006960: 696f 6e20 6966 2079 6f75 2070 6173 7320  ion if you pass 
-00006970: 616e 2075 6e6b 6e6f 776e 2065 7665 6e74  an unknown event
-00006980: 2069 642c 2075 6e6c 696b 6520 7468 6520   id, unlike the 
-00006990: 6066 696e 645f 7860 206d 6574 686f 6473  `find_x` methods
-000069a0: 2028 0a20 2020 2020 2020 2020 2074 6865   (.          the
-000069b0: 7920 7265 7475 726e 204e 6f6e 6529 2e0a  y return None)..
-000069c0: 2020 2020 2020 2020 2a20 4966 2079 6f75          * If you
-000069d0: 2077 616e 7420 746f 206b 6e6f 7720 7468   want to know th
-000069e0: 6174 2073 7065 6369 6669 6564 2065 7665  at specified eve
-000069f0: 6e74 2065 7869 7374 732c 2075 7365 2074  nt exists, use t
-00006a00: 6865 2070 7974 686f 6e20 6069 6e60 206b  he python `in` k
-00006a10: 6579 776f 7264 2028 652e 672e 2060 2765  eyword (e.g. `'e
-00006a20: 7665 6e74 2d69 6427 2069 6e20 6576 656e  vent-id' in even
-00006a30: 7473 5f74 7265 6560 292e 0a20 2020 2020  ts_tree`)..     
-00006a40: 2020 202a 2055 7365 2074 6865 2070 7974     * Use the pyt
-00006a50: 686f 6e20 606c 656e 6020 6b65 7977 6f72  hon `len` keywor
-00006a60: 6420 746f 2067 6574 2065 7665 6e74 7320  d to get events 
-00006a70: 6e75 6d62 6572 2069 6e20 7468 6520 7472  number in the tr
-00006a80: 6565 2e0a 2020 2020 2020 2020 0a20 2020  ee..        .   
-00006a90: 2020 2020 2023 2323 2046 6965 6c64 7352       ### FieldsR
-00006aa0: 6573 6f6c 7665 720a 2020 2020 2020 2020  esolver.        
-00006ab0: 5468 6520 6964 6561 206f 6620 7573 696e  The idea of usin
-00006ac0: 6720 7265 736f 6c76 6572 733a 2020 0a20  g resolvers:  . 
-00006ad0: 2020 2020 2020 2049 7420 736f 6c76 6573         It solves
-00006ae0: 2074 6865 2070 726f 626c 656d 206f 6620   the problem of 
-00006af0: 6861 7669 6e67 2061 2066 6577 2044 6174  having a few Dat
-00006b00: 6153 6f75 7263 6573 2077 6974 6820 7468  aSources with th
-00006b10: 6520 7361 6d65 2064 6174 612c 200a 2020  e same data, .  
-00006b20: 2020 2020 2020 6275 7420 7769 7468 2064        but with d
-00006b30: 6966 6665 7265 6e74 2077 6179 7320 746f  ifferent ways to
-00006b40: 2067 6574 2069 742e 0a20 2020 2020 2020   get it..       
-00006b50: 200a 2020 2020 2020 2020 5468 6573 6520   .        These 
-00006b60: 636c 6173 7365 7320 7072 6f76 6964 6520  classes provide 
-00006b70: 796f 7520 6765 7474 6572 206d 6574 686f  you getter metho
-00006b80: 6473 2e20 0a20 2020 2020 2020 2055 7369  ds. .        Usi
-00006b90: 6e67 2074 6865 7365 2063 6c61 7373 6573  ng these classes
-00006ba0: 2061 6c6c 6f77 7320 796f 7520 746f 2066   allows you to f
-00006bb0: 7265 656c 7920 7377 6974 6368 2062 6574  reely switch bet
-00006bc0: 7765 656e 2064 6966 6665 7265 6e74 2064  ween different d
-00006bd0: 6174 6120 0a20 2020 2020 2020 2066 6f72  ata .        for
-00006be0: 6d61 7473 2061 6e64 2064 6f6e 2774 2063  mats and don't c
-00006bf0: 6861 6e67 6520 796f 7572 2063 6f64 652e  hange your code.
-00006c00: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
-00006c10: 2020 2052 6573 6f6c 7665 7273 2073 6f6c     Resolvers sol
-00006c20: 7665 2074 6865 2070 726f 626c 656d 206f  ve the problem o
-00006c30: 6620 6461 7461 2d66 6f72 6d61 7420 6d69  f data-format mi
-00006c40: 6772 6174 696f 6e2e 2020 0a20 2020 2020  gration.  .     
-00006c50: 2020 202d 2066 6965 6c64 7320 706c 6163     - fields plac
-00006c60: 6520 6361 6e20 6265 2063 6861 6e67 6564  e can be changed
-00006c70: 0a20 2020 2020 2020 202d 2066 6965 6c64  .        - field
-00006c80: 7320 6e61 6d65 7320 6361 6e20 6265 2063  s names can be c
-00006c90: 6861 6e67 6564 0a20 2020 2020 2020 200a  hanged.        .
-00006ca0: 2020 2020 2020 2020 5265 736f 6c76 6572          Resolver
-00006cb0: 7320 6361 6e20 776f 726b 206f 6e6c 7920  s can work only 
-00006cc0: 7769 7468 206f 6e65 2065 7665 6e74 2f6d  with one event/m
-00006cd0: 6573 7361 6765 2e20 0a20 2020 2020 2020  essage. .       
-00006ce0: 2049 7420 6d65 616e 732c 2069 6620 796f   It means, if yo
-00006cf0: 7572 206d 6573 7361 6765 2068 6173 2073  ur message has s
-00006d00: 7562 2d6d 6573 7361 6765 7320 6974 2077  ub-messages it w
-00006d10: 6f6e 2774 2077 6f72 6b2c 2062 6563 6175  on't work, becau
-00006d20: 7365 2072 6573 6f6c 7665 7220 7769 6c6c  se resolver will
-00006d30: 206e 6f74 200a 2020 2020 2020 2020 6b6e   not .        kn
-00006d40: 6f77 2077 6974 6820 7768 6963 6820 7375  ow with which su
-00006d50: 622d 6d65 7373 6167 6520 7368 6f75 6c64  b-message should
-00006d60: 2069 7420 776f 726b 2e20 0a20 2020 2020   it work. .     
-00006d70: 2020 200a 2020 2020 2020 2020 496d 706c     .        Impl
-00006d80: 656d 656e 7461 7469 6f6e 2061 6476 6963  ementation advic
-00006d90: 653a 0a20 2020 2020 2020 2031 2e20 7261  e:.        1. ra
-00006da0: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
-00006db0: 6564 4572 726f 7220 2d2d 2069 6620 796f  edError -- if yo
-00006dc0: 7572 2049 6d70 6c65 6d65 6e74 6174 696f  ur Implementatio
-00006dd0: 6e20 646f 6573 6e27 7420 7375 7070 6f72  n doesn't suppor
-00006de0: 7420 7468 6973 2067 6574 7465 722e 0a20  t this getter.. 
-00006df0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006e00: 5065 7266 6f72 6d61 6e63 6520 696d 7061  Performance impa
-00006e10: 6374 3a0a 2020 2020 2020 2020 2d20 4974  ct:.        - It
-00006e20: 2061 2062 6974 2073 6c6f 7765 7220 7468   a bit slower th
-00006e30: 616e 2075 7369 6e67 206e 616b 6564 2066  an using naked f
-00006e40: 6965 6c64 2061 6363 6573 7320 6064 6963  ield access `dic
-00006e50: 745b 276b 6579 275d 602e 200a 2020 2020  t['key']`. .    
-00006e60: 2020 2020 0a20 2020 2020 2020 2023 2320      .        ## 
-00006e70: 322e 342e 204c 696e 6b73 0a20 2020 2020  2.4. Links.     
-00006e80: 2020 200a 2020 2020 2020 2020 2d20 5b52     .        - [R
-00006e90: 6570 6f72 7420 4461 7461 2050 726f 7669  eport Data Provi
-00006ea0: 6465 725d 2868 7474 7073 3a2f 2f67 6974  der](https://git
-00006eb0: 6875 622e 636f 6d2f 7468 322d 6e65 742f  hub.com/th2-net/
-00006ec0: 7468 322d 7270 742d 6461 7461 2d70 726f  th2-rpt-data-pro
-00006ed0: 7669 6465 7229 0a20 2020 2020 2020 202d  vider).        -
-00006ee0: 205b 5468 3220 4461 7461 2053 6572 7669   [Th2 Data Servi
-00006ef0: 6365 7320 5574 696c 735d 2868 7474 7073  ces Utils](https
-00006f00: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
-00006f10: 322d 6e65 742f 7468 322d 6461 7461 2d73  2-net/th2-data-s
-00006f20: 6572 7669 6365 732d 7574 696c 7329 0a20  ervices-utils). 
-00006f30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006f40: 2320 332e 2042 6573 7420 7072 6163 7469  # 3. Best practi
-00006f50: 6365 730a 2020 2020 2020 2020 4465 7065  ces.        Depe
-00006f60: 6e64 696e 6720 6f6e 2068 6f77 2079 6f75  nding on how you
-00006f70: 2077 6f72 6b20 7769 7468 2060 4461 7461   work with `Data
-00006f80: 206f 626a 6563 7460 2c20 6974 2063 616e   object`, it can
-00006f90: 2062 6520 736c 6f77 206f 6620 6661 7374   be slow of fast
-00006fa0: 2e20 200a 2020 2020 2020 2020 4173 2077  .  .        As w
-00006fb0: 6974 6820 6120 7265 6c61 7469 6f6e 616c  ith a relational
-00006fc0: 2064 6174 6162 6173 652c 2079 6f75 2063   database, you c
-00006fd0: 616e 2077 7269 7465 2061 2071 7565 7279  an write a query
-00006fe0: 2074 6861 7420 7769 6c6c 2072 6574 7572   that will retur
-00006ff0: 6e20 6461 7461 2073 6c6f 776c 7920 6f72  n data slowly or
-00007000: 2071 7569 636b 6c79 2c20 0a20 2020 2020   quickly, .     
-00007010: 2020 2074 6865 2073 616d 6520 7768 656e     the same when
-00007020: 2077 6f72 6b69 6e67 2077 6974 6820 6120   working with a 
-00007030: 6044 6174 6120 6f62 6a65 6374 602e 0a20  `Data object`.. 
-00007040: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007050: 466f 6c6c 6f77 2074 6865 2072 756c 6573  Follow the rules
-00007060: 2074 6f20 6d61 6b65 2079 6f75 7220 776f   to make your wo
-00007070: 726b 2077 6974 6820 4461 7461 206f 626a  rk with Data obj
-00007080: 6563 7420 6661 7374 3a0a 2020 2020 2020  ect fast:.      
-00007090: 2020 312e 2055 7365 2060 4461 7461 2e75    1. Use `Data.u
-000070a0: 7365 5f63 6163 6865 2829 6020 6966 2079  se_cache()` if y
-000070b0: 6f75 2069 7465 7261 7465 2064 6174 6120  ou iterate data 
-000070c0: 6d6f 7265 2074 6861 6e20 6f6e 6520 7469  more than one ti
-000070d0: 6d65 2e0a 2020 2020 2020 2020 322e 2054  me..        2. T
-000070e0: 7279 2074 6f20 646f 6e27 7420 6974 6572  ry to don't iter
-000070f0: 6174 6520 6f6e 6520 6044 6174 6120 6f62  ate one `Data ob
-00007100: 6a65 6374 6020 696e 7369 6465 2074 6865  ject` inside the
-00007110: 206f 7468 6572 206f 6e65 2e20 200a 2020   other one.  .  
-00007120: 2020 2020 2020 2020 2049 6620 796f 7520           If you 
-00007130: 7368 6f75 6c64 2074 6f20 646f 2069 742c  should to do it,
-00007140: 2075 7365 2073 686f 7274 2060 4461 7461   use short `Data
-00007150: 206f 626a 6563 7460 2066 6972 7374 2061   object` first a
-00007160: 6e64 206c 6f6e 6720 6044 6174 6120 6f62  nd long `Data ob
-00007170: 6a65 6374 6020 696e 7369 6465 2074 6865  ject` inside the
-00007180: 206c 6f6f 702e 2020 0a20 2020 2020 2020   loop.  .       
-00007190: 2020 2020 4974 276c 6c20 616c 6c6f 7720      It'll allow 
-000071a0: 796f 7520 6f70 656e 2074 6865 2063 6163  you open the cac
-000071b0: 6865 2066 696c 6520 6f72 2063 7265 6174  he file or creat
-000071c0: 6520 6120 7265 7175 6573 7420 746f 2060  e a request to `
-000071d0: 4461 7461 2073 6f75 7263 6560 206c 6573  Data source` les
-000071e0: 7320 6e75 6d62 6572 206f 6620 7469 6d65  s number of time
-000071f0: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
-00007200: 2020 2020 2320 342e 204f 6666 6963 6961      # 4. Officia
-00007210: 6c20 4461 7461 536f 7572 6365 2069 6d70  l DataSource imp
-00007220: 6c65 6d65 6e74 6174 696f 6e73 0a20 2020  lementations.   
-00007230: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
-00007240: 5b4c 6967 6874 7765 6967 6874 2044 6174  [Lightweight Dat
-00007250: 6120 5072 6f76 6964 6572 2044 6174 6120  a Provider Data 
-00007260: 536f 7572 6365 5d28 6874 7470 733a 2f2f  Source](https://
-00007270: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
-00007280: 6574 2f74 6832 2d64 732d 736f 7572 6365  et/th2-ds-source
-00007290: 2d6c 7764 7029 0a20 2020 2020 2020 200a  -lwdp).        .
-000072a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000072b0: 2023 2035 2e20 4150 490a 2020 2020 2020   # 5. API.      
-000072c0: 2020 0a20 2020 2020 2020 2049 6620 796f    .        If yo
-000072d0: 7520 6172 6520 6c6f 6f6b 696e 6720 666f  u are looking fo
-000072e0: 7220 636c 6173 7365 7320 6465 7363 7269  r classes descri
-000072f0: 7074 696f 6e20 7365 6520 7468 6520 5b41  ption see the [A
-00007300: 5049 2044 6f63 756d 656e 7461 7469 6f6e  PI Documentation
-00007310: 5d28 646f 6375 6d65 6e74 6174 696f 6e2f  ](documentation/
-00007320: 6170 692f 696e 6465 782e 6d64 292e 0a20  api/index.md).. 
-00007330: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007340: 2320 362e 2045 7861 6d70 6c65 730a 2020  # 6. Examples.  
-00007350: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
-00007360: 205b 6765 745f 7374 6172 7465 645f 6578   [get_started_ex
-00007370: 616d 706c 652e 7079 5d28 6578 616d 706c  ample.py](exampl
-00007380: 6573 2f67 6574 5f73 7461 7274 6564 5f65  es/get_started_e
-00007390: 7861 6d70 6c65 2e70 7929 0a20 2020 2020  xample.py).     
-000073a0: 2020 200a 506c 6174 666f 726d 3a20 554e     .Platform: UN
-000073b0: 4b4e 4f57 4e0a 5265 7175 6972 6573 2d50  KNOWN.Requires-P
-000073c0: 7974 686f 6e3a 203e 3d33 2e37 0a44 6573  ython: >=3.7.Des
-000073d0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-000073e0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-000073f0: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
-00007400: 7472 613a 2072 6470 0a50 726f 7669 6465  tra: rdp.Provide
-00007410: 732d 4578 7472 613a 2072 6470 350a 5072  s-Extra: rdp5.Pr
-00007420: 6f76 6964 6573 2d45 7874 7261 3a20 7264  ovides-Extra: rd
-00007430: 7036 0a50 726f 7669 6465 732d 4578 7472  p6.Provides-Extr
-00007440: 613a 206c 7764 700a 5072 6f76 6964 6573  a: lwdp.Provides
-00007450: 2d45 7874 7261 3a20 6c77 6470 310a 5072  -Extra: lwdp1.Pr
-00007460: 6f76 6964 6573 2d45 7874 7261 3a20 6c77  ovides-Extra: lw
-00007470: 6470 320a 5072 6f76 6964 6573 2d45 7874  dp2.Provides-Ext
-00007480: 7261 3a20 6c77 6470 2d64 6576 0a50 726f  ra: lwdp-dev.Pro
-00007490: 7669 6465 732d 4578 7472 613a 2075 7469  vides-Extra: uti
-000074a0: 6c73 2d72 7074 2d76 6965 7765 720a 5072  ls-rpt-viewer.Pr
-000074b0: 6f76 6964 6573 2d45 7874 7261 3a20 7574  ovides-Extra: ut
-000074c0: 696c 732d 7270 742d 7669 6577 6572 350a  ils-rpt-viewer5.
-000074d0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000074e0: 7574 696c 732d 6164 7661 6e63 6564 0a    utils-advanced.
+00003ee0: 332e 332e 315d 2047 6574 206c 6561 7665  3.3.1] Get leave
+00003ef0: 7320 6f66 2061 6c6c 2074 7265 6573 2e0a  s of all trees..
+00003f00: 2020 2020 2020 2020 6c65 6176 6573 3a20          leaves: 
+00003f10: 5475 706c 655b 6469 6374 5d20 3d20 6574  Tuple[dict] = et
+00003f20: 632e 6765 745f 6c65 6176 6573 2829 0a20  c.get_leaves(). 
+00003f30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003f40: 2320 5b33 2e33 2e32 5d20 4765 7420 726f  # [3.3.2] Get ro
+00003f50: 6f74 7320 6964 7320 6f66 2061 6c6c 2074  ots ids of all t
+00003f60: 7265 6573 2e0a 2020 2020 2020 2020 726f  rees..        ro
+00003f70: 6f74 733a 204c 6973 745b 7374 725d 203d  ots: List[str] =
+00003f80: 2065 7463 2e67 6574 5f72 6f6f 7473 5f69   etc.get_roots_i
+00003f90: 6473 2829 0a20 2020 2020 2020 200a 2020  ds().        .  
+00003fa0: 2020 2020 2020 2320 5b33 2e33 2e33 5d20        # [3.3.3] 
+00003fb0: 4669 6e64 2061 6e20 6576 656e 7420 696e  Find an event in
+00003fc0: 2061 6c6c 2074 7265 6573 2e0a 2020 2020   all trees..    
+00003fd0: 2020 2020 6669 6e64 5f65 7665 6e74 3a20      find_event: 
+00003fe0: 4f70 7469 6f6e 616c 5b64 6963 745d 203d  Optional[dict] =
+00003ff0: 2065 7463 2e66 696e 6428 6c61 6d62 6461   etc.find(lambda
+00004000: 2065 7665 6e74 3a20 2253 656e 6420 6d65   event: "Send me
+00004010: 7373 6167 6522 2069 6e20 6576 656e 745b  ssage" in event[
+00004020: 2265 7665 6e74 5479 7065 225d 290a 2020  "eventType"]).  
+00004030: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00004040: 205b 332e 332e 345d 2046 696e 6420 616c   [3.3.4] Find al
+00004050: 6c20 6576 656e 7473 2069 6e20 616c 6c20  l events in all 
+00004060: 7472 6565 732e 2054 6865 7265 2069 7320  trees. There is 
+00004070: 616c 736f 2069 7465 7261 626c 6520 7665  also iterable ve
+00004080: 7273 696f 6e20 2766 696e 6461 6c6c 5f69  rsion 'findall_i
+00004090: 7465 7227 2e0a 2020 2020 2020 2020 6669  ter'..        fi
+000040a0: 6e64 5f65 7665 6e74 733a 204c 6973 745b  nd_events: List[
+000040b0: 6469 6374 5d20 3d20 6574 632e 6669 6e64  dict] = etc.find
+000040c0: 616c 6c28 6c61 6d62 6461 2065 7665 6e74  all(lambda event
+000040d0: 3a20 6576 656e 745b 2273 7563 6365 7373  : event["success
+000040e0: 6675 6c22 5d20 6973 2054 7275 6529 0a20  ful"] is True). 
+000040f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00004100: 2320 5b33 2e33 2e35 5d20 4669 6e64 2061  # [3.3.5] Find a
+00004110: 6e20 616e 6365 7374 6f72 206f 6620 7468  n ancestor of th
+00004120: 6520 6576 656e 742e 0a20 2020 2020 2020  e event..       
+00004130: 2061 6e63 6573 746f 723a 204f 7074 696f   ancestor: Optio
+00004140: 6e61 6c5b 6469 6374 5d20 3d20 6574 632e  nal[dict] = etc.
+00004150: 6669 6e64 5f61 6e63 6573 746f 7228 0a20  find_ancestor(. 
+00004160: 2020 2020 2020 2020 2020 2022 3862 6265             "8bbe
+00004170: 3337 3137 2d63 6635 392d 3131 6562 2d61  3717-cf59-11eb-a
+00004180: 3366 372d 3039 3466 3930 3463 3361 3632  3f7-094f904c3a62
+00004190: 222c 2066 696c 7465 723d 6c61 6d62 6461  ", filter=lambda
+000041a0: 2065 7665 6e74 3a20 2252 6f6f 7445 7665   event: "RootEve
+000041b0: 6e74 2220 696e 2065 7665 6e74 5b22 6576  nt" in event["ev
+000041c0: 656e 744e 616d 6522 5d0a 2020 2020 2020  entName"].      
+000041d0: 2020 290a 2020 2020 2020 2020 0a20 2020    ).        .   
+000041e0: 2020 2020 2023 205b 332e 332e 365d 2047       # [3.3.6] G
+000041f0: 6574 2063 6869 6c64 7265 6e20 6f66 2074  et children of t
+00004200: 6865 2065 7665 6e74 2e20 5468 6572 6520  he event. There 
+00004210: 6973 2061 6c73 6f20 6974 6572 6162 6c65  is also iterable
+00004220: 2076 6572 7369 6f6e 2027 6765 745f 6368   version 'get_ch
+00004230: 696c 6472 656e 5f69 7465 7227 2e0a 2020  ildren_iter'..  
+00004240: 2020 2020 2020 6368 696c 6472 656e 3a20        children: 
+00004250: 5475 706c 655b 6469 6374 5d20 3d20 6574  Tuple[dict] = et
+00004260: 632e 6765 745f 6368 696c 6472 656e 2822  c.get_children("
+00004270: 3831 3434 3232 6531 2d39 6336 382d 3131  814422e1-9c68-11
+00004280: 6562 2d38 3539 382d 3639 3165 6264 3766  eb-8598-691ebd7f
+00004290: 3431 3364 2229 0a20 2020 2020 2020 200a  413d").        .
+000042a0: 2020 2020 2020 2020 2320 5b33 2e33 2e37          # [3.3.7
+000042b0: 5d20 4765 7420 7375 6274 7265 6520 666f  ] Get subtree fo
+000042c0: 7220 7370 6563 6966 6965 6420 6576 656e  r specified even
+000042d0: 742e 0a20 2020 2020 2020 2073 7562 7472  t..        subtr
+000042e0: 6565 3a20 4576 656e 7454 7265 6520 3d20  ee: EventTree = 
+000042f0: 6574 632e 6765 745f 7375 6274 7265 6528  etc.get_subtree(
+00004300: 2238 6532 3337 3734 642d 6366 3539 2d31  "8e23774d-cf59-1
+00004310: 3165 622d 6136 6533 2d35 3562 6664 6232  1eb-a6e3-55bfdb2
+00004320: 6233 6632 3122 290a 2020 2020 2020 2020  b3f21").        
+00004330: 0a20 2020 2020 2020 2023 205b 332e 332e  .        # [3.3.
+00004340: 385d 2047 6574 2066 756c 6c20 7061 7468  8] Get full path
+00004350: 2074 6f20 7468 6520 6576 656e 742e 0a20   to the event.. 
+00004360: 2020 2020 2020 2023 204c 6f6f 6b73 206c         # Looks l
+00004370: 696b 6520 5b61 6e63 6573 746f 725f 726f  ike [ancestor_ro
+00004380: 6f74 2c20 616e 6365 7374 6f72 5f6c 6576  ot, ancestor_lev
+00004390: 656c 312c 2061 6e63 6573 746f 725f 6c65  el1, ancestor_le
+000043a0: 7665 6c32 2c20 6576 656e 745d 0a20 2020  vel2, event].   
+000043b0: 2020 2020 2065 7665 6e74 5f70 6174 683a       event_path:
+000043c0: 204c 6973 745b 6469 6374 5d20 3d20 6574   List[dict] = et
+000043d0: 632e 6765 745f 6675 6c6c 5f70 6174 6828  c.get_full_path(
+000043e0: 2238 6532 3532 3466 612d 6366 3539 2d31  "8e2524fa-cf59-1
+000043f0: 3165 622d 6133 6637 2d30 3934 6639 3034  1eb-a3f7-094f904
+00004400: 6333 6136 3222 290a 2020 2020 2020 2020  c3a62").        
+00004410: 0a20 2020 2020 2020 2023 205b 332e 332e  .        # [3.3.
+00004420: 395d 2047 6574 2070 6172 656e 7420 6f66  9] Get parent of
+00004430: 2074 6865 2065 7665 6e74 2e0a 2020 2020   the event..    
+00004440: 2020 2020 7061 7265 6e74 203d 2065 7463      parent = etc
+00004450: 2e67 6574 5f70 6172 656e 7428 2238 6532  .get_parent("8e2
+00004460: 3532 3466 612d 6366 3539 2d31 3165 622d  524fa-cf59-11eb-
+00004470: 6133 6637 2d30 3934 6639 3034 6333 6136  a3f7-094f904c3a6
+00004480: 3222 290a 2020 2020 2020 2020 0a20 2020  2").        .   
+00004490: 2020 2020 2023 205b 332e 332e 3130 5d20       # [3.3.10] 
+000044a0: 4170 7065 6e64 206e 6577 2065 7665 6e74  Append new event
+000044b0: 2074 6f20 7468 6520 636f 6c6c 6563 7469   to the collecti
+000044c0: 6f6e 2e0a 2020 2020 2020 2020 6574 632e  on..        etc.
+000044d0: 6170 7065 6e64 5f65 7665 6e74 280a 2020  append_event(.  
+000044e0: 2020 2020 2020 2020 2020 6576 656e 743d            event=
+000044f0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00004500: 2020 2265 7665 6e74 4964 223a 2022 6132    "eventId": "a2
+00004510: 3066 3565 6634 2d63 3366 652d 6262 3130  0f5ef4-c3fe-bb10
+00004520: 2d61 3239 632d 6464 3364 3738 3439 3039  -a29c-dd3d784909
+00004530: 6562 222c 0a20 2020 2020 2020 2020 2020  eb",.           
+00004540: 2020 2020 2022 7061 7265 6e74 4576 656e       "parentEven
+00004550: 7449 6422 3a20 2238 6532 3532 3466 612d  tId": "8e2524fa-
+00004560: 6366 3539 2d31 3165 622d 6133 6637 2d30  cf59-11eb-a3f7-0
+00004570: 3934 6639 3034 6333 6136 3222 2c0a 2020  94f904c3a62",.  
+00004580: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00004590: 7665 6e74 4e61 6d65 223a 2022 5374 7562  ventName": "Stub
+000045a0: 4576 656e 7422 2c0a 2020 2020 2020 2020  Event",.        
+000045b0: 2020 2020 7d0a 2020 2020 2020 2020 290a      }.        ).
+000045c0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000045d0: 2023 205b 332e 332e 3131 5d20 5368 6f77   # [3.3.11] Show
+000045e0: 2074 6865 2065 6e74 6972 6520 636f 6c6c   the entire coll
+000045f0: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
+00004600: 6574 632e 7368 6f77 2829 0a20 2020 2020  etc.show().     
+00004610: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
+00004620: 2e34 5d20 576f 726b 696e 6720 7769 7468  .4] Working with
+00004630: 2074 6865 2045 7665 6e74 5472 6565 2e0a   the EventTree..
+00004640: 2020 2020 2020 2020 2320 4576 656e 7454          # EventT
+00004650: 7265 6520 6861 7320 7468 6520 7361 6d65  ree has the same
+00004660: 206d 6574 686f 6473 2061 7320 4576 656e   methods as Even
+00004670: 7454 7265 6543 6f6c 6c65 6374 696f 6e2c  tTreeCollection,
+00004680: 2062 7574 206f 6e6c 7920 666f 7220 6974   but only for it
+00004690: 7320 6f77 6e20 7472 6565 2e0a 2020 2020  s own tree..    
+000046a0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
+000046b0: 332e 342e 315d 2047 6574 2063 6f6c 6c65  3.4.1] Get colle
+000046c0: 6374 696f 6e20 7472 6565 732e 0a20 2020  ction trees..   
+000046d0: 2020 2020 2074 7265 6573 3a20 4c69 7374       trees: List
+000046e0: 5b45 7665 6e74 5472 6565 5d20 3d20 6574  [EventTree] = et
+000046f0: 632e 6765 745f 7472 6565 7328 290a 2020  c.get_trees().  
+00004700: 2020 2020 2020 7472 6565 3a20 4576 656e        tree: Even
+00004710: 7454 7265 6520 3d20 7472 6565 735b 305d  tTree = trees[0]
+00004720: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00004730: 2020 2320 4275 7420 4576 656e 7454 7265    # But EventTre
+00004740: 6520 7072 6f76 6964 6573 2061 2077 6f72  e provides a wor
+00004750: 6b20 7769 7468 2074 6865 2074 7265 652c  k with the tree,
+00004760: 2062 7574 2064 6f65 7320 6e6f 7420 6d6f   but does not mo
+00004770: 6469 6679 2069 742e 0a20 2020 2020 2020  dify it..       
+00004780: 2023 2049 6620 796f 7520 7761 6e74 2074   # If you want t
+00004790: 6f20 6d6f 6469 6679 2074 6865 2074 7265  o modify the tre
+000047a0: 652c 2075 7365 2045 7665 6e74 5472 6565  e, use EventTree
+000047b0: 436f 6c6c 6563 7469 6f6e 732e 0a20 2020  Collections..   
+000047c0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+000047d0: 5b33 2e35 5d20 576f 726b 696e 6720 7769  [3.5] Working wi
+000047e0: 7468 2050 6172 656e 746c 6573 7354 7265  th ParentlessTre
+000047f0: 652e 0a20 2020 2020 2020 2023 2050 6172  e..        # Par
+00004800: 656e 746c 6573 7354 7265 6520 6973 2045  entlessTree is E
+00004810: 7665 6e74 5472 6565 2077 6869 6368 2068  ventTree which h
+00004820: 6173 2064 6574 6163 6865 6420 6576 656e  as detached even
+00004830: 7473 2077 6974 6820 7374 7562 732e 0a20  ts with stubs.. 
+00004840: 2020 2020 2020 2070 6172 656e 746c 6573         parentles
+00004850: 735f 7472 6565 733a 204c 6973 745b 4576  s_trees: List[Ev
+00004860: 656e 7454 7265 655d 203d 2065 7463 2e67  entTree] = etc.g
+00004870: 6574 5f70 6172 656e 746c 6573 735f 7472  et_parentless_tr
+00004880: 6565 7328 290a 2020 2020 2020 2020 0a20  ees().        . 
+00004890: 2020 2020 2020 2023 205b 332e 365d 2057         # [3.6] W
+000048a0: 6f72 6b69 6e67 2077 6974 6820 5061 7265  orking with Pare
+000048b0: 6e74 4576 656e 7454 7265 6543 6f6c 6c65  ntEventTreeColle
+000048c0: 6374 696f 6e2e 0a20 2020 2020 2020 2023  ction..        #
+000048d0: 2050 6172 656e 7445 7665 6e74 5472 6565   ParentEventTree
+000048e0: 436f 6c6c 6563 7469 6f6e 2069 7320 6120  Collection is a 
+000048f0: 7472 6565 2063 6f6c 6c65 6374 696f 6e20  tree collection 
+00004900: 6c69 6b65 2045 7665 6e74 5472 6565 436f  like EventTreeCo
+00004910: 6c6c 6563 7469 6f6e 2c0a 2020 2020 2020  llection,.      
+00004920: 2020 2320 6275 7420 6974 2068 6173 206f    # but it has o
+00004930: 6e6c 7920 6576 656e 7473 2074 6861 7420  nly events that 
+00004940: 6861 7665 2072 6566 6572 656e 6365 732e  have references.
+00004950: 0a20 2020 2020 2020 2064 6174 615f 736f  .        data_so
+00004960: 7572 6365 3a20 4944 6174 6153 6f75 7263  urce: IDataSourc
+00004970: 6520 2023 2059 6f75 2073 686f 756c 6420  e  # You should 
+00004980: 696e 6974 2044 6174 6153 6f75 7263 6520  init DataSource 
+00004990: 6f62 6a65 6374 2e20 452e 672e 2066 726f  object. E.g. fro
+000049a0: 6d20 4c77 4450 206d 6f64 756c 652e 0a20  m LwDP module.. 
+000049b0: 2020 2020 2020 2023 2045 5443 4472 6976         # ETCDriv
+000049c0: 6572 2068 6572 6520 6973 2061 2073 7475  er here is a stu
+000049d0: 622c 2061 6374 7561 6c6c 7920 7468 6520  b, actually the 
+000049e0: 6c69 6220 646f 6e27 7420 6861 7665 2073  lib don't have s
+000049f0: 7563 6820 636c 6173 732e 0a20 2020 2020  uch class..     
+00004a00: 2020 2023 2059 6f75 2063 616e 2074 616b     # You can tak
+00004a10: 6520 6974 2069 6e20 4c77 4450 206d 6f64  e it in LwDP mod
+00004a20: 756c 6520 6f72 2063 7265 6174 6520 796f  ule or create yo
+00004a30: 7572 7365 6c66 2063 6c61 7373 2069 6620  urself class if 
+00004a40: 796f 7520 6861 7665 2073 6f6d 6520 7370  you have some sp
+00004a50: 6563 6961 6c20 6576 656e 7473 2073 7472  ecial events str
+00004a60: 7563 7475 7265 2e0a 2020 2020 2020 2020  ucture..        
+00004a70: 6472 6976 6572 203d 2045 5443 4472 6976  driver = ETCDriv
+00004a80: 6572 2864 6174 615f 736f 7572 6365 3d64  er(data_source=d
+00004a90: 6174 615f 736f 7572 6365 290a 2020 2020  ata_source).    
+00004aa0: 2020 2020 6574 6320 3d20 5061 7265 6e74      etc = Parent
+00004ab0: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
+00004ac0: 696f 6e28 6472 6976 6572 290a 2020 2020  ion(driver).    
+00004ad0: 2020 2020 6574 632e 6275 696c 6428 6576      etc.build(ev
+00004ae0: 656e 7473 290a 2020 2020 2020 2020 0a20  ents).        . 
+00004af0: 2020 2020 2020 2065 7463 2e73 686f 7728         etc.show(
+00004b00: 290a 2020 2020 2020 2020 6060 600a 2020  ).        ```.  
+00004b10: 2020 2020 2020 3c21 2d2d 2065 6e64 2067        <!-- end g
+00004b20: 6574 5f73 7461 7274 6564 5f65 7861 6d70  et_started_examp
+00004b30: 6c65 2e70 7920 2d2d 3e0a 2020 2020 2020  le.py -->.      
+00004b40: 2020 0a20 2020 2020 2020 2023 2320 322e    .        ## 2.
+00004b50: 332e 2053 686f 7274 2074 6865 6f72 790a  3. Short theory.
+00004b60: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004b70: 2054 6865 206c 6962 7261 7279 2070 726f   The library pro
+00004b80: 7669 6465 7320 746f 6f6c 7320 666f 7220  vides tools for 
+00004b90: 6861 6e64 6c69 6e67 2073 7472 6561 6d20  handling stream 
+00004ba0: 6461 7461 2e20 5768 6174 2773 2061 2073  data. What's a s
+00004bb0: 7472 6561 6d3f 2049 7427 7320 6120 7365  tream? It's a se
+00004bc0: 7175 656e 6365 206f 6620 656c 656d 656e  quence of elemen
+00004bd0: 7473 2066 726f 6d20 6120 736f 7572 6365  ts from a source
+00004be0: 2074 6861 740a 2020 2020 2020 2020 7375   that.        su
+00004bf0: 7070 6f72 7473 2061 6767 7265 6761 7465  pports aggregate
+00004c00: 206f 7065 7261 7469 6f6e 732e 0a20 2020   operations..   
+00004c10: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
+00004c20: 2320 5465 726d 730a 2020 2020 2020 2020  # Terms.        
+00004c30: 0a20 2020 2020 2020 202d 202a 2a44 6174  .        - **Dat
+00004c40: 6120 6f62 6a65 6374 2a2a 3a20 416e 2069  a object**: An i
+00004c50: 6e73 7461 6e63 6520 6f66 2060 4461 7461  nstance of `Data
+00004c60: 6020 636c 6173 7320 7768 6963 6820 6973  ` class which is
+00004c70: 2077 7261 7070 6572 2075 6e64 6572 2073   wrapper under s
+00004c80: 7472 6561 6d2e 0a20 2020 2020 2020 202d  tream..        -
+00004c90: 202a 2a53 6571 7565 6e63 6520 6f66 2065   **Sequence of e
+00004ca0: 6c65 6d65 6e74 732a 2a3a 0a20 2020 2020  lements**:.     
+00004cb0: 2020 2020 2041 205f 4461 7461 206f 626a       A _Data obj
+00004cc0: 6563 745f 2070 726f 7669 6465 7320 616e  ect_ provides an
+00004cd0: 2069 6e74 6572 6661 6365 2074 6f20 6120   interface to a 
+00004ce0: 7365 7175 656e 6365 6420 7365 7420 6f66  sequenced set of
+00004cf0: 2076 616c 7565 7320 6f66 2061 2073 7065   values of a spe
+00004d00: 6369 6669 6320 656c 656d 656e 7420 7479  cific element ty
+00004d10: 7065 2e20 5374 7265 616d 2069 6e73 6964  pe. Stream insid
+00004d20: 6520 7468 6520 5f44 6174 610a 2020 2020  e the _Data.    
+00004d30: 2020 2020 2020 6f62 6a65 6374 5f20 2a2a        object_ **
+00004d40: 646f 6e19 7420 6163 7475 616c 6c79 2073  don.t actually s
+00004d50: 746f 7265 2a2a 2065 6c65 6d65 6e74 733b  tore** elements;
+00004d60: 2074 6865 7920 6172 6520 636f 6d70 7574   they are comput
+00004d70: 6564 206f 6e20 6465 6d61 6e64 2e0a 2020  ed on demand..  
+00004d80: 2020 2020 2020 2d20 2a2a 6461 7461 2073        - **data s
+00004d90: 6f75 7263 652a 2a20 2865 7861 6374 6c79  ource** (exactly
+00004da0: 2069 6e20 736d 616c 6c20 6c65 7474 6572   in small letter
+00004db0: 7329 3a0a 2020 2020 2020 2020 2020 416e  s):.          An
+00004dc0: 7920 736f 7572 6365 206f 6620 6461 7461  y source of data
+00004dd0: 2e20 452e 672e 205b 4c69 6768 7477 6569  . E.g. [Lightwei
+00004de0: 6768 7420 4461 7461 2050 726f 7669 6465  ght Data Provide
+00004df0: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
+00004e00: 622e 636f 6d2f 7468 322d 6e65 742f 7468  b.com/th2-net/th
+00004e10: 322d 6c77 2d64 6174 612d 7072 6f76 6964  2-lw-data-provid
+00004e20: 6572 292c 2063 6f6c 6c65 6374 696f 6e73  er), collections
+00004e30: 2c0a 2020 2020 2020 2020 2020 6172 7261  ,.          arra
+00004e40: 7973 2c20 6f72 2049 2f4f 2072 6573 6f75  ys, or I/O resou
+00004e50: 7263 6573 2e0a 2020 2020 2020 2020 2d20  rces..        - 
+00004e60: 2a2a 4461 7461 536f 7572 6365 2a2a 3a0a  **DataSource**:.
+00004e70: 2020 2020 2020 2020 2020 4120 636c 6173            A clas
+00004e80: 7320 7468 6174 2069 7320 616e 2069 6e74  s that is an int
+00004e90: 6572 6d65 6469 6174 6520 6c69 6e6b 2062  ermediate link b
+00004ea0: 6574 7765 656e 2074 6865 2053 6f75 7263  etween the Sourc
+00004eb0: 6541 5049 2061 6e64 2043 6f6d 6d61 6e64  eAPI and Command
+00004ec0: 732e 0a20 2020 2020 2020 202d 202a 2a53  s..        - **S
+00004ed0: 6f75 7263 6541 5049 2a2a 3a0a 2020 2020  ourceAPI**:.    
+00004ee0: 2020 2020 2020 4561 6368 2073 6f75 7263        Each sourc
+00004ef0: 6520 6861 7320 6974 7320 6f77 6e20 4150  e has its own AP
+00004f00: 4920 746f 2072 6574 7269 6576 6520 6461  I to retrieve da
+00004f10: 7461 2e20 536f 7572 6365 4150 4920 6973  ta. SourceAPI is
+00004f20: 2061 2063 6c61 7373 2074 6861 7420 7072   a class that pr
+00004f30: 6f76 6964 6520 4150 4920 666f 7220 736f  ovide API for so
+00004f40: 6d65 2064 6174 6120 736f 7572 6365 2e0a  me data source..
+00004f50: 2020 2020 2020 2020 2d20 2a2a 436f 6d6d          - **Comm
+00004f60: 616e 6473 2a2a 3a0a 2020 2020 2020 2020  ands**:.        
+00004f70: 2020 436c 6173 7365 7320 7468 6174 2070    Classes that p
+00004f80: 726f 7669 6465 2075 7365 722d 6672 6965  rovide user-frie
+00004f90: 6e64 6c79 2069 6e74 6572 6661 6365 7320  ndly interfaces 
+00004fa0: 666f 7220 6765 7474 696e 6720 736f 6d65  for getting some
+00004fb0: 2064 6174 6120 6672 6f6d 2044 6174 6153   data from DataS
+00004fc0: 6f75 7263 652e 2043 6f6d 6d61 6e64 7320  ource. Commands 
+00004fd0: 7573 6520 5f53 6f75 7263 6541 5049 5f20  use _SourceAPI_ 
+00004fe0: 746f 0a20 2020 2020 2020 2020 2061 6368  to.          ach
+00004ff0: 6965 7665 2069 742e 0a20 2020 2020 2020  ieve it..       
+00005000: 202d 202a 2a41 6461 7074 6572 732a 2a3a   - **Adapters**:
+00005010: 0a20 2020 2020 2020 2020 2049 7427 7320  .          It's 
+00005020: 7369 6d69 6c61 7220 746f 2066 756e 6374  similar to funct
+00005030: 696f 6e20 666f 7220 6044 6174 612e 6d61  ion for `Data.ma
+00005040: 7060 206d 6574 686f 642e 2041 646f 7074  p` method. Adopt
+00005050: 6162 6c65 2063 6f6d 6d61 6e64 7320 7573  able commands us
+00005060: 6564 2069 7420 746f 2075 7064 6174 6520  ed it to update 
+00005070: 7468 6520 6461 7461 2073 7472 6561 6d2e  the data stream.
+00005080: 0a20 2020 2020 2020 202d 202a 2a41 6767  .        - **Agg
+00005090: 7265 6761 7465 206f 7065 7261 7469 6f6e  regate operation
+000050a0: 732a 2a3a 0a20 2020 2020 2020 2020 2043  s**:.          C
+000050b0: 6f6d 6d6f 6e20 6f70 6572 6174 696f 6e73  ommon operations
+000050c0: 2073 7563 6820 6173 2066 696c 7465 722c   such as filter,
+000050d0: 206d 6170 2c20 6c69 6d69 7420 616e 6420   map, limit and 
+000050e0: 736f 206f 6e2e 0a20 2020 2020 2020 202d  so on..        -
+000050f0: 202a 2a57 6f72 6b66 6c6f 772a 2a3a 2041   **Workflow**: A
+00005100: 6e20 6f72 6465 7265 6420 7365 7420 6f66  n ordered set of
+00005110: 205f 4167 6772 6567 6174 6520 6f70 6572   _Aggregate oper
+00005120: 6174 696f 6e73 5f2e 0a20 2020 2020 2020  ations_..       
+00005130: 200a 2020 2020 2020 2020 2323 2320 436f   .        ### Co
+00005140: 6e63 6570 740a 2020 2020 2020 2020 0a20  ncept.        . 
+00005150: 2020 2020 2020 2054 6865 206c 6962 7261         The libra
+00005160: 7279 2064 6573 6372 6962 6573 2074 6865  ry describes the
+00005170: 2068 6967 682d 6c65 7665 6c20 696e 7465   high-level inte
+00005180: 7266 6163 6573 2060 4953 6f75 7263 6541  rfaces `ISourceA
+00005190: 5049 602c 2060 4944 6174 6153 6f75 7263  PI`, `IDataSourc
+000051a0: 6560 2c20 6049 436f 6d6d 616e 6460 2c20  e`, `ICommand`, 
+000051b0: 6049 4164 6170 7465 7260 2e0a 2020 2020  `IAdapter`..    
+000051c0: 2020 2020 0a20 2020 2020 2020 2041 6e79      .        Any
+000051d0: 2064 6174 6120 736f 7572 6365 206d 7573   data source mus
+000051e0: 7420 6265 2064 6573 6372 6962 6564 2062  t be described b
+000051f0: 7920 7468 6520 6049 4461 7461 536f 7572  y the `IDataSour
+00005200: 6365 6020 6162 7374 7261 6374 2063 6c61  ce` abstract cla
+00005210: 7373 2e20 5468 6573 6520 6361 6e20 6265  ss. These can be
+00005220: 205f 4669 6c65 4461 7461 536f 7572 6365   _FileDataSource
+00005230: 5f2c 200a 2020 2020 2020 2020 5f43 5356  _, .        _CSV
+00005240: 4461 7461 536f 7572 6365 5f2c 205f 4442  DataSource_, _DB
+00005250: 4461 7461 536f 7572 6365 5f20 616e 6420  DataSource_ and 
+00005260: 6f74 6865 722e 0a20 2020 2020 2020 200a  other..        .
+00005270: 2020 2020 2020 2020 5573 7561 6c6c 792c          Usually,
+00005280: 2064 6174 6120 736f 7572 6365 7320 6861   data sources ha
+00005290: 7665 2073 6f6d 6520 6b69 6e64 206f 6620  ve some kind of 
+000052a0: 4150 492e 2044 6174 6162 6173 6573 202d  API. Databases -
+000052b0: 2070 726f 7669 6465 2053 514c 206c 616e   provide SQL lan
+000052c0: 6775 6167 652c 2077 6865 6e20 776f 726b  guage, when work
+000052d0: 696e 6720 7769 7468 2061 2066 696c 652c  ing with a file,
+000052e0: 2079 6f75 2063 616e 2072 6561 640a 2020   you can read.  
+000052f0: 2020 2020 2020 6c69 6e65 2062 7920 6c69        line by li
+00005300: 6e65 2c20 6574 632e 2054 6869 7320 4150  ne, etc. This AP
+00005310: 4920 6973 2064 6573 6372 6962 6564 2062  I is described b
+00005320: 7920 7468 6520 6049 536f 7572 6365 4150  y the `ISourceAP
+00005330: 4960 2063 6c61 7373 2e20 4265 6361 7573  I` class. Becaus
+00005340: 6520 6469 6666 6572 656e 7420 7665 7273  e different vers
+00005350: 696f 6e73 206f 6620 7468 6520 7361 6d65  ions of the same
+00005360: 2064 6174 6120 736f 7572 6365 0a20 2020   data source.   
+00005370: 2020 2020 206d 6179 2068 6176 6520 6469       may have di
+00005380: 6666 6572 656e 7420 4150 492c 2069 7420  fferent API, it 
+00005390: 6973 2062 6574 7465 7220 746f 2063 7265  is better to cre
+000053a0: 6174 6520 6120 636c 6173 7320 666f 7220  ate a class for 
+000053b0: 6561 6368 2076 6572 7369 6f6e 2e0a 2020  each version..  
+000053c0: 2020 2020 2020 0a20 2020 2020 2020 2047        .        G
+000053d0: 656e 6572 616c 6c79 2c20 6461 7461 2073  enerally, data s
+000053e0: 6f75 7263 6520 4150 4973 2061 7265 2068  ource APIs are h
+000053f0: 6964 6465 6e20 6265 6869 6e64 2063 6f6e  idden behind con
+00005400: 7665 6e69 656e 7420 696e 7465 7266 6163  venient interfac
+00005410: 6573 2e20 5468 6520 726f 6c65 206f 6620  es. The role of 
+00005420: 7468 6573 6520 696e 7465 7266 6163 6573  these interfaces
+00005430: 2069 7320 706c 6179 6564 0a20 2020 2020   is played.     
+00005440: 2020 2062 7920 6049 436f 6d6d 616e 6460     by `ICommand`
+00005450: 2063 6c61 7373 6573 2e0a 2020 2020 2020   classes..      
+00005460: 2020 0a20 2020 2020 2020 2060 4941 6461    .        `IAda
+00005470: 7074 6572 6020 636c 6173 7365 7320 7472  pter` classes tr
+00005480: 616e 7366 6f72 6d20 6461 7461 2073 7472  ansform data str
+00005490: 6561 6d20 6c69 6b65 2066 756e 6374 696f  eam like functio
+000054a0: 6e73 2066 6f72 2060 4461 7461 2e6d 6170  ns for `Data.map
+000054b0: 6020 6d65 7468 6f64 2e20 4573 7365 6e74  ` method. Essent
+000054c0: 6961 6c6c 7920 6974 2773 2074 6865 2073  ially it's the s
+000054d0: 616d 6520 7468 696e 6720 6275 7420 6d6f  ame thing but mo
+000054e0: 7265 0a20 2020 2020 2020 2066 6c65 7869  re.        flexi
+000054f0: 626c 652e 0a20 2020 2020 2020 200a 2020  ble..        .  
+00005500: 2020 2020 2020 466f 7220 6578 616d 706c        For exampl
+00005510: 652c 204c 7744 5020 4461 7461 536f 7572  e, LwDP DataSour
+00005520: 6365 2868 7474 7073 3a2f 2f67 6974 6875  ce(https://githu
+00005530: 622e 636f 6d2f 7468 322d 6e65 742f 7468  b.com/th2-net/th
+00005540: 322d 6473 2d73 6f75 7263 652d 6c77 6470  2-ds-source-lwdp
+00005550: 2920 7573 6573 2074 6865 7365 2061 6273  ) uses these abs
+00005560: 7472 6163 7420 636c 6173 7365 7320 746f  tract classes to
+00005570: 2062 7569 6c64 2069 7473 2069 6d70 6c65   build its imple
+00005580: 6d65 6e74 6174 696f 6e2e 596f 7520 6361  mentation.You ca
+00005590: 6e20 6561 7369 6c79 2063 7265 6174 6520  n easily create 
+000055a0: 796f 7572 206f 776e 2075 6e69 7175 6520  your own unique 
+000055b0: 636f 6d6d 616e 6473 2066 6f72 205f 4c77  commands for _Lw
+000055c0: 4450 2044 6174 6153 6f75 7263 655f 2c20  DP DataSource_, 
+000055d0: 6173 2077 656c 6c20 6173 2065 6e74 6972  as well as entir
+000055e0: 650a 2020 2020 2020 2020 5f44 6174 6153  e.        _DataS
+000055f0: 6f75 7263 655f 2063 6c61 7373 6573 2e20  ource_ classes. 
+00005600: 5b48 6572 6520 6973 2061 2064 6f63 756d  [Here is a docum
+00005610: 656e 7461 7469 6f6e 5d28 646f 6375 6d65  entation](docume
+00005620: 6e74 6174 696f 6e2f 6461 7461 736f 7572  ntation/datasour
+00005630: 6365 2e6d 6429 206f 6e20 686f 7720 746f  ce.md) on how to
+00005640: 2069 6d70 6c65 6d65 6e74 2074 6865 7365   implement these
+00005650: 2069 6e74 6572 6661 6365 732e 0a20 2020   interfaces..   
+00005660: 2020 2020 200a 2020 2020 2020 2020 215b       .        ![
+00005670: 4461 7461 2073 7472 6561 6d20 7069 7065  Data stream pipe
+00005680: 6c69 6e65 5d28 646f 6375 6d65 6e74 6174  line](documentat
+00005690: 696f 6e2f 696d 672f 636f 6e63 6570 742e  ion/img/concept.
+000056a0: 706e 6729 0a20 2020 2020 2020 200a 2020  png).        .  
+000056b0: 2020 2020 2020 2323 2320 5374 7265 616d        ### Stream
+000056c0: 206f 7065 7261 7469 6f6e 730a 2020 2020   operations.    
+000056d0: 2020 2020 0a20 2020 2020 2020 2046 7572      .        Fur
+000056e0: 7468 6572 6d6f 7265 2c20 7374 7265 616d  thermore, stream
+000056f0: 206f 7065 7261 7469 6f6e 7320 6861 7665   operations have
+00005700: 2074 776f 2066 756e 6461 6d65 6e74 616c   two fundamental
+00005710: 2063 6861 7261 6374 6572 6973 7469 6373   characteristics
+00005720: 2074 6861 7420 6d61 6b65 2074 6865 6d20   that make them 
+00005730: 7665 7279 2064 6966 6665 7265 6e74 2066  very different f
+00005740: 726f 6d20 636f 6c6c 6563 7469 6f6e 0a20  rom collection. 
+00005750: 2020 2020 2020 206f 7065 7261 7469 6f6e         operation
+00005760: 733a 205f 5069 7065 6c69 6e69 6e67 5f20  s: _Pipelining_ 
+00005770: 616e 6420 5f49 6e74 6572 6e61 6c20 6974  and _Internal it
+00005780: 6572 6174 696f 6e5f 2e0a 2020 2020 2020  eration_..      
+00005790: 2020 0a20 2020 2020 2020 2023 2323 2320    .        #### 
+000057a0: 5069 7065 6c69 6e69 6e67 0a20 2020 2020  Pipelining.     
+000057b0: 2020 200a 2020 2020 2020 2020 4d61 6e79     .        Many
+000057c0: 2073 7472 6561 6d20 6f70 6572 6174 696f   stream operatio
+000057d0: 6e73 2072 6574 7572 6e20 6120 7374 7265  ns return a stre
+000057e0: 616d 2074 6865 6d73 656c 7665 732e 2054  am themselves. T
+000057f0: 6869 7320 616c 6c6f 7773 206f 7065 7261  his allows opera
+00005800: 7469 6f6e 7320 746f 2062 6520 6368 6169  tions to be chai
+00005810: 6e65 6420 746f 2066 6f72 6d20 6120 6c61  ned to form a la
+00005820: 7267 6572 2070 6970 656c 696e 652e 0a20  rger pipeline.. 
+00005830: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005840: 215b 4461 7461 2073 7472 6561 6d20 7069  ![Data stream pi
+00005850: 7065 6c69 6e65 5d28 646f 6375 6d65 6e74  peline](document
+00005860: 6174 696f 6e2f 696d 672f 6461 7461 5f73  ation/img/data_s
+00005870: 7472 6561 6d5f 7069 7065 6c69 6e65 2e70  tream_pipeline.p
+00005880: 6e67 290a 2020 2020 2020 2020 0a20 2020  ng).        .   
+00005890: 2020 2020 2023 2323 2320 496e 7465 726e       #### Intern
+000058a0: 616c 2069 7465 7261 7469 6f6e 0a20 2020  al iteration.   
+000058b0: 2020 2020 200a 2020 2020 2020 2020 496e       .        In
+000058c0: 2063 6f6e 7472 6173 7420 746f 2063 6f6c   contrast to col
+000058d0: 6c65 6374 696f 6e73 2c20 7768 6963 6820  lections, which 
+000058e0: 6172 6520 6974 6572 6174 6564 2065 7870  are iterated exp
+000058f0: 6c69 6369 746c 7920 2865 7874 6572 6e61  licitly (externa
+00005900: 6c20 6974 6572 6174 696f 6e29 2c20 7374  l iteration), st
+00005910: 7265 616d 206f 7065 7261 7469 6f6e 7320  ream operations 
+00005920: 646f 2074 6865 2069 7465 7261 7469 6f6e  do the iteration
+00005930: 0a20 2020 2020 2020 2062 6568 696e 6420  .        behind 
+00005940: 7468 6520 7363 656e 6573 2066 6f72 2079  the scenes for y
+00005950: 6f75 2e20 4e6f 7465 2c20 6974 2064 6f65  ou. Note, it doe
+00005960: 736e 2774 206d 6561 6e20 796f 7520 6361  sn't mean you ca
+00005970: 6e6e 6f74 2069 7465 7261 7465 2074 6865  nnot iterate the
+00005980: 205f 4461 7461 206f 626a 6563 745f 2e0a   _Data object_..
+00005990: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000059a0: 2023 2323 2044 6174 6120 6361 6368 696e   ### Data cachin
+000059b0: 670a 2020 2020 2020 2020 0a20 2020 2020  g.        .     
+000059c0: 2020 2054 6865 205f 4461 7461 206f 626a     The _Data obj
+000059d0: 6563 745f 2070 726f 7669 6465 7320 7468  ect_ provides th
+000059e0: 6520 6162 696c 6974 7920 746f 2075 7365  e ability to use
+000059f0: 2074 6865 2063 6163 6865 2e20 5468 6520   the cache. The 
+00005a00: 6361 6368 6520 776f 726b 7320 666f 7220  cache works for 
+00005a10: 6561 6368 205f 4461 7461 206f 626a 6563  each _Data objec
+00005a20: 745f 2c20 7468 6174 2069 732c 2079 6f75  t_, that is, you
+00005a30: 2063 686f 6f73 650a 2020 2020 2020 2020   choose.        
+00005a40: 7768 6963 6820 5f44 6174 6120 6f62 6a65  which _Data obje
+00005a50: 6374 5f20 796f 7520 7761 6e74 2074 6f20  ct_ you want to 
+00005a60: 7361 7665 2e20 5468 6520 5f44 6174 6120  save. The _Data 
+00005a70: 6f62 6a65 6374 5f20 6361 6368 6520 6973  object_ cache is
+00005a80: 2073 6176 6564 2061 6674 6572 2074 6865   saved after the
+00005a90: 2066 6972 7374 2069 7465 7261 7469 6f6e   first iteration
+00005aa0: 2c20 6275 7420 7468 6520 6974 6572 6174  , but the iterat
+00005ab0: 696f 6e0a 2020 2020 2020 2020 736f 7572  ion.        sour
+00005ac0: 6365 206d 6179 2062 6520 6469 6666 6572  ce may be differ
+00005ad0: 656e 742e 0a20 2020 2020 2020 200a 2020  ent..        .  
+00005ae0: 2020 2020 2020 4966 2079 6f75 2064 6f6e        If you don
+00005af0: 2774 2075 7365 2074 6865 2063 6163 6865  't use the cache
+00005b00: 2c20 796f 7572 2073 6f75 7263 6520 7769  , your source wi
+00005b10: 6c6c 2062 6520 7468 6520 6461 7461 2073  ll be the data s
+00005b20: 6f75 7263 6520 796f 7520 6861 7665 2069  ource you have i
+00005b30: 6e20 7468 6520 5f44 6174 6120 4f62 6a65  n the _Data Obje
+00005b40: 6374 5f2e 2042 7574 2069 6620 796f 7520  ct_. But if you 
+00005b50: 7573 6520 7468 6520 6361 6368 652c 0a20  use the cache,. 
+00005b60: 2020 2020 2020 2079 6f75 7220 736f 7572         your sour
+00005b70: 6365 2063 616e 2062 6520 7468 6520 6461  ce can be the da
+00005b80: 7461 2073 6f75 7263 652c 2074 6865 2070  ta source, the p
+00005b90: 6172 656e 7420 6361 6368 652c 206f 7220  arent cache, or 
+00005ba0: 6f77 6e20 6361 6368 653a 0a20 2020 2020  own cache:.     
+00005bb0: 2020 200a 2020 2020 2020 2020 2a20 5468     .        * Th
+00005bc0: 6520 6461 7461 2073 6f75 7263 653a 0a20  e data source:. 
+00005bd0: 2020 2020 2020 2020 2049 6620 7468 6520           If the 
+00005be0: 5f44 6174 6120 4f62 6a65 6374 5f20 646f  _Data Object_ do
+00005bf0: 6573 6e27 7420 6861 7665 2061 2070 6172  esn't have a par
+00005c00: 656e 7420 6361 6368 6520 616e 6420 6974  ent cache and it
+00005c10: 7320 6361 6368 652e 0a20 2020 2020 2020  s cache..       
+00005c20: 202a 2054 6865 2070 6172 656e 7420 6361   * The parent ca
+00005c30: 6368 653a 0a20 2020 2020 2020 2020 2049  che:.          I
+00005c40: 6620 7468 6520 5f44 6174 6120 4f62 6a65  f the _Data Obje
+00005c50: 6374 5f20 6861 7320 6120 7061 7265 6e74  ct_ has a parent
+00005c60: 2063 6163 6865 2e20 4974 2064 6f65 736e   cache. It doesn
+00005c70: 2774 206d 6174 7465 7220 7768 6174 2070  't matter what p
+00005c80: 6f73 6974 696f 6e20 7468 6520 7061 7265  osition the pare
+00005c90: 6e74 2063 6163 6865 2068 6173 2069 6e20  nt cache has in 
+00005ca0: 696e 6865 7269 7461 6e63 652e 0a20 2020  inheritance..   
+00005cb0: 2020 2020 2020 205f 4461 7461 204f 626a         _Data Obj
+00005cc0: 6563 745f 2075 6e64 6572 7374 616e 6473  ect_ understands
+00005cd0: 2077 686f 7365 2063 6163 6865 2069 7420   whose cache it 
+00005ce0: 6973 2061 6e64 2065 7865 6375 7465 7320  is and executes 
+00005cf0: 7468 6520 7061 7274 206f 6620 7468 6520  the part of the 
+00005d00: 776f 726b 666c 6f77 2074 6861 7420 7761  workflow that wa
+00005d10: 7320 6e6f 7420 6578 6563 7574 6564 2e0a  s not executed..
+00005d20: 2020 2020 2020 2020 2a20 5468 6520 6f77          * The ow
+00005d30: 6e20 6361 6368 653a 0a20 2020 2020 2020  n cache:.       
+00005d40: 2020 2049 6620 6974 2069 7320 6e6f 7420     If it is not 
+00005d50: 7468 6520 6669 7273 7420 6974 6572 6174  the first iterat
+00005d60: 696f 6e20 6f66 2074 6869 7320 4461 7461  ion of this Data
+00005d70: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
+00005d80: 200a 2020 2020 2020 2020 4e6f 7465 2074   .        Note t
+00005d90: 6861 7420 7468 6520 6361 6368 6520 7374  hat the cache st
+00005da0: 6174 6520 6f66 2074 6865 2044 6174 6120  ate of the Data 
+00005db0: 6f62 6a65 6374 2069 7320 6e6f 7420 696e  object is not in
+00005dc0: 6865 7269 7465 642e 0a20 2020 2020 2020  herited..       
+00005dd0: 200a 2020 2020 2020 2020 2323 2323 2046   .        #### F
+00005de0: 6f72 6365 6420 6361 6368 696e 670a 2020  orced caching.  
+00005df0: 2020 2020 2020 596f 7520 6361 6e20 7465        You can te
+00005e00: 6c6c 2044 5320 746f 2063 6163 6865 2064  ll DS to cache d
+00005e10: 6174 6120 746f 2073 7065 6369 6669 6320  ata to specific 
+00005e20: 6361 6368 6520 6669 6c65 2c20 7768 6963  cache file, whic
+00005e30: 6820 776f 6e27 7420 6265 2064 656c 6574  h won't be delet
+00005e40: 6564 2061 6674 6572 2073 6372 6970 7420  ed after script 
+00005e50: 656e 642e 0a20 2020 2020 2020 2059 6f75  end..        You
+00005e60: 2063 616e 2073 6565 2065 7861 6d70 6c65   can see example
+00005e70: 2069 6e20 312e 3132 2073 6563 7469 6f6e   in 1.12 section
+00005e80: 206f 6620 5b67 6574 5f73 7461 7274 6564   of [get_started
+00005e90: 5f65 7861 6d70 6c65 5d28 6578 616d 706c  _example](exampl
+00005ea0: 6573 2f67 6574 5f73 7461 7274 6564 5f65  es/get_started_e
+00005eb0: 7861 6d70 6c65 2e70 7929 2e0a 2020 2020  xample.py)..    
+00005ec0: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
+00005ed0: 2020 2020 2020 2323 2320 4576 656e 7454        ### EventT
+00005ee0: 7265 6520 616e 6420 636f 6c6c 6563 7469  ree and collecti
+00005ef0: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
+00005f00: 2020 2020 2023 2323 2320 4576 656e 7454       #### EventT
+00005f10: 7265 650a 2020 2020 2020 2020 0a20 2020  ree.        .   
+00005f20: 2020 2020 2060 4576 656e 7454 7265 6560       `EventTree`
+00005f30: 2069 7320 6120 7472 6565 2d62 6173 6564   is a tree-based
+00005f40: 2064 6174 6120 7374 7275 6374 7572 6520   data structure 
+00005f50: 6f66 2065 7665 6e74 732e 2049 7420 616c  of events. It al
+00005f60: 6c6f 7773 2079 6f75 2067 6574 2063 6869  lows you get chi
+00005f70: 6c64 7265 6e20 616e 6420 7061 7265 6e74  ldren and parent
+00005f80: 7320 6f66 2065 7665 6e74 2c20 0a20 2020  s of event, .   
+00005f90: 2020 2020 2064 6973 706c 6179 2074 7265       display tre
+00005fa0: 652c 2067 6574 2066 756c 6c20 7061 7468  e, get full path
+00005fb0: 2074 6f20 6576 656e 7420 6574 632e 0a20   to event etc.. 
+00005fc0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005fd0: 4465 7461 696c 733a 0a20 2020 2020 2020  Details:.       
+00005fe0: 200a 2020 2020 2020 2020 2a20 6045 7665   .        * `Eve
+00005ff0: 6e74 5472 6565 6020 636f 6e74 6169 6e73  ntTree` contains
+00006000: 2061 6c6c 2065 7665 6e74 7320 696e 206d   all events in m
+00006010: 656d 6f72 792e 0a20 2020 2020 2020 202a  emory..        *
+00006020: 2054 7265 6520 6861 7320 736f 6d65 2069   Tree has some i
+00006030: 6d70 6f72 7461 6e74 2074 6572 6d73 3a0a  mportant terms:.
+00006040: 2020 2020 2020 2020 2020 2020 312e 205f              1. _
+00006050: 416e 6365 7374 6f72 5f20 6973 2061 6e79  Ancestor_ is any
+00006060: 2072 656c 6174 6976 6520 6f66 2074 6865   relative of the
+00006070: 2065 7665 6e74 2075 7020 7468 6520 7472   event up the tr
+00006080: 6565 2028 6772 616e 6470 6172 656e 742c  ee (grandparent,
+00006090: 2070 6172 656e 7420 6574 632e 292e 0a20   parent etc.).. 
+000060a0: 2020 2020 2020 2020 2020 2032 2e20 5f50             2. _P
+000060b0: 6172 656e 745f 2069 7320 6f6e 6c79 2074  arent_ is only t
+000060c0: 6865 2066 6972 7374 2072 656c 6174 6976  he first relativ
+000060d0: 6520 6f66 2074 6865 2065 7665 6e74 2075  e of the event u
+000060e0: 7020 7468 6520 7472 6565 2e0a 2020 2020  p the tree..    
+000060f0: 2020 2020 2020 2020 332e 205f 4368 696c          3. _Chil
+00006100: 645f 2069 7320 7468 6520 6669 7273 7420  d_ is the first 
+00006110: 7265 6c61 7469 7665 206f 6620 7468 6520  relative of the 
+00006120: 6576 656e 7420 646f 776e 2074 6865 2074  event down the t
+00006130: 7265 652e 0a20 2020 2020 2020 200a 2020  ree..        .  
+00006140: 2020 2020 2020 5461 6b65 2061 206c 6f6f        Take a loo
+00006150: 6b20 6174 2074 6865 2066 6f6c 6c6f 7769  k at the followi
+00006160: 6e67 2048 544d 4c20 7472 6565 2074 6f20  ng HTML tree to 
+00006170: 756e 6465 7273 7461 6e64 2074 6865 6d2e  understand them.
+00006180: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00006190: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+000061a0: 2020 2020 203c 626f 6479 3e20 3c21 2d2d       <body> <!--
+000061b0: 2061 6e63 6573 746f 7220 2867 7261 6e64   ancestor (grand
+000061c0: 7061 7265 6e74 292c 2062 7574 206e 6f74  parent), but not
+000061d0: 2070 6172 656e 7420 2d2d 3e0a 2020 2020   parent -->.    
+000061e0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000061f0: 3e20 3c21 2d2d 2070 6172 656e 7420 2620  > <!-- parent & 
+00006200: 616e 6365 7374 6f72 202d 2d3e 0a20 2020  ancestor -->.   
+00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006220: 203c 703e 4865 6c6c 6f2c 2077 6f72 6c64   <p>Hello, world
+00006230: 213c 2f70 3e20 3c21 2d2d 2063 6869 6c64  !</p> <!-- child
+00006240: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
+00006250: 2020 2020 2020 2020 203c 703e 476f 6f64           <p>Good
+00006260: 6279 6521 3c2f 703e 203c 212d 2d20 7369  bye!</p> <!-- si
+00006270: 626c 696e 6720 2d2d 3e0a 2020 2020 2020  bling -->.      
+00006280: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00006290: 0a20 2020 2020 2020 2020 2020 203c 2f62  .            </b
+000062a0: 6f64 793e 0a20 2020 2020 2020 2020 2020  ody>.           
+000062b0: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
+000062c0: 2020 2020 2023 2323 2320 436f 6c6c 6563       #### Collec
+000062d0: 7469 6f6e 730a 2020 2020 2020 2020 0a20  tions.        . 
+000062e0: 2020 2020 2020 202a 2a45 7665 6e74 5472         **EventTr
+000062f0: 6565 436f 6c6c 6563 7469 6f6e 2a2a 2069  eeCollection** i
+00006300: 7320 6120 636f 6c6c 6563 7469 6f6e 206f  s a collection o
+00006310: 6620 4576 656e 7454 7265 6573 2e20 5468  f EventTrees. Th
+00006320: 6520 636f 6c6c 6563 7469 6f6e 2062 7569  e collection bui
+00006330: 6c64 7320 6120 6665 7720 5f45 7665 6e74  lds a few _Event
+00006340: 5472 6565 5f20 6279 2070 6173 7365 6420  Tree_ by passed 
+00006350: 5f44 6174 610a 2020 2020 2020 2020 6f62  _Data.        ob
+00006360: 6a65 6374 5f2e 2041 6c74 686f 7567 6820  ject_. Although 
+00006370: 796f 7520 6361 6e20 6368 616e 6765 2074  you can change t
+00006380: 6865 2074 7265 6520 6469 7265 6374 6c79  he tree directly
+00006390: 2c20 6974 2773 2062 6574 7465 7220 746f  , it's better to
+000063a0: 2064 6f20 6974 2074 6872 6f75 6768 2063   do it through c
+000063b0: 6f6c 6c65 6374 696f 6e73 2062 6563 6175  ollections becau
+000063c0: 7365 2074 6865 7920 6172 6520 6177 6172  se they are awar
+000063d0: 6520 6f66 0a20 2020 2020 2020 2060 6465  e of.        `de
+000063e0: 7461 6368 6564 5f65 7665 6e74 7360 2061  tached_events` a
+000063f0: 6e64 2063 616e 2073 6f6c 7665 2073 6f6d  nd can solve som
+00006400: 6520 6576 656e 7473 2064 6570 656e 6465  e events depende
+00006410: 6e63 6965 732e 2054 6865 2063 6f6c 6c65  ncies. The colle
+00006420: 6374 696f 6e20 6861 7320 7369 6d69 6c61  ction has simila
+00006430: 7220 6665 6174 7572 6573 206c 696b 6520  r features like 
+00006440: 6120 7369 6e67 6c65 205f 4576 656e 7454  a single _EventT
+00006450: 7265 655f 0a20 2020 2020 2020 2062 7574  ree_.        but
+00006460: 2061 7070 6c79 696e 6720 7468 656d 2066   applying them f
+00006470: 6f72 2061 6c6c 205f 4576 656e 7454 7265  or all _EventTre
+00006480: 6573 5f2e 0a20 2020 2020 2020 200a 2020  es_..        .  
+00006490: 2020 2020 2020 2a2a 5061 7265 6e74 4576        **ParentEv
+000064a0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+000064b0: 6e2a 2a20 6973 2061 2063 6f6c 6c65 6374  n** is a collect
+000064c0: 696f 6e20 7369 6d69 6c61 7220 746f 205f  ion similar to _
+000064d0: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
+000064e0: 696f 6e5f 2062 7574 2063 6f6e 7461 696e  ion_ but contain
+000064f0: 696e 6720 6f6e 6c79 2070 6172 656e 7420  ing only parent 
+00006500: 6576 656e 7473 2074 6861 740a 2020 2020  events that.    
+00006510: 2020 2020 6172 6520 7265 6665 7265 6e63      are referenc
+00006520: 6564 2069 6e20 7468 6520 6461 7461 2073  ed in the data s
+00006530: 7472 6561 6d2e 2054 6865 2063 6f6c 6c65  tream. The colle
+00006540: 6374 696f 6e20 6861 7320 6665 6174 7572  ction has featur
+00006550: 6573 2073 696d 696c 6172 2074 6f20 5f45  es similar to _E
+00006560: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
+00006570: 6f6e 5f2e 0a20 2020 2020 2020 200a 2020  on_..        .  
+00006580: 2020 2020 2020 4465 7461 696c 733a 0a20        Details:. 
+00006590: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000065a0: 2a20 546f 2075 7365 2045 5420 636f 6c6c  * To use ET coll
+000065b0: 6563 7469 6f6e 7320 796f 7520 6e65 6564  ections you need
+000065c0: 2074 6f20 696e 6974 6961 6c69 7a65 2074   to initialize t
+000065d0: 6865 6d20 6279 205f 4554 4344 7269 7665  hem by _ETCDrive
+000065e0: 725f 2e20 4461 7461 2073 6f75 7263 6573  r_. Data sources
+000065f0: 2075 7375 616c 6c79 2070 726f 7669 6465   usually provide
+00006600: 2074 6865 6d2e 0a20 2020 2020 2020 2020   them..         
+00006610: 2059 6f75 2063 616e 2063 7265 6174 6520   You can create 
+00006620: 6974 2062 7920 796f 7572 7365 6c66 2064  it by yourself d
+00006630: 6570 656e 6469 6e67 206f 6e20 796f 7572  epending on your
+00006640: 2064 6174 6120 7374 7275 6374 7572 652e   data structure.
+00006650: 2020 0a20 2020 2020 2020 202a 2054 6865    .        * The
+00006660: 2063 6f6c 6c65 6374 696f 6e20 6861 7320   collection has 
+00006670: 6120 6665 6174 7572 6520 746f 2072 6563  a feature to rec
+00006680: 6f76 6572 2065 7665 6e74 732e 2041 6c6c  over events. All
+00006690: 2065 7665 6e74 7320 7468 6174 2061 7265   events that are
+000066a0: 206e 6f74 2069 6e20 7468 6520 7265 6365   not in the rece
+000066b0: 6976 6564 2064 6174 6120 7374 7265 616d  ived data stream
+000066c0: 2c20 6275 7420 7768 6963 6820 6172 650a  , but which are.
+000066d0: 2020 2020 2020 2020 2020 7265 6665 7265            refere
+000066e0: 6e63 6564 2077 696c 6c20 6265 206c 6f61  nced will be loa
+000066f0: 6465 6420 6672 6f6d 2074 6865 2064 6174  ded from the dat
+00006700: 6120 736f 7572 6365 2e0a 2020 2020 2020  a source..      
+00006710: 2020 2a20 596f 7520 6361 6e20 7461 6b65    * You can take
+00006720: 2060 6465 7461 6368 6564 5f65 7665 6e74   `detached_event
+00006730: 7360 2074 6f20 7365 6520 7768 6963 6820  s` to see which 
+00006740: 6576 656e 7473 2061 7265 206d 6973 7369  events are missi
+00006750: 6e67 2e0a 2020 2020 2020 2020 2a20 4966  ng..        * If
+00006760: 2079 6f75 2077 616e 742c 2079 6f75 2063   you want, you c
+00006770: 616e 2062 7569 6c64 2070 6172 656e 746c  an build parentl
+00006780: 6573 7320 7472 6565 7320 7768 6572 6520  ess trees where 
+00006790: 7468 6520 6d69 7373 696e 6720 6576 656e  the missing even
+000067a0: 7473 2061 7265 2073 7475 6262 6564 2069  ts are stubbed i
+000067b0: 6e73 7465 6164 2e20 4a75 7374 0a20 2020  nstead. Just.   
+000067c0: 2020 2020 2020 2075 7365 2060 6765 745f         use `get_
+000067d0: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
+000067e0: 2829 602e 0a20 2020 2020 2020 200a 2020  ()`..        .  
+000067f0: 2020 2020 2020 5265 7175 6972 656d 656e        Requiremen
+00006800: 7473 3a0a 2020 2020 2020 2020 0a20 2020  ts:.        .   
+00006810: 2020 2020 2031 2e20 4576 656e 7473 2070       1. Events p
+00006820: 726f 7669 6465 6420 746f 2045 5443 2068  rovided to ETC h
+00006830: 6176 6520 746f 2068 6176 6520 6065 7665  ave to have `eve
+00006840: 6e74 5f6e 616d 6560 2c20 6065 7665 6e74  nt_name`, `event
+00006850: 5f69 6460 2c20 6070 6172 656e 745f 6576  _id`, `parent_ev
+00006860: 656e 745f 6964 6020 6669 656c 6473 2e20  ent_id` fields. 
+00006870: 5468 6579 200a 2020 2020 2020 2020 6361  They .        ca
+00006880: 6e20 6861 7665 2061 6e6f 7468 6572 206e  n have another n
+00006890: 616d 6573 2028 6974 2072 6573 6f6c 7665  ames (it resolve
+000068a0: 7320 696e 2074 6865 2064 7269 7665 7229  s in the driver)
+000068b0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+000068c0: 2020 2023 2323 2320 4869 6e74 730a 2020     #### Hints.  
+000068d0: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
+000068e0: 2052 656d 6f76 6520 616c 6c20 756e 6e65   Remove all unne
+000068f0: 6365 7373 6172 7920 6669 656c 6473 2066  cessary fields f
+00006900: 726f 6d20 6576 656e 7473 2062 6566 6f72  rom events befor
+00006910: 6520 7061 7373 696e 6720 746f 2061 205f  e passing to a _
+00006920: 636f 6c6c 6563 7469 6f6e 5f20 746f 2072  collection_ to r
+00006930: 6564 7563 6520 6d65 6d6f 7279 2075 7361  educe memory usa
+00006940: 6765 2e0a 2020 2020 2020 2020 2a20 5573  ge..        * Us
+00006950: 6520 6073 686f 7728 2960 206d 6574 686f  e `show()` metho
+00006960: 6420 746f 2070 7269 6e74 2074 6865 2074  d to print the t
+00006970: 7265 6520 696e 2074 7265 652d 6c69 6b65  ree in tree-like
+00006980: 2076 6965 772e 0a20 2020 2020 2020 202a   view..        *
+00006990: 204e 6f74 6520 7468 6174 2074 6865 2060   Note that the `
+000069a0: 6765 745f 7860 206d 6574 686f 6473 2077  get_x` methods w
+000069b0: 696c 6c20 7261 6973 6520 616e 2065 7863  ill raise an exc
+000069c0: 6570 7469 6f6e 2069 6620 796f 7520 7061  eption if you pa
+000069d0: 7373 2061 6e20 756e 6b6e 6f77 6e20 6576  ss an unknown ev
+000069e0: 656e 7420 6964 2c20 756e 6c69 6b65 2074  ent id, unlike t
+000069f0: 6865 2060 6669 6e64 5f78 6020 6d65 7468  he `find_x` meth
+00006a00: 6f64 7320 280a 2020 2020 2020 2020 2020  ods (.          
+00006a10: 7468 6579 2072 6574 7572 6e20 4e6f 6e65  they return None
+00006a20: 292e 0a20 2020 2020 2020 202a 2049 6620  )..        * If 
+00006a30: 796f 7520 7761 6e74 2074 6f20 6b6e 6f77  you want to know
+00006a40: 2074 6861 7420 7370 6563 6966 6965 6420   that specified 
+00006a50: 6576 656e 7420 6578 6973 7473 2c20 7573  event exists, us
+00006a60: 6520 7468 6520 7079 7468 6f6e 2060 696e  e the python `in
+00006a70: 6020 6b65 7977 6f72 6420 2865 2e67 2e20  ` keyword (e.g. 
+00006a80: 6027 6576 656e 742d 6964 2720 696e 2065  `'event-id' in e
+00006a90: 7665 6e74 735f 7472 6565 6029 2e0a 2020  vents_tree`)..  
+00006aa0: 2020 2020 2020 2a20 5573 6520 7468 6520        * Use the 
+00006ab0: 7079 7468 6f6e 2060 6c65 6e60 206b 6579  python `len` key
+00006ac0: 776f 7264 2074 6f20 6765 7420 6576 656e  word to get even
+00006ad0: 7473 206e 756d 6265 7220 696e 2074 6865  ts number in the
+00006ae0: 2074 7265 652e 0a20 2020 2020 2020 200a   tree..        .
+00006af0: 2020 2020 2020 2020 2323 2320 4669 656c          ### Fiel
+00006b00: 6473 5265 736f 6c76 6572 0a20 2020 2020  dsResolver.     
+00006b10: 2020 2054 6865 2069 6465 6120 6f66 2075     The idea of u
+00006b20: 7369 6e67 2072 6573 6f6c 7665 7273 3a20  sing resolvers: 
+00006b30: 200a 2020 2020 2020 2020 4974 2073 6f6c   .        It sol
+00006b40: 7665 7320 7468 6520 7072 6f62 6c65 6d20  ves the problem 
+00006b50: 6f66 2068 6176 696e 6720 6120 6665 7720  of having a few 
+00006b60: 4461 7461 536f 7572 6365 7320 7769 7468  DataSources with
+00006b70: 2074 6865 2073 616d 6520 6461 7461 2c20   the same data, 
+00006b80: 0a20 2020 2020 2020 2062 7574 2077 6974  .        but wit
+00006b90: 6820 6469 6666 6572 656e 7420 7761 7973  h different ways
+00006ba0: 2074 6f20 6765 7420 6974 2e0a 2020 2020   to get it..    
+00006bb0: 2020 2020 0a20 2020 2020 2020 2054 6865      .        The
+00006bc0: 7365 2063 6c61 7373 6573 2070 726f 7669  se classes provi
+00006bd0: 6465 2079 6f75 2067 6574 7465 7220 6d65  de you getter me
+00006be0: 7468 6f64 732e 200a 2020 2020 2020 2020  thods. .        
+00006bf0: 5573 696e 6720 7468 6573 6520 636c 6173  Using these clas
+00006c00: 7365 7320 616c 6c6f 7773 2079 6f75 2074  ses allows you t
+00006c10: 6f20 6672 6565 6c79 2073 7769 7463 6820  o freely switch 
+00006c20: 6265 7477 6565 6e20 6469 6666 6572 656e  between differen
+00006c30: 7420 6461 7461 200a 2020 2020 2020 2020  t data .        
+00006c40: 666f 726d 6174 7320 616e 6420 646f 6e27  formats and don'
+00006c50: 7420 6368 616e 6765 2079 6f75 7220 636f  t change your co
+00006c60: 6465 2e20 0a20 2020 2020 2020 200a 2020  de. .        .  
+00006c70: 2020 2020 2020 5265 736f 6c76 6572 7320        Resolvers 
+00006c80: 736f 6c76 6520 7468 6520 7072 6f62 6c65  solve the proble
+00006c90: 6d20 6f66 2064 6174 612d 666f 726d 6174  m of data-format
+00006ca0: 206d 6967 7261 7469 6f6e 2e20 200a 2020   migration.  .  
+00006cb0: 2020 2020 2020 2d20 6669 656c 6473 2070        - fields p
+00006cc0: 6c61 6365 2063 616e 2062 6520 6368 616e  lace can be chan
+00006cd0: 6765 640a 2020 2020 2020 2020 2d20 6669  ged.        - fi
+00006ce0: 656c 6473 206e 616d 6573 2063 616e 2062  elds names can b
+00006cf0: 6520 6368 616e 6765 640a 2020 2020 2020  e changed.      
+00006d00: 2020 0a20 2020 2020 2020 2052 6573 6f6c    .        Resol
+00006d10: 7665 7273 2063 616e 2077 6f72 6b20 6f6e  vers can work on
+00006d20: 6c79 2077 6974 6820 6f6e 6520 6576 656e  ly with one even
+00006d30: 742f 6d65 7373 6167 652e 200a 2020 2020  t/message. .    
+00006d40: 2020 2020 4974 206d 6561 6e73 2c20 6966      It means, if
+00006d50: 2079 6f75 7220 6d65 7373 6167 6520 6861   your message ha
+00006d60: 7320 7375 622d 6d65 7373 6167 6573 2069  s sub-messages i
+00006d70: 7420 776f 6e27 7420 776f 726b 2c20 6265  t won't work, be
+00006d80: 6361 7573 6520 7265 736f 6c76 6572 2077  cause resolver w
+00006d90: 696c 6c20 6e6f 7420 0a20 2020 2020 2020  ill not .       
+00006da0: 206b 6e6f 7720 7769 7468 2077 6869 6368   know with which
+00006db0: 2073 7562 2d6d 6573 7361 6765 2073 686f   sub-message sho
+00006dc0: 756c 6420 6974 2077 6f72 6b2e 200a 2020  uld it work. .  
+00006dd0: 2020 2020 2020 0a20 2020 2020 2020 2049        .        I
+00006de0: 6d70 6c65 6d65 6e74 6174 696f 6e20 6164  mplementation ad
+00006df0: 7669 6365 3a0a 2020 2020 2020 2020 312e  vice:.        1.
+00006e00: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+00006e10: 656e 7465 6445 7272 6f72 202d 2d20 6966  entedError -- if
+00006e20: 2079 6f75 7220 496d 706c 656d 656e 7461   your Implementa
+00006e30: 7469 6f6e 2064 6f65 736e 2774 2073 7570  tion doesn't sup
+00006e40: 706f 7274 2074 6869 7320 6765 7474 6572  port this getter
+00006e50: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00006e60: 2020 2050 6572 666f 726d 616e 6365 2069     Performance i
+00006e70: 6d70 6163 743a 0a20 2020 2020 2020 202d  mpact:.        -
+00006e80: 2049 7420 6120 6269 7420 736c 6f77 6572   It a bit slower
+00006e90: 2074 6861 6e20 7573 696e 6720 6e61 6b65   than using nake
+00006ea0: 6420 6669 656c 6420 6163 6365 7373 2060  d field access `
+00006eb0: 6469 6374 5b27 6b65 7927 5d60 2e20 0a20  dict['key']`. . 
+00006ec0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00006ed0: 2323 2032 2e34 2e20 4c69 6e6b 730a 2020  ## 2.4. Links.  
+00006ee0: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+00006ef0: 205b 5265 706f 7274 2044 6174 6120 5072   [Report Data Pr
+00006f00: 6f76 6964 6572 5d28 6874 7470 733a 2f2f  ovider](https://
+00006f10: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
+00006f20: 6574 2f74 6832 2d72 7074 2d64 6174 612d  et/th2-rpt-data-
+00006f30: 7072 6f76 6964 6572 290a 2020 2020 2020  provider).      
+00006f40: 2020 2d20 5b54 6832 2044 6174 6120 5365    - [Th2 Data Se
+00006f50: 7276 6963 6573 2055 7469 6c73 5d28 6874  rvices Utils](ht
+00006f60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00006f70: 2f74 6832 2d6e 6574 2f74 6832 2d64 6174  /th2-net/th2-dat
+00006f80: 612d 7365 7276 6963 6573 2d75 7469 6c73  a-services-utils
+00006f90: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00006fa0: 2020 2023 2033 2e20 4265 7374 2070 7261     # 3. Best pra
+00006fb0: 6374 6963 6573 0a20 2020 2020 2020 2044  ctices.        D
+00006fc0: 6570 656e 6469 6e67 206f 6e20 686f 7720  epending on how 
+00006fd0: 796f 7520 776f 726b 2077 6974 6820 6044  you work with `D
+00006fe0: 6174 6120 6f62 6a65 6374 602c 2069 7420  ata object`, it 
+00006ff0: 6361 6e20 6265 2073 6c6f 7720 6f66 2066  can be slow of f
+00007000: 6173 742e 2020 0a20 2020 2020 2020 2041  ast.  .        A
+00007010: 7320 7769 7468 2061 2072 656c 6174 696f  s with a relatio
+00007020: 6e61 6c20 6461 7461 6261 7365 2c20 796f  nal database, yo
+00007030: 7520 6361 6e20 7772 6974 6520 6120 7175  u can write a qu
+00007040: 6572 7920 7468 6174 2077 696c 6c20 7265  ery that will re
+00007050: 7475 726e 2064 6174 6120 736c 6f77 6c79  turn data slowly
+00007060: 206f 7220 7175 6963 6b6c 792c 200a 2020   or quickly, .  
+00007070: 2020 2020 2020 7468 6520 7361 6d65 2077        the same w
+00007080: 6865 6e20 776f 726b 696e 6720 7769 7468  hen working with
+00007090: 2061 2060 4461 7461 206f 626a 6563 7460   a `Data object`
+000070a0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+000070b0: 2020 2046 6f6c 6c6f 7720 7468 6520 7275     Follow the ru
+000070c0: 6c65 7320 746f 206d 616b 6520 796f 7572  les to make your
+000070d0: 2077 6f72 6b20 7769 7468 2044 6174 6120   work with Data 
+000070e0: 6f62 6a65 6374 2066 6173 743a 0a20 2020  object fast:.   
+000070f0: 2020 2020 2031 2e20 5573 6520 6044 6174       1. Use `Dat
+00007100: 612e 7573 655f 6361 6368 6528 2960 2069  a.use_cache()` i
+00007110: 6620 796f 7520 6974 6572 6174 6520 6461  f you iterate da
+00007120: 7461 206d 6f72 6520 7468 616e 206f 6e65  ta more than one
+00007130: 2074 696d 652e 0a20 2020 2020 2020 2032   time..        2
+00007140: 2e20 5472 7920 746f 2064 6f6e 2774 2069  . Try to don't i
+00007150: 7465 7261 7465 206f 6e65 2060 4461 7461  terate one `Data
+00007160: 206f 626a 6563 7460 2069 6e73 6964 6520   object` inside 
+00007170: 7468 6520 6f74 6865 7220 6f6e 652e 2020  the other one.  
+00007180: 0a20 2020 2020 2020 2020 2020 4966 2079  .           If y
+00007190: 6f75 2073 686f 756c 6420 746f 2064 6f20  ou should to do 
+000071a0: 6974 2c20 7573 6520 7368 6f72 7420 6044  it, use short `D
+000071b0: 6174 6120 6f62 6a65 6374 6020 6669 7273  ata object` firs
+000071c0: 7420 616e 6420 6c6f 6e67 2060 4461 7461  t and long `Data
+000071d0: 206f 626a 6563 7460 2069 6e73 6964 6520   object` inside 
+000071e0: 7468 6520 6c6f 6f70 2e20 200a 2020 2020  the loop.  .    
+000071f0: 2020 2020 2020 2049 7427 6c6c 2061 6c6c         It'll all
+00007200: 6f77 2079 6f75 206f 7065 6e20 7468 6520  ow you open the 
+00007210: 6361 6368 6520 6669 6c65 206f 7220 6372  cache file or cr
+00007220: 6561 7465 2061 2072 6571 7565 7374 2074  eate a request t
+00007230: 6f20 6044 6174 6120 736f 7572 6365 6020  o `Data source` 
+00007240: 6c65 7373 206e 756d 6265 7220 6f66 2074  less number of t
+00007250: 696d 6573 2e0a 2020 2020 2020 2020 0a20  imes..        . 
+00007260: 2020 2020 2020 2023 2034 2e20 4f66 6669         # 4. Offi
+00007270: 6369 616c 2044 6174 6153 6f75 7263 6520  cial DataSource 
+00007280: 696d 706c 656d 656e 7461 7469 6f6e 730a  implementations.
+00007290: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000072a0: 202d 205b 4c69 6768 7477 6569 6768 7420   - [Lightweight 
+000072b0: 4461 7461 2050 726f 7669 6465 7220 4461  Data Provider Da
+000072c0: 7461 2053 6f75 7263 655d 2868 7474 7073  ta Source](https
+000072d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
+000072e0: 322d 6e65 742f 7468 322d 6473 2d73 6f75  2-net/th2-ds-sou
+000072f0: 7263 652d 6c77 6470 290a 2020 2020 2020  rce-lwdp).      
+00007300: 2020 0a20 2020 2020 2020 200a 2020 2020    .        .    
+00007310: 2020 2020 2320 352e 2041 5049 0a20 2020      # 5. API.   
+00007320: 2020 2020 200a 2020 2020 2020 2020 4966       .        If
+00007330: 2079 6f75 2061 7265 206c 6f6f 6b69 6e67   you are looking
+00007340: 2066 6f72 2063 6c61 7373 6573 2064 6573   for classes des
+00007350: 6372 6970 7469 6f6e 2073 6565 2074 6865  cription see the
+00007360: 205b 4150 4920 446f 6375 6d65 6e74 6174   [API Documentat
+00007370: 696f 6e5d 2864 6f63 756d 656e 7461 7469  ion](documentati
+00007380: 6f6e 2f61 7069 2f69 6e64 6578 2e6d 6429  on/api/index.md)
+00007390: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+000073a0: 2020 2023 2036 2e20 4578 616d 706c 6573     # 6. Examples
+000073b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000073c0: 2020 2d20 5b67 6574 5f73 7461 7274 6564    - [get_started
+000073d0: 5f65 7861 6d70 6c65 2e70 795d 2865 7861  _example.py](exa
+000073e0: 6d70 6c65 732f 6765 745f 7374 6172 7465  mples/get_starte
+000073f0: 645f 6578 616d 706c 652e 7079 290a 2020  d_example.py).  
+00007400: 2020 2020 2020 0a50 6c61 7466 6f72 6d3a        .Platform:
+00007410: 2055 4e4b 4e4f 574e 0a52 6571 7569 7265   UNKNOWN.Require
+00007420: 732d 5079 7468 6f6e 3a20 3e3d 332e 370a  s-Python: >=3.7.
+00007430: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+00007440: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+00007450: 6172 6b64 6f77 6e0a 5072 6f76 6964 6573  arkdown.Provides
+00007460: 2d45 7874 7261 3a20 7264 700a 5072 6f76  -Extra: rdp.Prov
+00007470: 6964 6573 2d45 7874 7261 3a20 7264 7035  ides-Extra: rdp5
+00007480: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00007490: 2072 6470 360a 5072 6f76 6964 6573 2d45   rdp6.Provides-E
+000074a0: 7874 7261 3a20 6c77 6470 0a50 726f 7669  xtra: lwdp.Provi
+000074b0: 6465 732d 4578 7472 613a 206c 7764 7031  des-Extra: lwdp1
+000074c0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+000074d0: 206c 7764 7032 0a50 726f 7669 6465 732d   lwdp2.Provides-
+000074e0: 4578 7472 613a 206c 7764 702d 6465 760a  Extra: lwdp-dev.
+000074f0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00007500: 7574 696c 732d 7270 742d 7669 6577 6572  utils-rpt-viewer
+00007510: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00007520: 2075 7469 6c73 2d72 7074 2d76 6965 7765   utils-rpt-viewe
+00007530: 7235 0a50 726f 7669 6465 732d 4578 7472  r5.Provides-Extr
+00007540: 613a 2075 7469 6c73 2d61 6476 616e 6365  a: utils-advance
+00007550: 640a                                     d.
```

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev5738245039/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5738217622/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev5738245039/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

