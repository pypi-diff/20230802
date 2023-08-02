# Comparing `tmp/conda-project-0.2.0.tar.gz` & `tmp/conda-project-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda-project-0.2.0.tar", last modified: Mon Apr 24 21:41:53 2023, max compression
+gzip compressed data, was "conda-project-0.2.1.tar", last modified: Wed Aug  2 14:35:34 2023, max compression
```

## Comparing `conda-project-0.2.0.tar` & `conda-project-0.2.1.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.586355 conda-project-0.2.0/
--rw-r--r--   0 adefusco   (502) staff       (20)      136 2023-04-05 14:24:50.000000 conda-project-0.2.0/.flake8
--rw-r--r--   0 adefusco   (502) staff       (20)       58 2022-04-01 15:52:07.000000 conda-project-0.2.0/.gitattributes
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.567293 conda-project-0.2.0/.github/
--rw-r--r--   0 adefusco   (502) staff       (20)       71 2022-04-14 22:10:46.000000 conda-project-0.2.0/.github/disclaimer.txt
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.567885 conda-project-0.2.0/.github/workflows/
--rw-r--r--   0 adefusco   (502) staff       (20)     1163 2022-12-06 15:55:00.000000 conda-project-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 adefusco   (502) staff       (20)     5597 2023-04-24 21:40:33.000000 conda-project-0.2.0/.github/workflows/main.yaml
--rw-r--r--   0 adefusco   (502) staff       (20)     1913 2023-04-06 01:03:58.000000 conda-project-0.2.0/.gitignore
--rw-r--r--   0 adefusco   (502) staff       (20)      999 2023-04-05 20:34:59.000000 conda-project-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 adefusco   (502) staff       (20)     1111 2023-04-24 21:40:33.000000 conda-project-0.2.0/CHANGELOG.md
--rw-r--r--   0 adefusco   (502) staff       (20)     1544 2022-04-01 15:50:48.000000 conda-project-0.2.0/LICENSE
--rw-r--r--   0 adefusco   (502) staff       (20)     6180 2023-04-24 21:41:53.586156 conda-project-0.2.0/PKG-INFO
--rw-r--r--   0 adefusco   (502) staff       (20)     4751 2023-04-24 21:40:33.000000 conda-project-0.2.0/README.md
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.568056 conda-project-0.2.0/conda.recipe/
--rw-r--r--   0 adefusco   (502) staff       (20)     1154 2023-04-24 21:40:33.000000 conda-project-0.2.0/conda.recipe/meta.yaml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.568518 conda-project-0.2.0/docs/
--rw-r--r--   0 adefusco   (502) staff       (20)     1759 2023-04-06 01:03:58.000000 conda-project-0.2.0/docs/Makefile
--rw-r--r--   0 adefusco   (502) staff       (20)      112 2022-12-06 15:55:00.000000 conda-project-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.570545 conda-project-0.2.0/docs/source/
--rw-r--r--   0 adefusco   (502) staff       (20)     1771 2023-04-06 01:03:58.000000 conda-project-0.2.0/docs/source/conf.py
--rw-r--r--   0 adefusco   (502) staff       (20)     4022 2023-04-24 21:40:33.000000 conda-project-0.2.0/docs/source/experimental.md
--rw-r--r--   0 adefusco   (502) staff       (20)      151 2023-04-24 21:40:33.000000 conda-project-0.2.0/docs/source/index.md
--rw-r--r--   0 adefusco   (502) staff       (20)     1636 2023-03-28 16:19:13.000000 conda-project-0.2.0/docs/source/setup_for_development.md
--rw-r--r--   0 adefusco   (502) staff       (20)     5873 2023-03-30 21:40:52.000000 conda-project-0.2.0/docs/source/tutorial.md
--rw-r--r--   0 adefusco   (502) staff       (20)    12563 2023-03-30 21:40:52.000000 conda-project-0.2.0/docs/source/user_guide.md
--rw-r--r--   0 adefusco   (502) staff       (20)      259 2023-04-24 21:40:33.000000 conda-project-0.2.0/environment.yml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.571349 conda-project-0.2.0/etc/
--rw-r--r--   0 adefusco   (502) staff       (20)      102 2023-04-05 14:24:50.000000 conda-project-0.2.0/etc/build-environment.yml
--rw-r--r--   0 adefusco   (502) staff       (20)      263 2023-04-24 21:40:33.000000 conda-project-0.2.0/etc/test-environment.yml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.571753 conda-project-0.2.0/examples/
--rw-r--r--   0 adefusco   (502) staff       (20)       95 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/.gitignore
--rw-r--r--   0 adefusco   (502) staff       (20)      621 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/README.md
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.573179 conda-project-0.2.0/examples/cmds-and-vars/
--rw-r--r--   0 adefusco   (502) staff       (20)     1959 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/cmds-and-vars/README.md
--rw-r--r--   0 adefusco   (502) staff       (20)    22470 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/cmds-and-vars/conda-lock.default.yml
--rw-r--r--   0 adefusco   (502) staff       (20)      317 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/cmds-and-vars/conda-project.yml
--rw-r--r--   0 adefusco   (502) staff       (20)       54 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/cmds-and-vars/environment.yml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.573787 conda-project-0.2.0/examples/condarc-settings/
--rw-r--r--   0 adefusco   (502) staff       (20)       16 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/condarc-settings/.condarc
--rw-r--r--   0 adefusco   (502) staff       (20)      389 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/condarc-settings/README.md
--rw-r--r--   0 adefusco   (502) staff       (20)       92 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/condarc-settings/environment.yml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.574322 conda-project-0.2.0/examples/env-file-only/
--rw-r--r--   0 adefusco   (502) staff       (20)     1434 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/env-file-only/README.md
--rw-r--r--   0 adefusco   (502) staff       (20)       40 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/env-file-only/environment.yml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.576299 conda-project-0.2.0/examples/multi-env-files/
--rw-r--r--   0 adefusco   (502) staff       (20)     2971 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/README.md
--rw-r--r--   0 adefusco   (502) staff       (20)    22470 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/conda-lock.default.yml
--rw-r--r--   0 adefusco   (502) staff       (20)    33992 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/conda-lock.test.yml
--rw-r--r--   0 adefusco   (502) staff       (20)      117 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/conda-project.yml
--rw-r--r--   0 adefusco   (502) staff       (20)       54 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/environment.yml
--rw-r--r--   0 adefusco   (502) staff       (20)       49 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/extras.yml
--rw-r--r--   0 adefusco   (502) staff       (20)      299 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/print_version.py
--rw-r--r--   0 adefusco   (502) staff       (20)      195 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/test_get_version.py
--rw-r--r--   0 adefusco   (502) staff       (20)     3120 2023-04-24 21:40:33.000000 conda-project-0.2.0/pyproject.toml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.576520 conda-project-0.2.0/scripts/
--rw-r--r--   0 adefusco   (502) staff       (20)     6189 2023-04-24 21:40:33.000000 conda-project-0.2.0/scripts/ap-to-cp.py
--rw-r--r--   0 adefusco   (502) staff       (20)       38 2023-04-24 21:41:53.586422 conda-project-0.2.0/setup.cfg
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.564498 conda-project-0.2.0/src/
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.579357 conda-project-0.2.0/src/conda_project/
--rw-r--r--   0 adefusco   (502) staff       (20)      303 2023-04-06 01:03:58.000000 conda-project-0.2.0/src/conda_project/__init__.py
--rw-r--r--   0 adefusco   (502) staff       (20)      134 2023-04-05 14:24:50.000000 conda-project-0.2.0/src/conda_project/__main__.py
--rw-r--r--   0 adefusco   (502) staff       (20)      160 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project/_version.py
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.581736 conda-project-0.2.0/src/conda_project/cli/
--rw-r--r--   0 adefusco   (502) staff       (20)       99 2023-04-05 14:24:50.000000 conda-project-0.2.0/src/conda_project/cli/__init__.py
--rw-r--r--   0 adefusco   (502) staff       (20)     4687 2023-04-24 21:40:33.000000 conda-project-0.2.0/src/conda_project/cli/commands.py
--rw-r--r--   0 adefusco   (502) staff       (20)    13155 2023-04-24 21:40:33.000000 conda-project-0.2.0/src/conda_project/cli/main.py
--rw-r--r--   0 adefusco   (502) staff       (20)     5094 2023-04-24 21:40:33.000000 conda-project-0.2.0/src/conda_project/conda.py
--rw-r--r--   0 adefusco   (502) staff       (20)     6798 2023-04-21 15:52:22.000000 conda-project-0.2.0/src/conda_project/conda_transfer.py
--rw-r--r--   0 adefusco   (502) staff       (20)      264 2023-04-11 15:51:33.000000 conda-project-0.2.0/src/conda_project/exceptions.py
--rw-r--r--   0 adefusco   (502) staff       (20)    30045 2023-04-24 21:40:33.000000 conda-project-0.2.0/src/conda_project/project.py
--rw-r--r--   0 adefusco   (502) staff       (20)     2619 2023-04-24 00:49:12.000000 conda-project-0.2.0/src/conda_project/project_file.py
--rw-r--r--   0 adefusco   (502) staff       (20)     5010 2023-04-24 21:40:33.000000 conda-project-0.2.0/src/conda_project/utils.py
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.580713 conda-project-0.2.0/src/conda_project.egg-info/
--rw-r--r--   0 adefusco   (502) staff       (20)     6180 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project.egg-info/PKG-INFO
--rw-r--r--   0 adefusco   (502) staff       (20)     2158 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project.egg-info/SOURCES.txt
--rw-r--r--   0 adefusco   (502) staff       (20)        1 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project.egg-info/dependency_links.txt
--rw-r--r--   0 adefusco   (502) staff       (20)       62 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project.egg-info/entry_points.txt
--rw-r--r--   0 adefusco   (502) staff       (20)      230 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project.egg-info/requires.txt
--rw-r--r--   0 adefusco   (502) staff       (20)       14 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project.egg-info/top_level.txt
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.585073 conda-project-0.2.0/tests/
--rw-r--r--   0 adefusco   (502) staff       (20)       99 2022-04-14 22:10:46.000000 conda-project-0.2.0/tests/__init__.py
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.585824 conda-project-0.2.0/tests/assets/
--rw-r--r--   0 adefusco   (502) staff       (20)     6798 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/assets/no-top-level-dir.tar.gz
--rw-r--r--   0 adefusco   (502) staff       (20)     6850 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/assets/relative-paths.tar.gz
--rw-r--r--   0 adefusco   (502) staff       (20)     6855 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/assets/top-level-dir.tar.gz
--rw-r--r--   0 adefusco   (502) staff       (20)     6848 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/assets/unnamed-top-level-dir.tar.gz
--rw-r--r--   0 adefusco   (502) staff       (20)     2509 2023-04-18 17:50:49.000000 conda-project-0.2.0/tests/conftest.py
--rw-r--r--   0 adefusco   (502) staff       (20)     3665 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/test_archive.py
--rw-r--r--   0 adefusco   (502) staff       (20)    11521 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/test_cli.py
--rw-r--r--   0 adefusco   (502) staff       (20)    12269 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/test_commands.py
--rw-r--r--   0 adefusco   (502) staff       (20)     6297 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/test_conda.py
--rw-r--r--   0 adefusco   (502) staff       (20)    35061 2023-04-19 03:34:42.000000 conda-project-0.2.0/tests/test_project.py
--rw-r--r--   0 adefusco   (502) staff       (20)     4922 2023-04-01 01:55:09.000000 conda-project-0.2.0/tests/test_project_file.py
--rw-r--r--   0 adefusco   (502) staff       (20)     7628 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:34.034312 conda-project-0.2.1/
+-rw-r--r--   0 adefusco   (502) staff       (20)      136 2023-04-05 14:24:50.000000 conda-project-0.2.1/.flake8
+-rw-r--r--   0 adefusco   (502) staff       (20)       58 2022-04-01 15:52:07.000000 conda-project-0.2.1/.gitattributes
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:33.983651 conda-project-0.2.1/.github/
+-rw-r--r--   0 adefusco   (502) staff       (20)       71 2022-04-14 22:10:46.000000 conda-project-0.2.1/.github/disclaimer.txt
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:33.985649 conda-project-0.2.1/.github/workflows/
+-rw-r--r--   0 adefusco   (502) staff       (20)     1323 2023-07-21 22:30:47.000000 conda-project-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)     5744 2023-07-31 16:05:16.000000 conda-project-0.2.1/.github/workflows/main.yaml
+-rw-r--r--   0 adefusco   (502) staff       (20)     1913 2023-07-15 22:58:10.000000 conda-project-0.2.1/.gitignore
+-rw-r--r--   0 adefusco   (502) staff       (20)      999 2023-08-02 14:34:44.000000 conda-project-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 adefusco   (502) staff       (20)     1897 2023-08-02 14:34:44.000000 conda-project-0.2.1/CHANGELOG.md
+-rw-r--r--   0 adefusco   (502) staff       (20)     1544 2022-04-01 15:50:48.000000 conda-project-0.2.1/LICENSE
+-rw-r--r--   0 adefusco   (502) staff       (20)     6307 2023-08-02 14:35:34.034037 conda-project-0.2.1/PKG-INFO
+-rw-r--r--   0 adefusco   (502) staff       (20)     4878 2023-07-21 22:30:47.000000 conda-project-0.2.1/README.md
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:33.986114 conda-project-0.2.1/conda.recipe/
+-rw-r--r--   0 adefusco   (502) staff       (20)     1154 2023-07-15 22:56:18.000000 conda-project-0.2.1/conda.recipe/meta.yaml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:33.988386 conda-project-0.2.1/docs/
+-rw-r--r--   0 adefusco   (502) staff       (20)     1759 2023-04-06 01:03:58.000000 conda-project-0.2.1/docs/Makefile
+-rw-r--r--   0 adefusco   (502) staff       (20)      112 2022-12-06 15:55:00.000000 conda-project-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:33.991665 conda-project-0.2.1/docs/source/
+-rw-r--r--   0 adefusco   (502) staff       (20)     1771 2023-04-06 01:03:58.000000 conda-project-0.2.1/docs/source/conf.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     4022 2023-04-24 21:40:33.000000 conda-project-0.2.1/docs/source/experimental.md
+-rw-r--r--   0 adefusco   (502) staff       (20)      151 2023-04-24 21:40:33.000000 conda-project-0.2.1/docs/source/index.md
+-rw-r--r--   0 adefusco   (502) staff       (20)     1636 2023-03-28 16:19:13.000000 conda-project-0.2.1/docs/source/setup_for_development.md
+-rw-r--r--   0 adefusco   (502) staff       (20)     5873 2023-03-30 21:40:52.000000 conda-project-0.2.1/docs/source/tutorial.md
+-rw-r--r--   0 adefusco   (502) staff       (20)    12563 2023-07-21 22:30:44.000000 conda-project-0.2.1/docs/source/user_guide.md
+-rw-r--r--   0 adefusco   (502) staff       (20)      259 2023-07-10 18:54:24.000000 conda-project-0.2.1/environment.yml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:33.994797 conda-project-0.2.1/etc/
+-rw-r--r--   0 adefusco   (502) staff       (20)      102 2023-04-05 14:24:50.000000 conda-project-0.2.1/etc/build-environment.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)      263 2023-07-21 22:30:44.000000 conda-project-0.2.1/etc/test-environment.yml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:33.996291 conda-project-0.2.1/examples/
+-rw-r--r--   0 adefusco   (502) staff       (20)       95 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/.gitignore
+-rw-r--r--   0 adefusco   (502) staff       (20)      621 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/README.md
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:33.998797 conda-project-0.2.1/examples/cmds-and-vars/
+-rw-r--r--   0 adefusco   (502) staff       (20)     1959 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/cmds-and-vars/README.md
+-rw-r--r--   0 adefusco   (502) staff       (20)    22470 2023-07-15 22:56:22.000000 conda-project-0.2.1/examples/cmds-and-vars/conda-lock.default.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)      317 2023-07-15 22:56:25.000000 conda-project-0.2.1/examples/cmds-and-vars/conda-project.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)       54 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/cmds-and-vars/environment.yml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:34.001834 conda-project-0.2.1/examples/condarc-settings/
+-rw-r--r--   0 adefusco   (502) staff       (20)       16 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/condarc-settings/.condarc
+-rw-r--r--   0 adefusco   (502) staff       (20)      389 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/condarc-settings/README.md
+-rw-r--r--   0 adefusco   (502) staff       (20)       92 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/condarc-settings/environment.yml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:34.002386 conda-project-0.2.1/examples/env-file-only/
+-rw-r--r--   0 adefusco   (502) staff       (20)     1434 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/env-file-only/README.md
+-rw-r--r--   0 adefusco   (502) staff       (20)       40 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/env-file-only/environment.yml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:34.010024 conda-project-0.2.1/examples/multi-env-files/
+-rw-r--r--   0 adefusco   (502) staff       (20)     2971 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/multi-env-files/README.md
+-rw-r--r--   0 adefusco   (502) staff       (20)    22470 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/multi-env-files/conda-lock.default.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)    33992 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/multi-env-files/conda-lock.test.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)      117 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/multi-env-files/conda-project.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)       54 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/multi-env-files/environment.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)       49 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/multi-env-files/extras.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)      299 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/multi-env-files/print_version.py
+-rw-r--r--   0 adefusco   (502) staff       (20)      195 2023-04-01 01:55:09.000000 conda-project-0.2.1/examples/multi-env-files/test_get_version.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     3120 2023-06-09 19:13:12.000000 conda-project-0.2.1/pyproject.toml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:34.010243 conda-project-0.2.1/scripts/
+-rw-r--r--   0 adefusco   (502) staff       (20)     6189 2023-04-24 21:40:33.000000 conda-project-0.2.1/scripts/ap-to-cp.py
+-rw-r--r--   0 adefusco   (502) staff       (20)       38 2023-08-02 14:35:34.034386 conda-project-0.2.1/setup.cfg
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:33.978937 conda-project-0.2.1/src/
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:34.021000 conda-project-0.2.1/src/conda_project/
+-rw-r--r--   0 adefusco   (502) staff       (20)      303 2023-04-06 01:03:58.000000 conda-project-0.2.1/src/conda_project/__init__.py
+-rw-r--r--   0 adefusco   (502) staff       (20)      134 2023-04-05 14:24:50.000000 conda-project-0.2.1/src/conda_project/__main__.py
+-rw-r--r--   0 adefusco   (502) staff       (20)      160 2023-08-02 14:35:33.000000 conda-project-0.2.1/src/conda_project/_version.py
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:34.025810 conda-project-0.2.1/src/conda_project/cli/
+-rw-r--r--   0 adefusco   (502) staff       (20)       99 2023-04-05 14:24:50.000000 conda-project-0.2.1/src/conda_project/cli/__init__.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     4687 2023-07-21 22:30:44.000000 conda-project-0.2.1/src/conda_project/cli/commands.py
+-rw-r--r--   0 adefusco   (502) staff       (20)    13155 2023-07-21 22:30:44.000000 conda-project-0.2.1/src/conda_project/cli/main.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     5094 2023-04-24 21:40:33.000000 conda-project-0.2.1/src/conda_project/conda.py
+-rw-r--r--   0 adefusco   (502) staff       (20)      264 2023-04-11 15:51:33.000000 conda-project-0.2.1/src/conda_project/exceptions.py
+-rw-r--r--   0 adefusco   (502) staff       (20)    31747 2023-08-01 17:59:49.000000 conda-project-0.2.1/src/conda_project/project.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     2619 2023-07-24 22:05:09.000000 conda-project-0.2.1/src/conda_project/project_file.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     5379 2023-07-31 16:05:16.000000 conda-project-0.2.1/src/conda_project/utils.py
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:34.023082 conda-project-0.2.1/src/conda_project.egg-info/
+-rw-r--r--   0 adefusco   (502) staff       (20)     6307 2023-08-02 14:35:33.000000 conda-project-0.2.1/src/conda_project.egg-info/PKG-INFO
+-rw-r--r--   0 adefusco   (502) staff       (20)     2163 2023-08-02 14:35:33.000000 conda-project-0.2.1/src/conda_project.egg-info/SOURCES.txt
+-rw-r--r--   0 adefusco   (502) staff       (20)        1 2023-08-02 14:35:33.000000 conda-project-0.2.1/src/conda_project.egg-info/dependency_links.txt
+-rw-r--r--   0 adefusco   (502) staff       (20)       62 2023-08-02 14:35:33.000000 conda-project-0.2.1/src/conda_project.egg-info/entry_points.txt
+-rw-r--r--   0 adefusco   (502) staff       (20)      230 2023-08-02 14:35:33.000000 conda-project-0.2.1/src/conda_project.egg-info/requires.txt
+-rw-r--r--   0 adefusco   (502) staff       (20)       14 2023-08-02 14:35:33.000000 conda-project-0.2.1/src/conda_project.egg-info/top_level.txt
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:34.030591 conda-project-0.2.1/tests/
+-rw-r--r--   0 adefusco   (502) staff       (20)       99 2022-04-14 22:10:46.000000 conda-project-0.2.1/tests/__init__.py
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-08-02 14:35:34.033543 conda-project-0.2.1/tests/assets/
+-rw-r--r--   0 adefusco   (502) staff       (20)     6798 2023-04-24 21:40:33.000000 conda-project-0.2.1/tests/assets/no-top-level-dir.tar.gz
+-rw-r--r--   0 adefusco   (502) staff       (20)     6850 2023-04-24 21:40:33.000000 conda-project-0.2.1/tests/assets/relative-paths.tar.gz
+-rw-r--r--   0 adefusco   (502) staff       (20)     6855 2023-04-24 21:40:33.000000 conda-project-0.2.1/tests/assets/top-level-dir.tar.gz
+-rw-r--r--   0 adefusco   (502) staff       (20)     6848 2023-04-24 21:40:33.000000 conda-project-0.2.1/tests/assets/unnamed-top-level-dir.tar.gz
+-rw-r--r--   0 adefusco   (502) staff       (20)     2509 2023-07-21 22:30:44.000000 conda-project-0.2.1/tests/conftest.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     4803 2023-07-16 00:12:57.000000 conda-project-0.2.1/tests/test_archive.py
+-rw-r--r--   0 adefusco   (502) staff       (20)    11521 2023-07-21 22:30:44.000000 conda-project-0.2.1/tests/test_cli.py
+-rw-r--r--   0 adefusco   (502) staff       (20)    12269 2023-04-24 21:40:33.000000 conda-project-0.2.1/tests/test_commands.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     6297 2023-04-24 21:40:33.000000 conda-project-0.2.1/tests/test_conda.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     5549 2023-07-16 00:12:57.000000 conda-project-0.2.1/tests/test_init.py
+-rw-r--r--   0 adefusco   (502) staff       (20)    10113 2023-07-31 16:05:16.000000 conda-project-0.2.1/tests/test_install.py
+-rw-r--r--   0 adefusco   (502) staff       (20)    24149 2023-08-01 17:59:49.000000 conda-project-0.2.1/tests/test_project.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     4922 2023-07-21 22:30:44.000000 conda-project-0.2.1/tests/test_project_file.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     8281 2023-07-31 16:05:16.000000 conda-project-0.2.1/tests/test_utils.py
```

### Comparing `conda-project-0.2.0/.github/workflows/docs.yml` & `conda-project-0.2.1/.github/workflows/docs.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 name: Docs
 
 on:
-  # Runs on pushes targeting the default branch
+  # Run build & publish on pushes targeting the default branch (after PR is merged)
   push:
-    branches: ["main"]
-
+    branches:
+    - main
+  # Run build during PRs (but not publish)
+  pull_request:
+    branches:
+    - main
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 # Allow one concurrent deployment
 concurrency:
   group: "pages"
   cancel-in-progress: true
@@ -33,15 +37,15 @@
       - name: Upload artifact
         uses: actions/upload-pages-artifact@v1
         with:
           # Upload entire repository
           path: 'docs/_build/html'
 
   pages:
-
+    if: github.ref == 'refs/heads/main'
     runs-on: ubuntu-latest
     needs: [docs]
 
     # Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
     permissions:
       contents: read
       pages: write
```

### Comparing `conda-project-0.2.0/.github/workflows/main.yaml` & `conda-project-0.2.1/.github/workflows/main.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 on:
   push:
     paths-ignore:
       - "README.md"
       - "LICENSE"
       - "MANIFEST"
       - "docs/**"
+      - ".github/workflows/docs.yml"
     branches:
       - main
   pull_request:
     paths-ignore:
       - "README.md"
       - "LICENSE"
       - "MANIFEST"
       - "docs/**"
+      - ".github/workflows/docs.yml"
     branches:
       - main
+
+
 jobs:
   package:
     name: Build package
     runs-on: "ubuntu-latest"
     steps:
       - uses: actions/checkout@v3
         with:
@@ -45,19 +49,17 @@
     name: Test (conda ${{ matrix.conda-version }}, Python ${{ matrix.python-version }}, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest", "macos-latest", "windows-latest"]
         python-version: [3.8, 3.9, "3.10"]
-        conda-version: ["4.9", "4.10", "4.11", "4.12", "4.13", "4.14", "22.9", "22.11", "23.1"]
+        conda-version: ["4.11", "4.12", "4.13", "4.14", "22.9", "22.11", "23.1", "23.3", "23.5"]
         exclude:
           # Python 3.10
-          - conda-version: "4.9"
-            python-version: "3.10"
           - conda-version: "4.11"
             python-version: "3.10"
     env:
       OS: ${{ matrix.os }}
       PYTHON: ${{ matrix.python-version }}
     steps:
       - uses: actions/checkout@v3
@@ -75,14 +77,17 @@
           ./conda.exe config --set auto_update_conda false
           ./conda.exe clean -ay
           ./conda.exe info
       - name: Setup miniconda
         shell: bash
         run: |
           ./conda.exe create -p $HOME/miniconda conda=${{ matrix.conda-version }} python=${{ matrix.python-version }}
+      - name: Update with test dependencies
+        shell: bash
+        run: |
           if [ $RUNNER_OS == 'Windows' ]; then
             source $HOME/miniconda/Scripts/activate root && conda env update -f etc/test-environment.yml -p $HOME/miniconda && $HOME/miniconda/Scripts/pip install --no-deps .
           else
             source $HOME/miniconda/bin/activate root && conda env update -f etc/test-environment.yml -p $HOME/miniconda && $HOME/miniconda/bin/pip install --no-deps .
           fi
       - name: Install Libmamba
         shell: bash
@@ -94,14 +99,16 @@
             else
               source $HOME/miniconda/bin/activate root && \
               conda install conda-libmamba-solver -p $HOME/miniconda
             fi
           fi
       - name: py.test
         shell: bash
+        env:
+          CONDA_DEFAULT_CHANNELS: conda-forge
         run: |
           if [ $RUNNER_OS == 'Windows' ]; then
             source $HOME/miniconda/Scripts/activate root && \
             conda --version && \
             py.test \
               -xv \
               --cov-report xml:./coverage.xml \
```

### Comparing `conda-project-0.2.0/.gitignore` & `conda-project-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/.pre-commit-config.yaml` & `conda-project-0.2.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     -   id: trailing-whitespace
 -   repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
     -   id: isort
         name: isort
 -   repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
     -   id: black
 -   repo: https://github.com/pycqa/flake8
-    rev: 6.0.0
+    rev: 6.1.0
     hooks:
     -   id: flake8
 -   repo: https://github.com/Lucas-C/pre-commit-hooks
     rev: v1.5.1
     hooks:
     -   id: insert-license
         files: \.py$
```

### Comparing `conda-project-0.2.0/CHANGELOG.md` & `conda-project-0.2.1/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## [0.2.1] - 2023-08-01
+
+## Fixes
+
+- Fix expand `~` in paths [#110](https://github.com/conda-incubator/conda-project/pull/110)
+- Fix relative paths in `conda-lock.<env>.yml` [#125](https://github.com/conda-incubator/conda-project/pull/125)
+- Fix support for newer conda-lock versions [#129](https://github.com/conda-incubator/conda-project/pull/129)
+- Fix for inconsistent installed envs [#135](https://github.com/conda-incubator/conda-project/pull/135)
+- Fix for error messages from conda [#134](https://github.com/conda-incubator/conda-project/pull/134)
+- Fix locking platforms message [#137](https://github.com/conda-incubator/conda-project/pull/137)
+
+## Maintenance
+
+- Add new static badge linking to documentation [#116](https://github.com/conda-incubator/conda-project/pull/116)
+
 ## [0.2.0] - 2023-04-24
 
 ## Added
 
 - Experimental: run commands using an external conda environment. [#106](https://github.com/conda-incubator/conda-project/pull/106)
 - Experimental: download and extract a project archive on first use. [#106](https://github.com/conda-incubator/conda-project/pull/106)
 - Experimental: Anaconda Project -> Conda Project conversion script. [#106](https://github.com/conda-incubator/conda-project/pull/106)
```

### Comparing `conda-project-0.2.0/LICENSE` & `conda-project-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/PKG-INFO` & `conda-project-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-project
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tool for encapsulating, running, and reproducing projects with conda environments
 Author-email: Albert DeFusco <adefusco@anaconda.com>, Matt Kramer <mkramer@anaconda.com>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/conda-incubator/conda-project
 Project-URL: homepage, https://github.com/conda-incubator/conda-project
 Project-URL: documentation, https://conda-incubator.github.io/conda-project/user_guide.html
 Project-URL: Issue Tracker, https://github.com/conda-incubator/conda-project/issues
@@ -28,14 +28,15 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 # conda-project
 
 [![codecov](https://codecov.io/gh/conda-incubator/conda-project/branch/main/graph/badge.svg?token=XNRS8JKT75)](https://codecov.io/gh/conda-incubator/conda-project)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/conda-incubator/conda-project/main.svg)](https://results.pre-commit.ci/latest/github/conda-incubator/conda-project/main)
+[![Static Badge](https://img.shields.io/badge/docs-success-blue?logo=github)](https://conda-incubator.github.io/conda-project)
 
 Tool for encapsulating, running, and reproducing projects with conda environments.
 
 
 ## Why?
 
 Sharing your work is more than sharing your code in a script file or notebook. To make your work properly reproducible, it is necessary to include the list of required third-party dependencies, specifications for how to run your code, and
```

### Comparing `conda-project-0.2.0/README.md` & `conda-project-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # conda-project
 
 [![codecov](https://codecov.io/gh/conda-incubator/conda-project/branch/main/graph/badge.svg?token=XNRS8JKT75)](https://codecov.io/gh/conda-incubator/conda-project)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/conda-incubator/conda-project/main.svg)](https://results.pre-commit.ci/latest/github/conda-incubator/conda-project/main)
+[![Static Badge](https://img.shields.io/badge/docs-success-blue?logo=github)](https://conda-incubator.github.io/conda-project)
 
 Tool for encapsulating, running, and reproducing projects with conda environments.
 
 
 ## Why?
 
 Sharing your work is more than sharing your code in a script file or notebook. To make your work properly reproducible, it is necessary to include the list of required third-party dependencies, specifications for how to run your code, and
```

### Comparing `conda-project-0.2.0/conda.recipe/meta.yaml` & `conda-project-0.2.1/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/docs/Makefile` & `conda-project-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/docs/source/conf.py` & `conda-project-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/docs/source/experimental.md` & `conda-project-0.2.1/docs/source/experimental.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/docs/source/setup_for_development.md` & `conda-project-0.2.1/docs/source/setup_for_development.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/docs/source/tutorial.md` & `conda-project-0.2.1/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/docs/source/user_guide.md` & `conda-project-0.2.1/docs/source/user_guide.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/examples/README.md` & `conda-project-0.2.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/examples/cmds-and-vars/README.md` & `conda-project-0.2.1/examples/cmds-and-vars/README.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/examples/cmds-and-vars/conda-lock.default.yml` & `conda-project-0.2.1/examples/cmds-and-vars/conda-lock.default.yml`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/examples/env-file-only/README.md` & `conda-project-0.2.1/examples/env-file-only/README.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/examples/multi-env-files/README.md` & `conda-project-0.2.1/examples/multi-env-files/README.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/examples/multi-env-files/conda-lock.default.yml` & `conda-project-0.2.1/examples/multi-env-files/conda-lock.default.yml`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/examples/multi-env-files/conda-lock.test.yml` & `conda-project-0.2.1/examples/multi-env-files/conda-lock.test.yml`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/pyproject.toml` & `conda-project-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/scripts/ap-to-cp.py` & `conda-project-0.2.1/scripts/ap-to-cp.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/src/conda_project/cli/commands.py` & `conda-project-0.2.1/src/conda_project/cli/commands.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/src/conda_project/cli/main.py` & `conda-project-0.2.1/src/conda_project/cli/main.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/src/conda_project/conda.py` & `conda-project-0.2.1/src/conda_project/conda.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/src/conda_project/project.py` & `conda-project-0.2.1/src/conda_project/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,21 @@
 from .project_file import (
     ENVIRONMENT_YAML_FILENAMES,
     PROJECT_YAML_FILENAMES,
     CondaProjectYaml,
     EnvironmentYaml,
     yaml,
 )
-from .utils import Spinner, env_variable, find_file, prepare_variables
+from .utils import (
+    Spinner,
+    dedupe_list_of_dicts,
+    env_variable,
+    find_file,
+    prepare_variables,
+)
 
 _TEMPFILE_DELETE = False if sys.platform.startswith("win") else True
 
 DEFAULT_PLATFORMS = set(["osx-64", "win-64", "linux-64", current_platform()])
 
 # A regex pattern used to extract package name and hash from output of "pip freeze"
 _PIP_FREEZE_REGEX_PATTERN = re.compile(r"(?P<name>[\w-]+) @ .*sha256=(?P<sha256>\w+)")
@@ -85,15 +91,15 @@
         else:
             raise e
 
     pip_sha256: dict[str, str] = {}
     for line in pip_freeze.stdout.strip().splitlines():
         m = _PIP_FREEZE_REGEX_PATTERN.match(line)
         if m is not None:
-            pip_sha256[m.group("name")] = m.group("sha256")
+            pip_sha256[m.group("name").lower().replace("_", "-")] = m.group("sha256")
     return pip_sha256
 
 
 class CondaProject:
     """A project managed by `conda-project`.
 
     Attributes:
@@ -107,15 +113,15 @@
 
     Raises:
         CondaProjectError: If no suitable environment file is found.
 
     """
 
     def __init__(self, directory: Union[Path, str] = "."):
-        self.directory = Path(directory).resolve()
+        self.directory = Path(directory).expanduser().resolve()
         logger.info(f"created Project instance at {self.directory}")
 
         self.project_yaml_path = find_file(self.directory, PROJECT_YAML_FILENAMES)
         if self.project_yaml_path is not None:
             self._project_file = CondaProjectYaml.parse_yaml(self.project_yaml_path)
         else:
             options = " or ".join(PROJECT_YAML_FILENAMES)
@@ -144,22 +150,23 @@
         cls,
         fn: Union[Path, str],
         storage_options: Optional[Dict[str, str]] = None,
         output_directory: Union[Path, str] = ".",
     ):
         """Extra a conda-project archive and load the project"""
 
-        if isinstance(output_directory, str):
-            output_directory = Path(output_directory)
+        output_directory = Path(output_directory).expanduser()
 
         storage_options = {} if storage_options is None else storage_options
         protocol, _ = split_protocol(fn)
         if protocol is not None:
             options = {protocol: storage_options}
+            fn = f"simplecache::{fn}"
         else:
+            fn = Path(fn).expanduser()
             options = {}
 
         files = fsspec.open_files(f"libarchive://**::{fn}", **options)
         archive_name = Path(Path(fn).name.split(".", maxsplit=1)[0])
 
         first_parts = set(Path(p.path).parts[0] for p in files)
         if ".." in first_parts:
@@ -239,15 +246,15 @@
             verbose:           Print information to stdout. The default value is False.
 
         Returns:
             CondaProject instance for the project directory.
 
         """
 
-        directory = Path(directory).resolve()
+        directory = Path(directory).expanduser().resolve()
         if not directory.exists():
             directory.mkdir(parents=True)
 
         existing_project_file = find_file(directory, PROJECT_YAML_FILENAMES)
         if existing_project_file is not None:
             if verbose:
                 print(f"Existing project file found at {existing_project_file}.")
@@ -471,38 +478,44 @@
 
         # Here, we ensure that we clear the cache on the PrefixData class. This is to
         # ensure that we freshly load the installed packages each time.
         PrefixData._cache_.pop(self.prefix, None)
 
         pip_sha256 = _load_pip_sha256_hashes(str(self.prefix))
 
-        # Generate a set of (name, version, manager, sha256) tuples from the conda environment
+        # Generate a set of (name, version, manager, hash) tuples from the conda environment
         # We also convert the conda package_type attribute to a string in the set
         # {"conda", "pip"} to allow direct comparison with conda-lock.
         # TODO: pip_interop_enabled is marked "DO NOT USE". What is the alternative?
         pd = PrefixData(self.prefix, pip_interop_enabled=True)
         installed_pkgs = set()
         for p in pd.iter_records():
             manager = _package_type_to_manager(p.package_type)
             if manager == "pip":
                 sha256 = pip_sha256.get(p.name)
             else:
-                sha256 = p.sha256
+                sha256 = p.md5  # not all conda packages will have a published sha256
 
             installed_pkgs.add((p.name, p.version, manager, sha256))
 
-        # Generate a set of (name, version, manager, sha256) tuples from the lockfile
+        # Generate a set of (name, version, manager, hash) tuples from the lockfile
         # We only include locked packages for the current platform, and don't
         # include optional dependencies (e.g. compile/build)
         lock = parse_conda_lock_file(self.lockfile)
-        locked_pkgs = {
-            (p.name, p.version, p.manager, p.hash.sha256)
-            for p in lock.package
-            if p.platform == current_platform() and not p.optional
-        }
+
+        # When an environment is installed pypi packages take precedence
+        deduped_lock = dedupe_list_of_dicts(
+            lock.package, key=lambda x: x.name, keep=lambda x: x.manager == "pip"
+        )
+
+        locked_pkgs = set()
+        for p in deduped_lock:
+            if p.platform == current_platform() and p.category == "main":
+                hash = p.hash.md5 if p.manager == "conda" else p.hash.sha256
+                locked_pkgs.add((p.name, p.version, p.manager, hash))
 
         # Compare the sets
         # We can do this because the tuples are hashable. Also we don't need to
         # consider ordering.
         return installed_pkgs == locked_pkgs
 
     def lock(
@@ -529,70 +542,94 @@
             return
 
         # Setup temporary file for conda-lock to write to.
         # If a package is removed from the environment source
         # after the lockfile has been created conda-lock updates
         # the hash in the lockfile but does not remove the unspecified
         # package (and necessary orphaned dependencies) from the lockfile.
-        # To avoid this scenario lockfiles are written to a temporary location
-        # and copied back to the self.lockfile path if successful.
-        tempdir = Path(tempfile.mkdtemp())
-        lockfile = tempdir / self.lockfile.name
+        # To avoid this scenario lockfiles are written to a temporary name
+        # and copied to the self.lockfile path if successful. It is
+        # important to create the lock file in the same directory so that
+        # conda-lock's relative path handling works as expected.
+        lockname = self.lockfile.name
+        templock = Path(
+            tempfile.mktemp(prefix=lockname + ".", dir=self.lockfile.parent)
+        )
+        tempname = templock.name
 
         channel_overrides, platform_overrides = self._overrides
 
         specified_channels = []
+        specified_platforms = set()
         for fn in self.sources:
             env = EnvironmentYaml.parse_yaml(fn)
             for channel in env.channels or []:
                 if channel not in specified_channels:
                     specified_channels.append(channel)
+            if env.platforms:
+                specified_platforms.update(env.platforms)
 
         with redirect_stderr(StringIO()) as _:
             with env_variable("CONDARC", str(self.project.condarc)):
                 if verbose:
-                    p = (
+                    p = sorted(
                         platform_overrides
                         if platform_overrides is not None
-                        else DEFAULT_PLATFORMS
+                        else specified_platforms
                     )
                     context = Spinner(
                         prefix=f"Locking dependencies for environment {self.name} on "
                         f"platforms {', '.join(p)}"
                     )
                 else:
                     context = nullcontext()
 
                 with context:
                     try:
                         make_lock_files(
                             conda=CONDA_EXE,
                             src_files=list(self.sources),
-                            lockfile_path=lockfile,
+                            lockfile_path=templock,
                             kinds=["lock"],
                             platform_overrides=platform_overrides,
                             channel_overrides=channel_overrides,
                         )
-                        shutil.copy(lockfile, self.lockfile)
+                        with open(templock, "r") as fp:
+                            data = fp.read()
+                        # Replace the occurences of the temporary filename
+                        # (in the header comment) with the proper filename
+                        data = data.replace(tempname, lockname)
+                        with open(templock, "w") as fp:
+                            fp.write(data)
+                        shutil.copy(templock, self.lockfile)
                     except SubprocessError as e:
                         try:
                             output = json.loads(e.output)
                         except json.decoder.JSONDecodeError:
-                            # A bug in conda-libmamba-solver causes # serialization
+                            # A bug in conda-libmamba-solver causes serialization
                             # errors so we'll just print the full stack trace on error.
                             raise CondaProjectLockFailed(e.stderr)
 
-                        msg = output["message"].replace(
-                            "target environment",
-                            f"supplied channels: {channel_overrides or specified_channels}",
-                        )
+                        original_msg = output.get("message")
+                        if original_msg is not None:
+                            msg = original_msg.replace(
+                                "target environment",
+                                f"supplied channels: {channel_overrides or specified_channels}",
+                            )
+                        else:
+                            msg = output.get(
+                                "traceback",
+                                "<something went wrong during the lock and the message could not be recovered>",
+                            )
+
                         msg = "Project failed to lock\n" + msg
                         raise CondaProjectLockFailed(msg)
                     finally:
-                        shutil.rmtree(tempdir)
+                        if os.path.exists(templock):
+                            os.unlink(templock)
 
         lock = parse_conda_lock_file(self.lockfile)
         msg = f"Locked dependencies for {', '.join(lock.metadata.platforms)} platforms"
         logger.info(msg)
 
     def install(
         self,
```

### Comparing `conda-project-0.2.0/src/conda_project/project_file.py` & `conda-project-0.2.1/src/conda_project/project_file.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/src/conda_project/utils.py` & `conda-project-0.2.1/src/conda_project/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 import sys
 import threading
 import time
 from collections import ChainMap
 from collections.abc import Generator
 from contextlib import contextmanager
 from inspect import Traceback
+from itertools import groupby
 from pathlib import Path
 from subprocess import Popen
-from typing import Dict, List, NoReturn, Optional, Type, Union
+from typing import Callable, Dict, List, NoReturn, Optional, Type, Union
 
 import shellingham
 from dotenv import dotenv_values
 
 from .exceptions import CondaProjectError
 
 
@@ -178,7 +179,18 @@
             shell_name = shell_path = os.environ.get("COMSPEC", "cmd.exe")
         else:
             raise RuntimeError(
                 "Could not determine an appropriate shell to activate for your OS."
             )
 
     return shell_name, shell_path
+
+
+def dedupe_list_of_dicts(data: list, key: Callable, keep: Callable) -> list:
+    deduped = []
+    for _, g in groupby(sorted(data, key=key), key=key):
+        values = list(g)
+        if len(values) > 1:
+            deduped.extend(list(filter(keep, values)))
+        else:
+            deduped.extend(values)
+    return deduped
```

### Comparing `conda-project-0.2.0/src/conda_project.egg-info/PKG-INFO` & `conda-project-0.2.1/src/conda_project.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-project
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tool for encapsulating, running, and reproducing projects with conda environments
 Author-email: Albert DeFusco <adefusco@anaconda.com>, Matt Kramer <mkramer@anaconda.com>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/conda-incubator/conda-project
 Project-URL: homepage, https://github.com/conda-incubator/conda-project
 Project-URL: documentation, https://conda-incubator.github.io/conda-project/user_guide.html
 Project-URL: Issue Tracker, https://github.com/conda-incubator/conda-project/issues
@@ -28,14 +28,15 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 # conda-project
 
 [![codecov](https://codecov.io/gh/conda-incubator/conda-project/branch/main/graph/badge.svg?token=XNRS8JKT75)](https://codecov.io/gh/conda-incubator/conda-project)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/conda-incubator/conda-project/main.svg)](https://results.pre-commit.ci/latest/github/conda-incubator/conda-project/main)
+[![Static Badge](https://img.shields.io/badge/docs-success-blue?logo=github)](https://conda-incubator.github.io/conda-project)
 
 Tool for encapsulating, running, and reproducing projects with conda environments.
 
 
 ## Why?
 
 Sharing your work is more than sharing your code in a script file or notebook. To make your work properly reproducible, it is necessary to include the list of required third-party dependencies, specifications for how to run your code, and
```

### Comparing `conda-project-0.2.0/src/conda_project.egg-info/SOURCES.txt` & `conda-project-0.2.1/src/conda_project.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 examples/multi-env-files/print_version.py
 examples/multi-env-files/test_get_version.py
 scripts/ap-to-cp.py
 src/conda_project/__init__.py
 src/conda_project/__main__.py
 src/conda_project/_version.py
 src/conda_project/conda.py
-src/conda_project/conda_transfer.py
 src/conda_project/exceptions.py
 src/conda_project/project.py
 src/conda_project/project_file.py
 src/conda_project/utils.py
 src/conda_project.egg-info/PKG-INFO
 src/conda_project.egg-info/SOURCES.txt
 src/conda_project.egg-info/dependency_links.txt
@@ -61,14 +60,16 @@
 src/conda_project/cli/main.py
 tests/__init__.py
 tests/conftest.py
 tests/test_archive.py
 tests/test_cli.py
 tests/test_commands.py
 tests/test_conda.py
+tests/test_init.py
+tests/test_install.py
 tests/test_project.py
 tests/test_project_file.py
 tests/test_utils.py
 tests/assets/no-top-level-dir.tar.gz
 tests/assets/relative-paths.tar.gz
 tests/assets/top-level-dir.tar.gz
 tests/assets/unnamed-top-level-dir.tar.gz
```

### Comparing `conda-project-0.2.0/tests/assets/no-top-level-dir.tar.gz` & `conda-project-0.2.1/tests/assets/no-top-level-dir.tar.gz`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/tests/assets/relative-paths.tar.gz` & `conda-project-0.2.1/tests/assets/relative-paths.tar.gz`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/tests/assets/top-level-dir.tar.gz` & `conda-project-0.2.1/tests/assets/top-level-dir.tar.gz`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/tests/assets/unnamed-top-level-dir.tar.gz` & `conda-project-0.2.1/tests/assets/unnamed-top-level-dir.tar.gz`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/tests/conftest.py` & `conda-project-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/tests/test_archive.py` & `conda-project-0.2.1/tests/test_archive.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from pathlib import Path
 
 import pytest
 
 from conda_project.exceptions import CondaProjectError
 from conda_project.project import CondaProject
+from conda_project.utils import is_windows
 
 ASSETS_DIR = Path(__file__).parents[0] / "assets"
 
 PROJECT_CONTENTS = [
     Path(".condarc"),
     Path(".env"),
     Path("README.md"),
@@ -119,7 +120,41 @@
     _ = CondaProject.from_archive(
         f"file:///{fn}", storage_options={"key1": "valueA", "key2": "valueB"}
     )
 
     assert mocked_open_files.call_args_list[0].kwargs == {
         "file": {"key1": "valueA", "key2": "valueB"}
     }
+    assert "simplecache" in mocked_open_files.call_args_list[0].args[0]
+
+
+def test_archive_path_expanduser(mocker):
+    from pathlib import Path
+
+    expanduser = mocker.spy(Path, "expanduser")
+
+    archive = "~__a-conda-project-user__/project.tar.gz"
+    if is_windows():
+        with pytest.raises(FileNotFoundError):
+            _ = CondaProject.from_archive(fn=archive)
+    else:
+        with pytest.raises(RuntimeError):
+            _ = CondaProject.from_archive(fn=archive)
+
+    assert expanduser.call_count == 2
+
+
+def test_archive_output_directory_expanduser(mocker):
+    from pathlib import Path
+
+    expanduser = mocker.spy(Path, "expanduser")
+
+    archive = ASSETS_DIR / "top-level-dir.tar.gz"
+
+    output_directory = "~__a-conda-project-user__/project"
+    if is_windows():
+        _ = CondaProject.from_archive(fn=archive, output_directory=output_directory)
+        assert expanduser.call_count == 3
+    else:
+        with pytest.raises(RuntimeError):
+            _ = CondaProject.from_archive(fn=archive, output_directory=output_directory)
+        assert expanduser.call_count == 1
```

### Comparing `conda-project-0.2.0/tests/test_cli.py` & `conda-project-0.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/tests/test_commands.py` & `conda-project-0.2.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/tests/test_conda.py` & `conda-project-0.2.1/tests/test_conda.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/tests/test_project.py` & `conda-project-0.2.1/tests/test_project.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2022 Anaconda, Inc
 # SPDX-License-Identifier: BSD-3-Clause
 import json
-import logging
 import os
 from pathlib import Path
 from textwrap import dedent
 
 import pytest
+from pytest_mock import MockerFixture
 from ruamel.yaml import YAML
 
 from conda_project.conda import call_conda
 from conda_project.exceptions import CondaProjectError, CondaProjectLockFailed
 from conda_project.project import DEFAULT_PLATFORMS, CondaProject
 
 
@@ -20,391 +20,136 @@
     result = json.loads(proc.stdout)
     if result:
         return result[0]["name"] == "conda-libmamba-solver"
     else:
         return False
 
 
-def test_project_create_new_directory(tmp_path, capsys):
-    project_directory = tmp_path / "new-project"
-    assert not os.path.exists(project_directory)
-
-    p = CondaProject.init(project_directory, lock_dependencies=False, verbose=True)
-
-    assert os.path.exists(project_directory)
-    assert p.project_yaml_path.exists()
-    assert p.default_environment.sources[0].exists()
-    assert not p.default_environment.is_locked
-
-    assert p.condarc.exists()
-    with p.condarc.open() as f:
-        condarc = YAML().load(f)
-    assert condarc == {}
-
-    out, _ = capsys.readouterr()
-    assert f"Project created at {project_directory}\n" == out
-
-
-def test_project_create_twice(tmp_path, capsys):
-    _ = CondaProject.init(tmp_path, lock_dependencies=False)
-    p = CondaProject.init(tmp_path, lock_dependencies=False, verbose=True)
-
-    out, _ = capsys.readouterr()
-    assert f"Existing project file found at {p.project_yaml_path}.\n" == out
-
-
-def test_project_create_default_platforms(tmp_path):
-    p = CondaProject.init(tmp_path, lock_dependencies=False)
-
-    with p.default_environment.sources[0].open() as f:
-        env = YAML().load(f)
-
-    assert env["platforms"] == list(DEFAULT_PLATFORMS)
-
-
-def test_project_create_specific_platforms(tmp_path):
-    p = CondaProject.init(tmp_path, platforms=["linux-64"], lock_dependencies=False)
-
-    with p.default_environment.sources[0].open() as f:
-        env = YAML().load(f)
-
-    assert env["platforms"] == ["linux-64"]
-
-
-def test_project_create_specific_channels(tmp_path):
-    p = CondaProject.init(
-        tmp_path,
-        dependencies=["python=3.8", "numpy"],
-        channels=["conda-forge", "defaults"],
-        lock_dependencies=False,
-    )
-
-    with p.default_environment.sources[0].open() as f:
-        env = YAML().load(f)
-
-    assert env["dependencies"] == ["python=3.8", "numpy"]
-    assert env["channels"] == ["conda-forge", "defaults"]
-
-
-def test_project_create_default_channel(tmp_path):
-    p = CondaProject.init(
-        tmp_path, dependencies=["python=3.8", "numpy"], lock_dependencies=False
-    )
-
-    with p.default_environment.sources[0].open() as f:
-        env = YAML().load(f)
-
-    assert env["dependencies"] == ["python=3.8", "numpy"]
-    assert env["channels"] == ["defaults"]
-
-
-def test_project_create_conda_configs(tmp_path):
-    p = CondaProject.init(
-        tmp_path,
-        dependencies=["python=3.8", "numpy"],
-        conda_configs=["experimental_solver=libmamba"],
-        lock_dependencies=False,
-    )
-
-    with p.condarc.open() as f:
-        condarc = YAML().load(f)
-
-    assert condarc["experimental_solver"] == "libmamba"
-
-
 @pytest.mark.slow
-def test_project_create_and_lock(tmp_path):
-    p = CondaProject.init(tmp_path, dependencies=["python=3.8"], lock_dependencies=True)
-    assert p.default_environment.lockfile.exists()
-    assert p.default_environment.lockfile == tmp_path / "conda-lock.default.yml"
-
-
-def test_conda_project_init_empty_dir(tmp_path, caplog):
-    caplog.set_level(logging.INFO)
-
-    with pytest.raises(CondaProjectError) as excinfo:
-        CondaProject(tmp_path)
-    assert "No conda environment.yml or environment.yaml file was found" in str(
-        excinfo.value
-    )
-
-    assert "No conda-project.yml or conda-project.yaml file was found" in caplog.text
-
-
-def test_conda_project_init_with_env_yaml(project_directory_factory):
+def test_install_and_clean(project_directory_factory):
     env_yaml = dedent(
         """\
         name: test
-        dependencies: []
+        dependencies:
+          - python=3.8
         """
     )
     project_path = project_directory_factory(env_yaml=env_yaml)
-    project = CondaProject(project_path)
-
-    assert project.default_environment == project.environments["default"]
-
-    assert (
-        project.default_environment.lockfile
-        == project.directory / "conda-lock.default.yml"
-    )
-    assert project.default_environment.sources == (
-        (project.directory / "environment").with_suffix(
-            project_directory_factory._suffix
-        ),
-    )
-    assert project.default_environment.prefix == project.directory / "envs" / "default"
-
-
-def test_project_init_expands_cwd(monkeypatch, project_directory_factory):
-    project_path = project_directory_factory(env_yaml="")
-    monkeypatch.chdir(project_path)
-
-    project = CondaProject()
-    assert project.directory.samefile(project_path)
-
-
-def test_project_init_path(project_directory_factory):
-    project_path = project_directory_factory(env_yaml="")
-
-    project = CondaProject(project_path)
-    assert project.directory.samefile(project_path)
-
 
-def test_prepare_with_gitignore(project_directory_factory):
-    env_yaml = dedent(
-        """\
-        name: test
-        dependencies: []
-        """
-    )
-    project_path = project_directory_factory(env_yaml=env_yaml)
     project = CondaProject(project_path)
-
-    env_dir = project.default_environment.install()
-    assert (env_dir / ".gitignore").exists()
-    with (env_dir / ".gitignore").open("rt") as f:
-        assert f.read().strip() == "*"
-
-
-def test_prepare_no_dependencies(project_directory_factory):
-    env_yaml = dedent(
-        """\
-        name: test
-        dependencies: []
-        """
-    )
-    project_path = project_directory_factory(env_yaml=env_yaml)
-    project = CondaProject(project_path)
-
     env_dir = project.default_environment.install()
     assert env_dir.samefile(project_path / "envs" / "default")
 
     conda_history = env_dir / "conda-meta" / "history"
     assert conda_history.exists()
-    assert project.default_environment.is_consistent
-
-
-@pytest.mark.slow
-def test_is_prepared(project_directory_factory):
-    env_yaml = dedent(
-        """\
-        name: test
-        dependencies: [python=3.8]
-        """
-    )
-    project_path = project_directory_factory(env_yaml=env_yaml)
-    project = CondaProject(project_path)
 
-    _ = project.default_environment.install()
-    assert project.default_environment.is_consistent
-
-    updated_yaml = dedent(
-        """\
-        name: test
-        dependencies:
-          - python=3.8
-          - requests
-        """
-    )
+    with conda_history.open() as f:
+        assert "create -y --file" in f.read()
+    conda_history_mtime = os.path.getmtime(conda_history)
 
-    with (project.default_environment.sources[0]).open("wt") as f:
-        f.write(updated_yaml)
+    project.default_environment.install()
+    assert conda_history_mtime == os.path.getmtime(conda_history)
 
-    assert not project.default_environment.is_locked
-    assert not project.default_environment.is_consistent
+    project.default_environment.install(force=True)
+    assert conda_history_mtime < os.path.getmtime(conda_history)
 
-    _ = project.default_environment.install(force=False)
-    assert project.default_environment.is_locked
+    project.default_environment.clean()
+    assert not conda_history.exists()
     assert not project.default_environment.is_consistent
 
-    _ = project.default_environment.install(force=True)
-    assert project.default_environment.is_consistent
-
 
 @pytest.mark.slow
-def test_is_prepared_with_pip_package(project_directory_factory):
-    """Test that we can import the package if it is installed with pip."""
+def test_lock(project_directory_factory):
     env_yaml = dedent(
         """\
         name: test
         dependencies:
           - python=3.8
-          - pip
-          - pip:
-            - requests
         """
     )
     project_path = project_directory_factory(env_yaml=env_yaml)
-    project = CondaProject(project_path)
-
-    _ = project.default_environment.install()
 
-    # This assertion won't pass if there are pip packages
-    assert project.default_environment.is_consistent
-
-    args = [
-        "run",
-        *("-p", str(project.environments["default"].prefix)),
-        "python",
-        *("-c", "import requests"),
-    ]
-    result = call_conda(args, condarc_path=project.condarc)
-    assert result.returncode == 0
-
-
-@pytest.mark.slow
-def test_is_prepared_live_env_changed(project_directory_factory, capsys):
-    env_yaml = dedent(
-        """\
-        name: test
-        dependencies: [python=3.8]
-        """
-    )
-    project_path = project_directory_factory(env_yaml=env_yaml)
     project = CondaProject(project_path)
+    project.default_environment.lock()
 
-    _ = project.default_environment.install()
-    assert project.default_environment.is_locked
-    assert project.default_environment.is_consistent
-
-    _ = call_conda(
-        ["install", "-p", str(project.default_environment.prefix), "requests", "-y"]
-    )
-
+    lockfile = project_path / "conda-lock.default.yml"
+    assert lockfile == project.default_environment.lockfile
+    assert lockfile.exists()
     assert project.default_environment.is_locked
-    assert not project.default_environment.is_consistent
-
-    _ = project.default_environment.install(force=False, verbose=True)
-    assert not project.default_environment.is_consistent
-
-    stdout = capsys.readouterr().out
-    assert "The environment exists but does not match the locked dependencies" in stdout
 
 
 @pytest.mark.slow
-def test_is_prepared_source_changed(project_directory_factory, capsys):
-    env_yaml = dedent(
-        """\
-        name: test
-        dependencies: [python=3.8]
-        """
-    )
-    project_path = project_directory_factory(env_yaml=env_yaml)
-    project = CondaProject(project_path)
+def test_lock_message_supplied_platforms(
+    project_directory_factory, mocker: MockerFixture
+):
+    import conda_project.project
 
-    _ = project.default_environment.install()
-    assert project.default_environment.is_locked
-    assert project.default_environment.is_consistent
+    spinner = mocker.spy(conda_project.project, "Spinner")
 
-    _ = call_conda(
-        ["install", "-p", str(project.default_environment.prefix), "requests", "-y"]
-    )
-
-    assert project.default_environment.is_locked
-    assert not project.default_environment.is_consistent
-
-    _ = project.default_environment.install(force=False, verbose=True)
-    assert not project.default_environment.is_consistent
-
-    stdout = capsys.readouterr().out
-    assert "The environment exists but does not match the locked dependencies" in stdout
-
-
-def test_install_env_exists(project_directory_factory, capsys):
     env_yaml = dedent(
         """\
         name: test
-        dependencies: []
+        dependencies:
+          - python=3.8
+        platforms: [osx-arm64, linux-64]
         """
     )
     project_path = project_directory_factory(env_yaml=env_yaml)
-    project = CondaProject(project_path)
 
-    env_dir = project.default_environment.install(verbose=True)
+    project = CondaProject(project_path)
+    project.default_environment.lock(verbose=True)
 
-    stdout = capsys.readouterr().out
-    assert f"environment created at {env_dir}" in stdout
+    assert (
+        spinner.call_args.kwargs["prefix"]
+        == "Locking dependencies for environment default on platforms linux-64, osx-arm64"
+    )
 
-    _ = project.default_environment.install(verbose=True)
 
-    stdout = capsys.readouterr().out
-    assert "The environment already exists" in stdout
+@pytest.mark.slow
+def test_lock_message_default_platforms(
+    project_directory_factory, mocker: MockerFixture
+):
+    import conda_project.project
 
+    spinner = mocker.spy(conda_project.project, "Spinner")
 
-@pytest.mark.slow
-def test_install_and_clean(project_directory_factory):
     env_yaml = dedent(
         """\
         name: test
         dependencies:
           - python=3.8
         """
     )
     project_path = project_directory_factory(env_yaml=env_yaml)
 
     project = CondaProject(project_path)
-    env_dir = project.default_environment.install()
-    assert env_dir.samefile(project_path / "envs" / "default")
-
-    conda_history = env_dir / "conda-meta" / "history"
-    assert conda_history.exists()
-
-    with conda_history.open() as f:
-        assert "create -y --file" in f.read()
-    conda_history_mtime = os.path.getmtime(conda_history)
-
-    project.default_environment.install()
-    assert conda_history_mtime == os.path.getmtime(conda_history)
-
-    project.default_environment.install(force=True)
-    assert conda_history_mtime < os.path.getmtime(conda_history)
+    project.default_environment.lock(verbose=True)
 
-    project.default_environment.clean()
-    assert not conda_history.exists()
-    assert not project.default_environment.is_consistent
+    platforms = ", ".join(sorted(DEFAULT_PLATFORMS))
+    assert (
+        spinner.call_args.kwargs["prefix"]
+        == f"Locking dependencies for environment default on platforms {platforms}"
+    )
 
 
-@pytest.mark.slow
-def test_lock(project_directory_factory):
+def test_lock_failed_from_conda(project_directory_factory):
     env_yaml = dedent(
         """\
         name: test
-        dependencies:
-          - python=3.8
+        dependencies: []
         """
     )
-    project_path = project_directory_factory(env_yaml=env_yaml)
+    condarc = "channels: {___}"
+    project_path = project_directory_factory(
+        env_yaml=env_yaml, files={".condarc": condarc}
+    )
 
     project = CondaProject(project_path)
-    project.default_environment.lock()
-
-    lockfile = project_path / "conda-lock.default.yml"
-    assert lockfile == project.default_environment.lockfile
-    assert lockfile.exists()
-    assert project.default_environment.is_locked
+    with pytest.raises(CondaProjectLockFailed):
+        project.default_environment.lock()
 
 
 def test_lock_no_channels(project_directory_factory):
     env_yaml = dedent(
         """\
         name: test
         dependencies: []
@@ -479,64 +224,14 @@
 
     with project.default_environment.lockfile.open() as f:
         lock = YAML().load(f)
 
     assert lock["metadata"]["platforms"] == ["linux-64", "osx-64"]
 
 
-def test_lock_wrong_platform(project_directory_factory):
-    env_yaml = dedent(
-        """\
-        name: test
-        dependencies: []
-        platforms: [dummy-platform]
-        """
-    )
-
-    project_path = project_directory_factory(env_yaml=env_yaml)
-
-    project = CondaProject(project_path)
-    project.default_environment.lock()
-    assert project.default_environment.is_locked
-
-    with pytest.raises(CondaProjectError) as e:
-        project.default_environment.install()
-    assert "not in the supported locked platforms" in str(e.value)
-
-
-def test_install_as_platform(project_directory_factory):
-    env_yaml = dedent(
-        """\
-        name: test
-        dependencies: []
-        platforms: [dummy-platform]
-        """
-    )
-
-    project_path = project_directory_factory(env_yaml=env_yaml)
-
-    project = CondaProject(project_path)
-    project.default_environment.lock()
-    assert project.default_environment.is_locked
-
-    project.default_environment.install(as_platform="dummy-platform")
-
-    with project.default_environment.prefix / "condarc" as f:
-        env_condarc = YAML().load(f)
-
-    assert env_condarc["subdir"] == "dummy-platform"
-
-    project.default_environment.install(force=True)
-
-    with project.default_environment.prefix / "condarc" as f:
-        env_condarc = YAML().load(f)
-
-    assert env_condarc["subdir"] == "dummy-platform"
-
-
 def test_force_relock(project_directory_factory, capsys):
     env_yaml = dedent(
         """\
         name: test
         dependencies: []
         """
     )
@@ -711,42 +406,14 @@
     assert "python" in [p["name"] for p in lock["package"]]
     assert "requests" in [p["name"] for p in lock["package"]]
     assert "_bad-package-8933" not in [p["name"] for p in lock["package"]]
 
     assert lockfile_mtime == os.path.getmtime(project.default_environment.lockfile)
 
 
-def test_install_relocks(project_directory_factory, capsys):
-    env_yaml = dedent(
-        """\
-        name: test
-        dependencies: []
-        """
-    )
-    project_path = project_directory_factory(env_yaml=env_yaml)
-
-    project = CondaProject(project_path)
-    project.default_environment.lock(verbose=True)
-    assert project.default_environment.is_locked
-
-    updated_env_yaml = dedent(
-        """\
-        name: test
-        dependencies:
-          - python=3.8
-        """
-    )
-    with (project.default_environment.sources[0]).open("wt") as f:
-        f.write(updated_env_yaml)
-
-    project.default_environment.install(verbose=True, force=True)
-
-    assert "is out-of-date, re-locking" in capsys.readouterr().out
-
-
 def test_project_named_environment(project_directory_factory):
     env_yaml = "dependencies: []\n"
 
     project_yaml = dedent(
         f"""\
         name: test
         environments:
@@ -797,45 +464,14 @@
                 project_directory_factory._suffix
             )
         )
     )
     assert project.default_environment == project.environments["my-env"]
 
 
-def test_install_named_environment(project_directory_factory):
-    env_yaml = "dependencies: []\n"
-
-    project_yaml = dedent(
-        f"""\
-        name: test
-        environments:
-          standard: [environment{project_directory_factory._suffix}]
-        """
-    )
-
-    project_path = project_directory_factory(
-        env_yaml=env_yaml, project_yaml=project_yaml
-    )
-    project = CondaProject(project_path)
-    project.default_environment.lock()
-    env_dir = project.default_environment.install()
-
-    assert project.environments["standard"].lockfile.samefile(
-        project_path / "conda-lock.standard.yml"
-    )
-    assert project.environments["standard"].prefix.samefile(
-        project_path / "envs" / "standard"
-    )
-
-    assert env_dir.samefile(project_path / "envs" / "standard")
-
-    conda_history = env_dir / "conda-meta" / "history"
-    assert conda_history.exists()
-
-
 def test_project_environments_immutable(project_directory_factory):
     env_yaml = "dependencies: []\n"
 
     project_yaml = dedent(
         f"""\
         name: test
         environments:
```

### Comparing `conda-project-0.2.0/tests/test_project_file.py` & `conda-project-0.2.1/tests/test_project_file.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.2.0/tests/test_utils.py` & `conda-project-0.2.1/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 
 import pytest
 from shellingham import ShellDetectionFailure
 
 from conda_project.exceptions import CondaProjectError
 from conda_project.utils import (
+    dedupe_list_of_dicts,
     detect_shell,
     env_variable,
     execvped,
     find_file,
     is_windows,
     prepare_variables,
 )
@@ -269,7 +270,29 @@
         "conda_project.utils.shellingham.detect_shell",
         side_effect=ShellDetectionFailure(),
     )
     mocker.patch("os.name", return_value="nope")
 
     with pytest.raises(RuntimeError):
         _ = detect_shell()
+
+
+def test_dedupe_list_of_dicts():
+    duplicated = [
+        {"name": "aaa", "k1": "cat1"},  # <-- keep this
+        {"name": "bbb", "k1": "cat1"},
+        {"name": "ccc", "k1": "cat2"},
+        {"name": "aaa", "k1": "cat2"},
+        {"name": "ddd", "k1": "cat2"},
+        {"name": "ccc", "k1": "cat1"},  # <-- keep this
+    ]
+
+    deupded = dedupe_list_of_dicts(
+        duplicated, lambda x: x["name"], lambda x: x["k1"] == "cat1"
+    )
+
+    assert deupded == [
+        {"name": "aaa", "k1": "cat1"},
+        {"name": "bbb", "k1": "cat1"},
+        {"name": "ccc", "k1": "cat1"},
+        {"name": "ddd", "k1": "cat2"},
+    ]
```

