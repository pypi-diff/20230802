# Comparing `tmp/google-pso-data-validator-3.2.0.tar.gz` & `tmp/google-pso-data-validator-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-pso-data-validator-3.2.0.tar", last modified: Fri Jun  2 16:20:16 2023, max compression
+gzip compressed data, was "google-pso-data-validator-4.0.0.tar", last modified: Wed Aug  2 18:27:42 2023, max compression
```

## Comparing `google-pso-data-validator-3.2.0.tar` & `google-pso-data-validator-4.0.0.tar`

### file list

```diff
@@ -1,113 +1,100 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.191492 google-pso-data-validator-3.2.0/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    37001 2023-06-02 16:20:16.191492 google-pso-data-validator-3.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    36289 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.143489 google-pso-data-validator-3.2.0/data_validation/
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20968 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1986 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/app.py
--rw-r--r--   0 root         (0) root         (0)    45053 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/cli_tools.py
--rw-r--r--   0 root         (0) root         (0)      881 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/client_info.py
--rw-r--r--   0 root         (0) root         (0)    10409 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/clients.py
--rw-r--r--   0 root         (0) root         (0)    13911 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/combiner.py
--rw-r--r--   0 root         (0) root         (0)    34436 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/config_manager.py
--rw-r--r--   0 root         (0) root         (0)     5052 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/consts.py
--rw-r--r--   0 root         (0) root         (0)    16222 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/data_validation.py
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1269 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/jellyfish_distance.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/metadata.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/partition_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.147489 google-pso-data-validator-3.2.0/data_validation/query_builder/
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/query_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/query_builder/partition_row_builder.py
--rw-r--r--   0 root         (0) root         (0)    18741 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/query_builder/query_builder.py
--rw-r--r--   0 root         (0) root         (0)     7520 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/query_builder/random_row_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.147489 google-pso-data-validator-3.2.0/data_validation/result_handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/result_handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3970 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/result_handlers/bigquery.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/result_handlers/text.py
--rw-r--r--   0 root         (0) root         (0)    11146 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/schema_validation.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/secret_manager.py
--rw-r--r--   0 root         (0) root         (0)     9481 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/state_manager.py
--rw-r--r--   0 root         (0) root         (0)    16109 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/data_validation/validation_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.151489 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/
--rw-r--r--   0 root         (0) root         (0)    37001 2023-06-02 16:20:16.000000 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3610 2023-06-02 16:20:16.000000 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 16:20:16.000000 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-02 16:20:16.000000 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      587 2023-06-02 16:20:16.000000 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-02 16:20:16.000000 google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-02 16:20:16.191492 google-pso-data-validator-3.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2877 2023-06-02 16:18:41.000000 google-pso-data-validator-3.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.123487 google-pso-data-validator-3.2.0/third_party/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.127488 google-pso-data-validator-3.2.0/third_party/ibis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.155490 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/alchemy.py
--rw-r--r--   0 root         (0) root         (0)     1198 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/api.py
--rw-r--r--   0 root         (0) root         (0)     7727 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/client.py
--rw-r--r--   0 root         (0) root         (0)    18668 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.155490 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/expr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/expr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4949 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/expr/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     2373 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/expr/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.159490 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1524 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.159490 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/base_sqlalchemy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/base_sqlalchemy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7579 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/base_sqlalchemy/alchemy.py
--rw-r--r--   0 root         (0) root         (0)     3551 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/datatypes.py
--rw-r--r--   0 root         (0) root         (0)    13566 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.167491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/
--rw-r--r--   0 root         (0) root         (0)        2 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2069 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/api.py
--rw-r--r--   0 root         (0) root         (0)    14574 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/client.py
--rw-r--r--   0 root         (0) root         (0)     1898 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/compiler.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.171491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4944 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)    14058 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)    14908 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/test_compiler.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/test_datatypes.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.171491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_impala/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_impala/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7090 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_impala/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.175491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4042 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/api.py
--rw-r--r--   0 root         (0) root         (0)     9537 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/client.py
--rw-r--r--   0 root         (0) root         (0)    15249 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.175491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/expr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/expr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4032 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/expr/api.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/expr/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.179491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2135 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/alchemy.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/api.py
--rw-r--r--   0 root         (0) root         (0)     9908 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/client.py
--rw-r--r--   0 root         (0) root         (0)    17172 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.179491 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/expr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/expr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/expr/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/expr/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.183492 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/udf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/udf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6995 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/udf/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.183492 google-pso-data-validator-3.2.0/third_party/ibis/ibis_postgres/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_postgres/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.187492 google-pso-data-validator-3.2.0/third_party/ibis/ibis_redshift/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_redshift/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10245 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_redshift/client.py
--rw-r--r--   0 root         (0) root         (0)      660 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_redshift/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 16:20:16.187492 google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/api.py
--rw-r--r--   0 root         (0) root         (0)     9302 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/client.py
--rw-r--r--   0 root         (0) root         (0)    26138 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/compiler.py
--rw-r--r--   0 root         (0) root         (0)     4830 2023-06-02 16:18:42.000000 google-pso-data-validator-3.2.0/third_party/ibis/ibis_teradata/datatypes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.511742 google-pso-data-validator-4.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    38445 2023-08-02 18:27:42.511742 google-pso-data-validator-4.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    37732 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.475739 google-pso-data-validator-4.0.0/data_validation/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21056 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/app.py
+-rw-r--r--   0 root         (0) root         (0)    45493 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/cli_tools.py
+-rw-r--r--   0 root         (0) root         (0)      881 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/client_info.py
+-rw-r--r--   0 root         (0) root         (0)     9475 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/clients.py
+-rw-r--r--   0 root         (0) root         (0)    13412 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/combiner.py
+-rw-r--r--   0 root         (0) root         (0)    37509 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/config_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/consts.py
+-rw-r--r--   0 root         (0) root         (0)    14684 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/data_validation.py
+-rw-r--r--   0 root         (0) root         (0)      687 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/jellyfish_distance.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/metadata.py
+-rw-r--r--   0 root         (0) root         (0)    13862 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/partition_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.475739 google-pso-data-validator-4.0.0/data_validation/query_builder/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/query_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/query_builder/partition_row_builder.py
+-rw-r--r--   0 root         (0) root         (0)    18793 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/query_builder/query_builder.py
+-rw-r--r--   0 root         (0) root         (0)     3680 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/query_builder/random_row_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.479740 google-pso-data-validator-4.0.0/data_validation/result_handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/result_handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3970 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/result_handlers/bigquery.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/result_handlers/text.py
+-rw-r--r--   0 root         (0) root         (0)    14245 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/schema_validation.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/secret_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9694 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/state_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16109 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/data_validation/validation_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.483740 google-pso-data-validator-4.0.0/google_pso_data_validator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    38445 2023-08-02 18:27:42.000000 google-pso-data-validator-4.0.0/google_pso_data_validator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3105 2023-08-02 18:27:42.000000 google-pso-data-validator-4.0.0/google_pso_data_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 18:27:42.000000 google-pso-data-validator-4.0.0/google_pso_data_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-08-02 18:27:42.000000 google-pso-data-validator-4.0.0/google_pso_data_validator.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      586 2023-08-02 18:27:42.000000 google-pso-data-validator-4.0.0/google_pso_data_validator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-02 18:27:42.000000 google-pso-data-validator-4.0.0/google_pso_data_validator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-08-02 18:27:42.511742 google-pso-data-validator-4.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2877 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.455738 google-pso-data-validator-4.0.0/third_party/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.459738 google-pso-data-validator-4.0.0/third_party/ibis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.483740 google-pso-data-validator-4.0.0/third_party/ibis/ibis_addon/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_addon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_addon/api.py
+-rw-r--r--   0 root         (0) root         (0)    14001 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_addon/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.491740 google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/
+-rw-r--r--   0 root         (0) root         (0)     6854 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/api.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/client.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.491740 google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/tests/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4999 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.495741 google-pso-data-validator-4.0.0/third_party/ibis/ibis_db2/
+-rw-r--r--   0 root         (0) root         (0)     2676 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_db2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_db2/api.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_db2/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_db2/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)    16002 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_db2/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.499741 google-pso-data-validator-4.0.0/third_party/ibis/ibis_impala/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_impala/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7181 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_impala/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.499741 google-pso-data-validator-4.0.0/third_party/ibis/ibis_mssql/
+-rw-r--r--   0 root         (0) root         (0)     2835 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_mssql/api.py
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_mssql/datatypes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.499741 google-pso-data-validator-4.0.0/third_party/ibis/ibis_mysql/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.503741 google-pso-data-validator-4.0.0/third_party/ibis/ibis_mysql/base_sql_compiler/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_mysql/base_sql_compiler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_mysql/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.503741 google-pso-data-validator-4.0.0/third_party/ibis/ibis_oracle/
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_oracle/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_oracle/api.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_oracle/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     5939 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_oracle/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)    14055 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_oracle/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.503741 google-pso-data-validator-4.0.0/third_party/ibis/ibis_postgres/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_postgres/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.507741 google-pso-data-validator-4.0.0/third_party/ibis/ibis_redshift/
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_redshift/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_redshift/api.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_redshift/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.507741 google-pso-data-validator-4.0.0/third_party/ibis/ibis_snowflake/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_snowflake/api.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_snowflake/datatypes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:27:42.511742 google-pso-data-validator-4.0.0/third_party/ibis/ibis_teradata/
+-rw-r--r--   0 root         (0) root         (0)     7684 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_teradata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_teradata/api.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_teradata/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     6283 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_teradata/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     7528 2023-08-02 18:25:55.000000 google-pso-data-validator-4.0.0/third_party/ibis/ibis_teradata/registry.py
```

### Comparing `google-pso-data-validator-3.2.0/LICENSE` & `google-pso-data-validator-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.2.0/PKG-INFO` & `google-pso-data-validator-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: google-pso-data-validator
-Version: 3.2.0
+Version: 4.0.0
 Summary: A package to enable easy data validation
 Home-page: https://github.com/pypa/sampleproject
 Author: Dylan Hercher
 Author-email: dhercher@google.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: apache-airflow
 Provides-Extra: pyspark
 License-File: LICENSE
 
 # Data Validation Tool
 
@@ -30,40 +30,41 @@
 compared to ensure they are matched and correct after each migration step
 (e.g. data and schema migration, SQL script translation, ETL migration, etc.).
 The Data Validation Tool (DVT) provides an automated and repeatable solution to
 perform this task.
 
 DVT supports the following validations:
 * Column validation (count, sum, avg, min, max, group by)
-* Row validation (BQ, Hive, Teradata, Oracle, SQL Server, Postgres, Mysql only)
-* Schema validation 
+* Row validation (Not supported for FileSystem connections)
+* Schema validation
 * Custom Query validation
 * Ad hoc SQL exploration
 
 DVT supports the following connection types:
 
+*   [AlloyDB](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#alloydb)
 *   [BigQuery](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#google-bigquery)
 *   [DB2](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#db2)
 *   [FileSystem](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#filesystem)
 *   [Hive](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#hive)
 *   [Impala](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#impala)
 *   [MSSQL](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#mssql-server)
 *   [MySQL](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#mysql)
 *   [Oracle](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#oracle)
 *   [Postgres](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#postgres)
 *   [Redshift](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#redshift)
 *   [Spanner](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#google-spanner)
 *   [Teradata](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#teradata)
-*   [AlloyDB](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#alloydb)
+*   [Snowflake](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#snowflake)
 
 The [Connections](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md) page provides details about how to create
 and list connections for the validation tool.
 
 ### Disclaimer
-This is not an officially supported Google product. Please be aware that bugs may lurk, and that we reserve the right to make small backwards-incompatible changes. Feel free to open bugs or feature requests, or contribute directly 
+This is not an officially supported Google product. Please be aware that bugs may lurk, and that we reserve the right to make small backwards-incompatible changes. Feel free to open bugs or feature requests, or contribute directly
 (see [CONTRIBUTING.md](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/CONTRIBUTING.md) for details).
 
 ## Installation
 
 The [Installation](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/installation.md) page describes the prerequisites and
 setup steps needed to install and use the Data Validation Tool.
 
@@ -94,15 +95,15 @@
 
 #### Column Validations
 
 Below is the command syntax for column validations. To run a grouped column
 validation, simply specify the `--grouped-columns` flag.
 
 You can specify a list of string columns for aggregations in order to calculate
-an aggregation over the `length(string_col)`. Running an aggregation 
+an aggregation over the `length(string_col)`. Running an aggregation
 over all columns ('*') will only run over numeric columns, unless the
 `--wildcard-include-string-len` flag is present.
 
 ```
 data-validation (--verbose or -v) (--log-level or -ll) validate column
   --source-conn or -sc SOURCE_CONN
                         Source connection details
@@ -114,15 +115,15 @@
                         Comma separated list of tables in the form schema.table=target_schema.target_table
                         Target schema name and table name are optional.
                         i.e 'bigquery-public-data.new_york_citibike.citibike_trips'
   [--grouped-columns or -gc GROUPED_COLUMNS]
                         Comma separated list of columns for Group By i.e col_a,col_b
   [--primary-keys or -pk PRIMARY_KEYS]
                         Comma separated list of columns to use as primary keys
-                        (Note) Only use with grouped column validation
+                        (Note) Only use with grouped column validation. See *Primary Keys* section. 
   [--count COLUMNS]     Comma separated list of columns for count or * for all columns
   [--sum COLUMNS]       Comma separated list of columns for sum or * for all numeric
   [--min COLUMNS]       Comma separated list of columns for min or * for all numeric
   [--max COLUMNS]       Comma separated list of columns for max or * for all numeric
   [--avg COLUMNS]       Comma separated list of columns for avg or * for all numeric
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
@@ -152,23 +153,23 @@
 The default aggregation type is a 'COUNT *'. If no aggregation flag (i.e count,
 sum , min, etc.) is provided, the default aggregation will run.
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md) page provides many examples of how a tool can be used to run powerful validations without writing any queries.
 
 #### Row Validations
 
-(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Redshift, Postgres, Mysql, Db2 and Alloy DB. Struct and array data types are not currently supported.
-In addition, please note that SHA256 is not a supported function on Teradata systems. 
-If you wish to perform this comparison on Teradata you will need to 
+(Note: Row hash validation not supported for FileSystem connections. 
+In addition, please note that SHA256 is not a supported function on Teradata systems.
+If you wish to perform this comparison on Teradata you will need to
 [deploy a UDF to perform the conversion](https://github.com/akuroda/teradata-udf-sha2/blob/master/src/sha256.c).)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass a `--primary-key` flag which defines what field(s)
 the validation will be compared on, as well as either the `--comparison-fields` flag
-or the `--hash` flag.
+or the `--hash` flag. See *Primary Keys* section
 
 The `--comparison-fields` flag specifies the values (e.g. columns) whose raw values will be compared
 based on the primary key join. The `--hash` flag will run a checksum across specified columns in
 the table. This will include casting to string, sanitizing the data (ifnull, rtrim, upper), concatenating,
 and finally hashing the row.
 
 
@@ -185,19 +186,19 @@
                         Target connection details
                         See: *Connections* section for each data source
   --tables-list or -tbls SOURCE_SCHEMA.SOURCE_TABLE=TARGET_SCHEMA.TARGET_TABLE
                         Comma separated list of tables in the form schema.table=target_schema.target_table
                         Target schema name and table name are optional.
                         i.e 'bigquery-public-data.new_york_citibike.citibike_trips'
   --primary-keys or -pk PRIMARY_KEYS
-                        Comma separated list of columns to use as primary keys
+                        Comma separated list of columns to use as primary keys.  See *Primary Keys* section
   --comparison-fields or -comp-fields FIELDS
                         Comma separated list of columns to compare. Can either be a physical column or an alias
                         See: *Calculated Fields* section for details
-  --hash COLUMNS        Comma separated list of columns to hash or * for all columns 
+  --hash COLUMNS        Comma separated list of columns to hash or * for all columns
   --concat COLUMNS      Comma separated list of columns to concatenate or * for all columns (use if a common hash function is not available between databases)
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--filters SOURCE_FILTER:TARGET_FILTER]
@@ -215,21 +216,21 @@
   [--random-row-batch-size or -rbs]
                         Row batch size used for random row filters (default 10,000).
   [--filter-status or -fs STATUSES_LIST]
                         Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail). If no list is provided, all statuses are returned.
 ```
 #### Generate Table Partitions for Large Table Row Validations
 
-Below is the command syntax for generating table partitions in order to perform row validations on large tables with memory constraints. 
+(Note: This is only supported for Oracle and Postgres connections.)
 
-The command generates and stores multiple YAML configs that represent chunks of the large table using filters (`WHERE partition_key > X AND partition_key < Y`). You can then run the configs in the directory serially with the `data-validation configs run --config-dir PATH` command as described [here](https://github.com/GoogleCloudPlatform/professional-services-data-validator#yaml-configuration-files).
+When performing row validations, Data Validation Tool brings each row into memory and can run into MemoryError. Below is the command syntax for generating table partitions in order to perform row validations on large tables to alleviate MemoryError. Each partition contains a range of primary key(s) and the ranges of keys across partitions are distinct. The partitions have nearly equal number of rows. See *Primary Keys* section
 
-The command takes the same parameters as required for `Row Validation` *plus* few commands to implement the partitioning logic.
+The command generates and stores multiple YAML configs that represent chunks of the large table using filters (`WHERE primary_key(s) >= X AND primary_key(s) < Y`). You can then run the configs in the directory serially (or in parallel in multiple containers, VMs) with the `data-validation configs run --config-dir PATH` command as described [here](https://github.com/GoogleCloudPlatform/professional-services-data-validator#yaml-configuration-files).
 
-(Note: As of now, only monotonically increasing key is supported for `--partition-key`.)
+The command takes the same parameters as required for `Row Validation` *plus* a few parameters to support partitioning. Single and multiple primary keys are supported and keys can be of any indexable type. A parameter used in earlier versions, ```partition-key``` is no longer supported. 
 
 ```
 data-validation (--verbose or -v) (--log-level or -ll) generate-table-partitions
 
   --source-conn or -sc SOURCE_CONN
                         Source connection details
                         See: *Data Source Configurations* section for each data source
@@ -237,67 +238,71 @@
                         Target connection details
                         See: *Connections* section for each data source
   --tables-list or -tbls SOURCE_SCHEMA.SOURCE_TABLE=TARGET_SCHEMA.TARGET_TABLE
                         Comma separated list of tables in the form schema.table=target_schema.target_table
                         Target schema name and table name are optional.
                         i.e 'bigquery-public-data.new_york_citibike.citibike_trips'
   --primary-keys PRIMARY_KEYS, -pk PRIMARY_KEYS
-                        Comma separated list of primary key columns 'col_a,col_b'
+                        Comma separated list of primary key columns 'col_a,col_b'.  See *Primary Keys* section
   --comparison-fields or -comp-fields FIELDS
                         Comma separated list of columns to compare. Can either be a physical column or an alias
                         See: *Calculated Fields* section for details
-  --hash COLUMNS        Comma separated list of columns to hash or * for all columns 
+  --hash COLUMNS        Comma separated list of columns to hash or * for all columns
   --concat COLUMNS      Comma separated list of columns to concatenate or * for all columns (use if a common hash function is not available between databases)
   --config-dir CONFIG_DIR, -cdir CONFIG_DIR
                         Directory Path to store YAML Config Files
                         GCS: Provide a full gs:// path of the target directory. Eg: `gs://<BUCKET>/partitions_dir`
                         Local: Provide a relative path of the target directory. Eg: `partitions_dir`
   --partition-num [1-1000], -pn [1-1000]
                         Number of partitions/config files to generate
                         In case this value exceeds the row count of the source/target table, it will be decreased to max(source_row_count, target_row_count)
-  [--partition-key PARTITION_KEY, -partkey PARTITION_KEY]
-                        Column on which the partitions would be generated. Column type must be integer. Defaults to Primary key
   [--filters SOURCE_FILTER:TARGET_FILTER]
                         Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
 ```
 #### Schema Validations
 
 Below is the syntax for schema validations. These can be used to compare case insensitive column names and
 types between source and target.
 
+Note: An exclamation point before a data type (`!string`) signifies the column is non-nullable or required.
+
 ```
 data-validation (--verbose or -v) (--log-level or -ll) validate schema
   --source-conn or -sc SOURCE_CONN
                         Source connection details
                         See: *Data Source Configurations* section for each data source
   --target-conn or -tc TARGET_CONN
                         Target connection details
                         See: *Connections* section for each data source
   --tables-list or -tbls SOURCE_SCHEMA.SOURCE_TABLE=TARGET_SCHEMA.TARGET_TABLE
                         Comma separated list of tables in the form schema.table=target_schema.target_table
                         Target schema name and table name are optional.
-                        i.e 'bigquery-public-data.new_york_citibike.citibike_trips'
+                        e.g.: 'bigquery-public-data.new_york_citibike.citibike_trips'
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--config-file or -c CONFIG_FILE]
                         YAML Config File Path to be used for storing validations.
   [--format or -fmt]    Format for stdout output. Supported formats are (text, csv, json, table).
                         Defaults  to table.
   [--filter-status or -fs STATUSES_LIST]
-                        Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail). If no list is provided, all statuses are returned.
+                        Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail).
+                        If no list is provided, all statuses are returned.
   [--exclusion-columns or -ec EXCLUSION_COLUMNS]
-                        Comma separated list of columns to be excluded from the schema validation, i.e col_a,col_b.
-
+                        Comma separated list of columns to be excluded from the schema validation, e.g.: col_a,col_b.
   [--allow-list or -al ALLOW_LIST]
-                        Comma separated list of data-type mappings of source and destination data sources which will be validated in case of missing data types in destination data source. e.g: "decimal(4,2):decimal(5,4),string[non-nullable]:string"                 
+                        Comma separated list of data-type mappings of source and destination data sources which will be validated in case of missing data types in destination data source. e.g: "decimal(4,2):decimal(5,4),!string:string"
+  [--allow-list-file ALLOW_LIST_FILE, -alf ALLOW_LIST_FILE]
+                        YAML file containing default --allow-list mappings. Can be used in conjunction with --allow-list.
+                        e.g.: samples/allow_list/oracle_to_bigquery.yaml or gs://dvt-allow-list-files/oracle_to_bigquery.yaml
+                        See example files in samples/allow_list/.
 ```
 
 #### Custom Query Column Validations
 
 Below is the command syntax for custom query column validations.
 
 ```
@@ -339,22 +344,22 @@
 The default aggregation type is a 'COUNT *'. If no aggregation flag (i.e count,
 sum , min, etc.) is provided, the default aggregation will run.
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md)
 page provides few examples of how this tool can be used to run custom query validations.
 
 
-#### Custom Query Row Validations 
+#### Custom Query Row Validations
 
-(Note: Custom query row validation is currently only supported for BigQuery, Teradata, SQL Server, PostgreSQL, Oracle, Redshift, DB2, AlloyDB, and Impala/Hive. Struct and array data types are not currently supported.)
+(Note: Custom query row validation is not supported for FileSystem connections. Struct and array data types are not currently supported.)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass `--hash` flag which will specify the fields
 of the custom query result that will be concatenated and hashed. The primary key should be included
-in the SELECT statement of both source_query.sql and target_query.sql
+in the SELECT statement of both source_query.sql and target_query.sql.  See *Primary Keys* section
 
 Below is the command syntax for custom query row validations.
 
 ```
 data-validation (--verbose or -v) (--log-level or -ll) validate custom-query row
   --source-conn or -sc SOURCE_CONN
                         Source connection details
@@ -425,18 +430,18 @@
 
 You can customize the configuration for any given validation by providing use
 case specific CLI arguments or editing the YAML configuration file.
 
 For example, the following command creates a YAML file for the validation of the
 `new_york_citibike` table: `data-validation validate column -sc my_bq_conn -tc
 my_bq_conn -tbls bigquery-public-data.new_york_citibike.citibike_trips -c
-citibike.yaml`. 
+citibike.yaml`.
 
 The vaildation config file is saved to the GCS path specified by the `PSO_DV_CONFIG_HOME`
-env variable if that has been set; otherwise, it is saved to wherever the tool is run. 
+env variable if that has been set; otherwise, it is saved to wherever the tool is run.
 
 You can now edit the YAML file if, for example, the `new_york_citibike` table is
 stored in datasets that have different names in the source and target systems.
 Once the file is updated and saved, the following command runs the
 validation:
 
 ```
@@ -451,21 +456,21 @@
 
 data-validation configs run -cdir gs://my-bucket/my-validations/
 ```
 
 View the complete YAML file for a Grouped Column validation on the
 [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-yaml-config-grouped-column-validation) page.
 
-You can view a list of all saved validation YAML files using `data-validation configs list`, and print a YAML config using `data-validation configs get -c citibike.yaml`. 
+You can view a list of all saved validation YAML files using `data-validation configs list`, and print a YAML config using `data-validation configs get -c citibike.yaml`.
 
 ### Validation Reports
 
 The result handlers tell DVT where to store the results of
 each validation. The tool can write the results of a validation run to Google
-BigQuery or print to stdout (default). View the schema of the results 
+BigQuery or print to stdout (default). View the schema of the results
 table [here](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/terraform/results_schema.json).
 
 To output to BigQuery, simply include the `-bqrh` flag during a validation run
 like so:
 ```
 data-validation validate column
   -sc bq_conn
@@ -563,14 +568,20 @@
 written in the syntax of the given source.
 
 Note that you are writing the query to execute, which does not have to match
 between source and target as long as the results can be expected to align. If
 the target filter is omitted, the source filter will run on both the source and
 target tables.
 
+### Primary Keys
+
+In many cases, validations (e.g. count, min, max etc) produce one row per table. The comparison between the source
+and target table is to compare the value for each column in the source with the value of the column in the target.
+`grouped-columns` validation and `validate row` produce multiple rows per table. Data Validation Tool needs one or more columns to uniquely identify each row so the source and target can be compared. Data Validation Tool refers to these columns as primary keys. These do not need to be primary keys in the table. The only requirement is that the keys uniquely identify the row in the results.
+
 ### Grouped Columns
 
 Grouped Columns contain the fields you want your aggregations to be broken out
 by, e.g. `SELECT last_updated::DATE, COUNT(*) FROM my.table` will produce a
 resultset that breaks down the count of rows per calendar date.
 
 ### Hash, Concat, and Comparison Fields
@@ -639,43 +650,43 @@
   FROM my.table
   ) as table_0
 ```
 
 If you generate the config file for a row validation, you can see that it uses
 calculated fields to generate the query. You can also use calculated fields
 in column level validations to generate the length of a string, or cast
-a INT field to BIGINT for aggregations. 
+a INT field to BIGINT for aggregations.
 
 See the [Examples page](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-yaml-with-calc-fields-cast-to-numeric-before-aggregation) for a sample
 cast to NUMERIC.
 
 #### Custom Calculated Fields
 
 DVT supports certain functions required for row hash validation natively (i.e. CAST() and CONCAT()),
 which are listed in the CalculatedField() class methods in the [QueryBuilder](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/data_validation/query_builder/query_builder.py).
 
 You can also specify custom functions (i.e. replace() or truncate()) from the Ibis expression
-[API reference](https://ibis-project.org/docs/3.2.0/api/expressions/). Keep in mind these will run
+[API reference](https://ibis-project.org/reference/expressions/generic/). Keep in mind these will run
 on both source and target systems. You will need to specify the Ibis API expression and the parameters
 required, if any, with the 'params' block as shown below:
 
 ```yaml
 - calculated_fields:
   - depth: 0
     field_alias: format_start_time
     source_calculated_columns:
     - start_time
     target_calculated_columns:
     - start_time
     type: custom
-    ibis_expr: ibis.expr.api.TimestampValue.strftime
+    ibis_expr: ibis.expr.types.TemporalValue.strftime
     params:
     - format_str: '%m%d%Y'
 ```
 
-The above block references the [TimestampValue.strftime](https://ibis-project.org/docs/3.2.0/api/expressions/timestamps/#ibis.expr.types.temporal.TemporalValue.strftime) Ibis API expression.
+The above block references the [TemporalValue.strftime](https://ibis-project.org/reference/expressions/timestamps/#ibis.expr.types.temporal.TemporalValue.strftime) Ibis API expression.
 See the [Examples page](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-row-validation-yaml-with-custom-calc-field)
 for a sample YAML with a custom calculated field.
 
 ## Contributing
 
 Contributions are welcome. See the [Contributing guide](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/CONTRIBUTING.md) for details.
```

### Comparing `google-pso-data-validator-3.2.0/README.md` & `google-pso-data-validator-4.0.0/google_pso_data_validator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: google-pso-data-validator
+Version: 4.0.0
+Summary: A package to enable easy data validation
+Home-page: https://github.com/pypa/sampleproject
+Author: Dylan Hercher
+Author-email: dhercher@google.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: apache-airflow
+Provides-Extra: pyspark
+License-File: LICENSE
+
 # Data Validation Tool
 
 The Data Validation Tool is an open sourced Python CLI tool based on the
 [Ibis framework](https://ibis-project.org/docs/)
 that compares heterogeneous data source tables with multi-leveled validation
 functions.
 
@@ -10,40 +30,41 @@
 compared to ensure they are matched and correct after each migration step
 (e.g. data and schema migration, SQL script translation, ETL migration, etc.).
 The Data Validation Tool (DVT) provides an automated and repeatable solution to
 perform this task.
 
 DVT supports the following validations:
 * Column validation (count, sum, avg, min, max, group by)
-* Row validation (BQ, Hive, Teradata, Oracle, SQL Server, Postgres, Mysql only)
-* Schema validation 
+* Row validation (Not supported for FileSystem connections)
+* Schema validation
 * Custom Query validation
 * Ad hoc SQL exploration
 
 DVT supports the following connection types:
 
+*   [AlloyDB](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#alloydb)
 *   [BigQuery](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#google-bigquery)
 *   [DB2](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#db2)
 *   [FileSystem](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#filesystem)
 *   [Hive](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#hive)
 *   [Impala](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#impala)
 *   [MSSQL](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#mssql-server)
 *   [MySQL](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#mysql)
 *   [Oracle](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#oracle)
 *   [Postgres](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#postgres)
 *   [Redshift](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#redshift)
 *   [Spanner](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#google-spanner)
 *   [Teradata](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#teradata)
-*   [AlloyDB](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#alloydb)
+*   [Snowflake](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#snowflake)
 
 The [Connections](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md) page provides details about how to create
 and list connections for the validation tool.
 
 ### Disclaimer
-This is not an officially supported Google product. Please be aware that bugs may lurk, and that we reserve the right to make small backwards-incompatible changes. Feel free to open bugs or feature requests, or contribute directly 
+This is not an officially supported Google product. Please be aware that bugs may lurk, and that we reserve the right to make small backwards-incompatible changes. Feel free to open bugs or feature requests, or contribute directly
 (see [CONTRIBUTING.md](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/CONTRIBUTING.md) for details).
 
 ## Installation
 
 The [Installation](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/installation.md) page describes the prerequisites and
 setup steps needed to install and use the Data Validation Tool.
 
@@ -74,15 +95,15 @@
 
 #### Column Validations
 
 Below is the command syntax for column validations. To run a grouped column
 validation, simply specify the `--grouped-columns` flag.
 
 You can specify a list of string columns for aggregations in order to calculate
-an aggregation over the `length(string_col)`. Running an aggregation 
+an aggregation over the `length(string_col)`. Running an aggregation
 over all columns ('*') will only run over numeric columns, unless the
 `--wildcard-include-string-len` flag is present.
 
 ```
 data-validation (--verbose or -v) (--log-level or -ll) validate column
   --source-conn or -sc SOURCE_CONN
                         Source connection details
@@ -94,15 +115,15 @@
                         Comma separated list of tables in the form schema.table=target_schema.target_table
                         Target schema name and table name are optional.
                         i.e 'bigquery-public-data.new_york_citibike.citibike_trips'
   [--grouped-columns or -gc GROUPED_COLUMNS]
                         Comma separated list of columns for Group By i.e col_a,col_b
   [--primary-keys or -pk PRIMARY_KEYS]
                         Comma separated list of columns to use as primary keys
-                        (Note) Only use with grouped column validation
+                        (Note) Only use with grouped column validation. See *Primary Keys* section. 
   [--count COLUMNS]     Comma separated list of columns for count or * for all columns
   [--sum COLUMNS]       Comma separated list of columns for sum or * for all numeric
   [--min COLUMNS]       Comma separated list of columns for min or * for all numeric
   [--max COLUMNS]       Comma separated list of columns for max or * for all numeric
   [--avg COLUMNS]       Comma separated list of columns for avg or * for all numeric
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
@@ -132,23 +153,23 @@
 The default aggregation type is a 'COUNT *'. If no aggregation flag (i.e count,
 sum , min, etc.) is provided, the default aggregation will run.
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md) page provides many examples of how a tool can be used to run powerful validations without writing any queries.
 
 #### Row Validations
 
-(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Redshift, Postgres, Mysql, Db2 and Alloy DB. Struct and array data types are not currently supported.
-In addition, please note that SHA256 is not a supported function on Teradata systems. 
-If you wish to perform this comparison on Teradata you will need to 
+(Note: Row hash validation not supported for FileSystem connections. 
+In addition, please note that SHA256 is not a supported function on Teradata systems.
+If you wish to perform this comparison on Teradata you will need to
 [deploy a UDF to perform the conversion](https://github.com/akuroda/teradata-udf-sha2/blob/master/src/sha256.c).)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass a `--primary-key` flag which defines what field(s)
 the validation will be compared on, as well as either the `--comparison-fields` flag
-or the `--hash` flag.
+or the `--hash` flag. See *Primary Keys* section
 
 The `--comparison-fields` flag specifies the values (e.g. columns) whose raw values will be compared
 based on the primary key join. The `--hash` flag will run a checksum across specified columns in
 the table. This will include casting to string, sanitizing the data (ifnull, rtrim, upper), concatenating,
 and finally hashing the row.
 
 
@@ -165,19 +186,19 @@
                         Target connection details
                         See: *Connections* section for each data source
   --tables-list or -tbls SOURCE_SCHEMA.SOURCE_TABLE=TARGET_SCHEMA.TARGET_TABLE
                         Comma separated list of tables in the form schema.table=target_schema.target_table
                         Target schema name and table name are optional.
                         i.e 'bigquery-public-data.new_york_citibike.citibike_trips'
   --primary-keys or -pk PRIMARY_KEYS
-                        Comma separated list of columns to use as primary keys
+                        Comma separated list of columns to use as primary keys.  See *Primary Keys* section
   --comparison-fields or -comp-fields FIELDS
                         Comma separated list of columns to compare. Can either be a physical column or an alias
                         See: *Calculated Fields* section for details
-  --hash COLUMNS        Comma separated list of columns to hash or * for all columns 
+  --hash COLUMNS        Comma separated list of columns to hash or * for all columns
   --concat COLUMNS      Comma separated list of columns to concatenate or * for all columns (use if a common hash function is not available between databases)
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--filters SOURCE_FILTER:TARGET_FILTER]
@@ -195,21 +216,21 @@
   [--random-row-batch-size or -rbs]
                         Row batch size used for random row filters (default 10,000).
   [--filter-status or -fs STATUSES_LIST]
                         Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail). If no list is provided, all statuses are returned.
 ```
 #### Generate Table Partitions for Large Table Row Validations
 
-Below is the command syntax for generating table partitions in order to perform row validations on large tables with memory constraints. 
+(Note: This is only supported for Oracle and Postgres connections.)
 
-The command generates and stores multiple YAML configs that represent chunks of the large table using filters (`WHERE partition_key > X AND partition_key < Y`). You can then run the configs in the directory serially with the `data-validation configs run --config-dir PATH` command as described [here](https://github.com/GoogleCloudPlatform/professional-services-data-validator#yaml-configuration-files).
+When performing row validations, Data Validation Tool brings each row into memory and can run into MemoryError. Below is the command syntax for generating table partitions in order to perform row validations on large tables to alleviate MemoryError. Each partition contains a range of primary key(s) and the ranges of keys across partitions are distinct. The partitions have nearly equal number of rows. See *Primary Keys* section
 
-The command takes the same parameters as required for `Row Validation` *plus* few commands to implement the partitioning logic.
+The command generates and stores multiple YAML configs that represent chunks of the large table using filters (`WHERE primary_key(s) >= X AND primary_key(s) < Y`). You can then run the configs in the directory serially (or in parallel in multiple containers, VMs) with the `data-validation configs run --config-dir PATH` command as described [here](https://github.com/GoogleCloudPlatform/professional-services-data-validator#yaml-configuration-files).
 
-(Note: As of now, only monotonically increasing key is supported for `--partition-key`.)
+The command takes the same parameters as required for `Row Validation` *plus* a few parameters to support partitioning. Single and multiple primary keys are supported and keys can be of any indexable type. A parameter used in earlier versions, ```partition-key``` is no longer supported. 
 
 ```
 data-validation (--verbose or -v) (--log-level or -ll) generate-table-partitions
 
   --source-conn or -sc SOURCE_CONN
                         Source connection details
                         See: *Data Source Configurations* section for each data source
@@ -217,67 +238,71 @@
                         Target connection details
                         See: *Connections* section for each data source
   --tables-list or -tbls SOURCE_SCHEMA.SOURCE_TABLE=TARGET_SCHEMA.TARGET_TABLE
                         Comma separated list of tables in the form schema.table=target_schema.target_table
                         Target schema name and table name are optional.
                         i.e 'bigquery-public-data.new_york_citibike.citibike_trips'
   --primary-keys PRIMARY_KEYS, -pk PRIMARY_KEYS
-                        Comma separated list of primary key columns 'col_a,col_b'
+                        Comma separated list of primary key columns 'col_a,col_b'.  See *Primary Keys* section
   --comparison-fields or -comp-fields FIELDS
                         Comma separated list of columns to compare. Can either be a physical column or an alias
                         See: *Calculated Fields* section for details
-  --hash COLUMNS        Comma separated list of columns to hash or * for all columns 
+  --hash COLUMNS        Comma separated list of columns to hash or * for all columns
   --concat COLUMNS      Comma separated list of columns to concatenate or * for all columns (use if a common hash function is not available between databases)
   --config-dir CONFIG_DIR, -cdir CONFIG_DIR
                         Directory Path to store YAML Config Files
                         GCS: Provide a full gs:// path of the target directory. Eg: `gs://<BUCKET>/partitions_dir`
                         Local: Provide a relative path of the target directory. Eg: `partitions_dir`
   --partition-num [1-1000], -pn [1-1000]
                         Number of partitions/config files to generate
                         In case this value exceeds the row count of the source/target table, it will be decreased to max(source_row_count, target_row_count)
-  [--partition-key PARTITION_KEY, -partkey PARTITION_KEY]
-                        Column on which the partitions would be generated. Column type must be integer. Defaults to Primary key
   [--filters SOURCE_FILTER:TARGET_FILTER]
                         Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
 ```
 #### Schema Validations
 
 Below is the syntax for schema validations. These can be used to compare case insensitive column names and
 types between source and target.
 
+Note: An exclamation point before a data type (`!string`) signifies the column is non-nullable or required.
+
 ```
 data-validation (--verbose or -v) (--log-level or -ll) validate schema
   --source-conn or -sc SOURCE_CONN
                         Source connection details
                         See: *Data Source Configurations* section for each data source
   --target-conn or -tc TARGET_CONN
                         Target connection details
                         See: *Connections* section for each data source
   --tables-list or -tbls SOURCE_SCHEMA.SOURCE_TABLE=TARGET_SCHEMA.TARGET_TABLE
                         Comma separated list of tables in the form schema.table=target_schema.target_table
                         Target schema name and table name are optional.
-                        i.e 'bigquery-public-data.new_york_citibike.citibike_trips'
+                        e.g.: 'bigquery-public-data.new_york_citibike.citibike_trips'
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--config-file or -c CONFIG_FILE]
                         YAML Config File Path to be used for storing validations.
   [--format or -fmt]    Format for stdout output. Supported formats are (text, csv, json, table).
                         Defaults  to table.
   [--filter-status or -fs STATUSES_LIST]
-                        Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail). If no list is provided, all statuses are returned.
+                        Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail).
+                        If no list is provided, all statuses are returned.
   [--exclusion-columns or -ec EXCLUSION_COLUMNS]
-                        Comma separated list of columns to be excluded from the schema validation, i.e col_a,col_b.
-
+                        Comma separated list of columns to be excluded from the schema validation, e.g.: col_a,col_b.
   [--allow-list or -al ALLOW_LIST]
-                        Comma separated list of data-type mappings of source and destination data sources which will be validated in case of missing data types in destination data source. e.g: "decimal(4,2):decimal(5,4),string[non-nullable]:string"                 
+                        Comma separated list of data-type mappings of source and destination data sources which will be validated in case of missing data types in destination data source. e.g: "decimal(4,2):decimal(5,4),!string:string"
+  [--allow-list-file ALLOW_LIST_FILE, -alf ALLOW_LIST_FILE]
+                        YAML file containing default --allow-list mappings. Can be used in conjunction with --allow-list.
+                        e.g.: samples/allow_list/oracle_to_bigquery.yaml or gs://dvt-allow-list-files/oracle_to_bigquery.yaml
+                        See example files in samples/allow_list/.
 ```
 
 #### Custom Query Column Validations
 
 Below is the command syntax for custom query column validations.
 
 ```
@@ -319,22 +344,22 @@
 The default aggregation type is a 'COUNT *'. If no aggregation flag (i.e count,
 sum , min, etc.) is provided, the default aggregation will run.
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md)
 page provides few examples of how this tool can be used to run custom query validations.
 
 
-#### Custom Query Row Validations 
+#### Custom Query Row Validations
 
-(Note: Custom query row validation is currently only supported for BigQuery, Teradata, SQL Server, PostgreSQL, Oracle, Redshift, DB2, AlloyDB, and Impala/Hive. Struct and array data types are not currently supported.)
+(Note: Custom query row validation is not supported for FileSystem connections. Struct and array data types are not currently supported.)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass `--hash` flag which will specify the fields
 of the custom query result that will be concatenated and hashed. The primary key should be included
-in the SELECT statement of both source_query.sql and target_query.sql
+in the SELECT statement of both source_query.sql and target_query.sql.  See *Primary Keys* section
 
 Below is the command syntax for custom query row validations.
 
 ```
 data-validation (--verbose or -v) (--log-level or -ll) validate custom-query row
   --source-conn or -sc SOURCE_CONN
                         Source connection details
@@ -405,18 +430,18 @@
 
 You can customize the configuration for any given validation by providing use
 case specific CLI arguments or editing the YAML configuration file.
 
 For example, the following command creates a YAML file for the validation of the
 `new_york_citibike` table: `data-validation validate column -sc my_bq_conn -tc
 my_bq_conn -tbls bigquery-public-data.new_york_citibike.citibike_trips -c
-citibike.yaml`. 
+citibike.yaml`.
 
 The vaildation config file is saved to the GCS path specified by the `PSO_DV_CONFIG_HOME`
-env variable if that has been set; otherwise, it is saved to wherever the tool is run. 
+env variable if that has been set; otherwise, it is saved to wherever the tool is run.
 
 You can now edit the YAML file if, for example, the `new_york_citibike` table is
 stored in datasets that have different names in the source and target systems.
 Once the file is updated and saved, the following command runs the
 validation:
 
 ```
@@ -431,21 +456,21 @@
 
 data-validation configs run -cdir gs://my-bucket/my-validations/
 ```
 
 View the complete YAML file for a Grouped Column validation on the
 [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-yaml-config-grouped-column-validation) page.
 
-You can view a list of all saved validation YAML files using `data-validation configs list`, and print a YAML config using `data-validation configs get -c citibike.yaml`. 
+You can view a list of all saved validation YAML files using `data-validation configs list`, and print a YAML config using `data-validation configs get -c citibike.yaml`.
 
 ### Validation Reports
 
 The result handlers tell DVT where to store the results of
 each validation. The tool can write the results of a validation run to Google
-BigQuery or print to stdout (default). View the schema of the results 
+BigQuery or print to stdout (default). View the schema of the results
 table [here](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/terraform/results_schema.json).
 
 To output to BigQuery, simply include the `-bqrh` flag during a validation run
 like so:
 ```
 data-validation validate column
   -sc bq_conn
@@ -543,14 +568,20 @@
 written in the syntax of the given source.
 
 Note that you are writing the query to execute, which does not have to match
 between source and target as long as the results can be expected to align. If
 the target filter is omitted, the source filter will run on both the source and
 target tables.
 
+### Primary Keys
+
+In many cases, validations (e.g. count, min, max etc) produce one row per table. The comparison between the source
+and target table is to compare the value for each column in the source with the value of the column in the target.
+`grouped-columns` validation and `validate row` produce multiple rows per table. Data Validation Tool needs one or more columns to uniquely identify each row so the source and target can be compared. Data Validation Tool refers to these columns as primary keys. These do not need to be primary keys in the table. The only requirement is that the keys uniquely identify the row in the results.
+
 ### Grouped Columns
 
 Grouped Columns contain the fields you want your aggregations to be broken out
 by, e.g. `SELECT last_updated::DATE, COUNT(*) FROM my.table` will produce a
 resultset that breaks down the count of rows per calendar date.
 
 ### Hash, Concat, and Comparison Fields
@@ -619,43 +650,43 @@
   FROM my.table
   ) as table_0
 ```
 
 If you generate the config file for a row validation, you can see that it uses
 calculated fields to generate the query. You can also use calculated fields
 in column level validations to generate the length of a string, or cast
-a INT field to BIGINT for aggregations. 
+a INT field to BIGINT for aggregations.
 
 See the [Examples page](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-yaml-with-calc-fields-cast-to-numeric-before-aggregation) for a sample
 cast to NUMERIC.
 
 #### Custom Calculated Fields
 
 DVT supports certain functions required for row hash validation natively (i.e. CAST() and CONCAT()),
 which are listed in the CalculatedField() class methods in the [QueryBuilder](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/data_validation/query_builder/query_builder.py).
 
 You can also specify custom functions (i.e. replace() or truncate()) from the Ibis expression
-[API reference](https://ibis-project.org/docs/3.2.0/api/expressions/). Keep in mind these will run
+[API reference](https://ibis-project.org/reference/expressions/generic/). Keep in mind these will run
 on both source and target systems. You will need to specify the Ibis API expression and the parameters
 required, if any, with the 'params' block as shown below:
 
 ```yaml
 - calculated_fields:
   - depth: 0
     field_alias: format_start_time
     source_calculated_columns:
     - start_time
     target_calculated_columns:
     - start_time
     type: custom
-    ibis_expr: ibis.expr.api.TimestampValue.strftime
+    ibis_expr: ibis.expr.types.TemporalValue.strftime
     params:
     - format_str: '%m%d%Y'
 ```
 
-The above block references the [TimestampValue.strftime](https://ibis-project.org/docs/3.2.0/api/expressions/timestamps/#ibis.expr.types.temporal.TemporalValue.strftime) Ibis API expression.
+The above block references the [TemporalValue.strftime](https://ibis-project.org/reference/expressions/timestamps/#ibis.expr.types.temporal.TemporalValue.strftime) Ibis API expression.
 See the [Examples page](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-row-validation-yaml-with-custom-calc-field)
 for a sample YAML with a custom calculated field.
 
 ## Contributing
 
 Contributions are welcome. See the [Contributing guide](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/CONTRIBUTING.md) for details.
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/__init__.py` & `google-pso-data-validator-4.0.0/data_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.2.0/data_validation/__main__.py` & `google-pso-data-validator-4.0.0/data_validation/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,22 +64,22 @@
         "float32",
         "int8",
         "int16",
         "int32",
         "int64",
         "decimal",
         "timestamp",
-        "float64[non-nullable]",
-        "float32[non-nullable]",
-        "int8[non-nullable]",
-        "int16[non-nullable]",
-        "int32[non-nullable]",
-        "int64[non-nullable]",
-        "decimal[non-nullable]",
-        "timestamp[non-nullable]",
+        "!float64",
+        "!float32",
+        "!int8",
+        "!int16",
+        "!int32",
+        "!int64",
+        "!decimal",
+        "!timestamp",
     ]
 
     if args.wildcard_include_string_len:
         supported_data_types.append("string")
 
     cast_to_bigint = True if args.cast_to_bigint else False
 
@@ -134,15 +134,16 @@
     if len(fields) > 0:
         max_depth = max([x["depth"] for x in fields])
     else:
         max_depth = 0
     for field in fields:
         calculated_configs.append(
             config_manager.build_config_calculated_fields(
-                field["reference"],
+                field["source_reference"],
+                field["target_reference"],
                 field["calc_type"],
                 field["name"],
                 field["depth"],
                 custom_params=field.get("calc_params"),
             )
         )
     if args.hash:
@@ -170,16 +171,15 @@
     # Append SCHEMA_VALIDATION configs
     if config_manager.validation_type == consts.SCHEMA_VALIDATION:
         if args.exclusion_columns is not None:
             exclusion_columns = cli_tools.get_arg_list(args.exclusion_columns)
             config_manager.append_exclusion_columns(
                 [col.casefold() for col in exclusion_columns]
             )
-        if args.allow_list is not None:
-            config_manager.append_allow_list(args.allow_list)
+        config_manager.append_allow_list(args.allow_list, args.allow_list_file)
 
     # Append CUSTOM_QUERY configs
     if config_manager.validation_type == consts.CUSTOM_QUERY:
         config_manager.append_custom_query_type(args.custom_query_type)
 
         # Get source sql query from source sql file or inline query
         if args.source_query:
@@ -387,20 +387,24 @@
     table_configs = _compare_match_tables(
         source_table_map, target_table_map, score_cutoff=score_cutoff
     )
     return json.dumps(table_configs)
 
 
 def run_raw_query_against_connection(args):
-    """Return results of raw query for adhoc usage."""
+    """Return results of raw query for ad hoc usage."""
     mgr = state_manager.StateManager()
     client = clients.get_data_client(mgr.get_connection_config(args.conn))
-
-    with client.raw_sql(args.query, results=True) as cur:
-        return cur.fetchall()
+    cursor = client.raw_sql(args.query)
+    res = cursor.fetchall()
+    try:
+        cursor.close()
+    except Exception:
+        pass
+    return res
 
 
 def convert_config_to_yaml(args, config_managers):
     """Return dict objects formatted for yaml validations.
 
     Args:
         config_managers (list[ConfigManager]): List of config manager instances.
@@ -433,16 +437,20 @@
         result_handler=None,
         verbose=verbose,
     )
     if dry_run:
         print(
             json.dumps(
                 {
-                    "source_query": validator.validation_builder.get_source_query().compile(),
-                    "target_query": validator.validation_builder.get_target_query().compile(),
+                    "source_query": str(
+                        validator.validation_builder.get_source_query().compile()
+                    ),
+                    "target_query": str(
+                        validator.validation_builder.get_target_query().compile()
+                    ),
                 },
                 indent=4,
             )
         )
     else:
         validator.execute()
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/app.py` & `google-pso-data-validator-4.0.0/data_validation/app.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.2.0/data_validation/cli_tools.py` & `google-pso-data-validator-4.0.0/data_validation/cli_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         ["database", "Database to connect to (default master)"],
     ],
     "Snowflake": [
         ["user", "Username to connect to"],
         ["password", "Password for authentication of user"],
         ["account", "Snowflake account to connect to"],
         ["database", "Database in snowflake to connect to"],
-        ["schema", "Schema in the database to connect to"],
+        ["connect_args", "(Optional) Additional connection arg mapping"],
     ],
     "Postgres": [
         ["host", "Desired Postgres host."],
         ["port", "Postgres port to connect on (ie. 5432)"],
         ["user", "Username to connect to"],
         ["password", "Password for authentication of user"],
         ["database", "Database in postgres to connect to (default postgres)"],
@@ -113,15 +113,15 @@
         ["instance_id", "ID of Spanner instance to connect to"],
         ["database_id", "ID of Spanner database (schema) to connect to"],
         ["google_service_account_key_path", "(Optional) GCP SA Key Path"],
     ],
     "FileSystem": [
         ["table_name", "Table name to use as reference for file data"],
         ["file_path", "The local, s3, or GCS file path to the data"],
-        ["file_type", "The file type of the file.'csv' or 'json'"],
+        ["file_type", "The file type of the file. 'csv' or 'json'"],
     ],
     "Impala": [
         ["host", "Desired Impala host"],
         ["port", "Desired Imapala port (10000 if not provided)"],
         ["database", "Desired Impala database (default if not provided)"],
         ["auth_mechanism", "Desired Impala auth mechanism (PLAIN if not provided)"],
         [
@@ -332,15 +332,15 @@
         "-dr",
         action="store_true",
         help="Prints source and target SQL to stdout in lieu of performing a validation.",
     )
     run_parser.add_argument(
         "--config-file",
         "-c",
-        help="YAML Config File Path to be used for building or running validations.",
+        help="YAML Config File path to be used for building or running validations.",
     )
     run_parser.add_argument(
         "--config-dir",
         "-cdir",
         help="Directory path containing YAML Config Files to be used for running validations.",
     )
 
@@ -606,15 +606,20 @@
         "--exclusion-columns",
         "-ec",
         help="Comma separated list of columns 'col_a,col_b' to be excluded from the schema validation",
     )
     optional_arguments.add_argument(
         "--allow-list",
         "-al",
-        help="Comma separated list of datatype mappings due to incompatible datatypes in source and target. e.g: decimal(12,2):decimal(38,9),string[non-nullable]:string",
+        help="Comma separated list of datatype mappings due to incompatible datatypes in source and target. e.g.: decimal(12,2):decimal(38,9),!string:string,decimal(10-18,0):int64",
+    )
+    optional_arguments.add_argument(
+        "--allow-list-file",
+        "-alf",
+        help="YAML file containing default --allow-list mappings. Can be used in conjunction with --allow-list. e.g.: samples/allow_list/oracle_to_bigquery.yaml or gs://dvt-allow-list-files/oracle_to_bigquery.yaml. See example files in samples/allow_list/",
     )
 
     # Group required arguments
     required_arguments = schema_parser.add_argument_group("required arguments")
     required_arguments.add_argument(
         "--tables-list",
         "-tbls",
@@ -657,14 +662,25 @@
     )
     optional_arguments.add_argument(
         "--threshold",
         "-th",
         type=threshold_float,
         help="Float max threshold for percent difference",
     )
+    optional_arguments.add_argument(
+        "--use-random-row",
+        "-rr",
+        action="store_true",
+        help="Finds a set of random rows of the first primary key supplied.",
+    )
+    optional_arguments.add_argument(
+        "--random-row-batch-size",
+        "-rbs",
+        help="Row batch size used for random row filters (default 10,000).",
+    )
 
     # Group required arguments
     required_arguments = custom_query_row_parser.add_argument_group(
         "required arguments"
     )
     required_arguments.add_argument(
         "--primary-keys",
@@ -887,15 +903,15 @@
     required_arguments.add_argument(
         "--target-conn", "-tc", required=True, help="Target connection name"
     )
     required_arguments.add_argument(
         "--config-dir",
         "-cdir",
         required=True,
-        help="Directory Path to store YAML Config Files. "
+        help="Directory path to store YAML config files. "
         "GCS: Provide a full gs:// path of the target directory. "
         "Eg: `gs://<BUCKET>/partiitons_dir`. "
         "Local: Provide a relative path of the target directory. "
         "Eg: `partitions_dir`",
     )
     required_arguments.add_argument(
         "--partition-num",
@@ -936,22 +952,14 @@
         # TODO: update if we start to support other statuses
         help=(
             "Comma separated list of statuses to filter the validation results. "
             "Supported statuses are (success, fail). If no list is provided, "
             "all statuses are returned"
         ),
     )
-    optional_arguments.add_argument(
-        "--partition-key",
-        "-partkey",
-        help=(
-            "Column on which the partitions would be generated. "
-            "Column type must be integer. Defaults to Primary key"
-        ),
-    )
 
 
 def get_connection_config_from_args(args):
     """Return dict with connection config supplied."""
     config = {
         consts.SOURCE_TYPE: args.connect_type,
         consts.SECRET_MANAGER_TYPE: getattr(args, consts.SECRET_MANAGER_TYPE),
@@ -1259,15 +1267,14 @@
     # Get random row arguments. Not supported in case of schema validation,
     # custom-query validation and generate-table-partitions
     use_random_rows = None
     random_row_batch_size = None
     if (
         args.command != "generate-table-partitions"
         and config_type != consts.SCHEMA_VALIDATION
-        and config_type != consts.CUSTOM_QUERY
     ):
         use_random_rows = args.use_random_row
         random_row_batch_size = args.random_row_batch_size
 
     # Get table list. Not supported in case of custom query validation
     is_filesystem = source_client._source_type == "FileSystem"
     if config_type == consts.CUSTOM_QUERY:
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/client_info.py` & `google-pso-data-validator-4.0.0/data_validation/client_info.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.2.0/data_validation/clients.py` & `google-pso-data-validator-4.0.0/data_validation/clients.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,100 +10,81 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import copy
-import warnings
 import logging
+import warnings
+
 import google.oauth2.service_account
 import ibis
-import ibis.backends.pandas
-import ibis_bigquery
 import pandas
-import third_party.ibis.ibis_addon.datatypes
-import third_party.ibis.ibis_addon.base_sqlalchemy.alchemy
-import third_party.ibis.ibis_postgres.client
 from google.cloud import bigquery
-from ibis.backends.mysql.client import MySQLClient
-from ibis.backends.pandas.client import PandasClient
-from ibis.backends.postgres.client import PostgreSQLClient
-from third_party.ibis.ibis_cloud_spanner.api import connect as spanner_connect
-from third_party.ibis.ibis_impala.api import impala_connect
+
 from data_validation import client_info, consts, exceptions
 from data_validation.secret_manager import SecretManagerBuilder
-from third_party.ibis.ibis_redshift.client import RedShiftClient
+from third_party.ibis.ibis_cloud_spanner.api import spanner_connect
+from third_party.ibis.ibis_impala.api import impala_connect
+from third_party.ibis.ibis_mssql.api import mssql_connect
+from third_party.ibis.ibis_redshift.api import redshift_connect
 
 ibis.options.sql.default_limit = None
 
-# Our customized Ibis Datatype logic add support for new types
-third_party.ibis.ibis_addon.datatypes
-
-# TODO(googleapis/google-auth-library-python#520): Remove after issue is resolved
-warnings.filterwarnings(
-    "ignore", "Your application has authenticated using end user credentials"
-)
+# Filter Ibis MySQL error when loading client.table()
 warnings.filterwarnings(
     "ignore",
-    "Cannot create BigQuery Storage client, the dependency google-cloud-bigquery-storage is not installed",
-)
-warnings.filterwarnings(
-    "ignore", "The GenericFunction 'regex_extract' is already registered"
+    "`BaseBackend.database` is deprecated; use equivalent methods in the backend",
 )
 
 
 def _raise_missing_client_error(msg):
     def get_client_call(*args, **kwargs):
         raise Exception(msg)
 
     return get_client_call
 
 
-# If you have a Teradata License there is an optional teradatasql import
+# Teradata requires teradatasql and licensing
 try:
-    from third_party.ibis.ibis_teradata.client import TeradataClient
+    from third_party.ibis.ibis_teradata.api import teradata_connect
 except Exception:
     msg = "pip install teradatasql (requires Teradata licensing)"
-    TeradataClient = _raise_missing_client_error(msg)
+    teradata_connect = _raise_missing_client_error(msg)
 
-# If you have an cx_Oracle driver installed
+# Oracle requires cx_Oracle driver
 try:
-    from third_party.ibis.ibis_oracle.client import OracleClient
+    from third_party.ibis.ibis_oracle.api import oracle_connect
 except Exception:
-    OracleClient = _raise_missing_client_error("pip install cx_Oracle")
+    oracle_connect = _raise_missing_client_error("pip install cx_Oracle")
 
+# Snowflake requires snowflake-connector-python and snowflake-sqlalchemy
 try:
-    from third_party.ibis.ibis_mssql.client import MSSQLClient
-except Exception:
-    MSSQLClient = _raise_missing_client_error("pip install pyodbc")
-
-try:
-    from third_party.ibis.ibis_snowflake.client import (
-        SnowflakeClient as snowflake_connect,
-    )
+    from third_party.ibis.ibis_snowflake.api import snowflake_connect
 except Exception:
     snowflake_connect = _raise_missing_client_error(
-        "pip install snowflake-connector-python"
+        "pip install snowflake-connector-python && pip install snowflake-sqlalchemy"
     )
 
-# If you have Db2 client installed
+# DB2 requires ibm_db_sa
 try:
-    from third_party.ibis.ibis_DB2.client import DB2Client
+    from third_party.ibis.ibis_db2.api import db2_connect
 except Exception:
-    DB2Client = _raise_missing_client_error("pip install ibm_db_sa")
+    db2_connect = _raise_missing_client_error("pip install ibm_db_sa")
 
 
-def get_bigquery_client(project_id, dataset_id=None, credentials=None):
+def get_bigquery_client(project_id, dataset_id="", credentials=None):
     info = client_info.get_http_client_info()
     google_client = bigquery.Client(
         project=project_id, client_info=info, credentials=credentials
     )
-    ibis_client = ibis_bigquery.connect(
-        project_id, dataset_id=dataset_id, credentials=credentials
+
+    ibis_client = ibis.bigquery.connect(
+        project_id=project_id, dataset_id=dataset_id, credentials=credentials
     )
 
     # Override the BigQuery client object to ensure the correct user agent is
     # included.
     ibis_client.client = google_client
     return ibis_client
 
@@ -118,109 +99,102 @@
     if file_type == "csv":
         df = pandas.read_csv(file_path)
     elif file_type == "json":
         df = pandas.read_json(file_path)
     else:
         raise ValueError(f"Unknown Pandas File Type: {file_type}")
 
-    pandas_client = ibis.backends.pandas.connect({table_name: df})
+    pandas_client = ibis.pandas.connect({table_name: df})
 
     return pandas_client
 
 
 def is_oracle_client(client):
     try:
-        return isinstance(client, OracleClient)
+        return client.name == "oracle"
     except TypeError:
-        # When no Oracle client has been installed OracleClient is not a class
+        # When no Oracle backend has been installed OracleBackend is not a class
         return False
 
 
 def get_ibis_table(client, schema_name, table_name, database_name=None):
     """Return Ibis Table for Supplied Client.
 
     client (IbisClient): Client to use for table
     schema_name (str): Schema name of table object
     table_name (str): Table name of table object
     database_name (str): Database name (generally default is used)
     """
-    if type(client) in [
-        OracleClient,
-        PostgreSQLClient,
-        DB2Client,
-        MSSQLClient,
-        RedShiftClient,
+    if client.name in [
+        "oracle",
+        "postgres",
+        "db2",
+        "mssql",
+        "redshift",
     ]:
         return client.table(table_name, database=database_name, schema=schema_name)
-    elif type(client) in [PandasClient]:
+    elif client.name == "pandas":
         return client.table(table_name, schema=schema_name)
     else:
         return client.table(table_name, database=schema_name)
 
 
 def get_ibis_query(client, query):
     """Return Ibis Table from query expression for Supplied Client."""
     return client.sql(query)
 
 
 def get_ibis_table_schema(client, schema_name, table_name):
     """Return Ibis Table Schema for Supplied Client.
 
     client (IbisClient): Client to use for table
-    schema_name (str): Schema name of table object
+    schema_name (str): Schema name of table object, may not need this since Backend uses database
     table_name (str): Table name of table object
     database_name (str): Database name (generally default is used)
     """
-    if type(client) in [MySQLClient, PostgreSQLClient, RedShiftClient]:
-        return client.schema(schema_name).table(table_name).schema()
+    if client.name in [
+        "mysql",
+        "oracle",
+        "postgres",
+        "db2",
+        "mssql",
+        "redshift",
+        "snowflake",
+    ]:
+        return client.table(table_name, schema=schema_name).schema()
     else:
         return client.get_schema(table_name, schema_name)
 
 
 def list_schemas(client):
     """Return a list of schemas in the DB."""
-    if type(client) in [
-        OracleClient,
-        PostgreSQLClient,
-        DB2Client,
-        MSSQLClient,
-        RedShiftClient,
-    ]:
-        return client.list_schemas()
-    elif hasattr(client, "list_databases"):
-        return client.list_databases()
+    if hasattr(client, "list_databases"):
+        try:
+            return client.list_databases()
+        except NotImplementedError:
+            return [None]
     else:
         return [None]
 
 
 def list_tables(client, schema_name):
     """Return a list of tables in the DB schema."""
-    if type(client) in [
-        OracleClient,
-        PostgreSQLClient,
-        DB2Client,
-        MSSQLClient,
-        RedShiftClient,
-    ]:
-        return client.list_tables(schema=schema_name)
-    elif schema_name:
-        return client.list_tables(database=schema_name)
-    else:
+    if client.name in ["oracle", "postgres", "db2", "mssql", "redshift", "snowflake"]:
         return client.list_tables()
+    return client.list_tables(database=schema_name)
 
 
 def get_all_tables(client, allowed_schemas=None):
     """Return a list of tuples with database and table names.
 
     client (IbisClient): Client to use for tables
     allowed_schemas (List[str]): List of schemas to pull.
     """
     table_objs = []
     schemas = list_schemas(client)
-
     for schema_name in schemas:
         if allowed_schemas and schema_name not in allowed_schemas:
             continue
         try:
             tables = list_tables(client, schema_name)
         except Exception as e:
             logging.warning(f"List Tables Error: {schema_name} -> {e}")
@@ -295,18 +269,18 @@
             return 30
     return 128
 
 
 CLIENT_LOOKUP = {
     "BigQuery": get_bigquery_client,
     "Impala": impala_connect,
-    "MySQL": MySQLClient,
-    "Oracle": OracleClient,
+    "MySQL": ibis.mysql.connect,
+    "Oracle": oracle_connect,
     "FileSystem": get_pandas_client,
-    "Postgres": PostgreSQLClient,
-    "Redshift": RedShiftClient,
-    "Teradata": TeradataClient,
-    "MSSQL": MSSQLClient,
+    "Postgres": ibis.postgres.connect,
+    "Redshift": redshift_connect,
+    "Teradata": teradata_connect,
+    "MSSQL": mssql_connect,
     "Snowflake": snowflake_connect,
     "Spanner": spanner_connect,
-    "DB2": DB2Client,
+    "DB2": db2_connect,
 }
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/combiner.py` & `google-pso-data-validator-4.0.0/data_validation/combiner.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,71 +90,60 @@
     result_df = client.execute(documented)
     result_df.validation_status.fillna(consts.VALIDATION_STATUS_FAIL, inplace=True)
     return result_df
 
 
 def _calculate_difference(field_differences, datatype, validation, is_value_comparison):
     pct_threshold = ibis.literal(validation.threshold)
-
     if isinstance(datatype, ibis.expr.datatypes.Timestamp):
         source_value = field_differences["differences_source_value"].epoch_seconds()
         target_value = field_differences["differences_target_value"].epoch_seconds()
-    elif isinstance(datatype, ibis.expr.datatypes.Float64):
-        # Float64 type results from AVG() aggregation
-        source_value = field_differences["differences_source_value"].round(digits=4)
-        target_value = field_differences["differences_target_value"].round(digits=4)
-    elif isinstance(datatype, ibis.expr.datatypes.Decimal):
+    elif isinstance(datatype, ibis.expr.datatypes.Decimal) or isinstance(
+        datatype, ibis.expr.datatypes.Float64
+    ):
         source_value = (
             field_differences["differences_source_value"]
-            .cast("float64")
+            .cast("float32")
             .round(digits=4)
         )
         target_value = (
             field_differences["differences_target_value"]
-            .cast("float64")
+            .cast("float32")
             .round(digits=4)
         )
     else:
         source_value = field_differences["differences_source_value"]
         target_value = field_differences["differences_target_value"]
 
     # Does not calculate difference between agg values for row hash due to int64 overflow
-    if is_value_comparison:
-        difference = pct_difference = ibis.null()
+    if is_value_comparison or isinstance(datatype, ibis.expr.datatypes.String):
+        # String data types i.e "None" can be returned for NULL timestamp/datetime aggs
+        if is_value_comparison:
+            difference = pct_difference = ibis.null()
+        else:
+            difference = pct_difference = ibis.null().cast("float64")
         validation_status = (
             ibis.case()
             .when(
                 target_value.isnull() & source_value.isnull(),
                 consts.VALIDATION_STATUS_SUCCESS,
             )
             .when(
                 target_value == source_value,
                 consts.VALIDATION_STATUS_SUCCESS,
             )
             .else_(consts.VALIDATION_STATUS_FAIL)
             .end()
         )
-    # String data types i.e "None" can be returned for NULL timestamp/datetime aggs
-    elif isinstance(datatype, ibis.expr.datatypes.String):
-        difference = pct_difference = ibis.null().cast("float64")
-        validation_status = (
-            ibis.case()
-            .when(
-                target_value.isnull() & source_value.isnull(),
-                consts.VALIDATION_STATUS_SUCCESS,
-            )
-            .else_(consts.VALIDATION_STATUS_FAIL)
-            .end()
-        )
     else:
         difference = (target_value - source_value).cast("float64")
 
         pct_difference_nonzero = (
             ibis.literal(100.0)
-            * difference
+            * difference.cast("float32")
             / (
                 source_value.case()
                 .when(ibis.literal(0), target_value)
                 .else_(source_value)
                 .end()
             ).cast("float64")
         ).cast("float64")
@@ -362,14 +351,12 @@
 def _add_metadata(joined, run_metadata):
     # TODO: Add source and target queries to metadata
     run_metadata.end_time = datetime.datetime.now(datetime.timezone.utc)
 
     joined = joined[
         joined,
         ibis.literal(run_metadata.run_id).name("run_id"),
-        ibis.literal(
-            run_metadata.labels, type="array<struct<key:string,value:string>>"
-        ).name("labels"),
+        ibis.literal(run_metadata.labels).name("labels"),
         ibis.literal(run_metadata.start_time).name("start_time"),
         ibis.literal(run_metadata.end_time).name("end_time"),
     ]
     return joined
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/config_manager.py` & `google-pso-data-validator-4.0.0/data_validation/config_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import logging
 from typing import Optional, Union, TYPE_CHECKING
+import yaml
 
 import google.oauth2.service_account
-from ibis_bigquery.client import BigQueryClient
+
 import ibis.expr.datatypes as dt
 
 from data_validation import clients, consts, state_manager
 from data_validation.result_handlers.bigquery import BigQueryResultHandler
 from data_validation.result_handlers.text import TextResultHandler
 from data_validation.validation_builder import ValidationBuilder
 
@@ -101,15 +102,15 @@
     def use_random_rows(self):
         """Return if the validation should use a random row filter."""
         return self._config.get(consts.CONFIG_USE_RANDOM_ROWS) or False
 
     def random_row_batch_size(self):
         """Return if the validation should use a random row filter."""
         return (
-            self._config.get(consts.CONFIG_RANDOM_ROW_BATCH_SIZE)
+            int(self._config.get(consts.CONFIG_RANDOM_ROW_BATCH_SIZE))
             or consts.DEFAULT_NUM_RANDOM_ROWS
         )
 
     def get_random_row_batch_size(self):
         """Return number of random rows or None."""
         return self.random_row_batch_size() if self.use_random_rows() else None
 
@@ -308,17 +309,36 @@
 
     def append_exclusion_columns(self, column_configs):
         """Append exclusion columns to existing config."""
         self._config[consts.CONFIG_EXCLUSION_COLUMNS] = (
             self.exclusion_columns + column_configs
         )
 
-    def append_allow_list(self, allow_list):
-        """Append allow_list of datatype to existing config."""
-        self._config[consts.CONFIG_ALLOW_LIST] = allow_list
+    def append_allow_list(
+        self, allow_list: Union[str, None], allow_list_file: Union[str, None]
+    ):
+        """Append datatype allow_list to existing config."""
+        full_allow_list = []
+        if allow_list:
+            allow_list = allow_list.replace(" ", "")
+            full_allow_list.append(allow_list)
+        if allow_list_file:
+            mgr = state_manager.StateManager(file_system_root_path=allow_list_file)
+            try:
+                allow_list_yaml = mgr.read_file(allow_list_file)
+            except FileNotFoundError as e:
+                raise ValueError(
+                    "Cannot locate --allow-list-file: {allow_list_file}"
+                ) from e
+            allow_list_dict = yaml.safe_load(allow_list_yaml)
+            full_allow_list.append(
+                ",".join([f"{_[0]}:{_[1]}" for _ in allow_list_dict.items()])
+            )
+
+        self._config[consts.CONFIG_ALLOW_LIST] = ",".join(full_allow_list)
 
     def get_source_ibis_table(self):
         """Return IbisTable from source."""
         if not hasattr(self, "_source_ibis_table"):
             self._source_ibis_table = clients.get_ibis_table(
                 self.source_client, self.source_schema, self.source_table
             )
@@ -568,24 +588,24 @@
 
         if calculated_config[consts.CONFIG_FIELD_ALIAS] not in existing_calc_fields:
             self.append_calculated_fields([calculated_config])
         return calculated_config
 
     def append_pre_agg_calc_field(
         self, source_column, target_column, agg_type, column_type, column_position
-    ):
+    ) -> dict:
         """Append calculated field for length(string) or epoch_seconds(timestamp) for preprocessing before column validation aggregation."""
         depth, cast_type = 0, None
-
         if column_type == "string":
             calc_func = "length"
 
-        elif column_type == "timestamp":
-            if isinstance(self.source_client, BigQueryClient) or isinstance(
-                self.target_client, BigQueryClient
+        elif column_type == "timestamp" or column_type == "!timestamp":
+            if (
+                self.source_client.name == "bigquery"
+                or self.target_client.name == "bigquery"
             ):
                 calc_func = "cast"
                 cast_type = "timestamp"
                 pre_calculated_config = self.build_and_append_pre_agg_calc_config(
                     source_column,
                     target_column,
                     calc_func,
@@ -596,22 +616,18 @@
                 source_column = target_column = pre_calculated_config[
                     consts.CONFIG_FIELD_ALIAS
                 ]
                 depth = 1
 
             calc_func = "epoch_seconds"
 
-        elif column_type == "int32":
+        elif column_type == "int32" or column_type == "!int32":
             calc_func = "cast"
             cast_type = "int64"
 
-        elif column_type == "decimal":
-            calc_func = "cast"
-            cast_type = "float64"
-
         else:
             raise ValueError(f"Unsupported column type: {column_type}")
 
         calculated_config = self.build_and_append_pre_agg_calc_config(
             source_column, target_column, calc_func, column_position, cast_type, depth
         )
 
@@ -628,14 +644,35 @@
 
         return aggregate_config
 
     def build_config_column_aggregates(
         self, agg_type, arg_value, supported_types, cast_to_bigint=False
     ):
         """Return list of aggregate objects of given agg_type."""
+
+        def decimal_too_big_for_64bit(
+            source_column_ibis_type, target_column_ibis_type
+        ) -> bool:
+            return bool(
+                (
+                    isinstance(source_column_ibis_type, dt.Decimal)
+                    and (
+                        source_column_ibis_type.precision is None
+                        or source_column_ibis_type.precision > 18
+                    )
+                )
+                and (
+                    isinstance(target_column_ibis_type, dt.Decimal)
+                    and (
+                        target_column_ibis_type.precision is None
+                        or target_column_ibis_type.precision > 18
+                    )
+                )
+            )
+
         aggregate_configs = []
         source_table = self.get_source_ibis_calculated_table()
         target_table = self.get_target_ibis_calculated_table()
 
         casefold_source_columns = {x.casefold(): str(x) for x in source_table.columns}
         casefold_target_columns = {x.casefold(): str(x) for x in target_table.columns}
 
@@ -643,16 +680,21 @@
             arg_value = [x.casefold() for x in arg_value]
             if supported_types:
                 supported_types.append("string")
 
         allowlist_columns = arg_value or casefold_source_columns
         for column_position, column in enumerate(casefold_source_columns):
             # Get column type and remove precision/scale attributes
-            column_type_str = str(source_table[casefold_source_columns[column]].type())
-            column_type = column_type_str.split("(")[0]
+            source_column_ibis_type = source_table[
+                casefold_source_columns[column]
+            ].type()
+            target_column_ibis_type = target_table[
+                casefold_target_columns[column]
+            ].type()
+            column_type = str(source_column_ibis_type).split("(")[0]
 
             if column not in allowlist_columns:
                 continue
             elif column not in casefold_target_columns:
                 logging.warning(
                     f"Skipping {agg_type} on {column} as column is not present in target table"
                 )
@@ -661,26 +703,28 @@
                 if self.verbose:
                     logging.info(
                         f"Skipping {agg_type} on {column} due to data type: {column_type}"
                     )
                 continue
 
             if (
-                column_type == "string"
-                or (cast_to_bigint and column_type == "int32")
+                (column_type == "string" or column_type == "!string")
+                or (
+                    cast_to_bigint
+                    and (column_type == "int32" or column_type == "!int32")
+                )
                 or (
-                    column_type == "timestamp"
+                    (column_type == "timestamp" or column_type == "!timestamp")
                     and agg_type
                     in (
                         "sum",
                         "avg",
                         "bit_xor",
                     )  # For timestamps: do not convert to epoch seconds for min/max
                 )
-                or (column_type == "decimal")
             ):
                 aggregate_config = self.append_pre_agg_calc_field(
                     casefold_source_columns[column],
                     casefold_target_columns[column],
                     agg_type,
                     column_type,
                     column_position,
@@ -691,22 +735,27 @@
                     consts.CONFIG_SOURCE_COLUMN: casefold_source_columns[column],
                     consts.CONFIG_TARGET_COLUMN: casefold_target_columns[column],
                     consts.CONFIG_FIELD_ALIAS: self._prefix_calc_col_name(
                         column, f"{agg_type}", column_position
                     ),
                     consts.CONFIG_TYPE: agg_type,
                 }
+                if decimal_too_big_for_64bit(
+                    source_column_ibis_type, target_column_ibis_type
+                ):
+                    aggregate_config[consts.CONFIG_CAST] = "string"
 
             aggregate_configs.append(aggregate_config)
 
         return aggregate_configs
 
     def build_config_calculated_fields(
         self,
-        reference,
+        source_reference,
+        target_reference,
         calc_type,
         alias,
         depth,
         supported_types=None,
         arg_value=None,
         custom_params: Optional[dict] = None,
     ) -> dict:
@@ -731,16 +780,16 @@
             elif supported_types and column_type not in supported_types:
                 if self.verbose:
                     msg = f"Skipping {calc_type} on {column} due to data type: {column_type}"
                     logging.info(msg)
                 continue
 
         calculated_config = {
-            consts.CONFIG_CALCULATED_SOURCE_COLUMNS: reference,
-            consts.CONFIG_CALCULATED_TARGET_COLUMNS: reference,
+            consts.CONFIG_CALCULATED_SOURCE_COLUMNS: source_reference,
+            consts.CONFIG_CALCULATED_TARGET_COLUMNS: target_reference,
             consts.CONFIG_FIELD_ALIAS: alias,
             consts.CONFIG_TYPE: calc_type,
             consts.CONFIG_DEPTH: depth,
         }
 
         if calc_type == consts.CONFIG_CUSTOM and custom_params:
             calculated_config.update(custom_params)
@@ -756,56 +805,57 @@
                 ]
             )
         return self._comparison_max_col_length
 
     def _strftime_format(
         self, column_type: Union[dt.Date, dt.Timestamp], client
     ) -> str:
-        if isinstance(column_type, dt.Timestamp):
+        if column_type.is_timestamp():
             return "%Y-%m-%d %H:%M:%S"
         if clients.is_oracle_client(client):
             # Oracle DATE is a DateTime
             return "%Y-%m-%d %H:%M:%S"
         return "%Y-%m-%d"
 
     def _apply_base_cast_overrides(
         self,
-        column: str,
+        source_column: str,
+        target_column: str,
         col_config: dict,
         source_table: "ibis.expr.types.TableExpr",
         target_table: "ibis.expr.types.TableExpr",
     ) -> dict:
         """Mutates col_config to contain any overrides. Also returns col_config for convenience."""
         if col_config["calc_type"] != "cast":
             return col_config
 
         source_table_schema = {k: v for k, v in source_table.schema().items()}
         target_table_schema = {k: v for k, v in target_table.schema().items()}
 
         if isinstance(
-            source_table_schema[column], (dt.Date, dt.Timestamp)
-        ) and isinstance(target_table_schema[column], (dt.Date, dt.Timestamp)):
+            source_table_schema[source_column], (dt.Date, dt.Timestamp)
+        ) and isinstance(target_table_schema[target_column], (dt.Date, dt.Timestamp)):
             # Use strftime rather than cast for temporal comparisons.
             # Pick the most permissive format across the two engines.
             # For example Date -> Timestamp should format both source and target as Date.
             fmt = min(
                 [
                     self._strftime_format(
-                        source_table_schema[column], self.source_client
+                        source_table_schema[source_column], self.source_client
                     ),
                     self._strftime_format(
-                        source_table_schema[column], self.target_client
+                        source_table_schema[source_column], self.target_client
                     ),
                 ],
                 key=len,
             )
             col_config["calc_type"] = consts.CONFIG_CUSTOM
             custom_params = {
                 "calc_params": {
-                    consts.CONFIG_CUSTOM_IBIS_EXPR: "ibis.expr.api.TimestampValue.strftime",
+                    consts.CONFIG_CUSTOM_IBIS_EXPR: "ibis.expr.types.TemporalValue.strftime",
                     consts.CONFIG_CUSTOM_PARAMS: [
                         {consts.CONFIG_CUSTOM_PARAM_FORMAT_STR: fmt}
                     ],
                 }
             }
             col_config.update(custom_params)
 
@@ -813,20 +863,31 @@
 
     def build_dependent_aliases(self, calc_type, col_list=None):
         """This is a utility function for determining the required depth of all fields"""
         source_table = self.get_source_ibis_calculated_table()
         target_table = self.get_target_ibis_calculated_table()
 
         order_of_operations = []
-        if col_list is None:
+        casefold_source_columns = {x.casefold(): str(x) for x in source_table.columns}
+        casefold_target_columns = {x.casefold(): str(x) for x in target_table.columns}
+
+        if col_list:
+            casefold_col_list = [x.casefold() for x in col_list]
+            # Filter columns based on col_list if provided
             casefold_source_columns = {
-                x.casefold(): str(x) for x in source_table.columns
+                k: v
+                for (k, v) in casefold_source_columns.items()
+                if k in casefold_col_list
             }
-        else:
-            casefold_source_columns = {x.casefold(): str(x) for x in col_list}
+            casefold_target_columns = {
+                k: v
+                for (k, v) in casefold_target_columns.items()
+                if k in casefold_col_list
+            }
+
         if calc_type == "hash":
             order_of_operations = [
                 "cast",
                 "ifnull",
                 "rstrip",
                 "upper",
                 "concat",
@@ -840,41 +901,52 @@
                 "upper",
                 "concat",
             ]
         column_aliases = {}
         col_names = []
         for i, calc in enumerate(order_of_operations):
             if i == 0:
-                previous_level = [x for x in casefold_source_columns.values()]
+                previous_level = [x for x in casefold_source_columns.keys()]
             else:
                 previous_level = [k for k, v in column_aliases.items() if v == i - 1]
             if calc in ["concat", "hash"]:
                 col = {}
-                col["reference"] = previous_level
+                col["source_reference"] = previous_level
+                col["target_reference"] = previous_level
                 col["name"] = f"{calc}__all"
                 col["calc_type"] = calc
                 col["depth"] = i
                 name = col["name"]
                 # need to capture all aliases at the previous level. probably name concat__all
                 column_aliases[name] = i
                 col_names.append(col)
             else:
                 # This needs to be the previous manifest of columns
                 for j, column in enumerate(previous_level):
                     col = {}
-                    col["reference"] = [column]
+                    col["source_reference"] = [column]
+                    col["target_reference"] = [column]
                     col["name"] = self._prefix_calc_col_name(column, calc, j)
                     col["calc_type"] = calc
                     col["depth"] = i
 
                     if i == 0:
+                        # If depth 0, get raw column name with correct casing
+                        source_column = casefold_source_columns[column]
+                        target_column = casefold_target_columns[column]
+                        col["source_reference"] = [source_column]
+                        col["target_reference"] = [target_column]
                         # If we are casting the base column (i == 0) then apply any
                         # datatype specific overrides.
                         col = self._apply_base_cast_overrides(
-                            column, col, source_table, target_table
+                            source_column,
+                            target_column,
+                            col,
+                            source_table,
+                            target_table,
                         )
 
                     name = col["name"]
                     column_aliases[name] = i
                     col_names.append(col)
         return col_names
 
@@ -882,15 +954,15 @@
         """Return query from input file"""
         query = ""
         try:
             file = open(filename, "r")
             query = file.read()
             query = query.rstrip(";\n")
         except IOError:
-            logging.warning("Cannot read query file: ", filename)
+            logging.error("Cannot read query file: ", filename)
 
         if not query or query.isspace():
             raise ValueError(
                 "Expected file with sql query, got empty file or file with white spaces. "
                 f"input file: {filename}"
             )
         file.close()
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/consts.py` & `google-pso-data-validator-4.0.0/data_validation/consts.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,7 +163,11 @@
     "aggregation_type",
     "difference",
     "primary_keys",
     "group_by_columns",
     "num_random_rows",
     "pct_threshold",
 ]
+
+# Constants for the named column used in generate partitions
+# this cannot conflict with primary key column names
+DVT_POS_COL = "dvt_pos_num"
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/data_validation.py` & `google-pso-data-validator-4.0.0/data_validation/data_validation.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 
 import json
 import logging
 import warnings
 from concurrent.futures import ThreadPoolExecutor
 
 import ibis.backends.pandas
-import ibis.expr.datatypes as dt
-import numpy
 import pandas
 
 from data_validation import combiner, consts, metadata
 from data_validation.config_manager import ConfigManager
 from data_validation.query_builder.random_row_builder import RandomRowBuilder
 from data_validation.schema_validation import SchemaValidation
 from data_validation.validation_builder import ValidationBuilder
@@ -106,24 +104,34 @@
         """Add random row filters to the validation builder."""
         if not self.config_manager.primary_keys:
             raise ValueError("Primary Keys are required for Random Row Filters")
 
         # Filter for only first primary key (multi-pk filter not supported)
         primary_key_info = self.config_manager.primary_keys[0]
 
-        query = RandomRowBuilder(
+        randomRowBuilder = RandomRowBuilder(
             [primary_key_info[consts.CONFIG_SOURCE_COLUMN]],
             self.config_manager.random_row_batch_size(),
-        ).compile(
-            self.config_manager.source_client,
-            self.config_manager.source_schema,
-            self.config_manager.source_table,
-            self.validation_builder.source_builder,
         )
 
+        if (self.config_manager.validation_type == consts.CUSTOM_QUERY) and (
+            self.config_manager.custom_query_type == consts.ROW_VALIDATION.lower()
+        ):
+            query = randomRowBuilder.compile_custom_query(
+                self.config_manager.source_client,
+                self.config_manager.source_query,
+            )
+        else:
+            query = randomRowBuilder.compile(
+                self.config_manager.source_client,
+                self.config_manager.source_schema,
+                self.config_manager.source_table,
+                self.validation_builder.source_builder,
+            )
+
         random_rows = self.config_manager.source_client.execute(query)
         if len(random_rows) == 0:
             return
         filter_field = {
             consts.CONFIG_TYPE: consts.FILTER_TYPE_ISIN,
             consts.CONFIG_FILTER_SOURCE_COLUMN: primary_key_info[
                 consts.CONFIG_SOURCE_COLUMN
@@ -251,51 +259,14 @@
                 consts.CONFIG_FILTER_TARGET_COLUMN: validation_builder.get_grouped_alias_target_column(
                     alias
                 ),
                 consts.CONFIG_FILTER_TARGET_VALUE: value,
             }
             validation_builder.add_filter(filter_field)
 
-    @classmethod
-    def _get_pandas_schema(
-        cls,
-        source_df: pandas.core.frame.DataFrame,
-        target_df: pandas.core.frame.DataFrame,
-        join_on_schema: dict,
-        verbose=False,
-    ):
-        """Return a pandas schema which aligns source and target for joins."""
-        for join_on_field in join_on_schema:
-            if isinstance(join_on_schema[join_on_field], (dt.Date, dt.Timestamp)):
-                # TODO(dhercher): We are experiencing issues around datetime coming as string
-                # and not matching. Currently the hack to cast it to string works, but is not ideal.
-                # We should look at both types, and if one is
-                # date-like than use pandas.to_datetime on the other.
-                source_df[join_on_field] = source_df[join_on_field].astype(str)
-                target_df[join_on_field] = target_df[join_on_field].astype(str)
-
-        # Loop over index keys() instead of iteritems() because pandas is
-        # failing with datetime64[ns, UTC] data type on Python 3.9.
-        schema_data = []
-        schema_index = []
-        for key in source_df.dtypes.keys():
-            dtype = source_df.dtypes[key]
-            # The Ibis pandas backend fails with `KeyError: dtype('O')` if
-            # object dtypes are passed in.
-            if dtype in {numpy.dtype("O")}:
-                continue
-            schema_data.append(dtype)
-            schema_index.append(key)
-        pd_schema = pandas.Series(schema_data, index=schema_index)
-        if verbose:
-            logging.info("-- ** Pandas Schema ** --")
-            logging.info(pd_schema)
-
-        return pd_schema
-
     def _execute_validation(self, validation_builder, process_in_memory=True):
         """Execute Against a Supplied Validation Builder"""
         self.run_metadata.validations = validation_builder.get_metadata()
 
         source_query = validation_builder.get_source_query()
         target_query = validation_builder.get_target_query()
 
@@ -331,29 +302,24 @@
                     executor.submit(
                         self.config_manager.target_client.execute, target_query
                     )
                 )
                 source_df = futures[0].result()
                 target_df = futures[1].result()
 
-            join_on_schema = {_: source_query.schema()[_] for _ in join_on_fields}
-            pd_schema = self._get_pandas_schema(
-                source_df, target_df, join_on_schema, verbose=self.verbose
-            )
-
-            pandas_client = ibis.backends.pandas.connect(
+            pandas_client = ibis.pandas.connect(
                 {combiner.DEFAULT_SOURCE: source_df, combiner.DEFAULT_TARGET: target_df}
             )
 
             try:
                 result_df = combiner.generate_report(
                     pandas_client,
                     self.run_metadata,
-                    pandas_client.table(combiner.DEFAULT_SOURCE, schema=pd_schema),
-                    pandas_client.table(combiner.DEFAULT_TARGET, schema=pd_schema),
+                    pandas_client.table(combiner.DEFAULT_SOURCE),
+                    pandas_client.table(combiner.DEFAULT_TARGET),
                     join_on_fields=join_on_fields,
                     is_value_comparison=is_value_comparison,
                     verbose=self.verbose,
                 )
             except Exception as e:
                 if self.verbose:
                     logging.error("-- ** Logging Source DF ** --")
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/jellyfish_distance.py` & `google-pso-data-validator-4.0.0/data_validation/jellyfish_distance.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.2.0/data_validation/metadata.py` & `google-pso-data-validator-4.0.0/data_validation/metadata.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.2.0/data_validation/query_builder/__init__.py` & `google-pso-data-validator-4.0.0/data_validation/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.2.0/data_validation/query_builder/partition_row_builder.py` & `google-pso-data-validator-4.0.0/data_validation/query_builder/partition_row_builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,58 +16,50 @@
 from data_validation import clients
 from data_validation.query_builder.query_builder import QueryBuilder
 
 
 class PartitionRowBuilder(object):
     def __init__(
         self,
-        partition_key: str,
-        data_client: ibis.client,
+        primary_keys: [str],
+        data_client: ibis.backends.base.BaseBackend,
         schema_name: str,
         table_name: str,
         query_builder: QueryBuilder,
     ) -> None:
         """Build a PartitionRowBuilder object which is ready to build a partition row filter query.
 
         Args:
-            partition_key (str): Partition key used to generate Partitions.
-            data_client (IbisClient): The client used to query random rows.
+            primary_keys [str]: Keys used to identify a row for validation
+            data_client (BaseBackend): The Backend used to query random rows.
             schema_name (String): The name of the schema for the given table.
             table_name (String): The name of the table to query.
             query_builder (QueryBuilder): QueryBuilder object.
         """
-        self.partition_key = partition_key
+        self.primary_keys = primary_keys
         self.query = self._compile_query(
             data_client, schema_name, table_name, query_builder
         )
 
     def _compile_query(
         self,
-        data_client: ibis.client,
+        data_client: ibis.backends.base.BaseBackend,
         schema_name: str,
         table_name: str,
         query_builder: QueryBuilder,
     ) -> ibis.Expr:
         """Return an Ibis query object
 
         Args:
-            data_client (IbisClient): The client used to query random rows.
+            data_client (BaseBackend): The Backend used to query random rows.
             schema_name (String): The name of the schema for the given table.
             table_name (String): The name of the table to query.
             query_builder (QueryBuilder): QueryBuilder object.
         """
         table = clients.get_ibis_table(data_client, schema_name, table_name)
         compiled_filters = query_builder.compile_filter_fields(table)
         filtered_table = table.filter(compiled_filters) if compiled_filters else table
         return filtered_table
 
-    def get_max_query(self) -> ibis.Expr:
-        """Return an Ibis query object to get Max of Primary Key column"""
-        return self.query[self.partition_key].max()
-
-    def get_min_query(self) -> ibis.Expr:
-        """Return an Ibis query object to get Min of Primary Key column"""
-        return self.query[self.partition_key].min()
-
-    def get_count_query(self) -> ibis.Expr:
-        """Return an Ibis query object to get count of Primary Key column"""
-        return self.query[self.partition_key].count()
+    def get_count(self) -> int:
+        """Return a count of rows of primary keys - they should be all distinct"""
+        return self.query[self.primary_keys].count().execute()
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/query_builder/query_builder.py` & `google-pso-data-validator-4.0.0/data_validation/query_builder/query_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,34 +276,34 @@
     @staticmethod
     def concat(config, fields):
         if config.get("default_concat_separator") is None:
             config["default_concat_separator"] = ibis.literal("")
         fields = [config["default_concat_separator"], fields]
         cast = "string"
         return CalculatedField(
-            ibis.expr.api.StringValue.join,
+            ibis.expr.types.StringValue.join,
             config,
             fields,
             cast=cast,
         )
 
     @staticmethod
     def hash(config, fields):
         if config.get("default_hash_function") is None:
             how = "sha256"
             return CalculatedField(
-                ibis.expr.api.StringValue.hashbytes,
+                ibis.expr.types.StringValue.hashbytes,
                 config,
                 fields,
                 how=how,
             )
         else:
             how = "farm_fingerprint"
             return CalculatedField(
-                ibis.expr.api.ValueExpr.hash,
+                ibis.expr.types.Value.hash,
                 config,
                 fields,
                 how=how,
             )
 
     @staticmethod
     def to_char(config, fields):
@@ -315,47 +315,47 @@
     @staticmethod
     def ifnull(config, fields):
         default_null_string = ibis.literal(
             config.get("default_null_string", "DEFAULT_REPLACEMENT_STRING")
         )
         fields = [fields[0], default_null_string]
         return CalculatedField(
-            ibis.expr.api.ValueExpr.fillna,
+            ibis.expr.types.Value.fillna,
             config,
             fields,
         )
 
     @staticmethod
     def length(config, fields):
         return CalculatedField(
-            ibis.expr.api.StringValue.length,
+            ibis.expr.types.StringValue.length,
             config,
             fields,
         )
 
     @staticmethod
     def rstrip(config, fields):
         return CalculatedField(
-            ibis.expr.api.StringValue.rstrip,
+            ibis.expr.types.StringValue.rstrip,
             config,
             fields,
         )
 
     @staticmethod
     def upper(config, fields):
         return CalculatedField(
-            ibis.expr.api.StringValue.upper,
+            ibis.expr.types.StringValue.upper,
             config,
             fields,
         )
 
     @staticmethod
     def epoch_seconds(config, fields):
         return CalculatedField(
-            ibis.expr.api.TimestampValue.epoch_seconds,
+            ibis.expr.types.TimestampValue.epoch_seconds,
             config,
             fields,
         )
 
     @staticmethod
     def cast(config, fields):
         target_type = config.get(consts.CONFIG_DEFAULT_CAST, "string")
@@ -491,23 +491,24 @@
             for n in range(0, (depth_limit + 1)):
                 table = table.mutate(self.compile_calculated_fields(table, n))
 
         if (
             validation_type == consts.ROW_VALIDATION
             or validation_type == consts.CUSTOM_QUERY
         ):
-            table = table.projection(self.compile_comparison_fields(table))
+            if self.comparison_fields:
+                table = table.projection(self.compile_comparison_fields(table))
         else:
             if self.comparison_fields:
                 table = table.mutate(self.compile_comparison_fields(table))
         compiled_filters = self.compile_filter_fields(table)
         filtered_table = table.filter(compiled_filters) if compiled_filters else table
         compiled_groups = self.compile_group_fields(filtered_table)
         grouped_table = (
-            filtered_table.groupby(compiled_groups)
+            filtered_table.group_by(compiled_groups)
             if compiled_groups
             else filtered_table
         )
         if self.aggregate_fields:
             query = grouped_table.aggregate(
                 self.compile_aggregate_fields(filtered_table)
             )
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/query_builder/random_row_builder.py` & `google-pso-data-validator-4.0.0/third_party/ibis/ibis_teradata/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,251 +1,245 @@
-# Copyright 2020 Google LLC
+# Copyright 2023 Google Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#      http://www.apache.org/licenses/LICENSE-2.0
+# http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import pandas
+import warnings
 
-import random
-import logging
-from typing import List
-from io import StringIO
-import sqlalchemy as sa
-import ibis
-import ibis.expr.operations as ops
-import ibis.expr.types as tz
-import ibis.expr.rules as rlz
-import ibis.backends.base_sqlalchemy.compiler as sql_compiler
-import ibis.backends.base_sqlalchemy.alchemy as sqla
-import ibis.backends.pandas.execution.util as pandas_util
-
-from ibis_bigquery import BigQueryClient
-from ibis.backends.impala.client import ImpalaClient
-from ibis.backends.pandas.client import PandasClient
-from ibis.backends.postgres.client import PostgreSQLClient
-from ibis.backends.mysql.client import MySQLClient
-from ibis.expr.signature import Argument as Arg
-from data_validation import clients
-from data_validation.query_builder.query_builder import QueryBuilder
-
-
-""" The QueryBuilder for retreiving random row values to filter against."""
-
-######################################
-### Adding new datasources should be
-### done by adding the Client and
-### syntax for random sorts in the
-### dict below. If upstream injection
-### is required, feel free to reach
-### out to dhercher
-######################################
-RANDOM_SORT_SUPPORTS = {
-    PandasClient: "NA",
-    BigQueryClient: "RAND()",
-    clients.TeradataClient: None,
-    ImpalaClient: "RAND()",
-    clients.OracleClient: "DBMS_RANDOM.VALUE",
-    PostgreSQLClient: "RANDOM()",
-    clients.MSSQLClient: "NEWID()",
-    clients.DB2Client: "RAND()",
-    MySQLClient: "RAND()",
-}
-
-
-class RandomSortExpr(tz.AnyValue, tz.SortExpr):
-    _dtype = rlz.string
-    _name = "RandomSortExpr"
-
-    def __init__(self, arg):
-        self._arg = arg
-
-    def type(self):
-        return self._dtype
-
-
-class RandomSortKey(ops.SortKey):
-    expr = Arg(rlz.any)
-    value = None
-
-    def equals(self, other, cache=None):
-        return isinstance(other, RandomSortKey)
-
-    def output_type(self):
-        return RandomSortExpr
-
-    def resolve_name(self):
-        return "RandomSortKey"
-
-
-class RandomRowBuilder(object):
-    def __init__(self, primary_keys: List[str], batch_size: int):
-        """Build a RandomRowBuilder object which is ready to build a random row filter query.
-
-        Args:
-            primary_keys: A list of primary key field strings used to find random rows.
-            batch_size: A max size for the number of random row values to find.
-        """
-        self.primary_keys = primary_keys
-        self.batch_size = batch_size
+import teradatasql
+import ibis.expr.datatypes as dt
+import ibis.expr.types as ir
+from typing import Mapping, Any
+import ibis.expr.schema as sch
+from ibis.backends.base.sql import BaseSQLBackend
+from third_party.ibis.ibis_teradata.compiler import TeradataCompiler
+from third_party.ibis.ibis_teradata.datatypes import (
+    TeradataTypeTranslator,
+    _teradatasql_to_ibis_type,
+)
+
+
+class Backend(BaseSQLBackend):
+    name = "teradata"
+    compiler = TeradataCompiler
+    NO_LOCK_SQL = "LOCKING ROW FOR ACCESS "
 
-    def compile(
+    def do_connect(
         self,
-        data_client: ibis.client,
-        schema_name: str,
-        table_name: str,
-        query_builder: QueryBuilder,
-    ) -> ibis.Expr:
-        """Return an Ibis query object
-
-        Args:
-            data_client (IbisClient): The client used to query random rows.
-            schema_name (String): The name of the schema for the given table.
-            table_name (String): The name of the table to query.
-        """
-        table = clients.get_ibis_table(data_client, schema_name, table_name)
-        compiled_filters = query_builder.compile_filter_fields(table)
-        filtered_table = table.filter(compiled_filters) if compiled_filters else table
-        randomly_sorted_table = self.maybe_add_random_sort(data_client, filtered_table)
-        query = randomly_sorted_table.limit(self.batch_size)[self.primary_keys]
-
-        return query
-
-    def maybe_add_random_sort(
-        self, data_client: ibis.client, table: ibis.Expr
-    ) -> ibis.Expr:
-        """Return a randomly sorted query if it is supported for the client."""
-        if type(data_client) in RANDOM_SORT_SUPPORTS:
-            # Teradata 'SAMPLE' is random by nature and does not require a sort by
-            if type(data_client) == clients.TeradataClient:
-                return table
-
-            return table.sort_by(
-                RandomSortKey(RANDOM_SORT_SUPPORTS[type(data_client)]).to_expr()
-            )
-
-        logging.warning(
-            "Data Client %s Does Not Enforce Random Sort on Sample",
-            str(type(data_client)),
-        )
-        return table
-
-
-##################################
-### Custom Pandas Client Logic ###
-##################################
-
-# Save old version to be wrapped
-_compute_sorted_frame = pandas_util.compute_sorted_frame
-
-
-class RandomColumn:
-    def __init__(self, name):
-        self._name = name
-
-    def op(self):
-        return self
-
-    def to_expr(self):
-        return self._name
-
-
-def build_and_assign_random_column(df, key, random_name):
-    if not isinstance(key.op(), RandomSortKey):
-        return key
-
-    random.shuffle(df.index.values)
-    df[random_name] = df.index.values
-    return RandomColumn(random_name)
+        host: str = "localhost",
+        user_name: str = None,
+        password: str = None,
+        port: int = 1025,
+        logmech: str = "TD2",
+        use_no_lock_tables: bool = False,
+    ) -> None:
+        self.teradata_config = {
+            "host": host,
+            "user": user_name,
+            "password": password,
+            "dbs_port": port,
+            "logmech": logmech,
+        }
+
+        self.client = teradatasql.connect(**self.teradata_config)
+        self.con = self.client.cursor()
+        self.use_no_lock_tables = use_no_lock_tables
+
+    def close(self):
+        """Close the connection."""
+        self.con.close()
+    
+    def __del__ (self):
+        self.con.close()
+
+    @property
+    def version(self):
+        return teradatasql.vernumber.sVersionNumber
+
+    LIST_DATABASE_SQL = """
+    SELECT * FROM DBC.Databases
+    WHERE DatabaseName LIKE '%{database_like}%'
+    """
+
+    def list_databases(self, like=None):
+        database_like = like or ""
+
+        list_database_sql = self.LIST_DATABASE_SQL.format(database_like=database_like)
+        databases_df = self._execute(list_database_sql, results=True)
+
+        return list(databases_df.DatabaseName.str.rstrip())
+
+    LIST_TABLE_SQL = """
+        SELECT * FROM DBC.Tables
+        WHERE DatabaseName LIKE '%{database_like}%'
+        AND TableName LIKE '%{table_like}%'
+    """
+
+    def list_tables(self, like=None, database=None):
+        database = database or ""
+        table = like or ""
 
+        list_table_sql = self.LIST_TABLE_SQL.format(
+            database_like=database, table_like=table
+        )
+        tables_df = self._execute(list_table_sql, results=True)
+        return list(tables_df.TableName.str.rstrip())
 
-def compute_sorted_frame(df, order_by, group_by=(), timecontext=None, **kwargs):
-    new_order_by = [
-        build_and_assign_random_column(df, key, f"__random_sort_{i}__")
-        for i, key in enumerate(order_by)
-    ]
-    sorted_results = _compute_sorted_frame(
-        df, new_order_by, group_by=group_by, timecontext=timecontext, **kwargs
-    )
+    def _fully_qualified_name(self, name, database):
+        if database:
+            return "{}.{}".format(database, name)
+        else:
+            return name
 
-    return sorted_results
+    def _breakdown_qualified_name(self, qualified_name):
+        database, table = qualified_name.split(".")
+        return database, table
+
+    def _get_table_schema(self, qualified_name):
+        dataset, table = self._breakdown_qualified_name(qualified_name)
+        return self.get_schema(table, database=dataset)
+
+    TABLE_SCHEMA_SQL = """
+    HELP COLUMN {qualified_name}.*;
+    """
+
+    def _get_teradata_schema(self, qualified_name):
+        query = self.TABLE_SCHEMA_SQL.format(qualified_name=qualified_name)
+        schema_df = self._execute(query, results=True)
+        schema_list = schema_df.to_dict("records")
+        schema = {}
+        for col_data in schema_list:
+            schema[
+                col_data["Column SQL Name"].rstrip()
+            ] = TeradataTypeTranslator.to_ibis(col_data)
+
+        return schema
+
+    def get_schema(self, table_name: str, database: str = None) -> sch.Schema:
+        """Return a Schema object for the indicated table and database.
+        Parameters
+        ----------
+        table_name
+            Table name
+        database
+            Database name
+        Returns
+        -------
+        Schema
+            Ibis schema
+        """
+        qualified_name = self._fully_qualified_name(table_name, database)
+        schema = self._get_teradata_schema(qualified_name)
+        return sch.Schema(schema)
+
+    def _get_schema_using_query(self, query):
+        cur = self.raw_sql(query)
+        # resets the state of the cursor and closes operation
+        cur.fetchall()
+        ibis_fields = self._adapt_types(cur.description)
+        return sch.Schema(ibis_fields)
+
+    def _adapt_types(self, descr):
+        names = []
+        adapted_types = []
+        for col in descr:
+            names.append(col[0])
+            teradata_typename = col[1]
+            typename = _teradatasql_to_ibis_type[teradata_typename]
+
+            if typename == "decimal":
+                precision, scale = col[4:6]
+                adapted_types.append(dt.Decimal(precision, scale))
+            else:
+                adapted_types.append(typename)
+        return dict(zip(names, adapted_types))
+
+    def _execute(self, sql, results=False):
+        if self.use_no_lock_tables and sql.strip().startswith("SELECT"):
+            sql = self.NO_LOCK_SQL + sql
+
+        with warnings.catch_warnings():
+            # Suppress pandas warning of SQLAlchemy connectable DB support
+            warnings.simplefilter("ignore")
+            df = pandas.read_sql(sql, self.client)
 
+        if results:
+            return df
 
-pandas_util.compute_sorted_frame = compute_sorted_frame
+        return None
 
+    def execute(
+        self,
+        expr: ir.Expr,
+        params: Mapping[ir.Scalar, Any] = None,
+        limit: str = "default",
+        **kwargs: Any,
+    ):
+        """Compile and execute an Ibis expression.
+        Compile and execute Ibis expression using this backend client
+        interface, returning results in-memory in the appropriate object type
+        Parameters
+        ----------
+        expr
+            Ibis expression
+        limit
+            For expressions yielding result sets; retrieve at most this number
+            of values/rows. Overrides any limit already set on the expression.
+        params
+            Named unbound parameters
+        kwargs
+            Backend specific arguments. For example, the clickhouse backend
+            uses this to receive `external_tables` as a dictionary of pandas
+            DataFrames.
+        Returns
+        -------
+        DataFrame | Series | Scalar
+            * `Table`: pandas.DataFrame
+            * `Column`: pandas.Series
+            * `Scalar`: Python scalar value
+        """
+        # Overwrite the execute() function to use read_sql method
+        kwargs.pop("timecontext", None)
+        query_ast = self.compiler.to_ast_ensure_limit(expr, limit, params=params)
+        sql = query_ast.compile()
+        self._log(sql)
 
-#####################################
-##### Override Order By for SQL #####
-#####################################
+        schema = self.ast_schema(query_ast, **kwargs)
 
+        self._register_in_memory_tables(expr)
 
-def format_order_by(self):
-    if not self.order_by:
-        return None
+        if self.use_no_lock_tables and sql.strip().startswith("SELECT"):
+            sql = self.NO_LOCK_SQL + self.compiled_sql
 
-    buf = StringIO()
-    buf.write("ORDER BY ")
+        with warnings.catch_warnings():
+            # Suppress pandas warning of SQLAlchemy connectable DB support
+            warnings.simplefilter("ignore")
+            df = pandas.read_sql(sql, self.client)
+        return df
 
-    formatted = []
-    for expr in self.order_by:
-        ##### ADDING CODE TO FORMAT #####
-        if isinstance(expr, RandomSortExpr):
-            literal_sql = expr.op().expr.op()
-            formatted.append(literal_sql.value)
-            continue
-        ##### END ADDING CODE TO FORMAT #####
-
-        key = expr.op()
-        translated = self._translate(key.expr)
-        if not key.ascending:
-            translated += " DESC"
-        formatted.append(translated)
-
-    buf.write(", ".join(formatted))
-    return buf.getvalue()
-
-
-sql_compiler.Select.format_order_by = format_order_by
-
-#######################################
-##### Override Order By for SQL Alchemy
-#######################################
-
-
-def _add_order_by(self, fragment):
-    if not len(self.order_by):
-        return fragment
-
-    clauses = []
-    for expr in self.order_by:
-        key = expr.op()
-        sort_expr = key.expr
-
-        ##### ADDING CODE TO FORMAT #####
-        if isinstance(expr, RandomSortExpr):
-            arg = sa.sql.literal_column(sort_expr.op().value)
-            clauses.append(arg)
-            continue
-        ##### END ADDING CODE TO FORMAT #####
-
-        # here we have to determine if key.expr is in the select set (as it
-        # will be in the case of order_by fused with an aggregation
-        if sqla._can_lower_sort_column(self.table_set, sort_expr):
-            arg = sort_expr.get_name()
-        else:
-            arg = self._translate(sort_expr)
+    # Methods we need to implement for BaseSQLBackend
+    def create_table(self):
+        pass
 
-        if not key.ascending:
-            arg = sa.desc(arg)
+    def create_view(self):
+        pass
 
-        clauses.append(arg)
+    def current_database(self):
+        pass
 
-    return fragment.order_by(*clauses)
+    def drop_table(self):
+        pass
 
+    def drop_view(self):
+        pass
 
-sqla.AlchemySelect._add_order_by = _add_order_by
+    def fetch_from_cursor(self, cursor, schema):
+        pass
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/result_handlers/bigquery.py` & `google-pso-data-validator-4.0.0/data_validation/result_handlers/bigquery.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.2.0/data_validation/result_handlers/text.py` & `google-pso-data-validator-4.0.0/data_validation/result_handlers/text.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,34 +32,35 @@
     def __init__(
         self, format, status_list=None, cols_filter_list=consts.COLUMN_FILTER_LIST
     ):
         self.format = format
         self.cols_filter_list = cols_filter_list
         self.status_list = status_list
 
+    def _get_formatted(self, result_df):
+        if self.format == "text":
+            return result_df.drop(self.cols_filter_list, axis=1).to_string(index=False)
+        elif self.format == "csv":
+            return result_df.to_csv(index=False)
+        elif self.format == "json":
+            return result_df.to_json(orient="index")
+        else:
+            return result_df.drop(self.cols_filter_list, axis=1).to_markdown(
+                tablefmt="fancy_grid", index=False
+            )
+
     def print_formatted_(self, result_df):
         """
         Utility for printing formatted results
         :param result_df
         """
         if self.status_list is not None:
             result_df = filter_validation_status(self.status_list, result_df)
 
-        if self.format == "text":
-            print(result_df.drop(self.cols_filter_list, axis=1).to_string(index=False))
-        elif self.format == "csv":
-            print(result_df.drop(self.cols_filter_list, axis=1).to_csv(index=False))
-        elif self.format == "json":
-            print(result_df.drop(self.cols_filter_list, axis=1).to_json(orient="index"))
-        else:
-            print(
-                result_df.drop(self.cols_filter_list, axis=1).to_markdown(
-                    tablefmt="fancy_grid", index=False
-                )
-            )
+        print(self._get_formatted(result_df))
 
         if self.format not in consts.FORMAT_TYPES:
             error_msg = (
                 f"format [{self.format}] not supported, results printed in default(table) mode. "
                 f"Supported formats are [text, csv, json, table]"
             )
             raise ValueError(error_msg)
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/secret_manager.py` & `google-pso-data-validator-4.0.0/data_validation/secret_manager.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.2.0/data_validation/state_manager.py` & `google-pso-data-validator-4.0.0/data_validation/state_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,17 @@
         file_names = self._list_directory(self._get_connections_directory())
         return [
             file_name.rsplit(".", 2)[0]
             for file_name in file_names
             if file_name.endswith(".connection.json")
         ]
 
+    def read_file(self, file_path: str) -> str:
+        return self._read_file(file_path)
+
     def _get_connections_directory(self) -> str:
         """Returns the connections directory path."""
         if self.file_system == FileSystem.LOCAL:
             return self.file_system_root_path
 
         return os.path.join(self.file_system_root_path, "connections/")
 
@@ -180,15 +183,16 @@
             return os.path.join("./", name)
         return name
 
     def _read_file(self, file_path: str) -> str:
         if self.file_system == FileSystem.GCS:
             return self._read_gcs_file(file_path)
         else:
-            return open(file_path, "r").read()
+            with open(file_path, "r") as f:
+                return f.read()
 
     def _write_file(self, file_path: str, data: str):
         if self.file_system == FileSystem.GCS:
             self._write_gcs_file(file_path, data)
         else:
             with open(file_path, "w") as file:
                 file.write(data)
@@ -238,15 +242,16 @@
 
     def _get_gcs_file_path(self, gcs_file_path: str):
         return str.join("", gcs_file_path[5:].split("/", 1)[1:])
 
     def _read_gcs_file(self, file_path: str) -> str:
         gcs_file_path = self._get_gcs_file_path(file_path)
         blob = self.gcs_bucket.get_blob(gcs_file_path)
-
+        if not blob:
+            raise ValueError(f"Invalid Cloud Storage Path: {file_path}")
         return blob.download_as_bytes()
 
     def _write_gcs_file(self, file_path: str, data: str):
         gcs_file_path = self._get_gcs_file_path(file_path)
         blob = self.gcs_bucket.blob(gcs_file_path)
         blob.upload_from_string(data)
```

### Comparing `google-pso-data-validator-3.2.0/data_validation/validation_builder.py` & `google-pso-data-validator-4.0.0/data_validation/validation_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/PKG-INFO` & `google-pso-data-validator-4.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: google-pso-data-validator
-Version: 3.2.0
-Summary: A package to enable easy data validation
-Home-page: https://github.com/pypa/sampleproject
-Author: Dylan Hercher
-Author-email: dhercher@google.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: apache-airflow
-Provides-Extra: pyspark
-License-File: LICENSE
-
 # Data Validation Tool
 
 The Data Validation Tool is an open sourced Python CLI tool based on the
 [Ibis framework](https://ibis-project.org/docs/)
 that compares heterogeneous data source tables with multi-leveled validation
 functions.
 
@@ -30,40 +10,41 @@
 compared to ensure they are matched and correct after each migration step
 (e.g. data and schema migration, SQL script translation, ETL migration, etc.).
 The Data Validation Tool (DVT) provides an automated and repeatable solution to
 perform this task.
 
 DVT supports the following validations:
 * Column validation (count, sum, avg, min, max, group by)
-* Row validation (BQ, Hive, Teradata, Oracle, SQL Server, Postgres, Mysql only)
-* Schema validation 
+* Row validation (Not supported for FileSystem connections)
+* Schema validation
 * Custom Query validation
 * Ad hoc SQL exploration
 
 DVT supports the following connection types:
 
+*   [AlloyDB](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#alloydb)
 *   [BigQuery](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#google-bigquery)
 *   [DB2](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#db2)
 *   [FileSystem](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#filesystem)
 *   [Hive](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#hive)
 *   [Impala](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#impala)
 *   [MSSQL](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#mssql-server)
 *   [MySQL](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#mysql)
 *   [Oracle](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#oracle)
 *   [Postgres](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#postgres)
 *   [Redshift](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#redshift)
 *   [Spanner](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#google-spanner)
 *   [Teradata](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#teradata)
-*   [AlloyDB](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#alloydb)
+*   [Snowflake](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#snowflake)
 
 The [Connections](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md) page provides details about how to create
 and list connections for the validation tool.
 
 ### Disclaimer
-This is not an officially supported Google product. Please be aware that bugs may lurk, and that we reserve the right to make small backwards-incompatible changes. Feel free to open bugs or feature requests, or contribute directly 
+This is not an officially supported Google product. Please be aware that bugs may lurk, and that we reserve the right to make small backwards-incompatible changes. Feel free to open bugs or feature requests, or contribute directly
 (see [CONTRIBUTING.md](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/CONTRIBUTING.md) for details).
 
 ## Installation
 
 The [Installation](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/installation.md) page describes the prerequisites and
 setup steps needed to install and use the Data Validation Tool.
 
@@ -94,15 +75,15 @@
 
 #### Column Validations
 
 Below is the command syntax for column validations. To run a grouped column
 validation, simply specify the `--grouped-columns` flag.
 
 You can specify a list of string columns for aggregations in order to calculate
-an aggregation over the `length(string_col)`. Running an aggregation 
+an aggregation over the `length(string_col)`. Running an aggregation
 over all columns ('*') will only run over numeric columns, unless the
 `--wildcard-include-string-len` flag is present.
 
 ```
 data-validation (--verbose or -v) (--log-level or -ll) validate column
   --source-conn or -sc SOURCE_CONN
                         Source connection details
@@ -114,15 +95,15 @@
                         Comma separated list of tables in the form schema.table=target_schema.target_table
                         Target schema name and table name are optional.
                         i.e 'bigquery-public-data.new_york_citibike.citibike_trips'
   [--grouped-columns or -gc GROUPED_COLUMNS]
                         Comma separated list of columns for Group By i.e col_a,col_b
   [--primary-keys or -pk PRIMARY_KEYS]
                         Comma separated list of columns to use as primary keys
-                        (Note) Only use with grouped column validation
+                        (Note) Only use with grouped column validation. See *Primary Keys* section. 
   [--count COLUMNS]     Comma separated list of columns for count or * for all columns
   [--sum COLUMNS]       Comma separated list of columns for sum or * for all numeric
   [--min COLUMNS]       Comma separated list of columns for min or * for all numeric
   [--max COLUMNS]       Comma separated list of columns for max or * for all numeric
   [--avg COLUMNS]       Comma separated list of columns for avg or * for all numeric
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
@@ -152,23 +133,23 @@
 The default aggregation type is a 'COUNT *'. If no aggregation flag (i.e count,
 sum , min, etc.) is provided, the default aggregation will run.
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md) page provides many examples of how a tool can be used to run powerful validations without writing any queries.
 
 #### Row Validations
 
-(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Redshift, Postgres, Mysql, Db2 and Alloy DB. Struct and array data types are not currently supported.
-In addition, please note that SHA256 is not a supported function on Teradata systems. 
-If you wish to perform this comparison on Teradata you will need to 
+(Note: Row hash validation not supported for FileSystem connections. 
+In addition, please note that SHA256 is not a supported function on Teradata systems.
+If you wish to perform this comparison on Teradata you will need to
 [deploy a UDF to perform the conversion](https://github.com/akuroda/teradata-udf-sha2/blob/master/src/sha256.c).)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass a `--primary-key` flag which defines what field(s)
 the validation will be compared on, as well as either the `--comparison-fields` flag
-or the `--hash` flag.
+or the `--hash` flag. See *Primary Keys* section
 
 The `--comparison-fields` flag specifies the values (e.g. columns) whose raw values will be compared
 based on the primary key join. The `--hash` flag will run a checksum across specified columns in
 the table. This will include casting to string, sanitizing the data (ifnull, rtrim, upper), concatenating,
 and finally hashing the row.
 
 
@@ -185,19 +166,19 @@
                         Target connection details
                         See: *Connections* section for each data source
   --tables-list or -tbls SOURCE_SCHEMA.SOURCE_TABLE=TARGET_SCHEMA.TARGET_TABLE
                         Comma separated list of tables in the form schema.table=target_schema.target_table
                         Target schema name and table name are optional.
                         i.e 'bigquery-public-data.new_york_citibike.citibike_trips'
   --primary-keys or -pk PRIMARY_KEYS
-                        Comma separated list of columns to use as primary keys
+                        Comma separated list of columns to use as primary keys.  See *Primary Keys* section
   --comparison-fields or -comp-fields FIELDS
                         Comma separated list of columns to compare. Can either be a physical column or an alias
                         See: *Calculated Fields* section for details
-  --hash COLUMNS        Comma separated list of columns to hash or * for all columns 
+  --hash COLUMNS        Comma separated list of columns to hash or * for all columns
   --concat COLUMNS      Comma separated list of columns to concatenate or * for all columns (use if a common hash function is not available between databases)
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--filters SOURCE_FILTER:TARGET_FILTER]
@@ -215,21 +196,21 @@
   [--random-row-batch-size or -rbs]
                         Row batch size used for random row filters (default 10,000).
   [--filter-status or -fs STATUSES_LIST]
                         Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail). If no list is provided, all statuses are returned.
 ```
 #### Generate Table Partitions for Large Table Row Validations
 
-Below is the command syntax for generating table partitions in order to perform row validations on large tables with memory constraints. 
+(Note: This is only supported for Oracle and Postgres connections.)
 
-The command generates and stores multiple YAML configs that represent chunks of the large table using filters (`WHERE partition_key > X AND partition_key < Y`). You can then run the configs in the directory serially with the `data-validation configs run --config-dir PATH` command as described [here](https://github.com/GoogleCloudPlatform/professional-services-data-validator#yaml-configuration-files).
+When performing row validations, Data Validation Tool brings each row into memory and can run into MemoryError. Below is the command syntax for generating table partitions in order to perform row validations on large tables to alleviate MemoryError. Each partition contains a range of primary key(s) and the ranges of keys across partitions are distinct. The partitions have nearly equal number of rows. See *Primary Keys* section
 
-The command takes the same parameters as required for `Row Validation` *plus* few commands to implement the partitioning logic.
+The command generates and stores multiple YAML configs that represent chunks of the large table using filters (`WHERE primary_key(s) >= X AND primary_key(s) < Y`). You can then run the configs in the directory serially (or in parallel in multiple containers, VMs) with the `data-validation configs run --config-dir PATH` command as described [here](https://github.com/GoogleCloudPlatform/professional-services-data-validator#yaml-configuration-files).
 
-(Note: As of now, only monotonically increasing key is supported for `--partition-key`.)
+The command takes the same parameters as required for `Row Validation` *plus* a few parameters to support partitioning. Single and multiple primary keys are supported and keys can be of any indexable type. A parameter used in earlier versions, ```partition-key``` is no longer supported. 
 
 ```
 data-validation (--verbose or -v) (--log-level or -ll) generate-table-partitions
 
   --source-conn or -sc SOURCE_CONN
                         Source connection details
                         See: *Data Source Configurations* section for each data source
@@ -237,67 +218,71 @@
                         Target connection details
                         See: *Connections* section for each data source
   --tables-list or -tbls SOURCE_SCHEMA.SOURCE_TABLE=TARGET_SCHEMA.TARGET_TABLE
                         Comma separated list of tables in the form schema.table=target_schema.target_table
                         Target schema name and table name are optional.
                         i.e 'bigquery-public-data.new_york_citibike.citibike_trips'
   --primary-keys PRIMARY_KEYS, -pk PRIMARY_KEYS
-                        Comma separated list of primary key columns 'col_a,col_b'
+                        Comma separated list of primary key columns 'col_a,col_b'.  See *Primary Keys* section
   --comparison-fields or -comp-fields FIELDS
                         Comma separated list of columns to compare. Can either be a physical column or an alias
                         See: *Calculated Fields* section for details
-  --hash COLUMNS        Comma separated list of columns to hash or * for all columns 
+  --hash COLUMNS        Comma separated list of columns to hash or * for all columns
   --concat COLUMNS      Comma separated list of columns to concatenate or * for all columns (use if a common hash function is not available between databases)
   --config-dir CONFIG_DIR, -cdir CONFIG_DIR
                         Directory Path to store YAML Config Files
                         GCS: Provide a full gs:// path of the target directory. Eg: `gs://<BUCKET>/partitions_dir`
                         Local: Provide a relative path of the target directory. Eg: `partitions_dir`
   --partition-num [1-1000], -pn [1-1000]
                         Number of partitions/config files to generate
                         In case this value exceeds the row count of the source/target table, it will be decreased to max(source_row_count, target_row_count)
-  [--partition-key PARTITION_KEY, -partkey PARTITION_KEY]
-                        Column on which the partitions would be generated. Column type must be integer. Defaults to Primary key
   [--filters SOURCE_FILTER:TARGET_FILTER]
                         Colon separated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
 ```
 #### Schema Validations
 
 Below is the syntax for schema validations. These can be used to compare case insensitive column names and
 types between source and target.
 
+Note: An exclamation point before a data type (`!string`) signifies the column is non-nullable or required.
+
 ```
 data-validation (--verbose or -v) (--log-level or -ll) validate schema
   --source-conn or -sc SOURCE_CONN
                         Source connection details
                         See: *Data Source Configurations* section for each data source
   --target-conn or -tc TARGET_CONN
                         Target connection details
                         See: *Connections* section for each data source
   --tables-list or -tbls SOURCE_SCHEMA.SOURCE_TABLE=TARGET_SCHEMA.TARGET_TABLE
                         Comma separated list of tables in the form schema.table=target_schema.target_table
                         Target schema name and table name are optional.
-                        i.e 'bigquery-public-data.new_york_citibike.citibike_trips'
+                        e.g.: 'bigquery-public-data.new_york_citibike.citibike_trips'
   [--bq-result-handler or -bqrh PROJECT_ID.DATASET.TABLE]
                         BigQuery destination for validation results. Defaults to stdout.
                         See: *Validation Reports* section
   [--service-account or -sa PATH_TO_SA_KEY]
                         Service account to use for BigQuery result handler output.
   [--config-file or -c CONFIG_FILE]
                         YAML Config File Path to be used for storing validations.
   [--format or -fmt]    Format for stdout output. Supported formats are (text, csv, json, table).
                         Defaults  to table.
   [--filter-status or -fs STATUSES_LIST]
-                        Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail). If no list is provided, all statuses are returned.
+                        Comma separated list of statuses to filter the validation results. Supported statuses are (success, fail).
+                        If no list is provided, all statuses are returned.
   [--exclusion-columns or -ec EXCLUSION_COLUMNS]
-                        Comma separated list of columns to be excluded from the schema validation, i.e col_a,col_b.
-
+                        Comma separated list of columns to be excluded from the schema validation, e.g.: col_a,col_b.
   [--allow-list or -al ALLOW_LIST]
-                        Comma separated list of data-type mappings of source and destination data sources which will be validated in case of missing data types in destination data source. e.g: "decimal(4,2):decimal(5,4),string[non-nullable]:string"                 
+                        Comma separated list of data-type mappings of source and destination data sources which will be validated in case of missing data types in destination data source. e.g: "decimal(4,2):decimal(5,4),!string:string"
+  [--allow-list-file ALLOW_LIST_FILE, -alf ALLOW_LIST_FILE]
+                        YAML file containing default --allow-list mappings. Can be used in conjunction with --allow-list.
+                        e.g.: samples/allow_list/oracle_to_bigquery.yaml or gs://dvt-allow-list-files/oracle_to_bigquery.yaml
+                        See example files in samples/allow_list/.
 ```
 
 #### Custom Query Column Validations
 
 Below is the command syntax for custom query column validations.
 
 ```
@@ -339,22 +324,22 @@
 The default aggregation type is a 'COUNT *'. If no aggregation flag (i.e count,
 sum , min, etc.) is provided, the default aggregation will run.
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md)
 page provides few examples of how this tool can be used to run custom query validations.
 
 
-#### Custom Query Row Validations 
+#### Custom Query Row Validations
 
-(Note: Custom query row validation is currently only supported for BigQuery, Teradata, SQL Server, PostgreSQL, Oracle, Redshift, DB2, AlloyDB, and Impala/Hive. Struct and array data types are not currently supported.)
+(Note: Custom query row validation is not supported for FileSystem connections. Struct and array data types are not currently supported.)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass `--hash` flag which will specify the fields
 of the custom query result that will be concatenated and hashed. The primary key should be included
-in the SELECT statement of both source_query.sql and target_query.sql
+in the SELECT statement of both source_query.sql and target_query.sql.  See *Primary Keys* section
 
 Below is the command syntax for custom query row validations.
 
 ```
 data-validation (--verbose or -v) (--log-level or -ll) validate custom-query row
   --source-conn or -sc SOURCE_CONN
                         Source connection details
@@ -425,18 +410,18 @@
 
 You can customize the configuration for any given validation by providing use
 case specific CLI arguments or editing the YAML configuration file.
 
 For example, the following command creates a YAML file for the validation of the
 `new_york_citibike` table: `data-validation validate column -sc my_bq_conn -tc
 my_bq_conn -tbls bigquery-public-data.new_york_citibike.citibike_trips -c
-citibike.yaml`. 
+citibike.yaml`.
 
 The vaildation config file is saved to the GCS path specified by the `PSO_DV_CONFIG_HOME`
-env variable if that has been set; otherwise, it is saved to wherever the tool is run. 
+env variable if that has been set; otherwise, it is saved to wherever the tool is run.
 
 You can now edit the YAML file if, for example, the `new_york_citibike` table is
 stored in datasets that have different names in the source and target systems.
 Once the file is updated and saved, the following command runs the
 validation:
 
 ```
@@ -451,21 +436,21 @@
 
 data-validation configs run -cdir gs://my-bucket/my-validations/
 ```
 
 View the complete YAML file for a Grouped Column validation on the
 [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-yaml-config-grouped-column-validation) page.
 
-You can view a list of all saved validation YAML files using `data-validation configs list`, and print a YAML config using `data-validation configs get -c citibike.yaml`. 
+You can view a list of all saved validation YAML files using `data-validation configs list`, and print a YAML config using `data-validation configs get -c citibike.yaml`.
 
 ### Validation Reports
 
 The result handlers tell DVT where to store the results of
 each validation. The tool can write the results of a validation run to Google
-BigQuery or print to stdout (default). View the schema of the results 
+BigQuery or print to stdout (default). View the schema of the results
 table [here](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/terraform/results_schema.json).
 
 To output to BigQuery, simply include the `-bqrh` flag during a validation run
 like so:
 ```
 data-validation validate column
   -sc bq_conn
@@ -563,14 +548,20 @@
 written in the syntax of the given source.
 
 Note that you are writing the query to execute, which does not have to match
 between source and target as long as the results can be expected to align. If
 the target filter is omitted, the source filter will run on both the source and
 target tables.
 
+### Primary Keys
+
+In many cases, validations (e.g. count, min, max etc) produce one row per table. The comparison between the source
+and target table is to compare the value for each column in the source with the value of the column in the target.
+`grouped-columns` validation and `validate row` produce multiple rows per table. Data Validation Tool needs one or more columns to uniquely identify each row so the source and target can be compared. Data Validation Tool refers to these columns as primary keys. These do not need to be primary keys in the table. The only requirement is that the keys uniquely identify the row in the results.
+
 ### Grouped Columns
 
 Grouped Columns contain the fields you want your aggregations to be broken out
 by, e.g. `SELECT last_updated::DATE, COUNT(*) FROM my.table` will produce a
 resultset that breaks down the count of rows per calendar date.
 
 ### Hash, Concat, and Comparison Fields
@@ -639,43 +630,43 @@
   FROM my.table
   ) as table_0
 ```
 
 If you generate the config file for a row validation, you can see that it uses
 calculated fields to generate the query. You can also use calculated fields
 in column level validations to generate the length of a string, or cast
-a INT field to BIGINT for aggregations. 
+a INT field to BIGINT for aggregations.
 
 See the [Examples page](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-yaml-with-calc-fields-cast-to-numeric-before-aggregation) for a sample
 cast to NUMERIC.
 
 #### Custom Calculated Fields
 
 DVT supports certain functions required for row hash validation natively (i.e. CAST() and CONCAT()),
 which are listed in the CalculatedField() class methods in the [QueryBuilder](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/data_validation/query_builder/query_builder.py).
 
 You can also specify custom functions (i.e. replace() or truncate()) from the Ibis expression
-[API reference](https://ibis-project.org/docs/3.2.0/api/expressions/). Keep in mind these will run
+[API reference](https://ibis-project.org/reference/expressions/generic/). Keep in mind these will run
 on both source and target systems. You will need to specify the Ibis API expression and the parameters
 required, if any, with the 'params' block as shown below:
 
 ```yaml
 - calculated_fields:
   - depth: 0
     field_alias: format_start_time
     source_calculated_columns:
     - start_time
     target_calculated_columns:
     - start_time
     type: custom
-    ibis_expr: ibis.expr.api.TimestampValue.strftime
+    ibis_expr: ibis.expr.types.TemporalValue.strftime
     params:
     - format_str: '%m%d%Y'
 ```
 
-The above block references the [TimestampValue.strftime](https://ibis-project.org/docs/3.2.0/api/expressions/timestamps/#ibis.expr.types.temporal.TemporalValue.strftime) Ibis API expression.
+The above block references the [TemporalValue.strftime](https://ibis-project.org/reference/expressions/timestamps/#ibis.expr.types.temporal.TemporalValue.strftime) Ibis API expression.
 See the [Examples page](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md#sample-row-validation-yaml-with-custom-calc-field)
 for a sample YAML with a custom calculated field.
 
 ## Contributing
 
 Contributions are welcome. See the [Contributing guide](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/CONTRIBUTING.md) for details.
```

### Comparing `google-pso-data-validator-3.2.0/google_pso_data_validator.egg-info/SOURCES.txt` & `google-pso-data-validator-4.0.0/google_pso_data_validator.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -29,62 +29,51 @@
 data_validation/result_handlers/text.py
 google_pso_data_validator.egg-info/PKG-INFO
 google_pso_data_validator.egg-info/SOURCES.txt
 google_pso_data_validator.egg-info/dependency_links.txt
 google_pso_data_validator.egg-info/entry_points.txt
 google_pso_data_validator.egg-info/requires.txt
 google_pso_data_validator.egg-info/top_level.txt
-third_party/ibis/ibis_DB2/__init__.py
-third_party/ibis/ibis_DB2/alchemy.py
-third_party/ibis/ibis_DB2/api.py
-third_party/ibis/ibis_DB2/client.py
-third_party/ibis/ibis_DB2/compiler.py
-third_party/ibis/ibis_DB2/expr/__init__.py
-third_party/ibis/ibis_DB2/expr/datatypes.py
-third_party/ibis/ibis_DB2/expr/types.py
 third_party/ibis/ibis_addon/__init__.py
 third_party/ibis/ibis_addon/api.py
-third_party/ibis/ibis_addon/datatypes.py
 third_party/ibis/ibis_addon/operations.py
-third_party/ibis/ibis_addon/base_sqlalchemy/__init__.py
-third_party/ibis/ibis_addon/base_sqlalchemy/alchemy.py
 third_party/ibis/ibis_cloud_spanner/__init__.py
 third_party/ibis/ibis_cloud_spanner/api.py
 third_party/ibis/ibis_cloud_spanner/client.py
 third_party/ibis/ibis_cloud_spanner/compiler.py
 third_party/ibis/ibis_cloud_spanner/datatypes.py
-third_party/ibis/ibis_cloud_spanner/table.py
+third_party/ibis/ibis_cloud_spanner/registry.py
 third_party/ibis/ibis_cloud_spanner/to_pandas.py
 third_party/ibis/ibis_cloud_spanner/tests/__init__.py
 third_party/ibis/ibis_cloud_spanner/tests/conftest.py
-third_party/ibis/ibis_cloud_spanner/tests/test_client.py
-third_party/ibis/ibis_cloud_spanner/tests/test_compiler.py
-third_party/ibis/ibis_cloud_spanner/tests/test_datatypes.py
+third_party/ibis/ibis_db2/__init__.py
+third_party/ibis/ibis_db2/api.py
+third_party/ibis/ibis_db2/compiler.py
+third_party/ibis/ibis_db2/datatypes.py
+third_party/ibis/ibis_db2/registry.py
 third_party/ibis/ibis_impala/__init__.py
 third_party/ibis/ibis_impala/api.py
 third_party/ibis/ibis_mssql/__init__.py
 third_party/ibis/ibis_mssql/api.py
-third_party/ibis/ibis_mssql/client.py
-third_party/ibis/ibis_mssql/compiler.py
-third_party/ibis/ibis_mssql/expr/__init__.py
-third_party/ibis/ibis_mssql/expr/api.py
-third_party/ibis/ibis_mssql/expr/operations.py
+third_party/ibis/ibis_mssql/datatypes.py
+third_party/ibis/ibis_mysql/__init__.py
+third_party/ibis/ibis_mysql/compiler.py
+third_party/ibis/ibis_mysql/base_sql_compiler/__init__.py
+third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py
 third_party/ibis/ibis_oracle/__init__.py
-third_party/ibis/ibis_oracle/alchemy.py
 third_party/ibis/ibis_oracle/api.py
-third_party/ibis/ibis_oracle/client.py
 third_party/ibis/ibis_oracle/compiler.py
-third_party/ibis/ibis_oracle/expr/__init__.py
-third_party/ibis/ibis_oracle/expr/datatypes.py
-third_party/ibis/ibis_oracle/expr/types.py
-third_party/ibis/ibis_oracle/udf/__init__.py
-third_party/ibis/ibis_oracle/udf/api.py
+third_party/ibis/ibis_oracle/datatypes.py
+third_party/ibis/ibis_oracle/registry.py
 third_party/ibis/ibis_postgres/__init__.py
 third_party/ibis/ibis_postgres/client.py
 third_party/ibis/ibis_redshift/__init__.py
-third_party/ibis/ibis_redshift/client.py
+third_party/ibis/ibis_redshift/api.py
 third_party/ibis/ibis_redshift/compiler.py
+third_party/ibis/ibis_snowflake/__init__.py
+third_party/ibis/ibis_snowflake/api.py
+third_party/ibis/ibis_snowflake/datatypes.py
 third_party/ibis/ibis_teradata/__init__.py
 third_party/ibis/ibis_teradata/api.py
-third_party/ibis/ibis_teradata/client.py
 third_party/ibis/ibis_teradata/compiler.py
-third_party/ibis/ibis_teradata/datatypes.py
+third_party/ibis/ibis_teradata/datatypes.py
+third_party/ibis/ibis_teradata/registry.py
```

### Comparing `google-pso-data-validator-3.2.0/setup.py` & `google-pso-data-validator-4.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,48 +14,48 @@
 
 import os
 
 import setuptools
 
 name = "google-pso-data-validator"
 description = "A package to enable easy data validation"
-version = "3.2.0"
+version = "4.0.0"
 release_status = "Development Status :: 3 - Alpha"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 dependencies = [
     # Dependency corrections from our requirements
-    "attrs==20.3.0",
-    "grpcio==1.47.0",
-    "lazy-object-proxy==1.7.1",
-    "marshmallow==3.10.0",
+    "attrs==23.1.0",
+    "grpcio==1.53.0",
+    "lazy-object-proxy==1.9.0",
+    "marshmallow==3.19.0",
     # Core dependencies
-    "google-api-python-client==1.12.8",
-    "ibis-framework==1.4.0",
-    "ibis-bigquery==1.0.0",
-    "impyla==0.17.0",
-    "SQLAlchemy==1.3.22",
-    "PyMySQL==1.0.2",
-    "psycopg2-binary==2.9.3",
+    "fsspec>=2022.8.2",
+    "google-api-python-client==2.91.0",
+    "ibis-framework==5.1.0",
+    "impyla==0.18.0",
+    "SQLAlchemy==1.4.49",
+    "PyMySQL==1.1.0",
+    "psycopg2-binary==2.9.6",
     "PyYAML==6.0",
-    "pandas==1.3.5",
-    "proto-plus==1.13.0",
-    "pyarrow==6.0.1",
-    "pydata-google-auth==1.1.0",
-    "google-cloud-bigquery==2.30.0",
-    "google-cloud-bigquery-storage==2.3.0",
-    "google-cloud-spanner==3.1.0",
-    "google-cloud-storage==1.42.2",
+    "pandas==1.5.3",
+    "proto-plus==1.22.3",
+    "pyarrow==10.0.1",
+    "pydata-google-auth==1.8.0",
+    "google-cloud-bigquery==3.11.3",
+    "google-cloud-bigquery-storage==2.20.0",
+    "google-cloud-spanner==3.36.0",
+    "google-cloud-storage==2.10.0",
     "setuptools>=34.0.0",
-    "jellyfish==0.8.2",
-    "tabulate==0.8.9",
-    "Flask==2.0.2",
-    "parsy==2.0",
+    "jellyfish==1.0.0",
+    "tabulate==0.9.0",
+    "Flask==2.3.2",
+    "parsy==2.1",
     "google-cloud-secret-manager<=2.15.0",
 ]
 
 extras_require = {
     "apache-airflow": "1.10.11",
     "pyspark": "3.0.0",
 }
@@ -80,20 +80,20 @@
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=packages,
     classifiers=[
         release_status,
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=dependencies,
     extras_require=extras_require,
     entry_points={
         "console_scripts": [
             "data-validation=data_validation.__main__:main",
         ]
     },
```

### Comparing `google-pso-data-validator-3.2.0/third_party/ibis/ibis_DB2/compiler.py` & `google-pso-data-validator-4.0.0/third_party/ibis/ibis_db2/registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,87 @@
-# Copyright 2020 Google Inc.
+# Copyright 2023 Google Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 import functools
 import itertools
 import locale
 import platform
 import re
 import string
 import warnings
+import operator
 
-import ibm_db_sa
 import sqlalchemy as sa
-from sqlalchemy.ext.compiler import compiles
-from sqlalchemy.sql.functions import GenericFunction
 
-import ibis
 import ibis.common.exceptions as com
-import ibis.common.geospatial as geo
-import ibis.expr.datatypes as dt
 import ibis.expr.operations as ops
-import ibis.expr.types as ir
-import ibis.backends.base_sqlalchemy.alchemy as alch
-import third_party.ibis.ibis_DB2.alchemy as db2_alch
-
-# used for literal translate
-from ibis.backends.base_sqlalchemy.alchemy import (
-    _get_sqla_table,
-    _variance_reduction,
+
+from ibis.backends.base.sql.alchemy import (
     fixed_arity,
-    infix_op,
+    sqlalchemy_operation_registry,
+    sqlalchemy_window_functions_registry,
     unary,
+    get_sqla_table,
 )
+from ibis.backends.base.sql.alchemy.registry import variance_reduction
 
-_operation_registry = alch._operation_registry.copy()
-_operation_registry.update(alch._window_functions)
-
-
-class DB2UDFNode(ops.ValueOp):
-    pass
+operation_registry = sqlalchemy_operation_registry.copy()
+operation_registry.update(sqlalchemy_window_functions_registry)
 
 
-# TODO: substr and find are copied from SQLite, we should really have a
-# "base" set of SQL functions that are the most common APIs across the major
-# RDBMS
-def _substr(t, expr):
+def _substr(t, op):
     f = sa.func.substr
+    sa_arg = t.translate(op.arg)
+    sa_start = t.translate(op.start)
 
-    arg, start, length = expr.op().args
-
-    sa_arg = t.translate(arg)
-    sa_start = t.translate(start)
-
-    if length is None:
+    if op.length is None:
         return f(sa_arg, sa_start + 1)
     else:
-        sa_length = t.translate(length)
+        sa_length = t.translate(op.length)
         return f(sa_arg, sa_start + 1, sa_length)
 
 
-def _string_find(t, expr):
-    arg, substr, start, _ = expr.op().args
-    if start is not None:
+def _string_find(t, op):
+    if op.start is not None:
         raise NotImplementedError
 
-    sa_arg = t.translate(arg)
-    sa_substr = t.translate(substr)
+    sa_arg = t.translate(op.arg)
+    sa_substr = t.translate(op.substr)
 
-    return sa.func.instr(sa_arg, sa_substr) - 1
+    return sa.func.instr(sa_arg, sa_substr)
 
 
-def _extract(fmt, output_type=sa.SMALLINT):
-    def translator(t, expr, output_type=output_type):
-        (arg,) = expr.op().args
-        sa_arg = t.translate(arg)
-        return sa.cast(sa.extract(fmt, sa_arg), output_type)
+def _extract(fmt: str):
+    def translator(t, op: ops.Node):
+        return sa.cast(sa.extract(fmt, t.translate(op.arg)), sa.SMALLINT)
 
     return translator
 
 
-def _second(t, expr):
+def _second(t, op):
     # extracting the second gives us the fractional part as well, so smash that
     # with a cast to SMALLINT
-    (sa_arg,) = map(t.translate, expr.op().args)
-    return sa.cast(sa.func.FLOOR(sa.extract('second', sa_arg)), sa.SMALLINT)
+    return sa.cast(sa.func.FLOOR(sa.extract('second', t.translate(op.arg))), sa.SMALLINT)
 
 
-def _millisecond(t, expr):
+def _millisecond(t, op):
     # we get total number of milliseconds including seconds with extract so we
     # mod 1000
-    (sa_arg,) = map(t.translate, expr.op().args)
     return (
-        sa.cast(sa.func.floor(sa.extract('millisecond', sa_arg)), sa.SMALLINT)
+        sa.cast(sa.func.floor(sa.extract('millisecond', op.arg)), sa.SMALLINT)
         % 1000
     )
 
 
 _truncate_precisions = {
     'us': 'microseconds',
     'ms': 'milliseconds',
@@ -116,79 +92,65 @@
     'W': 'week',
     'M': 'month',
     'Q': 'quarter',
     'Y': 'year',
 }
 
 
-def _timestamp_truncate(t, expr):
-    arg, unit = expr.op().args
-    sa_arg = t.translate(arg)
-    try:
-        precision = _truncate_precisions[unit]
-    except KeyError:
-        raise com.UnsupportedOperationError(
-            'Unsupported truncate unit {!r}'.format(unit)
-        )
-    return sa.func.date_trunc(precision, sa_arg)
-
-
-def _interval_from_integer(t, expr):
-    arg, unit = expr.op().args
-    sa_arg = t.translate(arg)
-    interval = sa.text("INTERVAL '1 {}'".format(expr.type().resolution))
-    return sa_arg * interval
-
+def _timestamp_truncate(t, op):
+    arg = t.translate(op.arg)
+    unit = op.unit
+    if unit not in _truncate_precisions:
+        raise com.UnsupportedOperationError(f'Unsupported truncate unit {op.unit!r}')
 
-def _timestamp_add(t, expr):
-    sa_args = list(map(t.translate, expr.op().args))
-    return sa_args[0] + sa_args[1]
+    return sa.func.datetrunc(sa.text(_truncate_precisions[unit]), arg)
 
 
-def _is_nan(t, expr):
-    (arg,) = expr.op().args
-    sa_arg = t.translate(arg)
+def _is_nan(t, op):
+    sa_arg = t.translate(op.arg)
     return sa_arg == float('nan')
 
 
-def _is_inf(t, expr):
-    (arg,) = expr.op().args
-    sa_arg = t.translate(arg)
+def _is_inf(t, op):
+    sa_arg = t.translate(op.arg)
     inf = float('inf')
     return sa.or_(sa_arg == inf, sa_arg == -inf)
 
 
-def _cast(t, expr):
-    arg, typ = expr.op().args
+def _cast(t, op):
+    arg = op.arg
+    typ = op.to
+    arg_dtype = arg.output_dtype
 
     sa_arg = t.translate(arg)
-    sa_type = t.get_sqla_type(typ)
 
     # specialize going from an integer type to a timestamp
-    if isinstance(arg.type(), dt.Integer) and isinstance(sa_type, sa.DateTime):
-        return sa.func.timezone('UTC', sa.func.to_timestamp(sa_arg))
+    if arg_dtype.is_integer() and typ.is_timestamp():
+        return t.integer_to_timestamp(sa_arg, tz=typ.timezone)
 
-    if arg.type().equals(dt.binary) and typ.equals(dt.string):
+    if arg_dtype.is_binary() and typ.is_string():
         return sa.func.encode(sa_arg, 'escape')
 
-    if typ.equals(dt.binary):
+    if typ.is_binary():
         #  decode yields a column of memoryview which is annoying to deal with
         # in pandas. CAST(expr AS BYTEA) is correct and returns byte strings.
         return sa.cast(sa_arg, sa.LargeBinary())
 
-    return sa.cast(sa_arg, sa_type)
+    if typ.is_json() and not t.native_json_type:
+        return sa_arg
 
+    return sa.cast(sa_arg, t.get_sqla_type(typ))
 
-def _string_agg(t, expr):
-    arg, sep, where = expr.op().args
-    sa_arg = t.translate(arg)
-    sa_sep = t.translate(sep)
 
-    if where is not None:
-        operand = t.translate(where.ifelse(arg, ibis.NA))
+def _string_agg(t, op):
+    sa_arg = t.translate(op.arg)
+    sa_sep = t.translate(op.sep)
+
+    if (where := op.where) is not None:
+        operand = t.translate(where.ifelse(op.arg, ibis.NA))
     else:
         operand = sa_arg
     return sa.func.listagg(operand, sa_sep)
 
 
 _strftime_to_db2_rules = {
     '%a': 'TMDy',  # TM does it in a locale dependent way
@@ -330,49 +292,46 @@
         # append result to r if we had more tokens or if we have no
         # blacklisted tokens
         if curtokens:
             reduced.append(sa.func.to_char(arg, ''.join(curtokens)))
     return reduced
 
 
-def _strftime(t, expr):
-    arg, pattern = map(t.translate, expr.op().args)
+def _strftime(arg, pattern):
     tokens, _ = _scanner.scan(pattern.value)
     reduced = _reduce_tokens(tokens, arg)
     result = functools.reduce(sa.sql.ColumnElement.concat, reduced)
     return result
 
 
-def _regex_replace(t, expr):
-    string, pattern, replacement = map(t.translate, expr.op().args)
-
-    return sa.func.regexp_replace(string, pattern, replacement)
+def _regex_replace(t, op):
+    return sa.func.regexp_replace(t.translate(op.string), t.translate(op.pattern), t.translate(op.replacement))
 
 
 def _reduction(func_name):
-    def reduction_compiler(t, expr):
-        arg, where = expr.op().args
+    def reduction_compiler(t, op):
+        arg, where = op.args
 
-        if arg.type().equals(dt.boolean):
+        if arg.output_dtype.is_boolean():
             arg = arg.cast('int32')
 
         func = getattr(sa.func, func_name)
 
         if where is not None:
             arg = where.ifelse(arg, None)
         return func(t.translate(arg))
 
     return reduction_compiler
 
+
 def _count_start(sa_func):
     return sa_func
 
 def _reduction_count(sa_func):
-    def formatter(t, expr):
-        op = expr.op()
+    def formatter(t, op):
         *args, where = op.args
 
         return _reduction_format(t, sa_func, where, *args)
 
     return formatter
 
 def _reduction_format(t, sa_func, where, arg, *args):
@@ -383,155 +342,125 @@
 
     #Db2 doesn't allow '*' to be parameterized, probably better way to fix this... 
     if arg == '*':
         arg = None
 
     return sa_func(arg, *map(t.translate, args))
 
-def _log(t, expr):
-    arg, base = expr.op().args
+def _log(t, op):
+    arg, base = op.args
     sa_arg = t.translate(arg)
     if base is not None:
         sa_base = t.translate(base)
         return sa.cast(
-            sa.func.log(
-                sa.cast(sa_base, sa.NUMERIC), sa.cast(sa_arg, sa.NUMERIC)
-            ),
-            t.get_sqla_type(expr.type()),
+            sa.func.log(sa.cast(sa_base, sa.NUMERIC), sa.cast(sa_arg, sa.NUMERIC)),
+            t.get_sqla_type(op.output_dtype),
         )
     return sa.func.ln(sa_arg)
 
 
-class regex_extract(GenericFunction):
-    def __init__(self, string, pattern, index):
-        super().__init__(string, pattern, index)
-        self.string = string
-        self.pattern = pattern
-        self.index = index
-
-
-@compiles(regex_extract, 'db2')
-def compile_regex_extract(element, compiler, **kw):
-    result = '(SELECT regexp_substr({}, {}, {}) as TMP FROM dual)'.format(
-        compiler.process(element.string, **kw),
-        compiler.process(element.pattern, **kw),
-        compiler.process(element.index, **kw),
-    )
-    return result
+def _regex_extract(t, op):
+    return sa.func.regex_extract(t.translate(op.string), t.translate(op.pattern), t.translate(op.index +1))
 
 
-def _regex_extract(t, expr):
-    string, pattern, index = map(t.translate, expr.op().args)
-    result = sa.func.regexp_extract(string, pattern, index + 1)
-    return result
-
-
-def _identical_to(t, expr):
-    left, right = args = expr.op().args
+def _identical_to(t, op):
+    left, right = args = op.args
     if left.equals(right):
         return True
     else:
         left, right = map(t.translate, args)
         return left.op('IS NOT DISTINCT FROM')(right)
 
 
-def _hll_cardinality(t, expr):
-    arg, _ = expr.op().args
-    sa_arg = t.translate(arg)
-    return sa.func.count(sa.distinct(sa_arg))
+def get_col(sa_table, op: ops.TableColumn):
+    """Extract a column from a table."""
+    cols = sa_table.exported_columns
+    colname = op.name
+
+    if (col := cols.get(colname)) is not None:
+        return col
+
+    # `cols` is a SQLAlchemy column collection that contains columns
+    # with names that are secretly prefixed by table that contains them
+    #
+    # for example, in `t0.join(t1).select(t0.a, t1.b)` t0.a will be named `t0_a`
+    # and t1.b will be named `t1_b`
+    #
+    # unfortunately SQLAlchemy doesn't let you select by the *un*prefixed
+    # column name despite the uniqueness of `colname`
+    #
+    # however, in ibis we have already deduplicated column names so we can
+    # refer to the name by position
+    colindex = op.table.schema._name_locs[colname]
+    return cols[colindex]
 
 
-def _table_column(t, expr):
-    op = expr.op()
+def _table_column(t, op):
     ctx = t.context
     table = op.table
 
-    sa_table = _get_sqla_table(ctx, table)
-    out_expr = getattr(sa_table.c, op.name)
-
-    expr_type = expr.type()
+    sa_table = get_sqla_table(ctx, table)
 
-    if isinstance(expr_type, dt.Timestamp):
-        timezone = expr_type.timezone
-        if timezone is not None:
-            out_expr = out_expr.op('AT TIME ZONE')(timezone).label(op.name)
+    out_expr = get_col(sa_table, op)
+    out_expr.quote = t._quote_column_names
 
     # If the column does not originate from the table set in the current SELECT
     # context, we should format as a subquery
     if t.permit_subquery and ctx.is_foreign_expr(table):
-        return sa.select([out_expr])
+        try:
+            subq = sa_table.subquery()
+        except AttributeError:
+            subq = sa_table
+        return sa.select(subq.c[out_expr.name])
 
     return out_expr
 
 
-def _round(t, expr):
-    arg, digits = expr.op().args
-    sa_arg = t.translate(arg)
-
-    if digits is None:
-        return sa.func.round(sa_arg)
+def _round(t, op):
+    sa_arg = t.translate(op.arg)
 
-    result = sa.func.round(sa.cast(sa_arg, sa.NUMERIC), t.translate(digits))
-    if digits is not None and isinstance(arg.type(), dt.Decimal):
-        return result
-    result = sa.cast(result, ibm_db_sa.double)
-    return result
-
-
-def _mod(t, expr):
-    left, right = map(t.translate, expr.op().args)
-
-    if not isinstance(expr.type(), dt.Integer):
-        left = sa.cast(left, sa.NUMERIC)
-        right = sa.cast(right, sa.NUMERIC)
-
-    result = left % right
-    if expr.type().equals(dt.double):
-        return sa.cast(result, ibm_db_sa.double)
+    if op.digits is not None:
+        return sa.func.round(sa_arg, t.translate(op.digits))
     else:
-        return result
+        return sa.func.round(sa_arg)
 
 
-def _string_join(t, expr):
-    sep, elements = expr.op().args
-    columns = [col.name for col in map(t.translate, elements)]
+def _string_join(t, op):
+    sep, elements = op.args
+    columns = [str(col.name) for col in map(t.translate, elements)]
     return sa.sql.literal_column(" || ".join(columns))
 
 
-def _literal(t, expr):
-    dtype = expr.type()
-    op = expr.op()
+def _literal(t, op):
+    dtype = op.output_dtype
     value = op.value
 
-    if isinstance(dtype, dt.Interval):
-        return sa.text("INTERVAL '{} {}'".format(value, dtype.resolution))
-    elif isinstance(dtype, dt.Set):
+    if dtype.is_interval():
+        return sa.literal_column(f"INTERVAL '{value} {dtype.resolution}'")
+    elif dtype.is_set():
         return list(map(sa.literal, value))
-    elif isinstance(expr, ir.GeoSpatialScalar):
-        # inline_metadata ex: 'SRID=4326;POINT( ... )'
-        return sa.text(geo.translate_literal(expr, inline_metadata=True))
     else:
         return sa.literal(value)
 
 
 def _random(t, expr):
     return sa.func.random()
 
 
-def _day_of_week_index(t, expr):
-    (sa_arg,) = map(t.translate, expr.op().args)
+def _day_of_week_index(t, op):
+    (sa_arg,) = map(t.translate, op.arg)
     return sa.func.dayofweek(sa_arg)
 
 
-def _day_of_week_name(t, expr):
-    (sa_arg,) = map(t.translate, expr.op().args)
+def _day_of_week_name(t, op):
+    (sa_arg,) = map(t.translate, op.arg)
     return sa.func.dayname(sa_arg)
 
 
-_operation_registry.update(
+operation_registry.update(
     {
         ops.Literal: _literal,
         ops.TableColumn: _table_column,
         # types
         ops.Cast: _cast,
         # Floating
         ops.IsNan: _is_nan,
@@ -554,81 +483,48 @@
         ops.RegexExtract: _regex_extract,
         ops.StringJoin: _string_join,
         # math
         ops.Log: _log,
         ops.Log2: unary(lambda x: sa.func.log(2, x)),
         ops.Log10: unary(sa.func.log),
         ops.Round: _round,
-        ops.Modulus: _mod,
+        ops.Modulus: fixed_arity(operator.mod, 2),
         ops.Power: fixed_arity(sa.func.power, 2),
         # dates and times
         ops.Date: unary(lambda x: sa.cast(x, sa.Date)),
         ops.DateTruncate: _timestamp_truncate,
         ops.TimestampTruncate: _timestamp_truncate,
-        ops.IntervalFromInteger: _interval_from_integer,
-        ops.DateAdd: infix_op('+'),
-        ops.DateSub: infix_op('-'),
-        ops.DateDiff: infix_op('-'),
-        ops.TimestampAdd: infix_op('+'),
-        ops.TimestampSub: infix_op('-'),
-        ops.TimestampDiff: infix_op('-'),
+        ops.DateAdd: fixed_arity(operator.add, 2),
+        ops.DateSub: fixed_arity(operator.sub, 2),
+        ops.DateDiff: fixed_arity(operator.sub, 2),
+        ops.TimestampAdd: fixed_arity(operator.add, 2),
+        ops.TimestampSub: fixed_arity(operator.sub, 2),
+        ops.TimestampDiff: fixed_arity(operator.sub, 2),
         ops.Strftime: _strftime,
         ops.ExtractYear: _extract('year'),
         ops.ExtractMonth: _extract('month'),
         ops.ExtractDay: _extract('day'),
-        #ops.ExtractDayOfYear: _extract('doy'),
-        #ops.ExtractQuarter: _extract('quarter'),
-        #ops.ExtractEpochSeconds: _extract('epoch', sa.BigInteger),
+        ops.ExtractDayOfYear: _extract('doy'),
+        ops.ExtractQuarter: _extract('quarter'),
+        ops.ExtractEpochSeconds: _extract('epoch'),
         ops.ExtractHour: _extract('hour'),
         ops.ExtractMinute: _extract('minute'),
         ops.ExtractSecond: _second,
         ops.ExtractMillisecond: _millisecond,
         ops.DayOfWeekIndex: _day_of_week_index,
         ops.DayOfWeekName: _day_of_week_name,
         ops.Sum: _reduction('sum'),
         ops.Mean: _reduction('avg'),
         ops.Min: _reduction('min'),
         ops.Max: _reduction('max'),
-        ops.Variance: _variance_reduction('variance'),
-        ops.StandardDev: _variance_reduction('stddev'),
-        #ops.RandomScalar: _random,
+        ops.Variance: variance_reduction('var', suffix={'sample': '', 'pop': 'p'}),
+        ops.StandardDev: variance_reduction('stdev', suffix={'sample': '', 'pop': 'p'}),
+        ops.RandomScalar: _random,
         ops.TimestampNow: lambda *args: sa.func.timezone('UTC', sa.func.now()),
         ops.CumulativeAll: unary(sa.func.bool_and),
         ops.CumulativeAny: unary(sa.func.bool_or),
         ops.IdenticalTo: _identical_to,
-        ops.HLLCardinality: _hll_cardinality,
         # aggregate methods
         ops.Count: _reduction_count(sa.func.count),
 
     }
-)
-
-
-def add_operation(op, translation_func):
-    _operation_registry[op] = translation_func
-
-
-class DB2ExprTranslator(db2_alch.AlchemyExprTranslator):
-
-    _registry = _operation_registry
-    _rewrites = db2_alch.AlchemyExprTranslator._rewrites.copy()
-    _type_map = db2_alch.AlchemyExprTranslator._type_map.copy()
-    _type_map.update({dt.Double: ibm_db_sa.DOUBLE, dt.Float: ibm_db_sa.REAL})
-
-
-rewrites = DB2ExprTranslator.rewrites
-compiles = DB2ExprTranslator.compiles
-
-
-@rewrites(ops.Any)
-@rewrites(ops.All)
-@rewrites(ops.NotAny)
-@rewrites(ops.NotAll)
-def _any_all_no_op(expr):
-    return expr
-
-
-class DB2Dialect(db2_alch.AlchemyDialect):
-    translator = DB2ExprTranslator
-
-
-dialect = DB2Dialect
+)
```

### Comparing `google-pso-data-validator-3.2.0/third_party/ibis/ibis_addon/operations.py` & `google-pso-data-validator-4.0.0/third_party/ibis/ibis_addon/operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,328 +18,337 @@
 Raw SQL Filters:
 The ability to inject RawSQL into a query DNE in Ibis.  It must be built out
 and applied to each Ibis Data Source directly as each has
 extended its own registry.  Eventually this can potentially be pushed to
 Ibis as an override, though it would not apply for Pandas and other
 non-textual languages.
 """
-
 import ibis
-import sqlalchemy as sa
-
-import ibis.expr.api
 import ibis.expr.datatypes as dt
-import ibis.expr.rules as rlz
 import ibis.expr.operations as ops
-
-from data_validation.clients import _raise_missing_client_error
-from ibis_bigquery.compiler import (
-    reduction as bq_reduction,
-    BigQueryExprTranslator,
+import ibis.expr.rules as rlz
+import sqlalchemy as sa
+from ibis.backends.base.sql.alchemy.registry import \
+    fixed_arity as sa_fixed_arity
+from ibis.backends.base.sql.alchemy.translator import AlchemyExprTranslator
+from ibis.backends.base.sql.compiler.translator import ExprTranslator
+from ibis.backends.base.sql.registry import fixed_arity
+from ibis.backends.bigquery.client import _DTYPE_TO_IBIS_TYPE
+from ibis.backends.bigquery.compiler import BigQueryExprTranslator
+from ibis.backends.bigquery.registry import \
     STRFTIME_FORMAT_FUNCTIONS as BQ_STRFTIME_FORMAT_FUNCTIONS
-)
-from ibis.backends.base_sqlalchemy.alchemy import fixed_arity
-from ibis.expr.operations import Arg, Cast, Comparison, Reduction, Strftime, ValueOp
-from ibis.expr.types import BinaryValue, IntegerColumn, StringValue, NumericValue, TemporalValue
 from ibis.backends.impala.compiler import ImpalaExprTranslator
-from ibis.backends.pandas import client as _pandas_client
-from ibis.backends.base_sqlalchemy.alchemy import AlchemyExprTranslator
-from ibis.backends.base_sqlalchemy.compiler import ExprTranslator
-from ibis.backends.base_sql.compiler import BaseExprTranslator
-from third_party.ibis.ibis_oracle.compiler import OracleExprTranslator
-from third_party.ibis.ibis_teradata.compiler import TeradataExprTranslator
-from third_party.ibis.ibis_mssql.compiler import MSSQLExprTranslator
-from ibis.backends.postgres.compiler import PostgreSQLExprTranslator
+from ibis.backends.mssql.compiler import MsSqlExprTranslator
 from ibis.backends.mysql.compiler import MySQLExprTranslator
+from ibis.backends.postgres.compiler import PostgreSQLExprTranslator
+from ibis.expr.operations import (Cast, Comparison, HashBytes, IfNull,
+                                  RandomScalar, Strftime, StringJoin,
+                                  Value, ExtractEpochSeconds)
+from ibis.expr.types import NumericValue, TemporalValue
+
+import third_party.ibis.ibis_mysql.compiler
+import third_party.ibis.ibis_postgres.client
+from third_party.ibis.ibis_db2.compiler import Db2ExprTranslator
+from third_party.ibis.ibis_oracle.compiler import OracleExprTranslator
 from third_party.ibis.ibis_redshift.compiler import RedShiftExprTranslator
 
-# avoid errors if Db2 is not installed and not needed
+# TD requires teradatasql
 try:
-    from third_party.ibis.ibis_DB2.compiler import DB2ExprTranslator
+    from third_party.ibis.ibis_teradata.compiler import TeradataExprTranslator
 except Exception:
-    DB2ExprTranslator = None
-
-
-# from third_party.ibis.ibis_snowflake.compiler import SnowflakeExprTranslator
-# from third_party.ibis.ibis_oracle.compiler import OracleExprTranslator <<<<<< DB2
-
-class BitXor(Reduction):
-    """Aggregate bitwise XOR operation."""
-
-    arg = Arg(rlz.column(rlz.integer))
-    where = Arg(rlz.boolean, default=None)
-    output_type = rlz.scalar_like("arg")
-
+    TeradataExprTranslator = None
 
-class Hash(ValueOp):
-    arg = Arg(rlz.any)
-    how = Arg(rlz.isin({"fnv", "farm_fingerprint"}))
-    output_type = rlz.shape_like("arg", dt.int64)
-
-
-class HashBytes(ValueOp):
-    arg = Arg(rlz.one_of([rlz.value(dt.string), rlz.value(dt.binary)]))
-    how = Arg(rlz.isin({"sha256", "farm_fingerprint"}))
-    output_type = rlz.shape_like("arg", "binary")
+# Snowflake requires snowflake-connector-python and snowflake-sqlalchemy
+try:
+    from ibis.backends.snowflake import SnowflakeExprTranslator
+except Exception:
+    SnowflakeExprTranslator = None
 
-class ToChar(ValueOp):
-    arg = Arg(rlz.one_of([rlz.value(dt.Decimal), rlz.value(dt.float64), rlz.value(dt.Date), rlz.value(dt.Time), rlz.value(dt.Timestamp)]))
-    fmt = Arg(rlz.string)
-    output_type = rlz.shape_like("arg", dt.string)
+class ToChar(Value):
+    arg = rlz.one_of([rlz.value(dt.Decimal), rlz.value(dt.float64), rlz.value(dt.Date), rlz.value(dt.Time), rlz.value(dt.Timestamp)])
+    fmt = rlz.string
+    output_type = rlz.shape_like("arg")
 
 class RawSQL(Comparison):
     pass
 
 
-def compile_hash(numeric_value, how):
-    return Hash(numeric_value, how=how).to_expr()
-
-
-def compile_hash(binary_value, how):
-    return Hash(binary_value, how=how).to_expr()
-
-
-def format_hash_bigquery(translator, expr):
-    op = expr.op()
-    arg, how = op.args
-
-    arg_formatted = translator.translate(arg)
-
-    if how == "farm_fingerprint":
-        return f"farm_fingerprint({arg_formatted})"
-    else:
-        raise NotImplementedError(how)
-
-
-def compile_hashbytes(binary_value, how):
-    return HashBytes(binary_value, how=how).to_expr()
-
-
 def compile_to_char(numeric_value, fmt):
     return ToChar(numeric_value, fmt=fmt).to_expr()
 
 
-def format_hash_bigquery(translator, expr):
-    arg, how = expr.op().args
-    compiled_arg = translator.translate(arg)
-    if how == "farm_fingerprint":
-        return f"FARM_FINGERPRINT({compiled_arg})"
+def format_hash_bigquery(translator, op):
+    arg = translator.translate(op.arg)
+    if op.how == "farm_fingerprint":
+        return f"FARM_FINGERPRINT({rg})"
     else:
         raise ValueError(f"unexpected value for 'how': {how}")
 
 
-def format_hashbytes_bigquery(translator, expr):
-    arg, how = expr.op().args
-    compiled_arg = translator.translate(arg)
-    if how == "sha256":
-        return f"TO_HEX(SHA256({compiled_arg}))"
+def format_hashbytes_bigquery(translator, op):
+    arg = translator.translate(op.arg)
+    if op.how == "sha256":
+        return f"TO_HEX(SHA256({arg}))"
     elif how == "farm_fingerprint":
-        return f"FARM_FINGERPRINT({compiled_arg})"
+        return f"FARM_FINGERPRINT({arg})"
+    else:
+        raise ValueError(f"unexpected value for 'how': {how}")
+
+
+def format_hashbytes_teradata(translator, op):
+    arg = translator.translate(op.arg)
+    if op.how == "sha256":
+        return f"rtrim(hash_sha256({arg}))"
+    elif op.how == "sha512":
+        return f"rtrim(hash_sha512({arg}))"
+    elif op.how == "md5":
+        return f"rtrim(hash_md5({arg}))"
     else:
         raise ValueError(f"unexpected value for 'how': {how}")
 
 
-def strftime_bigquery(translator, expr):
-    """Timestamp formatting. Copied from bigquery_ibis in order to inject TIMESTAMP cast"""
-    arg, format_string = expr.op().args
-    arg_type = arg.type()
+def strftime_bigquery(translator, op):
+    """Timestamp formatting."""
+    arg = op.arg
+    format_str = op.format_str
+    arg_type = arg.output_dtype
     strftime_format_func_name = BQ_STRFTIME_FORMAT_FUNCTIONS[type(arg_type)]
-    fmt_string = translator.translate(format_string)
+    fmt_string = translator.translate(format_str)
     arg_formatted = translator.translate(arg)
     if isinstance(arg_type, dt.Timestamp):
         return "FORMAT_{}({}, {}({}), {!r})".format(
             strftime_format_func_name,
             fmt_string,
             strftime_format_func_name,
             arg_formatted,
             arg_type.timezone if arg_type.timezone is not None else "UTC",
         )
     return "FORMAT_{}({}, {})".format(
         strftime_format_func_name, fmt_string, arg_formatted
     )
 
-def strftime_mysql(translator, expr):
-    arg, format_string = expr.op().args 
+def strftime_mysql(translator, op):
+    arg = op.arg
+    format_string = op.format_str
     arg_formatted = translator.translate(arg)
-    arg_type = arg.type()
+    arg_type = arg.output_dtype
     fmt_string = translator.translate(format_string)
     if isinstance(arg_type, dt.Timestamp):
         fmt_string = "%Y-%m-%d %H:%i:%S"
     return sa.func.date_format(arg_formatted, fmt_string)
 
+def strftime_mssql(translator, op):
+    """Use MS SQL CONVERT() in place of STRFTIME().
+
+    This is pretty restrictive due to the limited styles offered by SQL Server,
+    we've just covered off the generic formats used when casting date based columns
+    to string in order to complete row data comparison."""
+    arg, pattern = map(translator.translate, op.args)
+    supported_convert_styles = {
+        "%Y-%m-%d": 23, # ISO8601
+        "%Y-%m-%d %H:%M:%S": 20, # ODBC canonical
+        "%Y-%m-%d %H:%M:%S.%f": 21, # ODBC canonical (with milliseconds)
+    }
+    try:
+        convert_style = supported_convert_styles[pattern.value]
+    except KeyError:
+        raise NotImplementedError(
+            f'strftime format {pattern.value} not supported for SQL Server.'
+        )
+    result = sa.func.convert(sa.text('VARCHAR(32)'), arg, convert_style)
+    return result
 
-def format_hashbytes_teradata(translator, expr):
-    arg, how = expr.op().args
-    compiled_arg = translator.translate(arg)
-    if how == "sha256":
-        return f"rtrim(hash_sha256({compiled_arg}))"
-    elif how == "sha512":
-        return f"rtrim(hash_sha512({compiled_arg}))"
-    elif how == "md5":
-        return f"rtrim(hash_md5({compiled_arg}))"
-    else:
-        raise ValueError(f"unexpected value for 'how': {how}")
 
-def format_hashbytes_hive(translator, expr):
-    arg, how = expr.op().args
-    compiled_arg = translator.translate(arg)
-    if how == "sha256":
-        return f"sha2({compiled_arg}, 256)"
-    elif how == "md5":
-        return f"md5({compiled_arg})"
+def strftime_impala(t, op):
+    import sqlglot as sg
+
+    hive_dialect = sg.dialects.hive.Hive
+    if (time_mapping := getattr(hive_dialect, "TIME_MAPPING", None)) is None:
+        time_mapping = hive_dialect.time_mapping
+    reverse_hive_mapping = {v: k for k, v in time_mapping.items()}
+    format_str = sg.time.format_time(op.format_str.value, reverse_hive_mapping)
+    targ = t.translate(ops.Cast(op.arg, to=dt.string))
+    return f"from_unixtime(unix_timestamp({targ}, {format_str!r}), {format_str!r})"
+
+
+def format_hashbytes_hive(translator, op):
+    arg = translator.translate(op.arg)
+    if op.how == "sha256":
+        return f"sha2({arg}, 256)"
+    elif op.how == "md5":
+        return f"md5({arg})"
     else:
-        raise ValueError(f"unexpected value for 'how': {how}")
+        raise ValueError(f"unexpected value for 'how': {op.how}")
 
-def format_hashbytes_alchemy(translator, expr):
-    arg, how = expr.op().args
-    compiled_arg = translator.translate(arg)
-    if how == "sha256":
-        return f"sha2({compiled_arg}, 256)"
-    elif how == "md5":
-        return f"md5({compiled_arg})"
+def format_hashbytes_alchemy(translator, op):
+    arg = translator.translate(op.arg)
+    if op.how == "sha256":
+        return f"sha2({arg}, 256)"
+    elif op.how == "md5":
+        return f"md5({arg})"
     else:
-        raise ValueError(f"unexpected value for 'how': {how}")
+        raise ValueError(f"unexpected value for 'how': {op.how}")
 
-def format_hashbytes_base(translator, expr):
-    arg, how  = expr.op().args
-    compiled_arg = translator.translate(arg)
-    return f"sha2({compiled_arg}, 256)"
+def format_hashbytes_base(translator, op):
+    arg = translator.translate(op.arg)
+    return f"sha2({arg}, 256)"
 
 def compile_raw_sql(table, sql):
     op = RawSQL(table[table.columns[0]].cast(dt.string), ibis.literal(sql))
     return op.to_expr()
 
 
-def format_raw_sql(translator, expr):
-    op = expr.op()
+def format_raw_sql(translator, op):
     rand_col, raw_sql = op.args
-    return raw_sql.op().args[0]
+    return raw_sql.args[0]
 
 
-def sa_format_raw_sql(translator, expr):
-    op = expr.op()
+def sa_format_raw_sql(translator, op):
     rand_col, raw_sql = op.args
-    return sa.text(raw_sql.op().args[0])
+    return sa.text(raw_sql.args[0])
 
-def sa_format_hashbytes_mssql(translator, expr):
-    arg, how = expr.op().args
-    compiled_arg = translator.translate(arg)
-    hash_func = sa.func.hashbytes(sa.sql.literal_column("'SHA2_256'"), compiled_arg)
+def sa_format_hashbytes_mssql(translator, op):
+    arg = translator.translate(op.arg)
+    cast_arg = sa.func.convert(sa.sql.literal_column("VARCHAR(MAX)"), arg)
+    hash_func = sa.func.hashbytes(sa.sql.literal_column("'SHA2_256'"), cast_arg)
     hash_to_string = sa.func.convert(sa.sql.literal_column('CHAR(64)'), hash_func, sa.sql.literal_column('2'))
     return sa.func.lower(hash_to_string)
 
-def sa_format_hashbytes_oracle(translator, expr):
-    arg, how = expr.op().args
-    compiled_arg = translator.translate(arg)
-    hash_func = sa.func.standard_hash(compiled_arg, sa.sql.literal_column("'SHA256'"))
+def sa_format_hashbytes_oracle(translator, op):
+    arg = translator.translate(op.arg)
+    convert = sa.func.convert(arg, sa.sql.literal_column("'UTF8'"))
+    hash_func = sa.func.standard_hash(convert, sa.sql.literal_column("'SHA256'"))
     return sa.func.lower(hash_func)
 
-def sa_format_hashbytes_mysql(translator, expr):
-    arg, how = expr.op().args
-    compiled_arg = translator.translate(arg)
-    hash_func = sa.func.sha2(compiled_arg, sa.sql.literal_column("'256'"))
+def sa_format_hashbytes_mysql(translator, op):
+    arg = translator.translate(op.arg)
+    hash_func = sa.func.sha2(arg, sa.sql.literal_column("'256'"))
     return hash_func
 
-def sa_format_hashbytes_db2(translator, expr):
-    arg, how = expr.op().args
-    compiled_arg = translator.translate(arg)
+def sa_format_hashbytes_db2(translator, op):
+    compiled_arg = translator.translate(op.arg)
     hashfunc = sa.func.hash(compiled_arg,sa.sql.literal_column("2"))
     hex = sa.func.hex(hashfunc)
     return sa.func.lower(hex)
 
-def sa_format_hashbytes_redshift(translator, expr):
-    arg, how  = expr.op().args
-    compiled_arg = translator.translate(arg)
-    return sa.sql.literal_column(f"sha2({compiled_arg}, 256)")
-
-def sa_format_hashbytes_postgres(translator, expr):
-    arg, how = expr.op().args
-    compiled_arg = translator.translate(arg)
-    convert = sa.func.convert_to(compiled_arg, sa.sql.literal_column("'UTF8'"))
+def sa_format_hashbytes_redshift(translator, op):
+    arg = translator.translate(op.arg)
+    return sa.sql.literal_column(f"sha2({arg}, 256)")
+
+def sa_format_hashbytes_postgres(translator, op):
+    arg = translator.translate(op.arg)
+    convert = sa.func.convert_to(arg, sa.sql.literal_column("'UTF8'"))
     hash_func = sa.func.sha256(convert)
     return sa.func.encode(hash_func, sa.sql.literal_column("'hex'"))
 
-def sa_format_to_char(translator, expr):
-    arg, fmt = expr.op().args
-    compiled_arg = translator.translate(arg)
-    compiled_fmt = translator.translate(fmt)
-    return sa.func.to_char(compiled_arg, compiled_fmt)
-
-def sa_format_to_stringjoin(translator, expr):
-    sep, elements = expr.op().args
-    return sa.func.concat_ws(translator.translate(sep), *map(translator.translate, elements))
-
-
-def sa_cast_postgres(t, expr):
-    arg, typ = expr.op().args
+def sa_format_hashbytes_snowflake(translator, op):
+    arg = translator.translate(op.arg)
+    return sa.func.sha2(arg)
+
+def sa_epoch_time_snowflake(translator, op):
+    arg = translator.translate(op.arg)
+    return sa.func.date_part(sa.sql.literal_column("epoch_seconds"), arg)
+
+def sa_format_to_char(translator, op):
+    arg = translator.translate(op.arg)
+    fmt = translator.translate(op.fmt)
+    return sa.func.to_char(arg, fmt)
+
+
+def sa_cast_postgres(t, op):
+    # Add cast from numeric to string
+    arg = op.arg
+    typ = op.to
+    arg_dtype = arg.output_dtype
 
     sa_arg = t.translate(arg)
-    sa_type = t.get_sqla_type(typ)
-
-    # Specialize going from an integer type to a timestamp
-    if isinstance(arg.type(), dt.Integer) and isinstance(sa_type, sa.DateTime):
-        return sa.func.timezone('UTC', sa.func.to_timestamp(sa_arg))
 
     # Specialize going from numeric(p,s>0) to string
-    if isinstance(arg.type(), dt.Decimal) and arg.type().scale > 0 and typ.equals(dt.string):
+    if arg_dtype.is_decimal() and arg_dtype.scale and arg_dtype.scale > 0 and typ.is_string():
         # When casting a number to string PostgreSQL includes the full scale, e.g.:
         #   SELECT CAST(CAST(100 AS DECIMAL(5,2)) AS VARCHAR(10));
         #     100.00
         # This doesn't match most engines which would return "100".
         # Using to_char() function instead of cast to return a more typical value.
         # We've wrapped to_char in rtrim(".") due to whole numbers having a trailing ".".
         # Would have liked to use trim_scale but this is only available in PostgreSQL 13+
-        #     return (sa.cast(sa.func.trim_scale(sa_arg), sa_type))
-        precision = arg.type().precision or 38
-        fmt = "FM" + ("9" * (precision - arg.type().scale)) + "." + ("9" * arg.type().scale)
+        #     return (sa.cast(sa.func.trim_scale(arg), typ))
+        precision = arg_dtype.precision or 38
+        fmt = "FM" + ("9" * (precision - arg_dtype.scale)) + "." + ("9" * arg_dtype.scale)
         return sa.func.rtrim(sa.func.to_char(sa_arg, fmt), ".")
 
-    if arg.type().equals(dt.binary) and typ.equals(dt.string):
+    # specialize going from an integer type to a timestamp
+    if arg_dtype.is_integer() and typ.is_timestamp():
+        return t.integer_to_timestamp(sa_arg, tz=typ.timezone)
+
+    if arg_dtype.is_binary() and typ.is_string():
         return sa.func.encode(sa_arg, 'escape')
 
-    if typ.equals(dt.binary):
-        # Decode yields a column of memoryview which is annoying to deal with
+    if typ.is_binary():
+        #  decode yields a column of memoryview which is annoying to deal with
         # in pandas. CAST(expr AS BYTEA) is correct and returns byte strings.
         return sa.cast(sa_arg, sa.LargeBinary())
 
-    return sa.cast(sa_arg, sa_type)
+    if typ.is_json() and not t.native_json_type:
+        return sa_arg
+
+    return sa.cast(sa_arg, t.get_sqla_type(typ))
+
+def _sa_string_join(t, op):
+    return sa.func.concat(*map(t.translate, op.arg))
 
+def sa_format_new_id(t, op):
+    return sa.func.NEWID()
 
-_pandas_client._inferable_pandas_dtypes["floating"] = _pandas_client.dt.float64
-IntegerColumn.bit_xor = ibis.expr.api._agg_function("bit_xor", BitXor, True)
-BinaryValue.hash = compile_hash
-StringValue.hash = compile_hash
-BinaryValue.hashbytes = compile_hashbytes
-StringValue.hashbytes = compile_hashbytes
 NumericValue.to_char = compile_to_char
 TemporalValue.to_char = compile_to_char
-BigQueryExprTranslator._registry[BitXor] = bq_reduction("BIT_XOR")
-BigQueryExprTranslator._registry[Hash] = format_hash_bigquery
+
 BigQueryExprTranslator._registry[HashBytes] = format_hashbytes_bigquery
 BigQueryExprTranslator._registry[RawSQL] = format_raw_sql
 BigQueryExprTranslator._registry[Strftime] = strftime_bigquery
-MySQLExprTranslator._registry[Strftime] = strftime_mysql
+_DTYPE_TO_IBIS_TYPE["TIMESTAMP"] = dt.Timestamp(timezone="UTC")
+
 AlchemyExprTranslator._registry[RawSQL] = format_raw_sql
 AlchemyExprTranslator._registry[HashBytes] = format_hashbytes_alchemy
-MSSQLExprTranslator._registry[HashBytes] = sa_format_hashbytes_mssql
-MSSQLExprTranslator._registry[RawSQL] = sa_format_raw_sql
-BaseExprTranslator._registry[RawSQL] = format_raw_sql
-BaseExprTranslator._registry[HashBytes] = format_hashbytes_base
+ExprTranslator._registry[RawSQL] = format_raw_sql
+ExprTranslator._registry[HashBytes] = format_hashbytes_base
+
 ImpalaExprTranslator._registry[RawSQL] = format_raw_sql
 ImpalaExprTranslator._registry[HashBytes] = format_hashbytes_hive
+ImpalaExprTranslator._registry[RandomScalar] = fixed_arity("RAND", 0)
+ImpalaExprTranslator._registry[Strftime] = strftime_impala
+
 OracleExprTranslator._registry[RawSQL] = sa_format_raw_sql
 OracleExprTranslator._registry[HashBytes] = sa_format_hashbytes_oracle
 OracleExprTranslator._registry[ToChar] = sa_format_to_char
-TeradataExprTranslator._registry[RawSQL] = format_raw_sql
-TeradataExprTranslator._registry[HashBytes] = format_hashbytes_teradata
+
 PostgreSQLExprTranslator._registry[HashBytes] = sa_format_hashbytes_postgres
 PostgreSQLExprTranslator._registry[RawSQL] = sa_format_raw_sql
 PostgreSQLExprTranslator._registry[ToChar] = sa_format_to_char
 PostgreSQLExprTranslator._registry[Cast] = sa_cast_postgres
+
+MsSqlExprTranslator._registry[HashBytes] = sa_format_hashbytes_mssql
+MsSqlExprTranslator._registry[RawSQL] = sa_format_raw_sql
+MsSqlExprTranslator._registry[IfNull] = sa_fixed_arity(sa.func.isnull,2)
+MsSqlExprTranslator._registry[StringJoin] = _sa_string_join
+MsSqlExprTranslator._registry[RandomScalar] = sa_format_new_id
+MsSqlExprTranslator._registry[Strftime] = strftime_mssql
+
 MySQLExprTranslator._registry[RawSQL] = sa_format_raw_sql
 MySQLExprTranslator._registry[HashBytes] = sa_format_hashbytes_mysql
-MySQLExprTranslator._registry[ops.IfNull] = fixed_arity(sa.func.ifnull, 2)
-MySQLExprTranslator._registry[ops.StringJoin] = sa_format_to_stringjoin
+MySQLExprTranslator._registry[Strftime] = strftime_mysql
+
 RedShiftExprTranslator._registry[HashBytes] = sa_format_hashbytes_redshift
+RedShiftExprTranslator._registry[RawSQL] = sa_format_raw_sql
+
+Db2ExprTranslator._registry[HashBytes] = sa_format_hashbytes_db2
+Db2ExprTranslator._registry[RawSQL] = sa_format_raw_sql
 
-if DB2ExprTranslator: #check if Db2 driver is loaded
-    DB2ExprTranslator._registry[HashBytes] = sa_format_hashbytes_db2
+if TeradataExprTranslator:
+    TeradataExprTranslator._registry[RawSQL] = format_raw_sql
+    TeradataExprTranslator._registry[HashBytes] = format_hashbytes_teradata
+
+if SnowflakeExprTranslator:
+    SnowflakeExprTranslator._registry[HashBytes] = sa_format_hashbytes_snowflake
+    SnowflakeExprTranslator._registry[RawSQL] = sa_format_raw_sql
+    SnowflakeExprTranslator._registry[IfNull] = sa_fixed_arity(sa.func.ifnull, 2)
+    SnowflakeExprTranslator._registry[ExtractEpochSeconds] = sa_epoch_time_snowflake
```

### Comparing `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/api.py` & `google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,73 +8,35 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-"""CloudSpanner public API."""
-
-
-from third_party.ibis.ibis_cloud_spanner.client import CloudSpannerClient
-from third_party.ibis.ibis_cloud_spanner.compiler import dialect
-
 import google.cloud.spanner  # noqa: F401, fail early if spanner is missing
-import ibis.common.exceptions as com
-
-__all__ = ("compile", "connect", "verify")
-
-
-def compile(expr, params=None):
-    """Compile an expression for Cloud Spanner.
-
-    Returns
-    -------
-    compiled : str
 
-    See Also
-    --------
-    ibis.expr.types.Expr.compile
+from third_party.ibis.ibis_cloud_spanner import Backend as SpannerBackend
 
-    """
-    from third_party.ibis.ibis_cloud_spanner.compiler import to_sql
-
-    return to_sql(expr, dialect.make_context(params=params))
-
-
-def verify(expr, params=None):
-    """Check if an expression can be compiled using Cloud Spanner."""
-    try:
-        compile(expr, params=params)
-        return True
-    except com.TranslationError:
-        return False
 
-
-def connect(
+def spanner_connect(
     instance_id,
     database_id,
     project_id=None,
-) -> CloudSpannerClient:
-    """Create a CloudSpannerClient for use with Ibis.
+):
+    """Create a Cloud Spanner Backend for use with Ibis.
 
     Parameters
     ----------
     instance_id : str
         A Cloud Spanner Instance id.
     database_id : str
         A database id inside of the Cloud Spanner Instance
     project_id  : str (Optional)
         The ID of the project which owns the instances, tables and data.
-
-    Returns
-    -------
-    CloudSpannerClient
-
     """
-
-    return CloudSpannerClient(
+    backend = SpannerBackend()
+    backend.do_connect(
         instance_id=instance_id,
         database_id=database_id,
         project_id=project_id,
     )
+    return backend
```

### Comparing `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py` & `google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
-import random
 import pathlib
+import random
 
-from google.cloud import spanner_v1
 import pytest
-from third_party.ibis.ibis_cloud_spanner.api import connect
+from google.cloud import spanner_v1
 
+from third_party.ibis.ibis_cloud_spanner.api import spanner_connect
 
 DATA_DIR = pathlib.Path(__file__).parent
 
 RANDOM_MAX = 0xFFFFFFFF
 INSTANCE_ID_PREFIX = "data-validation-tool-"
 INSTANCE_ID_TEMPLATE = f"{INSTANCE_ID_PREFIX}{{timestamp}}"
 INSTANCE_ID_TIMESTAMP_FORMAT = "%Y%m%d-%H%M%S"
@@ -62,15 +62,17 @@
 
     These instances can be leftover if Cloud Build terminates the test run
     before the cleanup in the instance_id fixture compltetes.
     """
     for instance in spanner_client.list_instances():
         instance_id = instance.name.split("/")[-1]
         if instance_id.startswith(INSTANCE_ID_PREFIX):
-            creation_time = datetime.datetime.strptime(instance_id[len(INSTANCE_ID_PREFIX):], INSTANCE_ID_TIMESTAMP_FORMAT)
+            creation_time = datetime.datetime.strptime(
+                instance_id[len(INSTANCE_ID_PREFIX) :], INSTANCE_ID_TIMESTAMP_FORMAT
+            )
             if datetime.datetime.now() - creation_time > datetime.timedelta(days=1):
                 instance = spanner_client.instance(instance_id)
                 instance.delete()
 
 
 @pytest.fixture(scope="session")
 def spanner_client():
@@ -127,20 +129,20 @@
     database.run_in_transaction(insert_rows2)
     yield database_id
     database.drop()
 
 
 @pytest.fixture(scope="session")
 def client(instance_id, database_id):
-    return connect(instance_id, database_id)
+    return spanner_connect(instance_id, database_id)
 
 
 @pytest.fixture(scope="session")
 def client2(instance_id, database_id):
-    return connect(instance_id, database_id)
+    return spanner_connect(instance_id, database_id)
 
 
 @pytest.fixture(scope="session")
 def alltypes(client):
     return client.table("functional_alltypes")
```

### Comparing `google-pso-data-validator-3.2.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py` & `google-pso-data-validator-4.0.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,19 +30,13 @@
         else:
             data_qry = snapshot.execute_sql(sql)
 
         data = []
         for row in data_qry:
             data.append(row)
 
-        columns_dict = {}
+        columns = [f.name for f in data_qry.fields]
 
-        for item in data_qry.fields:
-            columns_dict[item.name] = item.type_.code.name
-
-        # Creating list of columns to be mapped with the data
-        column_list = [k for k, v in columns_dict.items()]
-
-        # Creating pandas dataframe from data and columns_list
-        df = DataFrame(data, columns=column_list)
+        # Creating pandas dataframe from data and columns
+        df = DataFrame(data, columns=columns)
 
         return df
```

### Comparing `google-pso-data-validator-3.2.0/third_party/ibis/ibis_impala/api.py` & `google-pso-data-validator-4.0.0/third_party/ibis/ibis_impala/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,231 +8,236 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ibis.backends.base_sql import fixed_arity
-from ibis.backends.impala import connect, udf
+import ibis
+from ibis.backends.impala import Backend as ImpalaBackend
+from ibis.backends.impala.client import ImpalaConnection
+
+from pathlib import Path
+from typing import Literal
+
+from ibis.backends.impala import udf
 from ibis.backends.impala.compiler import rewrites
 import ibis.expr.datatypes as dt
 import ibis.expr.operations as ops
 import ibis.expr.schema as sch
 import numpy as np
-import pandas as pd
-
-from ibis.config import options
-from ibis.backends.impala.client import (  
-    ImpalaClient,
-    ImpalaConnection,
-    ImpalaDatabase,
-    ImpalaTable,
-    ImpalaQuery,
-    _HS2_TTypeId_to_dtype
-)
-
-_impala_to_ibis_type = udf._impala_to_ibis_type
+import fsspec
 
-_impala_to_ibis_type["date"] = "date"
-_HS2_TTypeId_to_dtype["DATE"] = "datetime64[ns]"
 
-def impala_connect(
-    host=None,
-    port=10000,
-    database="default",
-    auth_mechanism="PLAIN",
-    kerberos_service_name="impala",
-    use_ssl=False,
-    timeout=45,
-    ca_cert=None,
-    user=None,
-    password=None,
-    pool_size=8,
-    hdfs_client=None,
-    use_http_transport=False,
-    http_path="",
+def do_connect(
+    # Override do_connect to add use_http_transport and http_path params
+    self,
+    host: str = "localhost",
+    port: int = 10000,
+    database: str = "default",
+    timeout: int = 45,
+    use_ssl: bool = False,
+    ca_cert: str = None,
+    user: str = None,
+    password: str = None,
+    auth_mechanism: Literal["NOSASL", "PLAIN", "GSSAPI", "LDAP"] = "PLAIN",
+    kerberos_service_name: str = "impala",
+    pool_size: int = 8,
+    hdfs_client: fsspec.spec.AbstractFileSystem = None,
+    use_http_transport: bool = False,
+    http_path: str = "",
 ):
+    self._temp_objects = set()
+    self._hdfs = hdfs_client
+   
     params = {
         'host': host,
         'port': port,
         'database': database,
         'timeout': timeout,
         'use_ssl': use_ssl,
         'ca_cert': ca_cert,
         'user': user,
         'password': password,
         'auth_mechanism': auth_mechanism,
         'kerberos_service_name': kerberos_service_name,
         'use_http_transport': use_http_transport,
         'http_path': http_path,
     }
-    con = ImpalaConnection(pool_size=pool_size, **params)
-    try:
-        client = ImpalaClient(con, hdfs_client=hdfs_client)
-    except Exception:
-        con.close()
-        raise
-    else:
-        if options.default_backend is None:
-            options.default_backend = client
-    return client
+    self.con = ImpalaConnection(pool_size=pool_size, **params)
+    self._ensure_temp_db_exists()
 
 
 def parse_type(t):
     """Returns the Ibis datatype from source type."""
     t = t.lower()
-    if t in _impala_to_ibis_type:
-        return _impala_to_ibis_type[t]
+    if t in udf._impala_to_ibis_type:
+        return udf._impala_to_ibis_type[t]
     else:
         if "varchar" in t or "char" in t:
             return "string"
         elif "decimal" in t:
             result = dt.dtype(t)
             if result:
                 return t
             else:
                 return ValueError(t)
         elif "struct" in t or "array" in t or "map" in t:
+            # Supports parsing through structs/arrays in schema in #444
             if "bigint" in t:
                 t = t.replace(":bigint", ":int64")
             elif "tinyint" in t:
                 t = t.replace(":tinyint", ":int8")
             elif "smallint" in t:
                 t = t.replace(":smallint", ":int16")
             else:
                 t = t.replace(":int", ":int32")
 
             if "varchar" in t:
                 t = t.replace(":varchar", ":string")
             else:
-                t = t.replace(":char",":string")
+                t = t.replace(":char", ":string")
             return t
         else:
             raise Exception(t)
 
 
 def get_schema(self, table_name, database=None):
     """
-        Return a Schema object for the indicated table and database
+    Return a Schema object for the indicated table and database
 
-        Parameters
-        ----------
-        table_name : string
-          May be fully qualified
-        database : string, default None
-
-        Returns
-        -------
-        schema : ibis Schema
-        """
+    Parameters
+    ----------
+    table_name : string
+      May be fully qualified
+    database : string, default None
+
+    Returns
+    -------
+    schema : ibis Schema
+    """
     qualified_name = self._fully_qualified_name(table_name, database)
     query = "DESCRIBE {}".format(qualified_name)
 
-    # only pull out the first two columns which are names and types
-    # pairs = [row[:2] for row in self.con.fetchall(query)]
     pairs = []
     for row in self.con.fetchall(query):
+        # Add check for empty row for Hive partitioned tables in #375
         if row[0] == "":
             break
         pairs.append(row[:2])
 
     names, types = zip(*pairs)
     ibis_types = [parse_type(type.lower()) for type in types]
-    names = [name.lower() for name in names]
-
-    return sch.Schema(names, ibis_types)
+    ibis_fields = dict(zip(names, ibis_types))
 
-
-def _fetch(self, cursor):
-        batches = cursor.fetchall(columnar=True)
-        names = []
-        for x in cursor.description:
-            name = x[0].split('.')[-1]
-            names.append(name)
-        df = _column_batches_to_dataframe(names, batches)
-        return df
-
-def _column_batches_to_dataframe(names, batches):
-    cols = {}
-    for name, chunks in zip(names, zip(*[b.columns for b in batches])):
-        cols[name] = _chunks_to_pandas_array(chunks)
-    return pd.DataFrame(cols, columns=names)
+    return sch.Schema(ibis_fields)
 
 
 def _chunks_to_pandas_array(chunks):
     total_length = 0
     have_nulls = False
     for c in chunks:
         total_length += len(c)
         have_nulls = have_nulls or c.nulls.any()
 
     type_ = chunks[0].data_type
-    numpy_type = _HS2_TTypeId_to_dtype[type_]
+    numpy_type = ibis.backends.impala._HS2_TTypeId_to_dtype[type_]
 
     def fill_nonnull(target, chunks):
         pos = 0
         for c in chunks:
             target[pos : pos + len(c)] = c.values
             pos += len(c.values)
 
     def fill(target, chunks, na_rep):
         pos = 0
         for c in chunks:
             nulls = c.nulls.copy()
             nulls.bytereverse()
-            bits = np.frombuffer(nulls.tobytes(), dtype='u1')
+            bits = np.frombuffer(nulls.tobytes(), dtype="u1")
             mask = np.unpackbits(bits).view(np.bool_)
 
             k = len(c)
 
             dest = target[pos : pos + k]
             dest[:] = c.values
             dest[mask[:k]] = na_rep
 
             pos += k
 
     if have_nulls:
-        if numpy_type in ('bool', 'datetime64[ns]'):
-            target = np.empty(total_length, dtype='O')
+        # Updating NaN to None for consistency across DBs as per #406
+        if numpy_type in ("bool", "datetime64[ns]"):
+            target = np.empty(total_length, dtype="O")
             na_rep = None
-        elif numpy_type.startswith('int'):
-            target = np.empty(total_length, dtype='f8')
+        elif numpy_type.startswith("int"):
+            target = np.empty(total_length, dtype="f8")
             na_rep = np.nan
-        elif numpy_type in ('object'):
+        elif numpy_type in ("object"):
             target = np.empty(total_length, dtype=object)
             na_rep = None
         else:
             target = np.empty(total_length, dtype=numpy_type)
             na_rep = np.nan
 
         fill(target, chunks, na_rep)
     else:
         target = np.empty(total_length, dtype=numpy_type)
         fill_nonnull(target, chunks)
 
     return target
 
+
 @rewrites(ops.IfNull)
-def _if_null(expr):
-    arg, fill_value = expr.op().args
-    return arg.coalesce(fill_value)
+def _if_null(op):
+    return ops.Coalesce((op.arg, op.ifnull_expr))
+
 
 def _get_schema_using_query(self, query):
-    with self._execute(query, results=True) as cur:
-        # resets the state of the cursor and closes operation
-        cur.fetchall()
-        names, ibis_types = self._adapt_types(cur.description)
-
-    # per #321; most Impala tables will be lower case already, but Avro
-    # data, depending on the version of Impala, might have field names in
-    # the metastore cased according to the explicit case in the declared
-    # avro schema. This is very annoying, so it's easier to just conform on
-    # all lowercase fields from Impala.
-    names = [x[3:].lower() for x in names]
+    # Removing LIMIT 0 around query since it returns no results in Hive
+    cur = self.raw_sql(query)
+    cur.fetchall()
+    ibis_fields = self._adapt_types(cur.description)
+    cur.release()
+
+    return sch.Schema(ibis_fields)
 
-    return sch.Schema(names, ibis_types)
 
 udf.parse_type = parse_type
-ImpalaClient.get_schema = get_schema
-ImpalaQuery._fetch = _fetch
-ImpalaClient._get_schema_using_query = _get_schema_using_query
+ibis.backends.impala._chunks_to_pandas_array = _chunks_to_pandas_array
+ImpalaBackend.get_schema = get_schema
+ImpalaBackend._get_schema_using_query = _get_schema_using_query
+ImpalaBackend.do_connect = do_connect
+
+def impala_connect(
+    host: str = "localhost",
+    port: int = 10000,
+    database: str = "default",
+    timeout: int = 45,
+    use_ssl: bool = False,
+    ca_cert: str = None,
+    user: str = None,
+    password: str = None,
+    auth_mechanism: Literal["NOSASL", "PLAIN", "GSSAPI", "LDAP"] = "PLAIN",
+    kerberos_service_name: str = "impala",
+    pool_size: int = 8,
+    hdfs_client: fsspec.spec.AbstractFileSystem = None,
+    use_http_transport: bool = False,
+    http_path: str = "",
+):
+    backend = ibis.impala.connect(
+        host=host,
+        port=port,
+        database=database,
+        timeout=timeout,
+        use_ssl=use_ssl,
+        ca_cert=ca_cert,
+        user=user,
+        password=password,
+        auth_mechanism=auth_mechanism,
+        kerberos_service_name=kerberos_service_name,
+        pool_size=pool_size,
+        hdfs_client=hdfs_client,
+        use_http_transport=use_http_transport,
+        http_path=http_path,
+    )
+    return backend
```

### Comparing `google-pso-data-validator-3.2.0/third_party/ibis/ibis_mssql/compiler.py` & `google-pso-data-validator-4.0.0/third_party/ibis/ibis_oracle/registry.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,518 +8,451 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-import math
+import functools
+import itertools
+import locale
+import platform
+import re
+import string
+import warnings
+import operator
 
 import sqlalchemy as sa
-import sqlalchemy.dialects.mssql as mssql
 
 import ibis.common.exceptions as com
-import ibis.expr.datatypes as dt
 import ibis.expr.operations as ops
-import ibis.expr.window as W
-import third_party.ibis.ibis_mssql.expr.operations as ms_ops
-import ibis.backends.base_sqlalchemy.alchemy as alch
-
-from ibis import literal as L
-from ibis.backends.base_sqlalchemy.alchemy import fixed_arity, unary, _cumulative_to_reduction
-
-
-def raise_unsupported_op_error(translator, expr, *args):
-    msg = "SQLServer backend doesn't support {} operation!"
-    op = expr.op()
-    raise com.UnsupportedOperationError(msg.format(type(op)))
-
-
-def _reduction(func_name, cast_type='int32'):
-    def reduction_compiler(t, expr):
-        arg, where = expr.op().args
-
-        if arg.type().equals(dt.boolean):
-            arg = arg.cast(cast_type)
 
-        func = getattr(sa.func, func_name)
-
-        if where is not None:
-            arg = where.ifelse(arg, None)
-        return func(t.translate(arg))
-
-    return reduction_compiler
-
-
-def _reduction_count(sa_func):
-    def formatter(t, expr):
-        op = expr.op()
-        *args, where = op.args
+from ibis.backends.base.sql.alchemy import (
+    fixed_arity,
+    sqlalchemy_operation_registry,
+    sqlalchemy_window_functions_registry,
+    unary,
+    get_sqla_table,
+)
 
-        return _reduction_format(t, sa_func, where, *args)
+operation_registry = sqlalchemy_operation_registry.copy()
+operation_registry.update(sqlalchemy_window_functions_registry)
 
-    return formatter
 
+def _substr(t, op):
+    f = sa.func.substr
+    sa_arg = t.translate(op.arg)
+    sa_start = t.translate(op.start)
 
-def _reduction_format(t, sa_func, where, arg, *args):
-    if where is not None:
-        arg = t.translate(where.ifelse(arg, None))
+    if op.length is None:
+        return f(sa_arg, sa_start + 1)
     else:
-        arg = t.translate(arg)
-
-    return sa_func(arg, *map(t.translate, args))
-
-
-def _variance_reduction(func_name):
-    suffix = {'sample': '', 'pop': 'p'}
-
-    def variance_compiler(t, expr):
-        arg, how, where = expr.op().args
-
-        if arg.type().equals(dt.boolean):
-            arg = arg.cast('int32')
-
-        func = getattr(sa.func, '{}{}'.format(func_name, suffix.get(how, '')))
+        sa_length = t.translate(op.length)
+        return f(sa_arg, sa_start + 1, sa_length)
 
-        if where is not None:
-            arg = where.ifelse(arg, None)
-        return func(t.translate(arg))
 
-    return variance_compiler
+def _string_find(t, op):
+    if op.start is not None:
+        raise NotImplementedError
 
+    sa_arg = t.translate(op.arg)
+    sa_substr = t.translate(op.substr)
 
-def _substr(t, expr):
-    f = sa.func.substring
+    return sa.func.instr(sa_arg, sa_substr)
 
-    arg, start, length = expr.op().args
 
-    sa_arg = t.translate(arg)
-    sa_start = t.translate(start)
+def _extract(fmt: str):
+    def translator(t, op: ops.Node):
+        return sa.cast(sa.extract(fmt, t.translate(op.arg)), sa.SMALLINT)
 
-    if length is None:
-        return f(sa_arg, sa_start + 1)
-    else:
-        sa_length = t.translate(length)
-        return f(sa_arg, sa_start + 1, sa_length)
+    return translator
 
 
-def _string_find(t, expr):
-    arg, substr, start, _ = expr.op().args
+def _second(t, op):
+    # extracting the second gives us the fractional part as well, so smash that
+    # with a cast to SMALLINT
+    return sa.cast(sa.func.FLOOR(sa.extract('second', t.translate(op.arg))), sa.SMALLINT)
+
+
+_truncate_precisions = {
+    'us': 'microseconds',
+    'ms': 'milliseconds',
+    's': 'second',
+    'm': 'minute',
+    'h': 'hour',
+    'D': 'day',
+    'W': 'week',
+    'M': 'month',
+    'Q': 'quarter',
+    'Y': 'year',
+}
+
+
+def _timestamp_truncate(t, op):
+    arg = t.translate(op.arg)
+    unit = op.unit
+    if unit not in _truncate_precisions:
+        raise com.UnsupportedOperationError(f'Unsupported truncate unit {op.unit!r}')
+
+    return sa.func.datetrunc(sa.text(_truncate_precisions[unit]), arg)
+
+
+def _cast(t, op):
+    arg = op.arg
+    typ = op.to
+    arg_dtype = arg.output_dtype
 
     sa_arg = t.translate(arg)
-    sa_substr = t.translate(substr)
 
-    if start is not None:
-        sa_start = t.translate(start)
-        return sa.func.charindex(sa_substr, sa_arg, sa_start) - 1
+    # specialize going from an integer type to a timestamp
+    if arg_dtype.is_integer() and typ.is_timestamp():
+        return t.integer_to_timestamp(sa_arg, tz=typ.timezone)
+
+    if arg_dtype.is_binary() and typ.is_string():
+        return sa.func.encode(sa_arg, 'escape')
+
+    if typ.is_binary():
+        #  decode yields a column of memoryview which is annoying to deal with
+        # in pandas. CAST(expr AS BYTEA) is correct and returns byte strings.
+        return sa.cast(sa_arg, sa.LargeBinary())
+
+    if typ.is_json() and not t.native_json_type:
+        return sa_arg
+
+    return sa.cast(sa_arg, t.get_sqla_type(typ))
+
+
+def _typeof(t, op):
+    sa_arg = t.translate(op.arg)
+    typ = sa.func.dump(sa_arg)
+    return typ
+
+
+def _string_agg(t, op):
+    agg = sa.func.string_agg(t.translate(op.arg), t.translate(op.sep))
+    if (where := op.where) is not None:
+        return agg.filter(t.translate(where))
+    return agg
+
+
+_strftime_to_oracle_rules = {
+    '%a': 'TMDy',  # TM does it in a locale dependent way
+    '%A': 'TMDay',
+    '%b': 'TMMon',  # Sep
+    '%B': 'TMMonth',  # September
+    '%d': 'DD',  # day of month
+    '%H': 'HH24',  # 09
+    '%I': 'HH12',  # 09
+    '%j': 'DDD',  # zero padded day of year
+    '%m': 'MM',  # 01
+    '%M': 'MI',  # zero padded minute
+    '%p': 'AM',  # AM or PM
+    '%S': 'SS',  # zero padded second
+    '%U': 'WW',  # 1-based week of year
+    '%w': 'D',
+    '%y': 'YY',  # 15
+    '%Y': 'YYYY',  # 2015
+    '%Z': 'TZ',  # uppercase timezone name
+}
 
-    return sa.func.charindex(sa_substr, sa_arg) - 1
+try:
 
+    _strftime_to_oracle_rules.update(
+        {
+            '%c': locale.nl_langinfo(locale.D_T_FMT),  # locale date and time
+            '%x': locale.nl_langinfo(locale.D_FMT),  # locale date
+            '%X': locale.nl_langinfo(locale.T_FMT),  # locale time
+        }
+    )
+except AttributeError:
+    warnings.warn(
+        'locale specific date formats (%%c, %%x, %%X) are not yet implemented '
+        'for %s' % platform.system()
+    )
 
-def _string_contains(t, expr):
-    arg, substr, start, _ = expr.op().args
-
-    sa_arg = t.translate(arg)
-    sa_substr = t.translate(substr)
-
-    if start is not None:
-        sa_start = t.translate(start)
-        return sa.func.charindex(sa_substr, sa_arg, sa_start) - 1
-
-    variable = sa.func.charindex(sa_substr, sa_arg) - 1
-    return sa.case([((variable >= 0), 1)], else_=0,)
 
+# translate strftime spec into mostly equivalent Oracle spec
+_scanner = re.Scanner(
+    # double quotes need to be escaped
+    [('"', lambda scanner, token: r'\"')]
+    + [
+        (
+            '|'.join(
+                map(
+                    '(?:{})'.format,
+                    itertools.chain(
+                        _strftime_to_oracle_rules.keys(),
+                        [
+                            # "%e" is in the C standard and Python actually
+                            # generates this if your spec contains "%c" but we
+                            # don't officially support it as a specifier so we
+                            # need to special case it in the scanner
+                            '%e',
+                            r'\s+',
+                            r'[{}]'.format(re.escape(string.punctuation)),
+                            r'[^{}\s]+'.format(re.escape(string.punctuation)),
+                        ],
+                    ),
+                )
+            ),
+            lambda scanner, token: token,
+        )
+    ]
+)
 
-def _string_like1(t, expr):
-    arg, pattern, escape = expr.op().args
-    result = t.translate(arg).like(t.translate(pattern), escape=escape)
-    return sa.case([(result, 1)], else_=0,)
 
+_lexicon_values = frozenset(_strftime_to_oracle_rules.values())
 
-def _strftime(t, expr):
-    """Use MS SQL CONVERT() in place of STRFTIME().
+_strftime_blacklist = frozenset(['%w', '%U', '%c', '%x', '%X', '%e'])
 
-    This is pretty restrictive due to the limited styles offered by SQL Server,
-    we've just covered off the generic formats used when casting date based columns
-    to string in order to complete row data comparison."""
-    arg, pattern = map(t.translate, expr.op().args)
-    supported_convert_styles = {
-        "%Y-%m-%d": 23, # ISO8601
-        "%Y-%m-%d %H:%M:%S": 20, # ODBC canonical
-        "%Y-%m-%d %H:%M:%S.%f": 21, # ODBC canonical (with milliseconds)
-    }
-    try:
-        convert_style = supported_convert_styles[pattern.value]
-    except KeyError:
-        raise NotImplementedError(
-            f'strftime format {pattern.value} not supported for SQL Server.'
-        )
-    result = sa.func.convert(sa.text('VARCHAR(32)'), arg, convert_style)
-    return result
 
+def _reduce_tokens(tokens, arg):
+    # current list of tokens
+    curtokens = []
 
-def _floor_divide(t, expr):
-    left, right = map(t.translate, expr.op().args)
-    return sa.func.floor(left / right)
+    # reduced list of tokens that accounts for blacklisted values
+    reduced = []
 
+    non_special_tokens = (
+        frozenset(_strftime_to_oracle_rules) - _strftime_blacklist
+    )
 
-def _extract(fmt):
-    def translator(t, expr):
-        (arg,) = expr.op().args
-        sa_arg = t.translate(arg)
-        return sa.cast(
-            sa.func.datepart(sa.literal_column(fmt), sa_arg), sa.SMALLINT
-        )
-
-    return translator
+    # TODO: how much of a hack is this?
+    for token in tokens:
+        # we are a non-special token %A, %d, etc.
+        if token in non_special_tokens:
+            curtokens.append(_strftime_to_oracle_rules[token])
+
+        # we have a string like DD, to escape this we
+        # surround it with double quotes
+        elif token in _lexicon_values:
+            curtokens.append('"{}"'.format(token))
+
+        # we have a token that needs special treatment
+        elif token in _strftime_blacklist:
+            if token == '%w':
+                value = sa.extract('dow', arg)  # 0 based day of week
+            elif token == '%U':
+                value = sa.cast(sa.func.to_char(arg, 'WW'), sa.SMALLINT) - 1
+            elif token == '%c' or token == '%x' or token == '%X':
+                # re scan and tokenize this pattern
+                try:
+                    new_pattern = _strftime_to_oracle_rules[token]
+                except KeyError:
+                    raise ValueError(
+                        'locale specific date formats (%%c, %%x, %%X) are '
+                        'not yet implemented for %s' % platform.system()
+                    )
+
+                new_tokens, _ = _scanner.scan(new_pattern)
+                value = functools.reduce(
+                    sa.sql.ColumnElement.concat,
+                    _reduce_tokens(new_tokens, arg),
+                )
+            elif token == '%e':
+                # pad with spaces instead of zeros
+                value = sa.func.replace(sa.func.to_char(arg, 'DD'), '0', ' ')
+
+            reduced += [
+                sa.func.to_char(arg, ''.join(curtokens)),
+                sa.cast(value, sa.TEXT),
+            ]
+
+            # empty current token list in case there are more tokens
+            del curtokens[:]
+
+        # uninteresting text
+        else:
+            curtokens.append(token)
+    else:
+        # append result to r if we had more tokens or if we have no
+        # blacklisted tokens
+        if curtokens:
+            reduced.append(sa.func.to_char(arg, ''.join(curtokens)))
+    return reduced
 
 
-def _round(t, expr):
-    op = expr.op()
-    arg, digits = op.args
-    sa_arg = t.translate(arg)
+def _strftime(t, op):
+    tokens, _ = _scanner.scan(op.format_str.value)
+    reduced = _reduce_tokens(tokens, t.translate(op.arg))
+    return functools.reduce(sa.sql.ColumnElement.concat, reduced)
 
-    f = sa.func.round
 
-    if digits is not None:
-        sa_digits = t.translate(digits)
-        return f(sa_arg, sa_digits)
-    else:
-        return f(sa_arg)
+def _regex_replace(t, op):
+    return sa.func.regexp_replace(t.translate(op.string), t.translate(op.pattern), t.translate(op.replacement))
 
 
-def _log(t, expr):
-    arg, base = expr.op().args
+def _log(t, op):
+    arg, base = op.args
     sa_arg = t.translate(arg)
     if base is not None:
         sa_base = t.translate(base)
         return sa.cast(
-            sa.func.log(
-                sa.cast(sa_arg, sa.NUMERIC), sa.cast(sa_base, sa.NUMERIC)
-            ),
-            t.get_sqla_type(expr.type()),
+            sa.func.log(sa.cast(sa_base, sa.NUMERIC), sa.cast(sa_arg, sa.NUMERIC)),
+            t.get_sqla_type(op.output_dtype),
         )
     return sa.func.ln(sa_arg)
 
 
-def _cumulative_to_window(translator, expr, window):
-    win = W.cumulative_window()
-    win = win.group_by(window._group_by).order_by(window._order_by)
-
-    op = expr.op()
-
-    klass = _cumulative_to_reduction[type(op)]
-    new_op = klass(*op.args)
-    new_expr = expr._factory(new_op, name=expr._name)
-
-    if type(new_op) in translator._rewrites:
-        new_expr = translator._rewrites[type(new_op)](new_expr)
-
-    return L.windowize_function(new_expr, win)
-
-
-def _window(t, expr):
-    op = expr.op()
-
-    arg, window = op.args
-    reduction = t.translate(arg)
-
-    window_op = arg.op()
-
-    if isinstance(window_op, (ops.Sum, ops.Mean, ops.Min, ops.Max)):
-        msg = """SQLServer backend doesn't support {}
-         operation with Window Function!"""
-        raise com.UnsupportedOperationError(msg.format(type(window_op)))
-
-    _require_order_by = (
-        ops.DenseRank,
-        ops.MinRank,
-        ops.NTile,
-        ops.PercentRank,
-        ops.Count,
-        ops.Mean,
-        ops.Min,
-        ops.Max,
-        ops.Sum,
-        ops.FirstValue,
-        ops.LastValue,
-        ops.Lag,
-        ops.Lead,
-    )
+def _regex_extract(t, op):
+    return sa.func.regex_extract(t.translate(op.string), t.translate(op.pattern), t.translate(op.index +1))
 
-    if isinstance(window_op, ops.CumulativeOp):
-        arg = _cumulative_to_window(t, arg, window)
-        return t.translate(arg)
-
-    if window.max_lookback is not None:
-        raise NotImplementedError(
-            'Rows with max lookback is not implemented '
-            'for SQLAlchemy-based backends.'
-        )
 
-    if isinstance(window_op, _require_order_by) and not window._order_by:
-        order_by = t.translate(window_op.args[0])
-    else:
-        order_by = list(map(t.translate, window._order_by))
+def get_col(sa_table, op: ops.TableColumn):
+    """Extract a column from a table."""
+    cols = sa_table.exported_columns
+    colname = op.name
+
+    if (col := cols.get(colname)) is not None:
+        return col
+
+    # `cols` is a SQLAlchemy column collection that contains columns
+    # with names that are secretly prefixed by table that contains them
+    #
+    # for example, in `t0.join(t1).select(t0.a, t1.b)` t0.a will be named `t0_a`
+    # and t1.b will be named `t1_b`
+    #
+    # unfortunately SQLAlchemy doesn't let you select by the *un*prefixed
+    # column name despite the uniqueness of `colname`
+    #
+    # however, in ibis we have already deduplicated column names so we can
+    # refer to the name by position
+    colindex = op.table.schema._name_locs[colname]
+    return cols[colindex]
+
+
+def _table_column(t, op):
+    ctx = t.context
+    table = op.table
+
+    sa_table = get_sqla_table(ctx, table)
+
+    out_expr = get_col(sa_table, op)
+    out_expr.quote = t._quote_column_names
+
+    # If the column does not originate from the table set in the current SELECT
+    # context, we should format as a subquery
+    if t.permit_subquery and ctx.is_foreign_expr(table):
+        try:
+            subq = sa_table.subquery()
+        except AttributeError:
+            subq = sa_table
+        return sa.select(subq.c[out_expr.name])
 
-    partition_by = list(map(t.translate, window._group_by))
+    return out_expr
 
-    frame_clause_not_allowed = (
-        ops.Lag,
-        ops.Lead,
-        ops.DenseRank,
-        ops.MinRank,
-        ops.NTile,
-        ops.PercentRank,
-        ops.RowNumber,
-    )
 
-    how = {'range': 'range_'}.get(window.how, window.how)
-    preceding = window.preceding
-    additional_params = (
-        {}
-        if isinstance(window_op, frame_clause_not_allowed)
-        else {
-            how: (
-                -preceding if preceding is not None else preceding,
-                window.following,
-            )
-        }
-    )
-    result = reduction.over(
-        partition_by=partition_by, order_by=order_by, **additional_params
-    )
+def _round(t, op):
+    sa_arg = t.translate(op.arg)
 
-    if isinstance(
-        window_op, (ops.RowNumber, ops.DenseRank, ops.MinRank, ops.NTile)
-    ):
-        return result - 1
+    if op.digits is not None:
+        return sa.func.round(sa_arg, t.translate(op.digits))
     else:
-        return result
+        return sa.func.round(sa_arg)
 
 
-def _lag(t, expr):
-    arg, offset, default = expr.op().args
-    if default is not None:
-        raise NotImplementedError()
-
-    sa_arg = t.translate(arg)
-    sa_offset = t.translate(offset) if offset is not None else 1
-    return sa.func.lag(sa_arg, sa_offset)
-
 
-def _lead(t, expr):
-    arg, offset, default = expr.op().args
-    if default is not None:
-        raise NotImplementedError()
-    sa_arg = t.translate(arg)
-    sa_offset = t.translate(offset) if offset is not None else 1
-    return sa.func.lead(sa_arg, sa_offset)
-
-
-def _ntile(t, expr):
-    op = expr.op()
-    args = op.args
-    arg, buckets = map(t.translate, args)
-    return sa.func.ntile(buckets)
-
-
-def _hll_cardinality(t, expr):
-    arg, _ = expr.op().args
-    sa_arg = t.translate(arg)
-    return sa.func.count(sa.distinct(sa_arg))
+def _string_join(t, op):
+    sep, elements = op.args
+    columns = [str(col.name) for col in map(t.translate, elements)]
+    return sa.sql.literal_column(" || ".join(columns))
 
 
-def _is_null1(t, expr):
-    arg = t.translate(expr.op().args[0])
-    res = arg.is_(sa.null())
-    return sa.case([(res, 1)], else_=0)
+def _literal(t, op):
+    dtype = op.output_dtype
+    value = op.value
 
+    if dtype.is_interval():
+        return sa.literal_column(f"INTERVAL '{value} {dtype.resolution}'")
+    elif dtype.is_set():
+        return list(map(sa.literal, value))
+    elif dtype.is_array():
+        return pg.array(value)
+    elif dtype.is_map():
+        return pg.hstore(list(value.keys()), list(value.values()))
+    else:
+        return sa.literal(value)
 
-def _not_null1(t, expr):
-    arg = t.translate(expr.op().args[0])
-    res = arg.isnot(sa.null())
-    return sa.case([(res, 1)], else_=0)
-
-
-def _not_any1(t, expr):
-    arg = t.translate(expr.op().args[0])
-    res = sa.func.max(sa.cast(arg, sa.INTEGER))
-    return sa.case([(res > 0, 0)], else_=1)
-
-
-def _not_all1(t, expr):
-    arg = t.translate(expr.op().args[0])
-    res = sa.func.min(sa.cast(arg, sa.INTEGER))
-    return sa.case([(res > 0, 0)], else_=1)
-
-
-def _between(t, expr):
-    (arg, lower, upper,) = map(t.translate, expr.op().args)
-    res = arg.between(lower, upper)
-    return sa.case([(res, 1)], else_=0)
-
-
-def _day_of_week_index(t, expr):
-    (sa_arg,) = map(t.translate, expr.op().args)
-    return sa.cast(
-        sa.cast(sa.extract('dow', sa_arg) + 5, sa.SMALLINT) % 7, sa.SMALLINT
-    )
-
+def _day_of_week_index(t, op):
+    return sa.func.to_char(t.translate(op.arg), 'd')
 
-def _day_of_week_name(t, expr):
-    (sa_arg,) = map(t.translate, expr.op().args)
-    return sa.func.trim(sa.func.format(sa_arg, 'dddd'))
 
+def _day_of_week_name(t, op):
+    return sa.func.to_char(t.translate(op.arg), 'Day')
 
-def _string_join(t, expr):
-    sep, elements = expr.op().args
-    return sa.func.concat(*map(t.translate, elements))
 
+def _random(t, op):
+    return sa.sql.literal_column("DBMS_RANDOM.VALUE")
 
-_operation_registry = alch._operation_registry.copy()
 
-_operation_registry.update(
+operation_registry.update(
     {
-        # aggregate methods
-        ops.Count: _reduction_count(sa.func.count),
-        ops.Max: _reduction('max'),
-        ops.Min: _reduction('min'),
-        ops.Sum: _reduction('sum'),
-        ops.Mean: _reduction('avg', 'float64'),
-        # string methods
-        ops.LStrip: unary(sa.func.ltrim),
-        ops.Lowercase: unary(sa.func.lower),
-        ops.RStrip: unary(sa.func.rtrim),
-        ops.Repeat: fixed_arity(sa.func.replicate, 2),
-        ops.Reverse: unary(sa.func.reverse),
+        ops.Literal: _literal,
+        # We override this here to support time zones
+        ops.TableColumn: _table_column,
+        # types
+        ops.Cast: _cast,
+        ops.TypeOf: _typeof,
+        # null handling
+        ops.IfNull: fixed_arity(sa.func.coalesce, 2),
+        # boolean reductions
+        ops.Any: unary(sa.func.bool_or),
+        ops.All: unary(sa.func.bool_and),
+        ops.NotAny: unary(lambda x: sa.not_(sa.func.bool_or(x))),
+        ops.NotAll: unary(lambda x: sa.not_(sa.func.bool_and(x))),
+        # strings
+        ops.Substring: _substr,
         ops.StringFind: _string_find,
-        ops.StringLength: unary(sa.func.length),
-        ops.StringReplace: fixed_arity(sa.func.replace, 3),
+        ops.GroupConcat: _string_agg,
+        ops.Capitalize: unary(sa.func.initcap),
+        ops.RegexSearch: fixed_arity(lambda x, y: x.op("~")(y), 2),
+        ops.RegexReplace: _regex_replace,
+        ops.Translate: fixed_arity('translate', 3),
+        ops.RegexExtract: _regex_extract,
         ops.StringJoin: _string_join,
-        ops.Strip: unary(sa.func.trim),
-        ops.Substring: _substr,
-        ops.Uppercase: unary(sa.func.upper),
         # math
-        ops.Abs: unary(sa.func.abs),
-        ops.Acos: unary(sa.func.acos),
-        ops.Asin: unary(sa.func.asin),
-        ops.Atan2: fixed_arity(sa.func.atn2, 2),
-        ops.Atan: unary(sa.func.atan),
-        ops.Ceil: unary(sa.func.ceiling),
-        ops.Cos: unary(sa.func.cos),
-        ops.Floor: unary(sa.func.floor),
-        ops.FloorDivide: _floor_divide,
+        ops.Log: _log,
+        ops.Log2: unary(lambda x: sa.func.log(2, x)),
+        ops.Log10: unary(sa.func.log),
+        ops.Round: _round,
+        ops.Modulus: fixed_arity(operator.mod, 2),
         ops.Power: fixed_arity(sa.func.power, 2),
-        ops.Sign: unary(sa.func.sign),
-        ops.Sin: unary(sa.func.sin),
-        ops.Sqrt: unary(sa.func.sqrt),
-        ops.Tan: unary(sa.func.tan),
-        # timestamp methods
-        ops.TimestampNow: fixed_arity(sa.func.GETDATE, 0),
+        # dates and times
+        ops.Date: unary(lambda x: sa.cast(x, sa.Date)),
+        ops.DateTruncate: _timestamp_truncate,
+        ops.TimestampTruncate: _timestamp_truncate,
+        ops.IntervalFromInteger: (
+            lambda t, op: t.translate(op.arg)
+            * sa.text(f"INTERVAL '1 {op.output_dtype.resolution}'")
+        ),
+        ops.DateAdd: fixed_arity(operator.add, 2),
+        ops.DateSub: fixed_arity(operator.sub, 2),
+        ops.DateDiff: fixed_arity(operator.sub, 2),
+        ops.TimestampAdd: fixed_arity(operator.add, 2),
+        ops.TimestampSub: fixed_arity(operator.sub, 2),
+        ops.TimestampDiff: fixed_arity(operator.sub, 2),
+        ops.Strftime: _strftime,
         ops.ExtractYear: _extract('year'),
         ops.ExtractMonth: _extract('month'),
         ops.ExtractDay: _extract('day'),
-        ops.ExtractDayOfYear: _extract('dayofyear'),
-        ops.ExtractHour: _extract('hour'),
-        ops.ExtractMinute: _extract('minute'),
-        ops.ExtractSecond: _extract('second'),
-        ops.ExtractMillisecond: _extract('millisecond'),
-        ops.ExtractWeekOfYear: _extract('iso_week'),
-        ops.Strftime: _strftime,
+        ops.ExtractDayOfYear: _extract('doy'),
+        ops.ExtractQuarter: _extract('quarter'),
         ops.ExtractEpochSeconds: fixed_arity(
             lambda x: sa.cast(
                 sa.func.datediff(sa.text('s'), '1970-01-01 00:00:00', x), sa.BIGINT
             ),
             1,
         ),
-        # newly added
-        ops.Lag: _lag,
-        ops.Lead: _lead,
-        ops.NTile: _ntile,
-        ops.FirstValue: unary(sa.func.first_value),
-        ops.LastValue: unary(sa.func.last_value),
-        ops.RowNumber: fixed_arity(lambda: sa.func.row_number(), 0),
-        ops.WindowOp: _window,
-        ops.CumulativeOp: _window,
+        ops.ExtractHour: _extract('hour'),
+        ops.ExtractMinute: _extract('minute'),
+        ops.ExtractSecond: _second,
         ops.DayOfWeekIndex: _day_of_week_index,
         ops.DayOfWeekName: _day_of_week_name,
-        ops.Round: _round,
-        ops.Log: _log,
-        ops.Log2: unary(lambda x: sa.func.log(x, 2)),
-        ops.Log10: unary(lambda x: sa.func.log(x, 10)),
-        ops.Ln: unary(lambda x: sa.func.log(x, math.e)),
-        ops.Exp: unary(sa.func.exp),
-        ops.StringAscii: unary(sa.func.ascii),
-        ops.Variance: _variance_reduction('var'),
-        ops.StandardDev: _variance_reduction('stdev'),
-        ms_ops.StringContains: _string_contains,
-        ms_ops.StringSQLLike: _string_like1,
-        ops.HLLCardinality: _hll_cardinality,
-        ms_ops.IsNull: _is_null1,
-        ms_ops.NotNull: _not_null1,
-        ops.DenseRank: unary(lambda arg: sa.func.dense_rank()),
-        ops.MinRank: unary(lambda arg: sa.func.rank()),
-        ops.PercentRank: unary(lambda arg: sa.func.percent_rank()),
-        ops.NullIf: fixed_arity(sa.func.nullif, 2),
-        ops.IfNull: fixed_arity(sa.func.isnull, 2),
-        ms_ops.Between: _between,
-        ops.Translate: fixed_arity('translate', 3),
-        ms_ops.NotAny: _not_any1,
-        ms_ops.NotAll: _not_all1,
+        ops.RandomScalar: _random,
+        # now is in the timezone of the server, but we want UTC
+        ops.TimestampNow: lambda *args: sa.func.timezone('UTC', sa.func.now()),
+
     }
 )
 
 
-_unsupported_ops = [
-    ops.NotAny,
-    ops.Least,
-    ops.Greatest,
-    ops.LPad,  # not supported by mssql
-    ops.RPad,  # not supported by mssql
-    ops.Capitalize,  # not supported by mssql
-    ops.RegexSearch,  # not supported by mssql
-    ops.RegexExtract,  # not supported by mssql
-    ops.RegexReplace,  # not supported by mssql
-    # aggregate methods
-    ops.CumulativeMax,
-    ops.CumulativeMin,
-    ops.CumulativeMean,
-    ops.CumulativeSum,
-    # datetime methods
-    ops.TimestampTruncate,
-]
-
-
-_unsupported_ops = {k: raise_unsupported_op_error for k in _unsupported_ops}
-_operation_registry.update(_unsupported_ops)
-
-
-class MSSQLExprTranslator(alch.AlchemyExprTranslator):
-    _registry = _operation_registry
-    _rewrites = alch.AlchemyExprTranslator._rewrites.copy()
-    _type_map = alch.AlchemyExprTranslator._type_map.copy()
-    # only used to map SQLAlchemy types back to SQL Server types, it does not add support to new data types, for that go to client.py
-    _type_map.update(
-        {
-            dt.Boolean: mssql.BIT,
-            dt.Int8: mssql.TINYINT,
-            dt.Int32: mssql.INTEGER,
-            dt.Int64: mssql.BIGINT,
-            dt.Float: mssql.REAL,
-            dt.Double: mssql.REAL,
-            dt.String: mssql.VARCHAR,
-        }
-    )
-
-
-rewrites = MSSQLExprTranslator.rewrites
-compiles = MSSQLExprTranslator.compiles
-
-
-class MSSQLDialect(alch.AlchemyDialect):
-
-      translator = MSSQLExprTranslator
-
 
-dialect = MSSQLDialect
```

### Comparing `google-pso-data-validator-3.2.0/third_party/ibis/ibis_oracle/api.py` & `google-pso-data-validator-4.0.0/third_party/ibis/ibis_mssql/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-# Copyright 2020 Google Inc.
+# Copyright 2023 Google Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Literal
 
-from third_party.ibis.ibis_oracle.client import OracleClient
-from third_party.ibis.ibis_oracle.compiler import (  # noqa: F401
-    dialect,
-    rewrites,
-)
+from third_party.ibis.ibis_mssql import Backend as MsSqlBackend
 
-from ibis.sql.alchemy import to_sqlalchemy
 
-
-def compile(expr, params=None):
-    return to_sqlalchemy(expr, dialect.make_context(params=params))
-
-
-def connect(
-    host=None, port=None, user=None, password=None, database=None, protocol='TCP', url=None, driver='cx_Oracle',
+def mssql_connect(
+    host: str = "localhost",
+    user: str = None,
+    password: str = None,
+    port: int = 1433,
+    database: str = None,
+    url: str = None,
+    driver: Literal["pyodbc"] = "pyodbc",
+    odbc_driver: str = "ODBC Driver 17 for SQL Server",
 ):
-
-    return OracleClient(
+    backend = MsSqlBackend()
+    backend.do_connect(
         host=host,
         port=port,
         user=user,
         password=password,
         database=database,
-        protocol=protocol,
         url=url,
         driver=driver,
+        odbc_driver=odbc_driver,
     )
+    return backend
```

