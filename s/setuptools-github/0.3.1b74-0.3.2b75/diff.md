# Comparing `tmp/setuptools-github-0.3.1b74.tar.gz` & `tmp/setuptools-github-0.3.2b75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.1b74.tar", last modified: Wed Aug  2 18:41:00 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.2b75.tar", last modified: Wed Aug  2 20:02:54 2023, max compression
```

## Comparing `setuptools-github-0.3.1b74.tar` & `setuptools-github-0.3.2b75.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:41:00.706325 setuptools-github-0.3.1b74/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-02 18:41:00.706325 setuptools-github-0.3.1b74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:41:00.706325 setuptools-github-0.3.1b74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:41:00.702324 setuptools-github-0.3.1b74/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:41:00.702324 setuptools-github-0.3.1b74/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:41:00.702324 setuptools-github-0.3.1b74/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 18:41:00.000000 setuptools-github-0.3.1b74/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:41:00.706325 setuptools-github-0.3.1b74/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-08-02 18:40:21.000000 setuptools-github-0.3.1b74/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:02:54.742569 setuptools-github-0.3.2b75/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-08-02 20:02:54.742569 setuptools-github-0.3.2b75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-08-02 20:02:54.000000 setuptools-github-0.3.2b75/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:02:54.742569 setuptools-github-0.3.2b75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:02:54.738569 setuptools-github-0.3.2b75/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-08-02 20:02:54.000000 setuptools-github-0.3.2b75/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 20:02:54.000000 setuptools-github-0.3.2b75/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:02:54.000000 setuptools-github-0.3.2b75/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 20:02:54.000000 setuptools-github-0.3.2b75/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 20:02:54.000000 setuptools-github-0.3.2b75/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 20:02:54.000000 setuptools-github-0.3.2b75/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:02:54.734568 setuptools-github-0.3.2b75/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:02:54.738569 setuptools-github-0.3.2b75/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 20:02:54.000000 setuptools-github-0.3.2b75/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:02:54.742569 setuptools-github-0.3.2b75/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-02 20:02:15.000000 setuptools-github-0.3.2b75/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.1b74/LICENSE` & `setuptools-github-0.3.2b75/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/PKG-INFO` & `setuptools-github-0.3.2b75/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.1b74
+Version: 0.3.2b75
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -14,22 +14,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # setuptools-github
+
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/branch/beta%2F0.3.1/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.1)
+[![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
+
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/workflows/master.yml)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/master/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/master)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
-[![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
-[![Types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
+[![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
 setuptools-github helps to implement a simple project life cycle
 aimed at delivering packages into [PyPI](https://pypi.org). Basically:
 - beta packages are built from a /beta/N.M.O branch generating a **project-name-N.M.ObX** into PyPI
 - tagging with /release/N.M.O a /beta/N.M.O branch commit will release **project-name-N.M.O**
```

### Comparing `setuptools-github-0.3.1b74/README.md` & `setuptools-github-0.3.2b75/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # setuptools-github
+
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/branch/beta%2F0.3.1/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.1)
+[![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
+
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/workflows/master.yml)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/master/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/master)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
-[![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
-[![Types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
+[![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
 setuptools-github helps to implement a simple project life cycle
 aimed at delivering packages into [PyPI](https://pypi.org). Basically:
 - beta packages are built from a /beta/N.M.O branch generating a **project-name-N.M.ObX** into PyPI
 - tagging with /release/N.M.O a /beta/N.M.O branch commit will release **project-name-N.M.O**
```

### Comparing `setuptools-github-0.3.1b74/pyproject.toml` & `setuptools-github-0.3.2b75/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/setup.py` & `setuptools-github-0.3.2b75/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 import sys
 
 sys.path.insert(0, str(pathlib.Path(__file__).parent / "src"))
 from setuptools_github import tools  # noqa E402
 from setuptools import setup, find_namespace_packages  # noqa E402
 
 
+fixers = {
+    "/actions/workflows/master.yml/badge.svg": "/actions/workflows/{{ ctx.workflow }}.yml/badge.svg",  # noqa: E501
+    "/actions/workflows/master.yml": "/actions/runs/{{ runid }}",
+    "/tree/master/graph/badge.svg?token=SIUMZ7MT5T": "/tree/{{ ctx.branch|urlquote }}/graph/badge.svg?token=SIUMZ7MT5T",  # noqa: E501
+    "/tree/master": "/tree/{{ ctx.branch|urlquote }}",
+}
 initfile = pathlib.Path(__file__).parent / "src/setuptools_github/__init__.py"
 readme = pathlib.Path(__file__).parent / "README.md"
 version = tools.process(initfile, os.getenv("GITHUB_DUMP"), readme)["version"]
 
 packages = find_namespace_packages(where="src")
 
 setup(
```

### Comparing `setuptools-github-0.3.1b74/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.2b75/setuptools_github.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.1b74
+Version: 0.3.2b75
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -14,22 +14,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # setuptools-github
+
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/branch/beta%2F0.3.1/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.1)
+[![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
+
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/workflows/master.yml)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/master/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/master)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
-[![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
-[![Types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
+[![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
 setuptools-github helps to implement a simple project life cycle
 aimed at delivering packages into [PyPI](https://pypi.org). Basically:
 - beta packages are built from a /beta/N.M.O branch generating a **project-name-N.M.ObX** into PyPI
 - tagging with /release/N.M.O a /beta/N.M.O branch commit will release **project-name-N.M.O**
```

### Comparing `setuptools-github-0.3.1b74/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.2b75/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/src/setuptools_github/checks.py` & `setuptools-github-0.3.2b75/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/src/setuptools_github/cli.py` & `setuptools-github-0.3.2b75/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/src/setuptools_github/scm.py` & `setuptools-github-0.3.2b75/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/src/setuptools_github/script.py` & `setuptools-github-0.3.2b75/src/setuptools_github/script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/src/setuptools_github/tools.py` & `setuptools-github-0.3.2b75/src/setuptools_github/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -251,14 +251,16 @@
     """
     result = {
         "version": get_module_var(initfile, "__version__"),
         "current": get_module_var(initfile, "__version__"),
         "branch": None,
         "hash": None,
         "build": None,
+        "runid": None,
+        "workflow": None,
     }
 
     path = Path(initfile)
     repo = scm.lookup(path)
 
     if not (repo or github_dump):
         if abort:
@@ -266,26 +268,29 @@
         return result
 
     if not github_dump and repo:
         gdata = {
             "ref": repo.head.name,
             "sha": repo.head.target.hex[:7],
             "run_number": 0,
+            "run_id": 0,
         }
         dirty = repo.dirty()
     else:
         gdata = json.loads(github_dump) if isinstance(github_dump, str) else github_dump
         dirty = False
 
     expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+([.]\d+)*)$")
     expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$")
 
     result["branch"] = lstrip(gdata["ref"], "refs/heads/")
     result["hash"] = gdata["sha"] + ("*" if dirty else "")
     result["build"] = gdata["run_number"]
+    result["runid"] = gdata["run_id"]
+    result["workflow"] = result["branch"]
 
     current = result["current"]
     if match := expr.search(gdata["ref"]):
         # setuptools double calls the update_version,
         # this fixes the issue
         match1 = expr1.search(current or "")
         if not match1:
@@ -293,14 +298,17 @@
         if match1.group("version") != match.group("version"):
             raise InvalidVersionError(
                 f"building package for {current} from '{gdata['ref']}' "
                 f"branch ({match.groupdict()} mismatch {match1.groupdict()})"
             )
         if match.group("what") == "beta":
             result["version"] = f"{match1.group('version')}b{gdata['run_number']}"
+            result["workflow"] = "beta"
+        else:
+            result["workflow"] = "tags"
     return result
 
 
 def update_version(
     initfile: str | Path, github_dump: str | None = None, abort: bool = True
 ) -> str | None:
     """extracts version information from github_dump and updates initfile in-place
@@ -319,14 +327,15 @@
     return data["version"]
 
 
 def process(
     initfile: str | Path,
     github_dump: str | None = None,
     paths: str | Path | list[str | Path] | None = None,
+    fixers: dict[str, str] | None = None,
     abort: bool = True,
 ) -> dict[str, str | None]:
     """get version from github_dump and updates initfile/paths
 
     Args:
         paths (str, Path): path(s) to files jinja2 processeable
         initfile (str, Path): path to the __init__.py file with a __version__ variable
@@ -336,15 +345,17 @@
         str: the new version for the package
 
     Example:
         {'branch': 'beta/0.3.1',
          'build': 0,
          'current': '0.3.1',
          'hash': 'c9e484a*',
-         'version': '0.3.1b0'}
+         'version': '0.3.1b0',
+         'runid': 0
+        }
     """
     from argparse import Namespace
     from functools import partial
     from urllib.parse import quote
 
     from jinja2 import Environment
 
@@ -358,10 +369,13 @@
     data = get_data(initfile, github_dump, abort)
     set_module_var(initfile, "__version__", data["version"])
     set_module_var(initfile, "__hash__", data["hash"])
 
     env = Environment(autoescape=True)
     env.filters["urlquote"] = partial(quote, safe="")
     for path in list_of_paths(paths):
-        tmpl = env.from_string(path.read_text())
+        txt = path.read_text()
+        for old, new in (fixers or {}).items():
+            txt = txt.replace(old, new, 1)
+        tmpl = env.from_string(txt)
         path.write_text(tmpl.render(ctx=Context(**data)))
     return data
```

### Comparing `setuptools-github-0.3.1b74/tests/conftest.py` & `setuptools-github-0.3.2b75/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/tests/test_checks.py` & `setuptools-github-0.3.2b75/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/tests/test_cli.py` & `setuptools-github-0.3.2b75/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/tests/test_conftest.py` & `setuptools-github-0.3.2b75/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/tests/test_scm.py` & `setuptools-github-0.3.2b75/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/tests/test_script.py` & `setuptools-github-0.3.2b75/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b74/tests/test_tools.py` & `setuptools-github-0.3.2b75/tests/test_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 
 # this is the output from ${{ toJson(github) }}
 GITHUB = {
     "beta": {
         "ref": "refs/heads/beta/0.0.4",
         "sha": "2169f90c22e",
         "run_number": "8",
+        "run_id": 123,
     },
     "release": {
         "ref": "refs/tags/release/0.0.3",
         "sha": "5547365c82",
         "run_number": "3",
+        "run_id": 456,
     },
     "master": {
         "ref": "refs/heads/master",
         "sha": "2169f90c",
         "run_number": "20",
+        "run_id": 789,
     },
 }
 
 
 def T(txt):  # noqa: N802
     from textwrap import dedent
 
@@ -356,15 +359,17 @@
     assert data["hash"][-1] != "*"
 
     assert tfile.read_text() == f"""
 Key[branch] = master
 Key[build] = 0
 Key[current] = 1.2.3
 Key[hash] = {data['hash']}
+Key[runid] = 0
 Key[version] = 1.2.3
+Key[workflow] = master
 """
 
     # clean and switch to new branch
     repo.revert(repo.initfile)
     write_tfile(tfile)
     repo.branch("beta/1.2.3", "master")
 
@@ -372,9 +377,11 @@
     assert data["hash"][-1] != "*"
 
     assert tfile.read_text() == f"""
 Key[branch] = beta/1.2.3
 Key[build] = 0
 Key[current] = 1.2.3
 Key[hash] = {data['hash']}
+Key[runid] = 0
 Key[version] = 1.2.3b0
+Key[workflow] = beta
 """
```

