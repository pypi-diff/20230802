# Comparing `tmp/help-tokens-2.2.0.tar.gz` & `tmp/help-tokens-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "help-tokens-2.2.0.tar", last modified: Thu Jan 20 10:18:42 2022, max compression
+gzip compressed data, was "help-tokens-2.3.0.tar", last modified: Wed Aug  2 20:40:43 2023, max compression
```

## Comparing `help-tokens-2.2.0.tar` & `help-tokens-2.3.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:18:42.424233 help-tokens-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-01-20 10:18:39.000000 help-tokens-2.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-01-20 10:18:39.000000 help-tokens-2.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35119 2022-01-20 10:18:39.000000 help-tokens-2.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-01-20 10:18:39.000000 help-tokens-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7310 2022-01-20 10:18:42.424233 help-tokens-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5389 2022-01-20 10:18:39.000000 help-tokens-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:18:42.424233 help-tokens-2.2.0/help_tokens/
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-01-20 10:18:39.000000 help-tokens-2.2.0/help_tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-01-20 10:18:39.000000 help-tokens-2.2.0/help_tokens/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-01-20 10:18:39.000000 help-tokens-2.2.0/help_tokens/context_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-01-20 10:18:39.000000 help-tokens-2.2.0/help_tokens/core.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-01-20 10:18:39.000000 help-tokens-2.2.0/help_tokens/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-01-20 10:18:39.000000 help-tokens-2.2.0/help_tokens/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-01-20 10:18:39.000000 help-tokens-2.2.0/help_tokens/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:18:42.424233 help-tokens-2.2.0/help_tokens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7310 2022-01-20 10:18:42.000000 help-tokens-2.2.0/help_tokens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-01-20 10:18:42.000000 help-tokens-2.2.0/help_tokens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-20 10:18:42.000000 help-tokens-2.2.0/help_tokens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-20 10:18:42.000000 help-tokens-2.2.0/help_tokens.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-20 10:18:42.000000 help-tokens-2.2.0/help_tokens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-01-20 10:18:42.000000 help-tokens-2.2.0/help_tokens.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:18:42.424233 help-tokens-2.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-01-20 10:18:39.000000 help-tokens-2.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-20 10:18:39.000000 help-tokens-2.2.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-01-20 10:18:42.428233 help-tokens-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5205 2022-01-20 10:18:39.000000 help-tokens-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 20:40:43.713103 help-tokens-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-08-02 20:40:39.000000 help-tokens-2.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-08-02 20:40:39.000000 help-tokens-2.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35119 2023-08-02 20:40:39.000000 help-tokens-2.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-08-02 20:40:39.000000 help-tokens-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7299 2023-08-02 20:40:43.713103 help-tokens-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5282 2023-08-02 20:40:39.000000 help-tokens-2.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 20:40:43.709103 help-tokens-2.3.0/help_tokens/
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 20:40:39.000000 help-tokens-2.3.0/help_tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-08-02 20:40:39.000000 help-tokens-2.3.0/help_tokens/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-08-02 20:40:39.000000 help-tokens-2.3.0/help_tokens/context_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-08-02 20:40:39.000000 help-tokens-2.3.0/help_tokens/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-08-02 20:40:39.000000 help-tokens-2.3.0/help_tokens/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-08-02 20:40:39.000000 help-tokens-2.3.0/help_tokens/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-08-02 20:40:39.000000 help-tokens-2.3.0/help_tokens/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 20:40:43.713103 help-tokens-2.3.0/help_tokens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7299 2023-08-02 20:40:43.000000 help-tokens-2.3.0/help_tokens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-08-02 20:40:43.000000 help-tokens-2.3.0/help_tokens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 20:40:43.000000 help-tokens-2.3.0/help_tokens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 20:40:43.000000 help-tokens-2.3.0/help_tokens.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-02 20:40:43.000000 help-tokens-2.3.0/help_tokens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-02 20:40:43.000000 help-tokens-2.3.0/help_tokens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 20:40:43.713103 help-tokens-2.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-08-02 20:40:39.000000 help-tokens-2.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-08-02 20:40:39.000000 help-tokens-2.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-08-02 20:40:43.713103 help-tokens-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5257 2023-08-02 20:40:39.000000 help-tokens-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 20:40:43.713103 help-tokens-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-08-02 20:40:39.000000 help-tokens-2.3.0/tests/test_context_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2062 2023-08-02 20:40:39.000000 help-tokens-2.3.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-08-02 20:40:39.000000 help-tokens-2.3.0/tests/test_views.py
```

### Comparing `help-tokens-2.2.0/CHANGELOG.rst` & `help-tokens-2.3.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,19 @@
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
+[2.3.0] - 2023-08-02
+====================
+
+* Added support for Django 4.2
+
 [2.2.0] - 2022-01-20
 ====================
 
 * Dropped support for django2.2, 3.0, 3.1 and 3.2
 * Added Django40 support in CI
 
 [2.1.0] - 2020-07-07
```

### Comparing `help-tokens-2.2.0/LICENSE.txt` & `help-tokens-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `help-tokens-2.2.0/PKG-INFO` & `help-tokens-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: help-tokens
-Version: 2.2.0
+Version: 2.3.0
 Summary: Django app for linking to help pages with short tokens
-Home-page: https://github.com/edx/help-tokens
+Home-page: https://github.com/openedx/help-tokens
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS
 
 ###########
 help-tokens
 ###########
 
@@ -134,24 +134,22 @@
 noted.  Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 *****************
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from GitHub interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/help-tokens/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/help-tokens/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from GitHub UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/help-tokens/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/help-tokens/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 *************************
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -163,28 +161,28 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/help-tokens.svg
     :target: https://pypi.python.org/pypi/help-tokens/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/help-tokens/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/help-tokens/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/help-tokens/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/help-tokens/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/help-tokens/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/help-tokens?branch=master
     :alt: Codecov
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/help-tokens.svg
     :target: https://pypi.python.org/pypi/help-tokens/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/help-tokens.svg
-    :target: https://github.com/edx/help-tokens/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/help-tokens/blob/master/LICENSE.txt
     :alt: License
 
 
 
 Change Log
 **********
 
@@ -194,14 +192,19 @@
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
+[2.3.0] - 2023-08-02
+====================
+
+* Added support for Django 4.2
+
 [2.2.0] - 2022-01-20
 ====================
 
 * Dropped support for django2.2, 3.0, 3.1 and 3.2
 * Added Django40 support in CI
 
 [2.1.0] - 2020-07-07
@@ -239,9 +242,7 @@
 * First version on PyPI.
 
 
 [1.0.0] - 2017-05-03
 ====================
 
 * First release.
-
-
```

#### html2text {}

```diff
@@ -1,94 +1,94 @@
-Metadata-Version: 2.1 Name: help-tokens Version: 2.2.0 Summary: Django app for
-linking to help pages with short tokens Home-page: https://github.com/edx/help-
-tokens Author: edX Author-email: oscm@edx.org License: AGPL 3.0 Keywords:
-Django edx Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
-Stable Classifier: Framework :: Django Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0 Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: GNU Affero General Public
-License v3 or later (AGPLv3+) Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 License-File: LICENSE.txt License-File: AUTHORS
-########### help-tokens ########### Django app for linking to help pages with
-short tokens. |pypi-badge| |ci-badge| |codecov-badge| |pyversions-badge|
-|license-badge| Overview ******** There are various factors that affect what
-help page an application should link to: - There may be a number of relevant
-books - The version of the application might affect which book to display - The
-application's language might affect which book to display This small Django app
-provides a means to use "help tokens" on the application pages, and then use
-those tokens, and various other settings, to determine the actual URL to use.
-Documentation ************* Help-tokens provides a context processor, and a
-redirection URL. Configuration is in a number of settings. Settings ========
-Help-tokens reads these Django settings to create URLs: * HELP_TOKENS_INI_FILE:
-Path to a .ini file containing help token definitions. The format of the ini
-file is described below. * HELP_TOKENS_BOOKS: a dictionary mapping book slugs
-to URLs. For example:: HELP_TOKENS_BOOKS = { 'learner': 'http://
-edx.readthedocs.io/projects/learner-guide', 'course_author': 'http://
-edx.readthedocs.io/projects/running-a-course', } * HELP_TOKENS_VERSION: a
-string used as part of the final URL, to choose the correct version of the
-book. For example, `"latest"`. * HELP_TOKENS_LANGUAGE_CODE: the language code
-to use as part of the book URL, mapped through the [locales] section of the ini
-file. INI file format =============== The .ini file pointed to by
-HELP_TOKENS_INI_FILE contains the definitions of the help tokens themselves.
-The `[pages]` section defines the help tokens. Each help token definition
-consists of a book slug (defined in HELP_TOKENS_BOOKS), a colon, and a URL
-path. The `default` token is used for missing tokens. For example:: [pages]
-default = learner:index.html instructor = learner:SFD_instructor_dash_help.html
-course = learner:index.html cohortmanual = course_author:course_features/
-cohorts/cohort_config.html#assign-learners-to-cohorts-manually cohortautomatic
-= course_author:course_features/cohorts/cohorts_overview.html#all-automated-
-assignment The `[locales]` section defines language codes, used with
-HELP_TOKENS_LANGUAGE_CODE to determine the language portion of the URL::
-[locales] default = en en = en en_us = en Context processor =================
-The context processor is `"help_tokens.context_processor"`. It adds a function
-`get_online_help_info`. Call it with a help token, and it will return a dict
-with a `doc_url` entry, the help URL. You can use it like this in a template::
-... This interface is a bit verbose, but is to maintain backward compatibility
-with a previous implementation of this context processor. Redirection view
-================ The `help_tokens.urls` URLs define a view that redirects to a
-help URL. You can include it in your app:: # For redirecting to help pages. url
-(r'^help_token/', include('help_tokens.urls')), Then visiting `help_token/
-foobar` will redirect to the URL defined by the "foobar" help token. License
-******* The code in this repository is licensed under the AGPL 3.0 unless
-otherwise noted. Please see ``LICENSE.txt`` for details. How To Contribute
-***************** Contributions are very welcome. Please read `How To
-Contribute
-github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details. Even
-though they were written with ``edx-platform`` in mind, the guidelines should
-be followed for Open edX code in general. PR description template should be
-automatically applied if you are sending PR from GitHub interface; otherwise
-you can find it it at `PULL_REQUEST_TEMPLATE.md
-github.com/edx/help-tokens/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+Metadata-Version: 2.1 Name: help-tokens Version: 2.3.0 Summary: Django app for
+linking to help pages with short tokens Home-page: https://github.com/openedx/
+help-tokens Author: edX Author-email: oscm@edx.org License: AGPL 3.0 Keywords:
+Django edx Classifier: Development Status :: 5 - Production/Stable Classifier:
+Framework :: Django Classifier: Framework :: Django :: 3.2 Classifier:
+Framework :: Django :: 4.0 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or
+later (AGPLv3+) Classifier: Natural Language :: English Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst License-File: LICENSE.txt License-File:
+AUTHORS ########### help-tokens ########### Django app for linking to help
+pages with short tokens. |pypi-badge| |ci-badge| |codecov-badge| |pyversions-
+badge| |license-badge| Overview ******** There are various factors that affect
+what help page an application should link to: - There may be a number of
+relevant books - The version of the application might affect which book to
+display - The application's language might affect which book to display This
+small Django app provides a means to use "help tokens" on the application
+pages, and then use those tokens, and various other settings, to determine the
+actual URL to use. Documentation ************* Help-tokens provides a context
+processor, and a redirection URL. Configuration is in a number of settings.
+Settings ======== Help-tokens reads these Django settings to create URLs: *
+HELP_TOKENS_INI_FILE: Path to a .ini file containing help token definitions.
+The format of the ini file is described below. * HELP_TOKENS_BOOKS: a
+dictionary mapping book slugs to URLs. For example:: HELP_TOKENS_BOOKS =
+{ 'learner': 'http://edx.readthedocs.io/projects/learner-guide',
+'course_author': 'http://edx.readthedocs.io/projects/running-a-course', } *
+HELP_TOKENS_VERSION: a string used as part of the final URL, to choose the
+correct version of the book. For example, `"latest"`. *
+HELP_TOKENS_LANGUAGE_CODE: the language code to use as part of the book URL,
+mapped through the [locales] section of the ini file. INI file format
+=============== The .ini file pointed to by HELP_TOKENS_INI_FILE contains the
+definitions of the help tokens themselves. The `[pages]` section defines the
+help tokens. Each help token definition consists of a book slug (defined in
+HELP_TOKENS_BOOKS), a colon, and a URL path. The `default` token is used for
+missing tokens. For example:: [pages] default = learner:index.html instructor =
+learner:SFD_instructor_dash_help.html course = learner:index.html cohortmanual
+= course_author:course_features/cohorts/cohort_config.html#assign-learners-to-
+cohorts-manually cohortautomatic = course_author:course_features/cohorts/
+cohorts_overview.html#all-automated-assignment The `[locales]` section defines
+language codes, used with HELP_TOKENS_LANGUAGE_CODE to determine the language
+portion of the URL:: [locales] default = en en = en en_us = en Context
+processor ================= The context processor is
+`"help_tokens.context_processor"`. It adds a function `get_online_help_info`.
+Call it with a help token, and it will return a dict with a `doc_url` entry,
+the help URL. You can use it like this in a template:: ... This interface is a
+bit verbose, but is to maintain backward compatibility with a previous
+implementation of this context processor. Redirection view ================ The
+`help_tokens.urls` URLs define a view that redirects to a help URL. You can
+include it in your app:: # For redirecting to help pages. url(r'^help_token/',
+include('help_tokens.urls')), Then visiting `help_token/foobar` will redirect
+to the URL defined by the "foobar" help token. License ******* The code in this
+repository is licensed under the AGPL 3.0 unless otherwise noted. Please see
+``LICENSE.txt`` for details. How To Contribute ***************** Contributions
+are very welcome. Please read `How To Contribute
+github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details. PR
+description template should be automatically applied if you are sending PR from
+GitHub interface; otherwise you can find it it at `PULL_REQUEST_TEMPLATE.md
+github.com/openedx/help-tokens/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 Issue report template should be automatically applied if you are sending it
 from GitHub UI as well; otherwise you can find it at `ISSUE_TEMPLATE.md
-github.com/edx/help-tokens/blob/master/.github/ISSUE_TEMPLATE.md>`_ Reporting
-Security Issues ************************* Please do not report security issues
-in public. Please email security@edx.org. Getting Help ************ Have a
-question about this repository, or about Open edX in general? Please refer to
-this `list of resources`_ if you need any assistance. .. _list of resources:
-https://open.edx.org/getting-help .. |pypi-badge| image:: https://
-img.shields.io/pypi/v/help-tokens.svg :target: https://pypi.python.org/pypi/
-help-tokens/ :alt: PyPI .. |ci-badge| image:: https://github.com/edx/help-
-tokens/workflows/Python%20CI/badge.svg?branch=master :target: https://
-github.com/edx/help-tokens/actions?query=workflow%3A%22Python+CI%22 :alt: CI ..
-|codecov-badge| image:: http://codecov.io/github/edx/help-tokens/
-coverage.svg?branch=master :target: http://codecov.io/github/edx/help-
-tokens?branch=master :alt: Codecov .. |pyversions-badge| image:: https://
-img.shields.io/pypi/pyversions/help-tokens.svg :target: https://
-pypi.python.org/pypi/help-tokens/ :alt: Supported Python versions .. |license-
-badge| image:: https://img.shields.io/github/license/edx/help-tokens.svg :
-target: https://github.com/edx/help-tokens/blob/master/LICENSE.txt :alt:
-License Change Log ********** .. All enhancements and patches to help_tokens
-will be documented in this file. It adheres to the structure of http://
-keepachangelog.com/ , but in reStructuredText instead of Markdown (for ease of
-incorporation into Sphinx documentation and the PyPI description). This project
-adheres to Semantic Versioning (http://semver.org/). .. There should always be
-an "Unreleased" section for changes pending release. [2.2.0] - 2022-01-20
-==================== * Dropped support for django2.2, 3.0, 3.1 and 3.2 * Added
-Django40 support in CI [2.1.0] - 2020-07-07 ==================== * Added
-support for django3.0, 3.1 and 3.2 [2.0.0] - 2020-01-19 ==================== *
-Removed support of python3.5 [1.1.0] - 2020-05-05 ==================== *
-Removed support of Django < 2.2 version * Added support for python 3.8 [1.0.3]
-- 2017-07-17 ==================== * Updated tests to support Django 1.11 *
-Updated dependency versions [1.0.2] - 2017-05-16 ==================== * Fixed
-the README. [1.0.1] - 2017-05-15 ==================== * First version on PyPI.
-[1.0.0] - 2017-05-03 ==================== * First release.
+github.com/openedx/help-tokens/blob/master/.github/ISSUE_TEMPLATE.md>`_
+Reporting Security Issues ************************* Please do not report
+security issues in public. Please email security@edx.org. Getting Help
+************ Have a question about this repository, or about Open edX in
+general? Please refer to this `list of resources`_ if you need any assistance.
+.. _list of resources: https://open.edx.org/getting-help .. |pypi-badge|
+image:: https://img.shields.io/pypi/v/help-tokens.svg :target: https://
+pypi.python.org/pypi/help-tokens/ :alt: PyPI .. |ci-badge| image:: https://
+github.com/openedx/help-tokens/workflows/Python%20CI/badge.svg?branch=master :
+target: https://github.com/openedx/help-tokens/
+actions?query=workflow%3A%22Python+CI%22 :alt: CI .. |codecov-badge| image::
+http://codecov.io/github/edx/help-tokens/coverage.svg?branch=master :target:
+http://codecov.io/github/edx/help-tokens?branch=master :alt: Codecov ..
+|pyversions-badge| image:: https://img.shields.io/pypi/pyversions/help-
+tokens.svg :target: https://pypi.python.org/pypi/help-tokens/ :alt: Supported
+Python versions .. |license-badge| image:: https://img.shields.io/github/
+license/edx/help-tokens.svg :target: https://github.com/openedx/help-tokens/
+blob/master/LICENSE.txt :alt: License Change Log ********** .. All enhancements
+and patches to help_tokens will be documented in this file. It adheres to the
+structure of http://keepachangelog.com/ , but in reStructuredText instead of
+Markdown (for ease of incorporation into Sphinx documentation and the PyPI
+description). This project adheres to Semantic Versioning (http://semver.org/).
+.. There should always be an "Unreleased" section for changes pending release.
+[2.3.0] - 2023-08-02 ==================== * Added support for Django 4.2
+[2.2.0] - 2022-01-20 ==================== * Dropped support for django2.2, 3.0,
+3.1 and 3.2 * Added Django40 support in CI [2.1.0] - 2020-07-07
+==================== * Added support for django3.0, 3.1 and 3.2 [2.0.0] - 2020-
+01-19 ==================== * Removed support of python3.5 [1.1.0] - 2020-05-05
+==================== * Removed support of Django < 2.2 version * Added support
+for python 3.8 [1.0.3] - 2017-07-17 ==================== * Updated tests to
+support Django 1.11 * Updated dependency versions [1.0.2] - 2017-05-16
+==================== * Fixed the README. [1.0.1] - 2017-05-15
+==================== * First version on PyPI. [1.0.0] - 2017-05-03
+==================== * First release.
```

### Comparing `help-tokens-2.2.0/README.rst` & `help-tokens-2.3.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -112,24 +112,22 @@
 noted.  Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 *****************
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from GitHub interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/help-tokens/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/help-tokens/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from GitHub UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/help-tokens/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/help-tokens/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 *************************
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -141,23 +139,23 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/help-tokens.svg
     :target: https://pypi.python.org/pypi/help-tokens/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/help-tokens/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/help-tokens/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/help-tokens/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/help-tokens/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/help-tokens/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/help-tokens?branch=master
     :alt: Codecov
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/help-tokens.svg
     :target: https://pypi.python.org/pypi/help-tokens/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/help-tokens.svg
-    :target: https://github.com/edx/help-tokens/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/help-tokens/blob/master/LICENSE.txt
     :alt: License
```

#### html2text {}

```diff
@@ -38,33 +38,31 @@
 help URL. You can include it in your app:: # For redirecting to help pages. url
 (r'^help_token/', include('help_tokens.urls')), Then visiting `help_token/
 foobar` will redirect to the URL defined by the "foobar" help token. License
 ******* The code in this repository is licensed under the AGPL 3.0 unless
 otherwise noted. Please see ``LICENSE.txt`` for details. How To Contribute
 ***************** Contributions are very welcome. Please read `How To
 Contribute
-github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details. Even
-though they were written with ``edx-platform`` in mind, the guidelines should
-be followed for Open edX code in general. PR description template should be
-automatically applied if you are sending PR from GitHub interface; otherwise
-you can find it it at `PULL_REQUEST_TEMPLATE.md
-github.com/edx/help-tokens/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details. PR
+description template should be automatically applied if you are sending PR from
+GitHub interface; otherwise you can find it it at `PULL_REQUEST_TEMPLATE.md
+github.com/openedx/help-tokens/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 Issue report template should be automatically applied if you are sending it
 from GitHub UI as well; otherwise you can find it at `ISSUE_TEMPLATE.md
-github.com/edx/help-tokens/blob/master/.github/ISSUE_TEMPLATE.md>`_ Reporting
-Security Issues ************************* Please do not report security issues
-in public. Please email security@edx.org. Getting Help ************ Have a
-question about this repository, or about Open edX in general? Please refer to
-this `list of resources`_ if you need any assistance. .. _list of resources:
-https://open.edx.org/getting-help .. |pypi-badge| image:: https://
-img.shields.io/pypi/v/help-tokens.svg :target: https://pypi.python.org/pypi/
-help-tokens/ :alt: PyPI .. |ci-badge| image:: https://github.com/edx/help-
-tokens/workflows/Python%20CI/badge.svg?branch=master :target: https://
-github.com/edx/help-tokens/actions?query=workflow%3A%22Python+CI%22 :alt: CI ..
-|codecov-badge| image:: http://codecov.io/github/edx/help-tokens/
-coverage.svg?branch=master :target: http://codecov.io/github/edx/help-
-tokens?branch=master :alt: Codecov .. |pyversions-badge| image:: https://
-img.shields.io/pypi/pyversions/help-tokens.svg :target: https://
-pypi.python.org/pypi/help-tokens/ :alt: Supported Python versions .. |license-
-badge| image:: https://img.shields.io/github/license/edx/help-tokens.svg :
-target: https://github.com/edx/help-tokens/blob/master/LICENSE.txt :alt:
-License
+github.com/openedx/help-tokens/blob/master/.github/ISSUE_TEMPLATE.md>`_
+Reporting Security Issues ************************* Please do not report
+security issues in public. Please email security@edx.org. Getting Help
+************ Have a question about this repository, or about Open edX in
+general? Please refer to this `list of resources`_ if you need any assistance.
+.. _list of resources: https://open.edx.org/getting-help .. |pypi-badge|
+image:: https://img.shields.io/pypi/v/help-tokens.svg :target: https://
+pypi.python.org/pypi/help-tokens/ :alt: PyPI .. |ci-badge| image:: https://
+github.com/openedx/help-tokens/workflows/Python%20CI/badge.svg?branch=master :
+target: https://github.com/openedx/help-tokens/
+actions?query=workflow%3A%22Python+CI%22 :alt: CI .. |codecov-badge| image::
+http://codecov.io/github/edx/help-tokens/coverage.svg?branch=master :target:
+http://codecov.io/github/edx/help-tokens?branch=master :alt: Codecov ..
+|pyversions-badge| image:: https://img.shields.io/pypi/pyversions/help-
+tokens.svg :target: https://pypi.python.org/pypi/help-tokens/ :alt: Supported
+Python versions .. |license-badge| image:: https://img.shields.io/github/
+license/edx/help-tokens.svg :target: https://github.com/openedx/help-tokens/
+blob/master/LICENSE.txt :alt: License
```

### Comparing `help-tokens-2.2.0/help_tokens/context_processor.py` & `help-tokens-2.3.0/help_tokens/context_processor.py`

 * *Files identical despite different names*

### Comparing `help-tokens-2.2.0/help_tokens/core.py` & `help-tokens-2.3.0/help_tokens/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                 )
 
         return self.config.get(section_name, default_option)
 
     def url_for_token(self, token):
         """Find the full URL for a help token."""
         book_url = self.get_config_value("pages", token)
-        book, _, url_tail = book_url.partition(':')  # pylint: disable=no-member
+        book, _, url_tail = book_url.partition(':')
         book_base = settings.HELP_TOKENS_BOOKS[book]
 
         url = book_base
 
         lang = getattr(settings, "HELP_TOKENS_LANGUAGE_CODE", None)
         if lang is not None:
             lang = self.get_config_value("locales", lang)
```

### Comparing `help-tokens-2.2.0/help_tokens.egg-info/PKG-INFO` & `help-tokens-2.3.0/help_tokens.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: help-tokens
-Version: 2.2.0
+Version: 2.3.0
 Summary: Django app for linking to help pages with short tokens
-Home-page: https://github.com/edx/help-tokens
+Home-page: https://github.com/openedx/help-tokens
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS
 
 ###########
 help-tokens
 ###########
 
@@ -134,24 +134,22 @@
 noted.  Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 *****************
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from GitHub interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/help-tokens/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/help-tokens/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from GitHub UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/help-tokens/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/help-tokens/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 *************************
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -163,28 +161,28 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/help-tokens.svg
     :target: https://pypi.python.org/pypi/help-tokens/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/help-tokens/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/help-tokens/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/help-tokens/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/help-tokens/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/help-tokens/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/help-tokens?branch=master
     :alt: Codecov
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/help-tokens.svg
     :target: https://pypi.python.org/pypi/help-tokens/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/help-tokens.svg
-    :target: https://github.com/edx/help-tokens/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/help-tokens/blob/master/LICENSE.txt
     :alt: License
 
 
 
 Change Log
 **********
 
@@ -194,14 +192,19 @@
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
+[2.3.0] - 2023-08-02
+====================
+
+* Added support for Django 4.2
+
 [2.2.0] - 2022-01-20
 ====================
 
 * Dropped support for django2.2, 3.0, 3.1 and 3.2
 * Added Django40 support in CI
 
 [2.1.0] - 2020-07-07
@@ -239,9 +242,7 @@
 * First version on PyPI.
 
 
 [1.0.0] - 2017-05-03
 ====================
 
 * First release.
-
-
```

#### html2text {}

```diff
@@ -1,94 +1,94 @@
-Metadata-Version: 2.1 Name: help-tokens Version: 2.2.0 Summary: Django app for
-linking to help pages with short tokens Home-page: https://github.com/edx/help-
-tokens Author: edX Author-email: oscm@edx.org License: AGPL 3.0 Keywords:
-Django edx Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
-Stable Classifier: Framework :: Django Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0 Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: GNU Affero General Public
-License v3 or later (AGPLv3+) Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 License-File: LICENSE.txt License-File: AUTHORS
-########### help-tokens ########### Django app for linking to help pages with
-short tokens. |pypi-badge| |ci-badge| |codecov-badge| |pyversions-badge|
-|license-badge| Overview ******** There are various factors that affect what
-help page an application should link to: - There may be a number of relevant
-books - The version of the application might affect which book to display - The
-application's language might affect which book to display This small Django app
-provides a means to use "help tokens" on the application pages, and then use
-those tokens, and various other settings, to determine the actual URL to use.
-Documentation ************* Help-tokens provides a context processor, and a
-redirection URL. Configuration is in a number of settings. Settings ========
-Help-tokens reads these Django settings to create URLs: * HELP_TOKENS_INI_FILE:
-Path to a .ini file containing help token definitions. The format of the ini
-file is described below. * HELP_TOKENS_BOOKS: a dictionary mapping book slugs
-to URLs. For example:: HELP_TOKENS_BOOKS = { 'learner': 'http://
-edx.readthedocs.io/projects/learner-guide', 'course_author': 'http://
-edx.readthedocs.io/projects/running-a-course', } * HELP_TOKENS_VERSION: a
-string used as part of the final URL, to choose the correct version of the
-book. For example, `"latest"`. * HELP_TOKENS_LANGUAGE_CODE: the language code
-to use as part of the book URL, mapped through the [locales] section of the ini
-file. INI file format =============== The .ini file pointed to by
-HELP_TOKENS_INI_FILE contains the definitions of the help tokens themselves.
-The `[pages]` section defines the help tokens. Each help token definition
-consists of a book slug (defined in HELP_TOKENS_BOOKS), a colon, and a URL
-path. The `default` token is used for missing tokens. For example:: [pages]
-default = learner:index.html instructor = learner:SFD_instructor_dash_help.html
-course = learner:index.html cohortmanual = course_author:course_features/
-cohorts/cohort_config.html#assign-learners-to-cohorts-manually cohortautomatic
-= course_author:course_features/cohorts/cohorts_overview.html#all-automated-
-assignment The `[locales]` section defines language codes, used with
-HELP_TOKENS_LANGUAGE_CODE to determine the language portion of the URL::
-[locales] default = en en = en en_us = en Context processor =================
-The context processor is `"help_tokens.context_processor"`. It adds a function
-`get_online_help_info`. Call it with a help token, and it will return a dict
-with a `doc_url` entry, the help URL. You can use it like this in a template::
-... This interface is a bit verbose, but is to maintain backward compatibility
-with a previous implementation of this context processor. Redirection view
-================ The `help_tokens.urls` URLs define a view that redirects to a
-help URL. You can include it in your app:: # For redirecting to help pages. url
-(r'^help_token/', include('help_tokens.urls')), Then visiting `help_token/
-foobar` will redirect to the URL defined by the "foobar" help token. License
-******* The code in this repository is licensed under the AGPL 3.0 unless
-otherwise noted. Please see ``LICENSE.txt`` for details. How To Contribute
-***************** Contributions are very welcome. Please read `How To
-Contribute
-github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details. Even
-though they were written with ``edx-platform`` in mind, the guidelines should
-be followed for Open edX code in general. PR description template should be
-automatically applied if you are sending PR from GitHub interface; otherwise
-you can find it it at `PULL_REQUEST_TEMPLATE.md
-github.com/edx/help-tokens/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+Metadata-Version: 2.1 Name: help-tokens Version: 2.3.0 Summary: Django app for
+linking to help pages with short tokens Home-page: https://github.com/openedx/
+help-tokens Author: edX Author-email: oscm@edx.org License: AGPL 3.0 Keywords:
+Django edx Classifier: Development Status :: 5 - Production/Stable Classifier:
+Framework :: Django Classifier: Framework :: Django :: 3.2 Classifier:
+Framework :: Django :: 4.0 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or
+later (AGPLv3+) Classifier: Natural Language :: English Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst License-File: LICENSE.txt License-File:
+AUTHORS ########### help-tokens ########### Django app for linking to help
+pages with short tokens. |pypi-badge| |ci-badge| |codecov-badge| |pyversions-
+badge| |license-badge| Overview ******** There are various factors that affect
+what help page an application should link to: - There may be a number of
+relevant books - The version of the application might affect which book to
+display - The application's language might affect which book to display This
+small Django app provides a means to use "help tokens" on the application
+pages, and then use those tokens, and various other settings, to determine the
+actual URL to use. Documentation ************* Help-tokens provides a context
+processor, and a redirection URL. Configuration is in a number of settings.
+Settings ======== Help-tokens reads these Django settings to create URLs: *
+HELP_TOKENS_INI_FILE: Path to a .ini file containing help token definitions.
+The format of the ini file is described below. * HELP_TOKENS_BOOKS: a
+dictionary mapping book slugs to URLs. For example:: HELP_TOKENS_BOOKS =
+{ 'learner': 'http://edx.readthedocs.io/projects/learner-guide',
+'course_author': 'http://edx.readthedocs.io/projects/running-a-course', } *
+HELP_TOKENS_VERSION: a string used as part of the final URL, to choose the
+correct version of the book. For example, `"latest"`. *
+HELP_TOKENS_LANGUAGE_CODE: the language code to use as part of the book URL,
+mapped through the [locales] section of the ini file. INI file format
+=============== The .ini file pointed to by HELP_TOKENS_INI_FILE contains the
+definitions of the help tokens themselves. The `[pages]` section defines the
+help tokens. Each help token definition consists of a book slug (defined in
+HELP_TOKENS_BOOKS), a colon, and a URL path. The `default` token is used for
+missing tokens. For example:: [pages] default = learner:index.html instructor =
+learner:SFD_instructor_dash_help.html course = learner:index.html cohortmanual
+= course_author:course_features/cohorts/cohort_config.html#assign-learners-to-
+cohorts-manually cohortautomatic = course_author:course_features/cohorts/
+cohorts_overview.html#all-automated-assignment The `[locales]` section defines
+language codes, used with HELP_TOKENS_LANGUAGE_CODE to determine the language
+portion of the URL:: [locales] default = en en = en en_us = en Context
+processor ================= The context processor is
+`"help_tokens.context_processor"`. It adds a function `get_online_help_info`.
+Call it with a help token, and it will return a dict with a `doc_url` entry,
+the help URL. You can use it like this in a template:: ... This interface is a
+bit verbose, but is to maintain backward compatibility with a previous
+implementation of this context processor. Redirection view ================ The
+`help_tokens.urls` URLs define a view that redirects to a help URL. You can
+include it in your app:: # For redirecting to help pages. url(r'^help_token/',
+include('help_tokens.urls')), Then visiting `help_token/foobar` will redirect
+to the URL defined by the "foobar" help token. License ******* The code in this
+repository is licensed under the AGPL 3.0 unless otherwise noted. Please see
+``LICENSE.txt`` for details. How To Contribute ***************** Contributions
+are very welcome. Please read `How To Contribute
+github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details. PR
+description template should be automatically applied if you are sending PR from
+GitHub interface; otherwise you can find it it at `PULL_REQUEST_TEMPLATE.md
+github.com/openedx/help-tokens/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 Issue report template should be automatically applied if you are sending it
 from GitHub UI as well; otherwise you can find it at `ISSUE_TEMPLATE.md
-github.com/edx/help-tokens/blob/master/.github/ISSUE_TEMPLATE.md>`_ Reporting
-Security Issues ************************* Please do not report security issues
-in public. Please email security@edx.org. Getting Help ************ Have a
-question about this repository, or about Open edX in general? Please refer to
-this `list of resources`_ if you need any assistance. .. _list of resources:
-https://open.edx.org/getting-help .. |pypi-badge| image:: https://
-img.shields.io/pypi/v/help-tokens.svg :target: https://pypi.python.org/pypi/
-help-tokens/ :alt: PyPI .. |ci-badge| image:: https://github.com/edx/help-
-tokens/workflows/Python%20CI/badge.svg?branch=master :target: https://
-github.com/edx/help-tokens/actions?query=workflow%3A%22Python+CI%22 :alt: CI ..
-|codecov-badge| image:: http://codecov.io/github/edx/help-tokens/
-coverage.svg?branch=master :target: http://codecov.io/github/edx/help-
-tokens?branch=master :alt: Codecov .. |pyversions-badge| image:: https://
-img.shields.io/pypi/pyversions/help-tokens.svg :target: https://
-pypi.python.org/pypi/help-tokens/ :alt: Supported Python versions .. |license-
-badge| image:: https://img.shields.io/github/license/edx/help-tokens.svg :
-target: https://github.com/edx/help-tokens/blob/master/LICENSE.txt :alt:
-License Change Log ********** .. All enhancements and patches to help_tokens
-will be documented in this file. It adheres to the structure of http://
-keepachangelog.com/ , but in reStructuredText instead of Markdown (for ease of
-incorporation into Sphinx documentation and the PyPI description). This project
-adheres to Semantic Versioning (http://semver.org/). .. There should always be
-an "Unreleased" section for changes pending release. [2.2.0] - 2022-01-20
-==================== * Dropped support for django2.2, 3.0, 3.1 and 3.2 * Added
-Django40 support in CI [2.1.0] - 2020-07-07 ==================== * Added
-support for django3.0, 3.1 and 3.2 [2.0.0] - 2020-01-19 ==================== *
-Removed support of python3.5 [1.1.0] - 2020-05-05 ==================== *
-Removed support of Django < 2.2 version * Added support for python 3.8 [1.0.3]
-- 2017-07-17 ==================== * Updated tests to support Django 1.11 *
-Updated dependency versions [1.0.2] - 2017-05-16 ==================== * Fixed
-the README. [1.0.1] - 2017-05-15 ==================== * First version on PyPI.
-[1.0.0] - 2017-05-03 ==================== * First release.
+github.com/openedx/help-tokens/blob/master/.github/ISSUE_TEMPLATE.md>`_
+Reporting Security Issues ************************* Please do not report
+security issues in public. Please email security@edx.org. Getting Help
+************ Have a question about this repository, or about Open edX in
+general? Please refer to this `list of resources`_ if you need any assistance.
+.. _list of resources: https://open.edx.org/getting-help .. |pypi-badge|
+image:: https://img.shields.io/pypi/v/help-tokens.svg :target: https://
+pypi.python.org/pypi/help-tokens/ :alt: PyPI .. |ci-badge| image:: https://
+github.com/openedx/help-tokens/workflows/Python%20CI/badge.svg?branch=master :
+target: https://github.com/openedx/help-tokens/
+actions?query=workflow%3A%22Python+CI%22 :alt: CI .. |codecov-badge| image::
+http://codecov.io/github/edx/help-tokens/coverage.svg?branch=master :target:
+http://codecov.io/github/edx/help-tokens?branch=master :alt: Codecov ..
+|pyversions-badge| image:: https://img.shields.io/pypi/pyversions/help-
+tokens.svg :target: https://pypi.python.org/pypi/help-tokens/ :alt: Supported
+Python versions .. |license-badge| image:: https://img.shields.io/github/
+license/edx/help-tokens.svg :target: https://github.com/openedx/help-tokens/
+blob/master/LICENSE.txt :alt: License Change Log ********** .. All enhancements
+and patches to help_tokens will be documented in this file. It adheres to the
+structure of http://keepachangelog.com/ , but in reStructuredText instead of
+Markdown (for ease of incorporation into Sphinx documentation and the PyPI
+description). This project adheres to Semantic Versioning (http://semver.org/).
+.. There should always be an "Unreleased" section for changes pending release.
+[2.3.0] - 2023-08-02 ==================== * Added support for Django 4.2
+[2.2.0] - 2022-01-20 ==================== * Dropped support for django2.2, 3.0,
+3.1 and 3.2 * Added Django40 support in CI [2.1.0] - 2020-07-07
+==================== * Added support for django3.0, 3.1 and 3.2 [2.0.0] - 2020-
+01-19 ==================== * Removed support of python3.5 [1.1.0] - 2020-05-05
+==================== * Removed support of Django < 2.2 version * Added support
+for python 3.8 [1.0.3] - 2017-07-17 ==================== * Updated tests to
+support Django 1.11 * Updated dependency versions [1.0.2] - 2017-05-16
+==================== * Fixed the README. [1.0.1] - 2017-05-15
+==================== * First version on PyPI. [1.0.0] - 2017-05-03
+==================== * First release.
```

### Comparing `help-tokens-2.2.0/requirements/constraints.txt` & `help-tokens-2.3.0/requirements/constraints.txt`

 * *Files 21% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 #
 # When pinning something here, please provide an explanation of why.  Ideally,
 # link to other information that will help people in the future to remove the
 # pin when possible.  Writing an issue against the offending project and
 # linking to it here is good.
 
 # This file contains all common constraints for edx-repos
--c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+-c common_constraints.txt
```

### Comparing `help-tokens-2.2.0/setup.py` & `help-tokens-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,17 +100,18 @@
 CHANGELOG = open(os.path.join(os.path.dirname(__file__), 'CHANGELOG.rst'), encoding='utf-8').read()
 
 setup(
     name='help-tokens',
     version=VERSION,
     description="""Django app for linking to help pages with short tokens""",
     long_description=README + '\n\n' + CHANGELOG,
+    long_description_content_type='text/x-rst',
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/help-tokens',
+    url='https://github.com/openedx/help-tokens',
     packages=[
         'help_tokens',
     ],
     include_package_data=True,
     install_requires=load_requirements('requirements/base.in'),
     license="AGPL 3.0",
     zip_safe=False,
```

