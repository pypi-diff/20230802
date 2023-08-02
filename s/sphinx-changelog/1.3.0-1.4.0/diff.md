# Comparing `tmp/sphinx_changelog-1.3.0.tar.gz` & `tmp/sphinx_changelog-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_changelog-1.3.0.tar", last modified: Wed Mar  1 14:46:10 2023, max compression
+gzip compressed data, was "sphinx_changelog-1.4.0.tar", last modified: Wed Aug  2 09:38:52 2023, max compression
```

## Comparing `sphinx_changelog-1.3.0.tar` & `sphinx_changelog-1.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:46:10.547319 sphinx_changelog-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-03-01 14:46:10.547319 sphinx_changelog-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:46:10.543319 sphinx_changelog-1.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/docs/test_changelogs.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:46:10.543319 sphinx_changelog-1.3.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/licenses/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/licenses/TEMPLATE_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-01 14:46:10.547319 sphinx_changelog-1.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:46:10.543319 sphinx_changelog-1.3.0/sphinx_changelog/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/sphinx_changelog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/sphinx_changelog/directive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/sphinx_changelog/towncrier.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-01 14:46:10.000000 sphinx_changelog-1.3.0/sphinx_changelog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:46:10.547319 sphinx_changelog-1.3.0/sphinx_changelog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-03-01 14:46:10.000000 sphinx_changelog-1.3.0/sphinx_changelog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-01 14:46:10.000000 sphinx_changelog-1.3.0/sphinx_changelog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 14:46:10.000000 sphinx_changelog-1.3.0/sphinx_changelog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 14:46:10.000000 sphinx_changelog-1.3.0/sphinx_changelog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-01 14:46:10.000000 sphinx_changelog-1.3.0/sphinx_changelog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-01 14:46:10.000000 sphinx_changelog-1.3.0/sphinx_changelog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-01 14:45:54.000000 sphinx_changelog-1.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:38:52.019782 sphinx_changelog-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-08-02 09:38:52.019782 sphinx_changelog-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:38:52.019782 sphinx_changelog-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/docs/test_changelogs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:38:52.019782 sphinx_changelog-1.4.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/licenses/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/licenses/TEMPLATE_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-02 09:38:52.019782 sphinx_changelog-1.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:38:52.019782 sphinx_changelog-1.4.0/sphinx_changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/sphinx_changelog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/sphinx_changelog/directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/sphinx_changelog/towncrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 09:38:51.000000 sphinx_changelog-1.4.0/sphinx_changelog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:38:52.019782 sphinx_changelog-1.4.0/sphinx_changelog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-08-02 09:38:51.000000 sphinx_changelog-1.4.0/sphinx_changelog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-02 09:38:52.000000 sphinx_changelog-1.4.0/sphinx_changelog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:38:51.000000 sphinx_changelog-1.4.0/sphinx_changelog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:38:51.000000 sphinx_changelog-1.4.0/sphinx_changelog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-02 09:38:51.000000 sphinx_changelog-1.4.0/sphinx_changelog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 09:38:51.000000 sphinx_changelog-1.4.0/sphinx_changelog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 09:38:33.000000 sphinx_changelog-1.4.0/tox.ini
```

### Comparing `sphinx_changelog-1.3.0/CHANGELOG.rst` & `sphinx_changelog-1.4.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Sphinx_Changelog 1.4.0 (2023-08-02)
+===================================
+
+Features
+--------
+
+- The ``towncrier`` version is now pinned to a specific version in ``sphinx_changelog`` dependencies. (`#17 <https://github.com/OpenAstronomy/sphinx-changelog/pull/17>`__)
+- Update supported version of towncrier to 23.6. (`#20 <https://github.com/OpenAstronomy/sphinx-changelog/pull/20>`__)
+
+
 v1.3.0 (2023-03-01)
 ===================
 
 Notes
 -----
 
 This release pins the version of towncrier to 22.12.0, this is because we rely on private API in towncrier, so changes are needed on every release.
```

### Comparing `sphinx_changelog-1.3.0/MANIFEST.in` & `sphinx_changelog-1.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sphinx_changelog-1.3.0/PKG-INFO` & `sphinx_changelog-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_changelog
-Version: 1.3.0
+Version: 1.4.0
 Summary: A changelog renderer for sphinx.
 Home-page: https://openastronomy.org
 Author: SunPy and OpenAstronomy Developers
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.6
 Provides-Extra: all
```

### Comparing `sphinx_changelog-1.3.0/README.rst` & `sphinx_changelog-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_changelog-1.3.0/docs/Makefile` & `sphinx_changelog-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_changelog-1.3.0/docs/conf.py` & `sphinx_changelog-1.4.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 # The master toctree document.
 master_doc = 'index'
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+intersphinx_mapping = {'python': ('https://docs.python.org/', None)}
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = 'alabaster'
```

### Comparing `sphinx_changelog-1.3.0/docs/index.rst` & `sphinx_changelog-1.4.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 Skipping towncrier on Release Builds
 ------------------------------------
 
 If you combine the towncrier and changelog file options, when the documentation builds on a release there will be no fragments to render.
 This means that towncrier will still render an empty changelog duplicating the pre-rendered header for the release.
-To disable towncrier output if no fragment files are found add the ``:towncrier-skip-if-emtpy:`` option to the directive:
+To disable towncrier output if no fragment files are found add the ``:towncrier-skip-if-empty:`` option to the directive:
 
 .. code-block:: rst
 
     .. changelog::
        :towncrier: ../
        :towncrier-skip-if-empty:
        :changelog_file: ../CHANGELOG.rst
```

### Comparing `sphinx_changelog-1.3.0/docs/make.bat` & `sphinx_changelog-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphinx_changelog-1.3.0/docs/test_changelogs.rst` & `sphinx_changelog-1.4.0/docs/test_changelogs.rst`

 * *Files identical despite different names*

### Comparing `sphinx_changelog-1.3.0/licenses/LICENSE.rst` & `sphinx_changelog-1.4.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sphinx_changelog-1.3.0/licenses/TEMPLATE_LICENSE.rst` & `sphinx_changelog-1.4.0/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sphinx_changelog-1.3.0/pyproject.toml` & `sphinx_changelog-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_changelog-1.3.0/setup.cfg` & `sphinx_changelog-1.4.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [options]
 zip_safe = False
 packages = find:
 python_requires = >=3.6
 setup_requires = setuptools_scm
 install_requires = 
 	sphinx
-	towncrier==22.12.0
+	towncrier==23.6.0
 
 [options.extras_require]
 all = 
 test = 
 	pytest
 	pytest-cov
 docs =
```

### Comparing `sphinx_changelog-1.3.0/setup.py` & `sphinx_changelog-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx_changelog-1.3.0/sphinx_changelog/directive.py` & `sphinx_changelog-1.4.0/sphinx_changelog/directive.py`

 * *Files identical despite different names*

### Comparing `sphinx_changelog-1.3.0/sphinx_changelog/towncrier.py` & `sphinx_changelog-1.4.0/sphinx_changelog/towncrier.py`

 * *Files identical despite different names*

### Comparing `sphinx_changelog-1.3.0/sphinx_changelog.egg-info/PKG-INFO` & `sphinx_changelog-1.4.0/sphinx_changelog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-changelog
-Version: 1.3.0
+Version: 1.4.0
 Summary: A changelog renderer for sphinx.
 Home-page: https://openastronomy.org
 Author: SunPy and OpenAstronomy Developers
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.6
 Provides-Extra: all
```

### Comparing `sphinx_changelog-1.3.0/sphinx_changelog.egg-info/SOURCES.txt` & `sphinx_changelog-1.4.0/sphinx_changelog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx_changelog-1.3.0/tox.ini` & `sphinx_changelog-1.4.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,22 @@
     build_docs
     codestyle
 isolated_build = true
 # This is included for testing of the template. You can remove it safely.
 skip_missing_interpreters = True
 
 [testenv]
-# Pass through the following environemnt variables which may be needed for the CI
+# Pass through the following environment variables which may be needed for the CI
 passenv = HOME,WINDIR,LC_ALL,LC_CTYPE,CC,CI,TRAVIS
 
 # Run the tests in a temporary directory to make sure that we don't import
 # the package from the source tree
 changedir = .tmp/{envname}
 
-# tox environments are constructued with so-called 'factors' (or terms)
+# tox environments are constructed with so-called 'factors' (or terms)
 # separated by hyphens, e.g. test-devdeps-cov. Lines below starting with factor:
 # will only take effect if that factor is included in the environment name. To
 # see a list of example environments that can be run, along with a description,
 # run:
 #
 #     tox -l -v
 #
@@ -45,16 +45,16 @@
 changedir = docs
 description = invoke sphinx-build to build the HTML docs
 extras = docs
 commands =
     pip freeze
     sphinx-build -W -b html . _build/html {posargs}
 
-[testenv:build_docs_latesttowncrier]
+[testenv:build_docs_devtowncrier]
 changedir = docs
 description = invoke sphinx-build to build the HTML docs
 extras = docs
 commands_pre =
-    python -m pip install towncrier --upgrade
+    python -m pip install --upgrade git+https://github.com/twisted/towncrier.git
 commands =
     pip freeze
     sphinx-build -W -b html . _build/html {posargs}
```

