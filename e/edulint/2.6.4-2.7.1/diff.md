# Comparing `tmp/edulint-2.6.4.tar.gz` & `tmp/edulint-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-8c62uyms/edulint-2.6.4.tar", last modified: Thu May 11 10:30:20 2023, max compression
+gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-dbv3bqci/edulint-2.7.1.tar", last modified: Wed Aug  2 14:38:10 2023, max compression
```

## Comparing `edulint-2.6.4.tar` & `edulint-2.7.1.tar`

### file list

```diff
@@ -1,63 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:20.000000 edulint-2.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 10:30:08.000000 edulint-2.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-11 10:30:20.000000 edulint-2.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-11 10:30:08.000000 edulint-2.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/config/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/config/config_translations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1873 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/explanations.py
--rw-r--r--   0 runner    (1001) docker     (123)   190327 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/explanations.toml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint/linting/
--rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint/linting/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/checkers/basic_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/checkers/improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/checkers/modified_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/checkers/python_ta_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/checkers/short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/checkers/simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/checkers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/linting.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/process_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/linting/tweakers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint/prepare_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/prepare_explanations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint/prepare_explanations/pylint_data/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/prepare_explanations/pylint_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15286 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/prepare_explanations/pylint_data/pylint_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint/prepare_explanations/thonny_data/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/prepare_explanations/thonny_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/prepare_explanations/thonny_data/thonny_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-11 10:30:08.000000 edulint-2.6.4/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 10:30:20.000000 edulint-2.6.4/edulint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-11 10:30:08.000000 edulint-2.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-11 10:30:20.000000 edulint-2.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 10:30:08.000000 edulint-2.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:30:20.000000 edulint-2.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-11 10:30:08.000000 edulint-2.6.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-11 10:30:08.000000 edulint-2.6.4/tests/test_improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    20554 2023-05-11 10:30:08.000000 edulint-2.6.4/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-11 10:30:08.000000 edulint-2.6.4/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-05-11 10:30:08.000000 edulint-2.6.4/tests/test_short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-05-11 10:30:08.000000 edulint-2.6.4/tests/test_simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-11 10:30:08.000000 edulint-2.6.4/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 14:37:53.000000 edulint-2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-02 14:38:10.000000 edulint-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-02 14:37:53.000000 edulint-2.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/config_translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/file_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/config/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/files/default.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/config/files/empty.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190327 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/explanations.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/linting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/linting/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/basic_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25119 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/duplication_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/modified_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/python_ta_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/checkers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/linting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/process_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/linting/tweakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/prepare_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/prepare_explanations/pylint_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/pylint_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/pylint_data/pylint_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint/prepare_explanations/thonny_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/thonny_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/thonny_data/thonny_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-08-02 14:37:53.000000 edulint-2.7.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 14:38:10.000000 edulint-2.7.1/edulint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-02 14:37:53.000000 edulint-2.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 14:38:10.000000 edulint-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 14:37:53.000000 edulint-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:10.000000 edulint-2.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21323 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-08-02 14:37:53.000000 edulint-2.7.1/tests/test_visitors.py
```

### Comparing `edulint-2.6.4/LICENSE` & `edulint-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edulint-2.6.4/PKG-INFO` & `edulint-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.6.4
+Version: 2.7.1
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.6.4/README.md` & `edulint-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `edulint-2.6.4/edulint/config/config.py` & `edulint-2.7.1/edulint/options.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,154 +1,204 @@
-from edulint.config.arg import ProcessedArg, UnprocessedArg, ImmutableArg
-from edulint.options import UnionT, ImmutableT, Option, TakesVal, OptionParse, get_option_parses, get_name_to_option
-from edulint.config.config_translations import get_config_translations, get_ib111_translations, Translation
-from typing import Dict, List, Optional, Tuple, Iterator
 from dataclasses import dataclass
-from argparse import Namespace
-import re
-import sys
-import shlex
+from typing import Dict, List, Any, TypeVar, Optional, Union, Callable, Tuple
+from enum import Enum, auto
 
 
-@dataclass(frozen=True)
-class Config:
+class NumberFromZero(Enum):
+    def __new__(cls, *args: Any) -> "NumberFromZero":
+        value = len(cls.__members__)
+        obj = object.__new__(cls)
+        obj._value_ = value
+        return obj
+
+
+T = TypeVar("T")
+UnionT = Union[bool, List[str], Optional[str], Optional[int]]
+ImmutableT = Union[bool, Tuple[str, ...], Optional[str], Optional[int]]
+
+
+class Option(NumberFromZero):
+    CONFIG = ()
+    PYLINT = ()
+    FLAKE8 = ()
+    ENHANCEMENT = ()
+    PYTHON_SPECIFIC = ()
+    COMPLEXITY = ()
+    ALLOWED_ONECHAR_NAMES = ()
+    IB111_WEEK = ()
+    NO_FLAKE8 = ()
 
-    config: Tuple[ImmutableArg]
+    def to_name(self) -> str:
+        return self.name.lower().replace("_", "-")
 
     @staticmethod
-    def to_immutable(v: UnionT) -> ImmutableT:
-        return v if not isinstance(v, list) else tuple(v)
+    def from_name(option_str: str) -> "Option":
+        for option in Option:
+            if option.to_name() == option_str.lower():
+                return option
+        assert False, "no such option: " + option_str
 
-    def __init__(self, config: Optional[List[ProcessedArg]] = None,
-                 option_parses: Dict[Option, OptionParse] = get_option_parses()) -> None:
-        config = config if config is not None else []
-        wip_config: List[Optional[ImmutableArg]] = [None for _ in Option]
+    def __int__(self) -> int:
+        return self.value  # type: ignore
 
-        for arg in config:
-            assert wip_config[int(arg.option)] is None
-            wip_config[int(arg.option)] = ImmutableArg(arg.option, self.to_immutable(arg.val))
 
-        object.__setattr__(self, "config", tuple([arg if arg is not None else ImmutableArg(
-            o, self.to_immutable(option_parses[o].default)) for o, arg in zip(Option, wip_config)]))
+class TakesVal(Enum):
+    YES = auto()
+    NO = auto()
+    OPTIONAL = auto()
 
-    def __str__(self) -> str:
-        return f"Config({', '.join(arg.option.name + '=' + str(arg.val) for arg in self.config)})"
 
-    def __getitem__(self, option: Option) -> ImmutableT:
-        return self.config[int(option)].val
+class MultivaluedEnum(Enum):
+    def __new__(cls, *args: Any, **kwds: Any) -> Any:
+        value = len(cls.__members__) + 1
+        obj = object.__new__(cls)
+        obj._value_ = value
+        return obj
 
-    def __contains__(self, option: Option) -> bool:
-        return self[option] is not None
 
-    def __iter__(self) -> Iterator[ImmutableArg]:
-        return filter(lambda x: x is not None, self.config.__iter__())
-
-
-def extract_args(filename: str) -> List[str]:
-    edulint_re = re.compile(r"\s*#[\s#]*edulint:\s*", re.IGNORECASE)
-    ib111_re = re.compile(r"\s*from\s+ib111\s+import\s+week_(\d+)", re.IGNORECASE)
-
-    result: List[str] = []
-    with open(filename, encoding="utf-8") as f:
-        for i, line in enumerate(f):
-            line = line.strip()
-
-            edmatch = edulint_re.match(line)
-            if edmatch:
-                raw_args = line[edmatch.end():]
-                result.extend(shlex.split(raw_args))
-
-            ibmatch = ib111_re.match(line)
-            if ibmatch:
-                result.append(f"{Option.IB111_WEEK.to_name()}={ibmatch.group(1)}")
-
-    return result
-
-
-def parse_args(args: List[str], option_parses: Dict[Option, OptionParse]) -> List[UnprocessedArg]:
-    name_to_option = get_name_to_option(option_parses)
-
-    def get_name_val(arg: str) -> Tuple[str, Optional[str]]:
-        if "=" in arg:
-            name, val = arg.split("=", 1)
-            return name, val
-        return arg, None
-
-    result: List[UnprocessedArg] = []
-    for arg in args:
-        name, val = get_name_val(arg)
-        option = name_to_option.get(name)
-
-        if option is None:
-            print(f"edulint: unrecognized option {name}", file=sys.stderr)
-        else:
-            option_parse = option_parses[option]
-            if option_parse.takes_val == TakesVal.YES and val is None:
-                print(f"edulint: option {name} takes an argument but none was supplied", file=sys.stderr)
-            elif option_parse.takes_val == TakesVal.NO and val is not None:
-                print(f"edulint: option {name} takes no argument but {val} was supplied", file=sys.stderr)
-            else:
-                result.append(UnprocessedArg(option, val))
-
-    return result
-
-
-def fill_in_val(arg: UnprocessedArg, translation: List[str]) -> List[str]:
-    result = []
-    for t in translation:
-        if "<val>" in t:
-            assert isinstance(arg.val, str)
-            result.append(t.replace("<val>", arg.val))
-        else:
-            result.append(t)
-    return result
+class Type(MultivaluedEnum):
+    @staticmethod
+    def _to_bool_val(val: Optional[str]) -> bool:
+        return val is None or val in ("true", "on")
 
+    @staticmethod
+    def _to_list_val(val: Optional[str]) -> List[str]:
+        return [val] if val is not None else []
 
-def combine_and_translate(
-        args: List[UnprocessedArg],
-        option_parses: Dict[Option, OptionParse],
-        config_translations: Dict[Option, Translation],
-        ib111_translations: List[Translation]) -> Config:
+    @staticmethod
+    def _to_str_val(val: Optional[str]) -> Optional[str]:
+        return val
 
-    def combine(option_vals: List[UnionT], option: Option, val: Optional[str]) -> None:
-        parse = option_parses[option]
-        old_val = option_vals[int(option)]
-        option_vals[int(option)] = parse.combine(old_val, parse.convert(val))
+    @staticmethod
+    def _to_int_val(val: Optional[str]) -> Optional[int]:
+        return int(val) if val is not None and val.isdecimal() else None
 
-    def apply_translation(option_vals: List[UnionT], translated: Translation) -> None:
-        translated_option = translated.for_linter.to_option()
-        for val in translated.vals:
-            combine(option_vals, translated_option, val)
+    def __init__(self, _: Enum, convert: Callable[[Optional[str]], UnionT]):
+        self.convert: Callable[[Optional[str]], UnionT] = convert.__func__  # type: ignore
 
-    option_vals = [option_parses[o].default for o in Option]
+    def __call__(self, arg: Optional[str]) -> UnionT:
+        return self.convert(arg)
 
-    for arg in args:
-        combine(option_vals, arg.option, arg.val)
+    BOOL = (auto(), _to_bool_val)
+    LIST = (auto(), _to_list_val)
+    STR = (auto(), _to_str_val)
+    INT = (auto(), _to_int_val)
 
-        translated = config_translations.get(arg.option)
-        if translated is not None and option_vals[int(arg.option)] not in (False, None):
-            apply_translation(option_vals, translated)
 
-    ib111_week = option_vals[int(Option.IB111_WEEK)]
-    if ib111_week is not None:
-        assert isinstance(ib111_week, int)
-        if 0 <= ib111_week < len(ib111_translations):
-            apply_translation(option_vals, ib111_translations[ib111_week])
-        else:
-            print(f"edulint: option {Option.IB111_WEEK.to_name()} has value {ib111_week} which is invalid;"
-                  f"allowed values are 0 to {len(ib111_translations)}", file=sys.stderr)
+class Combine(MultivaluedEnum):
+    @staticmethod
+    def _keep_right_combine(_lt: T, rt: T) -> T:
+        return rt
 
-    return Config([ProcessedArg(o, v) for o, v in zip(Option, option_vals) if v is not None])
+    @staticmethod
+    def _append_combine(lt: List[T], rt: T) -> List[T]:
+        return lt + [rt]
 
+    @staticmethod
+    def _extend_combine(lt: List[T], rt: List[T]) -> List[T]:
+        return lt + rt
 
-def get_config(
-        filename: str, cmd_args: List[str],
-        option_parses: Dict[Option, OptionParse] = get_option_parses(),
-        config_translations: Dict[Option, Translation] = get_config_translations(),
-        ib111_translation: List[Translation] = get_ib111_translations()) -> Config:
-    extracted = extract_args(filename) + cmd_args
-    parsed = parse_args(extracted, option_parses)
-    return combine_and_translate(parsed, option_parses, config_translations, ib111_translation)
+    def __init__(self, _: Enum, combine: Callable[[UnionT, UnionT], UnionT]):
+        self.combine: Callable[[UnionT, UnionT], UnionT] = combine.__func__  # type: ignore
 
+    def __call__(self, lt: UnionT, rt: UnionT) -> UnionT:
+        return self.combine(lt, rt)
 
-def get_cmd_args(args: Namespace) -> List[str]:
-    return [s for arg in args.options for s in shlex.split(arg)]
+    REPLACE = (auto(), _keep_right_combine)
+    APPEND = (auto(), _append_combine)
+    EXTEND = (auto(), _extend_combine)
+
+
+@dataclass
+class OptionParse:
+    option: Option
+    help_: str
+    takes_val: TakesVal
+    default: UnionT
+    convert: Type
+    combine: Combine
+
+
+DEFAULT_CONFIG = "default"
+BASE_CONFIG = "empty"
+
+OPTIONS: List[OptionParse] = [
+    OptionParse(
+        Option.CONFIG,
+        "config file to use for the linting (packaged name, local path or remote)",
+        TakesVal.YES,
+        DEFAULT_CONFIG,
+        Type.STR,
+        Combine.REPLACE,
+    ),
+    OptionParse(
+        Option.PYLINT,
+        "arguments to be passed to pylint (formatted to be passed through command line)",
+        TakesVal.YES,
+        [],
+        Type.LIST,
+        Combine.EXTEND,
+    ),
+    OptionParse(
+        Option.FLAKE8,
+        "arguments to be passed to flake8 (formatted to be passed through command line)",
+        TakesVal.YES,
+        [],
+        Type.LIST,
+        Combine.EXTEND,
+    ),
+    OptionParse(
+        Option.ENHANCEMENT,
+        "enable checking for ways to improve the code further",
+        TakesVal.NO,
+        False,
+        Type.BOOL,
+        Combine.REPLACE,
+    ),
+    OptionParse(
+        Option.PYTHON_SPECIFIC,
+        "enable checking for ways to improve the code with Python-specific constructions",
+        TakesVal.NO,
+        False,
+        Type.BOOL,
+        Combine.REPLACE,
+    ),
+    OptionParse(
+        Option.COMPLEXITY,
+        "enable checking for overly complicated pieces of code",
+        TakesVal.NO,
+        False,
+        Type.BOOL,
+        Combine.REPLACE,
+    ),
+    OptionParse(
+        Option.ALLOWED_ONECHAR_NAMES,
+        "only listed characters are allowed to be variable names of length one",
+        TakesVal.YES,
+        None,
+        Type.STR,
+        Combine.REPLACE,
+    ),
+    OptionParse(
+        Option.IB111_WEEK,
+        "set which week's limitation should be applied",
+        TakesVal.YES,
+        None,
+        Type.INT,
+        Combine.REPLACE,
+    ),
+    OptionParse(
+        Option.NO_FLAKE8, "turn off flake8", TakesVal.NO, False, Type.BOOL, Combine.REPLACE
+    ),
+]
+
+OLD_NAMES = {"python-spec": Option.PYTHON_SPECIFIC}
+
+
+def get_option_parses() -> Dict[Option, OptionParse]:
+    return {parse.option: parse for parse in OPTIONS}
+
+
+def get_name_to_option(option_parses: Dict[Option, OptionParse]) -> Dict[str, Option]:
+    from_options = {parse.option.to_name(): opt for opt, parse in option_parses.items()}
+    from_options.update(OLD_NAMES)
+    return from_options
```

### Comparing `edulint-2.6.4/edulint/config/config_translations.py` & `edulint-2.7.1/edulint/config/config_translations.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,40 +9,43 @@
     for_linter: Linter
     vals: List[str]
 
 
 CONFIG_TRANSLATIONS: Dict[Option, Translation] = {
     Option.ENHANCEMENT: Translation(
         Linter.PYLINT,
-        ["--enable=no-self-use,superfluous-parens,consider-using-min-builtin,"
-         "consider-using-max-builtin,consider-using-with,unspecified-encoding,"
-         "loop-shadows-control-variable,no-repeated-op,"
-         "forbidden-top-level-code,simplifiable-if-nested,simplifiable-if-seq,"
-         "simplifiable-if-return-conj,simplifiable-if-assignment-conj,simplifiable-if-expr-conj,"]
+        [
+            "--enable=no-self-use,superfluous-parens,consider-using-min-builtin,"
+            "consider-using-max-builtin,consider-using-with,unspecified-encoding,"
+            "loop-shadows-control-variable,no-repeated-op,"
+            "forbidden-top-level-code,simplifiable-if-nested,simplifiable-if-seq,"
+            "simplifiable-if-return-conj,simplifiable-if-assignment-conj,simplifiable-if-expr-conj,"
+        ],
     ),
     Option.PYTHON_SPECIFIC: Translation(
         Linter.PYLINT,
-        ["--enable=unidiomatic-typecheck,misplaced-format-function,"
-         "use-enumerate,consider-iterating-dictionary,"
-         "consider-using-dict-items,consider-using-f-string,"
-         "inconsistent-return-statements,consider-swap-variables,"
-         "consider-using-join,consider-using-set-comprehension,"
-         "unnecessary-comprehension,use-a-generator,use-list-literal,"
-         "use-dict-literal,consider-using-in,"]
+        [
+            "--enable=unidiomatic-typecheck,misplaced-format-function,"
+            "use-enumerate,consider-iterating-dictionary,"
+            "consider-using-dict-items,consider-using-f-string,"
+            "inconsistent-return-statements,consider-swap-variables,"
+            "consider-using-join,consider-using-set-comprehension,"
+            "unnecessary-comprehension,use-a-generator,use-list-literal,"
+            "use-dict-literal,consider-using-in,"
+        ],
     ),
     Option.COMPLEXITY: Translation(
         Linter.PYLINT,
-        ["--enable=too-many-arguments,too-many-branches,too-many-statements,"
-         "too-many-return-statements,too-many-nested-blocks,too-many-locals,"
-         "too-many-boolean-expressions,"]
+        [
+            "--enable=too-many-arguments,too-many-branches,too-many-statements,"
+            "too-many-return-statements,too-many-nested-blocks,too-many-locals,"
+            "too-many-boolean-expressions,"
+        ],
     ),
-    Option.ALLOWED_ONECHAR_NAMES: Translation(
-        Linter.PYLINT,
-        ["--bad-names-rgxs=^[a-z]$"]
-    )
+    Option.ALLOWED_ONECHAR_NAMES: Translation(Linter.PYLINT, ["--bad-names-rgxs=^[a-z]$"]),
 }
 
 
 def get_config_translations() -> Dict[Option, Translation]:
     return CONFIG_TRANSLATIONS
```

### Comparing `edulint-2.6.4/edulint/explanations.toml` & `edulint-2.7.1/edulint/explanations.toml`

 * *Files identical despite different names*

### Comparing `edulint-2.6.4/edulint/linters.py` & `edulint-2.7.1/edulint/linters.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.4/edulint/linting/checkers/basic_checker.py` & `edulint-2.7.1/edulint/linting/checkers/basic_checker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from astroid import nodes, Context  # type: ignore
 from typing import TYPE_CHECKING, Optional, List, Union, Tuple
 from enum import Enum, auto
 from functools import reduce
 
 from pylint.checkers import BaseChecker  # type: ignore
+from pylint.checkers.utils import only_required_for_messages
 
 if TYPE_CHECKING:
     from pylint.lint import PyLinter  # type: ignore
 
-from edulint.linting.checkers.utils import get_name, is_builtin, get_range_params
+from edulint.linting.checkers.utils import (
+    get_name,
+    is_builtin,
+    get_range_params,
+    get_statements_count,
+    is_parents_elif,
+)
 from edulint.linting.checkers.modified_listener import ModifiedListener
 
 
 class UsesIndex(Enum):
     OUTSIDE_SUBSCRIPT = auto()
     INSIDE_SUBSCRIPT = auto()
     NEVER = auto()
@@ -23,54 +30,58 @@
             return cls.INSIDE_SUBSCRIPT
         if lt == cls.OUTSIDE_SUBSCRIPT or rt == cls.OUTSIDE_SUBSCRIPT:
             return cls.OUTSIDE_SUBSCRIPT
         return cls.NEVER
 
 
 class ImproveForLoop(BaseChecker):  # type: ignore
-
     name = "improve-for-loop"
     msgs = {
         "R6101": (
-            "Iterate directly: \"for var in %s\" (with appropriate name for \"var\")",
+            'Iterate directly: "for var in %s" (with appropriate name for "var")',
             "use-foreach",
             "Emitted when a for-range loop is used while a for-each loop would suffice.",
         ),
         "R6102": (
-            "Iterate using enumerate: \"for %s, var in enumerate(%s)\" (with appropriate name for \"var\")",
+            'Iterate using enumerate: "for %s, var in enumerate(%s)" (with appropriate name for "var")',
             "use-enumerate",
             "Emitted when a for-range loop is used with the element at each index is accessed as well.",
         ),
     }
 
     def __init__(self, linter: Optional["PyLinter"] = None) -> None:
         super().__init__(linter)
 
     class StructureIndexedVisitor(ModifiedListener[Tuple[bool, bool]]):
         default = (False, False)
 
         @staticmethod
         def combine(results: List[Tuple[bool, bool]]) -> Tuple[bool, bool]:
-            return any(loaded for loaded, _stored in results), any(stored for _loaded, stored in results)
+            return any(loaded for loaded, _stored in results), any(
+                stored for _loaded, stored in results
+            )
 
         def __init__(self, structure: Union[nodes.Name, nodes.Attribute], index: nodes.Name):
             super().__init__([structure, index])
             self.structure = structure
             self.index = index
 
         def visit_subscript(self, subscript: nodes.Subscript) -> Tuple[bool, bool]:
             sub_loaded, sub_stored = self.visit_many(subscript.get_children())
 
-            if self.was_reassigned(self.structure, allow_definition=False) \
-                    or self.was_reassigned(self.index, allow_definition=False):
+            if self.was_reassigned(self.structure, allow_definition=False) or self.was_reassigned(
+                self.index, allow_definition=False
+            ):
                 return False, False
 
-            used = subscript.value.as_string() == self.structure.as_string() \
-                and isinstance(subscript.slice, nodes.Name) \
+            used = (
+                subscript.value.as_string() == self.structure.as_string()
+                and isinstance(subscript.slice, nodes.Name)
                 and subscript.slice.as_string() == self.index.as_string()
+            )
 
             if subscript.ctx == Context.Store:
                 return sub_loaded, sub_stored or used
 
             if subscript.ctx == Context.Load:
                 return sub_loaded or used, sub_stored
 
@@ -90,43 +101,60 @@
             self.index = index
 
         def visit_name(self, name: nodes.Name) -> UsesIndex:
             if name.name != self.index.name:
                 return UsesIndex.NEVER
 
             parent = name.parent
-            if isinstance(parent, nodes.Subscript) and parent.value.as_string() != self.structure.as_string():
+            if (
+                isinstance(parent, nodes.Subscript)
+                and parent.value.as_string() != self.structure.as_string()
+            ):
                 return UsesIndex.INSIDE_SUBSCRIPT
 
-            if not isinstance(name.parent, nodes.Subscript) \
-                    or not isinstance(self.structure, type(name.parent.value)) \
-                    or self.was_reassigned(name, allow_definition=False):
+            if (
+                not isinstance(name.parent, nodes.Subscript)
+                or not isinstance(self.structure, type(name.parent.value))
+                or self.was_reassigned(name, allow_definition=False)
+            ):
                 return UsesIndex.OUTSIDE_SUBSCRIPT
 
             subscript = name.parent
-            if not ((isinstance(subscript.value, nodes.Name)
-                    and subscript.value.name == self.structure.name)
-                    or (isinstance(subscript.value, nodes.Attribute)
-                    and subscript.value.attrname == self.structure.attrname)):
+            if not (
+                (
+                    isinstance(subscript.value, nodes.Name)
+                    and subscript.value.name == self.structure.name
+                )
+                or (
+                    isinstance(subscript.value, nodes.Attribute)
+                    and subscript.value.attrname == self.structure.attrname
+                )
+            ):
                 return UsesIndex.OUTSIDE_SUBSCRIPT
 
             if isinstance(subscript.parent, nodes.Assign) and subscript in subscript.parent.targets:
                 return UsesIndex.OUTSIDE_SUBSCRIPT
 
             return UsesIndex.NEVER
 
     def visit_for(self, node: nodes.For) -> None:
         range_params = get_range_params(node.iter)
         if range_params is None:
             return
 
         start, stop, step = range_params
-        if not isinstance(start, nodes.Const) or start.value != 0 \
-                or not isinstance(stop, nodes.Call) or not is_builtin(stop.func, "len") or len(stop.args) != 1 \
-                or not isinstance(step, nodes.Const) or step.value != 1:
+        if (
+            not isinstance(start, nodes.Const)
+            or start.value != 0
+            or not isinstance(stop, nodes.Call)
+            or not is_builtin(stop.func, "len")
+            or len(stop.args) != 1
+            or not isinstance(step, nodes.Const)
+            or step.value != 1
+        ):
             return
 
         structure = stop.args[0]
         index = node.target
         if not isinstance(structure, nodes.Name) and not isinstance(structure, nodes.Attribute):
             return
 
@@ -148,15 +176,15 @@
 
 class NoGlobalVars(BaseChecker):
     name = "no-global-variables"
     msgs = {
         "R6401": (
             "Do not use global variables; you use %s, modifying it for example at line %i.",
             "no-global-vars",
-            "Emitted when the code uses global variables."
+            "Emitted when the code uses global variables.",
         ),
     }
 
     def __init__(self, linter: "PyLinter"):
         super().__init__(linter)
         self.to_check = {}
 
@@ -175,18 +203,92 @@
 
     def close(self) -> None:
         for frame, vars_ in self.to_check.items():
             listener = ModifiedListener(list(vars_.values()))
             listener.visit(frame)
             for node in vars_.values():
                 if listener.was_modified(node, allow_definition=True):
-                    nonglobal_modifiers = [n for n in listener.get_all_modifiers(node) if n.scope() != node.scope()]
+                    nonglobal_modifiers = [
+                        n for n in listener.get_all_modifiers(node) if n.scope() != node.scope()
+                    ]
                     if nonglobal_modifiers:
-                        self.add_message("no-global-vars", node=node, args=(node.name, nonglobal_modifiers[0].lineno))
+                        self.add_message(
+                            "no-global-vars",
+                            node=node,
+                            args=(node.name, nonglobal_modifiers[0].lineno),
+                        )
+
+
+class LongCodeChecker(BaseChecker):
+    name = "long-code"
+    msgs = {
+        "R6701": (
+            "Too much code outside of functions or classes (%d which is over %d statements).",
+            "long-script",
+            "Emitted when there are too many lines of code on the top level that are not import or function or class "
+            "definition.",
+        ),
+        "R6702": (
+            "Function '%s' is too long (%d which is over %d statements).",
+            "long-function",
+            "Emitted when there are too many statements inside a function definition.",
+        ),
+        "R6703": (
+            "Use early return.",
+            "use-early-return",
+            "Emitted when a long block of code is followed by an else that just returns, breaks or continues.",
+        ),
+    }
+
+    @only_required_for_messages("long-script")
+    def visit_module(self, node: nodes.Module):
+        MAX_SCRIPT = 20
+
+        count = get_statements_count(node, include_defs=False, include_name_main=False)
+        if count > MAX_SCRIPT:
+            self.add_message("long-script", node=node, args=(count, MAX_SCRIPT))
+
+    @only_required_for_messages("long-function")
+    def visit_functiondef(self, node: nodes.FunctionDef):
+        MAX_FUNC = 20
+
+        count = get_statements_count(node.body, include_defs=False, include_name_main=False)
+        if count > MAX_FUNC:
+            self.add_message("long-function", node=node, args=(node.name, count, MAX_FUNC))
+
+    @only_required_for_messages("use-early-return")
+    def visit_if(self, node: nodes.If):
+        def ends_block(node: nodes.NodeNG) -> bool:
+            if isinstance(node, nodes.If):
+                return (
+                    ends_block(node.body[-1])
+                    and len(node.orelse) > 0
+                    and ends_block(node.orelse[-1])
+                )
+            return isinstance(node, (nodes.Return, nodes.Break, nodes.Continue))
+
+        if is_parents_elif(node):
+            return
+
+        if len(node.orelse) > 0:
+            if get_statements_count(node.orelse, include_defs=True, include_name_main=True) > 2:
+                return
+            last = node.orelse[-1]
+        elif ends_block(node.body[-1]):
+            last = node.next_sibling()
+        else:
+            return
+
+        if (
+            ends_block(last)
+            and get_statements_count(node.body, include_defs=True, include_name_main=True) > 3
+        ):
+            self.add_message("use-early-return", node=node)
 
 
 def register(linter: "PyLinter") -> None:
     """This required method auto registers the checker during initialization.
     :param linter: The linter to register the checker to.
     """
     linter.register_checker(ImproveForLoop(linter))
     linter.register_checker(NoGlobalVars(linter))
+    linter.register_checker(LongCodeChecker(linter))
```

### Comparing `edulint-2.6.4/edulint/linting/checkers/improper_loop.py` & `edulint-2.7.1/edulint/linting/checkers/improper_loop.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,148 @@
 from astroid import nodes  # type: ignore
-from typing import TYPE_CHECKING, List, Tuple, Iterator, Set
+from typing import TYPE_CHECKING, List, Tuple, Iterator, Set, Optional
 
 from pylint.checkers import BaseChecker  # type: ignore
 from pylint.checkers.utils import only_required_for_messages
 
 if TYPE_CHECKING:
     from pylint.lint import PyLinter  # type: ignore
 
 from edulint.linting.checkers.utils import get_name, get_range_params, get_const_value
 from edulint.linting.checkers.modified_listener import ModifiedListener
 
 
 class ImproperLoop(BaseChecker):
-
     name = "improper-loop"
     msgs = {
         "R6301": (
             "The while condition can be replaced with '<negated %s>'",
             "no-while-true",
             "Emitted when the condition of a while loop is 'True' unnecessarily.",
         ),
         "R6302": (
             "Use tighter range boundaries, the %s iteration never happens.",
             "use-tighter-boundaries",
-            "Emitted when the boundaries of a range can be made tighter."
+            "Emitted when the boundaries of a range can be made tighter.",
         ),
         "R6303": (
             "Iterated structure %s is being modified inside the for loop body. Use while loop or iterate over a copy.",
             "modifying-iterated-structure",
-            "Emitted when the structure that is being iterated over is being modified in the for loops body."
+            "Emitted when the structure that is being iterated over is being modified in the for loops body.",
         ),
         "R6304": (
             "Changing the control variable %s of a for loop has no effect.",
             "changing-control-variable",
-            "Emitted when the control variable of a for loop is being changed."
+            "Emitted when the control variable of a for loop is being changed.",
         ),
         "R6305": (
             "Use for loop.",
             "use-for-loop",
-            "Emitted when a while loop can be transformed into a for loop."
+            "Emitted when a while loop can be transformed into a for loop.",
         ),
         "R6306": (
             "Inner for loop shadows outer for loop's control variable %s.",
             "loop-shadows-control-variable",
-            "Emitted when a for loop shadows control variable of an outer for loop."
-        )
+            "Emitted when a for loop shadows control variable of an outer for loop.",
+        ),
     }
 
     def _check_no_while_true(self, node: nodes.While) -> None:
         if not isinstance(node.test, nodes.Const) or not node.test.bool_value():
             return
 
         first = node.body[0]
         if isinstance(first, nodes.If) and isinstance(first.body[-1], nodes.Break):
             self.add_message("no-while-true", node=node, args=(first.test.as_string()))
 
     def _check_use_for_loop(self, node: nodes.While) -> None:
-        def get_relevant_vals(node: nodes.NodeNG, result: Set[nodes.NodeNG] = None) -> Tuple[bool, Set[nodes.NodeNG]]:
+        def get_relevant_vals(
+            node: nodes.NodeNG, result: Optional[Set[nodes.NodeNG]] = None
+        ) -> Tuple[bool, Set[nodes.NodeNG]]:
             result = result if result is not None else set()
 
             if isinstance(node, nodes.Const):
                 return True, result
             if isinstance(node, nodes.Name):
                 result.add(node)
                 return True, result
             if isinstance(node, nodes.BinOp):
                 v1 = get_relevant_vals(node.left, result)
                 v2 = get_relevant_vals(node.right, result)
                 return v1 and v2, result
-            if isinstance(node, nodes.Call) and node.func.as_string() == "len" and len(node.args) == 1:
+            if (
+                isinstance(node, nodes.Call)
+                and node.func.as_string() == "len"
+                and len(node.args) == 1
+            ):
                 return get_relevant_vals(node.args[0], result)
             return False, result
 
         # TODO allow different increments?
         def adds_or_subtracts_one(node: nodes.NodeNG) -> bool:
             if not isinstance(node, nodes.AssignName):
                 return False
 
             expr = node.parent
             if isinstance(expr, nodes.AugAssign):
                 return expr.op in ("+=", "-=") and get_const_value(expr.value) == 1
             if isinstance(expr, nodes.Assign) and isinstance(expr.value, nodes.BinOp):
                 binop = expr.value
-                return binop.op in ("+", "-") \
-                    and ((binop.left.as_string() == node.as_string() and get_const_value(binop.right) == 1)
-                         or (binop.right.as_string() == node.as_string() and get_const_value(binop.left) == 1))
+                return binop.op in ("+", "-") and (
+                    (
+                        binop.left.as_string() == node.as_string()
+                        and get_const_value(binop.right) == 1
+                    )
+                    or (
+                        binop.right.as_string() == node.as_string()
+                        and get_const_value(binop.left) == 1
+                    )
+                )
             return False
 
         test = node.test
-        if not isinstance(test, nodes.Compare) or len(test.ops) != 1 or test.ops[0][0] not in ("<", "<=", ">", ">="):
+        if (
+            not isinstance(test, nodes.Compare)
+            or len(test.ops) != 1
+            or test.ops[0][0] not in ("<", "<=", ">", ">=")
+        ):
             return
 
         lt, rt = test.left, test.ops[0][1]
         lt_decomposable, lt_vals = get_relevant_vals(lt)
         rt_decomposable, rt_vals = get_relevant_vals(rt)
         if not lt_decomposable or not rt_decomposable:
             return
 
         all_vals = lt_vals | rt_vals
-        listener = ModifiedListener(all_vals)
+        listener: ModifiedListener[None] = ModifiedListener(list(all_vals))
         listener.visit_many(node.body)
 
         all_modifiers = [(val in lt_vals, listener.get_all_modifiers(val)) for val in all_vals]
-        nonempty_modifiers = [(from_lt, modifiers) for (from_lt, modifiers) in all_modifiers if len(modifiers) > 0]
+        nonempty_modifiers = [
+            (from_lt, modifiers) for (from_lt, modifiers) in all_modifiers if len(modifiers) > 0
+        ]
 
         if len(nonempty_modifiers) != 1:
             return
 
         from_lt, only_modifiers = nonempty_modifiers[0]
         if len(only_modifiers) != 1:
             return
 
         only_modifier = only_modifiers[0]
 
-        if self._get_block_line(only_modifier).parent != node or not adds_or_subtracts_one(only_modifier) \
-                or (only_modifier.as_string() != lt.as_string() and only_modifier.as_string() != rt.as_string()):
+        if (
+            self._get_block_line(only_modifier).parent != node
+            or not adds_or_subtracts_one(only_modifier)
+            or (
+                only_modifier.as_string() != lt.as_string()
+                and only_modifier.as_string() != rt.as_string()
+            )
+        ):
             return
 
         self.add_message("use-for-loop", node=node)
 
     @only_required_for_messages("no-while-true", "use-for-loop")
     def visit_while(self, node: nodes.While) -> None:
         self._check_no_while_true(node)
@@ -127,29 +151,41 @@
     def _check_use_tighter_bounds(self, node: nodes.For) -> None:
         def compares_equality(node: nodes.NodeNG) -> bool:
             return isinstance(node, nodes.Compare) and len(node.ops) == 1 and node.ops[0][0] == "=="
 
         def compares_to_start(node: nodes.Compare, var: str, start: nodes.NodeNG) -> bool:
             left, (_, right) = node.left, node.ops[0]
             left, right = left.as_string(), right.as_string()
-            return (left == var and right == start.as_string()) or (left == start.as_string() and right == var)
+            return (left == var and right == start.as_string()) or (
+                left == start.as_string() and right == var
+            )
 
         def is_last_before_end(node: nodes.NodeNG, stop: nodes.NodeNG, step: nodes.NodeNG) -> bool:
             const_node = get_const_value(node)
             const_stop = get_const_value(stop)
             const_step = get_const_value(step)
-            return (isinstance(node, nodes.BinOp) and node.op == "-"
-                    and node.left.as_string() == stop.as_string() and node.right.as_string() == step.as_string()) \
-                or (isinstance(const_node, int) and isinstance(const_stop, int) and isinstance(const_step, int)
-                    and const_node == const_stop - const_step)
-
-        def compares_to_last_before_end(node: nodes.Compare, var: str, stop: nodes.NodeNG, step: nodes.NodeNG) -> bool:
+            return (
+                isinstance(node, nodes.BinOp)
+                and node.op == "-"
+                and node.left.as_string() == stop.as_string()
+                and node.right.as_string() == step.as_string()
+            ) or (
+                isinstance(const_node, int)
+                and isinstance(const_stop, int)
+                and isinstance(const_step, int)
+                and const_node == const_stop - const_step
+            )
+
+        def compares_to_last_before_end(
+            node: nodes.Compare, var: str, stop: nodes.NodeNG, step: nodes.NodeNG
+        ) -> bool:
             left, (_, right) = node.left, node.ops[0]
-            return (left.as_string() == var and is_last_before_end(right, stop, step)) \
-                or (is_last_before_end(left, stop, step) and right.as_string() == var)
+            return (left.as_string() == var and is_last_before_end(right, stop, step)) or (
+                is_last_before_end(left, stop, step) and right.as_string() == var
+            )
 
         def relevant_nodes(body: List[nodes.NodeNG]) -> Iterator[nodes.If]:
             first = body[0]
             if isinstance(first, nodes.If):
                 yield first
                 while first.has_elif_block():
                     first = first.orelse[0]
@@ -165,48 +201,58 @@
         start, stop, step = range_params
 
         var = node.target.as_string()
         if isinstance(node.body[0], nodes.If):
             if_ = node.body[0]
             test = if_.test
 
-            if compares_equality(test) and len(if_.body) == 1 and type(if_.body[-1]) in (nodes.Break, nodes.Continue):
+            if (
+                compares_equality(test)
+                and len(if_.body) == 1
+                and type(if_.body[-1]) in (nodes.Break, nodes.Continue)
+            ):
                 if compares_to_start(test, var, start):
                     self.add_message("use-tighter-boundaries", node=node, args=("first",))
                 elif compares_to_last_before_end(test, var, stop, step):
                     self.add_message("use-tighter-boundaries", node=node, args=("last",))
             # TODO expand, tips: len(node.body) == 1, isinstance(if_.body[-1], nodes.Return), allow nodes in the middle,
             #                    allow longer bodies
 
     @staticmethod
-    def _get_block_line(node: nodes.NodeNG):
+    def _get_block_line(node: nodes.NodeNG) -> nodes.NodeNG:
         while not isinstance(node, nodes.Statement):
             node = node.parent
         return node
 
     @staticmethod
-    def _get_last_block_line(node: nodes.NodeNG):
+    def _get_last_block_line(node: nodes.NodeNG) -> nodes.NodeNG:
         node = ImproperLoop._get_block_line(node)
 
         while node.next_sibling() is not None:
             node = node.next_sibling()
         return node
 
     def _check_modifying_iterable(self, node: nodes.For) -> None:
         iterated = node.iter
         if type(iterated) not in (nodes.Name, nodes.Attribute):  # TODO allow any node type
             return
 
-        listener = ModifiedListener({iterated})
+        listener: ModifiedListener[None] = ModifiedListener([iterated])
         listener.visit_many(node.body)
 
         for modifier in listener.get_sure_modifiers(iterated):
-            if isinstance(modifier, nodes.Call) \
-                    and type(self._get_last_block_line(modifier)) not in (nodes.Break, nodes.Return):
-                self.add_message("modifying-iterated-structure", node=modifier, args=(get_name(iterated),))
+            if isinstance(modifier, nodes.Call) and type(
+                self._get_last_block_line(modifier)
+            ) not in (
+                nodes.Break,
+                nodes.Return,
+            ):
+                self.add_message(
+                    "modifying-iterated-structure", node=modifier, args=(get_name(iterated),)
+                )
 
     def _check_control_variable_changes(self, node: nodes.For) -> None:
         def is_last_block(node: nodes.NodeNG, for_: nodes.For) -> bool:
             stmt = self._get_block_line(node)
             while not isinstance(node, nodes.Module):
                 if type(stmt) in (nodes.For, nodes.While):
                     return False
@@ -222,26 +268,37 @@
         if range_params is None:
             return
 
         control_var = node.target
         if control_var.as_string().startswith("_"):
             return
 
-        listener = ModifiedListener({control_var})
+        listener: ModifiedListener[None] = ModifiedListener([control_var])
         listener.visit_many(node.body)
 
         for modifier in listener.get_all_modifiers(control_var):
             mod_statement = self._get_block_line(modifier)
-            if isinstance(mod_statement, nodes.For) and mod_statement.target.as_string() == control_var.as_string():
-                self.add_message("loop-shadows-control-variable", node=mod_statement, args=(modifier.as_string()))
+            if (
+                isinstance(mod_statement, nodes.For)
+                and mod_statement.target.as_string() == control_var.as_string()
+            ):
+                self.add_message(
+                    "loop-shadows-control-variable", node=mod_statement, args=(modifier.as_string())
+                )
             if is_last_block(mod_statement, node):
-                self.add_message("changing-control-variable", node=mod_statement, args=(control_var.as_string(),))
-
-    @only_required_for_messages("use-tighter-boundaries", "modifying-iterated-structure", "changing-control-variable",
-                                "loop-shadows-control-variable")
+                self.add_message(
+                    "changing-control-variable", node=mod_statement, args=(control_var.as_string(),)
+                )
+
+    @only_required_for_messages(
+        "use-tighter-boundaries",
+        "modifying-iterated-structure",
+        "changing-control-variable",
+        "loop-shadows-control-variable",
+    )
     def visit_for(self, node: nodes.For) -> None:
         self._check_use_tighter_bounds(node)
         self._check_modifying_iterable(node)
         self._check_control_variable_changes(node)
 
 
 def register(linter: "PyLinter") -> None:
```

### Comparing `edulint-2.6.4/edulint/linting/checkers/modified_listener.py` & `edulint-2.7.1/edulint/linting/checkers/modified_listener.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 from edulint.linting.checkers.utils import BaseVisitor, Named, get_name
 
 
 T = TypeVar("T")
 
 
 class ModifiedListener(BaseVisitor[T]):
-
-    NON_PURE_METHODS = re.compile(r"append|clear|extend|insert|pop|remove|reverse|sort|add|.*update|write")
+    NON_PURE_METHODS = re.compile(
+        r"append|clear|extend|insert|pop|remove|reverse|sort|add|.*update|write"
+    )
 
     def __init__(self, watched: List[Named]):
         self.watched = watched
-        self.modified = {get_name(var): [] for var in watched}
+        self.modified: Dict[str, List[nodes.NodeNG]] = {get_name(var): [] for var in watched}
         self.stack = [{get_name(var): var.scope() for var in watched}]
         super().__init__()
 
-    def _init_var_in_scope(self, node: nodes.NodeNG) -> T:
+    def _init_var_in_scope(self, node: nodes.NodeNG) -> None:
         self.stack[-1][get_name(node)] = node.scope()
 
     def visit_functiondef(self, node: nodes.FunctionDef) -> T:
         self.stack.append({})
         for arg in node.args.args:
             self._init_var_in_scope(arg)
 
@@ -47,15 +48,17 @@
         return len(self.get_all_modifiers(node)) > (1 if allow_definition else 0)
 
     @staticmethod
     def _reassigns(node: nodes.NodeNG) -> bool:
         return type(node) in (nodes.AssignName, nodes.AssignAttr, nodes.DelName, nodes.DelAttr)
 
     def was_reassigned(self, node: nodes.NodeNG, allow_definition: bool) -> bool:
-        return sum(self._reassigns(mod) for mod in self.get_all_modifiers(node)) > (1 if allow_definition else 0)
+        return sum(self._reassigns(mod) for mod in self.get_all_modifiers(node)) > (
+            1 if allow_definition else 0
+        )
 
     def get_all_modifiers(self, node: nodes.NodeNG) -> List[nodes.NodeNG]:
         return self.modified[get_name(node)]
 
     def get_sure_modifiers(self, node: nodes.NodeNG) -> List[nodes.NodeNG]:
         result = []
         for modifier in self.get_all_modifiers(node):
@@ -80,15 +83,16 @@
         for scope in reversed(self.stack):
             if var in scope:
                 return scope
         return None
 
     def _is_same_var(self, var: Named, node: Named) -> bool:
         varname = get_name(var)
-        return varname == get_name(node) and self._get_var_scope(varname)[varname] == var.scope()
+        scope = self._get_var_scope(varname)
+        return varname == get_name(node) and scope is not None and scope[varname] == var.scope()
 
     def _visit_assigned_to(self, node: nodes.NodeNG) -> None:
         stripped = self._strip(node)
         if stripped is None:
             return
 
         if isinstance(node, nodes.AssignName) and get_name(stripped) not in self.stack[-1]:
@@ -116,17 +120,17 @@
         return self.visit_many(node.get_children())
 
     def visit_annassign(self, node: nodes.AnnAssign) -> T:
         self._visit_assigned_to(node.target)
         return self.visit_many(node.get_children())
 
     def visit_attribute(self, node: nodes.Attribute) -> T:
-        if isinstance(node.parent, nodes.Call) \
-                and ModifiedListener.NON_PURE_METHODS.match(node.attrname):
-
+        if isinstance(node.parent, nodes.Call) and ModifiedListener.NON_PURE_METHODS.match(
+            node.attrname
+        ):
             stripped = self._strip(node)
             if stripped is None:
                 return self.visit_many(node.get_children())
 
             for var in self.watched:
                 if self._is_same_var(var, stripped):
                     self.modified[get_name(var)].append(node.parent)
```

### Comparing `edulint-2.6.4/edulint/linting/checkers/python_ta_checkers.py` & `edulint-2.7.1/edulint/linting/checkers/python_ta_checkers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # combined from
 # https://github.com/pyta-uoft/pyta/blob/683505e2a910c2a252739094593406e4e0f29a85/python_ta/checkers/invalid_for_target_checker.py
 # https://github.com/pyta-uoft/pyta/blob/683505e2a910c2a252739094593406e4e0f29a85/python_ta/checkers/one_iteration_checker.py
 # https://github.com/pyta-uoft/pyta/blob/683505e2a910c2a252739094593406e4e0f29a85/python_ta/checkers/shadowing_in_comprehension_checker.py
 # https://github.com/pyta-uoft/pyta/blob/683505e2a910c2a252739094593406e4e0f29a85/python_ta/checkers/top_level_code_checker.py
 
 
-from typing import Union
+from typing import TYPE_CHECKING, Union, List
 
 import re
 
 from astroid import nodes
 from pylint.checkers import BaseChecker
 from pylint.checkers.base import UpperCaseStyle
 from pylint.checkers.utils import only_required_for_messages
 
+if TYPE_CHECKING:
+    from pylint.lint import PyLinter
+
+from edulint.linting.checkers.utils import is_main_block
+
 
 class InvalidForTargetChecker(BaseChecker):
     # name is the same as file name but without _checker part
     name = "invalid_for_target"
     # use dashes for connecting words in message symbol
     msgs = {
         "E9984": (
@@ -42,15 +47,14 @@
     def visit_comprehension(self, node: nodes.Comprehension) -> None:
         invalid_for_targets = node.target.nodes_of_class(self.INVALID_TARGETS)
         for target in invalid_for_targets:
             self.add_message("invalid-for-target", node=target, args=target.as_string())
 
 
 class OneIterationChecker(BaseChecker):
-
     # name is the same as file name but without _checker part
     name = "one_iteration"
     # use dashes for connecting words in message symbol
     msgs = {
         "E9996": (
             "This loop will only ever run for one iteration",
             "one-iteration",
@@ -60,20 +64,20 @@
     }
 
     # this is important so that your checker is executed before others
     priority = -1
 
     # pass in message symbol as a parameter of only_required_for_messages
     @only_required_for_messages("one-iteration")
-    def visit_for(self, node):
+    def visit_for(self, node: nodes.For) -> None:
         if self._check_one_iteration(node):
             self.add_message("one-iteration", node=node)
 
     @only_required_for_messages("one-iteration")
-    def visit_while(self, node):
+    def visit_while(self, node: nodes.While) -> None:
         if self._check_one_iteration(node):
             self.add_message("one-iteration", node=node)
 
     def _check_one_iteration(self, node: Union[nodes.For, nodes.While]) -> bool:
         """Return whether the given loop is guaranteed to stop after one iteration.
         More precisely, Returns False if there exists a direct predecessor
         block `p` to the start of the loop block `s` such that the
@@ -98,32 +102,35 @@
                 if isinstance(node, nodes.For) and stmt is node.iter:
                     continue
                 return False
         return True
 
 
 class ShadowingInComprehensionChecker(BaseChecker):
-
     name = "shadowing_in_comprehension"
     msgs = {
         "E9988": (
             "Comprehension variable '%s' shadows a variable in an outer scope",
             "shadowing-in-comprehension",
             "Used when there is shadowing inside a comprehension",
         )
     }
 
     # this is important so that your checker is executed before others
     priority = -1
 
     @only_required_for_messages("shadowing-in-comprehension")
-    def visit_comprehension(self, node: nodes.Comprehension):
+    def visit_comprehension(self, node: nodes.Comprehension) -> None:
         if isinstance(node.target, nodes.Tuple):
             for target in node.target.elts:
-                if target.name in node.parent.frame().locals and target.name != "_":
+                if (
+                    isinstance(target, nodes.Name)
+                    and target.name in node.parent.frame().locals
+                    and target.name != "_"
+                ):
                     args = target.name
                     self.add_message("shadowing-in-comprehension", node=target, args=args)
         elif isinstance(node.target, nodes.AssignName):
             if node.target.name in node.parent.frame().locals and node.target.name != "_":
                 args = node.target.name
                 self.add_message("shadowing-in-comprehension", node=node.target, args=args)
 
@@ -139,73 +146,56 @@
         )
     }
 
     # this is important so that your checker is executed before others
     priority = -1
 
     @only_required_for_messages("forbidden-top-level-code")
-    def visit_module(self, node):
+    def visit_module(self, node: nodes.Module) -> None:
         for statement in node.body:
             if not (
                 _is_import(statement)
                 or _is_definition(statement)
                 or _is_assignment(statement)
-                or _is_main_block(statement)
+                or is_main_block(statement)
             ):
                 self.add_message("forbidden-top-level-code", node=statement, args=statement.lineno)
 
 
 # Helper functions
-def _is_import(statement) -> bool:
+def _is_import(statement: nodes.NodeNG) -> bool:
     """
     Return whether or not <statement> is an Import or an ImportFrom.
     """
     return isinstance(statement, (nodes.Import, nodes.ImportFrom))
 
 
-def _is_definition(statement) -> bool:
+def _is_definition(statement: nodes.NodeNG) -> bool:
     """
     Return whether or not <statement> is a function definition or a class definition.
     """
     return isinstance(statement, (nodes.FunctionDef, nodes.ClassDef))
 
 
-def _is_constant_assignment(statement) -> bool:
+def _is_constant_assignment(statement: nodes.NodeNG) -> bool:
     """
     Return whether or not <statement> is a constant assignment.
     """
     if not isinstance(statement, nodes.Assign):
         return False
 
-    names = []
+    names: List[str] = []
     for target in statement.targets:
         names.extend(node.name for node in target.nodes_of_class(nodes.AssignName, nodes.Name))
 
     return all(re.match(UpperCaseStyle.CONST_NAME_RGX, name) for name in names)
 
 
-def _is_assignment(statement) -> bool:
+def _is_assignment(statement: nodes.NodeNG) -> bool:
     return isinstance(statement, nodes.Assign)
 
 
-def _is_main_block(statement) -> bool:
-    """
-    Return whether or not <statement> is the main block.
-    """
-    return (
-        isinstance(statement, nodes.If)
-        and isinstance(statement.test, nodes.Compare)
-        and isinstance(statement.test.left, nodes.Name)
-        and isinstance(statement.test.left, nodes.Name)
-        and statement.test.left.name == "__name__"
-        and len(statement.test.ops) == 1
-        and statement.test.ops[0][0] == "=="
-        and isinstance(statement.test.ops[0][1], nodes.Const)
-        and statement.test.ops[0][1].value == "__main__"
-    )
-
-
-def register(linter):
+def register(linter: "PyLinter") -> None:
     linter.register_checker(InvalidForTargetChecker(linter))
     linter.register_checker(OneIterationChecker(linter))
     linter.register_checker(ShadowingInComprehensionChecker(linter))
     linter.register_checker(TopLevelCodeChecker(linter))
```

### Comparing `edulint-2.6.4/edulint/linting/checkers/short_problems.py` & `edulint-2.7.1/edulint/linting/checkers/short_problems.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,142 +1,156 @@
 from astroid import nodes  # type: ignore
 from typing import TYPE_CHECKING, Optional, List, Tuple, Union, Any, Callable
 
-from pylint.checkers import BaseChecker  # type: ignore
+from pylint.checkers import BaseChecker
 from pylint.checkers.utils import only_required_for_messages
 
 if TYPE_CHECKING:
-    from pylint.lint import PyLinter  # type: ignore
+    from pylint.lint import PyLinter
 
 from edulint.linting.checkers.utils import get_range_params, get_const_value, infer_to_value
 
 
 class Short(BaseChecker):
     name = "short-problems"
     msgs = {
         "R6601": (
             "Use %s.append(%s) instead of %s.",
             "use-append",
-            "Emitted when code extends list by a single argument instead of appending it."
+            "Emitted when code extends list by a single argument instead of appending it.",
         ),
         "R6602": (
             "Use integral division //.",
             "use-integral-division",
-            "Emitted when the code uses float division and converts the result to int."
+            "Emitted when the code uses float division and converts the result to int.",
         ),
         "R6603": (
             "Use isdecimal to test if string contains a number.",
             "use-isdecimal",
-            "Emitted when the code uses isdigit or isnumeric."
+            "Emitted when the code uses isdigit or isnumeric.",
         ),
         "R6604": (
             "Do not use %s loop with else.",
             "no-loop-else",
-            "Emitted when the code contains loop with else block."
+            "Emitted when the code contains loop with else block.",
         ),
         "R6605": (
             "Use elif.",
             "use-elif",
             "Emitted when the code contains else: if construction instead of elif. Might return a false positive if "
-            "the code mixes tabs and spaces."
+            "the code mixes tabs and spaces.",
         ),
         "R6606": (
             "Remove the for loop, as it makes %s.",
             "remove-for",
-            "Emitted when a for loop would always perform at most one iteration."
+            "Emitted when a for loop would always perform at most one iteration.",
         ),
         "R6607": (
             "Use %s instead of repeated %s in %s.",
             "no-repeated-op",
-            "Emitted when the code contains repeated adition/multiplication instead of multiplication/exponentiation."
+            "Emitted when the code contains repeated adition/multiplication instead of multiplication/exponentiation.",
         ),
         "R6608": (
             "Redundant arithmetic: %s",
             "redundant-arithmetic",
-            "Emitted when there is redundant arithmetic (e.g. +0, *1) in an expression."
+            "Emitted when there is redundant arithmetic (e.g. +0, *1) in an expression.",
         ),
         "R6609": (
             "Use augmenting assignment: '%s %s= %s'",
             "use-augmenting-assignment",
             "Emitted when an assignment can be simplified by using its augmented version.",
         ),
         "R6610": (
             "Do not multiply list with mutable content.",
             "do-not-multiply-mutable",
-            "Emitted when a list with mutable contents is being multiplied."
+            "Emitted when a list with mutable contents is being multiplied.",
         ),
         "R6611": (
             "Use else instead of elif.",
             "redundant-elif",
-            "Emitted when the condition in elif is negation of the condition in the if."
+            "Emitted when the condition in elif is negation of the condition in the if.",
         ),
         "R6612": (
             "Unreachable else.",
             "unreachable-else",
-            "Emitted when the else branch is unreachable due to totally exhaustive conditions before."
+            "Emitted when the else branch is unreachable due to totally exhaustive conditions before.",
         ),
         "R6613": (
             "Use '%s' directly rather than as '%s'.",
             "no-is-bool",
-            "Emitted when the is operator is used with a bool value."
+            "Emitted when the is operator is used with a bool value.",
         ),
         "R6614": (
-            "Use \"%s\" instead of using the magical constant %i.",
+            'Use "%s" instead of using the magical constant %i.',
             "use-ord-letter",
-            "Emitted when the code uses a magical constant instead of a string literal."
+            "Emitted when the code uses a magical constant instead of a string literal.",
         ),
         "R6615": (
             "Remove the call to 'ord' and compare to the string directly \"%s\" instead of using "
             "the magical constant %i. Careful, this may require changing the comparison operator.",
             "use-literal-letter",
-            "Emitted when the code uses a magical constant instead of a string literal in a comparison."
-        )
+            "Emitted when the code uses a magical constant instead of a string literal in a comparison.",
+        ),
     }
 
     def _check_extend(self, node: nodes.Call) -> None:
-        if isinstance(node.func, nodes.Attribute) and node.func.attrname == "extend" \
-                and len(node.args) == 1 \
-                and isinstance(node.args[0], nodes.List) and len(node.args[0].elts) == 1:
-            self.add_message("use-append", node=node, args=(
-                node.func.expr.as_string(),
-                node.args[0].elts[0].as_string(),
-                node.as_string()
-            ))
+        if (
+            isinstance(node.func, nodes.Attribute)
+            and node.func.attrname == "extend"
+            and len(node.args) == 1
+            and isinstance(node.args[0], nodes.List)
+            and len(node.args[0].elts) == 1
+        ):
+            self.add_message(
+                "use-append",
+                node=node,
+                args=(
+                    node.func.expr.as_string(),
+                    node.args[0].elts[0].as_string(),
+                    node.as_string(),
+                ),
+            )
 
     def _check_augassign_extend(self, node: nodes.AugAssign) -> None:
         if node.op == "+=" and isinstance(node.value, nodes.List) and len(node.value.elts) == 1:
-            self.add_message("use-append", node=node, args=(
-                node.target.as_string(),
-                node.value.elts[0].as_string(),
-                node.as_string())
+            self.add_message(
+                "use-append",
+                node=node,
+                args=(node.target.as_string(), node.value.elts[0].as_string(), node.as_string()),
             )
 
     def _check_isdecimal(self, node: nodes.Call) -> None:
-        if isinstance(node.func, nodes.Attribute) and node.func.attrname in ("isdigit", "isnumeric"):
+        if isinstance(node.func, nodes.Attribute) and node.func.attrname in (
+            "isdigit",
+            "isnumeric",
+        ):
             self.add_message("use-isdecimal", node=node)
 
     def _check_div(self, node: nodes.Call) -> None:
-        if isinstance(node.func, nodes.Name) and node.func.name == "int" \
-                and len(node.args) == 1 \
-                and isinstance(node.args[0], nodes.BinOp) and node.args[0].op == "/":
+        if (
+            isinstance(node.func, nodes.Name)
+            and node.func.name == "int"
+            and len(node.args) == 1
+            and isinstance(node.args[0], nodes.BinOp)
+            and node.args[0].op == "/"
+        ):
             self.add_message("use-integral-division", node=node)
 
     def _check_loop_else(self, nodes: List[nodes.NodeNG], parent_name: str) -> None:
         if nodes:
             self.add_message("no-loop-else", node=nodes[0].parent, args=(parent_name))
 
     def _check_else_if(self, node: nodes.If) -> None:
         if node.has_elif_block():
             first_body = node.body[0]
             first_orelse = node.orelse[0]
             if first_body.col_offset == first_orelse.col_offset:
                 self.add_message("use-elif", node=node.orelse[0])
 
     def _check_iteration_count(self, node: nodes.For) -> None:
-
         def get_const(node: nodes.NodeNG) -> Any:
             return node.value if isinstance(node, nodes.Const) else None
 
         range_params = get_range_params(node.iter)
         if range_params is None:
             return
 
@@ -145,16 +159,17 @@
 
         if start is not None and stop is not None and step is not None:
             if start >= stop:
                 self.add_message("remove-for", node=node, args=("no iterations",))
             elif start + step >= stop:
                 self.add_message("remove-for", node=node, args=("only one iteration",))
 
-    def _check_repeated_operation_rec(self, node: nodes.NodeNG, op: str, name: Optional[str] = None) \
-            -> Optional[Tuple[int, str]]:
+    def _check_repeated_operation_rec(
+        self, node: nodes.NodeNG, op: str, name: Optional[str] = None
+    ) -> Optional[Tuple[int, str]]:
         if isinstance(node, nodes.BinOp):
             if node.op != op:
                 return None
 
             lt = self._check_repeated_operation_rec(node.left, op, name)
             if lt is None:
                 return None
@@ -164,71 +179,109 @@
             rt = self._check_repeated_operation_rec(node.right, op, name_lt)
             if rt is None:
                 return None
 
             count_rt, _ = rt
             return count_lt + count_rt, name
 
-        if (name is None and type(node) in (nodes.Name, nodes.Attribute, nodes.Subscript)) or name == node.as_string():
+        if (
+            name is None and type(node) in (nodes.Name, nodes.Attribute, nodes.Subscript)
+        ) or name == node.as_string():
             return 1, node.as_string()
         return None
 
     def _check_repeated_operation(self, node: nodes.BinOp) -> None:
         if node.op in ("+", "*"):
             result = self._check_repeated_operation_rec(node, node.op)
             if result is None:
                 return
 
             # DANGER: on some structures, + may be available but not *
-            self.add_message("no-repeated-op", node=node, args=(
-                "multiplication" if node.op == "+" else "exponentiation",
-                "addition" if node.op == "+" else "muliplication",
-                node.as_string()
-            ))
+            self.add_message(
+                "no-repeated-op",
+                node=node,
+                args=(
+                    "multiplication" if node.op == "+" else "exponentiation",
+                    "addition" if node.op == "+" else "muliplication",
+                    node.as_string(),
+                ),
+            )
 
     def _check_redundant_arithmetic(self, node: Union[nodes.BinOp, nodes.AugAssign]) -> None:
         if isinstance(node, nodes.BinOp):
             op = node.op
             left = get_const_value(node.left)
             right = get_const_value(node.right)
         elif isinstance(node, nodes.AugAssign):
             op = node.op[:-1]
             left = None
             right = get_const_value(node.value)
         else:
             assert False, "unreachable"
 
-        if (op == "+" and (left in (0, "") or right in (0, ""))) \
-                or (op == "-" and (left == 0 or right == 0)) \
-                or (op == "*" and (left in (0, 1) or right in (0, 1))) \
-                or (op == "/" and right == 1) \
-                or (op in ("/", "//", "%")
-                    and (isinstance(node, nodes.BinOp) and node.left.as_string() == node.right.as_string()
-                         or isinstance(node, nodes.AugAssign) and node.target.as_string() == node.value.as_string())) \
-                or (op == "**" and right in (0, 1)):
+        if (
+            (op == "+" and (left in (0, "") or right in (0, "")))
+            or (op == "-" and (left == 0 or right == 0))
+            or (op == "*" and (left in (0, 1) or right in (0, 1)))
+            or (op == "/" and right == 1)
+            or (
+                op in ("/", "//", "%")
+                and (
+                    isinstance(node, nodes.BinOp)
+                    and node.left.as_string() == node.right.as_string()
+                    or isinstance(node, nodes.AugAssign)
+                    and node.target.as_string() == node.value.as_string()
+                )
+            )
+            or (op == "**" and right in (0, 1))
+        ):
             self.add_message("redundant-arithmetic", node=node, args=(node.as_string(),))
 
     def _check_augmentable(self, node: Union[nodes.Assign, nodes.AnnAssign]) -> None:
         IMMUTABLE_OPS = ("-", "*", "/", "//", "%", "**", "<<", ">>")
 
         def add_message(target: str, param: nodes.BinOp) -> None:
-            self.add_message("use-augmenting-assignment", node=node, args=(target, node.value.op, param.as_string()))
+            self.add_message(
+                "use-augmenting-assignment",
+                node=node,
+                args=(target, node.value.op, param.as_string()),
+            )
 
-        def is_immutable(node: nodes.NodeNG):
-            if isinstance(node, (nodes.Const)) and isinstance(node.value, (int, float, bool, str, bytes, tuple)):
+        def is_immutable(node: nodes.NodeNG) -> bool:
+            if isinstance(node, (nodes.Const)) and isinstance(
+                node.value, (int, float, bool, str, bytes, tuple)
+            ):
                 return True
             if isinstance(node, nodes.BinOp):
-                return node.op in IMMUTABLE_OPS \
-                    or is_immutable(node.left) or is_immutable(node.right)
+                return (
+                    node.op in IMMUTABLE_OPS or is_immutable(node.left) or is_immutable(node.right)
+                )
             if isinstance(node, nodes.Call):
-                return any(node.func.as_string().endswith(n) for n in (
-                    "int", "float", "bool", "str", "bytes", "tuple",
-                    "len", "sum", "chr", "ord",
-                    "trunc", "round", "sqrt", "cos", "sin", "radians", "degrees",
-                ))
+                return any(
+                    node.func.as_string().endswith(n)
+                    for n in (
+                        "int",
+                        "float",
+                        "bool",
+                        "str",
+                        "bytes",
+                        "tuple",
+                        "len",
+                        "sum",
+                        "chr",
+                        "ord",
+                        "trunc",
+                        "round",
+                        "sqrt",
+                        "cos",
+                        "sin",
+                        "radians",
+                        "degrees",
+                    )
+                )
             if isinstance(node, nodes.IfExp):
                 return is_immutable(node.body) or is_immutable(node.orelse)
             return False
 
         if not isinstance(node.value, nodes.BinOp):
             return
         bin_op = node.value
@@ -243,49 +296,67 @@
         left_value = infer_to_value(bin_op.left)
         right_value = infer_to_value(bin_op.right)
 
         if node.value.op in IMMUTABLE_OPS or is_immutable(left_value) or is_immutable(right_value):
             if target == bin_op.left.as_string():
                 add_message(target, bin_op.right)
             elif bin_op.op in "+*|&" and target == bin_op.right.as_string():
-                if not isinstance(left_value, nodes.Const) or not isinstance(left_value.value, (str, bytes, tuple)):
+                if not isinstance(left_value, nodes.Const) or not isinstance(
+                    left_value.value, (str, bytes, tuple)
+                ):
                     add_message(target, bin_op.left)
 
     def _check_multiplied_list(self, node: nodes.BinOp) -> None:
         def is_mutable(elem: nodes.NodeNG) -> bool:
-            return type(elem) in (nodes.List, nodes.Set, nodes.Dict) \
-                or (
-                    isinstance(elem, nodes.Call)
-                    and isinstance(elem.func, nodes.Name)
-                    and elem.func.name in ("list", "set", "dict")
-                )
+            return type(elem) in (nodes.List, nodes.Set, nodes.Dict) or (
+                isinstance(elem, nodes.Call)
+                and isinstance(elem.func, nodes.Name)
+                and elem.func.name in ("list", "set", "dict")
+            )
 
-        if node.op != "*" or (not isinstance(node.left, nodes.List) and not isinstance(node.right, nodes.List)):
+        if node.op != "*" or (
+            not isinstance(node.left, nodes.List) and not isinstance(node.right, nodes.List)
+        ):
             return
 
         assert not isinstance(node.left, nodes.List) or not isinstance(node.right, nodes.List)
         lst = node.left if isinstance(node.left, nodes.List) else node.right
 
         if any(is_mutable(elem) for elem in lst.elts):
             self.add_message("do-not-multiply-mutable", node=node)
 
     NEGATED_OP = {
-        ">=": "<", "<=": ">", ">": "<=", "<": ">=", "==": "!=", "!=": "==", "is": "is not", "is not": "is",
-        "in": "not in", "not in": "in", "and": "or", "or": "and"
+        ">=": "<",
+        "<=": ">",
+        ">": "<=",
+        "<": ">=",
+        "==": "!=",
+        "!=": "==",
+        "is": "is not",
+        "is not": "is",
+        "in": "not in",
+        "not in": "in",
+        "and": "or",
+        "or": "and",
     }
 
     def _check_redundant_elif(self, node: nodes.If) -> None:
-        def ops_match(lt: nodes.NodeNG, rt: nodes.NodeNG, lt_transform: Callable[[str], str]) -> bool:
-            return all(lt_transform(lt_op) == rt_op for (lt_op, _), (rt_op, _) in zip(lt.ops, rt.ops))
+        def ops_match(
+            lt: nodes.NodeNG, rt: nodes.NodeNG, lt_transform: Callable[[str], str]
+        ) -> bool:
+            return all(
+                lt_transform(lt_op) == rt_op for (lt_op, _), (rt_op, _) in zip(lt.ops, rt.ops)
+            )
 
         def to_values(node: nodes.NodeNG) -> List[nodes.NodeNG]:
             return [node.left] + [val for _, val in node.ops]
 
-        def all_are_negations(lt_values: List[nodes.NodeNG], rt_values: List[nodes.NodeNG], new_rt_negated: bool) \
-                -> bool:
+        def all_are_negations(
+            lt_values: List[nodes.NodeNG], rt_values: List[nodes.NodeNG], new_rt_negated: bool
+        ) -> bool:
             return all(is_negation(ll, rr, new_rt_negated) for ll, rr in zip(lt_values, rt_values))
 
         def strip_nots(node: nodes.NodeNG, negated_rt: bool) -> Tuple[nodes.NodeNG, bool]:
             while isinstance(node, nodes.UnaryOp) and node.op == "not":
                 negated_rt = not negated_rt
                 node = node.operand
             return node, negated_rt
@@ -294,16 +365,18 @@
             lt, negated_rt = strip_nots(lt, negated_rt)
             rt, negated_rt = strip_nots(rt, negated_rt)
 
             if not isinstance(lt, type(rt)):
                 return False
 
             if isinstance(lt, nodes.BoolOp) and isinstance(rt, nodes.BoolOp):
-                if len(lt.values) == len(rt.values) \
-                        and ((negated_rt and lt.op == rt.op) or (not negated_rt and Short.NEGATED_OP[lt.op] == rt.op)):
+                if len(lt.values) == len(rt.values) and (
+                    (negated_rt and lt.op == rt.op)
+                    or (not negated_rt and Short.NEGATED_OP[lt.op] == rt.op)
+                ):
                     return all_are_negations(lt.values, rt.values, negated_rt)
                 return False
 
             if isinstance(lt, nodes.Compare) and isinstance(rt, nodes.Compare):
                 if len(lt.ops) != len(rt.ops):
                     return False
 
@@ -323,75 +396,93 @@
         elif isinstance(node.next_sibling(), nodes.If) and len(node.next_sibling().orelse) == 0:
             next_if = node.next_sibling()
         else:
             return
 
         if is_negation(if_test, next_if.test, negated_rt=False):
             self.add_message("redundant-elif", node=next_if)
-            if node.has_elif_block() and next_if == node.orelse[0] and len(node.orelse[0].orelse) > 0:
+            if (
+                node.has_elif_block()
+                and next_if == node.orelse[0]
+                and len(node.orelse[0].orelse) > 0
+            ):
                 self.add_message("unreachable-else", node=node.orelse[0].orelse[0])
 
     def _check_no_is(self, node: nodes.Compare) -> None:
         for i, (op, val) in enumerate(node.ops):
-            if op in ("is", "is not") and isinstance(val, nodes.Const) and isinstance(val.value, bool):
+            if (
+                op in ("is", "is not")
+                and isinstance(val, nodes.Const)
+                and isinstance(val.value, bool)
+            ):
                 prev_val = node.ops[i - 1][1] if i > 0 else node.left
                 negate = (op == "is") != val.value
-                self.add_message("no-is-bool", node=node,
-                                 args=(f"{'not ' if negate else ''}{prev_val.as_string()}",
-                                       f"{prev_val.as_string()} {op} {val.as_string()}"))
+                self.add_message(
+                    "no-is-bool",
+                    node=node,
+                    args=(
+                        f"{'not ' if negate else ''}{prev_val.as_string()}",
+                        f"{prev_val.as_string()} {op} {val.as_string()}",
+                    ),
+                )
 
     def _is_ord(self, node: nodes.NodeNG) -> bool:
         return isinstance(node, nodes.Call) and node.func.as_string() == "ord"
 
     def _contains_ord(self, node: nodes.NodeNG) -> bool:
         if self._is_ord(node):
             return True
         if isinstance(node, nodes.BinOp):
             return self._is_ord(node.left) or self._is_ord(node.right)
         return False
 
     def _is_preffered(self, value: int) -> bool:
-        return chr(value) in 'azAZ09'
+        return chr(value) in "azAZ09"
 
     def _in_suggestable_range(self, value: int) -> bool:
-        return ord(' ') <= value < 127  # chr(127) is weird
+        return ord(" ") <= value < 127  # chr(127) is weird
 
     def _check_use_ord_letter(self, node: nodes.BinOp) -> None:
-        def add_message(param: nodes.NodeNG, value: int, suggestion: str):
+        def add_message(param: nodes.NodeNG, value: int, suggestion: str) -> None:
             self.add_message("use-ord-letter", node=param, args=(suggestion, value))
 
         if node.op not in ("+", "-"):
             return
 
         for ord_param, const_param in ((node.left, node.right), (node.right, node.left)):
             value = get_const_value(const_param)
-            if value is None or not isinstance(value, int) or not self._in_suggestable_range(value) \
-                    or not self._contains_ord(ord_param):
+            if (
+                value is None
+                or not isinstance(value, int)
+                or not self._in_suggestable_range(value)
+                or not self._contains_ord(ord_param)
+            ):
                 continue
 
             if self._is_preffered(value + 1):
                 suggestion = f"ord('{chr(value + 1)}') - 1"
             elif self._is_preffered(value - 1):
                 suggestion = f"ord('{chr(value - 1)}') + 1"
             elif not isinstance(ord_param, nodes.BinOp) or self._is_preffered(value):
                 suggestion = f"ord('{chr(value)}')"
             else:
                 continue
 
-            if (node.op == "-" and const_param == node.right and suggestion.endswith("+ 1")) \
-                    or (node.op == "+" and const_param == node.left and suggestion.endswith("- 1")):
+            if (node.op == "-" and const_param == node.right and suggestion.endswith("+ 1")) or (
+                node.op == "+" and const_param == node.left and suggestion.endswith("- 1")
+            ):
                 add_message(const_param, value, f"({suggestion})")
             else:
                 add_message(const_param, value, suggestion)
 
     def _check_magical_constant_in_ord_compare(self, node: nodes.Compare) -> None:
         def add_message(param: nodes.NodeNG, value: int, suggestion: str) -> None:
             self.add_message("use-literal-letter", node=param, args=(suggestion, value))
 
-        def change(op: str):
+        def change(op: str) -> str:
             if op == "<":
                 return "<="
             if op == "<=":
                 return "<"
             if op == ">":
                 return ">="
             if op == ">=":
@@ -411,22 +502,30 @@
 
             if i == 0:
                 op, other = node.ops[0]
                 if self._is_preffered(value + 1) and op in ("<", ">="):
                     add_message(param, value, f"'{chr(value + 1)}' {change(op)}")
                 elif self._is_preffered(value - 1) and op in (">", "<="):
                     add_message(param, value, f"'{chr(value - 1)}' {change(op)}")
-                elif not contains_ord[1] or not isinstance(other, nodes.BinOp) or self._is_preffered(value):
+                elif (
+                    not contains_ord[1]
+                    or not isinstance(other, nodes.BinOp)
+                    or self._is_preffered(value)
+                ):
                     add_message(param, value, f"'{chr(value)}' {op}")
             else:
                 if self._is_preffered(value + 1) and op in (">", "<="):
                     add_message(param, value, f"{change(op)} '{chr(value + 1)}'")
                 elif self._is_preffered(value - 1) and op in ("<", ">="):
                     add_message(param, value, f"{change(op)} '{chr(value - 1)}'")
-                elif not contains_ord[-2] or not isinstance(all_ops[-2][1], nodes.BinOp) or self._is_preffered(value):
+                elif (
+                    not contains_ord[-2]
+                    or not isinstance(all_ops[-2][1], nodes.BinOp)
+                    or self._is_preffered(value)
+                ):
                     add_message(param, value, f"{op} '{chr(value)}'")
 
     @only_required_for_messages("use-append", "use-isdecimal", "use-integral-division")
     def visit_call(self, node: nodes.Call) -> None:
         self._check_extend(node)
         self._check_isdecimal(node)
         self._check_div(node)
@@ -446,15 +545,17 @@
         self._check_iteration_count(node)
 
     @only_required_for_messages("use-elif", "redundant-elif")
     def visit_if(self, node: nodes.If) -> None:
         self._check_else_if(node)
         self._check_redundant_elif(node)
 
-    @only_required_for_messages("no-repeated-op", "redundant-arithmetic", "do-not-multiply-mutable", "use-ord-letter")
+    @only_required_for_messages(
+        "no-repeated-op", "redundant-arithmetic", "do-not-multiply-mutable", "use-ord-letter"
+    )
     def visit_binop(self, node: nodes.BinOp) -> None:
         self._check_repeated_operation(node)
         self._check_redundant_arithmetic(node)
         self._check_multiplied_list(node)
         self._check_use_ord_letter(node)
 
     @only_required_for_messages("use-augmenting-assignment")
```

### Comparing `edulint-2.6.4/edulint/linting/checkers/simplifiable_if.py` & `edulint-2.7.1/edulint/linting/checkers/simplifiable_if.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,122 +1,132 @@
 from astroid import nodes  # type: ignore
-from typing import TYPE_CHECKING, Optional, Tuple
+from typing import TYPE_CHECKING, Optional, Tuple, Union, List
 
 from pylint.checkers import BaseChecker  # type: ignore
 from pylint.checkers.utils import only_required_for_messages
 
 if TYPE_CHECKING:
     from pylint.lint import PyLinter  # type: ignore
 
 from edulint.linting.checkers.utils import get_name, get_assigned_to, is_any_assign
 
 
 class SimplifiableIf(BaseChecker):  # type: ignore
-
     name = "simplifiable-if"
     msgs = {
         "R6201": (
             "The if statement can be replaced with 'return %s'",
             "simplifiable-if-return",
             "Emitted when the condition of an if statement can be returned directly (possibly negated).",
         ),
         "R6202": (
             "The if statement can be replaced with 'return %s'",
             "simplifiable-if-return-conj",
             "Emitted when the condition of an if statement and the returned values "
-            "can be combined using logical operators."
+            "can be combined using logical operators.",
         ),
         "R6203": (
             "The conditional assignment can be replace with '%s = %s'",
             "simplifiable-if-assignment",
-            "Emitted when the condition of an if statement can be assigned directly (possibly negated)."
+            "Emitted when the condition of an if statement can be assigned directly (possibly negated).",
         ),
         "R6210": (
             "The conditional assignment can be replace with '%s = %s'",
             "simplifiable-if-assignment-conj",
             "Emitted when the condition of an if statement and the assigned values "
-            "can be combined using logical operators."
+            "can be combined using logical operators.",
         ),
         "R6204": (
             "The if expression can be replaced with '%s'",
             "simplifiable-if-expr",
-            "Emitted when the condition of an if expression can be returned directly (possibly negated)."
+            "Emitted when the condition of an if expression can be returned directly (possibly negated).",
         ),
         "R6209": (
             "The if expression can be replaced with '%s'",
             "simplifiable-if-expr-conj",
             "Emitted when the condition of an if expression and the returned values "
-            "can be combined using logical operators."
+            "can be combined using logical operators.",
         ),
         "R6205": (
             "Use 'if %s: <else body>' instead of 'pass'",
             "simplifiable-if-pass",
-            "Emitted when there is an if condition with a pass in the positive branch."
+            "Emitted when there is an if condition with a pass in the positive branch.",
         ),
         "R6206": (
             "Both branches should return a value explicitly (one returns implicit None)",
             "no-value-in-one-branch-return",
-            "Emitted when one branch returns a value and the other just returns."
+            "Emitted when one branch returns a value and the other just returns.",
         ),
         "R6207": (
             "The if statement can be merged with the nested one to 'if %s:'",
             "simplifiable-if-nested",
             "Emitted when the condition of an if statement can be merged "
-            "with its nested if's condition using logical operators."
+            "with its nested if's condition using logical operators.",
         ),
         "R6208": (
             "The if statement can be merged with the following one to 'if %s:'",
             "simplifiable-if-seq",
             "Emitted when the condition of an if statement can be merged "
-            "with the next if's condition using logical operators."
+            "with the next if's condition using logical operators.",
         ),
     }
 
     def _is_bool(self, node: nodes.NodeNG) -> bool:
         return isinstance(node, nodes.Const) and node.pytype() == "builtins.bool"
 
-    def _simplifiable_if_message(self, node: nodes.If, then: nodes.NodeNG, new_cond: str, only_replaces: bool) -> None:
+    def _simplifiable_if_message(
+        self, node: nodes.If, then: nodes.NodeNG, new_cond: str, only_replaces: bool
+    ) -> None:
         extra = "" if only_replaces else "-conj"
         if isinstance(node, nodes.IfExp):
             self.add_message("simplifiable-if-expr" + extra, node=node, args=(new_cond))
         elif isinstance(then, nodes.Return):
             self.add_message("simplifiable-if-return" + extra, node=node, args=(new_cond))
         else:
-            self.add_message("simplifiable-if-assignment" + extra, node=node,
-                             args=(get_name(get_assigned_to(then)[0]), new_cond))
+            self.add_message(
+                "simplifiable-if-assignment" + extra,
+                node=node,
+                args=(get_name(get_assigned_to(then)[0]), new_cond),
+            )
 
-    def _get_refactored(self, *args) -> str:
+    def _get_refactored(self, *args: Union[str, nodes.NodeNG]) -> str:
         result = []
         i = 0
         while i < len(args):
             arg = args[i]
             if isinstance(arg, str) and arg == "not":
-                refactored = args[i + 1].as_string()
-                if isinstance(args[i+1], nodes.BoolOp):
+                v = args[i + 1]
+                assert isinstance(v, nodes.NodeNG)
+                refactored = v.as_string()
+                if isinstance(v, nodes.BoolOp):
                     result.append(f"<negated ({refactored})>")
                 else:
                     result.append(f"<negated {refactored}>")
                 i += 2
             elif isinstance(arg, str) and arg in ("and", "or"):
                 prev = args[i - 1]
                 next_ = args[i + 1]
-                if isinstance(prev, nodes.BoolOp) and prev.op != arg and (i - 2 < 0 or args[i - 2] != "not"):
+                if (
+                    isinstance(prev, nodes.BoolOp)
+                    and prev.op != arg
+                    and (i - 2 < 0 or args[i - 2] != "not")
+                ):
                     result[-1] = f"({result[-1]})"
                 result.append(arg)
                 i += 1
                 if isinstance(next_, nodes.BoolOp) and next_.op != arg:
                     result.append(f"({next_.as_string()})")
                     i += 1
             elif isinstance(arg, nodes.NodeNG):
                 result.append(arg.as_string())
                 i += 1
 
         return " ".join(result)
 
-    def _names_assigned_to(self, node: nodes.NodeNG):
+    def _names_assigned_to(self, node: nodes.NodeNG) -> List[str]:
         return sorted([get_name(t) for t in get_assigned_to(node)])
 
     def _get_then_orelse(self, node: nodes.If) -> Optional[Tuple[nodes.NodeNG, nodes.NodeNG]]:
         if len(node.body) != 1 or len(node.orelse) > 1:
             return None
 
         then = node.body[0]
@@ -126,16 +136,17 @@
 
         after_if = node.next_sibling()
         if not isinstance(then, nodes.Return) or not isinstance(after_if, nodes.Return):
             return None
 
         return then, after_if
 
-    def _refactored_cond_from_then_orelse(self, node: nodes.If, then_value: nodes.NodeNG, orelse_value: nodes.NodeNG) \
-            -> Optional[Tuple[str, bool]]:
+    def _refactored_cond_from_then_orelse(
+        self, node: nodes.If, then_value: nodes.NodeNG, orelse_value: nodes.NodeNG
+    ) -> Optional[Tuple[str, bool]]:
         then_bool_value = then_value.value if self._is_bool(then_value) else None
         orelse_bool_value = orelse_value.value if self._is_bool(orelse_value) else None
 
         if then_bool_value is None and orelse_bool_value is None:
             return None
 
         if then_bool_value is not None and orelse_bool_value is not None:
@@ -160,87 +171,123 @@
         assert False, "unreachable"
 
     def _merge_nested(self, node: nodes.If) -> None:
         refactored = self._get_refactored(node.test, "and", node.body[0].test)
         self.add_message("simplifiable-if-nested", node=node, args=refactored)
 
     def _same_values(self, node1: nodes.NodeNG, node2: nodes.NodeNG) -> bool:
-        return (node1 is None and node2 is None) \
-             or (node1 is not None and node2 is not None and node1.as_string() == node2.as_string())
+        return (node1 is None and node2 is None) or (
+            node1 is not None and node2 is not None and node1.as_string() == node2.as_string()
+        )
 
     def _mergeable(self, node1: nodes.NodeNG, node2: nodes.NodeNG) -> bool:
         if not isinstance(node1, type(node2)):
             return False
 
         if isinstance(node1, nodes.Return):
             return node1.value is not None and node2.value is not None
 
         if is_any_assign(node1) and not isinstance(node1, nodes.For):
             assigned_to1 = get_assigned_to(node1)
             assigned_to2 = get_assigned_to(node2)
-            return len(assigned_to1) == 1 and len(assigned_to1) == len(assigned_to2) \
-                and isinstance(assigned_to1[0], type(assigned_to2[0])) \
-                and not isinstance(assigned_to1[0], nodes.Subscript) \
+            return (
+                len(assigned_to1) == 1
+                and len(assigned_to1) == len(assigned_to2)
+                and isinstance(assigned_to1[0], type(assigned_to2[0]))
+                and not isinstance(assigned_to1[0], nodes.Subscript)
                 and self._names_assigned_to(node1) == self._names_assigned_to(node2)
+            )
 
         return False
 
     def _merge_sequential(self, node: nodes.If) -> None:
         second_if = node.next_sibling()
 
-        if isinstance(node.test, nodes.BoolOp) or isinstance(second_if.test, nodes.BoolOp) \
-                or len(second_if.orelse) != 0 or len(node.body) != 1 or len(second_if.body) != 1:
+        if (
+            isinstance(node.test, nodes.BoolOp)
+            or isinstance(second_if.test, nodes.BoolOp)
+            or len(second_if.orelse) != 0
+            or len(node.body) != 1
+            or len(second_if.body) != 1
+        ):
             return
 
         body1 = node.body[0]
         body2 = second_if.body[0]
-        if not isinstance(body1, type(body2)) \
-                or not isinstance(body1, nodes.Return) \
-                or not self._same_values(body1.value, body2.value):
+        if (
+            not isinstance(body1, type(body2))
+            or not isinstance(body1, nodes.Return)
+            or not self._same_values(body1.value, body2.value)
+        ):
             return
 
         parent_body = node.parent.body
-        if all(isinstance(n, nodes.If) or isinstance(n, nodes.Return)
-                or (is_any_assign(n) and not isinstance(n, nodes.For)) for n in parent_body) \
-                and sum(1 if isinstance(n, nodes.If) else 0 for n in parent_body) > 2:
+        if (
+            all(
+                isinstance(n, nodes.If)
+                or isinstance(n, nodes.Return)
+                or (is_any_assign(n) and not isinstance(n, nodes.For))
+                for n in parent_body
+            )
+            and sum(1 if isinstance(n, nodes.If) else 0 for n in parent_body) > 2
+        ):
             return
 
         refactored = self._get_refactored(node.test, "or", second_if.test)
         self.add_message("simplifiable-if-seq", node=node, args=(refactored))
 
     def _is_just_returning_if(self, node: Optional[nodes.NodeNG]) -> bool:
-        return node is not None and isinstance(node, nodes.If) and isinstance(node.body[-1], nodes.Return)
-
-    @only_required_for_messages("simplifiable-if-return", "simplifiable-if-return-conj",
-                                "simplifiable-if-assignment", "simplifiable-if-assignment-conj",
-                                "simplifiable-if-pass", "no-value-in-one-branch-return",
-                                "simplifiable-if-nested", "simplifiable-if-seq")
+        return (
+            node is not None
+            and isinstance(node, nodes.If)
+            and isinstance(node.body[-1], nodes.Return)
+        )
+
+    @only_required_for_messages(
+        "simplifiable-if-return",
+        "simplifiable-if-return-conj",
+        "simplifiable-if-assignment",
+        "simplifiable-if-assignment-conj",
+        "simplifiable-if-pass",
+        "no-value-in-one-branch-return",
+        "simplifiable-if-nested",
+        "simplifiable-if-seq",
+    )
     def visit_if(self, node: nodes.If) -> None:
         if len(node.orelse) == 0:
-            if len(node.body) == 1 and isinstance(node.body[0], nodes.If) and len(node.body[0].orelse) == 0:
+            if (
+                len(node.body) == 1
+                and isinstance(node.body[0], nodes.If)
+                and len(node.body[0].orelse) == 0
+            ):
                 self._merge_nested(node)
                 return
 
             if node.next_sibling() is not None and isinstance(node.next_sibling(), nodes.If):
                 self._merge_sequential(node)
                 return
 
         if len(node.body) == 1 and isinstance(node.body[0], nodes.Pass) and len(node.orelse) > 0:
-            self.add_message("simplifiable-if-pass", node=node, args=(self._get_refactored("not", node.test)))
+            self.add_message(
+                "simplifiable-if-pass", node=node, args=(self._get_refactored("not", node.test))
+            )
             return
 
         then_orelse = self._get_then_orelse(node)
 
         if not then_orelse:
             return
 
         then, orelse = then_orelse
 
-        if isinstance(then, nodes.Return) and isinstance(orelse, nodes.Return) \
-                and (then.value is None) != (orelse.value is None):
+        if (
+            isinstance(then, nodes.Return)
+            and isinstance(orelse, nodes.Return)
+            and (then.value is None) != (orelse.value is None)
+        ):
             self.add_message("no-value-in-one-branch-return", node=node)
             return
 
         if not self._mergeable(then, orelse):
             return
 
         if len(node.orelse) == 0 and self._is_just_returning_if(node.previous_sibling()):
@@ -253,16 +300,17 @@
             self._simplifiable_if_message(node, then, new_cond, only_replaces)
 
     @only_required_for_messages("simplifiable-if-expr", "simplifiable-if-expr-conj")
     def visit_ifexp(self, node: nodes.IfExp) -> None:
         then, orelse = node.body, node.orelse
         assert then is not None and orelse is not None
 
-        if (not isinstance(then, nodes.Const) and not isinstance(then, nodes.Name)) or \
-                (not isinstance(orelse, nodes.Const) and not isinstance(orelse, nodes.Name)):
+        if (not isinstance(then, nodes.Const) and not isinstance(then, nodes.Name)) or (
+            not isinstance(orelse, nodes.Const) and not isinstance(orelse, nodes.Name)
+        ):
             return
 
         refactored = self._refactored_cond_from_then_orelse(node, then, orelse)
         if refactored is not None:
             new_cond, only_replaces = refactored
             self._simplifiable_if_message(node, then, new_cond, only_replaces)
```

### Comparing `edulint-2.6.4/edulint/linting/linting.py` & `edulint-2.7.1/edulint/linting/linting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 from typing import List, Callable, Tuple, Dict, Set, Any
-from edulint.config.arg import ImmutableArg
 from edulint.linting.problem import ProblemJson, Problem
 from edulint.linting.process_handler import ProcessHandler
 from edulint.linting.overrides import get_overriders
 from edulint.linting.tweakers import get_tweakers, Tweakers
 from edulint.config.config import Config
-from edulint.options import Option
+from edulint.options import Option, ImmutableT
 from edulint.linters import Linter
 from functools import partial
 import sys
 import json
-import pathlib
 import os
 
 
 def get_proper_path(path: str) -> str:
     return os.path.abspath(path) if os.path.isabs(path) else os.path.relpath(path)
 
 
 def flake8_to_problem(raw: ProblemJson) -> Problem:
     assert isinstance(raw["filename"], str), f'got {type(raw["filename"])} for filename'
     assert isinstance(raw["line_number"], int), f'got {type(raw["line_number"])} for line_number'
-    assert isinstance(raw["column_number"], int), f'got {type(raw["column_number"])} for column_number'
+    assert isinstance(
+        raw["column_number"], int
+    ), f'got {type(raw["column_number"])} for column_number'
     assert isinstance(raw["code"], str), f'got {type(raw["code"])} for code'
     assert isinstance(raw["text"], str), f'got {type(raw["text"])} for text'
 
     return Problem(
         Linter.FLAKE8,
         get_proper_path(raw["filename"]),
         raw["line_number"],
         raw["column_number"],
         raw["code"],
-        raw["text"]
+        raw["text"],
     )
 
 
 def pylint_to_problem(filenames: List[str], raw: ProblemJson) -> Problem:
     assert isinstance(raw["path"], str), f'got {type(raw["path"])} for path'
     assert isinstance(raw["line"], int), f'got {type(raw["line"])} for line'
     assert isinstance(raw["column"], int), f'got {type(raw["column"])} for column'
     assert isinstance(raw["message-id"], str), f'got {type(raw["message-id"])} for message-id'
     assert isinstance(raw["message"], str), f'got {type(raw["message"])} for message'
-    assert isinstance(raw["endLine"], int) or raw["endLine"] is None, f'got {type(raw["endLine"])} for endLine'
-    assert isinstance(raw["endColumn"], int) or raw["endColumn"] is None, f'got {type(raw["endColumn"])} for endColumn'
+    assert (
+        isinstance(raw["endLine"], int) or raw["endLine"] is None
+    ), f'got {type(raw["endLine"])} for endLine'
+    assert (
+        isinstance(raw["endColumn"], int) or raw["endColumn"] is None
+    ), f'got {type(raw["endColumn"])} for endColumn'
     assert isinstance(raw["symbol"], str), f'get {type(raw["symbol"])} for symbol'
 
     def get_used_filename(path: str) -> str:
         for filename in filenames:
             if os.path.abspath(filename) == os.path.abspath(path):
                 return filename
         assert False, "unreachable"
@@ -56,59 +60,75 @@
         get_proper_path(get_used_filename(raw["path"])),
         raw["line"],
         raw["column"],
         raw["message-id"],
         raw["message"],
         raw["endLine"],
         raw["endColumn"],
-        raw["symbol"]
+        raw["symbol"],
     )
 
 
 def lint_any(
-        linter: Linter, filenames: List[str], linter_args: List[str], config_arg: ImmutableArg,
-        result_getter: Callable[[Any], Any],
-        out_to_problem: Callable[[ProblemJson], Problem]) -> List[Problem]:
+    linter: Linter,
+    filenames: List[str],
+    linter_args: List[str],
+    config_arg: ImmutableT,
+    result_getter: Callable[[Any], Any],
+    out_to_problem: Callable[[ProblemJson], Problem],
+) -> List[Problem]:
     command = [sys.executable, "-m", str(linter)] + linter_args + list(config_arg) + filenames  # type: ignore
     return_code, outs, errs = ProcessHandler.run(command, timeout=1000)
 
     if ProcessHandler.is_status_code_by_timeout(return_code):
         print(f"edulint: {linter} was likely killed by timeout", file=sys.stderr)
         raise TimeoutError(f"Timeout from {linter}")
 
     print(errs, file=sys.stderr, end="")
-    if (linter == Linter.FLAKE8 and return_code not in (0, 1)) or (linter == Linter.PYLINT and return_code == 32):
+    if (linter == Linter.FLAKE8 and return_code not in (0, 1)) or (
+        linter == Linter.PYLINT and return_code == 32
+    ):
         print(f"edulint: {linter} exited with {return_code}", file=sys.stderr)
         exit(return_code)
 
     if not outs:
         return []
 
     result = result_getter(json.loads(outs))
     return list(map(out_to_problem, result))
 
 
 def lint_flake8(filenames: List[str], config: Config) -> List[Problem]:
     flake8_args = ["--format=json"]
     return lint_any(
-        Linter.FLAKE8, filenames, flake8_args, config[Option.FLAKE8],
+        Linter.FLAKE8,
+        filenames,
+        flake8_args,
+        config[Option.FLAKE8],
         lambda r: [problem for problems in r.values() for problem in problems],
-        flake8_to_problem)
+        flake8_to_problem,
+    )
 
 
 def lint_pylint(filenames: List[str], config: Config) -> List[Problem]:
-    pylintrc = (pathlib.Path(__file__).parent / ".pylintrc").resolve()
-    pylint_args = [f'--rcfile={pylintrc}', "--output-format=json"]
+    pylint_args = ["--output-format=json"]
     return lint_any(
-        Linter.PYLINT, filenames, pylint_args, config[Option.PYLINT],
-        lambda r: r, partial(pylint_to_problem, filenames))
+        Linter.PYLINT,
+        filenames,
+        pylint_args,
+        config[Option.PYLINT],
+        lambda r: r,
+        partial(pylint_to_problem, filenames),
+    )
 
 
 def apply_overrides(problems: List[Problem], overriders: Dict[str, Set[str]]) -> List[Problem]:
-    codes_on_lines: Dict[int, Set[str]] = {line: set() for line in set([problem.line for problem in problems])}
+    codes_on_lines: Dict[int, Set[str]] = {
+        line: set() for line in set([problem.line for problem in problems])
+    }
 
     for problem in problems:
         codes_on_lines[problem.line].add(problem.code)
 
     result = []
     for problem in problems:
         o = overriders.get(problem.code, set())
@@ -119,15 +139,17 @@
 
 
 def apply_tweaks(problems: List[Problem], tweakers: Tweakers, config: Config) -> List[Problem]:
     result = []
     for problem in problems:
         tweaker = tweakers.get((problem.source, problem.code))
         if tweaker:
-            if tweaker.should_keep(problem, [arg for arg in config if arg.option in tweaker.used_options]):
+            if tweaker.should_keep(
+                problem, [arg for arg in config if arg.option in tweaker.used_options]
+            ):
                 problem.text = tweaker.get_reword(problem)
                 result.append(problem)
         else:
             result.append(problem)
     return result
 
 
@@ -138,15 +160,17 @@
 def sort(filenames: List[str], problems: List[Problem]) -> List[Problem]:
     indices = {get_proper_path(fn): i for i, fn in enumerate(filenames)}
     problems.sort(key=lambda problem: (indices[problem.path], problem.line, problem.column))
     return problems
 
 
 def lint(filenames: List[str], config: Config) -> List[Problem]:
-    result = ([] if config[Option.NO_FLAKE8] else lint_flake8(filenames, config)) + lint_pylint(filenames, config)
+    result = ([] if config[Option.NO_FLAKE8] else lint_flake8(filenames, config)) + lint_pylint(
+        filenames, config
+    )
     result = apply_overrides(result, get_overriders())
     result = apply_tweaks(result, get_tweakers(), config)
     return sort(filenames, result)
 
 
 def lint_many(partition: List[Tuple[List[str], Config]]) -> List[Problem]:
     return [problem for filenames, config in partition for problem in lint(filenames, config)]
```

### Comparing `edulint-2.6.4/edulint/linting/overrides.py` & `edulint-2.7.1/edulint/linting/overrides.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.4/edulint/linting/problem.py` & `edulint-2.7.1/edulint/linting/problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 
 ProblemJson = Dict[str, Union[str, int]]
 
 
 @dataclass_json
 @dataclass
 class Problem:
-    source: Linter = field(metadata=config(
-        encoder=Linter.to_name,
-        decoder=Linter.from_name,
-        mm_field=mm_fields.Str()
-    ))
+    source: Linter = field(
+        metadata=config(encoder=Linter.to_name, decoder=Linter.from_name, mm_field=mm_fields.Str())
+    )
     path: str
     line: int
     column: int
     code: str
     text: str
     end_line: Optional[int] = None
     end_column: Optional[int] = None
@@ -54,17 +52,19 @@
 
     def set_end_column(self, v: Optional[int]) -> "Problem":
         self.end_column = v
         return self
 
     def has_value(self, attr: str) -> bool:
         val = getattr(self, attr)
-        return val is not None \
-            and (not isinstance(val, str) or val) \
+        return (
+            val is not None
+            and (not isinstance(val, str) or bool(val))
             and (not isinstance(val, int) or val >= 0)
+        )
 
     def __repr__(self) -> str:
         def get_attrvals() -> List[str]:
             result = []
             for f in fields(Problem):
                 attr = f.name
                 if self.has_value(attr):
```

### Comparing `edulint-2.6.4/edulint/linting/process_handler.py` & `edulint-2.7.1/edulint/linting/process_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 import os
 import sys
 from subprocess import PIPE, TimeoutExpired, Popen
 from typing import Optional, Tuple, List
 
 """ Author: Ondrej Borysek, License: MIT, Last update: 2021-04-19"""
 
-SIGKILL_STATUS_CODE = 137-128  # -9
-SIGTERM_STATUS_CODE = 143-128  # -15
+SIGKILL_STATUS_CODE = 137 - 128  # -9
+SIGTERM_STATUS_CODE = 143 - 128  # -15
 
 
 class ProcessHandler:
     """
-       This simple wrapper for subprocess library enables easier Input/Output testing of other programs.
-       No pip packages or additional linux packages are required.
-       Should work on Linux, Windows, and hopefully also on MacOS.
-       """
+    This simple wrapper for subprocess library enables easier Input/Output testing of other programs.
+    No pip packages or additional linux packages are required.
+    Should work on Linux, Windows, and hopefully also on MacOS.
+    """
 
     def __init__(self, timeout: float) -> None:
         self.last_child: Optional[Popen[bytes]] = None
         self.__try_to_be_nice()
         self.timeout: float = timeout
         self.sigterm_grace_period = 0.2  # second
         atexit.register(self.__kill_children)
         # Using prctl would be safer, but less portable: https://pythonhosted.org/python-prctl/#prctl.set_pdeathsig
 
     def __try_to_be_nice(self) -> None:
-        if getattr(os, 'nice', None):
+        if getattr(os, "nice", None):
             os.nice(10)
 
     def __kill_children(self) -> None:
         if self.last_child is None or self.last_child.poll() is not None:
             return
 
         print("Trying to terminate.", file=sys.stderr)
@@ -43,47 +43,55 @@
             print("Child refused to terminate. Trying SIGKILL if available.", file=sys.stderr)
             self.last_child.kill()  # Kill anyone still standing, just like Anakin did.
             # self.last_child.wait()  # Waiting would be safe on Linux, but on Windows .kill from Python
             # is just .terminate
 
         if self.last_child.poll():
             try:
-                _, _ = self.last_child.communicate(timeout=0.2)  # this can garbage collect the process
+                _, _ = self.last_child.communicate(
+                    timeout=0.2
+                )  # this can garbage collect the process
             except TimeoutExpired:
-                print("[Warning] The process refused to die. You might need to kill the zombie manually.",
-                      file=sys.stderr)
+                print(
+                    "[Warning] The process refused to die. You might need to kill the zombie manually.",
+                    file=sys.stderr,
+                )
                 ProcessHandler.linux_print_processes()
 
-    def __start_process(self, user_command: List[str], input_str: Optional[str] = None) -> Tuple[int, str, str]:
-
+    def __start_process(
+        self, user_command: List[str], input_str: Optional[str] = None
+    ) -> Tuple[int, str, str]:
         # Subprocess will be with the same niceness as the main program.
         # Warning: Do NOT use shell=True. That would only kill the shell, not the C program.
         proc = subprocess.Popen(user_command, shell=False, stdin=PIPE, stdout=PIPE, stderr=PIPE)
         self.last_child = proc
 
         return_code = SIGKILL_STATUS_CODE
 
         try:
-            outb, errb = proc.communicate(input=input_str.encode("utf8") if input_str else None, timeout=self.timeout)
+            outb, errb = proc.communicate(
+                input=input_str.encode("utf8") if input_str else None, timeout=self.timeout
+            )
             return_code = proc.returncode
         except TimeoutExpired:
             print("Timeout, trying to kill.", file=sys.stderr)
             proc.kill()
             outb, errb = proc.communicate()
             # proc.returncode will be ignored
 
         self.__kill_children()
         return return_code, outb.decode(), errb.decode()
 
     @staticmethod
-    def run(command: List[str],
-            input_str: Optional[str] = None,
-            print_output: bool = False,
-            timeout: float = 5  # seconds
-            ) -> Tuple[int, str, str]:
+    def run(
+        command: List[str],
+        input_str: Optional[str] = None,
+        print_output: bool = False,
+        timeout: float = 5,  # seconds
+    ) -> Tuple[int, str, str]:
         if command is None:
             return -1, "", "No command provided"
 
         ph = ProcessHandler(timeout=timeout)
         return_code, outs, errs = ph.__start_process(command, input_str=input_str)
         if print_output:
             print("Command:", command)
@@ -95,35 +103,40 @@
 
     @staticmethod
     def prettyfi_the_output(a: str) -> str:
         return a.replace("\\r\\n", "\n").replace("\\n", "\n")
 
     @staticmethod
     def linux_print_processes() -> None:
-        if not sys.platform.startswith('linux'):
+        if not sys.platform.startswith("linux"):
             return
-        print("""Please check that you don't see any zombie processes from the process of testing. They would have nice
-              value of 19. You can use command "ps a -o pid,ni,time,cmd" """, file=sys.stderr)
+        print(
+            """Please check that you don't see any zombie processes from the process of testing. They would have nice
+              value of 19. You can use command "ps a -o pid,ni,time,cmd" """,
+            file=sys.stderr,
+        )
 
     @staticmethod
     def is_status_code_by_timeout(status_code: int) -> bool:
         return status_code in [SIGTERM_STATUS_CODE, SIGKILL_STATUS_CODE]
 
 
 def usage_example() -> None:
-    command_to_execute = ['/bin/sh', '-c', 'echo Lorem Ipsum']
+    command_to_execute = ["/bin/sh", "-c", "echo Lorem Ipsum"]
     input_str = "Echo doesn't use input from stdin, but we can give it one anyway."
-    return_code, outs, errs = ProcessHandler.run(command_to_execute, input_str=input_str, print_output=True)
+    return_code, outs, errs = ProcessHandler.run(
+        command_to_execute, input_str=input_str, print_output=True
+    )
     assert return_code == 0
     assert "Lorem Ipsum" in outs  # beware different newlines based on system
     assert len(errs) == 0
 
 
 def usage_example_different_timeout() -> None:
-    command_to_execute = ['/bin/sh', '-c', 'while true; do sleep 1; done;']
+    command_to_execute = ["/bin/sh", "-c", "while true; do sleep 1; done;"]
     return_code, outs, errs = ProcessHandler.run(command_to_execute, print_output=True, timeout=0.5)
     assert return_code == -9  # SIGKILL
 
 
 if __name__ == "__main__":
     # Examples are presuming you're running Linux. If that's not the case, just edit the commands and arguments for
     # their Windows/other OS alternatives.
```

### Comparing `edulint-2.6.4/edulint/linting/tweakers.py` & `edulint-2.7.1/edulint/linting/tweakers.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,162 +35,107 @@
     if match.group(1).lower() == "module":
         return False
 
     name = match.group(2)
     style = match.group(3)
 
     if style == "snake_case naming style":
-        return name[0].isupper() or any(ch1.islower() and ch2.isupper() for ch1, ch2 in zip(name, name[1:]))
+        return name[0].isupper() or any(
+            ch1.islower() and ch2.isupper() for ch1, ch2 in zip(name, name[1:])
+        )
 
     if style == "PascalCase naming style":
         return name[0].islower() or "_" in name
 
     return True
 
 
 def disallowed_name_keep(self: Tweaker, problem: Problem, args: List[ImmutableArg]) -> bool:
-    if len(args) == 1 and args[0].option == Option.ALLOWED_ONECHAR_NAMES and args[0].val is not None:
+    if (
+        len(args) == 1
+        and args[0].option == Option.ALLOWED_ONECHAR_NAMES
+        and args[0].val is not None
+    ):
         assert isinstance(args[0].val, str)
         allowed_onechar_names = args[0].val
     else:
         allowed_onechar_names = ""
 
     match = self.match(problem)
     name = match.group(1)
 
     return len(name) != 1 or name not in allowed_onechar_names
 
 
 def disallowed_name_reword(self: Tweaker, problem: Problem) -> str:
     name = self.match(problem).group(1)
     if len(name) == 1:
-        return f"Disallowed single-character variable name \"{name}\", choose a more descriptive name"
+        return f'Disallowed single-character variable name "{name}", choose a more descriptive name'
     return problem.text
 
 
 def consider_using_in_reword(self: Tweaker, problem: Problem) -> str:
     match = self.match(problem)
 
     groups = match.groups()
     start = groups[0]
     outer_quote = groups[2]
     vals = groups[5].split(", ")
     assert vals
 
-    if all(val.count("(") == val.count(")") for val in vals) \
-            and all(v and v[0] == v[-1] and v[0] in "\"\'" and len(v) == 3 for v in vals):
+    if all(val.count("(") == val.count(")") for val in vals) and all(
+        v and v[0] == v[-1] and v[0] in "\"'" and len(v) == 3 for v in vals
+    ):
         inner_quote = vals[0][0]
-        return start + inner_quote + "".join(v.strip("\"\'") for v in vals) + inner_quote + outer_quote
+        return (
+            start + inner_quote + "".join(v.strip("\"'") for v in vals) + inner_quote + outer_quote
+        )
 
     return problem.text
 
 
-def _get_if_condition(filename: str, line: int) -> str:
-    line -= 1  # -1 adjusts for indexing from 0
-    with open(filename, encoding='utf8') as f:
-        lines = f.readlines()
-        result = [lines[line].strip()]
-        while result[-1][-1] == "\\":
-            result[-1] = result[-1].strip("\\ ")
-            line += 1
-            result.append(lines[line].strip())
-        return " ".join(result)
-
-
-def simplifiable_if_statement_reword(self: Tweaker, problem: Problem) -> str:
-    if_line = _get_if_condition(problem.path, problem.line)
-    if not if_line.startswith("if "):
-        return problem.text
-    if_line = if_line[len("if "):].strip(":")
-
-    match = self.match(problem)
-    return problem.text[:match.start(1)] + if_line + problem.text[match.end(1):]
-
-
-def _get_if_expression(problem: Problem) -> str:
-    with open(problem.path, encoding='utf8') as f:
-        selected_lines = f.readlines()[problem.line - 1:problem.end_line]
-    selected_lines[0] = selected_lines[0][problem.column:]  # no -1, columns indexed from 0
-
-    if problem.line == problem.end_line:
-        assert problem.end_column is not None
-        selected_lines[-1] = selected_lines[-1][:problem.end_column - problem.column]
-    else:
-        selected_lines[-1] = selected_lines[-1][:problem.end_column]
-
-    return " ".join(line.strip(" \t\n\\") for line in selected_lines)
-
-
-def simplifiable_if_expression_reword(self: Tweaker, problem: Problem) -> str:
-    if_expr = _get_if_expression(problem)
-    if_expr_match = re.match(r"(?:True|False) *if *(.*?) *else *(?:True|False)", if_expr)
-    if not if_expr_match:
-        return problem.text
-
-    match = self.match(problem)
-    return problem.text[:match.start(1)] + if_expr_match.group(1) + problem.text[match.end(1):]
-
-
 def unused_import_keep(self: Tweaker, problem: Problem, args: List[ImmutableArg]) -> bool:
     match = self.match(problem)
     return not match.group(1).startswith("ib111")
 
 
 def no_repeated_op_keep(self: Tweaker, problem: Problem, args: List[ImmutableArg]) -> bool:
     assert len(args) == 1 and args[0].option == Option.ENHANCEMENT
 
     match = self.match(problem)
     expr = match.group(1)
-    return args[0].val or expr.count("*") > 1
+    return bool(args[0].val) or expr.count("*") > 1
 
 
 Tweakers = Dict[Tuple[Linter, str], Tweaker]
 
 TWEAKERS = {
     (Linter.PYLINT, "C0103"): Tweaker(  # invalid-name
-        set(),
-        re.compile(r"^(.*) name \"(.*)\" doesn't conform to (.*)$"),
-        invalid_name_keep
+        set(), re.compile(r"^(.*) name \"(.*)\" doesn't conform to (.*)$"), invalid_name_keep
     ),
     (Linter.PYLINT, "C0104"): Tweaker(  # disallowed-name
         set([Option.ALLOWED_ONECHAR_NAMES]),
         re.compile(r"Disallowed name \"(.*)\""),
         disallowed_name_keep,
-        disallowed_name_reword
+        disallowed_name_reword,
     ),
     (Linter.PYLINT, "R1714"): Tweaker(  # consider-using-in
         set(),
         re.compile(
             r"^(Consider merging these comparisons with ['\"]in['\"] (to|by using) "
             r"(\"|\')([^\s]*)( not)? in )\((.+)\)(\"|\')"
         ),
-        reword=consider_using_in_reword
-    ),
-    (Linter.PYLINT, "R1703"): Tweaker(  # simplifiable-if-statement
-        set(),
-        re.compile(
-            r"^The if statement can be replaced with '.*?((?:bool\()?test\)?)'"
-        ),
-        reword=simplifiable_if_statement_reword
-    ),
-    (Linter.PYLINT, "R1719"): Tweaker(  # simplifiable-if-expression
-        set(),
-        re.compile(
-            r"^The if expression can be replaced with '.*?((?:bool\()?test\)?)'"
-        ),
-        reword=simplifiable_if_expression_reword
+        reword=consider_using_in_reword,
     ),
     (Linter.FLAKE8, "F401"): Tweaker(  # module imported but unused
-        set(),
-        re.compile("'(.*)' imported but unused"),
-        unused_import_keep
+        set(), re.compile("'(.*)' imported but unused"), unused_import_keep
     ),
     (Linter.PYLINT, "R6607"): Tweaker(  # no-repeated-op
         set([Option.ENHANCEMENT]),
         re.compile(r"^Use [^ ]* instead of repeated [^ ]* in ([^\.]*)."),
-        no_repeated_op_keep
-    )
+        no_repeated_op_keep,
+    ),
 }
 
 
 def get_tweakers() -> Tweakers:
     return TWEAKERS
```

### Comparing `edulint-2.6.4/edulint/prepare_explanations/__init__.py` & `edulint-2.7.1/edulint/prepare_explanations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 import tomli
 import tomli_w
 
 from pylint_data import extract_from_pylint
 from thonny_data import extract_from_edulint
 
 
-
 SCRIPT_PATH = os.path.dirname(os.path.abspath(__file__))
 PYLINT_FILE = extract_from_pylint.EDULINT_TOML
 THONNY_FILE = extract_from_edulint.EDULINT_TOML
 MANUAL_FILE = os.path.join(SCRIPT_PATH, "edulint_manual.toml")
 OUTPUT_FILE = os.path.join(SCRIPT_PATH, "../explanations.toml")
 
 
 def load_toml_file(filename: str) -> Dict[str, Any]:
-    with open(filename, 'rb') as f:
+    with open(filename, "rb") as f:
         return tomli.load(f)
 
 
 def combine_sources():
     pylint_data = load_toml_file(PYLINT_FILE)
     thonny_data = load_toml_file(THONNY_FILE)
     manual_data = load_toml_file(MANUAL_FILE)
@@ -32,21 +31,19 @@
     for data_source in [pylint_data, thonny_data, manual_data]:
         for check_id, check_data in data_source.items():
             for check_field_name, check_field_value in check_data.items():
                 if not check_field_value:
                     continue
                 answer[check_id][check_field_name] = check_field_value
 
-    with open(OUTPUT_FILE, 'wb') as f:
+    with open(OUTPUT_FILE, "wb") as f:
         tomli_w.dump(answer, f, multiline_strings=True)
 
 
-
 def main():
     extract_from_pylint.process_from_stored_data()
     extract_from_edulint.process_from_stored_data()
     combine_sources()
 
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `edulint-2.6.4/edulint/prepare_explanations/pylint_data/extract_from_pylint.py` & `edulint-2.7.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 import requests
 from tqdm import tqdm
 
 from thonny_process_slim import make_explanation_more_friedly
 
 # This doesn't work, but we need to version the code somewhere, so we might as well do it now.
 # pylint/doc/exts/pylint_messages is not in packaged pylint, but it's in the repo
-#from pylint_messages import _register_all_checkers_and_extensions, _get_all_messages, _get_message_data_path
+# from pylint_messages import _register_all_checkers_and_extensions, _get_all_messages, _get_message_data_path
 
 # _get_all_messages has to be modified:
-            # getattr(message, "shared", False),
-            # getattr(message, "default_enabled", False),
+# getattr(message, "shared", False),
+# getattr(message, "default_enabled", False),
 
 
 SCRIPT_PATH = os.path.dirname(os.path.abspath(__file__))
-PYLINT_EXPORT_JSON = os.path.join(SCRIPT_PATH, 'pylint_export.json')
-PYLINT_EXPORT_TOML = os.path.join(SCRIPT_PATH, 'pylint_export.toml')
-EDULINT_TOML = os.path.join(SCRIPT_PATH, '../edulint_pylint.toml')
+PYLINT_EXPORT_JSON = os.path.join(SCRIPT_PATH, "pylint_export.json")
+PYLINT_EXPORT_TOML = os.path.join(SCRIPT_PATH, "pylint_export.toml")
+EDULINT_TOML = os.path.join(SCRIPT_PATH, "../edulint_pylint.toml")
 
 
 class MyEncoder(json.JSONEncoder):
     def default(self, o):
         return o.__dict__
 
 
@@ -47,95 +47,97 @@
 
     for severity in messages:
         problems = messages[severity]
         for i in range(len(problems)):
             data_path = _get_message_data_path(problems[i].definition)
 
             problems[i] = problems[i]._asdict()
-            problems[i]['checker_module_path'] = 'REDACTED'
+            problems[i]["checker_module_path"] = "REDACTED"
             problems[i]["good_code"] = read_file_or_empty_string(data_path / "good.py")
             problems[i]["bad_code"] = read_file_or_empty_string(data_path / "bad.py")
-            
-    with open(output_filename, 'w', encoding='utf8') as f:
+
+    with open(output_filename, "w", encoding="utf8") as f:
         json.dump(messages, f, indent=4, cls=MyEncoder)
 
 
 def convert_json_to_toml(input_filename: str, output_filename: str):
-    with open(input_filename, encoding='utf8') as f:
+    with open(input_filename, encoding="utf8") as f:
         pylint_data = json.load(f)
-    
+
     answer = {}
     for severity in pylint_data:
         for checker in pylint_data[severity]:
             answer[checker["id"]] = checker
 
             checker["level"] = severity
             checker["description"] = checker["definition"]["description"]
             checker["msg"] = checker["definition"]["msg"]
             del checker["definition"]
 
             del checker["shared"]  # This prop is unreliable
             del checker["default_enabled"]  # This prop is unreliable
 
-    with open(output_filename, 'wb') as f:
+    with open(output_filename, "wb") as f:
         tomli_w.dump(answer, f, multiline_strings=True)
 
 
 def md_code_block_with_headline(code: str, headline: Optional[str] = None) -> str:
     if "# This is a placeholder for correct code for this message." in code:
         return ""
 
-    answer = ''
+    answer = ""
     if headline:
         answer += f"\n**{headline}**\n"
-    
+
     answer += f"""
 ```py
 {code}
 ```
 """
     return answer
 
 
 def produce_doc_link_if_available(checker: Dict[str, Any], skip_online_check: bool = True) -> str:
-    non_viable_text = '"**Additional details:**\n\nYou can help us make the doc better `by contributing'
-    if not checker['details'] or checker['details'].startswith(non_viable_text):
+    non_viable_text = (
+        '"**Additional details:**\n\nYou can help us make the doc better `by contributing'
+    )
+    if not checker["details"] or checker["details"].startswith(non_viable_text):
         return ""
-    
+
     doc_url = f'https://pylint.pycqa.org/en/latest/user_guide/messages/{checker["level"]}/{checker["name"]}.html'
     if not skip_online_check:
         resp = requests.get(doc_url)
         sleep(0.5)
         if resp.status_code != 200:
             return ""
-    
+
     return f'\n<a href="{doc_url}">Additional information</a>'
 
 
 def convert_pylint_toml_to_edulint_toml(input_filename: str, output_filename: str):
-    with open(input_filename, 'rb') as f:
+    with open(input_filename, "rb") as f:
         data = tomli.load(f)
 
     edulint_data = {}
 
     for checker_id, checker in tqdm(data.items()):
-        examples = ''
-        if checker['bad_code']:
-            examples += md_code_block_with_headline(checker['bad_code'], 'Problematic code')
-        if checker['good_code']:
-            examples += md_code_block_with_headline(checker['good_code'], 'How to fix it')
-        
+        examples = ""
+        if checker["bad_code"]:
+            examples += md_code_block_with_headline(checker["bad_code"], "Problematic code")
+        if checker["good_code"]:
+            examples += md_code_block_with_headline(checker["good_code"], "How to fix it")
+
         examples += produce_doc_link_if_available(checker)
 
         edulint_data[checker_id] = {
-            'why': make_explanation_more_friedly(checker['description']),
-            'examples': examples.lstrip(),
+            "why": make_explanation_more_friedly(checker["description"]),
+            "examples": examples.lstrip(),
         }
-        
-    with open(output_filename, 'wb') as f:
+
+    with open(output_filename, "wb") as f:
         tomli_w.dump(edulint_data, f, multiline_strings=True)
 
 
 def process_from_stored_data():
     convert_json_to_toml(PYLINT_EXPORT_JSON, PYLINT_EXPORT_TOML)
     convert_pylint_toml_to_edulint_toml(PYLINT_EXPORT_TOML, EDULINT_TOML)
```

#### html2text {}

```diff
@@ -1,57 +1,57 @@
 import json from pathlib import Path from typing import Optional, Dict, Any
 import os from time import sleep from pylint.lint import PyLinter import tomli
 import tomli_w import requests from tqdm import tqdm from thonny_process_slim
 import make_explanation_more_friedly # This doesn't work, but we need to
 version the code somewhere, so we might as well do it now. # pylint/doc/exts/
-pylint_messages is not in packaged pylint, but it's in the repo #from
+pylint_messages is not in packaged pylint, but it's in the repo # from
 pylint_messages import _register_all_checkers_and_extensions,
 _get_all_messages, _get_message_data_path # _get_all_messages has to be
 modified: # getattr(message, "shared", False), # getattr(message,
 "default_enabled", False), SCRIPT_PATH = os.path.dirname(os.path.abspath
 (__file__)) PYLINT_EXPORT_JSON = os.path.join(SCRIPT_PATH,
-'pylint_export.json') PYLINT_EXPORT_TOML = os.path.join(SCRIPT_PATH,
-'pylint_export.toml') EDULINT_TOML = os.path.join(SCRIPT_PATH, '../
-edulint_pylint.toml') class MyEncoder(json.JSONEncoder): def default(self, o):
+"pylint_export.json") PYLINT_EXPORT_TOML = os.path.join(SCRIPT_PATH,
+"pylint_export.toml") EDULINT_TOML = os.path.join(SCRIPT_PATH, "../
+edulint_pylint.toml") class MyEncoder(json.JSONEncoder): def default(self, o):
 return o.__dict__ def read_file_or_empty_string(filepath: str) -> str: if not
 Path(filepath).is_file(): return "" with open(filepath, encoding="utf8") as f:
 return f.read() def pylint_to_json(output_filename: str): linter = PyLinter()
 _register_all_checkers_and_extensions(linter) messages, _ = _get_all_messages
 (linter) for severity in messages: problems = messages[severity] for i in range
 (len(problems)): data_path = _get_message_data_path(problems[i].definition)
-problems[i] = problems[i]._asdict() problems[i]['checker_module_path'] =
-'REDACTED' problems[i]["good_code"] = read_file_or_empty_string(data_path /
+problems[i] = problems[i]._asdict() problems[i]["checker_module_path"] =
+"REDACTED" problems[i]["good_code"] = read_file_or_empty_string(data_path /
 "good.py") problems[i]["bad_code"] = read_file_or_empty_string(data_path /
-"bad.py") with open(output_filename, 'w', encoding='utf8') as f: json.dump
+"bad.py") with open(output_filename, "w", encoding="utf8") as f: json.dump
 (messages, f, indent=4, cls=MyEncoder) def convert_json_to_toml(input_filename:
-str, output_filename: str): with open(input_filename, encoding='utf8') as f:
+str, output_filename: str): with open(input_filename, encoding="utf8") as f:
 pylint_data = json.load(f) answer = {} for severity in pylint_data: for checker
 in pylint_data[severity]: answer[checker["id"]] = checker checker["level"] =
 severity checker["description"] = checker["definition"]["description"] checker
 ["msg"] = checker["definition"]["msg"] del checker["definition"] del checker
 ["shared"] # This prop is unreliable del checker["default_enabled"] # This prop
-is unreliable with open(output_filename, 'wb') as f: tomli_w.dump(answer, f,
+is unreliable with open(output_filename, "wb") as f: tomli_w.dump(answer, f,
 multiline_strings=True) def md_code_block_with_headline(code: str, headline:
 Optional[str] = None) -> str: if "# This is a placeholder for correct code for
-this message." in code: return "" answer = '' if headline: answer += f"\n**
+this message." in code: return "" answer = "" if headline: answer += f"\n**
 {headline}**\n" answer += f""" ```py {code} ``` """ return answer def
 produce_doc_link_if_available(checker: Dict[str, Any], skip_online_check: bool
-= True) -> str: non_viable_text = '"**Additional details:**\n\nYou can help us
-make the doc better `by contributing' if not checker['details'] or checker
-['details'].startswith(non_viable_text): return "" doc_url = f'https://
+= True) -> str: non_viable_text = ( '"**Additional details:**\n\nYou can help
+us make the doc better `by contributing' ) if not checker["details"] or checker
+["details"].startswith(non_viable_text): return "" doc_url = f'https://
 pylint.pycqa.org/en/latest/user_guide/messages/{checker["level"]}/{checker
 ["name"]}.html' if not skip_online_check: resp = requests.get(doc_url) sleep
 (0.5) if resp.status_code != 200: return "" return f'\nAdditional_information'
 def convert_pylint_toml_to_edulint_toml(input_filename: str, output_filename:
-str): with open(input_filename, 'rb') as f: data = tomli.load(f) edulint_data =
-{} for checker_id, checker in tqdm(data.items()): examples = '' if checker
-['bad_code']: examples += md_code_block_with_headline(checker['bad_code'],
-'Problematic code') if checker['good_code']: examples +=
-md_code_block_with_headline(checker['good_code'], 'How to fix it') examples +=
-produce_doc_link_if_available(checker) edulint_data[checker_id] = { 'why':
-make_explanation_more_friedly(checker['description']), 'examples':
-examples.lstrip(), } with open(output_filename, 'wb') as f: tomli_w.dump
+str): with open(input_filename, "rb") as f: data = tomli.load(f) edulint_data =
+{} for checker_id, checker in tqdm(data.items()): examples = "" if checker
+["bad_code"]: examples += md_code_block_with_headline(checker["bad_code"],
+"Problematic code") if checker["good_code"]: examples +=
+md_code_block_with_headline(checker["good_code"], "How to fix it") examples +=
+produce_doc_link_if_available(checker) edulint_data[checker_id] = { "why":
+make_explanation_more_friedly(checker["description"]), "examples":
+examples.lstrip(), } with open(output_filename, "wb") as f: tomli_w.dump
 (edulint_data, f, multiline_strings=True) def process_from_stored_data():
 convert_json_to_toml(PYLINT_EXPORT_JSON, PYLINT_EXPORT_TOML)
 convert_pylint_toml_to_edulint_toml(PYLINT_EXPORT_TOML, EDULINT_TOML) if
 __name__ == "__main__": # pylint_to_json(PYLINT_EXPORT_JSON)
 process_from_stored_data()
```

### Comparing `edulint-2.6.4/edulint/prepare_explanations/pylint_data/pylint_messages.py` & `edulint-2.7.1/edulint/prepare_explanations/pylint_data/pylint_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,36 +66,26 @@
     """Get the message data from the specified path."""
     good_py_path = data_path / "good.py"
     bad_py_path = data_path / "bad.py"
     details_rst_path = data_path / "details.rst"
     related_rst_path = data_path / "related.rst"
     if not data_path.exists():
         _create_placeholders(data_path, details_rst_path, good_py_path)
-    good_code = _get_titled_rst(
-        title="Correct code", text=_get_python_code_as_rst(good_py_path)
-    )
-    bad_code = _get_titled_rst(
-        title="Problematic code", text=_get_python_code_as_rst(bad_py_path)
-    )
-    details = _get_titled_rst(
-        title="Additional details", text=_get_rst_as_str(details_rst_path)
-    )
-    related = _get_titled_rst(
-        title="Related links", text=_get_rst_as_str(related_rst_path)
-    )
+    good_code = _get_titled_rst(title="Correct code", text=_get_python_code_as_rst(good_py_path))
+    bad_code = _get_titled_rst(title="Problematic code", text=_get_python_code_as_rst(bad_py_path))
+    details = _get_titled_rst(title="Additional details", text=_get_rst_as_str(details_rst_path))
+    related = _get_titled_rst(title="Related links", text=_get_rst_as_str(related_rst_path))
     _check_placeholders(bad_code, details, good_py_path, related)
     return good_code, bad_code, details, related
 
 
-def _check_placeholders(
-    bad_code: str, details: str, good_py_path: Path, related: str
-) -> None:
+def _check_placeholders(bad_code: str, details: str, good_py_path: Path, related: str) -> None:
     if bad_code or related:
         placeholder_details = "help us make the doc better" in details
-        with open(good_py_path, encoding='utf8') as f:
+        with open(good_py_path, encoding="utf8") as f:
             placeholder_good = "placeholder" in f.read()
         assert_msg = (
             f"Please remove placeholders in '{good_py_path.parent}' "
             f"as you started completing the documentation"
         )
         assert not placeholder_good and not placeholder_details, assert_msg
 
@@ -123,17 +113,15 @@
         return ""
     return f"""\
 .. literalinclude:: /{code_path.relative_to(Path.cwd())}
    :language: python
 """
 
 
-def _create_placeholders(
-    data_path: Path, details_rst_path: Path, good_py_path: Path
-) -> None:
+def _create_placeholders(data_path: Path, details_rst_path: Path, good_py_path: Path) -> None:
     data_path.mkdir(parents=True)
     with open(good_py_path, "w", encoding="utf-8") as file:
         file.write(
             """\
 # This is a placeholder for correct code for this message.
 """
         )
@@ -166,22 +154,19 @@
         "error": defaultdict(list),
         "warning": defaultdict(list),
         "convention": defaultdict(list),
         "refactor": defaultdict(list),
         "information": defaultdict(list),
     }
     checker_message_mapping = chain.from_iterable(
-        ((checker, msg) for msg in checker.messages)
-        for checker in linter.get_checkers()
+        ((checker, msg) for msg in checker.messages) for checker in linter.get_checkers()
     )
 
     for checker, message in checker_message_mapping:
-        good_code, bad_code, details, related = _get_message_data(
-            _get_message_data_path(message)
-        )
+        good_code, bad_code, details, related = _get_message_data(_get_message_data_path(message))
 
         checker_module = getmodule(checker)
 
         assert (
             checker_module and checker_module.__file__
         ), f"Cannot find module for checker {checker}"
 
@@ -248,17 +233,15 @@
         for message in messages:
             if message.shared:
                 continue
             if not _message_needs_update(message, category):
                 continue
             _write_single_message_page(category_dir, message)
         for _, shared_messages in groupby(
-            sorted(
-                (message for message in messages if message.shared), key=lambda m: m.id
-            ),
+            sorted((message for message in messages if message.shared), key=lambda m: m.id),
             key=lambda m: m.id,
         ):
             shared_messages_list = list(shared_messages)
             if len(shared_messages_list) > 1:
                 _write_single_shared_message_page(category_dir, shared_messages_list)
             else:
                 _write_single_message_page(category_dir, shared_messages_list[0])
@@ -296,31 +279,24 @@
    checker which requires the ``{message.checker_module_name}`` plugin to be loaded.
 
 """
     return body
 
 
 def _generate_checker_url(message: MessageData) -> str:
-    checker_module_rel_path = os.path.relpath(
-        message.checker_module_path, PYLINT_BASE_PATH
-    )
+    checker_module_rel_path = os.path.relpath(message.checker_module_path, PYLINT_BASE_PATH)
     return f"https://github.com/PyCQA/pylint/blob/main/{checker_module_rel_path}"
 
 
-def _write_single_shared_message_page(
-    category_dir: Path, messages: List[MessageData]
-) -> None:
+def _write_single_shared_message_page(category_dir: Path, messages: List[MessageData]) -> None:
     message = messages[0]
     with open(category_dir / f"{message.name}.rst", "w", encoding="utf-8") as stream:
         stream.write(_generate_single_message_body(message))
         checker_urls = ", ".join(
-            [
-                f"`{message.checker} <{_generate_checker_url(message)}>`__"
-                for message in messages
-            ]
+            [f"`{message.checker} <{_generate_checker_url(message)}>`__" for message in messages]
         )
         stream.write(f"Created by the {checker_urls} checkers.")
 
 
 def _write_single_message_page(category_dir: Path, message: MessageData) -> None:
     with open(category_dir / f"{message.name}.rst", "w", encoding="utf-8") as stream:
         stream.write(_generate_single_message_body(message))
@@ -361,17 +337,15 @@
         ):
             # We need to remove all duplicated shared messages
             messages = sorted(
                 {msg.id: msg for msg in messages_dict[category]}.values(),
                 key=lambda item: item.name,
             )
             old_messages = sorted(old_messages_dict[category], key=lambda item: item[0])
-            messages_string = "".join(
-                f"   {category}/{message.name}\n" for message in messages
-            )
+            messages_string = "".join(f"   {category}/{message.name}\n" for message in messages)
             old_messages_string = "".join(
                 f"   {category}/{old_message[0]}\n" for old_message in old_messages
             )
             # Write list per category. We need the '-category' suffix in the reference
             # because 'fatal' is also a message's symbol
             stream.write(
                 f"""
@@ -407,17 +381,15 @@
 
 def _write_redirect_old_page(
     category_dir: Path,
     old_name: Tuple[str, str],
     new_names: List[Tuple[str, str]],
 ) -> None:
     old_name_file = os.path.join(category_dir, f"{old_name[0]}.rst")
-    new_names_string = "".join(
-        f"   ../{new_name[1]}/{new_name[0]}.rst\n" for new_name in new_names
-    )
+    new_names_string = "".join(f"   ../{new_name[1]}/{new_name[0]}.rst\n" for new_name in new_names)
     content = f""".. _{old_name[0]}:
 
 {get_rst_title("/".join(old_name), "=")}
 "{old_name[0]} has been renamed. The new message can be found at:
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `edulint-2.6.4/edulint/prepare_explanations/pylint_data/thonny_process_slim.py` & `edulint-2.7.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     replace_prefixes = {
         "Used when an ": "It looks like the ",
         "Used when a ": "It looks like the ",
         "Used when ": "It looks like ",
         "Emitted when an ": "It looks like the ",
         "Emitted when a ": "It looks like the ",
         "Emitted when ": "It looks like ",
-    }    
+    }
 
     for prefix, replacement in replace_prefixes.items():
         if explanation.startswith(prefix):
-            explanation = replacement + explanation[len(prefix):]
+            explanation = replacement + explanation[len(prefix) :]
             break
-    
+
     return explanation
```

### Comparing `edulint-2.6.4/edulint/prepare_explanations/thonny_data/extract_from_edulint.py` & `edulint-2.7.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,43 +17,42 @@
     if not Path(FILENAME_TOML).is_file():
         reload_from_source = True
 
     if reload_from_source:
         checks = thonny_messages.checks_by_id
         for check in checks.values():
             if check.get("tho_xpln"):
-                check['customized_by_thonny'] = True
+                check["customized_by_thonny"] = True
 
         with open(FILENAME_TOML, "wb") as f:
             tomli_w.dump(checks, f, multiline_strings=True)
 
     with open(FILENAME_TOML, "rb") as f:
         checks = tomli.load(f)
 
-    return checks    
+    return checks
 
 
 def convert_to_edulint():
     with open(FILENAME_TOML, "rb") as f:
         checks = tomli.load(f)
 
-    checks = dict(filter(lambda x: x[1].get('customized_by_thonny'), checks.items()))
+    checks = dict(filter(lambda x: x[1].get("customized_by_thonny"), checks.items()))
 
     answer = {}
     for key, data in checks.items():
         answer[key] = {
-            'why': data['tho_xpln'],
-            'examples': '',
+            "why": data["tho_xpln"],
+            "examples": "",
         }
 
     with open(EDULINT_TOML, "wb") as f:
         tomli_w.dump(answer, f, multiline_strings=True)
 
 
 def process_from_stored_data():
     extract_msgs_from_thonny(reload_from_source=True)
     convert_to_edulint()
 
 
 if __name__ == "__main__":
     process_from_stored_data()
-
```

### Comparing `edulint-2.6.4/edulint/prepare_explanations/thonny_data/thonny_messages.py` & `edulint-2.7.1/edulint/prepare_explanations/thonny_data/thonny_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.4/edulint/prepare_explanations/thonny_data/thonny_process_backup.py` & `edulint-2.7.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # https://raw.githubusercontent.com/thonny/thonny/master/thonny/plugins/pylint/__init__.py
 
 
-import ast
 import subprocess
 from logging import getLogger
 
 from thonny import get_workbench, ui_utils
 from thonny.assistance import SubprocessProgramAnalyzer, add_program_analyzer
 from thonny.plugins.pylint.messages import checks_by_id
 from thonny.running import get_front_interpreter_for_subprocess
```

### Comparing `edulint-2.6.4/edulint.egg-info/PKG-INFO` & `edulint-2.7.1/edulint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.6.4
+Version: 2.7.1
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.6.4/edulint.egg-info/SOURCES.txt` & `edulint-2.7.1/edulint.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 ./edulint/explanations.toml
 ./edulint/linters.py
 ./edulint/options.py
 ./edulint/config/__init__.py
 ./edulint/config/arg.py
 ./edulint/config/config.py
 ./edulint/config/config_translations.py
-./edulint/linting/.pylintrc
+./edulint/config/file_config.py
+./edulint/config/files/default.toml
+./edulint/config/files/empty.toml
 ./edulint/linting/__init__.py
 ./edulint/linting/linting.py
 ./edulint/linting/overrides.py
 ./edulint/linting/problem.py
 ./edulint/linting/process_handler.py
 ./edulint/linting/tweakers.py
 ./edulint/linting/checkers/__init__.py
 ./edulint/linting/checkers/basic_checker.py
+./edulint/linting/checkers/duplication_checker.py
 ./edulint/linting/checkers/improper_loop.py
 ./edulint/linting/checkers/modified_listener.py
 ./edulint/linting/checkers/python_ta_checkers.py
 ./edulint/linting/checkers/short_problems.py
 ./edulint/linting/checkers/simplifiable_if.py
 ./edulint/linting/checkers/utils.py
 ./edulint/prepare_explanations/__init__.py
@@ -40,13 +43,14 @@
 ./edulint/prepare_explanations/thonny_data/thonny_process_backup.py
 edulint.egg-info/PKG-INFO
 edulint.egg-info/SOURCES.txt
 edulint.egg-info/dependency_links.txt
 edulint.egg-info/requires.txt
 edulint.egg-info/top_level.txt
 tests/test_config.py
+tests/test_duplication.py
 tests/test_improper_loop.py
 tests/test_lint.py
 tests/test_main.py
 tests/test_short_problems.py
 tests/test_simplifiable_if.py
 tests/test_visitors.py
```

### Comparing `edulint-2.6.4/setup.cfg` & `edulint-2.7.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -24,23 +24,24 @@
 python_requires = >=3.7
 install_requires = 
 	flake8 ==4.0.1
 	flake8-json ==21.7.0
 	pylint ==2.14.5
 	dataclasses-json
 	tomli
+	requests
 include_package_data = True
 
 [options.packages.find]
 where = .
 exclude = 
 	prepare_explanations/*
 
 [options.package_data]
 * = 
-	.pylintrc
 	explanations.toml
+	files/*
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `edulint-2.6.4/setup.py` & `edulint-2.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.4/tests/test_config.py` & `edulint-2.7.1/tests/test_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import pytest
 from edulint.linters import Linter
 from edulint.config.arg import UnprocessedArg, ProcessedArg
-from edulint.options import Option, TakesVal, Type, Combine, OptionParse, get_option_parses
-from edulint.config.config import Config, extract_args, parse_args, combine_and_translate
+from edulint.options import Option, TakesVal, Type, Combine, OptionParse, get_option_parses, DEFAULT_CONFIG
+from edulint.config.config import Config, extract_args, parse_args, parse_config_file, combine_and_translate
 from edulint.config.config_translations import get_config_translations, Translation
 from edulint.linting.tweakers import get_tweakers
 from typing import List, Set, Dict
+from pathlib import Path
 
 
 @pytest.fixture
 def all_advertised_options() -> List[Option]:
     return list(get_option_parses().keys())
 
 
 @pytest.fixture
 def advertised_options(all_advertised_options: List[Option]) -> Set[Option]:
     return set(all_advertised_options)
 
 
 @pytest.fixture
 def always_managed_options() -> Set[Option]:
-    return set((Option.PYLINT, Option.FLAKE8, Option.IB111_WEEK, Option.NO_FLAKE8))
+    return set((Option.CONFIG, Option.PYLINT, Option.FLAKE8, Option.IB111_WEEK, Option.NO_FLAKE8))
 
 
 @pytest.fixture
 def managed_translations_options() -> List[Option]:
     return list(get_config_translations().keys())
 
 
@@ -99,36 +100,50 @@
 
 
 @pytest.fixture
 def options() -> Dict[Option, OptionParse]:
     return {
         Option.PYTHON_SPECIFIC: OptionParse(Option.PYTHON_SPECIFIC, "", TakesVal.NO, False, Type.BOOL, Combine.REPLACE),
         Option.FLAKE8: OptionParse(Option.FLAKE8, "", TakesVal.YES, [], Type.STR, Combine.APPEND),
-        Option.IB111_WEEK: OptionParse(Option.IB111_WEEK, "", TakesVal.YES, None, Type.INT, Combine.REPLACE)
+        Option.IB111_WEEK: OptionParse(Option.IB111_WEEK, "", TakesVal.YES, None, Type.INT, Combine.REPLACE),
+        Option.CONFIG: OptionParse(Option.CONFIG, "", TakesVal.YES, DEFAULT_CONFIG, Type.STR, Combine.REPLACE)
     }
 
 
 @pytest.mark.parametrize("raw,parsed", [
-    (["python-specific"], [UnprocessedArg(Option.PYTHON_SPECIFIC, None)]),
-    (["python-spec"], [UnprocessedArg(Option.PYTHON_SPECIFIC, None)]),
-    (["flake8=foo"], [UnprocessedArg(Option.FLAKE8, "foo")]),
-    (["flake8="], [UnprocessedArg(Option.FLAKE8, "")]),
-    (["python-specific", "flake8=foo"], [
-        UnprocessedArg(Option.PYTHON_SPECIFIC, None), UnprocessedArg(Option.FLAKE8, "foo")
-    ]),
-    (["flake8=--enable=xxx"], [UnprocessedArg(Option.FLAKE8, "--enable=xxx")]),
-    (["ib111-week=02"], [UnprocessedArg(Option.IB111_WEEK, "02")]),
-    (["ib111-week=12", "ib111-week=02"], [
-        UnprocessedArg(Option.IB111_WEEK, "12"), UnprocessedArg(Option.IB111_WEEK, "02")
-    ]),
+    (["python-specific"], ("default", [UnprocessedArg(Option.PYTHON_SPECIFIC, None)])),
+    (["python-spec"], ("default", [UnprocessedArg(Option.PYTHON_SPECIFIC, None)])),
+    (["flake8=foo"], ("default", [UnprocessedArg(Option.FLAKE8, "foo")])),
+    (["flake8="], ("default", [UnprocessedArg(Option.FLAKE8, "")])),
+    (["python-specific", "flake8=foo"], ("default", [
+       UnprocessedArg(Option.PYTHON_SPECIFIC, None), UnprocessedArg(Option.FLAKE8, "foo")
+    ])),
+    (["flake8=--enable=xxx"], ("default", [UnprocessedArg(Option.FLAKE8, "--enable=xxx")])),
+    (["ib111-week=02"], ("default", [UnprocessedArg(Option.IB111_WEEK, "02")])),
+    (["ib111-week=12", "ib111-week=02"], ("default", [
+       UnprocessedArg(Option.IB111_WEEK, "12"), UnprocessedArg(Option.IB111_WEEK, "02")
+    ])),
+    (["config=empty"], ("empty", [UnprocessedArg(Option.CONFIG, "empty")]))
 ])
 def test_parse_args(raw: List[str], options: Dict[Option, OptionParse], parsed: List[UnprocessedArg]) -> None:
     assert parse_args(raw, options) == parsed
 
 
+def packaged_config_files():
+    packaged_config_dir = Path(__file__).parent / ".." / "edulint" / "config" / "files"
+    return [c.stem for c in packaged_config_dir.iterdir() if c.suffix == ".toml"]
+
+
+@pytest.mark.parametrize("config_name", packaged_config_files())
+def test_packaged_configs_parse(config_name: str):
+    option_parses = get_option_parses()
+    print(config_name)
+    assert parse_config_file(config_name, option_parses) is not None
+
+
 @pytest.fixture
 def config_translations() -> Dict[Option, Translation]:
     return {
         Option.ENHANCEMENT: Translation(
             Linter.PYLINT,
             ["aaa"]
         ),
```

### Comparing `edulint-2.6.4/tests/test_improper_loop.py` & `edulint-2.7.1/tests/test_improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.4/tests/test_lint.py` & `edulint-2.7.1/tests/test_lint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 import pytest
 from edulint.linters import Linter
 from edulint.options import Option
 from edulint.config.arg import Arg
-from edulint.config.config import Config
 from edulint.linting.problem import Problem
-from edulint.linting.linting import lint_one
-from utils import lazy_problem, lazy_equal, get_tests_path, apply_and_lint, create_apply_and_lint
+from utils import lazy_problem, apply_and_lint, create_apply_and_lint
 from typing import List
 
 
-@pytest.mark.parametrize("filename,config,expected_output", [
-    ("hello_world.py", Config(), []),
-    ("z202817-zkouska.py", Config(), [
+@pytest.mark.parametrize("filename,args,expected_output", [
+    ("hello_world.py", [], []),
+    ("z202817-zkouska.py", [], [
         lazy_problem().set_code("R6609").set_line(10),
         lazy_problem().set_code("R6303").set_line(42),
         lazy_problem().set_code("R6205").set_line(82),
         lazy_problem().set_code("R6101").set_line(171),
         lazy_problem().set_code("W0107").set_line(196)
     ]),
-    ("z202817-zkouska.py", Config([Arg(Option.PYLINT, ["--enable=C0115"])]), [
+    ("z202817-zkouska.py", [Arg(Option.PYLINT, "--enable=C0115")], [
         lazy_problem().set_code("R6609").set_line(10),
         lazy_problem().set_code("R6303").set_line(42),
         lazy_problem().set_code("R6205").set_line(82),
         lazy_problem().set_code("C0115").set_line(122),
         lazy_problem().set_code("C0115").set_line(128),
         lazy_problem().set_code("R6101").set_line(171),
         lazy_problem().set_code("W0107").set_line(196)
     ]),
-    ("z202817-zkouska.py", Config([Arg(Option.PYLINT, ["--enable=C0115", "--disable=W0107,R6609"])]), [
+    ("z202817-zkouska.py", [Arg(Option.PYLINT, "--enable=C0115"), Arg(Option.PYLINT, "--disable=W0107,R6609")], [
         lazy_problem().set_code("R6303").set_line(42),
         lazy_problem().set_code("R6205").set_line(82),
         lazy_problem().set_code("C0115").set_line(122),
         lazy_problem().set_code("C0115").set_line(128),
         lazy_problem().set_code("R6101").set_line(171),
     ]),
-    ("z202817-zkouska.py",
-     Config([Arg(Option.PYLINT, ["--disable=all"])]), []),
-    ("002814-p1_trapezoid.py", Config(), [
+    ("z202817-zkouska.py", [Arg(Option.PYLINT, "--disable=all")], []),
+    ("002814-p1_trapezoid.py", [], [
         lazy_problem().set_code("F401").set_line(1),
         lazy_problem().set_code("F401").set_line(1),
         lazy_problem().set_code("E501").set_line(1),
         lazy_problem().set_code("W293").set_line(19),
         lazy_problem().set_code("E303").set_line(22),
     ])
 ])
-def test_lint_basic(filename: str, config: Config, expected_output: List[Problem]) -> None:
-    lazy_equal(lint_one(get_tests_path(filename), config), expected_output)
+def test_lint_basic(filename: str, args: List[Arg], expected_output: List[Problem]) -> None:
+    apply_and_lint(filename, args, expected_output)
 
 
 @pytest.mark.parametrize("filename,args,expected_output", [
     ("z202817-zkouska.py", [Arg(Option.ENHANCEMENT, "on")], [
         lazy_problem().set_code("R6609").set_line(10),
         lazy_problem().set_code("R6303").set_line(42),
         lazy_problem().set_code("R6208").set_line(76),
@@ -474,14 +471,42 @@
         apply_and_lint(
             filename,
             [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=no-global-variables")],
             expected_output
         )
 
 
+class TestLongCode:
+    @pytest.mark.parametrize("filename,expected_output", [
+        ("hw48505.py", [
+            lazy_problem().set_line(80),
+            lazy_problem().set_line(196),
+        ]),
+    ])
+    def test_long_function_files(self, filename: str, expected_output: List[Problem]) -> None:
+        apply_and_lint(
+            filename,
+            [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=long-function")],
+            expected_output
+        )
+
+    @pytest.mark.parametrize("filename,expected_output", [
+        ("014422-next.py", [
+            lazy_problem().set_line(19)
+        ]),
+        ("023240-cards.py", []),
+    ])
+    def test_use_early_return(self, filename: str, expected_output: List[Problem]) -> None:
+        apply_and_lint(
+            filename,
+            [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=use-early-return")],
+            expected_output
+        )
+
+
 @pytest.mark.parametrize("filename,args,expected_output", [
     ("umime_count_a.py", [
         Arg(Option.PYTHON_SPECIFIC, "on"),
         Arg(Option.ALLOWED_ONECHAR_NAMES, ""),
         Arg(Option.ENHANCEMENT, "on"),
     ], [
         lazy_problem().set_code("C0104").set_line(2)
```

### Comparing `edulint-2.6.4/tests/test_main.py` & `edulint-2.7.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.4/tests/test_short_problems.py` & `edulint-2.7.1/tests/test_short_problems.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,14 +297,15 @@
         ]),
         ("m5435.py", [
             lazy_problem().set_code("R6609").set_line(7),
             lazy_problem().set_code("R6605").set_line(9).set_text("Use elif."),
             lazy_problem().set_code("R6608").set_line(53).set_text("Redundant arithmetic: valid += 0"),
             lazy_problem().set_code("R6608").set_line(64).set_text("Redundant arithmetic: valid += 0"),
         ]),
+        ("ut_157_0762_16_47.py", []),
     ])
     def test_short_files(self, filename: str, expected_output: List[Problem]) -> None:
         apply_and_lint(
             filename,
             [
                 Arg(Option.NO_FLAKE8, "on"),
                 Arg(Option.PYLINT, "--disable=all"),
```

### Comparing `edulint-2.6.4/tests/test_simplifiable_if.py` & `edulint-2.7.1/tests/test_simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.4/tests/test_visitors.py` & `edulint-2.7.1/tests/test_visitors.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     x = 1
     for y in range(11):
         x = 1
     x += 1""", 4, [astns.For, astns.Assign, astns.For, astns.Assign], [astns.AugAssign]),
 ])
 def test_split_n_lines(program: str, init_lines: int, before_types: List[type], after_types: List[type]):
     module = astroid.parse(program)
-    print(module)
     before, after = split_n_lines(module.body, init_lines)
 
     def compare(nodes: List[astns.NodeNG], node_types: List[type]):
         assert len(nodes) == len(node_types)
 
         for node, node_type in zip(nodes, node_types):
             assert isinstance(node, node_type)
```

