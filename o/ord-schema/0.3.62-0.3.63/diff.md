# Comparing `tmp/ord-schema-0.3.62.tar.gz` & `tmp/ord-schema-0.3.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord-schema-0.3.62.tar", last modified: Wed Jul 19 23:26:59 2023, max compression
+gzip compressed data, was "ord-schema-0.3.63.tar", last modified: Wed Aug  2 19:40:00 2023, max compression
```

## Comparing `ord-schema-0.3.62.tar` & `ord-schema-0.3.63.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:26:59.001477 ord-schema-0.3.62/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-19 23:26:38.000000 ord-schema-0.3.62/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 23:26:38.000000 ord-schema-0.3.62/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 23:26:38.000000 ord-schema-0.3.62/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-19 23:26:59.001477 ord-schema-0.3.62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-19 23:26:38.000000 ord-schema-0.3.62/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:26:58.997477 ord-schema-0.3.62/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:26:58.997477 ord-schema-0.3.62/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:26:58.997477 ord-schema-0.3.62/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:26:58.997477 ord-schema-0.3.62/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49196 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:26:59.001477 ord-schema-0.3.62/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45675 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-07-19 23:26:38.000000 ord-schema-0.3.62/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:26:58.997477 ord-schema-0.3.62/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-19 23:26:58.000000 ord-schema-0.3.62/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-19 23:26:58.000000 ord-schema-0.3.62/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 23:26:58.000000 ord-schema-0.3.62/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-19 23:26:58.000000 ord-schema-0.3.62/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 23:26:58.000000 ord-schema-0.3.62/ord_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:26:59.001477 ord-schema-0.3.62/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-19 23:26:38.000000 ord-schema-0.3.62/proto/dataset.proto
--rw-r--r--   0 runner    (1001) docker     (123)    46742 2023-07-19 23:26:38.000000 ord-schema-0.3.62/proto/reaction.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-19 23:26:38.000000 ord-schema-0.3.62/proto/test.proto
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-19 23:26:38.000000 ord-schema-0.3.62/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 23:26:59.001477 ord-schema-0.3.62/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-19 23:26:40.000000 ord-schema-0.3.62/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:00.235887 ord-schema-0.3.63/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-02 19:39:35.000000 ord-schema-0.3.63/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 19:39:35.000000 ord-schema-0.3.63/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 19:39:35.000000 ord-schema-0.3.63/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-02 19:40:00.231887 ord-schema-0.3.63/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-02 19:39:35.000000 ord-schema-0.3.63/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:00.227887 ord-schema-0.3.63/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:00.227887 ord-schema-0.3.63/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:00.231887 ord-schema-0.3.63/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:00.231887 ord-schema-0.3.63/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49196 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:00.231887 ord-schema-0.3.63/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21548 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45674 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21618 2023-08-02 19:39:35.000000 ord-schema-0.3.63/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:00.227887 ord-schema-0.3.63/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-02 19:40:00.000000 ord-schema-0.3.63/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-02 19:40:00.000000 ord-schema-0.3.63/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:40:00.000000 ord-schema-0.3.63/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-02 19:40:00.000000 ord-schema-0.3.63/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 19:40:00.000000 ord-schema-0.3.63/ord_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:40:00.231887 ord-schema-0.3.63/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-08-02 19:39:35.000000 ord-schema-0.3.63/proto/dataset.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    46742 2023-08-02 19:39:35.000000 ord-schema-0.3.63/proto/reaction.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-02 19:39:35.000000 ord-schema-0.3.63/proto/test.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 19:39:35.000000 ord-schema-0.3.63/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:40:00.235887 ord-schema-0.3.63/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-08-02 19:39:41.000000 ord-schema-0.3.63/setup.py
```

### Comparing `ord-schema-0.3.62/LICENSE` & `ord-schema-0.3.63/LICENSE`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/PKG-INFO` & `ord-schema-0.3.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.62
+Version: 0.3.63
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.62/README.md` & `ord-schema-0.3.63/README.md`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/__init__.py` & `ord-schema-0.3.63/ord_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/frozen_message.py` & `ord-schema-0.3.63/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/frozen_message_test.py` & `ord-schema-0.3.63/ord_schema/frozen_message_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/logging.py` & `ord-schema-0.3.63/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/macros/__init__.py` & `ord-schema-0.3.63/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/macros/solutions.py` & `ord-schema-0.3.63/ord_schema/macros/solutions.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/macros/solutions_test.py` & `ord-schema-0.3.63/ord_schema/macros/solutions_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/macros/workups.py` & `ord-schema-0.3.63/ord_schema/macros/workups.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/message_helpers.py` & `ord-schema-0.3.63/ord_schema/message_helpers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/message_helpers_test.py` & `ord-schema-0.3.63/ord_schema/message_helpers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/orm/__init__.py` & `ord-schema-0.3.63/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/orm/conftest.py` & `ord-schema-0.3.63/ord_schema/orm/conftest.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/orm/database.py` & `ord-schema-0.3.63/ord_schema/orm/database.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/orm/database_test.py` & `ord-schema-0.3.63/ord_schema/orm/database_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/orm/mappers.py` & `ord-schema-0.3.63/ord_schema/orm/mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/orm/mappers_test.py` & `ord-schema-0.3.63/ord_schema/orm/mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/orm/rdkit_mappers.py` & `ord-schema-0.3.63/ord_schema/orm/rdkit_mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/orm/rdkit_mappers_test.py` & `ord-schema-0.3.63/ord_schema/orm/rdkit_mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/proto/__init__.py` & `ord-schema-0.3.63/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/proto/dataset_pb2.py` & `ord-schema-0.3.63/ord_schema/proto/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/proto/dataset_pb2_test.py` & `ord-schema-0.3.63/ord_schema/proto/dataset_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/proto/reaction_pb2.py` & `ord-schema-0.3.63/ord_schema/proto/reaction_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/proto/reaction_pb2_test.py` & `ord-schema-0.3.63/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/proto/test_pb2.py` & `ord-schema-0.3.63/ord_schema/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/resolvers.py` & `ord-schema-0.3.63/ord_schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/resolvers_test.py` & `ord-schema-0.3.63/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/scripts/__init__.py` & `ord-schema-0.3.63/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/scripts/build_dataset.py` & `ord-schema-0.3.63/ord_schema/scripts/build_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/scripts/build_dataset_test.py` & `ord-schema-0.3.63/ord_schema/scripts/build_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/scripts/check_pb.py` & `ord-schema-0.3.63/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/scripts/check_pb_test.py` & `ord-schema-0.3.63/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/scripts/enumerate_dataset.py` & `ord-schema-0.3.63/ord_schema/scripts/enumerate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/scripts/enumerate_dataset_test.py` & `ord-schema-0.3.63/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/scripts/parse_uspto.py` & `ord-schema-0.3.63/ord_schema/scripts/parse_uspto.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/scripts/process_dataset.py` & `ord-schema-0.3.63/ord_schema/scripts/process_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/scripts/process_dataset_test.py` & `ord-schema-0.3.63/ord_schema/scripts/process_dataset_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
         assert filenames == [dataset_filename]
 
     def test_add_dataset_with_validation_errors(self, setup):
         test_subdirectory, _ = setup
         reaction = reaction_pb2.Reaction()
         ethylamine = reaction.inputs["ethylamine"]
         component = ethylamine.components.add()
-        component.identifiers.add(type="SMILES", value="C#O")
+        component.identifiers.add(type="SMILES", value="#")
         component.is_limiting = True
         component.amount.moles.value = 2
         component.amount.moles.units = reaction_pb2.Moles.MILLIMOLE
         reaction.outcomes.add().conversion.value = 25
         dataset = dataset_pb2.Dataset(reactions=[reaction])
         dataset_filename = os.path.join(test_subdirectory, "test.pbtxt")
         message_helpers.write_message(dataset, dataset_filename)
@@ -374,15 +374,15 @@
         reaction.outcomes.add().conversion.value = 25
         reaction.provenance.record_created.time.value = "2021-02-09"
         reaction.provenance.record_created.person.username = "bob"
         reaction.provenance.record_created.person.email = "bob@bob.com"
         dataset1 = dataset_pb2.Dataset(reactions=[reaction])
         dataset1_filename = os.path.join(test_subdirectory, "test1.pbtxt")
         message_helpers.write_message(dataset1, dataset1_filename)
-        reaction.inputs["ethylamine"].components[0].identifiers[0].value = "C#O"
+        reaction.inputs["ethylamine"].components[0].identifiers[0].value = "#"
         dataset2 = dataset_pb2.Dataset(reactions=[reaction])
         dataset2_filename = os.path.join(test_subdirectory, "test2.pbtxt")
         message_helpers.write_message(dataset2, dataset2_filename)
         with pytest.raises(validations.ValidationError, match="could not validate SMILES"):
             self._run(test_subdirectory)
 
     def test_modify_dataset_with_validation_errors(self, setup):
```

### Comparing `ord-schema-0.3.62/ord_schema/scripts/validate_dataset.py` & `ord-schema-0.3.63/ord_schema/scripts/validate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/scripts/validate_dataset_test.py` & `ord-schema-0.3.63/ord_schema/scripts/validate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/templating.py` & `ord-schema-0.3.63/ord_schema/templating.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/templating_test.py` & `ord-schema-0.3.63/ord_schema/templating_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/units.py` & `ord-schema-0.3.63/ord_schema/units.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/units_test.py` & `ord-schema-0.3.63/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/updates.py` & `ord-schema-0.3.63/ord_schema/updates.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/updates_test.py` & `ord-schema-0.3.63/ord_schema/updates_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema/validations.py` & `ord-schema-0.3.63/ord_schema/validations.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,35 +571,31 @@
         )
 
 
 def validate_compound_identifier(message: reaction_pb2.CompoundIdentifier):
     check_type_and_details(message)
     if not message.value:
         warnings.warn("value must be set", ValidationError)
-    if message.type == message.SMILES:
-        mol = Chem.MolFromSmiles(message.value)
-        if mol is None:
-            warnings.warn(
-                f"RDKit {RDKIT_VERSION} could not validate" f" SMILES identifier {message.value}",
-                ValidationError,
-            )
-    elif message.type == message.INCHI:
-        mol = Chem.MolFromInchi(message.value)
-        if mol is None:
-            warnings.warn(
-                f"RDKit {RDKIT_VERSION} could not validate" f" InChI identifier {message.value}",
-                ValidationError,
-            )
-    elif message.type == message.MOLBLOCK:
-        mol = Chem.MolFromMolBlock(message.value)
-        if mol is None:
-            warnings.warn(
-                f"RDKit {RDKIT_VERSION} could not validate MolBlock identifier",
-                ValidationError,
-            )
+    if message.type in (message.SMILES, message.INCHI, message.MOLBLOCK):
+        (parse_func, identifier_type) = {
+            message.SMILES: (Chem.MolFromSmiles, "SMILES"),
+            message.INCHI: (Chem.MolFromInchi, "InChI"),
+            message.MOLBLOCK: (Chem.MolFromMolBlock, "MolBlock"),
+        }[message.type]
+        if parse_func(message.value) is None:
+            if parse_func(message.value, False) is None:
+                warnings.warn(
+                    f"RDKit {RDKIT_VERSION} could not validate {identifier_type} identifier {message.value}",
+                    ValidationError,
+                )
+            else:
+                warnings.warn(
+                    f"RDKit {RDKIT_VERSION} could not sanitize {identifier_type} identifier {message.value}",
+                    ValidationWarning,
+                )
 
 
 def validate_vessel(message: reaction_pb2.Vessel):
     check_type_and_details(message)
 
 
 def validate_vessel_material(message: reaction_pb2.VesselMaterial):
```

### Comparing `ord-schema-0.3.62/ord_schema/validations_test.py` & `ord-schema-0.3.63/ord_schema/validations_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -218,14 +218,62 @@
     message = reaction_pb2.Reaction()
     message.identifiers.add(value="test", type="REACTION_SMILES")
     with pytest.raises(validations.ValidationError, match="requires at least two > characters"):
         _run_validation(message)
 
 
 @pytest.mark.parametrize(
+    "identifier_type, value",
+    (
+        ("SMILES", "CO"),
+        ("INCHI", "InChI=1S/CH4O/c1-2/h2H,1H3"),
+        (
+            "MOLBLOCK",
+            "\n     RDKit          2D\n\n  2  1  0  0  0  0  0  0  0  0999 V2000\n    0.0000    0.0000    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0\n    1.2990    0.7500    0.0000 O   0  0  0  0  0  0  0  0  0  0  0  0\n  1  2  1  0\nM  END\n",
+        ),
+    ),
+)
+def test_compound_identifier(identifier_type, value):
+    message = reaction_pb2.CompoundIdentifier(type=identifier_type, value=value)
+    output = _run_validation(message)
+    assert len(output.errors) == 0
+    assert len(output.warnings) == 0
+
+
+@pytest.mark.parametrize(
+    "identifier_type, value",
+    (
+        ("SMILES", "[O-]1(C)[Ir+]234([O-](C)[Ir+]1567[CH]=8CC[CH]7=[CH]6CC[CH]85)[CH]=9CC[CH]4=[CH]3CC[CH]92"),
+        ("SMILES", "CO(C)(C)(C)C"),
+        ("SMILES", "On1c(-c2ccccc2)c(-c2c(-c3ccccc3)nc3ccccc23)c2ccccc21"),
+    ),
+)
+def test_bad_compound_identifier(identifier_type, value):
+    message = reaction_pb2.CompoundIdentifier(type=identifier_type, value=value)
+    output = _run_validation(message)
+    assert len(output.errors) == 0
+    assert len(output.warnings) == 1
+    assert "could not sanitize" in output.warnings[0]
+
+
+@pytest.mark.parametrize(
+    "identifier_type, value",
+    (
+        ("SMILES", "###"),
+        ("INCHI", "###"),
+        ("MOLBLOCK", "###"),
+    ),
+)
+def test_invalid_compound_identifier(identifier_type, value):
+    message = reaction_pb2.CompoundIdentifier(type=identifier_type, value=value)
+    with pytest.raises(validations.ValidationError, match="could not validate"):
+        _run_validation(message)
+
+
+@pytest.mark.parametrize(
     "workup_text",
     (
         "type: ALIQUOT amount {mass {value: 1.0 units: GRAM}}",
         "type: ADDITION input {components {"
         'identifiers {value: "CCO" type: SMILES} '
         "amount {mass {value: 10.0 units: GRAM}}}}",
     ),
```

### Comparing `ord-schema-0.3.62/ord_schema.egg-info/PKG-INFO` & `ord-schema-0.3.63/ord_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.62
+Version: 0.3.63
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.62/ord_schema.egg-info/SOURCES.txt` & `ord-schema-0.3.63/ord_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/ord_schema.egg-info/requires.txt` & `ord-schema-0.3.63/ord_schema.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/proto/dataset.proto` & `ord-schema-0.3.63/proto/dataset.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/proto/reaction.proto` & `ord-schema-0.3.63/proto/reaction.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/proto/test.proto` & `ord-schema-0.3.63/proto/test.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.62/setup.py` & `ord-schema-0.3.63/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.62",
+    version="0.3.63",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

