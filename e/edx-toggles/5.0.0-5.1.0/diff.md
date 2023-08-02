# Comparing `tmp/edx-toggles-5.0.0.tar.gz` & `tmp/edx-toggles-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-toggles-5.0.0.tar", last modified: Wed May 11 19:05:08 2022, max compression
+gzip compressed data, was "edx-toggles-5.1.0.tar", last modified: Wed Aug  2 18:06:25 2023, max compression
```

## Comparing `edx-toggles-5.0.0.tar` & `edx-toggles-5.1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 19:05:08.170622 edx-toggles-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     9059 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35119 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12725 2022-05-11 19:05:08.170622 edx-toggles-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 19:05:08.166622 edx-toggles-5.0.0/edx_toggles/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 19:05:08.170622 edx-toggles-5.0.0/edx_toggles/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2599 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/tests/test_setting_toggles.py
--rw-r--r--   0 runner    (1001) docker     (121)     5492 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     3668 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/tests/test_testutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/tests/test_waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 19:05:08.170622 edx-toggles-5.0.0/edx_toggles/toggles/
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 19:05:08.170622 edx-toggles-5.0.0/edx_toggles/toggles/internal/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/internal/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/internal/setting_toggle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 19:05:08.170622 edx-toggles-5.0.0/edx_toggles/toggles/internal/waffle/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/internal/waffle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/internal/waffle/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/internal/waffle/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/internal/waffle/flag.py
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/internal/waffle/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 19:05:08.170622 edx-toggles-5.0.0/edx_toggles/toggles/state/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 19:05:08.170622 edx-toggles-5.0.0/edx_toggles/toggles/state/internal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/state/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8852 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/state/internal/report.py
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/toggles/testutils.py
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/edx_toggles/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 19:05:08.166622 edx-toggles-5.0.0/edx_toggles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12725 2022-05-11 19:05:08.000000 edx-toggles-5.0.0/edx_toggles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-05-11 19:05:08.000000 edx-toggles-5.0.0/edx_toggles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-11 19:05:08.000000 edx-toggles-5.0.0/edx_toggles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-11 19:05:08.000000 edx-toggles-5.0.0/edx_toggles.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-11 19:05:08.000000 edx-toggles-5.0.0/edx_toggles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-05-11 19:05:08.000000 edx-toggles-5.0.0/edx_toggles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-11 19:05:08.000000 edx-toggles-5.0.0/edx_toggles.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-11 19:05:08.170622 edx-toggles-5.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-05-11 19:05:08.170622 edx-toggles-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5308 2022-05-11 19:05:04.000000 edx-toggles-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:06:25.228938 edx-toggles-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     9308 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35119 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    12859 2023-08-02 18:06:25.228938 edx-toggles-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:06:25.224938 edx-toggles-5.1.0/edx_toggles/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      446 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:06:25.224938 edx-toggles-5.1.0/edx_toggles/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2599 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/tests/test_setting_toggles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5492 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3668 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/tests/test_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2092 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/tests/test_waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:06:25.224938 edx-toggles-5.1.0/edx_toggles/toggles/
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:06:25.224938 edx-toggles-5.1.0/edx_toggles/toggles/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/internal/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/internal/setting_toggle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:06:25.224938 edx-toggles-5.1.0/edx_toggles/toggles/internal/waffle/
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/internal/waffle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/internal/waffle/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/internal/waffle/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3424 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/internal/waffle/flag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/internal/waffle/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:06:25.224938 edx-toggles-5.1.0/edx_toggles/toggles/state/
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:06:25.224938 edx-toggles-5.1.0/edx_toggles/toggles/state/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/state/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8852 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/state/internal/report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2798 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/toggles/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/edx_toggles/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:06:25.224938 edx-toggles-5.1.0/edx_toggles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    12859 2023-08-02 18:06:25.000000 edx-toggles-5.1.0/edx_toggles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-08-02 18:06:25.000000 edx-toggles-5.1.0/edx_toggles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 18:06:25.000000 edx-toggles-5.1.0/edx_toggles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-08-02 18:06:25.000000 edx-toggles-5.1.0/edx_toggles.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 18:06:25.000000 edx-toggles-5.1.0/edx_toggles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-08-02 18:06:25.000000 edx-toggles-5.1.0/edx_toggles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-02 18:06:25.000000 edx-toggles-5.1.0/edx_toggles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:06:25.228938 edx-toggles-5.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-08-02 18:06:25.228938 edx-toggles-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5312 2023-08-02 18:06:20.000000 edx-toggles-5.1.0/setup.py
```

### Comparing `edx-toggles-5.0.0/CHANGELOG.rst` & `edx-toggles-5.1.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[5.1.0] - 2023-08-02
+--------------------
+
+* Added support for Django 4.2
+* Rename toggle_warnings to toggle_warning for consistency with setting_warning.
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
 [5.0.0] - 2022-04-22
 --------------------
 
 * BREAKING CHANGE: Removed LegacyWaffle* classes. Although this is a breaking change, all known uses have already been fixed.
 * Handle the case where certain toggle names come in as ``None`` when generating summary reports.
 * Add ADR for updating annotations for toggle life expectancy and use cases.
```

### Comparing `edx-toggles-5.0.0/LICENSE.txt` & `edx-toggles-5.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/PKG-INFO` & `edx-toggles-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edx-toggles
-Version: 5.0.0
+Version: 5.1.0
 Summary: Library and utilities for feature toggles
-Home-page: https://github.com/edx/edx-toggles
+Home-page: https://github.com/openedx/edx-toggles
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
@@ -26,44 +25,42 @@
 |license-badge|
 
 Library and utilities for implementing and reporting on feature toggles.
 
 Documentation is on `Read the Docs`_.  Code repository is on `GitHub`_.
 
 .. _Read the Docs: https://edx.readthedocs.io/projects/edx-toggles/en/latest/readme.html
-.. _GitHub: https://github.com/edx/edx-toggles
+.. _GitHub: https://github.com/openedx/edx-toggles
 
 See the `scripts README`_ for more information on the scripts for reporting on the status of
 feature toggles.
 
-.. _scripts README: https://github.com/edx/edx-toggles/blob/master/scripts/README.rst
+.. _scripts README: https://github.com/openedx/edx-toggles/blob/master/scripts/README.rst
 
 License
 -------
 
 The code in this repository is licensed under the AGPL 3.0 unless
 otherwise noted.
 
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/edx-toggles/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-toggles/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/edx-toggles/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-toggles/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -75,16 +72,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-toggles.svg
     :target: https://pypi.python.org/pypi/edx-toggles/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/edx-toggles/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/edx-toggles/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/edx-toggles/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/edx-toggles/actions?query=workflow%3A%22Python+CI%22
     :alt: Github CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/edx-toggles/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/edx-toggles?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/edx-toggles/badge/?version=latest
@@ -92,15 +89,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-toggles.svg
     :target: https://pypi.python.org/pypi/edx-toggles/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/edx-toggles.svg
-    :target: https://github.com/edx/edx-toggles/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/edx-toggles/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -112,14 +109,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[5.1.0] - 2023-08-02
+--------------------
+
+* Added support for Django 4.2
+* Rename toggle_warnings to toggle_warning for consistency with setting_warning.
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
 [5.0.0] - 2022-04-22
 --------------------
 
 * BREAKING CHANGE: Removed LegacyWaffle* classes. Although this is a breaking change, all known uses have already been fixed.
 * Handle the case where certain toggle names come in as ``None`` when generating summary reports.
 * Add ADR for updating annotations for toggle life expectancy and use cases.
 
@@ -277,9 +282,7 @@
 
 * Added support for python 3.8 and dropped support Django versions older than 2.2
 
 [0.1.0] - 2019-04-08
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * Initial version
-
-
```

### Comparing `edx-toggles-5.0.0/README.rst` & `edx-toggles-5.1.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -5,44 +5,42 @@
 |license-badge|
 
 Library and utilities for implementing and reporting on feature toggles.
 
 Documentation is on `Read the Docs`_.  Code repository is on `GitHub`_.
 
 .. _Read the Docs: https://edx.readthedocs.io/projects/edx-toggles/en/latest/readme.html
-.. _GitHub: https://github.com/edx/edx-toggles
+.. _GitHub: https://github.com/openedx/edx-toggles
 
 See the `scripts README`_ for more information on the scripts for reporting on the status of
 feature toggles.
 
-.. _scripts README: https://github.com/edx/edx-toggles/blob/master/scripts/README.rst
+.. _scripts README: https://github.com/openedx/edx-toggles/blob/master/scripts/README.rst
 
 License
 -------
 
 The code in this repository is licensed under the AGPL 3.0 unless
 otherwise noted.
 
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/edx-toggles/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-toggles/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/edx-toggles/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-toggles/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -54,16 +52,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-toggles.svg
     :target: https://pypi.python.org/pypi/edx-toggles/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/edx-toggles/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/edx-toggles/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/edx-toggles/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/edx-toggles/actions?query=workflow%3A%22Python+CI%22
     :alt: Github CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/edx-toggles/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/edx-toggles?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/edx-toggles/badge/?version=latest
@@ -71,9 +69,9 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-toggles.svg
     :target: https://pypi.python.org/pypi/edx-toggles/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/edx-toggles.svg
-    :target: https://github.com/edx/edx-toggles/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/edx-toggles/blob/master/LICENSE.txt
     :alt: License
```

### Comparing `edx-toggles-5.0.0/edx_toggles/tests/test_setting_toggles.py` & `edx-toggles-5.1.0/edx_toggles/tests/test_setting_toggles.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/edx_toggles/tests/test_state.py` & `edx-toggles-5.1.0/edx_toggles/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/edx_toggles/tests/test_testutils.py` & `edx-toggles-5.1.0/edx_toggles/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/edx_toggles/tests/test_waffle.py` & `edx-toggles-5.1.0/edx_toggles/tests/test_waffle.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/edx_toggles/toggles/internal/base.py` & `edx-toggles-5.1.0/edx_toggles/toggles/internal/base.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/edx_toggles/toggles/internal/setting_toggle.py` & `edx-toggles-5.1.0/edx_toggles/toggles/internal/setting_toggle.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/edx_toggles/toggles/internal/waffle/base.py` & `edx-toggles-5.1.0/edx_toggles/toggles/internal/waffle/base.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/edx_toggles/toggles/internal/waffle/flag.py` & `edx-toggles-5.1.0/edx_toggles/toggles/internal/waffle/flag.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/edx_toggles/toggles/internal/waffle/switch.py` & `edx-toggles-5.1.0/edx_toggles/toggles/internal/waffle/switch.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/edx_toggles/toggles/state/internal/report.py` & `edx-toggles-5.1.0/edx_toggles/toggles/state/internal/report.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/edx_toggles/toggles/testutils.py` & `edx-toggles-5.1.0/edx_toggles/toggles/testutils.py`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/edx_toggles.egg-info/PKG-INFO` & `edx-toggles-5.1.0/edx_toggles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edx-toggles
-Version: 5.0.0
+Version: 5.1.0
 Summary: Library and utilities for feature toggles
-Home-page: https://github.com/edx/edx-toggles
+Home-page: https://github.com/openedx/edx-toggles
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
@@ -26,44 +25,42 @@
 |license-badge|
 
 Library and utilities for implementing and reporting on feature toggles.
 
 Documentation is on `Read the Docs`_.  Code repository is on `GitHub`_.
 
 .. _Read the Docs: https://edx.readthedocs.io/projects/edx-toggles/en/latest/readme.html
-.. _GitHub: https://github.com/edx/edx-toggles
+.. _GitHub: https://github.com/openedx/edx-toggles
 
 See the `scripts README`_ for more information on the scripts for reporting on the status of
 feature toggles.
 
-.. _scripts README: https://github.com/edx/edx-toggles/blob/master/scripts/README.rst
+.. _scripts README: https://github.com/openedx/edx-toggles/blob/master/scripts/README.rst
 
 License
 -------
 
 The code in this repository is licensed under the AGPL 3.0 unless
 otherwise noted.
 
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/edx-toggles/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-toggles/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/edx-toggles/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-toggles/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -75,16 +72,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-toggles.svg
     :target: https://pypi.python.org/pypi/edx-toggles/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/edx-toggles/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/edx-toggles/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/edx-toggles/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/edx-toggles/actions?query=workflow%3A%22Python+CI%22
     :alt: Github CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/edx-toggles/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/edx-toggles?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/edx-toggles/badge/?version=latest
@@ -92,15 +89,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-toggles.svg
     :target: https://pypi.python.org/pypi/edx-toggles/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/edx-toggles.svg
-    :target: https://github.com/edx/edx-toggles/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/edx-toggles/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -112,14 +109,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[5.1.0] - 2023-08-02
+--------------------
+
+* Added support for Django 4.2
+* Rename toggle_warnings to toggle_warning for consistency with setting_warning.
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
 [5.0.0] - 2022-04-22
 --------------------
 
 * BREAKING CHANGE: Removed LegacyWaffle* classes. Although this is a breaking change, all known uses have already been fixed.
 * Handle the case where certain toggle names come in as ``None`` when generating summary reports.
 * Add ADR for updating annotations for toggle life expectancy and use cases.
 
@@ -277,9 +282,7 @@
 
 * Added support for python 3.8 and dropped support Django versions older than 2.2
 
 [0.1.0] - 2019-04-08
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * Initial version
-
-
```

### Comparing `edx-toggles-5.0.0/edx_toggles.egg-info/SOURCES.txt` & `edx-toggles-5.1.0/edx_toggles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-toggles-5.0.0/setup.py` & `edx-toggles-5.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 setup(
     name='edx-toggles',
     version=VERSION,
     description="""Library and utilities for feature toggles""",
     long_description=README + '\n\n' + CHANGELOG,
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/edx-toggles',
+    url='https://github.com/openedx/edx-toggles',
     packages=[
         'edx_toggles',
     ],
     entry_points={
         "lms.djangoapp": [
             "toggles = edx_toggles.apps:TogglesConfig",
         ],
```

