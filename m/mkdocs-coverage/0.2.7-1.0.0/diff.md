# Comparing `tmp/mkdocs_coverage-0.2.7.tar.gz` & `tmp/mkdocs_coverage-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_coverage-0.2.7.tar", last modified: Tue Apr 11 09:43:17 2023, max compression
+gzip compressed data, was "mkdocs_coverage-1.0.0.tar", last modified: Wed Aug  2 17:26:34 2023, max compression
```

## Comparing `mkdocs_coverage-0.2.7.tar` & `mkdocs_coverage-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      754 2023-04-11 09:21:19.888457 mkdocs_coverage-0.2.7/LICENSE
--rw-r--r--   0        0        0     1447 2023-04-11 09:21:22.561805 mkdocs_coverage-0.2.7/README.md
--rw-r--r--   0        0        0     2439 2023-04-11 09:43:17.543348 mkdocs_coverage-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      170 2023-04-11 09:21:19.791790 mkdocs_coverage-0.2.7/src/mkdocs_coverage/__init__.py
--rw-r--r--   0        0        0     1289 2023-04-11 09:22:19.352160 mkdocs_coverage-0.2.7/src/mkdocs_coverage/loggers.py
--rw-r--r--   0        0        0     4739 2023-04-11 09:34:18.910852 mkdocs_coverage-0.2.7/src/mkdocs_coverage/plugin.py
--rw-r--r--   0        0        0        0 2023-04-11 09:21:19.785123 mkdocs_coverage-0.2.7/src/mkdocs_coverage/py.typed
--rw-r--r--   0        0        0       37 2021-12-16 22:27:12.259244 mkdocs_coverage-0.2.7/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2021-12-16 22:27:12.259244 mkdocs_coverage-0.2.7/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      295 2021-12-16 22:27:12.259244 mkdocs_coverage-0.2.7/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2021-12-16 22:27:34.598920 mkdocs_coverage-0.2.7/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2021-12-16 22:27:34.598920 mkdocs_coverage-0.2.7/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       10 2021-12-16 22:27:32.335620 mkdocs_coverage-0.2.7/tests/.pytest_cache/v/randomly_seed
--rw-r--r--   0        0        0      168 2023-04-11 09:21:19.781790 mkdocs_coverage-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-04-11 09:21:19.778456 mkdocs_coverage-0.2.7/tests/conftest.py
--rw-r--r--   0        0        0      791 2023-04-11 09:37:31.333365 mkdocs_coverage-0.2.7/tests/test_plugin.py
--rw-r--r--   0        0        0     2976 1970-01-01 00:00:00.000000 mkdocs_coverage-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-08-02 17:06:00.672592 mkdocs_coverage-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1447 2023-08-02 17:06:03.419188 mkdocs_coverage-1.0.0/README.md
+-rw-r--r--   0        0        0     2709 2023-08-02 17:26:34.728375 mkdocs_coverage-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-08-02 17:06:00.572594 mkdocs_coverage-1.0.0/src/mkdocs_coverage/__init__.py
+-rw-r--r--   0        0        0      830 2023-08-02 17:18:48.684886 mkdocs_coverage-1.0.0/src/mkdocs_coverage/loggers.py
+-rw-r--r--   0        0        0     4753 2023-08-02 17:19:29.767337 mkdocs_coverage-1.0.0/src/mkdocs_coverage/plugin.py
+-rw-r--r--   0        0        0        0 2023-08-02 17:06:00.569261 mkdocs_coverage-1.0.0/src/mkdocs_coverage/py.typed
+-rw-r--r--   0        0        0       37 2021-12-16 22:27:12.259244 mkdocs_coverage-1.0.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2021-12-16 22:27:12.259244 mkdocs_coverage-1.0.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      295 2021-12-16 22:27:12.259244 mkdocs_coverage-1.0.0/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2021-12-16 22:27:34.598920 mkdocs_coverage-1.0.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2021-12-16 22:27:34.598920 mkdocs_coverage-1.0.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       10 2021-12-16 22:27:32.335620 mkdocs_coverage-1.0.0/tests/.pytest_cache/v/randomly_seed
+-rw-r--r--   0        0        0      168 2023-08-02 17:06:00.562595 mkdocs_coverage-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-02 17:06:00.559261 mkdocs_coverage-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      791 2023-04-11 09:37:31.333365 mkdocs_coverage-1.0.0/tests/test_plugin.py
+-rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 mkdocs_coverage-1.0.0/PKG-INFO
```

### Comparing `mkdocs_coverage-0.2.7/LICENSE` & `mkdocs_coverage-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_coverage-0.2.7/README.md` & `mkdocs_coverage-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 With `pip`:
 ```bash
 pip install mkdocs-coverage
 ```
 
 With [`pipx`](https://github.com/pipxproject/pipx):
 ```bash
-python3.7 -m pip install --user pipx
+python3.8 -m pip install --user pipx
 pipx install mkdocs-coverage
 ```
 
 ## Usage
 
 ```yaml
 # mkdocs.yml
```

### Comparing `mkdocs_coverage-0.2.7/pyproject.toml` & `mkdocs_coverage-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 [project]
 name = "mkdocs-coverage"
 description = "MkDocs plugin to integrate your coverage HTML report into your site."
 authors = [
     { name = "Timothée Mazzucotelli", email = "pawamoy@pm.me" },
 ]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = []
 dynamic = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Documentation",
     "Topic :: Software Development",
     "Topic :: Software Development :: Documentation",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "mkdocs>=1.2",
 ]
-version = "0.2.7"
+version = "1.0.0"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/mkdocs-coverage"
 Documentation = "https://pawamoy.github.io/mkdocs-coverage"
@@ -48,35 +48,48 @@
 Discussions = "https://github.com/pawamoy/mkdocs-coverage/discussions"
 Gitter = "https://gitter.im/mkdocs-coverage/community"
 Funding = "https://github.com/sponsors/pawamoy"
 
 [project.entry-points."mkdocs.plugins"]
 coverage = "mkdocs_coverage.plugin:MkDocsCoveragePlugin"
 
+[tool.pdm]
+plugins = [
+    "pdm-multirun",
+]
+
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.build]
 package-dir = "src"
 editable-backend = "editables"
 
 [tool.pdm.dev-dependencies]
 duty = [
     "duty>=0.10",
 ]
+ci-quality = [
+    "mkdocs-coverage[duty,docs,quality,typing,security]",
+]
+ci-tests = [
+    "mkdocs-coverage[duty,tests]",
+]
 docs = [
     "black>=23.1",
-    "mkdocs>=1.3",
+    "markdown-callouts>=0.2",
+    "markdown-exec>=0.5",
+    "mkdocs>=1.5",
+    "mkdocs-coverage>=0.2",
     "mkdocs-gen-files>=0.3",
+    "mkdocs-git-committers-plugin-2>=1.1",
     "mkdocs-literate-nav>=0.4",
     "mkdocs-material>=7.3",
-    "mkdocs-section-index>=0.3",
+    "mkdocs-minify-plugin>=0.6.4",
     "mkdocstrings[python]>=0.18",
-    "markdown-callouts>=0.2",
-    "markdown-exec>=0.5",
     "toml>=0.10",
 ]
 maintain = [
     "black>=23.1",
     "blacken-docs>=1.13",
     "git-changelog>=1.0",
 ]
@@ -88,12 +101,13 @@
     "pytest-cov>=3.0",
     "pytest-randomly>=3.10",
     "pytest-xdist>=2.4",
 ]
 typing = [
     "mypy>=0.910",
     "types-markdown>=3.3",
+    "types-pyyaml>=6.0",
     "types-toml>=0.10",
 ]
 security = [
     "safety>=2",
 ]
```

### Comparing `mkdocs_coverage-0.2.7/src/mkdocs_coverage/plugin.py` & `mkdocs_coverage-1.0.0/src/mkdocs_coverage/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 from tempfile import mkdtemp
 from typing import TYPE_CHECKING, Any, Sequence
 
 from mkdocs.config.config_options import Type as MkType
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.files import File, Files
 
-from mkdocs_coverage.loggers import get_logger
+from mkdocs_coverage.loggers import get_plugin_logger
 
 if TYPE_CHECKING:
     from mkdocs.config import Config
 
-log = get_logger(__name__)
+log = get_plugin_logger(__name__)
 
 
 class MkDocsCoveragePlugin(BasePlugin):
     """The MkDocs plugin to integrate the coverage HTML report in the site."""
 
     config_scheme: Sequence[tuple[str, MkType]] = (
         ("page_name", MkType(str, default="coverage")),
```

### Comparing `mkdocs_coverage-0.2.7/tests/test_plugin.py` & `mkdocs_coverage-1.0.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_coverage-0.2.7/PKG-INFO` & `mkdocs_coverage-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: mkdocs-coverage
-Version: 0.2.7
+Version: 1.0.0
 Summary: MkDocs plugin to integrate your coverage HTML report into your site.
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://pawamoy.github.io/mkdocs-coverage
 Project-URL: Documentation, https://pawamoy.github.io/mkdocs-coverage
 Project-URL: Changelog, https://pawamoy.github.io/mkdocs-coverage/changelog
 Project-URL: Repository, https://github.com/pawamoy/mkdocs-coverage
 Project-URL: Issues, https://github.com/pawamoy/mkdocs-coverage/issues
 Project-URL: Discussions, https://github.com/pawamoy/mkdocs-coverage/discussions
 Project-URL: Gitter, https://gitter.im/mkdocs-coverage/community
 Project-URL: Funding, https://github.com/sponsors/pawamoy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: mkdocs>=1.2
 Description-Content-Type: text/markdown
 
 # MkDocs Coverage Plugin
 
 [![ci](https://github.com/pawamoy/mkdocs-coverage/workflows/ci/badge.svg)](https://github.com/pawamoy/mkdocs-coverage/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/mkdocs-coverage/)
@@ -46,15 +46,15 @@
 With `pip`:
 ```bash
 pip install mkdocs-coverage
 ```
 
 With [`pipx`](https://github.com/pipxproject/pipx):
 ```bash
-python3.7 -m pip install --user pipx
+python3.8 -m pip install --user pipx
 pipx install mkdocs-coverage
 ```
 
 ## Usage
 
 ```yaml
 # mkdocs.yml
```

