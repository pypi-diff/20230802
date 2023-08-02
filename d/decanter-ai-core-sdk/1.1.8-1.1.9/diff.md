# Comparing `tmp/decanter-ai-core-sdk-1.1.8.tar.gz` & `tmp/decanter-ai-core-sdk-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/decanter-ai-core-sdk-1.1.8.tar", last modified: Mon Jan  3 06:50:07 2022, max compression
+gzip compressed data, was "dist/decanter-ai-core-sdk-1.1.9.tar", last modified: Mon Mar  7 02:53:23 2022, max compression
```

## Comparing `decanter-ai-core-sdk-1.1.8.tar` & `decanter-ai-core-sdk-1.1.9.tar`

### file list

```diff
@@ -1,48 +1,109 @@
-drwxrwxr-x   0 schwannden  (1000) schwannden  (1000)        0 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     6103 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/PKG-INFO
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     4808 2022-01-03 06:40:57.000000 decanter-ai-core-sdk-1.1.8/README.md
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)       38 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/setup.cfg
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     1152 2022-01-03 06:49:42.000000 decanter-ai-core-sdk-1.1.8/setup.py
-drwxrwxr-x   0 schwannden  (1000) schwannden  (1000)        0 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/
-drwxrwxr-x   0 schwannden  (1000) schwannden  (1000)        0 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/decanter/
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)        0 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/__init__.py
-drwxrwxr-x   0 schwannden  (1000) schwannden  (1000)        0 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     1037 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/__init__.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)    11184 2022-01-03 06:40:57.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/client.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     7123 2022-01-03 06:40:57.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/context.py
-drwxrwxr-x   0 schwannden  (1000) schwannden  (1000)        0 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)      313 2022-01-03 06:40:57.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/__init__.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)    11088 2022-01-03 06:40:57.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/api.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     7575 2022-01-03 06:40:57.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/body_obj.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     6943 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/model.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     4860 2021-07-12 15:44:12.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/predict_input.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     1829 2021-07-14 02:18:09.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/setup_input.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)    13150 2022-01-03 06:40:57.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/train_input.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)      571 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/worker.py
-drwxrwxr-x   0 schwannden  (1000) schwannden  (1000)        0 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/enums/
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)      704 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/enums/__init__.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     1539 2022-01-03 06:40:57.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/enums/algorithms.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)      162 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/enums/categorical_group_by_method.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     1754 2022-01-03 06:40:57.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/enums/evaluators.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)      154 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/enums/numerical_group_by_methods.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)      177 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/enums/time_units.py
-drwxrwxr-x   0 schwannden  (1000) schwannden  (1000)        0 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/extra/
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)       65 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/extra/__init__.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)      568 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/extra/const.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     2178 2021-07-12 15:13:00.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/extra/decorators.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     1759 2021-07-12 14:31:06.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/extra/utils.py
-drwxrwxr-x   0 schwannden  (1000) schwannden  (1000)        0 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)      242 2022-01-03 06:40:57.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/__init__.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     4272 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/data_setup.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     4286 2021-07-14 02:29:24.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/data_upload.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)    12054 2022-01-03 06:40:57.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/experiment.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     6270 2021-07-12 14:52:41.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/job.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     5110 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/predict_result.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)    10989 2022-01-03 06:40:57.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/task.py
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     3419 2021-06-30 04:08:18.000000 decanter-ai-core-sdk-1.1.8/src/decanter/core/plot.py
-drwxrwxr-x   0 schwannden  (1000) schwannden  (1000)        0 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/decanter_ai_core_sdk.egg-info/
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     6103 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/decanter_ai_core_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)     1356 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/decanter_ai_core_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)        1 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/decanter_ai_core_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)      156 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/decanter_ai_core_sdk.egg-info/requires.txt
--rw-rw-r--   0 schwannden  (1000) schwannden  (1000)        9 2022-01-03 06:50:07.000000 decanter-ai-core-sdk-1.1.8/src/decanter_ai_core_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.851120 decanter-ai-core-sdk-1.1.9/
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.823120 decanter-ai-core-sdk-1.1.9/.github/
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.827120 decanter-ai-core-sdk-1.1.9/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      674 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      604 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.827120 decanter-ai-core-sdk-1.1.9/.github/linters/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)       37 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/.github/linters/.isort.cfg
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.827120 decanter-ai-core-sdk-1.1.9/.github/workflows/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      676 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/.github/workflows/doc.yml
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     1437 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/.github/workflows/linter.yml
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     2056 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/.gitignore
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      440 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/.pylintrc
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     1395 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/LICENSE
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     1253 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/Makefile
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     6103 2022-03-07 02:53:23.851120 decanter-ai-core-sdk-1.1.9/PKG-INFO
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     4808 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/README.md
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.827120 decanter-ai-core-sdk-1.1.9/docs/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      705 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/Makefile
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.827120 decanter-ai-core-sdk-1.1.9/docs/source/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     2281 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/api.rst
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     2402 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/conf.py
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.831120 decanter-ai-core-sdk-1.1.9/docs/source/images/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    77814 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/images/flow_1.png
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)   113796 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/images/flow_2.png
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)   123021 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/images/flow_3.png
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    98031 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/images/flow_4.png
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    79661 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/images/flow_5.png
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    60950 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/images/flow_6.png
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    68265 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/images/jupyter.png
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     1257 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/index.rst
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.831120 decanter-ai-core-sdk-1.1.9/docs/source/notes/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)       60 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/notes/changelog.rst
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     4767 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/notes/contributing.rst
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     6553 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/docs/source/notes/design.rst
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     2955 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/docs/source/notes/example.rst
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.835120 decanter-ai-core-sdk-1.1.9/docs/source/user/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     2369 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/user/install.rst
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     1788 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/user/intro.rst
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     2137 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/docs/source/user/quickstart.rst
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.835120 decanter-ai-core-sdk-1.1.9/examples/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)        0 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/examples/__init__.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     2901 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/examples/auto_time_series_example.py
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.835120 decanter-ai-core-sdk-1.1.9/examples/data/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    12228 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/examples/data/test.csv
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    49047 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/examples/data/train.csv
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.835120 decanter-ai-core-sdk-1.1.9/examples/data/ts_data/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      623 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/examples/data/ts_data/iris_test.csv
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    26910 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/examples/data/ts_data/iris_train.csv
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     2788 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/examples/example.py
+-rwxrwxr-x   0 bagel     (1000) bagel     (1000)    56466 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/examples/jupyter_example.ipynb
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     8331 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/examples/jupyter_jobs_handle_example.ipynb
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      176 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/pytest.ini
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)       38 2022-03-07 02:53:23.851120 decanter-ai-core-sdk-1.1.9/setup.cfg
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     1152 2022-03-07 02:52:11.000000 decanter-ai-core-sdk-1.1.9/setup.py
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.839120 decanter-ai-core-sdk-1.1.9/src/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)        0 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/__init__.py
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.839120 decanter-ai-core-sdk-1.1.9/src/decanter/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)        0 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/__init__.py
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.839120 decanter-ai-core-sdk-1.1.9/src/decanter/core/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     1037 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/__init__.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    11184 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/client.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     7123 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/context.py
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.839120 decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      313 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/__init__.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    11088 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/api.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     7575 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/body_obj.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     6943 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/model.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     4860 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/predict_input.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     1829 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/setup_input.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    13150 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/train_input.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      571 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/worker.py
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.843120 decanter-ai-core-sdk-1.1.9/src/decanter/core/enums/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      704 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/enums/__init__.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     1565 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/enums/algorithms.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      162 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/enums/categorical_group_by_method.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     1754 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/enums/evaluators.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      154 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/enums/numerical_group_by_methods.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      177 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/enums/time_units.py
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.843120 decanter-ai-core-sdk-1.1.9/src/decanter/core/extra/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)       65 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/extra/__init__.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      568 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/extra/const.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     2178 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/extra/decorators.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     1759 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/extra/utils.py
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.847120 decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      242 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/__init__.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     4272 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/data_setup.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     4286 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/data_upload.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    12054 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/experiment.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     6270 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/job.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     5110 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/predict_result.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    10989 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/task.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     3419 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/src/decanter/core/plot.py
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.847120 decanter-ai-core-sdk-1.1.9/src/decanter_ai_core_sdk.egg-info/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     6103 2022-03-07 02:53:23.000000 decanter-ai-core-sdk-1.1.9/src/decanter_ai_core_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     2534 2022-03-07 02:53:23.000000 decanter-ai-core-sdk-1.1.9/src/decanter_ai_core_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)        1 2022-03-07 02:53:23.000000 decanter-ai-core-sdk-1.1.9/src/decanter_ai_core_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      156 2022-03-07 02:53:23.000000 decanter-ai-core-sdk-1.1.9/src/decanter_ai_core_sdk.egg-info/requires.txt
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)        9 2022-03-07 02:53:23.000000 decanter-ai-core-sdk-1.1.9/src/decanter_ai_core_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.851120 decanter-ai-core-sdk-1.1.9/tests/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)        0 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/tests/__init__.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     5683 2022-03-07 02:51:07.000000 decanter-ai-core-sdk-1.1.9/tests/conftest.py
+drwxrwxr-x   0 bagel     (1000) bagel     (1000)        0 2022-03-07 02:53:23.851120 decanter-ai-core-sdk-1.1.9/tests/data/
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)    12228 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/tests/data/test.csv
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)       28 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/tests/data/test.txt
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     5272 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/tests/test_context.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     3393 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/tests/test_data.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     6500 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/tests/test_experiment.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)     6097 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/tests/test_predict_result.py
+-rw-rw-r--   0 bagel     (1000) bagel     (1000)      430 2021-04-29 07:52:15.000000 decanter-ai-core-sdk-1.1.9/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `decanter-ai-core-sdk-1.1.8/PKG-INFO` & `decanter-ai-core-sdk-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decanter-ai-core-sdk
-Version: 1.1.8
+Version: 1.1.9
 Summary: Decanter AI Core SDK for the easy use of Decanter Core API.
 Home-page: https://github.com/MoBagel/decanter-ai-core-sdk
 Author: Mobagel
 Author-email: us@mobagel.com
 License: MIT
 Description: # MoBagel Decanter AI Core SDK
```

### Comparing `decanter-ai-core-sdk-1.1.8/README.md` & `decanter-ai-core-sdk-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/setup.py` & `decanter-ai-core-sdk-1.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     'pylint-quotes'
 ]
 
 setuptools.setup(
     name='decanter-ai-core-sdk',
     author='Mobagel',
     author_email='us@mobagel.com',
-    version='1.1.8',
+    version='1.1.9',
     license='MIT',
     description='Decanter AI Core SDK for the easy use of Decanter Core API.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/MoBagel/decanter-ai-core-sdk',
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/__init__.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/__init__.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/client.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/client.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/context.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/context.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/api.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/api.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/body_obj.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/body_obj.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/model.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/model.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/predict_input.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/predict_input.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/setup_input.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/setup_input.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/train_input.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/train_input.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/core_api/worker.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/core_api/worker.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/enums/__init__.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/enums/algorithms.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/enums/algorithms.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,7 +38,8 @@
     StackedEnsemble = 'StackedEnsemble'
     XGBoost = 'XGBoost'
     arima = 'arima'
     prophet = 'prophet'
     ets = 'ets'
     theta = 'theta'
     tpot = 'tpot'
+    lgbm_gpu = 'lgbm_gpu'
```

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/enums/evaluators.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/enums/evaluators.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/extra/const.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/extra/const.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/extra/decorators.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/extra/decorators.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/extra/utils.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/extra/utils.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/data_setup.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/data_setup.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/data_upload.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/data_upload.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/experiment.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/experiment.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/job.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/job.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/predict_result.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/predict_result.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/jobs/task.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/jobs/task.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter/core/plot.py` & `decanter-ai-core-sdk-1.1.9/src/decanter/core/plot.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-core-sdk-1.1.8/src/decanter_ai_core_sdk.egg-info/PKG-INFO` & `decanter-ai-core-sdk-1.1.9/src/decanter_ai_core_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decanter-ai-core-sdk
-Version: 1.1.8
+Version: 1.1.9
 Summary: Decanter AI Core SDK for the easy use of Decanter Core API.
 Home-page: https://github.com/MoBagel/decanter-ai-core-sdk
 Author: Mobagel
 Author-email: us@mobagel.com
 License: MIT
 Description: # MoBagel Decanter AI Core SDK
```

