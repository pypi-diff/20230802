# Comparing `tmp/iqm-cortex-cli-4.4.tar.gz` & `tmp/iqm-cortex-cli-4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqm-cortex-cli-4.4.tar", last modified: Thu Jul 13 07:33:42 2023, max compression
+gzip compressed data, was "iqm-cortex-cli-4.5.tar", last modified: Wed Aug  2 08:58:31 2023, max compression
```

## Comparing `iqm-cortex-cli-4.4.tar` & `iqm-cortex-cli-4.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.081749 iqm-cortex-cli-4.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.073748 iqm-cortex-cli-4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.073748 iqm-cortex-cli-4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/DEVELOPMENT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-07-13 07:33:42.081749 iqm-cortex-cli-4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.073748 iqm-cortex-cli-4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.073748 iqm-cortex-cli-4.4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.077748 iqm-cortex-cli-4.4/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   618471 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.077748 iqm-cortex-cli-4.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 07:33:42.081749 iqm-cortex-cli-4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.073748 iqm-cortex-cli-4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.077748 iqm-cortex-cli-4.4/src/cortex_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/src/cortex_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/src/cortex_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    27269 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/src/cortex_cli/cortex_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/src/cortex_cli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/src/cortex_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/src/cortex_cli/token_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.077748 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-07-13 07:33:42.000000 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-13 07:33:42.000000 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:33:42.000000 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 07:33:42.000000 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-13 07:33:42.000000 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 07:33:42.000000 iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.081749 iqm-cortex-cli-4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/cortex_cli_auth_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/cortex_cli_auth_logout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/cortex_cli_auth_status_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/cortex_cli_init_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/cortex_cli_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:33:42.081749 iqm-cortex-cli-4.4/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/resources/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/resources/tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tests/token_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-13 07:33:06.000000 iqm-cortex-cli-4.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:58:31.954783 iqm-cortex-cli-4.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:58:31.946783 iqm-cortex-cli-4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:58:31.946783 iqm-cortex-cli-4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/DEVELOPMENT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-08-02 08:58:31.954783 iqm-cortex-cli-4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:58:31.950783 iqm-cortex-cli-4.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:58:31.946783 iqm-cortex-cli-4.5/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:58:31.950783 iqm-cortex-cli-4.5/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   618471 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:58:31.950783 iqm-cortex-cli-4.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 08:58:31.954783 iqm-cortex-cli-4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:58:31.946783 iqm-cortex-cli-4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:58:31.950783 iqm-cortex-cli-4.5/src/cortex_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/src/cortex_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/src/cortex_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27269 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/src/cortex_cli/cortex_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/src/cortex_cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/src/cortex_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/src/cortex_cli/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:58:31.950783 iqm-cortex-cli-4.5/src/iqm_cortex_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-08-02 08:58:31.000000 iqm-cortex-cli-4.5/src/iqm_cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-02 08:58:31.000000 iqm-cortex-cli-4.5/src/iqm_cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 08:58:31.000000 iqm-cortex-cli-4.5/src/iqm_cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 08:58:31.000000 iqm-cortex-cli-4.5/src/iqm_cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-02 08:58:31.000000 iqm-cortex-cli-4.5/src/iqm_cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 08:58:31.000000 iqm-cortex-cli-4.5/src/iqm_cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:58:31.954783 iqm-cortex-cli-4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tests/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tests/cortex_cli_auth_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tests/cortex_cli_auth_logout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tests/cortex_cli_auth_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tests/cortex_cli_init_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tests/cortex_cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:58:31.954783 iqm-cortex-cli-4.5/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tests/resources/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tests/resources/tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tests/token_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-02 08:57:57.000000 iqm-cortex-cli-4.5/tox.ini
```

### Comparing `iqm-cortex-cli-4.4/.github/workflows/ci.yml` & `iqm-cortex-cli-4.5/.github/workflows/ci.yml`

 * *Files 26% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 jobs:
   test:
     runs-on: ${{ matrix.platform }}
 
     strategy:
       matrix:
         platform: [ ubuntu-latest, macos-latest, windows-latest ]
-        python-version: [ '3.9', '3.10.6' ]
-        # Replace 3.10.6 with 3.10 when mypy bug is fixed
-        # https://github.com/python/mypy/issues/13627
+        python-version: [ '3.9', '3.10', '3.11' ]
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v4
```

### Comparing `iqm-cortex-cli-4.4/.github/workflows/publish.yml` & `iqm-cortex-cli-4.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/.github/workflows/tag_and_release.yml` & `iqm-cortex-cli-4.5/.github/workflows/tag_and_release.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/CHANGELOG.rst` & `iqm-cortex-cli-4.5/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 =========
 Changelog
 =========
 
+Version 4.5
+===========
+
+* Support python 3.11 `#53 <https://github.com/iqm-finland/cortex-cli/pull/53>`_
+
 Version 4.4
 ===========
 
 * Support relative paths during init `#52 <https://github.com/iqm-finland/cortex-cli/pull/52>`_
 
-
 Version 4.3
 ===========
 
 * Fix logging for multi-user systems `#48 <https://github.com/iqm-finland/cortex-cli/pull/48>`_
 
 Version 4.2
 ===========
@@ -24,15 +28,14 @@
 * Generate license information for dependencies on every release `#44 <https://github.com/iqm-finland/cortex-cli/pull/44>`_
 
 Version 4.0
 ===========
 
 * Remove circuit execution command `#43 <https://github.com/iqm-finland/cortex-cli/pull/43>`_
 
-
 Version 3.6
 ============
 
 * Upgrade to IQMClient version 12.0 `#42 <https://github.com/iqm-finland/cortex-cli/pull/42>`_
 
 Version 3.5
 ===========
```

### Comparing `iqm-cortex-cli-4.4/DEVELOPMENT.rst` & `iqm-cortex-cli-4.5/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/LICENSE.rst` & `iqm-cortex-cli-4.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/PKG-INFO` & `iqm-cortex-cli-4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-cortex-cli
-Version: 4.4
+Version: 4.5
 Summary: CLI for managing user authentication when using IQM quantum computers
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Project-URL: repository, https://github.com/iqm-finland/cortex-cli.git
 Project-URL: changelog, https://github.com/iqm-finland/cortex-cli/blob/main/CHANGELOG.rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: <3.11,>=3.9
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: testing
 Provides-Extra: docs
 Provides-Extra: cicd
 License-File: LICENSE.rst
 License-File: AUTHORS.rst
```

### Comparing `iqm-cortex-cli-4.4/README.rst` & `iqm-cortex-cli-4.5/README.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/docs/Makefile` & `iqm-cortex-cli-4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/docs/_static/images/favicon.ico` & `iqm-cortex-cli-4.5/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/docs/_static/images/logo.png` & `iqm-cortex-cli-4.5/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/docs/_templates/autosummary-class-template.rst` & `iqm-cortex-cli-4.5/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/docs/_templates/autosummary-module-template.rst` & `iqm-cortex-cli-4.5/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/docs/_templates/page.html` & `iqm-cortex-cli-4.5/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/docs/_templates/versioning.html` & `iqm-cortex-cli-4.5/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/docs/conf.py` & `iqm-cortex-cli-4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/pyproject.toml` & `iqm-cortex-cli-4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Physics",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License"
 ]
-requires-python = ">=3.9, <3.11"
+requires-python = ">=3.9, <3.12"
 dependencies = [
     "click >= 7.1.2, < 8.1.4",  # upper limit until https://github.com/pallets/click/issues/2558 is fixed
     "jsonschema >= 4.6.0",
     "mechanize >= 0.4.8",
     "psutil >= 5.9.2",
     "pydantic >= 1.10.2, < 2.0",
     "python-daemon >= 2.3.0",
```

### Comparing `iqm-cortex-cli-4.4/src/cortex_cli/__init__.py` & `iqm-cortex-cli-4.5/src/cortex_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/src/cortex_cli/auth.py` & `iqm-cortex-cli-4.5/src/cortex_cli/auth.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/src/cortex_cli/cortex_cli.py` & `iqm-cortex-cli-4.5/src/cortex_cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/src/cortex_cli/models.py` & `iqm-cortex-cli-4.5/src/cortex_cli/models.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/src/cortex_cli/token_manager.py` & `iqm-cortex-cli-4.5/src/cortex_cli/token_manager.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/PKG-INFO` & `iqm-cortex-cli-4.5/src/iqm_cortex_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-cortex-cli
-Version: 4.4
+Version: 4.5
 Summary: CLI for managing user authentication when using IQM quantum computers
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Project-URL: repository, https://github.com/iqm-finland/cortex-cli.git
 Project-URL: changelog, https://github.com/iqm-finland/cortex-cli/blob/main/CHANGELOG.rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: <3.11,>=3.9
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: testing
 Provides-Extra: docs
 Provides-Extra: cicd
 License-File: LICENSE.rst
 License-File: AUTHORS.rst
```

### Comparing `iqm-cortex-cli-4.4/src/iqm_cortex_cli.egg-info/SOURCES.txt` & `iqm-cortex-cli-4.5/src/iqm_cortex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/tag-from-pipeline.sh` & `iqm-cortex-cli-4.5/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/tests/auth_test.py` & `iqm-cortex-cli-4.5/tests/auth_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/tests/conftest.py` & `iqm-cortex-cli-4.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/tests/cortex_cli_auth_login_test.py` & `iqm-cortex-cli-4.5/tests/cortex_cli_auth_login_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/tests/cortex_cli_auth_logout_test.py` & `iqm-cortex-cli-4.5/tests/cortex_cli_auth_logout_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/tests/cortex_cli_auth_status_test.py` & `iqm-cortex-cli-4.5/tests/cortex_cli_auth_status_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/tests/cortex_cli_init_test.py` & `iqm-cortex-cli-4.5/tests/cortex_cli_init_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/tests/cortex_cli_test.py` & `iqm-cortex-cli-4.5/tests/cortex_cli_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/tests/resources/tokens.json` & `iqm-cortex-cli-4.5/tests/resources/tokens.json`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/tests/token_manager_test.py` & `iqm-cortex-cli-4.5/tests/token_manager_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.4/tox.ini` & `iqm-cortex-cli-4.5/tox.ini`

 * *Files identical despite different names*

