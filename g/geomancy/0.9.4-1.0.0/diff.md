# Comparing `tmp/geomancy-0.9.4.tar.gz` & `tmp/geomancy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomancy-0.9.4.tar", last modified: Sun Jul 30 02:41:10 2023, max compression
+gzip compressed data, was "geomancy-1.0.0.tar", last modified: Wed Aug  2 21:34:17 2023, max compression
```

## Comparing `geomancy-0.9.4.tar` & `geomancy-1.0.0.tar`

### file list

```diff
@@ -1,88 +1,112 @@
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.367814 geomancy-0.9.4/
--rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-26 14:41:25.000000 geomancy-0.9.4/.editorconfig
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.342615 geomancy-0.9.4/.github/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.350307 geomancy-0.9.4/.github/workflows/
--rw-r--r--   0 jlorieau   (501) staff       (20)      757 2023-07-30 02:36:10.000000 geomancy-0.9.4/.github/workflows/tests.yml
--rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-24 22:25:03.000000 geomancy-0.9.4/.gitignore
--rw-r--r--   0 jlorieau   (501) staff       (20)      233 2023-07-25 16:40:32.000000 geomancy-0.9.4/.readthedocs.yaml
--rw-r--r--   0 jlorieau   (501) staff       (20)     1023 2023-07-26 00:50:48.000000 geomancy-0.9.4/LICENSE
--rw-r--r--   0 jlorieau   (501) staff       (20)     6318 2023-07-30 02:41:10.367471 geomancy-0.9.4/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     5138 2023-07-30 02:40:03.000000 geomancy-0.9.4/README.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     1711 2023-07-26 14:41:25.000000 geomancy-0.9.4/Taskfile.yaml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.350979 geomancy-0.9.4/changelog/
--rw-r--r--   0 jlorieau   (501) staff       (20)      310 2023-07-25 18:53:41.000000 geomancy-0.9.4/changelog/changelog_template.jinja
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.352235 geomancy-0.9.4/docs/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.353223 geomancy-0.9.4/docs/_static/
--rw-r--r--   0 jlorieau   (501) staff       (20)      466 2023-07-26 14:41:25.000000 geomancy-0.9.4/docs/_static/custom.css
--rw-r--r--   0 jlorieau   (501) staff       (20)    49829 2023-07-25 15:23:09.000000 geomancy-0.9.4/docs/_static/geomancy_logo.png
--rw-r--r--   0 jlorieau   (501) staff       (20)     6346 2023-07-28 19:38:01.000000 geomancy-0.9.4/docs/_static/geomancy_logo.svg
--rw-r--r--   0 jlorieau   (501) staff       (20)     3543 2023-07-30 02:36:10.000000 geomancy-0.9.4/docs/changelog.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     2121 2023-07-29 16:55:41.000000 geomancy-0.9.4/docs/conf.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      651 2023-07-28 19:38:01.000000 geomancy-0.9.4/docs/index.md
--rw-r--r--   0 jlorieau   (501) staff       (20)      121 2023-07-25 15:07:00.000000 geomancy-0.9.4/docs/quickstart.md
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.354119 geomancy-0.9.4/docs/usage/
--rw-r--r--   0 jlorieau   (501) staff       (20)     8813 2023-07-29 16:55:41.000000 geomancy-0.9.4/docs/usage/cmd_checks.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     1437 2023-07-28 19:38:01.000000 geomancy-0.9.4/docs/usage/cmd_run.md
--rw-r--r--   0 jlorieau   (501) staff       (20)    13139 2023-07-30 02:36:10.000000 geomancy-0.9.4/docs/usage/format.md
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.355260 geomancy-0.9.4/examples/
--rw-r--r--   0 jlorieau   (501) staff       (20)     1763 2023-07-30 02:36:10.000000 geomancy-0.9.4/examples/geomancy.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)     1883 2023-07-30 02:36:10.000000 geomancy-0.9.4/examples/geomancy.yaml
--rw-r--r--   0 jlorieau   (501) staff       (20)      272 2023-07-26 14:41:25.000000 geomancy-0.9.4/examples/geomancy_flat.yaml
--rw-r--r--   0 jlorieau   (501) staff       (20)      369 2023-07-30 02:36:10.000000 geomancy-0.9.4/examples/pyproject.toml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.355823 geomancy-0.9.4/geomancy/
--rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.9.4/geomancy/__description__.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      485 2023-07-30 02:40:59.000000 geomancy-0.9.4/geomancy/__init__.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.359986 geomancy-0.9.4/geomancy/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)      388 2023-07-30 02:36:10.000000 geomancy-0.9.4/geomancy/checks/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)    12445 2023-07-30 02:36:10.000000 geomancy-0.9.4/geomancy/checks/base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1696 2023-07-29 16:55:41.000000 geomancy-0.9.4/geomancy/checks/env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2426 2023-07-24 15:55:52.000000 geomancy-0.9.4/geomancy/checks/exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.9.4/geomancy/checks/path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2359 2023-07-30 02:36:10.000000 geomancy-0.9.4/geomancy/checks/platform.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1378 2023-07-30 02:36:10.000000 geomancy-0.9.4/geomancy/checks/python.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     5242 2023-07-29 16:55:41.000000 geomancy-0.9.4/geomancy/checks/utils.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2381 2023-07-30 02:36:10.000000 geomancy-0.9.4/geomancy/checks/version.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.360535 geomancy-0.9.4/geomancy/cli/
--rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-27 16:55:31.000000 geomancy-0.9.4/geomancy/cli/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     6640 2023-07-29 16:55:41.000000 geomancy-0.9.4/geomancy/cli/term.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.361091 geomancy-0.9.4/geomancy/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.9.4/geomancy/config/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)    13410 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/config/config.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.363009 geomancy-0.9.4/geomancy/entrypoints/
--rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/entrypoints/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     3423 2023-07-29 16:55:41.000000 geomancy-0.9.4/geomancy/entrypoints/check.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      546 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/entrypoints/config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     4136 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/entrypoints/environment.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1427 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/entrypoints/geo.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      487 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/entrypoints/run.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      904 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/entrypoints/utils.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.363570 geomancy-0.9.4/geomancy/environment/
--rw-r--r--   0 jlorieau   (501) staff       (20)      164 2023-07-29 16:55:41.000000 geomancy-0.9.4/geomancy/environment/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     8587 2023-07-29 16:55:41.000000 geomancy-0.9.4/geomancy/environment/dotenv.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.357527 geomancy-0.9.4/geomancy.egg-info/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6318 2023-07-30 02:41:10.000000 geomancy-0.9.4/geomancy.egg-info/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     1637 2023-07-30 02:41:10.000000 geomancy-0.9.4/geomancy.egg-info/SOURCES.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-30 02:41:10.000000 geomancy-0.9.4/geomancy.egg-info/dependency_links.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       53 2023-07-30 02:41:10.000000 geomancy-0.9.4/geomancy.egg-info/entry_points.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      167 2023-07-30 02:41:10.000000 geomancy-0.9.4/geomancy.egg-info/requires.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-30 02:41:10.000000 geomancy-0.9.4/geomancy.egg-info/top_level.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)     2836 2023-07-28 19:38:01.000000 geomancy-0.9.4/pyproject.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-30 02:41:10.367903 geomancy-0.9.4/setup.cfg
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.363848 geomancy-0.9.4/tests/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.365505 geomancy-0.9.4/tests/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)     5181 2023-07-29 16:55:41.000000 geomancy-0.9.4/tests/checks/test_base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2690 2023-07-29 16:55:41.000000 geomancy-0.9.4/tests/checks/test_env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1074 2023-07-29 02:10:42.000000 geomancy-0.9.4/tests/checks/test_exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2193 2023-07-29 16:55:41.000000 geomancy-0.9.4/tests/checks/test_path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      612 2023-07-30 02:36:10.000000 geomancy-0.9.4/tests/checks/test_platform.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      936 2023-07-30 02:36:10.000000 geomancy-0.9.4/tests/checks/test_python.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.366057 geomancy-0.9.4/tests/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.9.4/tests/config/config1.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)     7826 2023-07-28 19:38:01.000000 geomancy-0.9.4/tests/config/test_config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      524 2023-07-25 04:11:09.000000 geomancy-0.9.4/tests/conftest.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.366328 geomancy-0.9.4/tests/data/
--rw-r--r--   0 jlorieau   (501) staff       (20)      159 2023-07-25 01:20:06.000000 geomancy-0.9.4/tests/data/test.env
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.366602 geomancy-0.9.4/tests/entrypoints/
--rw-r--r--   0 jlorieau   (501) staff       (20)     4417 2023-07-28 19:38:01.000000 geomancy-0.9.4/tests/entrypoints/test_geo.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.366882 geomancy-0.9.4/tests/environment/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6043 2023-07-29 16:55:41.000000 geomancy-0.9.4/tests/environment/test_dotenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.514897 geomancy-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-02 21:34:06.000000 geomancy-1.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-02 21:34:06.000000 geomancy-1.0.0/.geomancy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.494896 geomancy-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.498896 geomancy-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-02 21:34:06.000000 geomancy-1.0.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-02 21:34:06.000000 geomancy-1.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-02 21:34:06.000000 geomancy-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-02 21:34:06.000000 geomancy-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-02 21:34:06.000000 geomancy-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-08-02 21:34:17.510897 geomancy-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-08-02 21:34:06.000000 geomancy-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-02 21:34:06.000000 geomancy-1.0.0/Taskfile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.498896 geomancy-1.0.0/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-02 21:34:06.000000 geomancy-1.0.0/changelog/changelog_template.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.498896 geomancy-1.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.498896 geomancy-1.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    49829 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/_static/geomancy_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/_static/geomancy_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.498896 geomancy-1.0.0/docs/about/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.498896 geomancy-1.0.0/docs/about/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/about/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/about/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/docs/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/checks/aws.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/checks/core.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/docs/checks/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/checks/snippets/base_args.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/guides/tips_and_tricks.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/usage/cmd_checks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/usage/cmd_run.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-08-02 21:34:06.000000 geomancy-1.0.0/docs/usage/format.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/examples/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-02 21:34:06.000000 geomancy-1.0.0/examples/aws/fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-02 21:34:06.000000 geomancy-1.0.0/examples/aws/geomancy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-02 21:34:06.000000 geomancy-1.0.0/examples/geomancy.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 21:34:06.000000 geomancy-1.0.0/examples/geomancy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-02 21:34:06.000000 geomancy-1.0.0/examples/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/geomancy/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/__description__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.506897 geomancy-1.0.0/geomancy/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.506897 geomancy-1.0.0/geomancy/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18066 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/checks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.506897 geomancy-1.0.0/geomancy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.506897 geomancy-1.0.0/geomancy/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/entrypoints/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.506897 geomancy-1.0.0/geomancy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-02 21:34:06.000000 geomancy-1.0.0/geomancy/environment/dotenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.502897 geomancy-1.0.0/geomancy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-08-02 21:34:17.000000 geomancy-1.0.0/geomancy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-08-02 21:34:17.000000 geomancy-1.0.0/geomancy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:34:17.000000 geomancy-1.0.0/geomancy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 21:34:17.000000 geomancy-1.0.0/geomancy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-02 21:34:17.000000 geomancy-1.0.0/geomancy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 21:34:17.000000 geomancy-1.0.0/geomancy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-08-02 21:34:06.000000 geomancy-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:34:17.514897 geomancy-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.506897 geomancy-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/checks/aws/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.494896 geomancy-1.0.0/tests/checks/aws/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_missing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/aws/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/test_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/checks/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/config/config1.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/data/test.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/entrypoints/test_geo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:34:17.510897 geomancy-1.0.0/tests/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-02 21:34:06.000000 geomancy-1.0.0/tests/environment/test_dotenv.py
```

### Comparing `geomancy-0.9.4/.github/workflows/tests.yml` & `geomancy-1.0.0/.github/workflows/tests.yml`

 * *Files 23% similar despite different names*

```diff
@@ -14,21 +14,26 @@
   test:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
         python-version: ["3.11"]
+    env:
+        AWS_ACCESS_KEY_ID: MOCK_ACCESS_KEY_ID
+        AWS_SECRET_ACCESS_KEY: MOCK_SECRET_ACCESS_KEY
+        AWS_SECURITY_TOKEN: MOCK_SECURITY_TOKEN
+        AWS_SESSION_TOKEN: MOCK_SESSION_TOKEN
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install .[dev]
+          python -m pip install .[all,dev]
       - name: Test with pytest
         run: |
           pytest --log-level=DEBUG
```

### Comparing `geomancy-0.9.4/.gitignore` & `geomancy-1.0.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+# Sphinx autosummary stubs
+docs/about/api/generated/*
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `geomancy-0.9.4/LICENSE` & `geomancy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/Taskfile.yaml` & `geomancy-1.0.0/Taskfile.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,91 @@
 # https://taskfile.dev/
 version: '3'
 
 vars:
-    PROJECT_NAME: geomancy
-    SPHINX_BUILD: .venv/bin/sphinx-build  # run from within virtualenv
-    SPHINX_OPTS: ""
-    SPHINX_SOURCE_DIR: .
-    SPHINX_BUILD_DIR: _build
+  PROJECT_NAME: geomancy
+  SPHINX_BUILD: .venv/bin/sphinx-build  # run from within virtualenv
+  SPHINX_OPTS: ""
+  SPHINX_SOURCE_DIR: .
+  SPHINX_BUILD_DIR: _build
+
 
 tasks:
 
   create-env:
     desc: Create a local virtual environment for development
     internal: true
     cmds:
       - python3 -m venv .venv
     generates:
       - .venv
 
   install:
     desc: Install the package in development (edit) mode
     cmds:
-      - python -m pip install -e ".[dev,docs]"
+      - python3 -m pip install -e ".[all,dev,docs]"
     sources:
       - pyproject.toml
 
   setup:
     desc: Setup the development environment
     cmds:
       - task: create-env
       - task: install
 
   upload:
     desc: Upload the package to PyPI
     cmds:
-      - python -m build
+      - python3 -m build
       - twine upload dist/*
 
+  build:
+    desc: Build docs, examples
+    cmds:
+      - task: examples:build
+      - task: docs:build
+
+  examples:run:
+    desc: Run geo with all examples
+    cmds:
+      - "geo examples/*.{toml,yaml}"
+
+  examples:build:
+    desc: Build files from examples/geomancy.yaml
+    cmds:
+      - "yj -yt -i < examples/geomancy.yaml > examples/geomancy.toml"
+    sources:
+      - "examples/geomancy.yaml"
+
   docs:help:
-      desc: Print the docs building help message
-      dir: docs
-      cmds:
-          - "../{{.SPHINX_BUILD}} -M help {{.SPHINX_SOURCE_DIR}} {{.SPHINX_BUILD_DIR}} {{.SPHINX_OPTS}}"
+    desc: Print the docs building help message
+    dir: docs
+    cmds:
+      - "../{{.SPHINX_BUILD}} -M help {{.SPHINX_SOURCE_DIR}} {{.SPHINX_BUILD_DIR}} {{.SPHINX_OPTS}}"
 
   docs:build:
-      desc: Build the docs
-      dir: docs
-      cmds:
-          - "../{{.SPHINX_BUILD}} -M html {{.SPHINX_SOURCE_DIR}} {{.SPHINX_BUILD_DIR}} -E -a {{.SPHINX_OPTS}}"
-      sources:
-          - "**/*.md"
-          - "**/*.rst"
-          - "_static/**"
+    desc: Build the docs (and examples)
+    dir: docs
+    cmds:
+      - "../{{.SPHINX_BUILD}} -M html {{.SPHINX_SOURCE_DIR}} {{.SPHINX_BUILD_DIR}} -E -a -W {{.SPHINX_OPTS}}"
+    sources:
+      - "**/*.md"
+      - "**/*.rst"
+      - "_static/**"
+      - "conf.py"
+      - "../README.md"
+      - "../geomancy/**/*.py"
 
   docs:clean:
-      desc: Clean the docs build directories
-      dir: docs
-      cmds:
-          - "../{{.SPHINX_BUILD}} -M clean {{.SPHINX_SOURCE_DIR}} {{.SPHINX_BUILD_DIR}} {{.SPHINX_OPTS}}"
+    desc: Clean the docs build directories
+    dir: docs
+    cmds:
+      - "../{{.SPHINX_BUILD}} -M clean {{.SPHINX_SOURCE_DIR}} {{.SPHINX_BUILD_DIR}} {{.SPHINX_OPTS}}"
 
   towncrier:cmds:
-      desc: A refresher of towncrier commands
-      silent: true
-      cmds:
-          - echo "towncrier create -c {msg} {issue}.{type}.md"
-          - echo "towncrier build [--draft] --name {{.PROJECT_NAME}}"
+    desc: A refresher of towncrier commands
+    silent: true
+    cmds:
+      - echo "towncrier create -c {msg} {issue}.{type}.md"
+      - echo "towncrier build [--draft] --name {{.PROJECT_NAME}}"
 
 # towncrier create -c "Implement towncrier" 8.docs.md
```

### Comparing `geomancy-0.9.4/docs/_static/geomancy_logo.png` & `geomancy-1.0.0/docs/_static/geomancy_logo.png`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/docs/_static/geomancy_logo.svg` & `geomancy-1.0.0/docs/_static/geomancy_logo.svg`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/docs/conf.py` & `geomancy-1.0.0/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,15 +23,21 @@
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ["myst_parser", "sphinx_design"]
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+    "myst_parser",
+    "sphinx_design",
+    "sphinx_remove_toctrees",  # Remove autosummary stubs from tocs
+]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
@@ -41,15 +47,23 @@
 myst_enable_extensions = ["colon_fence", "deflist", "fieldlist", "substitution"]
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "sphinx_book_theme"
+html_theme = "furo"
+html_title = " "
 html_logo = "_static/geomancy_logo.svg"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 html_css_files = ["custom.css"]
+
+# Other html variables (Furo)
+# https://pradyunsg.me/furo/customisation/colors/
+html_theme_options = {"light_css_variables": {"color-foreground-border": "#bfbfbf"}}
+
+# Remove the autosummary stub links from toctrees
+remove_from_toctrees = ["about/api/generated/*"]
```

### Comparing `geomancy-0.9.4/docs/index.md` & `geomancy-1.0.0/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -6,19 +6,14 @@
 :end-before: <!-- end badges -->
 ```
 ```{include} ../README.md
 :start-after: <!-- start intro -->
 :end-before: <!-- end intro -->
 ```
 
-```{include} ../README.md
-:start-after: <!-- start quickstart -->
-:end-before: <!-- end quickstart -->
-```
-
 ## Features
 
 ```{include} ../README.md
 :start-after: <!-- start features -->
 :end-before: <!-- end features -->
 ```
 
@@ -32,14 +27,33 @@
 :caption: Usage
 :maxdepth: 1
 
 usage/cmd_checks
 usage/cmd_run
 usage/format
 ```
+
+```{toctree}
+:hidden:
+:caption: Checks
+:maxdepth: 1
+
+checks/core
+checks/aws
+```
+
+```{toctree}
+:hidden:
+:caption: Guides
+:maxdepth: 1
+
+guides/tips_and_tricks
+```
+
 ```{toctree}
 :hidden:
 :caption: About the Project
 :maxdepth: 1
 
-changelog
+about/changelog
+about/api/index
 ```
```

### Comparing `geomancy-0.9.4/docs/usage/cmd_checks.md` & `geomancy-1.0.0/docs/usage/cmd_checks.md`

 * *Files 27% similar despite different names*

```diff
@@ -11,50 +11,60 @@
 
 ::::{tab-set}
 :::{tab-item} With arguments
 The following evaluates the checks listed in ``examples/geomancy.yaml``, if
 this file exists.
 ```shell
 $ geo examples/geomancy.yaml
-=========================== examples/geomancy.yaml ============================
-    checks (12 checks)
-[✔]   Environment (2 checks)
-[✔]     Check environment variable '$PATH'...passed
-[✔]     Check environment variable '$USER'...passed
-      Paths (4 checks)
-[✔]     ChecksFile (3 checks)
-[✔]       Check path 'examples/geomancy.toml'...passed
-[✔]       Check path 'examples/pyproject.toml'...passed
-[!]       Check path '.missing__.txt'...missing
-[✔]   Executables (1 checks)
-[✔]     Check executable 'python3>=3.11'...passed
-[✔]   PythonPackages (1 checks)
-[✔]     Check python package 'geomancy>=0.8'...passed
-========================= PASSED. 13 checks in 0.01s ==========================
+ [✔] examples/geomancy.yaml...passed
+ [✔]   checks...passed
+ [✔]     OperatingSystem...passed
+ [✔]       Check platform 'macOS >= 10.9'...passed
+ [!]       Check platform 'Linux >= 3.0'...wrong platform
+ [!]       Check platform 'Windows >= 10'...wrong platform
+ [✔]     Environment...passed
+ [✔]       Check environment variable '$PATH'...passed
+ [✔]       Username...passed
+ [✔]         Check environment variable '$USER'...passed
+ [!]         Check environment variable '$USERNAME'...empty string
+ [✔]     Paths...passed
+ [✔]       ChecksFile...passed
+ [✔]         Check path 'examples/geomancy.toml'...passed
+ [✔]         Check path 'examples/pyproject.toml'...passed
+ [!]         Check path '.missing__.txt'...missing
+ [✔]     Executables...passed
+ [✔]       Check executable 'python3>=3.11'...passed
+ [✔]     PythonPackages...passed
+ [✔]       Check python package 'geomancy>=0.8'...passed
 ```
 :::
 :::{tab-item} Without arguments
 When no arguments are specified, geo will search for checks in multiple locations.
 ```shell
 $ geo
-================================ geomancy.yaml ================================
-    checks (12 checks)
-[✔]   Environment (2 checks)
-[✔]     Check environment variable '$PATH'...passed
-[✔]     Check environment variable '$USER'...passed
-      Paths (4 checks)
-[✔]     ChecksFile (3 checks)
-[✔]       Check path 'examples/geomancy.toml'...passed
-[✔]       Check path 'examples/pyproject.toml'...passed
-[!]       Check path '.missing__.txt'...missing
-[✔]   Executables (1 checks)
-[✔]     Check executable 'python3>=3.11'...passed
-[✔]   PythonPackages (1 checks)
-[✔]     Check python package 'geomancy>=0.8'...passed
-========================= PASSED. 13 checks in 0.01s ==========================
+ [✔] examples/geomancy.yaml...passed
+ [✔]   checks...passed
+ [✔]     OperatingSystem...passed
+ [✔]       Check platform 'macOS >= 10.9'...passed
+ [!]       Check platform 'Linux >= 3.0'...wrong platform
+ [!]       Check platform 'Windows >= 10'...wrong platform
+ [✔]     Environment...passed
+ [✔]       Check environment variable '$PATH'...passed
+ [✔]       Username...passed
+ [✔]         Check environment variable '$USER'...passed
+ [!]         Check environment variable '$USERNAME'...empty string
+ [✔]     Paths...passed
+ [✔]       ChecksFile...passed
+ [✔]         Check path 'examples/geomancy.toml'...passed
+ [✔]         Check path 'examples/pyproject.toml'...passed
+ [!]         Check path '.missing__.txt'...missing
+ [✔]     Executables...passed
+ [✔]       Check executable 'python3>=3.11'...passed
+ [✔]     PythonPackages...passed
+ [✔]       Check python package 'geomancy>=0.8'...passed
 ```
 :::
 ::::
 
 If no checks files are listed as arguments, geo will search the following file
 locations in the current directory, and it wil run all the checks in existing
 files: ``.geomancy.yaml``, ``.geomancy.yml``, ``.geomancy.toml``,
@@ -262,7 +272,39 @@
    ${MYVAR+replaced}   # -> replaced
    ${MYVAR:+replaced}  # -> replaced
    $MYVAR+replaced     # -> replaced
    $MYVAR:+replaced    # -> replaced
    ${MISSING+replaced} # ""
    ${MISSING+replaced} # ""
    ```
+
+## Other Options
+
+The following are options available to ``geo`` and``geo check``.
+
+`-e`/`--env`
+: Environment variable file(s) to load for checks
+
+`--overwrite`
+: Overwrite existing environment variables with those listed in environment
+  variable files. This option requires environment variable files to be
+  specified with `-e`/`--env`
+
+`-f`/`--fixture`
+: Load a fixture file (yaml format) for mocking network requests. If the
+  fixture does not exist, it will be created. This option is helpful for
+  testing checks files when checks require authentication.
+
+  :::{dropdown} Example
+  The following command runs the AWS checks in ``examples/aws/geomancy.yaml``,
+  which require proper authentication of the AWS client. To bypass network
+  requests, a fixture can be loaded to test this example.
+
+  ```shell
+  $ geo --fixture examples/aws/fixtures.yaml examples/aws/geomancy.yaml
+   [✔] examples/aws/geomancy.yaml...passed
+   [✔]   checks...passed
+   [✔]     CloudFormationTemplateS3...passed
+   [✔]       Check AWS S3 bucket access 'myproject-cfn-templates'......passed
+   [✔]       Check AWS S3 bucket private 'myproject-cfn-templates'......passed
+  ```
+  :::
```

### Comparing `geomancy-0.9.4/docs/usage/cmd_run.md` & `geomancy-1.0.0/docs/usage/cmd_run.md`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/examples/geomancy.toml` & `geomancy-1.0.0/examples/geomancy.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,59 @@
 [config]
-# see `geo --config` for all options
-VERSION='0.1.0a'
-
   [config.CHECKBASE]
-  ENV_SUBSTITUTE_DEFAULT=true
-
-[checks.Environment]
-desc = "Check environment variables common to all development environments"
+    env_substitute = true
 
+[checks]
+  [checks.OperatingSystem]
+    desc = "Check the minimum operating system versions"
+    subchecks = "any"
+    [checks.OperatingSystem.checkMacOS]
+      desc = "MacOS 10.9 or later (released 2013)"
+      checkOS = "macOS >= 10.9"
+    [checks.OperatingSystem.checkLinuxOS]
+      desc = "Linux 4.0 or later (released 2015)"
+      checkOS = "Linux >= 3.0"
+    [checks.OperatingSystem.checkWindows]
+      desc = "Windows 10 or later (released 2015)"
+      checkOS = "Windows >= 10"
+  [checks.Environment]
+    desc = "Check environment variables common to all development environments"
     [checks.Environment.Path]
-    desc = "Paths to search for executables"
-    checkEnv = "$PATH"
-
+      decs = "Paths to search for executables"
+      checkEnv = "$PATH"
     [checks.Environment.Username]
-    subchecks = "any"
-
-        [checks.Environment.Username.UnixUsername]  # linux and macOS
+      subchecks = "any"
+      [checks.Environment.Username.UnixUsername]
         desc = "The current username"
         checkEnv = "$USER"
         regex = "[a-z_][a-z0-9_-]*[$]?"
-
-        [checks.Environment.Username.WindowsUsername]  # windows
+      [checks.Environment.Username.WindowsUsername]
         desc = "The current username"
         checkEnv = "$USERNAME"
         regex = "[a-z_][a-z0-9_-]*[$]?"
-
-[checks.Paths]
-desc = "Checks the existence of needed files and directories"
-
+  [checks.Paths]
+    desc = "Checks the existence of needed files and directories"
     [checks.Paths.ChecksFile]
-    desc = "Checks that at least one checks file exists"
-    subchecks = "any"
-
-        [checks.Paths.ChecksFile.Geomancy]
-        desc = "Check for 'geomancy.toml' file"
+      desc = "Checks that at least one checks file exists"
+      subchecks = "any"
+      [checks.Paths.ChecksFile.Geomancy]
+        desc = "Check for the 'geomancy.toml' file"
         checkPath = "examples/geomancy.toml"
         type = "file"
-
-        [checks.Paths.ChecksFile.Pyproject]
+      [checks.Paths.ChecksFile.Pyproject]
         desc = "Check for 'pyproject.toml' file"
         checkPath = "examples/pyproject.toml"
         type = "file"
-
-        [checks.Paths.ChecksFile.missing]
+      [checks.Paths.ChecksFile.missing]
         desc = "Check a missing file"
         checkPath = ".missing__.txt"
         type = "file"
-
-[checks.Executables]
-desc = "Check the availability of commands and their versions"
-
+  [checks.Executables]
+    desc = "Check the availability of commands and their versions"
     [checks.Executables.Python]
-    desc = "Python interpreter"
-    checkExec = "python3>=3.11"
-
-[checks.PythonPackages]
-desc = "Check the presence and, optional, the version of python packages"
-
-    [checks.PythonPackages.geomancy]
-    desc = "Geomancy python package"
-    checkPythonPkg = "geomancy>=0.1"
-
+      desc = "Python interpreter"
+      checkExec = "python3>=3.11"
+  [checks.PythonPackages]
+    desc = "Check the presence and, optional, the version of python packages"
+    [checks.PythonPackages.Geomancy]
+      desc = "Geomancy python package"
+      checkPythonPkg = "geomancy>=0.8"
```

### Comparing `geomancy-0.9.4/examples/geomancy.yaml` & `geomancy-1.0.0/examples/geomancy.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/geomancy/checks/env.py` & `geomancy-1.0.0/geomancy/checks/env.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 """
 Checks for environment variables
 """
 import typing as t
 import re
 
-from .base import CheckBase, CheckResult
+from .base import Check, Result, Executor
 from ..environment import sub_env
 from ..config import Parameter
 
 
-class CheckEnv(CheckBase):
+class CheckEnv(Check):
     """Check the current environment variables."""
 
-    # (Optional) regex to match the environment variable value
+    #: (Optional) regex to match the environment variable value
     regex: t.Optional[t.Tuple[str, ...]] = None
 
-    # The message for checking environment variables
     msg = Parameter(
         "CHECKENV.MSG",
-        default="Check environment variable '{check.raw_value}'...",
+        default="Check environment variable '{check.raw_value}'",
     )
 
-    # Alternative names for the class
     aliases = ("checkEnv",)
 
     def __init__(self, *args, regex: t.Optional[str] = None, **kwargs):
         super().__init__(*args, **kwargs)
         self.regex = regex
 
-    def check(self, level: int = 0) -> CheckResult:
+    def check(self, executor: t.Optional[Executor] = None, level: int = 0) -> Result:
         """Check the environment variable value."""
         # Substitute environment variables, if needed
         value = sub_env(self.raw_value) if self.raw_value is not None else None
-        passed = False
 
         if value is None:
             # If the value is None, the environment variable doesn't exist.
             status = "missing"
         elif value == "":
             # An empty string environment variable is considered not set
             status = "empty string"
         elif isinstance(self.regex, str) and re.match(self.regex, value) is None:
             # Check the regex, if specified
             status = f"does not match regex '{self.regex}'"
         else:
             # All checks passed!
             status = "passed"
-            passed = True
 
         msg = self.msg.format(check=self, status=status)
-        return CheckResult(passed=passed, msg=msg, status=status)
+        return Result(msg=msg, status=status)
```

### Comparing `geomancy-0.9.4/geomancy/checks/exec.py` & `geomancy-1.0.0/geomancy/checks/exec.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,25 +11,23 @@
 
 __all__ = ("CheckExec",)
 
 
 class CheckExec(CheckVersion):
     """Check for the presence and version of executables"""
 
-    # The executable may exist and be installed, but get_current_version
-    # may not be able to identify the current version
+    #: The executable may exist and be installed, but get_current_version
+    #: may not be able to identify the current version
     require_current_version = False
 
-    # The message for checking executables
     msg = Parameter(
         "CHECKEXEC.MSG",
-        default="Check executable '{check.raw_value}'...",
+        default="Check executable '{check.raw_value}'",
     )
 
-    # Alternative names for the class
     aliases = ("checkExec",)
 
     @property
     def value(
         self,
     ) -> t.Tuple[
         t.Union[str, None], t.Union[t.Callable, None], t.Union[t.Tuple[int], None]
```

### Comparing `geomancy-0.9.4/geomancy/checks/path.py` & `geomancy-1.0.0/geomancy/checks/path.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 """
 Checks for paths
 """
 import typing as t
 from pathlib import Path
 
-from .base import CheckBase, CheckException, CheckResult
+from .base import Check, Result, CheckException, Executor
 from ..config import Parameter
 
+__all__ = ("CheckPath",)
 
-class CheckPath(CheckBase):
+
+class CheckPath(Check):
     """Check paths for valid files and directories"""
 
-    # (Optional) the type of path expected
+    #: (Optional) the type of path expected
     type: t.Optional[str] = None
 
-    # The valid values of path types
+    #: The valid values of path types
     type_options = (None, "dir", "file")
 
-    # The message for checking environment variables
-    msg = Parameter("CHECKPATH.MSG", default="Check path '{check.value}'...")
+    msg = Parameter("CHECKPATH.MSG", default="Check path '{check.value}'")
 
-    # Alternative names for the class
     aliases = ("checkPath",)
 
     def __init__(self, *args, type: t.Optional[str] = None, **kwargs):
         super().__init__(*args, **kwargs)
         if type not in self.type_options:
             raise CheckException(
                 f"Path type '{type}' must be one of: "
                 f"{tuple(opt for opt in self.type_options if opt is not None)}"
             )
         self.type = type
 
-    def check(self, level: int = 0) -> CheckResult:
+    def check(self, executor: t.Optional[Executor] = None, level: int = 0) -> Result:
         """Check paths"""
-        passed = False
         value = self.value
         path = Path(value)
 
         if not path.exists():
             status = "missing"
         elif self.type == "dir" and not path.is_dir():
             status = "not dir"
         elif self.type == "file" and not path.is_file():
             status = "not file"
         else:
             status = "passed"
-            passed = True
 
         msg = self.msg.format(check=self, status=status)
-        return CheckResult(passed=passed, msg=msg, status=status)
+        return Result(msg=msg, status=status)
```

### Comparing `geomancy-0.9.4/geomancy/checks/platform.py` & `geomancy-1.0.0/geomancy/checks/platform.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Checks the platform (Operating System) and its version
 """
 import typing as t
 import platform
 import logging
 
-from .base import CheckResult
+from .base import Result, Executor
 from .version import CheckVersion
 from .utils import version_to_tuple
 from ..config import Parameter
 
 __all__ = ("CheckPlatform",)
 
 logger = logging.getLogger(__name__)
@@ -17,15 +17,15 @@
 
 class CheckPlatform(CheckVersion):
     """Check the availability and version of a python package"""
 
     # The message for checking python packages
     msg = Parameter(
         "CHECKPLATFORM.MSG",
-        default="Check platform '{check.raw_value}'...",
+        default="Check platform '{check.raw_value}'",
     )
 
     aliases = ("checkOS", "checkPlatform")
 
     def get_current_platform(self) -> str:
         """Retrieve the OS platform name"""
         uname = platform.uname()
@@ -56,19 +56,21 @@
             current_version = None
 
         logger.debug(
             f"current_platform: {current_platform}, current_version: {current_version}"
         )
         return current_version
 
-    def check(self, level: int = 0) -> CheckResult:
+    def check(self, executor: t.Optional[Executor] = None, level: int = 0) -> Result:
         """Check whether the OS matches and the version"""
+        msg = self.msg.format(check=self)
+
         # Get the OS name checked against
         name, op, version = self.value
         current_platform = self.get_current_platform()
 
         if current_platform.lower() != name.lower():
             # Failed check if the platform doesn't match this check
-            return CheckResult(passed=False, msg=self.msg, status="wrong platform")
+            return Result(msg=msg, status="wrong platform")
 
         # Check the version, as usual
         return super().check(level=level)
```

### Comparing `geomancy-0.9.4/geomancy/checks/python.py` & `geomancy-1.0.0/geomancy/checks/python.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class CheckPythonPackage(CheckVersion):
     """Check the availability and version of a python package"""
 
     # The message for checking python packages
     msg = Parameter(
         "CHECKPYTHONPACKAGE.MSG",
-        default="Check python package '{check.raw_value}'...",
+        default="Check python package '{check.raw_value}'",
     )
 
     aliases = ("checkPythonPackage", "checkPythonPkg", "CheckPythonPkg")
 
     def get_current_version(self) -> t.Union[None, t.Tuple[int]]:
         # Get the package name, operator and version to check against (the last
         # 2 aren't used here)
```

### Comparing `geomancy-0.9.4/geomancy/checks/utils.py` & `geomancy-1.0.0/geomancy/checks/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utility functions"""
 import typing as t
 import operator
 import re
 
-__all__ = ("all_subclasses", "version_to_tuple", "name_and_version")
+__all__ = ("all_subclasses", "pop_first", "version_to_tuple", "name_and_version")
 
 __missing__ = object()  # used an argument for missing values
 
 
 def all_subclasses(cls) -> t.List[t.Type]:
     """Retrieve all subclasses, sub-subclasses and so on for a class
```

### Comparing `geomancy-0.9.4/geomancy/checks/version.py` & `geomancy-1.0.0/geomancy/checks/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 """Check abstract base class for checks that include versions"""
 import typing as t
 from abc import abstractmethod
 
-from .base import CheckBase, CheckResult
+from .base import Check, Result, Executor
 from .utils import name_and_version
 
 __all__ = ("CheckVersion",)
 
 
-class CheckVersion(CheckBase):
+class CheckVersion(Check):
     """An abstract Check for package and program versions"""
 
-    # If true, the result of get_current_version must not be None
-    # Set to True if get_current_version should return a version if the command
-    # or package exists
-    # Set to False if get_current_version may not be able to return the
-    # version, even if the command or package is installed or present
+    #: If true, the result of get_current_version must not be None
+    #: Set to True if get_current_version should return a version if the command
+    #: or package exists
+    #: Set to False if get_current_version may not be able to return the
+    #: version, even if the command or package is installed or present
     require_current_version: bool = True
 
     @property
     def value(
         self,
     ) -> t.Tuple[
         t.Union[str, None], t.Union[t.Callable, None], t.Union[t.Tuple[int], None]
     ]:
         """Get the package name, comparison operator and version tuple."""
-        value = CheckBase.value.fget(self)
+        value = Check.value.fget(self)
         name, op, version = name_and_version(value)
         return name, op, version
 
     @value.setter
     def value(self, v):
-        CheckBase.value.fset(self, v)
+        Check.value.fset(self, v)
 
     @abstractmethod
     def get_current_version(self) -> t.Union[None, t.Tuple[int]]:
         """Get the current version as a tuple of integers, or None if it can't
         be found."""
         return None
 
-    def check(self, level: int = 0) -> CheckResult:
+    def check(self, executor: t.Optional[Executor] = None, level: int = 0) -> Result:
         """Check whether the current version is compatible with the version
         specified in the value."""
         name, op, version = self.value
         current_version = self.get_current_version()
-        passed = False
 
         if name is None:
             status = "missing"
         elif self.require_current_version and current_version is None:
             status = "missing"
         else:
             if version is not None and current_version is None:
@@ -58,12 +57,9 @@
                 and current_version is not None
                 and op is not None
                 and not op(current_version, version)
             ):
                 status = f"incorrect version=" f"{'.'.join(map(str, current_version))}"
             else:
                 status = "passed"
-                passed = True
 
-        return CheckResult(
-            passed=passed, msg=self.msg.format(check=self), status=status
-        )
+        return Result(msg=self.msg.format(check=self), status=status)
```

### Comparing `geomancy-0.9.4/geomancy/config/config.py` & `geomancy-1.0.0/geomancy/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,24 @@
 
     Notes
     -----
     The base class is deliberately modified dynamically with descriptors. This
     is because the Config was designed to be configured on the fly.
     """
 
-    # The root singleton instance
+    #: The root singleton instance
     _instance: t.Optional["Config"] = None
 
-    # The thread lock
+    #: The thread lock
     _lock: Lock = Lock()
 
-    # The regex to validate key names
+    #: The regex to validate key names
     key_regex = re.compile(r"^[_A-Za-z][_A-Za-z0-9]*$")
 
-    # Different names for subsections in a dict which could contain config settings
+    #: Different names for subsections in a dict which could contain config settings
     section_aliases = ("config", "Config")
 
     def __new__(cls, root: bool = True):
         # Create the singleton instance if it hasn't been created
         if cls._instance is None:
             # Lock the thread
             with cls._lock:
@@ -373,21 +373,21 @@
     is because the descriptor will be replaced if its corresponding class
     attribute is modified with a new value. Stated another way, the __set__
     method is not called from a class--only instances of a class.
     """
 
     __slots__ = ("key", "_config")
 
-    # The key/name of the parameter in the Config
+    #: The key/name of the parameter in the Config
     key: str
 
-    # The delimiter used for splitting keys
+    #: The delimiter used for splitting keys
     delim: str = "."
 
-    # A reference to the Config() singleton
+    #: A reference to the Config() singleton
     _config: Config
 
     def __init__(self, key, default=missing):
         self.key = key
         self._config = Config()
 
         # Set the default, if specified
```

### Comparing `geomancy-0.9.4/geomancy/entrypoints/config.py` & `geomancy-1.0.0/geomancy/entrypoints/config.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/geomancy/entrypoints/environment.py` & `geomancy-1.0.0/geomancy/entrypoints/environment.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/geomancy/entrypoints/geo.py` & `geomancy-1.0.0/geomancy/entrypoints/geo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """The geo CLI entrypoint"""
 import logging
+import os
 from pathlib import Path
 
 import click
 from click_default_group import DefaultGroup
 
 from .check import check
 from .run import run
@@ -20,15 +21,15 @@
     if not value or context.resilient_parsing:
         return
     click.echo(get_version())
     context.exit()
 
 
 @click.group(
-    cls=DefaultGroup, default="check", default_if_no_args=False, help=description
+    cls=DefaultGroup, default="check", default_if_no_args=True, help=description
 )
 @click.option("--debug", "-d", is_flag=True, help="Enable debugging information")
 @click.option(
     "--version",
     "-V",
     is_flag=True,
     is_eager=True,
@@ -38,15 +39,15 @@
 )
 @click.option("--disable-color", is_flag=True, help="Disable terminal coloring")
 @click.pass_context
 def geo_cli(ctx, debug, disable_color):
     """The main entrypoint for the 'geo' CLI"""
     # Disable coloring, if specified
     if disable_color:
-        ctx.color = False
+        os.environ["NO_COLOR"] = "TRUE"
 
     # Setup logging
     logging.basicConfig(
         level=logging.DEBUG if debug else None,
         format="%(levelname)s:%(name)s: %(message)s",
     )
```

### Comparing `geomancy-0.9.4/geomancy/entrypoints/utils.py` & `geomancy-1.0.0/geomancy/entrypoints/utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/geomancy/environment/dotenv.py` & `geomancy-1.0.0/geomancy/environment/dotenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,61 +6,61 @@
 import logging
 from pathlib import Path
 
 __all__ = ("sub_env", "parse_env", "load_env")
 
 logger = logging.getLogger(__name__)
 
-# Regex to match environment variables for subsitution--e.g. ${NAME} or $NAME
+#: Regex to match environment variables for subsitution--e.g. ${NAME} or $NAME
 sub_re = re.compile(
     r"[$]"  # Start with a '$'. e.g. $NAME
     r"((?P<name_nobrace>[a-zA-Z_][a-zA-Z0-9_:\-?+]*)|"  # e.g. $NAME
     r" \{(?P<name_brace>[a-zA-Z_][a-zA-Z0-9_\s:\-?+]*)\})",  # e.g ${NAME}
     re.VERBOSE,
 )
 
-# Regex to identify alternate variables from variable names
-# e.g. ${NAME:-default}
+#: Regex to identify alternate variables from variable names
+#: e.g. ${NAME:-default}
 sub_alt_re = re.compile(
     # Does not require a brace. e.g. $NAME
     r"(?P<name>[a-zA-Z_][a-zA-Z0-9_]*)"
     # May have an alternative descriptor
     r"((?P<default>:-|-)|(?P<error>:\?|\?)|(?P<replace>:\+|\+))?(?P<alt>[\w\s]*)",
     re.VERBOSE,
 )
 
-# Regex to match environment variable names
+#: Regex to match environment variable names
 env_name = r"(?P<name>[a-zA-Z_][a-zA-Z0-9_]*)"  # env variable name
 env_name_re = re.compile(env_name)
 
-# Regex to match environment variable values with substitution
+#: Regex to match environment variable values with substitution
 env_value = (
     # Quoted value--e.g. "My $VAR" or 'My $VAR'--allowing for escaped quotes
     r"""((?P<quote>["|']{1,3})(?P<qvalue>(?:\\.|[^"'\\])+)(?P=quote)[^'"\n]*|"""
     # Unquoted value--e.g. My $VAR
     r"""(?P<value>[^'"\n]+))"""
 )
 env_value_re = re.compile(
     env_value,
     re.MULTILINE | re.DOTALL,
 )
 
-# Regex to match "name=value" pairs from an env file
+#: Regex to match "name=value" pairs from an env file
 env_name_value_re = re.compile(
     r"^\s*{env_name}\s*=\s*{env_value}\s*$".format(
         env_name=env_name, env_value=env_value
     ),
     re.MULTILINE | re.DOTALL,
 )
 
-# Regex to strip comments to the end of a line--# and not escaped values, \#
+#: Regex to strip comments to the end of a line--# and not escaped values, \#
 comment_re = re.compile(r"(^|\s+)(#.+)$")
 
-# Regex to strip backslashes from escaped quotes.
-# e.g. r"Let\'s go" -> r"Let's go"
+#: Regex to strip backslashes from escaped quotes.
+#: e.g. r"Let\'s go" -> r"Let's go"
 escaped_quote_re = re.compile(r"\\(['\"])")
 
 
 def sub_env(
     string: str, missing_default: str = "", strip_values: bool = True, **kwargs
 ) -> str:
     """Try to substitute environment variables in the string.
@@ -75,27 +75,28 @@
         Remove whitespace at the start and end of non-quoted values
     kwargs
         In addition to os.environ, search the given kwargs for matches.
 
     Raises
     ------
     EnvironmentError
-        Raised if an environment variable was not found and the :?/? error
-        error is specified
-        e.g. ${MISSING?not found!}
+        Raised if an environment variable was not found and the ``:?``/``?``
+        error directive was specified
+        e.g. ``${MISSING?not found!}``
 
     Returns
     -------
     substituted_str
         The string with environment variables substituted
 
     Notes
     -----
     This function follows the docker compose_ format.
-    - Environment variable names are preceded with a '$' character and may
+
+    - Environment variable names are preceded with a ``$`` character and may
       include braces. e.g. ``$VAR_NAME`` or ``${VAR_NAME}``
     - Environment variables names may include directives for default values
       (``${MISSING-default}``), errors for missing values (``${missing?error``)
       or replacement values (``${MISSING+replace}``)
 
     .. _compose: https://docs.docker.com/compose/environment-variables/env-file/
     """
```

### Comparing `geomancy-0.9.4/geomancy.egg-info/SOURCES.txt` & `geomancy-1.0.0/geomancy.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 .editorconfig
+.geomancy.yaml
 .gitignore
 .readthedocs.yaml
 LICENSE
 README.md
 Taskfile.yaml
 pyproject.toml
+.github/workflows/publish-to-pypi.yml
 .github/workflows/tests.yml
 changelog/changelog_template.jinja
-docs/changelog.md
 docs/conf.py
 docs/index.md
 docs/quickstart.md
 docs/_static/custom.css
 docs/_static/geomancy_logo.png
 docs/_static/geomancy_logo.svg
+docs/about/changelog.md
+docs/about/api/index.rst
+docs/checks/aws.md
+docs/checks/core.md
+docs/checks/snippets/base_args.md
+docs/guides/tips_and_tricks.md
 docs/usage/cmd_checks.md
 docs/usage/cmd_run.md
 docs/usage/format.md
 examples/geomancy.toml
 examples/geomancy.yaml
-examples/geomancy_flat.yaml
 examples/pyproject.toml
+examples/aws/fixtures.yaml
+examples/aws/geomancy.yaml
 geomancy/__description__.txt
 geomancy/__init__.py
 geomancy.egg-info/PKG-INFO
 geomancy.egg-info/SOURCES.txt
 geomancy.egg-info/dependency_links.txt
 geomancy.egg-info/entry_points.txt
 geomancy.egg-info/requires.txt
@@ -34,16 +42,16 @@
 geomancy/checks/env.py
 geomancy/checks/exec.py
 geomancy/checks/path.py
 geomancy/checks/platform.py
 geomancy/checks/python.py
 geomancy/checks/utils.py
 geomancy/checks/version.py
-geomancy/cli/__init__.py
-geomancy/cli/term.py
+geomancy/checks/aws/__init__.py
+geomancy/checks/aws/s3.py
 geomancy/config/__init__.py
 geomancy/config/config.py
 geomancy/entrypoints/__init__.py
 geomancy/entrypoints/check.py
 geomancy/entrypoints/config.py
 geomancy/entrypoints/environment.py
 geomancy/entrypoints/geo.py
@@ -54,12 +62,19 @@
 tests/conftest.py
 tests/checks/test_base.py
 tests/checks/test_env.py
 tests/checks/test_exec.py
 tests/checks/test_path.py
 tests/checks/test_platform.py
 tests/checks/test_python.py
+tests/checks/aws/test_s3.py
+tests/checks/aws/cassettes/test_s3/test_check_aws_s3_forbidden.yaml
+tests/checks/aws/cassettes/test_s3/test_check_aws_s3_missing.yaml
+tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_acl.yaml
+tests/checks/aws/cassettes/test_s3/test_check_aws_s3_public_policy.yaml
+tests/checks/aws/cassettes/test_s3/test_check_aws_s3_valid.yaml
+tests/checks/aws/cassettes/test_s3/test_check_aws_s3_without_public_access_block.yaml
 tests/config/config1.toml
 tests/config/test_config.py
 tests/data/test.env
 tests/entrypoints/test_geo.py
 tests/environment/test_dotenv.py
```

### Comparing `geomancy-0.9.4/tests/checks/test_env.py` & `geomancy-1.0.0/tests/checks/test_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,12 +70,12 @@
         # The regex should not match
         check2 = CheckEnv(name="regex2", value=f"${variable_name}", regex=regex)
         assert not check2.check().passed
 
 
 def test_check_base_types_dict():
     """Test the CheckBase.types_dict() method for the CheckEnv class."""
-    types = CheckEnv.types_dict()
+    types = CheckEnv.types()
 
     # Verify CheckEnv entries and aliases
     assert types["CheckEnv"] == CheckEnv
     assert types["checkEnv"] == CheckEnv
```

### Comparing `geomancy-0.9.4/tests/checks/test_exec.py` & `geomancy-1.0.0/tests/checks/test_exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/tests/checks/test_path.py` & `geomancy-1.0.0/tests/checks/test_path.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/tests/checks/test_platform.py` & `geomancy-1.0.0/tests/checks/test_platform.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/tests/checks/test_python.py` & `geomancy-1.0.0/tests/checks/test_python.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/tests/config/test_config.py` & `geomancy-1.0.0/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.4/tests/entrypoints/test_geo.py` & `geomancy-1.0.0/tests/entrypoints/test_geo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Test the main CLI entrypoint"""
 import typing as t
 from pathlib import Path
-from itertools import chain
 import os
 
 from click.testing import CliRunner
 import pytest
 
 from geomancy.entrypoints import geo_cli
 from geomancy.config import Config
 
 
 def get_checks_files():
-    """Return a list of checks files to check"""
+    """Return a list of checks files to check in the root examples/"""
     checks_files = []
 
     # examples/
     for ext in ("toml", "yaml"):
         checks_files += list(Path("examples").glob(f"*.{ext}"))
 
     return checks_files
@@ -71,14 +70,25 @@
 
     # Check, for example, that environment variables were checked
     assert any(
         msg in result.output for msg in ("Check environment variable", "Check path")
     )
 
 
+@pytest.mark.parametrize(
+    "checks_file,fixture",
+    (("examples/aws/geomancy.yaml", "examples/aws/fixtures.yaml"),),
+)
+def test_cli_check_fixtures(run, checks_file, fixture):
+    """Test the CLI with checks that require network access and therefore use
+    fixtures."""
+    # Run the command and test that an 0 error code was received
+    result = run(("--fixture", fixture, checks_file))
+
+
 @pytest.mark.parametrize("flag", ("", "--toml", "--yaml"))
 def test_cli_config(run, flag):
     """Test the --config option"""
     if flag:
         result = run(("config", flag))
     else:
         result = run(("config",))
```

### Comparing `geomancy-0.9.4/tests/environment/test_dotenv.py` & `geomancy-1.0.0/tests/environment/test_dotenv.py`

 * *Files identical despite different names*

