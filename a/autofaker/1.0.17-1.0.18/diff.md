# Comparing `tmp/autofaker-1.0.17.tar.gz` & `tmp/autofaker-1.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofaker-1.0.17.tar", last modified: Wed Aug  2 21:44:30 2023, max compression
+gzip compressed data, was "autofaker-1.0.18.tar", last modified: Wed Aug  2 21:48:46 2023, max compression
```

## Comparing `autofaker-1.0.17.tar` & `autofaker-1.0.18.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:44:30.596421 autofaker-1.0.17/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 21:44:14.000000 autofaker-1.0.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-02 21:44:14.000000 autofaker-1.0.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-08-02 21:44:30.596421 autofaker-1.0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-08-02 21:44:14.000000 autofaker-1.0.17/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-02 21:44:14.000000 autofaker-1.0.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:44:30.596421 autofaker-1.0.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-02 21:44:19.000000 autofaker-1.0.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:44:30.588421 autofaker-1.0.17/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:44:30.592421 autofaker-1.0.17/src/autofaker/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-02 21:44:14.000000 autofaker-1.0.17/src/autofaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-02 21:44:14.000000 autofaker-1.0.17/src/autofaker/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-02 21:44:14.000000 autofaker-1.0.17/src/autofaker/autodata.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-02 21:44:14.000000 autofaker-1.0.17/src/autofaker/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-02 21:44:14.000000 autofaker-1.0.17/src/autofaker/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-02 21:44:14.000000 autofaker-1.0.17/src/autofaker/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-02 21:44:14.000000 autofaker-1.0.17/src/autofaker/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-08-02 21:44:14.000000 autofaker-1.0.17/src/autofaker/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 21:44:14.000000 autofaker-1.0.17/src/autofaker/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-02 21:44:14.000000 autofaker-1.0.17/src/autofaker/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-02 21:44:14.000000 autofaker-1.0.17/src/autofaker/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-08-02 21:44:14.000000 autofaker-1.0.17/src/autofaker/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:44:30.592421 autofaker-1.0.17/src/autofaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-08-02 21:44:30.000000 autofaker-1.0.17/src/autofaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-08-02 21:44:30.000000 autofaker-1.0.17/src/autofaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:44:30.000000 autofaker-1.0.17/src/autofaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 21:44:30.000000 autofaker-1.0.17/src/autofaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 21:44:30.000000 autofaker-1.0.17/src/autofaker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:44:30.592421 autofaker-1.0.17/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:44:30.596421 autofaker-1.0.17/tests/pytests/
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/pytests/test_decorator_anonymous_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/pytests/test_decorator_anonymous_data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/pytests/test_decorator_anonymous_data_classes_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/pytests/test_decorator_anonymous_dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/pytests/test_decorator_anonymous_enum_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/pytests/test_decorator_anonymous_nested_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/pytests/test_decorator_anonymous_simple_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_complex_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_data_class_with_fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_data_classes_with_fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_dataframe_with_fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_enum_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_nested_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_nested_classes_with_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_simple_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_anonymous_sut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_many_anonymous_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_many_anonymous_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_many_anonymous_nested_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_many_anonymous_nested_classes_with_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_create_many_anonymous_simple_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/test_decorator_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:44:30.596421 autofaker-1.0.17/tests/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/unittests/test_decorator_anonymous_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/unittests/test_decorator_anonymous_data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/unittests/test_decorator_anonymous_data_classes_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/unittests/test_decorator_anonymous_dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/unittests/test_decorator_anonymous_enum_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/unittests/test_decorator_anonymous_nested_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-08-02 21:44:14.000000 autofaker-1.0.17/tests/unittests/test_decorator_anonymous_simple_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:48:46.115811 autofaker-1.0.18/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 21:48:30.000000 autofaker-1.0.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-02 21:48:30.000000 autofaker-1.0.18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-08-02 21:48:46.115811 autofaker-1.0.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-08-02 21:48:30.000000 autofaker-1.0.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-02 21:48:30.000000 autofaker-1.0.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:48:46.115811 autofaker-1.0.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-02 21:48:32.000000 autofaker-1.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:48:46.107811 autofaker-1.0.18/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:48:46.111811 autofaker-1.0.18/src/autofaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-02 21:48:30.000000 autofaker-1.0.18/src/autofaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-02 21:48:30.000000 autofaker-1.0.18/src/autofaker/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-02 21:48:30.000000 autofaker-1.0.18/src/autofaker/autodata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-02 21:48:30.000000 autofaker-1.0.18/src/autofaker/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-02 21:48:30.000000 autofaker-1.0.18/src/autofaker/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-02 21:48:30.000000 autofaker-1.0.18/src/autofaker/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-02 21:48:30.000000 autofaker-1.0.18/src/autofaker/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-08-02 21:48:30.000000 autofaker-1.0.18/src/autofaker/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 21:48:30.000000 autofaker-1.0.18/src/autofaker/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-02 21:48:30.000000 autofaker-1.0.18/src/autofaker/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-02 21:48:30.000000 autofaker-1.0.18/src/autofaker/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-08-02 21:48:30.000000 autofaker-1.0.18/src/autofaker/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:48:46.111811 autofaker-1.0.18/src/autofaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-08-02 21:48:45.000000 autofaker-1.0.18/src/autofaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-08-02 21:48:46.000000 autofaker-1.0.18/src/autofaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:48:45.000000 autofaker-1.0.18/src/autofaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 21:48:45.000000 autofaker-1.0.18/src/autofaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 21:48:45.000000 autofaker-1.0.18/src/autofaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:48:46.111811 autofaker-1.0.18/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:48:46.111811 autofaker-1.0.18/tests/pytests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/pytests/test_decorator_anonymous_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/pytests/test_decorator_anonymous_data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/pytests/test_decorator_anonymous_data_classes_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/pytests/test_decorator_anonymous_dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/pytests/test_decorator_anonymous_enum_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/pytests/test_decorator_anonymous_nested_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/pytests/test_decorator_anonymous_simple_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_complex_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_data_class_with_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_data_classes_with_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_dataframe_with_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_enum_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_nested_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_nested_classes_with_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_simple_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_anonymous_sut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_many_anonymous_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_many_anonymous_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_many_anonymous_nested_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_many_anonymous_nested_classes_with_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_create_many_anonymous_simple_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/test_decorator_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:48:46.115811 autofaker-1.0.18/tests/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/unittests/test_decorator_anonymous_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/unittests/test_decorator_anonymous_data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/unittests/test_decorator_anonymous_data_classes_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/unittests/test_decorator_anonymous_dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/unittests/test_decorator_anonymous_enum_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/unittests/test_decorator_anonymous_nested_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-08-02 21:48:30.000000 autofaker-1.0.18/tests/unittests/test_decorator_anonymous_simple_classes.py
```

### Comparing `autofaker-1.0.17/LICENSE` & `autofaker-1.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/PKG-INFO` & `autofaker-1.0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofaker
-Version: 1.0.17
+Version: 1.0.18
 Summary: Python library designed to minimize the setup/arrange phase of your unit tests
 Home-page: https://github.com/christianhelle/autofaker
 Author: Christian Helle
 Author-email: christian.helle@outlook.com
 License: MIT License
 Description: AutoFaker is a Python library designed to minimize the setup/arrange phase of your unit tests by removing the need to manually 
         write code to create anonymous variables as part of a test cases setup/arrange phase.
```

### Comparing `autofaker-1.0.17/README.md` & `autofaker-1.0.18/README.md`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/setup.py` & `autofaker-1.0.18/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("docs/pypi.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autofaker",
-    version='1.0.17',
+    version='1.0.18',
     url="https://github.com/christianhelle/autofaker",
     license="MIT License",
     license_files=["LICENSE"],
     author="Christian Helle",
     author_email="christian.helle@outlook.com",
     description="Python library designed to minimize the setup/arrange phase of your unit tests",
     long_description=long_description,
```

### Comparing `autofaker-1.0.17/src/autofaker/attributes.py` & `autofaker-1.0.18/src/autofaker/attributes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/src/autofaker/autodata.py` & `autofaker-1.0.18/src/autofaker/autodata.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/src/autofaker/builtins.py` & `autofaker-1.0.18/src/autofaker/builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/src/autofaker/dataframe.py` & `autofaker-1.0.18/src/autofaker/dataframe.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/src/autofaker/dates.py` & `autofaker-1.0.18/src/autofaker/dates.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/src/autofaker/decorators.py` & `autofaker-1.0.18/src/autofaker/decorators.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/src/autofaker/factory.py` & `autofaker-1.0.18/src/autofaker/factory.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/src/autofaker/fakes.py` & `autofaker-1.0.18/src/autofaker/fakes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/src/autofaker/generator.py` & `autofaker-1.0.18/src/autofaker/generator.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/src/autofaker.egg-info/PKG-INFO` & `autofaker-1.0.18/src/autofaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofaker
-Version: 1.0.17
+Version: 1.0.18
 Summary: Python library designed to minimize the setup/arrange phase of your unit tests
 Home-page: https://github.com/christianhelle/autofaker
 Author: Christian Helle
 Author-email: christian.helle@outlook.com
 License: MIT License
 Description: AutoFaker is a Python library designed to minimize the setup/arrange phase of your unit tests by removing the need to manually 
         write code to create anonymous variables as part of a test cases setup/arrange phase.
```

### Comparing `autofaker-1.0.17/src/autofaker.egg-info/SOURCES.txt` & `autofaker-1.0.18/src/autofaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/pytests/test_decorator_anonymous_builtins.py` & `autofaker-1.0.18/tests/pytests/test_decorator_anonymous_builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/pytests/test_decorator_anonymous_data_classes.py` & `autofaker-1.0.18/tests/pytests/test_decorator_anonymous_data_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/pytests/test_decorator_anonymous_data_classes_nested.py` & `autofaker-1.0.18/tests/pytests/test_decorator_anonymous_data_classes_nested.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/pytests/test_decorator_anonymous_dataframe_pandas.py` & `autofaker-1.0.18/tests/pytests/test_decorator_anonymous_dataframe_pandas.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/pytests/test_decorator_anonymous_enum_classes.py` & `autofaker-1.0.18/tests/pytests/test_decorator_anonymous_enum_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/pytests/test_decorator_anonymous_nested_classes.py` & `autofaker-1.0.18/tests/pytests/test_decorator_anonymous_nested_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/pytests/test_decorator_anonymous_simple_classes.py` & `autofaker-1.0.18/tests/pytests/test_decorator_anonymous_simple_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_builtins.py` & `autofaker-1.0.18/tests/test_create_anonymous_builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_complex_classes.py` & `autofaker-1.0.18/tests/test_create_anonymous_complex_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_data_class_with_fakes.py` & `autofaker-1.0.18/tests/test_create_anonymous_data_class_with_fakes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_data_classes.py` & `autofaker-1.0.18/tests/test_create_anonymous_data_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_data_classes_with_fakes.py` & `autofaker-1.0.18/tests/test_create_anonymous_data_classes_with_fakes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_dataframe_pandas.py` & `autofaker-1.0.18/tests/test_create_anonymous_dataframe_pandas.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_dataframe_with_fakes.py` & `autofaker-1.0.18/tests/test_create_anonymous_dataframe_with_fakes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_dates.py` & `autofaker-1.0.18/tests/test_create_anonymous_dates.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_enum_classes.py` & `autofaker-1.0.18/tests/test_create_anonymous_enum_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_lists.py` & `autofaker-1.0.18/tests/test_create_anonymous_lists.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_nested_classes.py` & `autofaker-1.0.18/tests/test_create_anonymous_nested_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_nested_classes_with_lists.py` & `autofaker-1.0.18/tests/test_create_anonymous_nested_classes_with_lists.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_simple_classes.py` & `autofaker-1.0.18/tests/test_create_anonymous_simple_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_anonymous_sut.py` & `autofaker-1.0.18/tests/test_create_anonymous_sut.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_many_anonymous_builtins.py` & `autofaker-1.0.18/tests/test_create_many_anonymous_builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_many_anonymous_dates.py` & `autofaker-1.0.18/tests/test_create_many_anonymous_dates.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_many_anonymous_nested_classes.py` & `autofaker-1.0.18/tests/test_create_many_anonymous_nested_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_many_anonymous_nested_classes_with_lists.py` & `autofaker-1.0.18/tests/test_create_many_anonymous_nested_classes_with_lists.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_create_many_anonymous_simple_classes.py` & `autofaker-1.0.18/tests/test_create_many_anonymous_simple_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/test_decorator_exceptions.py` & `autofaker-1.0.18/tests/test_decorator_exceptions.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/unittests/test_decorator_anonymous_builtins.py` & `autofaker-1.0.18/tests/unittests/test_decorator_anonymous_builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/unittests/test_decorator_anonymous_data_classes.py` & `autofaker-1.0.18/tests/unittests/test_decorator_anonymous_data_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/unittests/test_decorator_anonymous_data_classes_nested.py` & `autofaker-1.0.18/tests/unittests/test_decorator_anonymous_data_classes_nested.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/unittests/test_decorator_anonymous_dataframe_pandas.py` & `autofaker-1.0.18/tests/unittests/test_decorator_anonymous_dataframe_pandas.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/unittests/test_decorator_anonymous_nested_classes.py` & `autofaker-1.0.18/tests/unittests/test_decorator_anonymous_nested_classes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.17/tests/unittests/test_decorator_anonymous_simple_classes.py` & `autofaker-1.0.18/tests/unittests/test_decorator_anonymous_simple_classes.py`

 * *Files identical despite different names*

