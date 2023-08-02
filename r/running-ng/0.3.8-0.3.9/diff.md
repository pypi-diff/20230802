# Comparing `tmp/running-ng-0.3.8.tar.gz` & `tmp/running-ng-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "running-ng-0.3.8.tar", last modified: Mon Feb 20 13:49:53 2023, max compression
+gzip compressed data, was "running-ng-0.3.9.tar", last modified: Wed Aug  2 04:49:45 2023, max compression
```

## Comparing `running-ng-0.3.8.tar` & `running-ng-0.3.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.568555 running-ng-0.3.8/
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.550680 running-ng-0.3.8/.github/
--rw-r--r--   0 caizixian   (501) staff       (20)      106 2021-10-11 12:28:38.000000 running-ng-0.3.8/.github/dependabot.yml
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.551319 running-ng-0.3.8/.github/workflows/
--rw-r--r--   0 caizixian   (501) staff       (20)      470 2022-02-20 06:52:54.000000 running-ng-0.3.8/.github/workflows/mdbook.yml
--rw-r--r--   0 caizixian   (501) staff       (20)     1216 2023-01-16 05:20:12.000000 running-ng-0.3.8/.github/workflows/python.yml
--rw-r--r--   0 caizixian   (501) staff       (20)     1809 2021-10-11 12:28:38.000000 running-ng-0.3.8/.gitignore
--rw-r--r--   0 caizixian   (501) staff       (20)    11357 2022-02-20 06:52:54.000000 running-ng-0.3.8/LICENSE
--rw-r--r--   0 caizixian   (501) staff       (20)     1611 2023-02-20 13:49:53.568355 running-ng-0.3.8/PKG-INFO
--rw-r--r--   0 caizixian   (501) staff       (20)      954 2022-10-12 05:14:15.000000 running-ng-0.3.8/README.md
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.551874 running-ng-0.3.8/docs/
--rw-r--r--   0 caizixian   (501) staff       (20)        5 2021-10-11 12:28:38.000000 running-ng-0.3.8/docs/.gitignore
--rw-r--r--   0 caizixian   (501) staff       (20)      116 2021-10-11 12:28:38.000000 running-ng-0.3.8/docs/book.toml
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.553893 running-ng-0.3.8/docs/src/
--rw-r--r--   0 caizixian   (501) staff       (20)      689 2021-11-06 11:26:31.000000 running-ng-0.3.8/docs/src/SUMMARY.md
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.554399 running-ng-0.3.8/docs/src/basics/
--rw-r--r--   0 caizixian   (501) staff       (20)     1619 2021-11-06 11:26:31.000000 running-ng-0.3.8/docs/src/basics/design.md
--rw-r--r--   0 caizixian   (501) staff       (20)      221 2021-10-11 12:28:38.000000 running-ng-0.3.8/docs/src/basics/index.md
--rw-r--r--   0 caizixian   (501) staff       (20)     7607 2023-02-20 13:48:58.000000 running-ng-0.3.8/docs/src/changelog.md
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.555516 running-ng-0.3.8/docs/src/commands/
--rw-r--r--   0 caizixian   (501) staff       (20)       11 2021-10-11 12:28:38.000000 running-ng-0.3.8/docs/src/commands/fillin.md
--rw-r--r--   0 caizixian   (501) staff       (20)      878 2021-11-06 11:26:31.000000 running-ng-0.3.8/docs/src/commands/index.md
--rw-r--r--   0 caizixian   (501) staff       (20)     2389 2022-02-16 02:25:49.000000 running-ng-0.3.8/docs/src/commands/minheap.md
--rw-r--r--   0 caizixian   (501) staff       (20)     6226 2023-02-14 11:19:25.000000 running-ng-0.3.8/docs/src/commands/runbms.md
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.555992 running-ng-0.3.8/docs/src/cookbook/
--rw-r--r--   0 caizixian   (501) staff       (20)       40 2021-11-06 11:26:31.000000 running-ng-0.3.8/docs/src/cookbook/index.md
--rw-r--r--   0 caizixian   (501) staff       (20)     4464 2021-11-06 11:26:31.000000 running-ng-0.3.8/docs/src/cookbook/perf_events.md
--rw-r--r--   0 caizixian   (501) staff       (20)       29 2021-11-06 11:26:31.000000 running-ng-0.3.8/docs/src/faq.md
--rw-r--r--   0 caizixian   (501) staff       (20)     1429 2022-02-20 07:25:27.000000 running-ng-0.3.8/docs/src/install.md
--rw-r--r--   0 caizixian   (501) staff       (20)     2910 2021-11-06 11:26:31.000000 running-ng-0.3.8/docs/src/intro.md
--rw-r--r--   0 caizixian   (501) staff       (20)     5034 2023-02-14 11:19:25.000000 running-ng-0.3.8/docs/src/quickstart.md
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.557446 running-ng-0.3.8/docs/src/references/
--rw-r--r--   0 caizixian   (501) staff       (20)     5373 2022-09-06 03:25:59.000000 running-ng-0.3.8/docs/src/references/index.md
--rw-r--r--   0 caizixian   (501) staff       (20)     2584 2022-10-12 05:13:38.000000 running-ng-0.3.8/docs/src/references/modifier.md
--rw-r--r--   0 caizixian   (501) staff       (20)      559 2022-02-03 03:09:20.000000 running-ng-0.3.8/docs/src/references/runtime.md
--rw-r--r--   0 caizixian   (501) staff       (20)     7444 2023-02-20 13:48:58.000000 running-ng-0.3.8/docs/src/references/suite.md
--rw-r--r--   0 caizixian   (501) staff       (20)     1156 2023-02-14 11:19:25.000000 running-ng-0.3.8/pyproject.toml
--rw-r--r--   0 caizixian   (501) staff       (20)       38 2023-02-20 13:49:53.568591 running-ng-0.3.8/setup.cfg
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.549629 running-ng-0.3.8/src/
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.560191 running-ng-0.3.8/src/running/
--rw-r--r--   0 caizixian   (501) staff       (20)        0 2022-02-20 06:52:54.000000 running-ng-0.3.8/src/running/__init__.py
--rw-r--r--   0 caizixian   (501) staff       (20)     1581 2022-09-06 03:25:59.000000 running-ng-0.3.8/src/running/__main__.py
--rw-r--r--   0 caizixian   (501) staff       (20)       62 2023-02-20 13:48:58.000000 running-ng-0.3.8/src/running/__version__.py
--rw-r--r--   0 caizixian   (501) staff       (20)    10006 2023-02-20 13:48:58.000000 running-ng-0.3.8/src/running/benchmark.py
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.561740 running-ng-0.3.8/src/running/command/
--rw-r--r--   0 caizixian   (501) staff       (20)        0 2022-02-20 06:52:54.000000 running-ng-0.3.8/src/running/command/__init__.py
--rw-r--r--   0 caizixian   (501) staff       (20)     2048 2022-02-20 06:52:54.000000 running-ng-0.3.8/src/running/command/fillin.py
--rw-r--r--   0 caizixian   (501) staff       (20)     2928 2022-02-20 06:52:54.000000 running-ng-0.3.8/src/running/command/genadvice.py
--rw-r--r--   0 caizixian   (501) staff       (20)     7462 2023-01-16 05:20:12.000000 running-ng-0.3.8/src/running/command/log_preprocessor.py
--rw-r--r--   0 caizixian   (501) staff       (20)     6781 2023-01-16 05:20:12.000000 running-ng-0.3.8/src/running/command/minheap.py
--rw-r--r--   0 caizixian   (501) staff       (20)    15940 2023-01-16 05:20:12.000000 running-ng-0.3.8/src/running/command/runbms.py
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.562255 running-ng-0.3.8/src/running/config/
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.564464 running-ng-0.3.8/src/running/config/base/
--rw-r--r--   0 caizixian   (501) staff       (20)     5346 2023-01-16 04:33:32.000000 running-ng-0.3.8/src/running/config/base/dacapo.yml
--rw-r--r--   0 caizixian   (501) staff       (20)       28 2022-09-06 03:25:59.000000 running-ng-0.3.8/src/running/config/base/jvms.yml
--rw-r--r--   0 caizixian   (501) staff       (20)       95 2022-02-20 06:52:54.000000 running-ng-0.3.8/src/running/config/base/minheap.yml
--rw-r--r--   0 caizixian   (501) staff       (20)     1220 2022-02-20 06:52:54.000000 running-ng-0.3.8/src/running/config/base/modifiers.yml
--rw-r--r--   0 caizixian   (501) staff       (20)      259 2022-02-20 06:52:54.000000 running-ng-0.3.8/src/running/config/base/runbms.yml
--rw-r--r--   0 caizixian   (501) staff       (20)      127 2022-02-20 06:52:54.000000 running-ng-0.3.8/src/running/config/base/specjbb2015.yml
--rw-r--r--   0 caizixian   (501) staff       (20)      132 2022-03-19 05:22:35.000000 running-ng-0.3.8/src/running/config/base/specjvm98.yml
--rw-r--r--   0 caizixian   (501) staff       (20)       75 2022-03-19 05:22:35.000000 running-ng-0.3.8/src/running/config/base/suites.yml
--rw-r--r--   0 caizixian   (501) staff       (20)      283 2022-02-20 06:52:54.000000 running-ng-0.3.8/src/running/config/base/temurin.yml
--rw-r--r--   0 caizixian   (501) staff       (20)      214 2022-09-06 03:25:59.000000 running-ng-0.3.8/src/running/config/minheap_example.yml
--rw-r--r--   0 caizixian   (501) staff       (20)      964 2022-09-06 03:25:59.000000 running-ng-0.3.8/src/running/config/runbms_example.yml
--rw-r--r--   0 caizixian   (501) staff       (20)     5750 2022-09-06 03:25:59.000000 running-ng-0.3.8/src/running/config.py
--rw-r--r--   0 caizixian   (501) staff       (20)     4754 2022-10-12 11:26:16.000000 running-ng-0.3.8/src/running/modifier.py
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.564643 running-ng-0.3.8/src/running/plugin/
--rw-r--r--   0 caizixian   (501) staff       (20)        0 2022-02-20 06:52:54.000000 running-ng-0.3.8/src/running/plugin/__init__.py
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.565352 running-ng-0.3.8/src/running/plugin/runbms/
--rw-r--r--   0 caizixian   (501) staff       (20)     2768 2023-02-20 13:46:54.000000 running-ng-0.3.8/src/running/plugin/runbms/__init__.py
--rw-r--r--   0 caizixian   (501) staff       (20)     3090 2022-02-20 06:52:54.000000 running-ng-0.3.8/src/running/plugin/runbms/copyfile.py
--rw-r--r--   0 caizixian   (501) staff       (20)     5917 2023-01-16 05:20:12.000000 running-ng-0.3.8/src/running/plugin/runbms/zulip.py
--rw-r--r--   0 caizixian   (501) staff       (20)     6049 2022-03-07 03:16:48.000000 running-ng-0.3.8/src/running/runtime.py
--rw-r--r--   0 caizixian   (501) staff       (20)    15630 2023-01-16 05:20:12.000000 running-ng-0.3.8/src/running/suite.py
--rw-r--r--   0 caizixian   (501) staff       (20)     4997 2023-02-14 11:19:25.000000 running-ng-0.3.8/src/running/util.py
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.566256 running-ng-0.3.8/src/running_ng.egg-info/
--rw-r--r--   0 caizixian   (501) staff       (20)     1611 2023-02-20 13:49:53.000000 running-ng-0.3.8/src/running_ng.egg-info/PKG-INFO
--rw-r--r--   0 caizixian   (501) staff       (20)     1955 2023-02-20 13:49:53.000000 running-ng-0.3.8/src/running_ng.egg-info/SOURCES.txt
--rw-r--r--   0 caizixian   (501) staff       (20)        1 2023-02-20 13:49:53.000000 running-ng-0.3.8/src/running_ng.egg-info/dependency_links.txt
--rw-r--r--   0 caizixian   (501) staff       (20)       50 2023-02-20 13:49:53.000000 running-ng-0.3.8/src/running_ng.egg-info/entry_points.txt
--rw-r--r--   0 caizixian   (501) staff       (20)      102 2023-02-20 13:49:53.000000 running-ng-0.3.8/src/running_ng.egg-info/requires.txt
--rw-r--r--   0 caizixian   (501) staff       (20)        8 2023-02-20 13:49:53.000000 running-ng-0.3.8/src/running_ng.egg-info/top_level.txt
-drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-02-20 13:49:53.567929 running-ng-0.3.8/tests/
--rw-r--r--   0 caizixian   (501) staff       (20)     2134 2022-03-07 03:16:48.000000 running-ng-0.3.8/tests/test_config.py
--rw-r--r--   0 caizixian   (501) staff       (20)      682 2021-10-11 12:28:38.000000 running-ng-0.3.8/tests/test_fillin.py
--rw-r--r--   0 caizixian   (501) staff       (20)     1858 2021-10-11 12:28:38.000000 running-ng-0.3.8/tests/test_log_preprocessor.py
--rw-r--r--   0 caizixian   (501) staff       (20)     2737 2022-03-19 05:00:18.000000 running-ng-0.3.8/tests/test_modifier.py
--rw-r--r--   0 caizixian   (501) staff       (20)      469 2021-10-11 12:28:38.000000 running-ng-0.3.8/tests/test_runbms.py
--rw-r--r--   0 caizixian   (501) staff       (20)     1956 2022-02-03 00:32:26.000000 running-ng-0.3.8/tests/test_suite.py
--rw-r--r--   0 caizixian   (501) staff       (20)      263 2021-10-11 12:28:38.000000 running-ng-0.3.8/tests/test_util.py
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.922871 running-ng-0.3.9/
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.905057 running-ng-0.3.9/.github/
+-rw-r--r--   0 caizixian   (501) staff       (20)      106 2021-10-11 12:28:38.000000 running-ng-0.3.9/.github/dependabot.yml
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.905561 running-ng-0.3.9/.github/workflows/
+-rw-r--r--   0 caizixian   (501) staff       (20)      470 2022-02-20 06:52:54.000000 running-ng-0.3.9/.github/workflows/mdbook.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)     1216 2023-01-16 05:20:12.000000 running-ng-0.3.9/.github/workflows/python.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)     1809 2021-10-11 12:28:38.000000 running-ng-0.3.9/.gitignore
+-rw-r--r--   0 caizixian   (501) staff       (20)    11357 2022-02-20 06:52:54.000000 running-ng-0.3.9/LICENSE
+-rw-r--r--   0 caizixian   (501) staff       (20)     1611 2023-08-02 04:49:45.922559 running-ng-0.3.9/PKG-INFO
+-rw-r--r--   0 caizixian   (501) staff       (20)      954 2022-10-12 05:14:15.000000 running-ng-0.3.9/README.md
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.906238 running-ng-0.3.9/docs/
+-rw-r--r--   0 caizixian   (501) staff       (20)        5 2021-10-11 12:28:38.000000 running-ng-0.3.9/docs/.gitignore
+-rw-r--r--   0 caizixian   (501) staff       (20)      116 2021-10-11 12:28:38.000000 running-ng-0.3.9/docs/book.toml
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.908124 running-ng-0.3.9/docs/src/
+-rw-r--r--   0 caizixian   (501) staff       (20)      689 2021-11-06 11:26:31.000000 running-ng-0.3.9/docs/src/SUMMARY.md
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.908893 running-ng-0.3.9/docs/src/basics/
+-rw-r--r--   0 caizixian   (501) staff       (20)     1619 2021-11-06 11:26:31.000000 running-ng-0.3.9/docs/src/basics/design.md
+-rw-r--r--   0 caizixian   (501) staff       (20)      221 2021-10-11 12:28:38.000000 running-ng-0.3.9/docs/src/basics/index.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     8051 2023-08-02 04:42:20.000000 running-ng-0.3.9/docs/src/changelog.md
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.909868 running-ng-0.3.9/docs/src/commands/
+-rw-r--r--   0 caizixian   (501) staff       (20)       11 2021-10-11 12:28:38.000000 running-ng-0.3.9/docs/src/commands/fillin.md
+-rw-r--r--   0 caizixian   (501) staff       (20)      878 2021-11-06 11:26:31.000000 running-ng-0.3.9/docs/src/commands/index.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     2389 2022-02-16 02:25:49.000000 running-ng-0.3.9/docs/src/commands/minheap.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     6226 2023-02-14 11:19:25.000000 running-ng-0.3.9/docs/src/commands/runbms.md
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.910500 running-ng-0.3.9/docs/src/cookbook/
+-rw-r--r--   0 caizixian   (501) staff       (20)       40 2021-11-06 11:26:31.000000 running-ng-0.3.9/docs/src/cookbook/index.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     4650 2023-07-25 06:10:45.000000 running-ng-0.3.9/docs/src/cookbook/perf_events.md
+-rw-r--r--   0 caizixian   (501) staff       (20)       29 2021-11-06 11:26:31.000000 running-ng-0.3.9/docs/src/faq.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     1429 2022-02-20 07:25:27.000000 running-ng-0.3.9/docs/src/install.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     2910 2021-11-06 11:26:31.000000 running-ng-0.3.9/docs/src/intro.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     5034 2023-02-14 11:19:25.000000 running-ng-0.3.9/docs/src/quickstart.md
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.912064 running-ng-0.3.9/docs/src/references/
+-rw-r--r--   0 caizixian   (501) staff       (20)     5373 2022-09-06 03:25:59.000000 running-ng-0.3.9/docs/src/references/index.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     2584 2022-10-12 05:13:38.000000 running-ng-0.3.9/docs/src/references/modifier.md
+-rw-r--r--   0 caizixian   (501) staff       (20)      559 2022-02-03 03:09:20.000000 running-ng-0.3.9/docs/src/references/runtime.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     7301 2023-08-02 04:42:20.000000 running-ng-0.3.9/docs/src/references/suite.md
+-rw-r--r--   0 caizixian   (501) staff       (20)     1156 2023-08-02 04:42:16.000000 running-ng-0.3.9/pyproject.toml
+-rw-r--r--   0 caizixian   (501) staff       (20)       38 2023-08-02 04:49:45.922914 running-ng-0.3.9/setup.cfg
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.903597 running-ng-0.3.9/src/
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.914764 running-ng-0.3.9/src/running/
+-rw-r--r--   0 caizixian   (501) staff       (20)        0 2022-02-20 06:52:54.000000 running-ng-0.3.9/src/running/__init__.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     1581 2022-09-06 03:25:59.000000 running-ng-0.3.9/src/running/__main__.py
+-rw-r--r--   0 caizixian   (501) staff       (20)       62 2023-08-02 04:42:20.000000 running-ng-0.3.9/src/running/__version__.py
+-rw-r--r--   0 caizixian   (501) staff       (20)    10006 2023-04-13 07:11:13.000000 running-ng-0.3.9/src/running/benchmark.py
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.916214 running-ng-0.3.9/src/running/command/
+-rw-r--r--   0 caizixian   (501) staff       (20)        0 2022-02-20 06:52:54.000000 running-ng-0.3.9/src/running/command/__init__.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     2048 2022-02-20 06:52:54.000000 running-ng-0.3.9/src/running/command/fillin.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     2928 2022-02-20 06:52:54.000000 running-ng-0.3.9/src/running/command/genadvice.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     7462 2023-01-16 05:20:12.000000 running-ng-0.3.9/src/running/command/log_preprocessor.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     6781 2023-01-16 05:20:12.000000 running-ng-0.3.9/src/running/command/minheap.py
+-rw-r--r--   0 caizixian   (501) staff       (20)    15940 2023-01-16 05:20:12.000000 running-ng-0.3.9/src/running/command/runbms.py
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.916731 running-ng-0.3.9/src/running/config/
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.918869 running-ng-0.3.9/src/running/config/base/
+-rw-r--r--   0 caizixian   (501) staff       (20)     5346 2023-01-16 04:33:32.000000 running-ng-0.3.9/src/running/config/base/dacapo.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)       28 2022-09-06 03:25:59.000000 running-ng-0.3.9/src/running/config/base/jvms.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)       95 2022-02-20 06:52:54.000000 running-ng-0.3.9/src/running/config/base/minheap.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)     1220 2022-02-20 06:52:54.000000 running-ng-0.3.9/src/running/config/base/modifiers.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      259 2022-02-20 06:52:54.000000 running-ng-0.3.9/src/running/config/base/runbms.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      127 2022-02-20 06:52:54.000000 running-ng-0.3.9/src/running/config/base/specjbb2015.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      132 2022-03-19 05:22:35.000000 running-ng-0.3.9/src/running/config/base/specjvm98.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)       75 2022-03-19 05:22:35.000000 running-ng-0.3.9/src/running/config/base/suites.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      283 2022-02-20 06:52:54.000000 running-ng-0.3.9/src/running/config/base/temurin.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      214 2022-09-06 03:25:59.000000 running-ng-0.3.9/src/running/config/minheap_example.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)      964 2022-09-06 03:25:59.000000 running-ng-0.3.9/src/running/config/runbms_example.yml
+-rw-r--r--   0 caizixian   (501) staff       (20)     5750 2022-09-06 03:25:59.000000 running-ng-0.3.9/src/running/config.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     4754 2022-10-12 11:26:16.000000 running-ng-0.3.9/src/running/modifier.py
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.919038 running-ng-0.3.9/src/running/plugin/
+-rw-r--r--   0 caizixian   (501) staff       (20)        0 2022-02-20 06:52:54.000000 running-ng-0.3.9/src/running/plugin/__init__.py
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.919594 running-ng-0.3.9/src/running/plugin/runbms/
+-rw-r--r--   0 caizixian   (501) staff       (20)     2768 2023-08-02 04:48:53.000000 running-ng-0.3.9/src/running/plugin/runbms/__init__.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     3090 2022-02-20 06:52:54.000000 running-ng-0.3.9/src/running/plugin/runbms/copyfile.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     5917 2023-01-16 05:20:12.000000 running-ng-0.3.9/src/running/plugin/runbms/zulip.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     6049 2022-03-07 03:16:48.000000 running-ng-0.3.9/src/running/runtime.py
+-rw-r--r--   0 caizixian   (501) staff       (20)    15772 2023-08-02 04:42:20.000000 running-ng-0.3.9/src/running/suite.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     4997 2023-02-14 11:19:25.000000 running-ng-0.3.9/src/running/util.py
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.920519 running-ng-0.3.9/src/running_ng.egg-info/
+-rw-r--r--   0 caizixian   (501) staff       (20)     1611 2023-08-02 04:49:45.000000 running-ng-0.3.9/src/running_ng.egg-info/PKG-INFO
+-rw-r--r--   0 caizixian   (501) staff       (20)     1955 2023-08-02 04:49:45.000000 running-ng-0.3.9/src/running_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 caizixian   (501) staff       (20)        1 2023-08-02 04:49:45.000000 running-ng-0.3.9/src/running_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 caizixian   (501) staff       (20)       50 2023-08-02 04:49:45.000000 running-ng-0.3.9/src/running_ng.egg-info/entry_points.txt
+-rw-r--r--   0 caizixian   (501) staff       (20)      102 2023-08-02 04:49:45.000000 running-ng-0.3.9/src/running_ng.egg-info/requires.txt
+-rw-r--r--   0 caizixian   (501) staff       (20)        8 2023-08-02 04:49:45.000000 running-ng-0.3.9/src/running_ng.egg-info/top_level.txt
+drwxr-xr-x   0 caizixian   (501) staff       (20)        0 2023-08-02 04:49:45.922271 running-ng-0.3.9/tests/
+-rw-r--r--   0 caizixian   (501) staff       (20)     2134 2022-03-07 03:16:48.000000 running-ng-0.3.9/tests/test_config.py
+-rw-r--r--   0 caizixian   (501) staff       (20)      682 2021-10-11 12:28:38.000000 running-ng-0.3.9/tests/test_fillin.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     1858 2021-10-11 12:28:38.000000 running-ng-0.3.9/tests/test_log_preprocessor.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     2737 2022-03-19 05:00:18.000000 running-ng-0.3.9/tests/test_modifier.py
+-rw-r--r--   0 caizixian   (501) staff       (20)      469 2021-10-11 12:28:38.000000 running-ng-0.3.9/tests/test_runbms.py
+-rw-r--r--   0 caizixian   (501) staff       (20)     2431 2023-08-02 04:48:28.000000 running-ng-0.3.9/tests/test_suite.py
+-rw-r--r--   0 caizixian   (501) staff       (20)      263 2021-10-11 12:28:38.000000 running-ng-0.3.9/tests/test_util.py
```

### Comparing `running-ng-0.3.8/.github/workflows/python.yml` & `running-ng-0.3.9/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/.gitignore` & `running-ng-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/LICENSE` & `running-ng-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/PKG-INFO` & `running-ng-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: running-ng
-Version: 0.3.8
+Version: 0.3.9
 Summary: Running: Next Generation
 Author-email: Zixian Cai <u5937495@anu.edu.au>
 License: Apache
 Project-URL: Homepage, https://github.com/anupli/running-ng
 Project-URL: Bug Tracker, https://github.com/anupli/running-ng/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `running-ng-0.3.8/README.md` & `running-ng-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/docs/src/SUMMARY.md` & `running-ng-0.3.9/docs/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/docs/src/basics/design.md` & `running-ng-0.3.9/docs/src/basics/design.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/docs/src/changelog.md` & `running-ng-0.3.9/docs/src/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 
 ### Removed
 
 ### Fixed
 
 ### Security
 
+## [`v0.3.9` (2023-08-02)](https://github.com/anupli/running-ng/releases/tag/v0.3.9)
+### Fixed
+#### Benchmark Suites
+- `DaCapo`: don't explicitly pass `-s default` to DaCapo unless the user requests so by setting the `size` key of `DaCapo` or overriding the sizes for individual benchmarks using the [benchmark specification syntax](./references/suite.md#benchmark-specification). This is so that users can override the size via `ProgramArg`.
+
 ## [`v0.3.8` (2023-02-21)](https://github.com/anupli/running-ng/releases/tag/v0.3.8)
 ### Changed
 #### Commands
 - `runbms`: companion programs are now expected to self-terminate.
 
 ## [`v0.3.7` (2023-02-14)](https://github.com/anupli/running-ng/releases/tag/v0.3.7)
 ### Fixed
```

### Comparing `running-ng-0.3.8/docs/src/commands/index.md` & `running-ng-0.3.9/docs/src/commands/index.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/docs/src/commands/minheap.md` & `running-ng-0.3.9/docs/src/commands/minheap.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/docs/src/commands/runbms.md` & `running-ng-0.3.9/docs/src/commands/runbms.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/docs/src/cookbook/perf_events.md` & `running-ng-0.3.9/docs/src/cookbook/perf_events.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Whole-Process Performance Event Monitoring
 ## JVMTI
-Please clone and build [`probes`](../quickstart.md#prepare-probes).
+Please clone and build [`probes`](../quickstart.md#prepare-probes), and then build [`distillation`](https://github.com/caizixian/distillation).
+You might need to change the paths referred in the `Makefile`s to match your environment.
 
-Under the `probes` folder, you will find a JVMTI agent, `libperf_statistics.so`.
-You can check the source code [here](https://github.com/anupli/probes/blob/master/native/jvmti_agents/perf_statistics.c).
+Under the `distillation` folder, you will find a JVMTI agent, `libperf_statistics.so`.
+You can check the source code [here](https://github.com/caizixian/distillation/blob/master/perf_statistics.c).
 To use the agent, there are four things you need to do.
 
 First, you will need to tell the dynamic linker to load the shared library before the VM boots.
 This ensures that the `inherit` flag of `perf_event_attr` works properly and all child threads subsequently spawned are included in the results.
 ```yaml
 modifiers:
   jvmti_env:
     type: EnvVar
     var: "LD_PRELOAD"
-    val: "/path/to/probes/libperf_statistics.so"
+    val: "/path/to/distillation/libperf_statistics.so"
 ```
 
 Second, you need to specify a list of events you want to measure.
 ```yaml
 modifiers:
   perf:
     type: EnvVar
@@ -28,27 +29,27 @@
 
 Third, you need to tell the JVM to load the agent.
 Note that you need to specify the absolute path.
 ```yaml
 modifiers:
   jvmti:
     type: JVMArg
-    val: "-agentpath:/path/to/probes/libperf_statistics.so"
+    val: "-agentpath:/path/to/distillation/libperf_statistics.so"
 ```
 
 Finally, you need to let the DaCapo benchmark inform the start and the end of a benchmark iteration.
 We will reuse the `RustMMTk` probe here, as the callback functions in the JVMTI agent are also called `harness_begin` and `harness_end`.
 ```yaml
 modifiers:
   probes_cp:
     type: JVMClasspath
-    val: "/path/to/probes /path/to/probes/probes.jar"
+    val: "/path/to/probes/out /path/to/probes/out/probes.jar"
   probes:
     type: JVMArg
-    val: "-Djava.library.path=/path/to/probes -Dprobes=RustMMTk"
+    val: "-Djava.library.path=/path/to/probes/out -Dprobes=RustMMTk"
 ```
 
 Now, putting it all together, you can define a set of modifiers, and use that set in your config strings.
 ```yaml
 modifiers:
   jvmti_common:
     type: ModifierSet
@@ -60,18 +61,18 @@
 You will need to build `mmtk-core` with the `perf_counter` feature.
 
 First, you need to let the DaCapo benchmark inform the start and the end of a benchmark iteration.
 ```yaml
 modifiers:
   probes_cp:
     type: JVMClasspath
-    val: "/path/to/probes /path/to/probes/probes.jar"
+    val: "/path/to/probes/out /path/to/probes/out/probes.jar"
   probes:
     type: JVMArg
-    val: "-Djava.library.path=/path/to/probes -Dprobes=RustMMTk"
+    val: "-Djava.library.path=/path/to/probes/out -Dprobes=RustMMTk"
 ```
 
 Then, you can specify a list of events you want to measure.
 ```yaml
 modifiers:
   mmtk_perf:
     type: EnvVar
@@ -88,16 +89,16 @@
 
 **Note that you might have to increase the value of `MAX_PHASES` in `crate::util::statistics::stats` to a larger value, e.g., `1 << 14`, so that the array storing the per-phase value will not overflow.**
 
 # Work-Packet Performance Event Monitoring
 It's similar to the whole-process performance event monitoring for MMTk.
 Just use `MMTK_WORK_PERF_EVENTS` instead of `MMTK_PHASE_PERF_EVENTS`.
 
-# Machine-Specific Notes
-On Xeon D-1540 Broadwell (`mole` and `vole`), the `PERF_COUNT_HW_CACHE_LL:MISS` event is always zero.
+# Machine-Specific Known Problems
+On Xeon D-1540 Broadwell, the `PERF_COUNT_HW_CACHE_LL:MISS` event is always zero.
 ```console
 perf stat -e LLC-load-misses,cycles /bin/ls
 
  Performance counter stats for '/bin/ls':
 
                  0      LLC-load-misses
          1,729,786      cycles
```

### Comparing `running-ng-0.3.8/docs/src/install.md` & `running-ng-0.3.9/docs/src/install.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/docs/src/intro.md` & `running-ng-0.3.9/docs/src/intro.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/docs/src/quickstart.md` & `running-ng-0.3.9/docs/src/quickstart.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/docs/src/references/index.md` & `running-ng-0.3.9/docs/src/references/index.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/docs/src/references/modifier.md` & `running-ng-0.3.9/docs/src/references/modifier.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/docs/src/references/runtime.md` & `running-ng-0.3.9/docs/src/references/runtime.md`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/docs/src/references/suite.md` & `running-ng-0.3.9/docs/src/references/suite.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   [...]
 ```
 
 A possible use-case could use wrapper shell scripts around the benchmark to
 output timing and other information in a tab-separated table.
 
 ## `DaCapo`
-[DaCapo benchmark suite](http://dacapo-bench.org/).
+[DaCapo benchmark suite](https://www.dacapobench.org/).
 ### Keys
 `release`: one of the possible values `["2006", "9.12", "evaluation"]`.
 The value is required.
 
 `path`: path to the DaCapo `jar`.
 The value is required.
 
@@ -85,21 +85,18 @@
   dacapo2006:
     - fop
 
 configs:
   - "temurin-17"
 ```
 In the log file, the output from the main program and the output from the companion program is separated by `*****`.
-A companion program should shutdown cleanly upon receiving `SIGINT` (Ctrl-C).
-In the case of `bpftrace`, one should avoid using `exit()`.
-Otherwise, a `SIGINT` during `exit()` will stop printing the rest of the maps, resulting in data loss.
 
 `size`: specifying the size of input data.
 Note that the names of the sizes are subject to change depending on the DaCapo releases.
-The default value is `default`.
+The default value is `null`, which means DaCapo will use the default size unless you override that for individual benchmarks.
 
 ### Benchmark Specification
 Some of the suite-wide keys can be overridden in a per-benchmark-basis.
 The keys currently supported are `timing_iteration`, `size`, and `timeout`.
 Note that, within a suite, your choice of `name` should uniquely identify a particular way of running a benchmark of name `bm_name`.
 The `name` is used to get the minheap value, etc., which can depend of the size of input data and/or the timing iteration.
 Therefore, it is highly recommended that you give a `name` different from the `bm_name`.
```

### Comparing `running-ng-0.3.8/pyproject.toml` & `running-ng-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 "Bug Tracker" = "https://github.com/anupli/running-ng/issues"
 
 [project.optional-dependencies]
 zulip = [
     "zulip~=0.8.2"
 ]
 tests = [
-    "pytest>=7.1.3,<7.3.0",
+    "pytest>=7.1.3,<7.5.0",
     "types-PyYAML~=6.0.11",
     "mypy>=0.971,<2.0"
 ]
 
 [project.scripts]
 running = "running.__main__:main"
```

### Comparing `running-ng-0.3.8/src/running/__main__.py` & `running-ng-0.3.9/src/running/__main__.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/benchmark.py` & `running-ng-0.3.9/src/running/benchmark.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/command/fillin.py` & `running-ng-0.3.9/src/running/command/fillin.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/command/genadvice.py` & `running-ng-0.3.9/src/running/command/genadvice.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/command/log_preprocessor.py` & `running-ng-0.3.9/src/running/command/log_preprocessor.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/command/minheap.py` & `running-ng-0.3.9/src/running/command/minheap.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/command/runbms.py` & `running-ng-0.3.9/src/running/command/runbms.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/config/base/dacapo.yml` & `running-ng-0.3.9/src/running/config/base/dacapo.yml`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/config/base/modifiers.yml` & `running-ng-0.3.9/src/running/config/base/modifiers.yml`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/config/runbms_example.yml` & `running-ng-0.3.9/src/running/config/runbms_example.yml`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/config.py` & `running-ng-0.3.9/src/running/config.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/modifier.py` & `running-ng-0.3.9/src/running/modifier.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/plugin/runbms/__init__.py` & `running-ng-0.3.9/src/running/plugin/runbms/__init__.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/plugin/runbms/copyfile.py` & `running-ng-0.3.9/src/running/plugin/runbms/copyfile.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/plugin/runbms/zulip.py` & `running-ng-0.3.9/src/running/plugin/runbms/zulip.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/runtime.py` & `running-ng-0.3.9/src/running/runtime.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running/suite.py` & `running-ng-0.3.9/src/running/suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,16 +135,17 @@
         self.callback = kwargs.get("callback")
         self.timeout: Optional[int]
         self.timeout = kwargs.get("timeout")
         self.wrapper: Optional[Union[Dict[str, str], str]]
         self.wrapper = kwargs.get("wrapper")
         self.companion: Optional[Union[Dict[str, str], str]]
         self.companion = kwargs.get("companion")
-        self.size: str
-        self.size = kwargs.get("size", "default")
+        # user overriding the default size for the entire suite
+        self.size: Optional[str]
+        self.size = kwargs.get("size")
 
     def __str__(self) -> str:
         return "{} DaCapo {} {}".format(super().__str__(), self.release, self.path)
 
     @staticmethod
     def parse_timing_iteration(v: Any):
         try:
@@ -170,14 +171,15 @@
                 raise KeyError(
                     "When a dictionary is used to speicfy a benchmark, you need to provide both `name` and `bm_name`")
             bm_name = bm_spec["bm_name"]
             name = bm_spec["name"]
             if "timing_iteration" in bm_spec:
                 timing_iteration = DaCapo.parse_timing_iteration(
                     bm_spec["timing_iteration"])
+            # user overriding the size for that benchmark
             if "size" in bm_spec:
                 size = bm_spec["size"]
             if "timeout" in bm_spec:
                 timeout = bm_spec["timeout"]
 
         if self.callback:
             cp = [str(self.path)]
@@ -191,15 +193,16 @@
         else:
             assert timing_iteration == "converge"
             if self.release == "2006":
                 program_args.append("-converge")
             else:
                 program_args.append("--converge")
         # Input size
-        program_args.extend(["-s", size])
+        if size:
+            program_args.extend(["-s", size])
         # Name of the benchmark
         program_args.append(bm_name)
         return JavaBenchmark(
             jvm_args=[],
             program_args=program_args,
             cp=cp,
             wrapper=self.get_wrapper(bm_name),
```

### Comparing `running-ng-0.3.8/src/running/util.py` & `running-ng-0.3.9/src/running/util.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/src/running_ng.egg-info/PKG-INFO` & `running-ng-0.3.9/src/running_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: running-ng
-Version: 0.3.8
+Version: 0.3.9
 Summary: Running: Next Generation
 Author-email: Zixian Cai <u5937495@anu.edu.au>
 License: Apache
 Project-URL: Homepage, https://github.com/anupli/running-ng
 Project-URL: Bug Tracker, https://github.com/anupli/running-ng/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `running-ng-0.3.8/src/running_ng.egg-info/SOURCES.txt` & `running-ng-0.3.9/src/running_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/tests/test_config.py` & `running-ng-0.3.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/tests/test_fillin.py` & `running-ng-0.3.9/tests/test_fillin.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/tests/test_log_preprocessor.py` & `running-ng-0.3.9/tests/test_log_preprocessor.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/tests/test_modifier.py` & `running-ng-0.3.9/tests/test_modifier.py`

 * *Files identical despite different names*

### Comparing `running-ng-0.3.8/tests/test_suite.py` & `running-ng-0.3.9/tests/test_suite.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,28 +20,40 @@
     c = Configuration({
         "suites": {
             "dacapo2006": {
                 "type": "DaCapo",
                 "release": "2006",
                 "path": "/usr/share/benchmarks/dacapo/dacapo-2006-10-MR2.jar",
                 "timing_iteration": 3
+            },
+            "dacapo2006_default": {
+                "type": "DaCapo",
+                "release": "2006",
+                "path": "/usr/share/benchmarks/dacapo/dacapo-2006-10-MR2.jar",
+                "timing_iteration": 3,
+                "size": "default"
             }
         },
         "benchmarks": {
             "dacapo2006": [
                 "fop",
                 dict(name="fop_small", bm_name="fop", size="small")
+            ],
+            "dacapo2006_default": [
+                "fop"
             ]
         }
     })
 
     c.resolve_class()
     fop = c.get("benchmarks")["dacapo2006"][0]
+    fop_default = c.get("benchmarks")["dacapo2006_default"][0]
     fop_small = c.get("benchmarks")["dacapo2006"][1]
-    assert "-s default" in fop.to_string(DummyRuntime("java"))
+    assert "-s" not in fop.to_string(DummyRuntime("java"))
+    assert "-s default" in fop_default.to_string(DummyRuntime("java"))
     assert "-s small" in fop_small.to_string(DummyRuntime("java"))
 
 
 def test_dacapo_timing_iteration():
     c = Configuration({
         "suites": {
             "dacapo2006": {
```

