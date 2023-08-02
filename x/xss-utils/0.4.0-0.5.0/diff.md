# Comparing `tmp/xss-utils-0.4.0.tar.gz` & `tmp/xss-utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xss-utils-0.4.0.tar", last modified: Thu Jan 20 10:57:56 2022, max compression
+gzip compressed data, was "xss-utils-0.5.0.tar", last modified: Wed Aug  2 13:27:49 2023, max compression
```

## Comparing `xss-utils-0.4.0.tar` & `xss-utils-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:57:56.277706 xss-utils-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-20 10:57:53.000000 xss-utils-0.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-01-20 10:57:53.000000 xss-utils-0.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    34520 2022-01-20 10:57:53.000000 xss-utils-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-01-20 10:57:53.000000 xss-utils-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4726 2022-01-20 10:57:56.277706 xss-utils-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3018 2022-01-20 10:57:53.000000 xss-utils-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:57:56.277706 xss-utils-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-01-20 10:57:53.000000 xss-utils-0.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-01-20 10:57:53.000000 xss-utils-0.4.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-01-20 10:57:56.277706 xss-utils-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5524 2022-01-20 10:57:53.000000 xss-utils-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:57:56.277706 xss-utils-0.4.0/xss_utils/
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-01-20 10:57:53.000000 xss-utils-0.4.0/xss_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-01-20 10:57:53.000000 xss-utils-0.4.0/xss_utils/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:57:56.277706 xss-utils-0.4.0/xss_utils/mako/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-20 10:57:53.000000 xss-utils-0.4.0/xss_utils/mako/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:57:56.277706 xss-utils-0.4.0/xss_utils/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-20 10:57:53.000000 xss-utils-0.4.0/xss_utils/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-01-20 10:57:53.000000 xss-utils-0.4.0/xss_utils/templatetags/django_markup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:57:56.277706 xss-utils-0.4.0/xss_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-20 10:57:53.000000 xss-utils-0.4.0/xss_utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-01-20 10:57:53.000000 xss-utils-0.4.0/xss_utils/tests/test_templatetags.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:57:56.277706 xss-utils-0.4.0/xss_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4726 2022-01-20 10:57:56.000000 xss-utils-0.4.0/xss_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-01-20 10:57:56.000000 xss-utils-0.4.0/xss_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-20 10:57:56.000000 xss-utils-0.4.0/xss_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-20 10:57:56.000000 xss-utils-0.4.0/xss_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-01-20 10:57:56.000000 xss-utils-0.4.0/xss_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-20 10:57:56.000000 xss-utils-0.4.0/xss_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 13:27:49.883426 xss-utils-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-02 13:27:45.000000 xss-utils-0.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-08-02 13:27:45.000000 xss-utils-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-08-02 13:27:45.000000 xss-utils-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-08-02 13:27:45.000000 xss-utils-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4879 2023-08-02 13:27:49.883426 xss-utils-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-08-02 13:27:45.000000 xss-utils-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 13:27:49.883426 xss-utils-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-08-02 13:27:45.000000 xss-utils-0.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-08-02 13:27:45.000000 xss-utils-0.5.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-08-02 13:27:49.883426 xss-utils-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5528 2023-08-02 13:27:45.000000 xss-utils-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 13:27:49.883426 xss-utils-0.5.0/xss_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-08-02 13:27:45.000000 xss-utils-0.5.0/xss_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-08-02 13:27:45.000000 xss-utils-0.5.0/xss_utils/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 13:27:49.883426 xss-utils-0.5.0/xss_utils/mako/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 13:27:45.000000 xss-utils-0.5.0/xss_utils/mako/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 13:27:49.883426 xss-utils-0.5.0/xss_utils/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 13:27:45.000000 xss-utils-0.5.0/xss_utils/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-08-02 13:27:45.000000 xss-utils-0.5.0/xss_utils/templatetags/django_markup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 13:27:49.883426 xss-utils-0.5.0/xss_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 13:27:45.000000 xss-utils-0.5.0/xss_utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-08-02 13:27:45.000000 xss-utils-0.5.0/xss_utils/tests/test_templatetags.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 13:27:49.883426 xss-utils-0.5.0/xss_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4879 2023-08-02 13:27:49.000000 xss-utils-0.5.0/xss_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-08-02 13:27:49.000000 xss-utils-0.5.0/xss_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 13:27:49.000000 xss-utils-0.5.0/xss_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 13:27:49.000000 xss-utils-0.5.0/xss_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-08-02 13:27:49.000000 xss-utils-0.5.0/xss_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-02 13:27:49.000000 xss-utils-0.5.0/xss_utils.egg-info/top_level.txt
```

### Comparing `xss-utils-0.4.0/CHANGELOG.rst` & `xss-utils-0.5.0/CHANGELOG.rst`

 * *Files 19% similar despite different names*

```diff
@@ -10,16 +10,22 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
-*
+[0.5.0] - 2023-08-01
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+* Added supportt for Django 4.2
+  
 [0.4.0] - 2022-01-20
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * Added Support for Django40
```

### Comparing `xss-utils-0.4.0/LICENSE` & `xss-utils-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xss-utils-0.4.0/PKG-INFO` & `xss-utils-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: xss-utils
-Version: 0.4.0
+Version: 0.5.0
 Summary: Utility functions to prevent possible XSS attack on django/mako templates
-Home-page: https://github.com/edx/xss-utils
+Home-page: https://github.com/openedx/xss-utils
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
@@ -48,24 +47,21 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/xss-utils/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/xss-utils/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/xss-utils/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/xss-utils/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -77,16 +73,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/xss-utils.svg
     :target: https://pypi.python.org/pypi/xss-utils/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/xss-utils/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/xss-utils/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/xss-utils/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/xss-utils/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/xss-utils/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/xss-utils?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/xss-utils/badge/?version=latest
@@ -94,15 +90,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/xss-utils.svg
     :target: https://pypi.python.org/pypi/xss-utils/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/xss-utils.svg
-    :target: https://github.com/edx/xss-utils/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/xss-utils/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -114,16 +110,22 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
-*
+[0.5.0] - 2023-08-01
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+* Added supportt for Django 4.2
+  
 [0.4.0] - 2022-01-20
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * Added Support for Django40
@@ -144,9 +146,7 @@
 [0.1.0] - 2018-08-17
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * Utilities to enable html escaping, preventing Cross Site Scripting (XSS) attacks in Django templates.
-
-
```

### Comparing `xss-utils-0.4.0/README.rst` & `xss-utils-0.5.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -26,24 +26,21 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/xss-utils/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/xss-utils/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/xss-utils/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/xss-utils/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -55,16 +52,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/xss-utils.svg
     :target: https://pypi.python.org/pypi/xss-utils/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/xss-utils/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/xss-utils/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/xss-utils/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/xss-utils/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/xss-utils/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/xss-utils?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/xss-utils/badge/?version=latest
@@ -72,9 +69,9 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/xss-utils.svg
     :target: https://pypi.python.org/pypi/xss-utils/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/xss-utils.svg
-    :target: https://github.com/edx/xss-utils/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/xss-utils/blob/master/LICENSE.txt
     :alt: License
```

### Comparing `xss-utils-0.4.0/requirements/constraints.txt` & `xss-utils-0.5.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `xss-utils-0.4.0/setup.cfg` & `xss-utils-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `xss-utils-0.4.0/setup.py` & `xss-utils-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 setup(
     name='xss-utils',
     version=VERSION,
     description="""Utility functions to prevent possible XSS attack on django/mako templates""",
     long_description=README + '\n\n' + CHANGELOG,
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/xss-utils',
+    url='https://github.com/openedx/xss-utils',
     packages=[
         'xss_utils',
     ],
     include_package_data=True,
     install_requires=load_requirements('requirements/base.in'),
     license="AGPL 3.0",
     zip_safe=False,
```

### Comparing `xss-utils-0.4.0/xss_utils/templatetags/django_markup.py` & `xss-utils-0.5.0/xss_utils/templatetags/django_markup.py`

 * *Files identical despite different names*

### Comparing `xss-utils-0.4.0/xss_utils/tests/test_templatetags.py` & `xss-utils-0.5.0/xss_utils/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `xss-utils-0.4.0/xss_utils.egg-info/PKG-INFO` & `xss-utils-0.5.0/xss_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: xss-utils
-Version: 0.4.0
+Version: 0.5.0
 Summary: Utility functions to prevent possible XSS attack on django/mako templates
-Home-page: https://github.com/edx/xss-utils
+Home-page: https://github.com/openedx/xss-utils
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
@@ -48,24 +47,21 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/xss-utils/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/xss-utils/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/xss-utils/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/xss-utils/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -77,16 +73,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/xss-utils.svg
     :target: https://pypi.python.org/pypi/xss-utils/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/xss-utils/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/xss-utils/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/xss-utils/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/xss-utils/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/xss-utils/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/xss-utils?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/xss-utils/badge/?version=latest
@@ -94,15 +90,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/xss-utils.svg
     :target: https://pypi.python.org/pypi/xss-utils/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/xss-utils.svg
-    :target: https://github.com/edx/xss-utils/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/xss-utils/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -114,16 +110,22 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
-*
+[0.5.0] - 2023-08-01
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+* Added supportt for Django 4.2
+  
 [0.4.0] - 2022-01-20
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * Added Support for Django40
@@ -144,9 +146,7 @@
 [0.1.0] - 2018-08-17
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * Utilities to enable html escaping, preventing Cross Site Scripting (XSS) attacks in Django templates.
-
-
```

### Comparing `xss-utils-0.4.0/xss_utils.egg-info/SOURCES.txt` & `xss-utils-0.5.0/xss_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

