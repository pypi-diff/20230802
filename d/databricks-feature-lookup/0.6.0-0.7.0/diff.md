# Comparing `tmp/databricks-feature-lookup-0.6.0.tar.gz` & `tmp/databricks-feature-lookup-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-feature-lookup-0.6.0.tar", last modified: Mon Jul 10 20:06:26 2023, max compression
+gzip compressed data, was "databricks-feature-lookup-0.7.0.tar", last modified: Tue Aug  1 01:10:08 2023, max compression
```

## Comparing `databricks-feature-lookup-0.6.0.tar` & `databricks-feature-lookup-0.7.0.tar`

### file list

```diff
@@ -1,81 +1,80 @@
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.683327 databricks-feature-lookup-0.6.0/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2414 2022-07-20 05:31:47.000000 databricks-feature-lookup-0.6.0/LICENSE.md
--rw-r--r--   0 mingyang.ge   (502) staff       (20)       30 2023-06-22 23:44:03.000000 databricks-feature-lookup-0.6.0/MANIFEST.in
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      426 2022-07-20 05:31:47.000000 databricks-feature-lookup-0.6.0/NOTICE.md
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4219 2023-07-10 20:06:26.683174 databricks-feature-lookup-0.6.0/PKG-INFO
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3488 2023-07-10 20:06:26.000000 databricks-feature-lookup-0.6.0/README.md
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.662340 databricks-feature-lookup-0.6.0/databricks/
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.665285 databricks-feature-lookup-0.6.0/databricks/_feature_store_pkg_metadata/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      166 2022-10-06 23:48:00.000000 databricks-feature-lookup-0.6.0/databricks/_feature_store_pkg_metadata/__init__.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.665660 databricks-feature-lookup-0.6.0/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-10-06 23:48:00.000000 databricks-feature-lookup-0.6.0/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/__init__.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.667250 databricks-feature-lookup-0.6.0/databricks/feature_store/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1980 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/__init__.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.673682 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1309 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/_feature_store_object.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1489 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/_proto_enum_entity.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      444 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/cloud.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3524 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/column_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      913 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/data_type.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2553 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_column_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3971 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_functions_for_serving.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    19863 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_spec.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      739 2023-06-08 17:27:16.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_spec_constants.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1544 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_table_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4065 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_tables_for_serving.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      673 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/function_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1978 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/on_demand_column_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     6817 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/online_feature_table.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     5966 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/online_store_for_serving.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      489 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/query_mode.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      855 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/source_data_column_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      659 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/store_type.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.674193 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     7556 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/feature_function_executor.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2817 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/feature_function_loader.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.674659 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/utils/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/utils/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1855 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/utils/codegen_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      139 2023-07-10 20:03:31.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_lookup_version.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.676420 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      891 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1068 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_brickstore_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     8034 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    21707 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      923 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2832 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_mysql_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     7916 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_sql_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2130 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    31382 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/mlflow_model.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1766 2023-06-22 23:43:16.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/mlflow_model_constants.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    11426 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/online_lookup_client.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.677124 databricks-feature-lookup-0.6.0/databricks/feature_store/protos/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-07-20 05:31:47.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/protos/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     6433 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/protos/feature_spec_pb2.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    21337 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/protos/feature_store_serving_pb2.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.681719 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3871 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/converter_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1736 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/cosmosdb_type_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      803 2023-05-31 17:19:14.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/cosmosdb_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      765 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/data_type_details_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1739 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/dynamodb_type_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     5030 2023-06-05 18:12:24.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/dynamodb_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3117 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/feature_function_type_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2317 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/feature_spec_test_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2631 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/metrics_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    11740 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/pandas_type_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     8049 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/serving_test_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1278 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/sql_type_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      374 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/test_utils_common.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    10313 2023-07-08 07:28:45.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/uc_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1539 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/utils_common.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.682916 databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4219 2023-07-10 20:06:26.000000 databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/PKG-INFO
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3435 2023-07-10 20:06:26.000000 databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/SOURCES.txt
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        1 2023-07-10 20:06:26.000000 databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/dependency_links.txt
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      107 2023-07-10 20:06:26.000000 databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/requires.txt
--rw-r--r--   0 mingyang.ge   (502) staff       (20)       11 2023-07-10 20:06:26.000000 databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/top_level.txt
--rw-r--r--   0 mingyang.ge   (502) staff       (20)       38 2023-07-10 20:06:26.683387 databricks-feature-lookup-0.6.0/setup.cfg
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2724 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/setup.py
+drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-08-01 01:10:08.077803 databricks-feature-lookup-0.7.0/
+-rw-r--r--   0 victor.sun   (502) staff       (20)     2414 2022-04-15 06:23:53.000000 databricks-feature-lookup-0.7.0/LICENSE.md
+-rw-r--r--   0 victor.sun   (502) staff       (20)       30 2023-06-27 21:53:39.000000 databricks-feature-lookup-0.7.0/MANIFEST.in
+-rw-r--r--   0 victor.sun   (502) staff       (20)      426 2022-04-15 06:23:53.000000 databricks-feature-lookup-0.7.0/NOTICE.md
+-rw-r--r--   0 victor.sun   (502) staff       (20)     4219 2023-08-01 01:10:08.077491 databricks-feature-lookup-0.7.0/PKG-INFO
+-rw-r--r--   0 victor.sun   (502) staff       (20)     3488 2023-08-01 01:10:07.000000 databricks-feature-lookup-0.7.0/README.md
+drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-08-01 01:10:08.034208 databricks-feature-lookup-0.7.0/databricks/
+drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-08-01 01:10:08.038745 databricks-feature-lookup-0.7.0/databricks/_feature_store_pkg_metadata/
+-rw-r--r--   0 victor.sun   (502) staff       (20)      166 2022-09-26 23:04:45.000000 databricks-feature-lookup-0.7.0/databricks/_feature_store_pkg_metadata/__init__.py
+drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-08-01 01:10:08.039440 databricks-feature-lookup-0.7.0/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/
+-rw-r--r--   0 victor.sun   (502) staff       (20)        0 2022-09-26 23:04:45.000000 databricks-feature-lookup-0.7.0/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/__init__.py
+drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-08-01 01:10:08.043035 databricks-feature-lookup-0.7.0/databricks/feature_store/
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1980 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/__init__.py
+drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-08-01 01:10:08.055789 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/
+-rw-r--r--   0 victor.sun   (502) staff       (20)        0 2022-09-28 20:02:48.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/__init__.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1309 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/_feature_store_object.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1489 2022-09-28 20:02:48.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/_proto_enum_entity.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)      444 2023-06-22 07:22:52.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/cloud.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     3524 2023-06-22 07:22:52.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/column_info.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)      913 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/data_type.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     2553 2023-06-22 07:22:52.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/feature_column_info.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     3971 2023-04-19 00:08:11.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/feature_functions_for_serving.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)    19863 2023-06-22 07:22:52.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/feature_spec.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)      739 2023-06-15 00:21:11.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/feature_spec_constants.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1544 2023-06-22 07:22:52.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/feature_table_info.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1697 2023-07-28 22:41:26.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/feature_tables_for_serving.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)      673 2023-06-22 07:22:52.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/function_info.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1978 2023-06-22 07:22:52.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/on_demand_column_info.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     3806 2023-07-28 22:41:26.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/online_feature_table.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     4175 2023-07-28 22:41:26.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/online_store_for_serving.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)      489 2023-06-22 07:22:52.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/query_mode.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)      855 2023-06-22 07:22:52.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/source_data_column_info.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)      659 2023-06-22 07:22:52.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/entities/store_type.py
+drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-08-01 01:10:08.056686 databricks-feature-lookup-0.7.0/databricks/feature_store/feature_functions/
+-rw-r--r--   0 victor.sun   (502) staff       (20)     7556 2023-05-11 01:52:53.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/feature_functions/feature_function_executor.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     2817 2023-05-11 01:52:53.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/feature_functions/feature_function_loader.py
+drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-08-01 01:10:08.057365 databricks-feature-lookup-0.7.0/databricks/feature_store/feature_functions/utils/
+-rw-r--r--   0 victor.sun   (502) staff       (20)        0 2023-05-11 01:52:53.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/feature_functions/utils/__init__.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1855 2023-05-11 01:52:53.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/feature_functions/utils/codegen_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)      139 2023-08-01 01:07:15.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/feature_lookup_version.py
+drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-08-01 01:10:08.062670 databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/
+-rw-r--r--   0 victor.sun   (502) staff       (20)      891 2023-06-15 00:21:11.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/__init__.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1068 2023-07-28 17:26:29.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_brickstore_engine.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     8106 2023-07-28 09:02:01.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)    21369 2023-07-28 22:41:26.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)      923 2023-03-30 17:46:27.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_engine.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     2832 2023-06-06 23:19:09.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_mysql_engine.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     7916 2023-07-03 05:50:56.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_sql_engine.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     2130 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)    29844 2023-07-28 22:41:26.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/mlflow_model.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1715 2023-07-28 22:41:26.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/mlflow_model_constants.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     9533 2023-07-28 22:41:26.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/online_lookup_client.py
+drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-08-01 01:10:08.064006 databricks-feature-lookup-0.7.0/databricks/feature_store/protos/
+-rw-r--r--   0 victor.sun   (502) staff       (20)        0 2022-04-15 06:23:53.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/protos/__init__.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     6433 2023-06-23 02:51:42.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/protos/feature_spec_pb2.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)    18475 2023-07-28 22:41:26.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/protos/feature_store_serving_pb2.py
+drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-08-01 01:10:08.073404 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/
+-rw-r--r--   0 victor.sun   (502) staff       (20)        0 2022-09-28 20:02:48.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/__init__.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     3871 2023-06-22 07:22:52.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/converter_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1736 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/cosmosdb_type_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)      861 2023-07-28 09:02:01.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/cosmosdb_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)      765 2022-12-14 01:59:08.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/data_type_details_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1739 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/dynamodb_type_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     5193 2023-07-28 09:02:01.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/dynamodb_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     3117 2023-05-23 01:05:42.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/feature_function_type_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     2317 2023-06-22 07:22:52.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/feature_spec_test_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     2631 2023-05-23 01:05:42.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/metrics_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)    11740 2023-05-11 01:52:53.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/pandas_type_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1278 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/sql_type_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)      374 2023-05-11 01:52:53.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/test_utils_common.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)    10313 2023-07-05 21:45:51.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/uc_utils.py
+-rw-r--r--   0 victor.sun   (502) staff       (20)     1539 2023-04-04 22:12:23.000000 databricks-feature-lookup-0.7.0/databricks/feature_store/utils/utils_common.py
+drwxr-xr-x   0 victor.sun   (502) staff       (20)        0 2023-08-01 01:10:08.077040 databricks-feature-lookup-0.7.0/databricks_feature_lookup.egg-info/
+-rw-r--r--   0 victor.sun   (502) staff       (20)     4219 2023-08-01 01:10:07.000000 databricks-feature-lookup-0.7.0/databricks_feature_lookup.egg-info/PKG-INFO
+-rw-r--r--   0 victor.sun   (502) staff       (20)     3382 2023-08-01 01:10:07.000000 databricks-feature-lookup-0.7.0/databricks_feature_lookup.egg-info/SOURCES.txt
+-rw-r--r--   0 victor.sun   (502) staff       (20)        1 2023-08-01 01:10:07.000000 databricks-feature-lookup-0.7.0/databricks_feature_lookup.egg-info/dependency_links.txt
+-rw-r--r--   0 victor.sun   (502) staff       (20)      107 2023-08-01 01:10:07.000000 databricks-feature-lookup-0.7.0/databricks_feature_lookup.egg-info/requires.txt
+-rw-r--r--   0 victor.sun   (502) staff       (20)       11 2023-08-01 01:10:07.000000 databricks-feature-lookup-0.7.0/databricks_feature_lookup.egg-info/top_level.txt
+-rw-r--r--   0 victor.sun   (502) staff       (20)       38 2023-08-01 01:10:08.077883 databricks-feature-lookup-0.7.0/setup.cfg
+-rw-r--r--   0 victor.sun   (502) staff       (20)     2724 2023-03-03 03:12:48.000000 databricks-feature-lookup-0.7.0/setup.py
```

### Comparing `databricks-feature-lookup-0.6.0/LICENSE.md` & `databricks-feature-lookup-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/PKG-INFO` & `databricks-feature-lookup-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-feature-lookup
-Version: 0.6.0
+Version: 0.7.0
 Summary: Databricks Feature Store Feature Lookup Client
 Author: Databricks
 Author-email: feedback@databricks.com
 License: Databricks Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `databricks-feature-lookup-0.6.0/README.md` & `databricks-feature-lookup-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/__init__.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/_feature_store_object.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/_feature_store_object.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/_proto_enum_entity.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/_proto_enum_entity.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/column_info.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/data_type.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/data_type.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_column_info.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/feature_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_functions_for_serving.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/feature_functions_for_serving.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_spec.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/feature_spec.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_spec_constants.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/feature_spec_constants.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_table_info.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/feature_table_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/function_info.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/function_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/on_demand_column_info.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/on_demand_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/online_store_for_serving.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/online_store_for_serving.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 from typing import Union
 
 from databricks.feature_store.entities._feature_store_object import _FeatureStoreObject
 from databricks.feature_store.entities.cloud import Cloud
 from databricks.feature_store.entities.query_mode import QueryMode
 from databricks.feature_store.entities.store_type import StoreType
-from databricks.feature_store.protos.feature_store_serving_pb2 import (
-    DynamoDbConf as ProtoDynamoDbConf,
-)
-from databricks.feature_store.protos.feature_store_serving_pb2 import (
-    OnlineStoreForSageMakerServing as ProtoOnlineStoreForSageMakerServing,
-)
 
 
 class BrickstoreConf(_FeatureStoreObject):
     def __init__(self, host: str, port: int):
         self._host = host
         self._port = port
 
@@ -68,21 +62,27 @@
         self._account_uri = account_uri
 
     @property
     def account_uri(self):
         return self._account_uri
 
 
-class AbstractOnlineStoreForServing(_FeatureStoreObject):
+class OnlineStoreForServing:
     def __init__(
         self,
+        cloud: Cloud,
+        store_type: StoreType,
+        read_secret_prefix: str,
         creation_timestamp_ms: int,
         extra_configs: Union[BrickstoreConf, MySqlConf, SqlServerConf, DynamoDbConf],
         query_mode: QueryMode,
     ):
+        self._cloud = cloud
+        self._store_type = store_type
+        self._read_secret_prefix = read_secret_prefix
         self._creation_timestamp_ms = creation_timestamp_ms
         self._extra_configs = extra_configs
         self._query_mode = query_mode
 
     @property
     def extra_configs(self):
         return self._extra_configs
@@ -91,28 +91,14 @@
     def creation_timestamp_ms(self):
         return self._creation_timestamp_ms
 
     @property
     def query_mode(self) -> QueryMode:
         return self._query_mode
 
-
-class OnlineStoreForServing(AbstractOnlineStoreForServing):
-    def __init__(
-        self,
-        cloud: Cloud,
-        store_type: StoreType,
-        read_secret_prefix: str,
-        **kwargs,
-    ):
-        self._cloud = cloud
-        self._store_type = store_type
-        self._read_secret_prefix = read_secret_prefix
-        super().__init__(**kwargs)
-
     @property
     def cloud(self):
         return self._cloud
 
     @property
     def store_type(self):
         return self._store_type
@@ -149,38 +135,7 @@
             cloud=the_proto.cloud,
             store_type=the_proto.store_type,
             extra_configs=conf,
             read_secret_prefix=the_proto.read_secret_prefix,
             creation_timestamp_ms=the_proto.creation_timestamp_ms,
             query_mode=the_proto.query_mode,
         )
-
-
-class OnlineStoreForSageMakerServing(AbstractOnlineStoreForServing):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    def to_proto(self) -> ProtoOnlineStoreForSageMakerServing:
-        return ProtoOnlineStoreForSageMakerServing(
-            creation_timestamp_ms=self.creation_timestamp_ms,
-            dynamodb_conf=ProtoDynamoDbConf(region=self.extra_configs.region),
-            query_mode=self.query_mode,
-        )
-
-    @classmethod
-    def from_proto(cls, the_proto: ProtoOnlineStoreForSageMakerServing):
-        if not (the_proto.WhichOneof("extra_configs") == "dynamodb_conf"):
-            raise Exception(
-                "Internal Error: Store type is not supported for SageMaker: "
-                f"{the_proto}"
-            )
-        conf = DynamoDbConf(the_proto.dynamodb_conf.region)
-
-        # The `query_mode` should always be defined. We explicitly check this to avoid erroneously retrieving the
-        # default QueryMode enum value `PRIMARY_KEY_LOOKUP` when the `query_mode` proto field is not set.
-        if not the_proto.HasField("query_mode"):
-            raise ValueError(f"'query_mode' should be defined: {the_proto}")
-        return cls(
-            creation_timestamp_ms=the_proto.creation_timestamp_ms,
-            extra_configs=conf,
-            query_mode=the_proto.query_mode,
-        )
```

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/source_data_column_info.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/source_data_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/store_type.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/entities/store_type.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/feature_function_executor.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/feature_functions/feature_function_executor.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/feature_function_loader.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/feature_functions/feature_function_loader.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/utils/codegen_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/feature_functions/utils/codegen_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/__init__.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_brickstore_engine.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_brickstore_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from databricks.feature_store.entities.online_feature_table import OnlineFeatureTable
 from databricks.feature_store.entities.query_mode import QueryMode
 from databricks.feature_store.lookup_engine.lookup_engine import LookupEngine
 from databricks.feature_store.utils.cosmosdb_type_utils import (
     COSMOSDB_DATA_TYPE_CONVERTER_FACTORY,
 )
 from databricks.feature_store.utils.cosmosdb_utils import (
+    DEFAULT_RETRY_CONFIG,
     FEATURE_STORE_SENTINEL_ID_VALUE,
     PARTITION_KEY,
     PATHS,
     PRIMARY_KEY_PROPERTY_NAME_VALUE,
     is_not_found_error,
     to_cosmosdb_primary_key,
 )
@@ -57,15 +58,17 @@
         }
         self.features_to_type_converter = {
             feature.name: COSMOSDB_DATA_TYPE_CONVERTER_FACTORY.get_converter(feature)
             for feature in online_feature_table.features
         }
 
         # Initialize the CosmosClient used for lookup.
-        self._client = CosmosClient(self.account_uri, authorization_key)
+        self._client = CosmosClient(
+            self.account_uri, authorization_key, **DEFAULT_RETRY_CONFIG
+        )
         self._database_client = self._client.get_database_client(self.database_name)
         self._container_client = self._database_client.get_container_client(
             self.container_name
         )
         self._validate_online_feature_table()
 
     def _validate_online_feature_table(
```

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from boto3.dynamodb.conditions import Key
 from botocore.exceptions import ClientError
 
-from databricks.feature_store.entities.online_feature_table import (
-    AbstractOnlineFeatureTable,
-)
+from databricks.feature_store.entities.online_feature_table import OnlineFeatureTable
 from databricks.feature_store.entities.query_mode import QueryMode
 from databricks.feature_store.lookup_engine.lookup_engine import LookupEngine
 from databricks.feature_store.utils.dynamodb_type_utils import (
     DYNAMODB_DATA_TYPE_CONVERTER_FACTORY,
 )
 from databricks.feature_store.utils.dynamodb_utils import (
     ATTRIBUTES_TO_GET,
@@ -55,43 +53,31 @@
     else:
         return [obj]
 
 
 LookupKeyType = Tuple[str, ...]
 
 
-def as_list(obj, default=None):
-    if not obj:
-        return default
-    elif isinstance(obj, list):
-        return obj
-    else:
-        return [obj]
-
-
 class AwsAccessKey:
     def __init__(self, access_key_id: str, secret_access_key: str):
         self.access_key_id = access_key_id
         self.secret_access_key = secret_access_key
 
 
 class LookupDynamoDbEngine(LookupEngine):
     def __init__(
         self,
-        online_feature_table: Union[
-            AbstractOnlineFeatureTable, List[AbstractOnlineFeatureTable]
-        ],
+        online_feature_table: Union[OnlineFeatureTable, List[OnlineFeatureTable]],
         access_key: Optional[AwsAccessKey],
     ):
         """
-        :param online_feature_table: AbstractOnlineFeatureTable to look up feature values from. If
+        :param online_feature_table: OnlineFeatureTable to look up feature values from. If
             a list of online feature tables is passed, they should have the same access credentials.
         :param access_key: Uses this access key to authenticate with AWS, if provided. If None,
-        role-based authentication is used. For example, SageMaker lookup passes access_key=None, and
-        the SageMaker execution role is used to authenticate.
+        role-based authentication is used.
         """
         online_feature_table_as_list = as_list(online_feature_table)
         self._online_feature_table_names_list = [
             oft.online_feature_table_name for oft in online_feature_table_as_list
         ]
         self._query_mode_map = {
             oft.online_feature_table_name: oft.online_store.query_mode
@@ -252,15 +238,15 @@
 
         :param batch_keys: The set of tables to retrieve from. A batch can contain at most 100
                            keys. Otherwise, Amazon DynamoDB returns an error.
         :return: The dictionary of retrieved items grouped under their respective
                  table names.
         """
         num_retry = 0
-        max_tries = 5
+        max_tries = 3
         backoff_in_seconds = (
             1  # Start with 1 second of sleep, then exponentially increase.
         )
         aggregated_response = {key: [] for key in batch_keys}
         unprocessed_keys = []
         while num_retry < max_tries:
             batch_get_item = lookup_call_maybe_with_metrics(
```

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_engine.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_mysql_engine.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_mysql_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_sql_engine.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_sql_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/mlflow_model.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/mlflow_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 import itertools
 import os
 from collections import Counter, defaultdict
 from typing import Dict, List, Optional, Tuple, Union
 
 import mlflow
 import pandas as pd
-from mlflow.models.container import SERVING_ENVIRONMENT
-from mlflow.sagemaker import SAGEMAKER_SERVING_ENVIRONMENT
 from mlflow.utils import databricks_utils
 
 from databricks.feature_store import mlflow_model_constants
 from databricks.feature_store.entities.feature_column_info import FeatureColumnInfo
 from databricks.feature_store.entities.feature_functions_for_serving import (
     FeatureFunctionsForServing,
 )
 from databricks.feature_store.entities.feature_spec import FeatureSpec
 from databricks.feature_store.entities.feature_tables_for_serving import (
-    AbstractFeatureTablesForServing,
-    FeatureTablesForSageMakerServing,
     FeatureTablesForServing,
 )
 from databricks.feature_store.entities.online_feature_table import (
-    AbstractOnlineFeatureTable,
     OnlineFeatureTable,
     PrimaryKeyDetails,
 )
 from databricks.feature_store.feature_functions.feature_function_executor import (
     FeatureFunctionExecutor,
 )
 from databricks.feature_store.feature_lookup_version import VERSION
@@ -69,33 +64,30 @@
     lookup keys (eg pickup_zip and dropoff_zip may each be used to lookup a geographic data feature
     table).
     """
 
     def __init__(
         self,
         feature_col_infos_by_lookup_key: LookupKeyToFeatureColumnInfosType,
-        online_ft: AbstractOnlineFeatureTable,
+        online_ft: OnlineFeatureTable,
     ):
         self.feature_col_infos_by_lookup_key = feature_col_infos_by_lookup_key
         self.online_ft = online_ft
 
 
 def _load_raw_model(path):
     raw_model_path = os.path.join(path, mlflow_model_constants.RAW_MODEL_FOLDER)
     return mlflow.pyfunc.load_model(raw_model_path)
 
 
 class _FeatureStoreModelWrapper:
     def __init__(self, path: str):
         print(f"Initializing feature store lookup client: {VERSION}")
         self._check_support()
-        self.serving_environment = self._get_serving_environment()
-        feature_tables_for_serving = self._load_feature_tables_for_serving(
-            self.serving_environment, path
-        )
+        feature_tables_for_serving = self._load_feature_tables_for_serving()
 
         self.raw_model = _load_raw_model(path)
 
         # Reformat local metastore 3L tables to 2L. Non-local metastore 3L tables and 2L tables are unchanged.
         # This guarantees table name consistency between feature_spec and feature_tables_for_serving.
         # https://docs.google.com/document/d/1x_V9GshlnoAAFFCuDsXWdJVtop9MG2HWTUo5IK_1mEw
         original_feature_spec = FeatureSpec.load(path)
@@ -143,51 +135,29 @@
             path, mlflow_model_constants.FEATURE_STORE_INTERNAL_DATA_DIR
         )
         return os.path.isfile(
             os.path.join(feature_function_dir, FeatureFunctionsForServing.DATA_FILE)
         )
 
     # true if all feature tables using DynamoDB under same authorization (ie same region and keys)
-    # this is true by default for customers using Sagemaker
     def _is_model_eligible_for_batch_lookup(
         self, ft_metadata: Dict[str, _FeatureTableMetadata]
     ):
-        env = self._get_serving_environment()
         online_feature_tables = [meta.online_ft for _, meta in ft_metadata.items()]
-        if env == mlflow_model_constants.SAGEMAKER:
-            return is_primary_key_lookup(online_feature_tables)
-        elif env == mlflow_model_constants.DATABRICKS:
-            return tables_share_dynamodb_access_keys(
-                online_feature_tables
-            ) and is_primary_key_lookup(online_feature_tables)
-
-        raise Exception(f"Internal Error: Unexpected serving_environment {env}.")
+        return tables_share_dynamodb_access_keys(
+            online_feature_tables
+        ) and is_primary_key_lookup(online_feature_tables)
 
     @staticmethod
-    def _load_feature_tables_for_serving(
-        serving_environment: str, path: str
-    ) -> AbstractFeatureTablesForServing:
-        if serving_environment == mlflow_model_constants.DATABRICKS:
-            return FeatureTablesForServing.load(
-                path=os.getenv(FEATURE_TABLES_FOR_SERVING_FILEPATH_ENV)
-            )
-        elif serving_environment == mlflow_model_constants.SAGEMAKER:
-            return FeatureTablesForSageMakerServing.load(path=path)
-
-        raise Exception(
-            f"Internal Error: Unexpected serving_environment {serving_environment}."
+    def _load_feature_tables_for_serving() -> FeatureTablesForServing:
+        return FeatureTablesForServing.load(
+            path=os.getenv(FEATURE_TABLES_FOR_SERVING_FILEPATH_ENV)
         )
 
     @staticmethod
-    def _get_serving_environment() -> str:
-        if os.environ.get(SERVING_ENVIRONMENT) == SAGEMAKER_SERVING_ENVIRONMENT:
-            return mlflow_model_constants.SAGEMAKER
-        return mlflow_model_constants.DATABRICKS
-
-    @staticmethod
     def _is_lookup_client_instrumentation_enabled() -> bool:
         # environment variables stored as string, rather than boolean
         return os.getenv(LOOKUP_CLIENT_INSTRUMENTATION_ENABLED_ENV) == "true"
 
     @staticmethod
     def _is_lookup_client_feature_function_evaluation_enabled() -> bool:
         return (
@@ -217,17 +187,15 @@
                     )
 
     def _create_lookup_clients(
         self, ft_metadata: Dict[str, _FeatureTableMetadata]
     ) -> Dict[str, OnlineLookupClient]:
         ft_to_lookup_client = {}
         for ft, meta in ft_metadata.items():
-            ft_to_lookup_client[ft] = OnlineLookupClient(
-                meta.online_ft, serving_environment=self.serving_environment
-            )
+            ft_to_lookup_client[ft] = OnlineLookupClient(meta.online_ft)
         return ft_to_lookup_client
 
     def _create_batch_lookup_client(
         self, ft_metadata: Dict[str, _FeatureTableMetadata]
     ) -> Optional[OnlineLookupClient]:
         """
         Creates and returns an OnlineLookupClient for batch lookup, or None if `ft_metadata` is
@@ -235,17 +203,15 @@
         """
         if not ft_metadata:
             return None
         online_fts = []
         for ft, meta in ft_metadata.items():
             online_fts.append(meta.online_ft)
 
-        return OnlineLookupClient(
-            online_fts, serving_environment=self.serving_environment
-        )
+        return OnlineLookupClient(online_fts)
 
     def predict(self, df: pd.DataFrame):
         self._validate_input(df)
 
         # if enabled, use metrics class to record metric values in child function calls
         output_metrics = None
         if self._is_lookup_client_instrumentation_enabled():
@@ -294,15 +260,15 @@
             prediction.attrs = output_metrics.get_metrics()
 
         return prediction
 
     def _get_ft_metadata(
         self,
         feature_spec: FeatureSpec,
-        fts_for_serving: AbstractFeatureTablesForServing,
+        fts_for_serving: FeatureTablesForServing,
     ) -> Dict[str, _FeatureTableMetadata]:
         ft_to_lookup_key_to_feature_col_infos = (
             self._group_fcis_by_feature_table_lookup_key(feature_spec)
         )
         ft_names = ft_to_lookup_key_to_feature_col_infos.keys()
         ft_to_online_ft = self._resolve_online_stores(
             feature_tables=ft_names, feature_tables_for_serving=fts_for_serving
@@ -701,18 +667,18 @@
                     lookup_key
                 ].rename(feature_name_to_output_names[oft_name][lookup_key], axis=1)
         return feature_values
 
     def _resolve_online_stores(
         self,
         feature_tables: List[str],
-        feature_tables_for_serving: AbstractFeatureTablesForServing,
-    ) -> Dict[str, AbstractOnlineFeatureTable]:
+        feature_tables_for_serving: FeatureTablesForServing,
+    ) -> Dict[str, OnlineFeatureTable]:
         """
-        :return: feature table name -> AbstractOnlineFeatureTable
+        :return: feature table name -> OnlineFeatureTable
         """
         all_fts_to_online_ft = {
             online_ft.feature_table_name: online_ft
             for online_ft in feature_tables_for_serving.online_feature_tables
         }
 
         missing = [ft for ft in feature_tables if ft not in all_fts_to_online_ft.keys()]
```

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/mlflow_model_constants.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/mlflow_model_constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,11 @@
 #
 # - The Feature lookup client major version (eg `{FEATURE_LOOKUP_CLIENT_PIP_PACKAGE}.0.1`)
 # - The pinned major version of the databricks-feature-lookup requirement in logged model's conda.yaml
 #
 # If needed, these can be decoupled into separate constants, but that decision should be carefully considered.
 FEATURE_LOOKUP_CLIENT_MAJOR_VERSION = 0
 
-DATABRICKS = "Databricks"
-SAGEMAKER = "SageMaker"
-
 # Model artifact directory where we expect Feature Store internal artifacts to live. This must
 # match the directory specified in ModelServingUtils:
 # https://src.dev.databricks.com/databricks/universe@4dff77c752b546579f239815e520d566d2dbda20/-/blob/model-serving/model-serving-common/src/main/scala/com/databricks/modelservingcommon/utils/ModelServingUtils.scala?L117
 FEATURE_STORE_INTERNAL_DATA_DIR = "_databricks_internal/"
```

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/online_lookup_client.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/online_lookup_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 import os
 from typing import Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 
-from databricks.feature_store.entities.online_feature_table import (
-    AbstractOnlineFeatureTable,
-    OnlineFeatureTable,
-    OnlineFeatureTableForSageMakerServing,
-)
+from databricks.feature_store.entities.online_feature_table import OnlineFeatureTable
 from databricks.feature_store.entities.query_mode import QueryMode
 from databricks.feature_store.entities.store_type import StoreType
 from databricks.feature_store.lookup_engine import (
     AwsAccessKey,
     LookupBrickstoreEngine,
     LookupCosmosDbEngine,
     LookupDynamoDbEngine,
     LookupEngine,
     LookupMySqlEngine,
     LookupSqlEngine,
     LookupSqlServerEngine,
 )
-from databricks.feature_store.mlflow_model_constants import DATABRICKS, SAGEMAKER
 from databricks.feature_store.utils.metrics_utils import LookupClientMetrics
 
 # The provisioner of this model is expected to set the following environment variable for each
 # feature table if the feature store is SQL based:
 #  (1) <online_store_for_serving.read_secret_prefix>_USER
 #  (2) <online_store_for_serving.read_secret_prefix>_PASSWORD
 USER_SUFFIX = "_USER"
@@ -41,51 +36,45 @@
 # For Cosmos DB the following variable should be set:
 #  (1) <online_store_for_serving.read_secret_prefix>_AUTHORIZATION_KEY
 AUTHORIZATION_KEY_SUFFIX = "_AUTHORIZATION_KEY"
 LookupKeyType = Tuple[str, ...]
 
 
 def generate_lookup_sql_engine(
-    online_feature_table: Union[
-        AbstractOnlineFeatureTable, List[AbstractOnlineFeatureTable]
-    ],
+    online_feature_table: Union[OnlineFeatureTable, List[OnlineFeatureTable]],
     creds: Tuple[str, str],
 ) -> LookupSqlEngine:
     if isinstance(online_feature_table, List):
         raise Exception(f"Internal error: Batch lookup is unsupported in SQL Engine.")
 
     ro_user, ro_password = creds
     if online_feature_table.online_store.store_type == StoreType.BRICKSTORE:
         return LookupBrickstoreEngine(online_feature_table, ro_user, ro_password)
     elif online_feature_table.online_store.store_type == StoreType.SQL_SERVER:
         return LookupSqlServerEngine(online_feature_table, ro_user, ro_password)
     return LookupMySqlEngine(online_feature_table, ro_user, ro_password)
 
 
 def generate_lookup_dynamodb_engine(
-    online_feature_table: Union[
-        AbstractOnlineFeatureTable, List[AbstractOnlineFeatureTable]
-    ],
+    online_feature_table: Union[OnlineFeatureTable, List[OnlineFeatureTable]],
     creds: Optional[Tuple[str, str]],
 ) -> LookupDynamoDbEngine:
     if creds:
         access_key_id, secret_access_key = creds
 
         return LookupDynamoDbEngine(
             online_feature_table,
             access_key=AwsAccessKey(access_key_id, secret_access_key),
         )
     else:
         return LookupDynamoDbEngine(online_feature_table, access_key=None)
 
 
 def generate_lookup_cosmosdb_engine(
-    online_feature_table: Union[
-        AbstractOnlineFeatureTable, List[AbstractOnlineFeatureTable]
-    ],
+    online_feature_table: Union[OnlineFeatureTable, List[OnlineFeatureTable]],
     creds: str,
 ) -> LookupCosmosDbEngine:
     if isinstance(online_feature_table, List):
         raise Exception(f"Internal error: Batch lookup is unsupported in Cosmos DB.")
     return LookupCosmosDbEngine(online_feature_table, authorization_key=creds)
 
 
@@ -99,30 +88,40 @@
         if env_var not in os.environ:
             raise Exception(
                 f"Internal error: {env_var} not found for feature table {online_ft.feature_table_name}."
             )
         return os.getenv(env_var)
 
     if online_ft.online_store.store_type == StoreType.DYNAMODB:
-        return (
-            get_env_var(ACCESS_KEY_ID_SUFFIX),
-            get_env_var(SECRET_ACCESS_KEY_SUFFIX),
-        )
+        try:
+            return (
+                get_env_var(ACCESS_KEY_ID_SUFFIX),
+                get_env_var(SECRET_ACCESS_KEY_SUFFIX),
+            )
+        except:
+            # It is assumed that if the secrets are not configured, the lookup will be authorized
+            # using instance profile. This is validated in serving-scheduler on endpoint creation
+            # see EndpointDeploymentProvisioner.verifyAndMaybeUpdateFsMetadataForInstanceProfile
+            # TODO (ML-33307): add env var check whether instance profile is configured
+            print(
+                "Secret credentials not configured, attempting to use cluster instance profile."
+            )
+            return None
     elif online_ft.online_store.store_type == StoreType.COSMOSDB:
         return get_env_var(AUTHORIZATION_KEY_SUFFIX)
     else:
         return (
             get_env_var(USER_SUFFIX),
             get_env_var(PASSWORD_SUFFIX),
         )
 
 
 # TODO(ML-26146): refactor this method and above helpers to appropriate seperate util files
 def tables_share_dynamodb_access_keys(
-    online_feature_tables: List[AbstractOnlineFeatureTable],
+    online_feature_tables: List[OnlineFeatureTable],
 ):
     # check region and credentials to see if all feature tables are using same DynamoDB accesss keys
     region, creds = None, None
     for ft in online_feature_tables:
         if ft.online_store.store_type != StoreType.DYNAMODB:
             return False
         elif region == None:
@@ -133,97 +132,37 @@
             or load_credentials_from_env(ft) != creds
         ):
             return False
     return True
 
 
 def is_primary_key_lookup(
-    online_feature_tables: List[AbstractOnlineFeatureTable],
+    online_feature_tables: List[OnlineFeatureTable],
 ):
     for oft in online_feature_tables:
         mode = oft.online_store.query_mode
         if mode == QueryMode.RANGE_QUERY:
             return False
         elif mode == QueryMode.PRIMARY_KEY_LOOKUP:
             continue
         else:
             raise ValueError(f"Unsupported query mode: {mode}")
     return True
 
 
-def check_instance_type(
-    online_feature_table: Union[
-        AbstractOnlineFeatureTable, List[AbstractOnlineFeatureTable]
-    ],
-    cls: Union[OnlineFeatureTable, OnlineFeatureTableForSageMakerServing],
-    serving_environment: str,
-):
-    if isinstance(online_feature_table, cls):
-        return True
-    elif isinstance(online_feature_table, List):
-        for oft in online_feature_table:
-            if not isinstance(oft, cls):
-                raise Exception(
-                    f"Internal Error: Expected {cls} when serving_environment={serving_environment}"
-                    f". Got {type(oft)}."
-                )
-        return True
-
-    raise Exception(
-        f"Internal Error: Expected {cls} when serving_environment={serving_environment}"
-        f". Got {type(online_feature_table)}."
-    )
-
-
 class OnlineLookupClient:
     def __init__(
-        self,
-        online_feature_table: Union[
-            AbstractOnlineFeatureTable, List[AbstractOnlineFeatureTable]
-        ],
-        serving_environment: str,
-    ):
-        self.lookup_engine = self._generate_lookup_engine(
-            online_feature_table, serving_environment
-        )
-
-    @staticmethod
-    def _generate_lookup_engine(
-        online_feature_table: Union[
-            AbstractOnlineFeatureTable, List[AbstractOnlineFeatureTable]
-        ],
-        serving_environment: str,
+        self, online_feature_table: Union[OnlineFeatureTable, List[OnlineFeatureTable]]
     ):
-        if serving_environment == DATABRICKS:
-            check_instance_type(
-                online_feature_table, OnlineFeatureTable, serving_environment
-            )
-            return OnlineLookupClient._generate_lookup_engine_databricks(
-                online_feature_table
-            )
-        elif serving_environment == SAGEMAKER:
-            check_instance_type(
-                online_feature_table,
-                OnlineFeatureTableForSageMakerServing,
-                serving_environment,
-            )
-            return OnlineLookupClient._generate_lookup_engine_sagemaker(
-                online_feature_table
-            )
-
-        raise Exception(
-            f"Internal Error: Unexpected serving_environment {serving_environment}."
-        )
+        self.lookup_engine = self._generate_lookup_engine(online_feature_table)
 
     @classmethod
-    def _generate_lookup_engine_databricks(
+    def _generate_lookup_engine(
         cls,
-        online_feature_table: Union[
-            AbstractOnlineFeatureTable, List[AbstractOnlineFeatureTable]
-        ],
+        online_feature_table: Union[OnlineFeatureTable, List[OnlineFeatureTable]],
     ):
         first_online_feature_table = None
         if isinstance(online_feature_table, List):
             if len(online_feature_table) == 0:
                 raise Exception(
                     f"Internal Error: No feature table passed while creating lookup engine."
                 )
@@ -235,20 +174,14 @@
         if first_online_feature_table.online_store.store_type == StoreType.DYNAMODB:
             return generate_lookup_dynamodb_engine(online_feature_table, creds)
         elif first_online_feature_table.online_store.store_type == StoreType.COSMOSDB:
             return generate_lookup_cosmosdb_engine(online_feature_table, creds)
         else:
             return generate_lookup_sql_engine(online_feature_table, creds)
 
-    @classmethod
-    def _generate_lookup_engine_sagemaker(
-        cls, online_feature_table: OnlineFeatureTableForSageMakerServing
-    ):
-        return generate_lookup_dynamodb_engine(online_feature_table, creds=None)
-
     def batch_lookup_features(
         self,
         lookup_df_dict: Dict[str, Dict[LookupKeyType, pd.DataFrame]],
         feature_names_dict: Dict[str, Dict[LookupKeyType, List[str]]],
         *,
         metrics: LookupClientMetrics = None,
     ) -> Dict[str, Dict[LookupKeyType, pd.DataFrame]]:
@@ -266,15 +199,15 @@
         lookup_df: pd.DataFrame,
         feature_names: List[str],
         *,
         metrics: LookupClientMetrics = None,
     ) -> pd.DataFrame:
         """Uses a Python database connection to lookup features in feature_names using
         the lookup keys and values in lookup_df. The online store database and table name are
-        obtained from the AbstractOnlineFeatureTable passed to the constructor.
+        obtained from the OnlineFeatureTable passed to the constructor.
 
         The resulting DataFrame has the same number of rows as lookup_df. In the case that a lookup
         key cannot be found, a row of NaNs will be returned in the resulting DataFrame.
 
         Throws an exception if the table, lookup keys, or feature columns do not exist in the
         online store.
```

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/protos/feature_spec_pb2.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/protos/feature_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/protos/feature_store_serving_pb2.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/protos/feature_store_serving_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from mlflow.protos.scalapb import scalapb_pb2 as scalapb_dot_scalapb__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66\x65\x61ture_store_serving.proto\x12\x12\x66\x65\x61turestorecommon\x1a\x15scalapb/scalapb.proto\"\x9b\x04\n\x15OnlineStoreForServing\x12(\n\x05\x63loud\x18\x01 \x01(\x0e\x32\x19.featurestorecommon.Cloud\x12\x31\n\nstore_type\x18\x02 \x01(\x0e\x32\x1d.featurestorecommon.StoreType\x12\x1a\n\x12read_secret_prefix\x18\x03 \x01(\t\x12\x1d\n\x15\x63reation_timestamp_ms\x18\x04 \x01(\x03\x12\x33\n\nmysql_conf\x18\x05 \x01(\x0b\x32\x1d.featurestorecommon.MySqlConfH\x00\x12<\n\x0fsql_server_conf\x18\x06 \x01(\x0b\x32!.featurestorecommon.SqlServerConfH\x00\x12\x39\n\rdynamodb_conf\x18\x07 \x01(\x0b\x32 .featurestorecommon.DynamoDbConfH\x00\x12\x39\n\rcosmosdb_conf\x18\x08 \x01(\x0b\x32 .featurestorecommon.CosmosDbConfH\x00\x12=\n\x0f\x62rickstore_conf\x18\t \x01(\x0b\x32\".featurestorecommon.BrickstoreConfH\x00\x12\x31\n\nquery_mode\x18\x15 \x01(\x0e\x32\x1d.featurestorecommon.QueryModeB\x0f\n\rextra_configs\"\'\n\tMySqlConf\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"+\n\rSqlServerConf\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x1e\n\x0c\x44ynamoDbConf\x12\x0e\n\x06region\x18\x01 \x01(\t\"#\n\x0c\x43osmosDbConf\x12\x13\n\x0b\x61\x63\x63ount_uri\x18\x01 \x01(\t\",\n\x0e\x42rickstoreConf\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"j\n\x0e\x46\x65\x61tureDetails\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tdata_type\x18\x02 \x01(\x0e\x32\x1c.featurestorecommon.DataType\x12\x19\n\x11\x64\x61ta_type_details\x18\x03 \x01(\t\"R\n\x11PrimaryKeyDetails\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tdata_type\x18\x02 \x01(\x0e\x32\x1c.featurestorecommon.DataType\"T\n\x13TimestampKeyDetails\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tdata_type\x18\x02 \x01(\x0e\x32\x1c.featurestorecommon.DataType\"\xe2\x02\n\x12OnlineFeatureTable\x12\x1a\n\x12\x66\x65\x61ture_table_name\x18\x01 \x01(\t\x12!\n\x19online_feature_table_name\x18\x02 \x01(\t\x12?\n\x0conline_store\x18\x03 \x01(\x0b\x32).featurestorecommon.OnlineStoreForServing\x12;\n\x0cprimary_keys\x18\x04 \x03(\x0b\x32%.featurestorecommon.PrimaryKeyDetails\x12\x18\n\x10\x66\x65\x61ture_table_id\x18\x05 \x01(\t\x12\x34\n\x08\x66\x65\x61tures\x18\x06 \x03(\x0b\x32\".featurestorecommon.FeatureDetails\x12?\n\x0etimestamp_keys\x18\x07 \x03(\x0b\x32\'.featurestorecommon.TimestampKeyDetails\"X\n\x17\x46\x65\x61tureTablesForServing\x12=\n\ronline_tables\x18\x01 \x03(\x0b\x32&.featurestorecommon.OnlineFeatureTable\"+\n\rMySqlMetadata\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"/\n\x11SqlServerMetadata\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"B\n\x10\x44ynamoDbMetadata\x12\x0e\n\x06region\x18\x01 \x01(\t\x12\x11\n\ttable_arn\x18\x02 \x01(\t\x12\x0b\n\x03ttl\x18\x03 \x01(\x03\"K\n\x10\x43osmosDbMetadata\x12\x13\n\x0b\x61\x63\x63ount_uri\x18\x01 \x01(\t\x12\x15\n\rcontainer_uri\x18\x02 \x01(\t\x12\x0b\n\x03ttl\x18\x03 \x01(\x03\"\xa9\x04\n\x0bOnlineStore\x12(\n\x05\x63loud\x18\x01 \x01(\x0e\x32\x19.featurestorecommon.Cloud\x12\x31\n\nstore_type\x18\x02 \x01(\x0e\x32\x1d.featurestorecommon.StoreType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12\x63reation_timestamp\x18\x04 \x01(\x03\x12\x1e\n\x16last_updated_timestamp\x18\x05 \x01(\x03\x12\x12\n\ncreator_id\x18\x06 \x01(\t\x12\x10\n\x04host\x18\x07 \x01(\tB\x02\x18\x01\x12\x10\n\x04port\x18\x08 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x13last_update_user_id\x18\t \x01(\t\x12;\n\x0emysql_metadata\x18\n \x01(\x0b\x32!.featurestorecommon.MySqlMetadataH\x00\x12\x44\n\x13sql_server_metadata\x18\x0b \x01(\x0b\x32%.featurestorecommon.SqlServerMetadataH\x00\x12\x41\n\x11\x64ynamodb_metadata\x18\x0c \x01(\x0b\x32$.featurestorecommon.DynamoDbMetadataH\x00\x12\x41\n\x11\x63osmosdb_metadata\x18\r \x01(\x0b\x32$.featurestorecommon.CosmosDbMetadataH\x00\x42\x15\n\x13\x61\x64\x64itional_metadata\"\xdf\x04\n\x13OnlineStoreDetailed\x12(\n\x05\x63loud\x18\x01 \x01(\x0e\x32\x19.featurestorecommon.Cloud\x12\x31\n\nstore_type\x18\x02 \x01(\x0e\x32\x1d.featurestorecommon.StoreType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12\x63reation_timestamp\x18\x04 \x01(\x03\x12\x1e\n\x16last_updated_timestamp\x18\x05 \x01(\x03\x12\x12\n\ncreator_id\x18\x06 \x01(\t\x12\x10\n\x04host\x18\x07 \x01(\tB\x02\x18\x01\x12\x10\n\x04port\x18\x08 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x13last_update_user_id\x18\t \x01(\t\x12\x10\n\x08\x66\x65\x61tures\x18\n \x03(\t\x12\x1a\n\x12read_secret_prefix\x18\x0b \x01(\t\x12;\n\x0emysql_metadata\x18\x0c \x01(\x0b\x32!.featurestorecommon.MySqlMetadataH\x00\x12\x44\n\x13sql_server_metadata\x18\r \x01(\x0b\x32%.featurestorecommon.SqlServerMetadataH\x00\x12\x41\n\x11\x64ynamodb_metadata\x18\x0e \x01(\x0b\x32$.featurestorecommon.DynamoDbMetadataH\x00\x12\x41\n\x11\x63osmosdb_metadata\x18\x0f \x01(\x0b\x32$.featurestorecommon.CosmosDbMetadataH\x00\x42\x15\n\x13\x61\x64\x64itional_metadata\"t\n FeatureTablesForSageMakerServing\x12P\n\ronline_tables\x18\x01 \x03(\x0b\x32\x39.featurestorecommon.OnlineFeatureTableForSageMakerServing\"\xfe\x02\n%OnlineFeatureTableForSageMakerServing\x12\x1a\n\x12\x66\x65\x61ture_table_name\x18\x01 \x01(\t\x12!\n\x19online_feature_table_name\x18\x02 \x01(\t\x12H\n\x0conline_store\x18\x03 \x01(\x0b\x32\x32.featurestorecommon.OnlineStoreForSageMakerServing\x12;\n\x0cprimary_keys\x18\x04 \x03(\x0b\x32%.featurestorecommon.PrimaryKeyDetails\x12\x18\n\x10\x66\x65\x61ture_table_id\x18\x05 \x01(\t\x12\x34\n\x08\x66\x65\x61tures\x18\x06 \x03(\x0b\x32\".featurestorecommon.FeatureDetails\x12?\n\x0etimestamp_keys\x18\x07 \x03(\x0b\x32\'.featurestorecommon.TimestampKeyDetails\"\xbe\x01\n\x1eOnlineStoreForSageMakerServing\x12\x1d\n\x15\x63reation_timestamp_ms\x18\x01 \x01(\x03\x12\x39\n\rdynamodb_conf\x18\x02 \x01(\x0b\x32 .featurestorecommon.DynamoDbConfH\x00\x12\x31\n\nquery_mode\x18\x10 \x01(\x0e\x32\x1d.featurestorecommon.QueryModeB\x0f\n\rextra_configs\"\x83\x01\n\x1c\x46\x65\x61tureFunctionParameterInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\ttype_text\x18\x02 \x01(\t\x12\x11\n\ttype_json\x18\x03 \x01(\t\x12/\n\ttype_name\x18\x04 \x01(\x0e\x32\x1c.featurestorecommon.DataType\"\xdb\x01\n\x19\x46\x65\x61tureFunctionForServing\x12\x11\n\tfull_name\x18\x01 \x01(\t\x12\x46\n\x0cinput_params\x18\x02 \x03(\x0b\x32\x30.featurestorecommon.FeatureFunctionParameterInfo\x12/\n\tdata_type\x18\x03 \x01(\x0e\x32\x1c.featurestorecommon.DataType\x12\x16\n\x0e\x66ull_data_type\x18\x04 \x01(\t\x12\x1a\n\x12routine_definition\x18\x05 \x01(\t\"c\n\x1a\x46\x65\x61tureFunctionsForServing\x12\x45\n\x0e\x66\x66_for_serving\x18\x01 \x03(\x0b\x32-.featurestorecommon.FeatureFunctionForServing*$\n\x05\x43loud\x12\x07\n\x03\x41WS\x10\x01\x12\t\n\x05\x41ZURE\x10\x02\x12\x07\n\x03GCP\x10\x03*d\n\tStoreType\x12\x10\n\x0c\x41URORA_MYSQL\x10\x01\x12\x0e\n\nSQL_SERVER\x10\x02\x12\t\n\x05MYSQL\x10\x03\x12\x0c\n\x08\x44YNAMODB\x10\x04\x12\x0c\n\x08\x43OSMOSDB\x10\x05\x12\x0e\n\nBRICKSTORE\x10\x06*\xa2\x01\n\x08\x44\x61taType\x12\x0b\n\x07INTEGER\x10\x01\x12\t\n\x05\x46LOAT\x10\x02\x12\x0b\n\x07\x42OOLEAN\x10\x03\x12\n\n\x06STRING\x10\x04\x12\n\n\x06\x44OUBLE\x10\x05\x12\x08\n\x04LONG\x10\x06\x12\r\n\tTIMESTAMP\x10\x07\x12\x08\n\x04\x44\x41TE\x10\x08\x12\t\n\x05SHORT\x10\t\x12\t\n\x05\x41RRAY\x10\n\x12\x07\n\x03MAP\x10\x0b\x12\n\n\x06\x42INARY\x10\x0c\x12\x0b\n\x07\x44\x45\x43IMAL\x10\r*4\n\tQueryMode\x12\x16\n\x12PRIMARY_KEY_LOOKUP\x10\x00\x12\x0f\n\x0bRANGE_QUERY\x10\x01\x42\x31\n\'com.databricks.proto.featurestorecommon\xa0\x01\x01\xe2?\x02\x10\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66\x65\x61ture_store_serving.proto\x12\x12\x66\x65\x61turestorecommon\x1a\x15scalapb/scalapb.proto\"\x9b\x04\n\x15OnlineStoreForServing\x12(\n\x05\x63loud\x18\x01 \x01(\x0e\x32\x19.featurestorecommon.Cloud\x12\x31\n\nstore_type\x18\x02 \x01(\x0e\x32\x1d.featurestorecommon.StoreType\x12\x1a\n\x12read_secret_prefix\x18\x03 \x01(\t\x12\x1d\n\x15\x63reation_timestamp_ms\x18\x04 \x01(\x03\x12\x33\n\nmysql_conf\x18\x05 \x01(\x0b\x32\x1d.featurestorecommon.MySqlConfH\x00\x12<\n\x0fsql_server_conf\x18\x06 \x01(\x0b\x32!.featurestorecommon.SqlServerConfH\x00\x12\x39\n\rdynamodb_conf\x18\x07 \x01(\x0b\x32 .featurestorecommon.DynamoDbConfH\x00\x12\x39\n\rcosmosdb_conf\x18\x08 \x01(\x0b\x32 .featurestorecommon.CosmosDbConfH\x00\x12=\n\x0f\x62rickstore_conf\x18\t \x01(\x0b\x32\".featurestorecommon.BrickstoreConfH\x00\x12\x31\n\nquery_mode\x18\x15 \x01(\x0e\x32\x1d.featurestorecommon.QueryModeB\x0f\n\rextra_configs\"\'\n\tMySqlConf\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"+\n\rSqlServerConf\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x1e\n\x0c\x44ynamoDbConf\x12\x0e\n\x06region\x18\x01 \x01(\t\"#\n\x0c\x43osmosDbConf\x12\x13\n\x0b\x61\x63\x63ount_uri\x18\x01 \x01(\t\",\n\x0e\x42rickstoreConf\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"j\n\x0e\x46\x65\x61tureDetails\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tdata_type\x18\x02 \x01(\x0e\x32\x1c.featurestorecommon.DataType\x12\x19\n\x11\x64\x61ta_type_details\x18\x03 \x01(\t\"R\n\x11PrimaryKeyDetails\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tdata_type\x18\x02 \x01(\x0e\x32\x1c.featurestorecommon.DataType\"T\n\x13TimestampKeyDetails\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tdata_type\x18\x02 \x01(\x0e\x32\x1c.featurestorecommon.DataType\"\xe2\x02\n\x12OnlineFeatureTable\x12\x1a\n\x12\x66\x65\x61ture_table_name\x18\x01 \x01(\t\x12!\n\x19online_feature_table_name\x18\x02 \x01(\t\x12?\n\x0conline_store\x18\x03 \x01(\x0b\x32).featurestorecommon.OnlineStoreForServing\x12;\n\x0cprimary_keys\x18\x04 \x03(\x0b\x32%.featurestorecommon.PrimaryKeyDetails\x12\x18\n\x10\x66\x65\x61ture_table_id\x18\x05 \x01(\t\x12\x34\n\x08\x66\x65\x61tures\x18\x06 \x03(\x0b\x32\".featurestorecommon.FeatureDetails\x12?\n\x0etimestamp_keys\x18\x07 \x03(\x0b\x32\'.featurestorecommon.TimestampKeyDetails\"X\n\x17\x46\x65\x61tureTablesForServing\x12=\n\ronline_tables\x18\x01 \x03(\x0b\x32&.featurestorecommon.OnlineFeatureTable\"+\n\rMySqlMetadata\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"/\n\x11SqlServerMetadata\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"B\n\x10\x44ynamoDbMetadata\x12\x0e\n\x06region\x18\x01 \x01(\t\x12\x11\n\ttable_arn\x18\x02 \x01(\t\x12\x0b\n\x03ttl\x18\x03 \x01(\x03\"K\n\x10\x43osmosDbMetadata\x12\x13\n\x0b\x61\x63\x63ount_uri\x18\x01 \x01(\t\x12\x15\n\rcontainer_uri\x18\x02 \x01(\t\x12\x0b\n\x03ttl\x18\x03 \x01(\x03\"\xa9\x04\n\x0bOnlineStore\x12(\n\x05\x63loud\x18\x01 \x01(\x0e\x32\x19.featurestorecommon.Cloud\x12\x31\n\nstore_type\x18\x02 \x01(\x0e\x32\x1d.featurestorecommon.StoreType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12\x63reation_timestamp\x18\x04 \x01(\x03\x12\x1e\n\x16last_updated_timestamp\x18\x05 \x01(\x03\x12\x12\n\ncreator_id\x18\x06 \x01(\t\x12\x10\n\x04host\x18\x07 \x01(\tB\x02\x18\x01\x12\x10\n\x04port\x18\x08 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x13last_update_user_id\x18\t \x01(\t\x12;\n\x0emysql_metadata\x18\n \x01(\x0b\x32!.featurestorecommon.MySqlMetadataH\x00\x12\x44\n\x13sql_server_metadata\x18\x0b \x01(\x0b\x32%.featurestorecommon.SqlServerMetadataH\x00\x12\x41\n\x11\x64ynamodb_metadata\x18\x0c \x01(\x0b\x32$.featurestorecommon.DynamoDbMetadataH\x00\x12\x41\n\x11\x63osmosdb_metadata\x18\r \x01(\x0b\x32$.featurestorecommon.CosmosDbMetadataH\x00\x42\x15\n\x13\x61\x64\x64itional_metadata\"\xdf\x04\n\x13OnlineStoreDetailed\x12(\n\x05\x63loud\x18\x01 \x01(\x0e\x32\x19.featurestorecommon.Cloud\x12\x31\n\nstore_type\x18\x02 \x01(\x0e\x32\x1d.featurestorecommon.StoreType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12\x63reation_timestamp\x18\x04 \x01(\x03\x12\x1e\n\x16last_updated_timestamp\x18\x05 \x01(\x03\x12\x12\n\ncreator_id\x18\x06 \x01(\t\x12\x10\n\x04host\x18\x07 \x01(\tB\x02\x18\x01\x12\x10\n\x04port\x18\x08 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x13last_update_user_id\x18\t \x01(\t\x12\x10\n\x08\x66\x65\x61tures\x18\n \x03(\t\x12\x1a\n\x12read_secret_prefix\x18\x0b \x01(\t\x12;\n\x0emysql_metadata\x18\x0c \x01(\x0b\x32!.featurestorecommon.MySqlMetadataH\x00\x12\x44\n\x13sql_server_metadata\x18\r \x01(\x0b\x32%.featurestorecommon.SqlServerMetadataH\x00\x12\x41\n\x11\x64ynamodb_metadata\x18\x0e \x01(\x0b\x32$.featurestorecommon.DynamoDbMetadataH\x00\x12\x41\n\x11\x63osmosdb_metadata\x18\x0f \x01(\x0b\x32$.featurestorecommon.CosmosDbMetadataH\x00\x42\x15\n\x13\x61\x64\x64itional_metadata\"\x83\x01\n\x1c\x46\x65\x61tureFunctionParameterInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\ttype_text\x18\x02 \x01(\t\x12\x11\n\ttype_json\x18\x03 \x01(\t\x12/\n\ttype_name\x18\x04 \x01(\x0e\x32\x1c.featurestorecommon.DataType\"\xdb\x01\n\x19\x46\x65\x61tureFunctionForServing\x12\x11\n\tfull_name\x18\x01 \x01(\t\x12\x46\n\x0cinput_params\x18\x02 \x03(\x0b\x32\x30.featurestorecommon.FeatureFunctionParameterInfo\x12/\n\tdata_type\x18\x03 \x01(\x0e\x32\x1c.featurestorecommon.DataType\x12\x16\n\x0e\x66ull_data_type\x18\x04 \x01(\t\x12\x1a\n\x12routine_definition\x18\x05 \x01(\t\"c\n\x1a\x46\x65\x61tureFunctionsForServing\x12\x45\n\x0e\x66\x66_for_serving\x18\x01 \x03(\x0b\x32-.featurestorecommon.FeatureFunctionForServing*$\n\x05\x43loud\x12\x07\n\x03\x41WS\x10\x01\x12\t\n\x05\x41ZURE\x10\x02\x12\x07\n\x03GCP\x10\x03*d\n\tStoreType\x12\x10\n\x0c\x41URORA_MYSQL\x10\x01\x12\x0e\n\nSQL_SERVER\x10\x02\x12\t\n\x05MYSQL\x10\x03\x12\x0c\n\x08\x44YNAMODB\x10\x04\x12\x0c\n\x08\x43OSMOSDB\x10\x05\x12\x0e\n\nBRICKSTORE\x10\x06*\xa2\x01\n\x08\x44\x61taType\x12\x0b\n\x07INTEGER\x10\x01\x12\t\n\x05\x46LOAT\x10\x02\x12\x0b\n\x07\x42OOLEAN\x10\x03\x12\n\n\x06STRING\x10\x04\x12\n\n\x06\x44OUBLE\x10\x05\x12\x08\n\x04LONG\x10\x06\x12\r\n\tTIMESTAMP\x10\x07\x12\x08\n\x04\x44\x41TE\x10\x08\x12\t\n\x05SHORT\x10\t\x12\t\n\x05\x41RRAY\x10\n\x12\x07\n\x03MAP\x10\x0b\x12\n\n\x06\x42INARY\x10\x0c\x12\x0b\n\x07\x44\x45\x43IMAL\x10\r*4\n\tQueryMode\x12\x16\n\x12PRIMARY_KEY_LOOKUP\x10\x00\x12\x0f\n\x0bRANGE_QUERY\x10\x01\x42\x31\n\'com.databricks.proto.featurestorecommon\xa0\x01\x01\xe2?\x02\x10\x01')
 
 _CLOUD = DESCRIPTOR.enum_types_by_name['Cloud']
 Cloud = enum_type_wrapper.EnumTypeWrapper(_CLOUD)
 _STORETYPE = DESCRIPTOR.enum_types_by_name['StoreType']
 StoreType = enum_type_wrapper.EnumTypeWrapper(_STORETYPE)
 _DATATYPE = DESCRIPTOR.enum_types_by_name['DataType']
 DataType = enum_type_wrapper.EnumTypeWrapper(_DATATYPE)
@@ -65,17 +65,14 @@
 _FEATURETABLESFORSERVING = DESCRIPTOR.message_types_by_name['FeatureTablesForServing']
 _MYSQLMETADATA = DESCRIPTOR.message_types_by_name['MySqlMetadata']
 _SQLSERVERMETADATA = DESCRIPTOR.message_types_by_name['SqlServerMetadata']
 _DYNAMODBMETADATA = DESCRIPTOR.message_types_by_name['DynamoDbMetadata']
 _COSMOSDBMETADATA = DESCRIPTOR.message_types_by_name['CosmosDbMetadata']
 _ONLINESTORE = DESCRIPTOR.message_types_by_name['OnlineStore']
 _ONLINESTOREDETAILED = DESCRIPTOR.message_types_by_name['OnlineStoreDetailed']
-_FEATURETABLESFORSAGEMAKERSERVING = DESCRIPTOR.message_types_by_name['FeatureTablesForSageMakerServing']
-_ONLINEFEATURETABLEFORSAGEMAKERSERVING = DESCRIPTOR.message_types_by_name['OnlineFeatureTableForSageMakerServing']
-_ONLINESTOREFORSAGEMAKERSERVING = DESCRIPTOR.message_types_by_name['OnlineStoreForSageMakerServing']
 _FEATUREFUNCTIONPARAMETERINFO = DESCRIPTOR.message_types_by_name['FeatureFunctionParameterInfo']
 _FEATUREFUNCTIONFORSERVING = DESCRIPTOR.message_types_by_name['FeatureFunctionForServing']
 _FEATUREFUNCTIONSFORSERVING = DESCRIPTOR.message_types_by_name['FeatureFunctionsForServing']
 OnlineStoreForServing = _reflection.GeneratedProtocolMessageType('OnlineStoreForServing', (_message.Message,), {
   'DESCRIPTOR' : _ONLINESTOREFORSERVING,
   '__module__' : 'feature_store_serving_pb2'
   # @@protoc_insertion_point(class_scope:featurestorecommon.OnlineStoreForServing)
@@ -190,35 +187,14 @@
 OnlineStoreDetailed = _reflection.GeneratedProtocolMessageType('OnlineStoreDetailed', (_message.Message,), {
   'DESCRIPTOR' : _ONLINESTOREDETAILED,
   '__module__' : 'feature_store_serving_pb2'
   # @@protoc_insertion_point(class_scope:featurestorecommon.OnlineStoreDetailed)
   })
 _sym_db.RegisterMessage(OnlineStoreDetailed)
 
-FeatureTablesForSageMakerServing = _reflection.GeneratedProtocolMessageType('FeatureTablesForSageMakerServing', (_message.Message,), {
-  'DESCRIPTOR' : _FEATURETABLESFORSAGEMAKERSERVING,
-  '__module__' : 'feature_store_serving_pb2'
-  # @@protoc_insertion_point(class_scope:featurestorecommon.FeatureTablesForSageMakerServing)
-  })
-_sym_db.RegisterMessage(FeatureTablesForSageMakerServing)
-
-OnlineFeatureTableForSageMakerServing = _reflection.GeneratedProtocolMessageType('OnlineFeatureTableForSageMakerServing', (_message.Message,), {
-  'DESCRIPTOR' : _ONLINEFEATURETABLEFORSAGEMAKERSERVING,
-  '__module__' : 'feature_store_serving_pb2'
-  # @@protoc_insertion_point(class_scope:featurestorecommon.OnlineFeatureTableForSageMakerServing)
-  })
-_sym_db.RegisterMessage(OnlineFeatureTableForSageMakerServing)
-
-OnlineStoreForSageMakerServing = _reflection.GeneratedProtocolMessageType('OnlineStoreForSageMakerServing', (_message.Message,), {
-  'DESCRIPTOR' : _ONLINESTOREFORSAGEMAKERSERVING,
-  '__module__' : 'feature_store_serving_pb2'
-  # @@protoc_insertion_point(class_scope:featurestorecommon.OnlineStoreForSageMakerServing)
-  })
-_sym_db.RegisterMessage(OnlineStoreForSageMakerServing)
-
 FeatureFunctionParameterInfo = _reflection.GeneratedProtocolMessageType('FeatureFunctionParameterInfo', (_message.Message,), {
   'DESCRIPTOR' : _FEATUREFUNCTIONPARAMETERINFO,
   '__module__' : 'feature_store_serving_pb2'
   # @@protoc_insertion_point(class_scope:featurestorecommon.FeatureFunctionParameterInfo)
   })
 _sym_db.RegisterMessage(FeatureFunctionParameterInfo)
 
@@ -244,22 +220,22 @@
   _ONLINESTORE.fields_by_name['host']._serialized_options = b'\030\001'
   _ONLINESTORE.fields_by_name['port']._options = None
   _ONLINESTORE.fields_by_name['port']._serialized_options = b'\030\001'
   _ONLINESTOREDETAILED.fields_by_name['host']._options = None
   _ONLINESTOREDETAILED.fields_by_name['host']._serialized_options = b'\030\001'
   _ONLINESTOREDETAILED.fields_by_name['port']._options = None
   _ONLINESTOREDETAILED.fields_by_name['port']._serialized_options = b'\030\001'
-  _CLOUD._serialized_start=4100
-  _CLOUD._serialized_end=4136
-  _STORETYPE._serialized_start=4138
-  _STORETYPE._serialized_end=4238
-  _DATATYPE._serialized_start=4241
-  _DATATYPE._serialized_end=4403
-  _QUERYMODE._serialized_start=4405
-  _QUERYMODE._serialized_end=4457
+  _CLOUD._serialized_start=3404
+  _CLOUD._serialized_end=3440
+  _STORETYPE._serialized_start=3442
+  _STORETYPE._serialized_end=3542
+  _DATATYPE._serialized_start=3545
+  _DATATYPE._serialized_end=3707
+  _QUERYMODE._serialized_start=3709
+  _QUERYMODE._serialized_end=3761
   _ONLINESTOREFORSERVING._serialized_start=75
   _ONLINESTOREFORSERVING._serialized_end=614
   _MYSQLCONF._serialized_start=616
   _MYSQLCONF._serialized_end=655
   _SQLSERVERCONF._serialized_start=657
   _SQLSERVERCONF._serialized_end=700
   _DYNAMODBCONF._serialized_start=702
@@ -286,20 +262,14 @@
   _DYNAMODBMETADATA._serialized_end=1702
   _COSMOSDBMETADATA._serialized_start=1704
   _COSMOSDBMETADATA._serialized_end=1779
   _ONLINESTORE._serialized_start=1782
   _ONLINESTORE._serialized_end=2335
   _ONLINESTOREDETAILED._serialized_start=2338
   _ONLINESTOREDETAILED._serialized_end=2945
-  _FEATURETABLESFORSAGEMAKERSERVING._serialized_start=2947
-  _FEATURETABLESFORSAGEMAKERSERVING._serialized_end=3063
-  _ONLINEFEATURETABLEFORSAGEMAKERSERVING._serialized_start=3066
-  _ONLINEFEATURETABLEFORSAGEMAKERSERVING._serialized_end=3448
-  _ONLINESTOREFORSAGEMAKERSERVING._serialized_start=3451
-  _ONLINESTOREFORSAGEMAKERSERVING._serialized_end=3641
-  _FEATUREFUNCTIONPARAMETERINFO._serialized_start=3644
-  _FEATUREFUNCTIONPARAMETERINFO._serialized_end=3775
-  _FEATUREFUNCTIONFORSERVING._serialized_start=3778
-  _FEATUREFUNCTIONFORSERVING._serialized_end=3997
-  _FEATUREFUNCTIONSFORSERVING._serialized_start=3999
-  _FEATUREFUNCTIONSFORSERVING._serialized_end=4098
+  _FEATUREFUNCTIONPARAMETERINFO._serialized_start=2948
+  _FEATUREFUNCTIONPARAMETERINFO._serialized_end=3079
+  _FEATUREFUNCTIONFORSERVING._serialized_start=3082
+  _FEATUREFUNCTIONFORSERVING._serialized_end=3301
+  _FEATUREFUNCTIONSFORSERVING._serialized_start=3303
+  _FEATUREFUNCTIONSFORSERVING._serialized_end=3402
 # @@protoc_insertion_point(module_scope)
```

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/converter_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/converter_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/cosmosdb_type_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/cosmosdb_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/cosmosdb_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/cosmosdb_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from azure.cosmos.exceptions import CosmosResourceNotFoundError
 
 PARTITION_KEY = "partitionKey"
 PATHS = "paths"
 PRIMARY_KEY_PROPERTY_NAME_VALUE = "_feature_store_internal__primary_keys"
 FEATURE_STORE_SENTINEL_ID_VALUE = "_fs"
 
+DEFAULT_RETRY_CONFIG = {"retry_total": 3, "timeout": 30}
+
 
 def to_cosmosdb_primary_key(primary_key_values: List[Any]):
     return json.dumps(primary_key_values)
 
 
 def is_not_found_error(e: Exception) -> bool:
     # Cosmos DB clients are lazily constructed without validation. This results in ContainerProxy.read_item potentially
```

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/data_type_details_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/data_type_details_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/dynamodb_type_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/dynamodb_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/dynamodb_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/dynamodb_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from typing import Any, Dict, List, Optional
 
 import boto3
 import numpy as np
+from botocore.config import Config
 
 DYNAMODB = "dynamodb"
 TABLE = "Table"
 ATTRIBUTE_NAME = "AttributeName"
 ATTRIBUTE_TYPE = "AttributeType"
 KEY_TYPE = "KeyType"
 KEY_SCHEMA = "KeySchema"
@@ -20,14 +21,18 @@
 BATCH_GET_ITEM_LIMIT = 100
 ATTRIBUTES_TO_GET = "AttributesToGet"
 
 PRIMARY_KEY_ATTRIBUTE_NAME_VALUE = "_feature_store_internal__primary_keys"
 PRIMARY_KEY_SCHEMA = {ATTRIBUTE_NAME: PRIMARY_KEY_ATTRIBUTE_NAME_VALUE, KEY_TYPE: HASH}
 TTL_KEY_ATTRIBUTE_NAME_VALUE = "_feature_store_internal__ttl_column"
 
+DEFAULT_CONFIG = Config(
+    retries={"max_attempts": 3, "mode": "standard"}, read_timeout=30
+)
+
 
 def to_dynamodb_primary_key(primary_key_values: List[Any]):
     return {PRIMARY_KEY_ATTRIBUTE_NAME_VALUE: json.dumps(primary_key_values)}
 
 
 def to_range_schema(timestamp_key: str):
     return {ATTRIBUTE_NAME: timestamp_key, KEY_TYPE: RANGE}
@@ -77,14 +82,15 @@
     return boto3.resource(
         DYNAMODB,
         aws_access_key_id=access_key_id,
         aws_secret_access_key=secret_access_key,
         region_name=region,
         aws_session_token=session_token,
         endpoint_url=endpoint_url,
+        config=DEFAULT_CONFIG,
     )
 
 
 def paginate_keys(
     batch_keys: Dict[str, List[Any]],
     batch_size_limit: int,
 ) -> List[Dict[str, List[Any]]]:
```

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/feature_function_type_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/feature_function_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/feature_spec_test_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/feature_spec_test_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/metrics_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/pandas_type_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/pandas_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/sql_type_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/sql_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/uc_utils.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/uc_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/utils_common.py` & `databricks-feature-lookup-0.7.0/databricks/feature_store/utils/utils_common.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/PKG-INFO` & `databricks-feature-lookup-0.7.0/databricks_feature_lookup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-feature-lookup
-Version: 0.6.0
+Version: 0.7.0
 Summary: Databricks Feature Store Feature Lookup Client
 Author: Databricks
 Author-email: feedback@databricks.com
 License: Databricks Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/SOURCES.txt` & `databricks-feature-lookup-0.7.0/databricks_feature_lookup.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 databricks/feature_store/utils/data_type_details_utils.py
 databricks/feature_store/utils/dynamodb_type_utils.py
 databricks/feature_store/utils/dynamodb_utils.py
 databricks/feature_store/utils/feature_function_type_utils.py
 databricks/feature_store/utils/feature_spec_test_utils.py
 databricks/feature_store/utils/metrics_utils.py
 databricks/feature_store/utils/pandas_type_utils.py
-databricks/feature_store/utils/serving_test_utils.py
 databricks/feature_store/utils/sql_type_utils.py
 databricks/feature_store/utils/test_utils_common.py
 databricks/feature_store/utils/uc_utils.py
 databricks/feature_store/utils/utils_common.py
 databricks_feature_lookup.egg-info/PKG-INFO
 databricks_feature_lookup.egg-info/SOURCES.txt
 databricks_feature_lookup.egg-info/dependency_links.txt
```

### Comparing `databricks-feature-lookup-0.6.0/setup.py` & `databricks-feature-lookup-0.7.0/setup.py`

 * *Files identical despite different names*

