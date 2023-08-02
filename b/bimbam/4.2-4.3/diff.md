# Comparing `tmp/bimbam-4.2.tar.gz` & `tmp/bimbam-4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimbam-4.2.tar", last modified: Mon Jul 31 22:27:43 2023, max compression
+gzip compressed data, was "bimbam-4.3.tar", last modified: Wed Aug  2 20:39:08 2023, max compression
```

## Comparing `bimbam-4.2.tar` & `bimbam-4.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.789517 bimbam-4.2/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-31 22:27:43.789517 bimbam-4.2/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.773517 bimbam-4.2/bimbam.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-31 22:27:43.000000 bimbam-4.2/bimbam.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-07-31 22:27:43.000000 bimbam-4.2/bimbam.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-31 22:27:43.000000 bimbam-4.2/bimbam.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-31 22:27:43.000000 bimbam-4.2/bimbam.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-31 22:27:43.000000 bimbam-4.2/bimbam.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-07-31 22:27:43.789517 bimbam-4.2/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1961 2023-07-31 22:27:33.000000 bimbam-4.2/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.777517 bimbam-4.2/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1805 2023-07-31 21:50:25.000000 bimbam-4.2/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.777517 bimbam-4.2/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17227 2023-07-31 21:56:01.000000 bimbam-4.2/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-4.2/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-4.2/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-4.2/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-4.2/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.781517 bimbam-4.2/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-4.2/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-4.2/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-4.2/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.781517 bimbam-4.2/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.781517 bimbam-4.2/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-4.2/thonnycontrib/docs/res/exception_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-4.2/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/failed_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-4.2/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/success_green_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.785517 bimbam-4.2/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-4.2/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16157 2023-07-31 21:17:00.000000 bimbam-4.2/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-4.2/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-4.2/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3712 2023-07-27 21:16:38.000000 bimbam-4.2/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.785517 bimbam-4.2/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-4.2/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.785517 bimbam-4.2/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-4.2/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-4.2/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-4.2/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-4.2/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23062 2023-07-31 22:27:12.000000 bimbam-4.2/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41365 2023-07-31 19:30:41.000000 bimbam-4.2/thonnycontrib/l1test_frontend/l1test_treeview.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.785517 bimbam-4.2/thonnycontrib/main_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-4.2/thonnycontrib/main_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5301 2023-07-28 14:35:18.000000 bimbam-4.2/thonnycontrib/main_generator/main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5453 2023-07-30 12:38:45.000000 bimbam-4.2/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-4.2/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.789517 bimbam-4.2/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/tests/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.789517 bimbam-4.2/thonnycontrib/tests/fixtures/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-4.2/thonnycontrib/tests/fixtures/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/tests/fixtures/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-4.2/thonnycontrib/tests/fixtures/workbench_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2505 2023-07-30 12:46:52.000000 bimbam-4.2/thonnycontrib/tests/tests_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-4.2/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-4.2/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-4.2/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-4.2/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-4.2/thonnycontrib/tests/tests_main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-4.2/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-4.2/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17914 2023-07-30 12:41:56.000000 bimbam-4.2/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.908606 bimbam-4.3/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-02 20:39:08.904606 bimbam-4.3/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.892605 bimbam-4.3/bimbam.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-02 20:39:08.000000 bimbam-4.3/bimbam.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-08-02 20:39:08.000000 bimbam-4.3/bimbam.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-08-02 20:39:08.000000 bimbam-4.3/bimbam.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-02 20:39:08.000000 bimbam-4.3/bimbam.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-02 20:39:08.000000 bimbam-4.3/bimbam.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-08-02 20:39:08.908606 bimbam-4.3/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1961 2023-08-02 20:38:47.000000 bimbam-4.3/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.896606 bimbam-4.3/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1741 2023-08-01 23:02:20.000000 bimbam-4.3/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.896606 bimbam-4.3/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17236 2023-08-01 23:42:41.000000 bimbam-4.3/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-4.3/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-4.3/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-4.3/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-4.3/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.896606 bimbam-4.3/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-4.3/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-4.3/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-4.3/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.896606 bimbam-4.3/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.900606 bimbam-4.3/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-4.3/thonnycontrib/docs/res/exception_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-4.3/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/docs/res/failed_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-4.3/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2144 2023-08-01 23:56:58.000000 bimbam-4.3/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/docs/res/success_green_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.900606 bimbam-4.3/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-4.3/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16176 2023-08-01 23:32:20.000000 bimbam-4.3/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-4.3/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-4.3/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3376 2023-08-02 00:12:04.000000 bimbam-4.3/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.900606 bimbam-4.3/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-4.3/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.904606 bimbam-4.3/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-4.3/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-4.3/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-4.3/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-4.3/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23055 2023-08-02 00:09:49.000000 bimbam-4.3/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41636 2023-08-01 23:49:06.000000 bimbam-4.3/thonnycontrib/l1test_frontend/l1test_treeview.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.904606 bimbam-4.3/thonnycontrib/main_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-4.3/thonnycontrib/main_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5301 2023-07-28 14:35:18.000000 bimbam-4.3/thonnycontrib/main_generator/main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5453 2023-07-30 12:38:45.000000 bimbam-4.3/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-4.3/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.904606 bimbam-4.3/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/tests/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 20:39:08.904606 bimbam-4.3/thonnycontrib/tests/fixtures/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-4.3/thonnycontrib/tests/fixtures/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-4.3/thonnycontrib/tests/fixtures/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-4.3/thonnycontrib/tests/fixtures/workbench_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2505 2023-07-30 12:46:52.000000 bimbam-4.3/thonnycontrib/tests/tests_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-4.3/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-4.3/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-4.3/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-4.3/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-4.3/thonnycontrib/tests/tests_main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-4.3/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-4.3/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17858 2023-08-01 23:47:43.000000 bimbam-4.3/thonnycontrib/utils.py
```

### Comparing `bimbam-4.2/PKG-INFO` & `bimbam-4.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 4.2
+Version: 4.3
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-4.2/bimbam.egg-info/PKG-INFO` & `bimbam-4.3/bimbam.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 4.2
+Version: 4.3
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-4.2/bimbam.egg-info/SOURCES.txt` & `bimbam-4.3/bimbam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/setup.py` & `bimbam-4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="bimbam",
-    version="4.2",
+    version="4.3",
     author="idtaleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests""",
     url="https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `bimbam-4.2/thonnycontrib/ThonnyLogsGenerator.py` & `bimbam-4.3/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 #Attention si le nom change ici, il faut aussi le changer dans Thonny-LoggingPlugin
 NOM_EVENT_TEST = "l1Tests"
 NOM_EVENT_DOC = "l1Tests.DocGenerator"
 wb = get_workbench() 
 
 # Modifié par Mathieu Bachelet, PJI 2022-2023, mais sur la V2 de L1test
 # Modifié par Mirabelle pour adaptation à la V3 de L1test
-def log_in_thonny(test_results: List[L1DocTest], selected):
-    filename = test_results[0].get_filename() if test_results != [] else None
+def log_in_thonny(test_results: List[L1DocTest], filename:str, selected):
     tests_data = []
     for l1doctest in test_results:
         for example in l1doctest.get_examples():
             # test:Example
             verdict = example.get_verdict() # type ExampleVerdict
             res = vars(verdict).copy() # pour récupérer les attributs filename, lineno, tested_line, expected_results, details
             res['details'] = str(res['details']) # sinon on peut récupérer un entier
```

### Comparing `bimbam-4.2/thonnycontrib/backend/ast_parser.py` & `bimbam-4.3/thonnycontrib/backend/ast_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if value == -1:
             return L1DocTestFlag.FAILED_FLAG
         elif value == 0:
             return L1DocTestFlag.EMPTY_FLAG
         else:
             return L1DocTestFlag.PASSED_FLAG
     
-    def get_image(self):
+    def get_image_basename(self):
         """This method returns the icon corresponding to the flag."""
         if self.value == -1:
             return "failed.png"
         elif self.value == 0:
             return "warning.png"
         else:
             return "passed.png"
```

### Comparing `bimbam-4.2/thonnycontrib/backend/doctest_parser.py` & `bimbam-4.3/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/backend/evaluator.py` & `bimbam-4.3/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/backend/l1test_backend.py` & `bimbam-4.3/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/backend/test_finder.py` & `bimbam-4.3/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `bimbam-4.3/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/backend/verdicts/FailedVerdict.py` & `bimbam-4.3/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `bimbam-4.3/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docs/res/error_icon.png` & `bimbam-4.3/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docs/res/exception_red_chip.png` & `bimbam-4.3/thonnycontrib/docs/res/exception_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docs/res/failed.png` & `bimbam-4.3/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docs/res/failed_red_chip.png` & `bimbam-4.3/thonnycontrib/docs/res/failed_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docs/res/l1test_icon.png` & `bimbam-4.3/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docs/res/l1test_icon_old.png` & `bimbam-4.3/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docs/res/outline_class.png` & `bimbam-4.3/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docs/res/outline_method.gif` & `bimbam-4.3/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docs/res/passed.png` & `bimbam-4.3/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docs/res/restart_icon.png` & `bimbam-4.3/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docs/res/success_green_chip.png` & `bimbam-4.3/thonnycontrib/docs/res/success_green_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docs/res/warning.png` & `bimbam-4.3/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docstring_generator/__init__.py` & `bimbam-4.3/thonnycontrib/docstring_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/docstring_generator/doc_generator.py` & `bimbam-4.3/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,15 @@
                 
                 self.set_has_exception(False) # success
     
     def _show_treeview(self):
         """
         Cleans the ErrorView and hides it. Retreives the Treeview and shows it.
         """
-        get_l1test_runner().show_treeview()
+        get_l1test_runner().hide_errorview_and_show_treeview()
     
     def _show_error(self, error_msg:str, error_title:str=CANNOT_GENERATE_THE_DOCSTRING):
         """
         Shows the error in the ErrorView if the docstring generator raises an exception.
         """
         l1test_runner = get_l1test_runner()
         if self.has_exception():
```

### Comparing `bimbam-4.2/thonnycontrib/docstring_generator/doc_template.py` & `bimbam-4.3/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/environement_vars.py` & `bimbam-4.3/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/exceptions.py` & `bimbam-4.3/thonnycontrib/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,16 +105,8 @@
 
 class DocGeneratorParserException(FrontendException):
     """
     Exception raised when no docstring cannot be generated by the generator.
     This exception is raised when a function signature contains a compilation
     error.
     """
-    pass
-
-class CannotSelectSeveralLines(FrontendException):
-    """
-    Exception raised when several lines are selected. For example, This exception 
-    is raised when the user tries to select several lines to run the tests of the selected
-    lines. Or, when a user tries to select several lines to generate the docstring.
-    """
-    pass
+    pass
```

### Comparing `bimbam-4.2/thonnycontrib/l1test_configuration/l1test_options.py` & `bimbam-4.3/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/l1test_frontend/__init__.py` & `bimbam-4.3/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/l1test_frontend/l1test_error_view.py` & `bimbam-4.3/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/l1test_frontend/l1test_outliner_menu.py` & `bimbam-4.3/thonnycontrib/l1test_frontend/l1test_outliner_menu.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/l1test_frontend/l1test_reporter.py` & `bimbam-4.3/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/l1test_frontend/l1test_runner.py` & `bimbam-4.3/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         
         self._reporter = L1TestReporter() if not reporter else reporter
         self._has_exception = False
         self._is_l1test_running = False
         self._is_pending = False
         self._has_reported_exception = False # indique si une ligne d'erreur de la tree a été clique et que l'exception
                                             # a été reporté sur la ErrorView
-        
+        self._filename = "<module>"
         # Quand le backend envoie une réponse de type `ToplevelResponse``,
         # alors le TestRunner va invoquer la fonction `show_verdicts`
         thonny.get_workbench().bind("ToplevelResponse", self._handle_backend_response, True)
         
         # Quand le backend envoie une réponse de type `InlineResponse``,
         # alors le TestRunner va invoquer la fonction `show_execution_state`
         thonny.get_workbench().bind("InlineResponse", self._handle_execution_state, True)
@@ -79,22 +79,24 @@
             # si aucun editeur n'est ouvert sur le workbench
             if not editor.get_current_editor():
                 raise NoEditorFoundException("No editor found !\n\nPlease open an editor before running the tests.")
             
             # cette ligne demande de sauver le fichier s'il n'a pas encore été sauvé sur
             # la machine. Si le fichier est déjà sauvé, il va permettre d'enregistrer la nouvelle
             # version du fichier.
-            filename = editors.get_saved_current_script_filename(force=True)
-            
+            filename = editors.get_saved_current_script_filename(force=True)          
+
             # si le filename est null alors le fichier n'a  pas été sauvé sur machine.  
             # Ce cas survient quand l'utilisatur quitte la fenetre de sauvegarde sans sauver le fichier.
             if not filename: 
                 msg = "The file is not saved.\n\nConsider to save the file before running the tests."
                 raise NotSavedFileException(msg)
 
+            self._filename = filename
+            
             if not editor.get_current_editor_content().strip():  # L'éditeur est vide. 
                 # on a pas envie d'envoyer une commande au backend si le fichier est vide.
                 # Dans tous les cas y a rien à tester.
                 raise EmptyEditorException("The editor is empty!\n")
             
             # si on est là alors le fichier est bien sauvegardé et contient quelque chose.
             self.request_backend(selected_line)         
@@ -111,17 +113,14 @@
         backend to be executed by the thonny's runner. 
         2. if the `L1test` is invoked a lot of times (lot of clicks), then we only
         consider the first invocation (first click) of the `L1test` command. While 
         the l1test still running, the other clicks are ignored.
 
         Args:
             selected_line (int): The number of the selected line.
-        Raises:
-            AlreadyRunningException: If the l1test is already running. This is raised 
-            when the user clicks on the `Run` button while the l1test is still running.
         """
         if not self.is_running(): # si l1test n'est est pas déjà en cours d'execution
             try:
                 self.set_is_running()
                 self.__request_backend(selected_line=selected_line)
             except:
                 self.set_is_running(False)
@@ -198,16 +197,15 @@
         Note: The data is deserialized before displaying it on the view.
         """   
        
         # On vérifie si le TopLevelRespone reçu est envoyé par le l1test_backend 
         if self._is_relevant_response(msg):
             verdicts, error_msg = self.__get_verdicts_and_error(msg)
             if not self.has_exception(): 
-                if verdicts:
-                    self.show_treeview(verdicts) 
+                self.set_and_show_verdicts_on_treeview(verdicts) 
             else: 
                 self.clean_treeview()
                 self.show_error_view(error_msg.msg, error_msg.title)
         else:
             # Le TopLevelReponse reçu ne nous intéresse pas.
             return 
         # On indique l'état de l'execution du la commande comme terminée
@@ -234,15 +232,15 @@
             self.clean_treeview()
             received_verdicts = msg.get(VERDICTS)
             if received_verdicts:
                 self.set_has_exception(False)
                 # deserialize the verdicts
                 l1doctests: List[L1DocTest] = pickle.loads(received_verdicts)
                 # log in thonny                    
-                log_in_thonny(l1doctests, os.environ.get(SELECTED_LINE_VAR) != None)
+                log_in_thonny(l1doctests, self._filename, os.environ.get(SELECTED_LINE_VAR) != None)
         return l1doctests, error_msg
     
     def __handle_raised_exception(self, exception: dict) -> ErrorMsg:
         """
         This function handles the raised exception by returning a tuple containing
         a prefix message and the exception message.
 
@@ -336,54 +334,56 @@
             # Si c'est False alors c'est un redémarrage partiel du backend (c'est le cas d'un appel 
             # d'une nouvelle commande).
             if event.get("full"):
                 self.terminate_running()
                 self.clean_treeview(clear_all=True, clear_verdicts_data=True)         
             elif self.is_running(): # si le plugin a été lancé par l'utilisateur
                 self.clean_treeview(clear_all=True, clear_verdicts_data=True) 
-                treeview.insert_in_header("Starting executing tests ...", clear=True, tags="blue", 
+                treeview.insert_in_header("Starting executing tests ...", clear=True, tags="gray", 
                                             image=PENDING_ICON)
             else: # probablement une autre commande a déclenché le Restart du backend -> on fait rien
                 pass
-            self.show_treeview()
+            self.hide_errorview_and_show_treeview()
     
     def _handle_execution_state(self, msg: InlineResponse):
         """
         This function is called when an event of type InlineResponse is received. 
         This function verifies the source of the event. If the source is L1Test so it will access to the 
         received response and then it will handle the state of the execution.
         """
         if self._is_relevant_response(msg):
             state:str = msg.get("state")
             if state == PENDING_STATE:
                 lineno = msg.get("lineno") # la ligne en cours d'execution est récupéré seulement si le state == PENDING_STATE
                 status_msg = L1TEST_IN_PROGRESS + ": line " + str(lineno) 
                 # you can comment the following line if you don't want to show the status message
-                #self._reporter.get_treeview().insert_in_header(status_msg, clear=True, tags="blue", image=PENDING_ICON)
+                self._reporter.get_treeview().insert_in_header(status_msg, clear=True, tags="gray", image=PENDING_ICON)
                 self.set_pending(True)
             else: # si le state == FINISHED_STATE
                 self.set_pending(False) 
     
     def show_error_view(self, error_msg=None, error_title=None, force=False, show_treeview=False):
         if self._has_exception or force:
             self.show_errors(exception_msg=error_msg, title=error_title)
             self._reporter.get_error_view().show_view()   
             if show_treeview:
                 self._reporter.get_treeview().show_view()
             else: 
                 self._reporter.get_treeview().hide_view()
     
-    def show_treeview(self, verdicts:List[L1DocTest]=None):
+    def set_and_show_verdicts_on_treeview(self, verdicts:List[L1DocTest]):
         if not self._has_exception:
-            if verdicts:
-                self.set_and_show_verdicts(verdicts)     
-            self._reporter.get_treeview().show_view()
-            self.clean_error_view()
-            self._reporter.get_error_view().hide_view()
+            self.set_and_show_verdicts(verdicts)     
+            self.hide_errorview_and_show_treeview()
     
+    def hide_errorview_and_show_treeview(self):
+        self._reporter.get_treeview().show_view()
+        self.clean_error_view()
+        self._reporter.get_error_view().hide_view()
+            
     def _handle_clicked_exception(self, event:WorkbenchEvent=None):
         """ 
         This function is called when the user clicks on an exception in the treeview. Then, 
         the error view is displayed with the details of the clicked exception. 
         """
         possible_keys = ["sequence", "error_title", "error_msg", "side_by_side"]
         if event and event.get("sequence") == L1TREE_VIEW_EVENT:
```

### Comparing `bimbam-4.2/thonnycontrib/l1test_frontend/l1test_treeview.py` & `bimbam-4.3/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from functools import partial
 from ..l1test_configuration.l1test_options import *
 import tkinter as tk, tkinter.font as tk_font, thonny
 from collections import namedtuple
 from thonny.codeview import *
 from typing import Dict, List
 from copy import deepcopy
+from tkinter import ttk
 
 # La hauteur, par défault, d'une ligne dans une Treeview
 ROW_HEIGHT = 40
 
 SMALL_MARGIN = 1.1
 NORMAL_MARGIN = 1.17
 
@@ -53,14 +54,15 @@
         ttk.Frame.__init__(self, master, borderwidth=0, relief="flat")
         self.workbench = thonny.get_workbench()
         self._origin_l1doctests: List[L1DocTest] = dict()
         self._copy_l1doctests = self._origin_l1doctests.copy()
         
         self.__init_treeview()
         self.__init_workbench_bindings()
+        self.__init_special_attributes()
     
     def __init_workbench_bindings(self):
         """
         Binds the events to the workbench.
         """
         # Le binding est censé augmenter/diminuer automatiquement la taille de la treeview
         self.workbench.bind("<Control-plus>", self.observe_font_changing, True)
@@ -109,15 +111,15 @@
         # définir un style par défault pour la treeview
         self.style = ttk.Style()
         self.style_mapping = self.style.map('Treeview')
         self.__update_tree_font(get_font_family_option(), get_font_size_option())
 
         # All the icons used in the treeview should be loaded here to keep thier references.
         # Otherwise, they will be garbage collected and the treeview will not show them.
-        self.image_references = {flag.name: get_photoImage(flag.get_image()) for flag in L1DocTestFlag}
+        self.image_references = {flag.get_image_basename(): get_photoImage(flag.get_image_basename()) for flag in L1DocTestFlag}
         self.image_references[PENDING_ICON] = get_photoImage(PENDING_ICON)
         self.image_references[ERROR_ICON] = get_photoImage(ERROR_ICON)
         self.image_references[RESTART_ICON] = get_photoImage(RESTART_ICON)
         self.image_references[FAILED_RED_CHIP] = get_photoImage(FAILED_RED_CHIP)
         self.image_references[EXCEPTION_RED_CHIP] = get_photoImage(EXCEPTION_RED_CHIP)
         self.image_references[SUCCESS_GREEN_CHIP] = get_photoImage(SUCCESS_GREEN_CHIP)
         
@@ -125,16 +127,14 @@
         self.treeview.tag_bind("nonClickable", "<<TreeviewSelect>>", self._remove_highlight_selection_effect)
         self.treeview.bind("<Motion>", self._on_hover_exception_test)
         self.treeview.bind("<Configure>", self.__wrap_tree_content) # Here we handle the motion event of the treeview 
         
         # add a menu to the treeview 
         self.menu = tk.Menu(self.treeview, name="menu", tearoff=False)        
         self.init_header(row=0, column=0)
-
-        self.__init_special_attributes()
         
     def __init_special_attributes(self):
         """
         Initializes the special attributes of the treeview.
         """
         self.__old_width = -1 # utilisé pour savoir si la hauteur de la treeview a changé
         self.__max_lines = 1 # le nombre de lignes du texte le plus long de la treeview
@@ -545,48 +545,53 @@
         self.__old_width = self.workbench.get_view("L1TestTreeView", False).winfo_width() if self.__old_width > 0 else -1
         
         self._restore_row_selection_effect() 
         self.clear_tree(clear_all=clear_header, clear_errorview=clear_errorview)
     
         if not self.__check_if_editor_is_open():
             return
-
+        
+        if not l1doctests:
+            self.insert_in_header("No test found !", image="warning.png", clear=True, tags=("orange",))
+            return
+        
+        self.enable_menu()
         self.__add_verdicts_to_treeview(l1doctests, parent)
         
         # on insère le summarize dans le header bar que si la treeview n'est pas vide
         if not self.is_empty() and clear_header:
             # We build the summarize object 
             summarize: Summarize = self.build_summarize_object(self._origin_l1doctests)
             # We insert the summarize infos into the header bar of the treeview
             self.insert_summarize_in_header_bar(summarize, self.header_bar)
             self.change_header_font() 
         
         self.update_row_height()
             
     def __add_verdicts_to_treeview(self, l1doctests:List[L1DocTest], parent=""):
         o_names = [c_l1doctest.get_name() for c_l1doctest in self._origin_l1doctests]
+        
         for l1doctest in l1doctests:
             o_index = o_names.index(l1doctest.get_name())
             current_node = self._add_node_to_tree(self._origin_l1doctests[o_index], parent)
             if l1doctest.get_flag() == L1DocTestFlag.EMPTY_FLAG:
                 self.treeview.insert(current_node, "end", values=l1doctest.get_node_lineno(), 
                                      text="No tests found", tags=("nonClickable", l1doctest.get_flag().get_color()))
             else:    
                 self._add_verdicts_to_node(current_node, l1doctest.get_examples())
          
         self.__wrap_tree_content()
-        self.enable_menu()
     
     def _add_node_to_tree(self, l1doctest: L1DocTest, parent=""):  
         flag: L1DocTestFlag = l1doctest.get_flag()
         open = get_option(OPEN_ONLY_RED_FUNCTIONS) and not get_option(CLOSE_FUNCTION_ROWS) \
                 if get_option(OPEN_ONLY_RED_FUNCTIONS) and flag.is_failing() \
                 else not get_option(OPEN_ONLY_RED_FUNCTIONS) and not get_option(CLOSE_FUNCTION_ROWS) 
         verdict_config = dict(text=self._get_l1doctest_stats(l1doctest),  
-                              image=self.get_icon(flag.name), 
+                              image=self.get_icon(flag.get_image_basename()), 
                               open=open)
         return self.treeview.insert(parent, "end", values=l1doctest.get_node_lineno(), tags=(CLICKABLE_TAG,), **verdict_config)
     
     def _add_verdicts_to_node(self, current_node:str, examples:list[Example]):
         """ 
         This function adds to the treeview all the rows that correspond 
         to the given ast node.
@@ -811,15 +816,15 @@
         """
         if clear:
             self.header_bar.direct_delete("1.0", tk.END)
         if image:
             if isinstance(image, str):
                 image = self.get_icon(image)
             self.header_bar.image_create(tk.END, image=image)
-            text = " " + text
+            text = " " + text # add a space after the image
         self.header_bar.direct_insert(tk.END, text, tags=tags)
         self.resize_header_bar()
            
     def is_empty(self):
         return len(self.treeview.get_children()) == 0
     
     def is_header_bar_cleared(self): 
@@ -853,8 +858,8 @@
         """
         if ref_name in self.image_references:
             return self.image_references[ref_name]
         return None
     
     def get_max_lines(self):
         """Returns the maximum number of lines of the longest wrapped line of the treeview."""
-        return self.__max_lines
+        return self.__max_lines
```

### Comparing `bimbam-4.2/thonnycontrib/main_generator/main_generator.py` & `bimbam-4.3/thonnycontrib/main_generator/main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/plugin_loader.py` & `bimbam-4.3/thonnycontrib/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/properties.py` & `bimbam-4.3/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/tests/fixtures/workbench_mock.py` & `bimbam-4.3/thonnycontrib/tests/fixtures/workbench_mock.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/tests/tests_doc_generator.py` & `bimbam-4.3/thonnycontrib/tests/tests_doc_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/tests/tests_example_no_expected.py` & `bimbam-4.3/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/tests/tests_example_with_exception.py` & `bimbam-4.3/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/tests/tests_example_with_expected.py` & `bimbam-4.3/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/tests/tests_l1TestRunner.py` & `bimbam-4.3/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/tests/tests_main_generator.py` & `bimbam-4.3/thonnycontrib/tests/tests_main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/tests/tests_test_finder.py` & `bimbam-4.3/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/tests/tests_view.py` & `bimbam-4.3/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.2/thonnycontrib/utils.py` & `bimbam-4.3/thonnycontrib/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from io import StringIO
-from tkinter import Text, ttk
 from types import ModuleType
 from thonny import get_workbench
-from thonnycontrib.exceptions import CannotImportModuleException, CannotSelectSeveralLines, CompilationError
+from thonnycontrib.exceptions import CannotImportModuleException, CompilationError
 from .properties import BACKEND_COMMAND 
 from .environement_vars import *
 import os, re, ast, traceback, textwrap, tkinter as tk
 import thonny
 from thonny.editors import EditorCodeViewText
 
 def wrap(string:str, length=8, break_long_words=False):
```

