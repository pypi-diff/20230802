# Comparing `tmp/CSET-0.2.0.tar.gz` & `tmp/CSET-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CSET-0.2.0.tar", last modified: Fri Jun 16 09:15:52 2023, max compression
+gzip compressed data, was "CSET-0.3.0.tar", last modified: Wed Aug  2 10:21:34 2023, max compression
```

## Comparing `CSET-0.2.0.tar` & `CSET-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.389007 CSET-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-06-16 09:15:28.000000 CSET-0.2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-16 09:15:52.389007 CSET-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-16 09:15:28.000000 CSET-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-16 09:15:28.000000 CSET-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-16 09:15:52.393007 CSET-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.385007 CSET-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.389007 CSET-0.2.0/src/CSET/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.389007 CSET-0.2.0/src/CSET/operators/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.389007 CSET-0.2.0/src/CSET/operators/RECIPES/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/RECIPES/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-16 09:15:28.000000 CSET-0.2.0/src/CSET/operators/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.389007 CSET-0.2.0/src/CSET.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-16 09:15:52.000000 CSET-0.2.0/src/CSET.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-16 09:15:52.000000 CSET-0.2.0/src/CSET.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:15:52.000000 CSET-0.2.0/src/CSET.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 09:15:52.000000 CSET-0.2.0/src/CSET.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-16 09:15:52.000000 CSET-0.2.0/src/CSET.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 09:15:52.000000 CSET-0.2.0/src/CSET.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:15:52.389007 CSET-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_recipe_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-16 09:15:28.000000 CSET-0.2.0/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:21:34.568877 CSET-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-08-02 10:21:02.000000 CSET-0.3.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-02 10:21:34.568877 CSET-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-08-02 10:21:02.000000 CSET-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-08-02 10:21:02.000000 CSET-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-02 10:21:34.572877 CSET-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:21:34.564876 CSET-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:21:34.568877 CSET-0.3.0/src/CSET/
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-02 10:21:02.000000 CSET-0.3.0/src/CSET/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-02 10:21:02.000000 CSET-0.3.0/src/CSET/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-02 10:21:02.000000 CSET-0.3.0/src/CSET/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-08-02 10:21:02.000000 CSET-0.3.0/src/CSET/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:21:34.568877 CSET-0.3.0/src/CSET/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-08-02 10:21:02.000000 CSET-0.3.0/src/CSET/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-08-02 10:21:02.000000 CSET-0.3.0/src/CSET/operators/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-02 10:21:02.000000 CSET-0.3.0/src/CSET/operators/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-02 10:21:02.000000 CSET-0.3.0/src/CSET/operators/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-02 10:21:02.000000 CSET-0.3.0/src/CSET/operators/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-08-02 10:21:02.000000 CSET-0.3.0/src/CSET/operators/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-02 10:21:02.000000 CSET-0.3.0/src/CSET/operators/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:21:34.568877 CSET-0.3.0/src/CSET/recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 10:21:02.000000 CSET-0.3.0/src/CSET/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:21:34.568877 CSET-0.3.0/src/CSET.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-02 10:21:34.000000 CSET-0.3.0/src/CSET.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-02 10:21:34.000000 CSET-0.3.0/src/CSET.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 10:21:34.000000 CSET-0.3.0/src/CSET.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 10:21:34.000000 CSET-0.3.0/src/CSET.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-02 10:21:34.000000 CSET-0.3.0/src/CSET.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 10:21:34.000000 CSET-0.3.0/src/CSET.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:21:34.568877 CSET-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-08-02 10:21:02.000000 CSET-0.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-08-02 10:21:02.000000 CSET-0.3.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 10:21:02.000000 CSET-0.3.0/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-02 10:21:02.000000 CSET-0.3.0/tests/test_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-08-02 10:21:02.000000 CSET-0.3.0/tests/test_run_recipes.py
```

### Comparing `CSET-0.2.0/LICENCE` & `CSET-0.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `CSET-0.2.0/PKG-INFO` & `CSET-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: CSET
-Version: 0.2.0
-Summary: Convective Scale Evaluation Tool for evaluation and investigation of regional models.
+Version: 0.3.0
+Summary: Toolkit for evaluation and investigation of numerical models for weather and climate applications.
 Author: Met Office, NIWA
 License: Apache-2.0
 Project-URL: Documentation, https://metoffice.github.io/CSET
 Project-URL: Source, https://github.com/MetOffice/CSET
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # CSET
 
-CSET is a tool to aid in evaluating regional model configurations. It aims to
-replace the collection of bespoke scripts littering people’s home directories,
-reducing effort wasted on duplicating already existing code. This centralisation
-of diagnostics should also make evaluations more consistent and comparable.
-Development takes place in the CSET repository on GitHub.
+CSET is a toolkit for evaluation and investigation of numerical models for
+weather and climate applications. It aims to replace the collection of bespoke
+scripts littering people’s home directories, reducing effort wasted on
+duplicating already existing code. This centralisation of diagnostics should
+also make evaluations more consistent and comparable. Development takes place in
+the CSET repository on GitHub.
 
 Please read [the documentation](https://metoffice.github.io/CSET) to learn more
 about CSET, and how to use it.
 
 ## Contributing
 
 Contributions are readily welcomed! To get started with developing CSET visit
-the [Working
-Practices](https://metoffice.github.io/CSET/working-practices/#getting-started)
-section of the documentation.
+the [Contributing](https://metoffice.github.io/CSET/contributing/) section of
+the documentation.
 
 In addition to reading the working practices, the key
 recommendation is early communication. Open an [issue on
 Github](https://github.com/MetOffice/CSET/issues) with your proposed change or
 addition in the design phase, and then others can provide guidance early.
 
 ## Licence
```

### Comparing `CSET-0.2.0/README.md` & `CSET-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # CSET
 
-CSET is a tool to aid in evaluating regional model configurations. It aims to
-replace the collection of bespoke scripts littering people’s home directories,
-reducing effort wasted on duplicating already existing code. This centralisation
-of diagnostics should also make evaluations more consistent and comparable.
-Development takes place in the CSET repository on GitHub.
+CSET is a toolkit for evaluation and investigation of numerical models for
+weather and climate applications. It aims to replace the collection of bespoke
+scripts littering people’s home directories, reducing effort wasted on
+duplicating already existing code. This centralisation of diagnostics should
+also make evaluations more consistent and comparable. Development takes place in
+the CSET repository on GitHub.
 
 Please read [the documentation](https://metoffice.github.io/CSET) to learn more
 about CSET, and how to use it.
 
 ## Contributing
 
 Contributions are readily welcomed! To get started with developing CSET visit
-the [Working
-Practices](https://metoffice.github.io/CSET/working-practices/#getting-started)
-section of the documentation.
+the [Contributing](https://metoffice.github.io/CSET/contributing/) section of
+the documentation.
 
 In addition to reading the working practices, the key
 recommendation is early communication. Open an [issue on
 Github](https://github.com/MetOffice/CSET/issues) with your proposed change or
 addition in the design phase, and then others can provide guidance early.
 
 ## Licence
```

### Comparing `CSET-0.2.0/pyproject.toml` & `CSET-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "CSET"
-version = "0.2.0"
-description = "Convective Scale Evaluation Tool for evaluation and investigation of regional models."
+version = "0.3.0"
+description = "Toolkit for evaluation and investigation of numerical models for weather and climate applications."
 authors = [{ name = "Met Office" }, { name = "NIWA" }]
 readme = "README.md"
 license = { text = "Apache-2.0" }
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dependencies = [
     "numpy",
-    "scitools-iris",
+    "scitools-iris >= 3.6",
     "ruamel.yaml >= 0.17",
-    "importlib_resources >= 3.0.0 ; python_version < '3.9'",
+    "pygraphviz >= 1.11"
 ]
 
 [project.urls]
 Documentation = "https://metoffice.github.io/CSET"
 Source = "https://github.com/MetOffice/CSET"
 
 [project.scripts]
@@ -45,18 +45,18 @@
 [tool.tox]
 legacy_tox_ini = '''
 [tox]
 requires = tox-conda
 isolated_build = True
 envlist =
     coverage-clean
-    py310-linux-tests
-    py310-linux-docs
+    py311-linux-tests
+    py311-linux-docs
 
-[testenv:py{38,39,310,311}-lock]
+[testenv:py{39,310,311}-lock]
 allowlist_externals = cp
 conda_channels = conda-forge
 conda_create_args = --override-channels
 conda_deps =
     pip
     conda-lock
 description = Create explicit environment specification conda lock files for CSET dependencies.
@@ -67,29 +67,27 @@
     YMLFILE = {toxinidir}{/}requirements{/}environment.yml
 commands =
     cp "{env:YMLFILE}" "{env:TMPFILE}"
     # Hacky script to avoid having to have per-python-version yaml files.
     python3 -c 'from sys import version_info as v; fh = open("{env:TMPFILE}", "a"); fh.write(f"\n  - python =\{v.major\}.\{v.minor\}\n")'
     conda-lock --channel conda-forge --kind explicit --file {env:TMPFILE} --platform linux-64 --filename-template "{env:LOCKDIR}{envname}-\{platform\}.txt" {posargs}
 
-[testenv:py{38,39,310,311}-{linux,osx,win}-tests]
+[testenv:py{39,310,311}-{linux,osx,win}-tests]
 description = Run unit and integration tests with PyTest.
 conda_spec =
-    py38-linux: {toxinidir}{/}requirements{/}locks{/}py38-lock-linux-64.txt
     py39-linux: {toxinidir}{/}requirements{/}locks{/}py39-lock-linux-64.txt
     py310-linux: {toxinidir}{/}requirements{/}locks{/}py310-lock-linux-64.txt
     py311-linux: {toxinidir}{/}requirements{/}locks{/}py311-lock-linux-64.txt
 usedevelop = true
 depends = coverage-clean
 commands = pytest {posargs}
 
 [testenv:py{38,39,310,311}-{linux,osx,win}-docs]
 description = Invoke sphinx-build to build the HTML docs.
 conda_spec =
-    py38-linux: {toxinidir}{/}requirements{/}locks{/}py38-lock-linux-64.txt
     py39-linux: {toxinidir}{/}requirements{/}locks{/}py39-lock-linux-64.txt
     py310-linux: {toxinidir}{/}requirements{/}locks{/}py310-lock-linux-64.txt
     py311-linux: {toxinidir}{/}requirements{/}locks{/}py311-lock-linux-64.txt
 usedevelop = true
 commands = sphinx-build -d "docs/build/doctree" docs/source "docs/build/html" --color -W -bhtml {posargs}
 
 [testenv:build-package]
@@ -99,7 +97,11 @@
 commands = python3 -m build
 
 [testenv:coverage-clean]
 deps = coverage
 skip_install = true
 commands = coverage erase
 '''
+
+[tool.codespell]
+ignore-words-list = "lazyness,meaned"
+skip = "build,*.css,*.ipynb,*.js,*.html,*.svg,*.xml,.git"
```

### Comparing `CSET-0.2.0/src/CSET/__main__.py` & `CSET-0.3.0/src/CSET/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import sys  # pragma: no cover
-from . import main  # pragma: no cover
+import sys
+from CSET import main
 
-sys.exit(main())  # pragma: no cover
+sys.exit(main())
```

### Comparing `CSET-0.2.0/src/CSET/operators/_internal.py` & `CSET-0.3.0/src/CSET/operators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Internal functions used to run operators."""
+"""This subpackage contains all of CSET's operators."""
+
+# Import operators here so they are exported for use by recipes.
+from CSET.operators import constraints, read, write, filters, plot, misc
+
 
-import logging
 from pathlib import Path
 from typing import Union
 import inspect
-import ruamel.yaml
+import logging
+
 import CSET.operators
+from CSET._common import parse_recipe
+
+# Stop iris giving a warning whenever it loads something.
+from iris import FUTURE
+
+FUTURE.datum_support = True
 
 
 def get_operator(name: str):
     """
     Gets an operator by its name.
 
     Parameters
@@ -43,14 +53,15 @@
 
     Examples
     --------
     >>> CSET.operators.get_operator("read.read_cubes")
     <function read_cubes at 0x7fcf9353c8b0>
     """
 
+    logging.debug("get_operator(%s)", name)
     try:
         name_sections = name.split(".")
         operator = CSET.operators
         for section in name_sections:
             operator = getattr(operator, section)
         if callable(operator):
             return operator
@@ -88,56 +99,40 @@
         The recipe is not well formed.
 
     TypeError
         The provided recipe is not a stream or Path.
     """
 
     def step_parser(step: dict, step_input: any, output_file_path: Path) -> str:
+        """Executes a recipe step, recursively executing any sub-steps."""
         logging.debug(f"Executing step: {step}")
         kwargs = {}
         for key in step.keys():
             if key == "operator":
                 operator = get_operator(step["operator"])
                 logging.info(f"operator: {step['operator']}")
-            elif type(step[key]) == dict and "operator" in step[key]:
+            elif isinstance(step[key], dict) and "operator" in step[key]:
                 logging.debug(f"Recursing into argument: {key}")
                 kwargs[key] = step_parser(step[key], step_input, output_file_path)
             elif step[key] == "CSET_OUTPUT_PATH":
                 kwargs[key] = output_file_path
             else:
                 kwargs[key] = step[key]
-
-        logging.debug(f"args: {kwargs}")
-        logging.debug(f"step_input: {step_input}")
-
+        logging.debug("args: %s", kwargs)
+        logging.debug("step_input: %s", step_input)
         # If first argument of operator is explicitly defined, use that rather
         # than step_input. This is known through introspection of the operator.
         first_arg = next(iter(inspect.signature(operator).parameters.keys()))
-        logging.debug(f"first_arg: {first_arg}")
+        logging.debug("first_arg: %s", first_arg)
         if first_arg not in kwargs:
             return operator(step_input, **kwargs)
         else:
             return operator(**kwargs)
 
-    with ruamel.yaml.YAML(typ="safe", pure=True) as yaml:
-        try:
-            recipe = yaml.load(recipe_yaml)
-        except ruamel.yaml.parser.ParserError:
-            raise ValueError("ParserError: Invalid YAML")
-        except ruamel.yaml.error.YAMLStreamError:
-            raise TypeError("Must provide a stream (with a read method)")
+    recipe = parse_recipe(recipe_yaml)
 
-    logging.debug(recipe)
+    # Execute the recipe.
     step_input = input_file
-    try:
-        if len(recipe["steps"]) < 1:
-            raise ValueError("Recipe must have at least 1 step.")
-        for step in recipe["steps"]:
-            step_input = step_parser(step, step_input, output_file)
-    except KeyError as err:
-        raise ValueError("Invalid Recipe:", err)
-    except TypeError as err:
-        if recipe is None:
-            raise ValueError("Recipe must have at least 1 step.")
-        # This should never be reached.
-        raise err  # pragma: no cover
-    logging.info(f"Recipe output: {step_input}")
+    for step in recipe["steps"]:
+        step_input = step_parser(step, step_input, output_file)
+
+    logging.info("Recipe output: %s", step_input)
```

### Comparing `CSET-0.2.0/src/CSET/operators/constraints.py` & `CSET-0.3.0/src/CSET/operators/constraints.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,37 +17,37 @@
 """
 
 import iris
 import iris.cube
 from datetime import datetime
 
 
-def generate_stash_constraint(stash: str) -> iris.AttributeConstraint:
+def generate_stash_constraint(stash: str, **kwargs) -> iris.AttributeConstraint:
     """
     Operator that takes a stash string, and uses iris to generate a constraint
     to be passed into the read operator to minimize the CubeList the read
     operator loads and speed up loading.
 
     Arguments
     ---------
     stash: str
-        stash code to build iris constraint, currently using "m01s03i236"
+        stash code to build iris constraint, such as "m01s03i236"
 
     Returns
     -------
     stash_constraint: iris.AttributeConstraint
     """
 
     # At a later stage str list an option to combine constraints. Arguments
     # could be a list of stash codes that combined build the constraint.
     stash_constraint = iris.AttributeConstraint(STASH=stash)
     return stash_constraint
 
 
-def generate_var_constraint(varname: str) -> iris.Constraint:
+def generate_var_constraint(varname: str, **kwargs) -> iris.Constraint:
     """
     Operator that takes a CF compliant variable name string, and uses iris to
     generate a constraint to be passed into the read operator to minimize the
     CubeList the read operator loads and speed up loading.
 
     Arguments
     ---------
@@ -59,15 +59,15 @@
     varname_constraint: iris.Constraint
     """
 
     varname_constraint = iris.Constraint(name=varname)
     return varname_constraint
 
 
-def generate_cell_methods_constraint(cell_methods: list) -> iris.Constraint:
+def generate_cell_methods_constraint(cell_methods: list, **kwargs) -> iris.Constraint:
     """
     Operator that takes a list of cell methods and generates a constraint from
     that.
 
     Arguments
     ---------
     cell_methods: list
@@ -85,15 +85,15 @@
             return False
 
     cell_methods_constraint = iris.Constraint(cube_func=check_cell_methods)
     return cell_methods_constraint
 
 
 def generate_time_constraint(
-    time_start: str, time_end: str = None
+    time_start: str, time_end: str = None, **kwargs
 ) -> iris.AttributeConstraint:
     """
     Operator that takes one or two ISO 8601 date strings, and returns a
     constraint that selects values between those dates (inclusive).
 
     Arguments
     ---------
@@ -104,26 +104,26 @@
         ISO date for upper bound. If omitted it defaults to the same as
         time_start
 
     Returns
     -------
     time_constraint: iris.Constraint
     """
-    if type(time_start) == str:
+    if isinstance(time_start, str):
         time_start = datetime.fromisoformat(time_start)
     if time_end is None:
         time_end = time_start
-    elif type(time_end) == str:
+    elif isinstance(time_end, str):
         time_end = datetime.fromisoformat(time_end)
     time_constraint = iris.Constraint(time=lambda t: time_start <= t.point <= time_end)
     return time_constraint
 
 
 def combine_constraints(
-    constraint: iris.Constraint = iris.Constraint(), **kwargs
+    constraint: iris.Constraint = None, **kwargs
 ) -> iris.Constraint:
     """
     Operator that combines multiple constraints into one.
 
     Arguments
     ---------
     constraint: iris.Constraint
@@ -140,12 +140,17 @@
     combined_constraint: iris.Constraint
 
     Raises
     ------
     TypeError
         If the provided arguments are not constraints.
     """
+    # If the first argument is not a constraint, it is ignored. This handles the
+    # automatic passing of the previous step's output.
+    if isinstance(constraint, iris.Constraint):
+        combined_constraint = constraint
+    else:
+        combined_constraint = iris.Constraint()
 
-    combined_constraint = constraint
     for constr in kwargs.values():
         combined_constraint = combined_constraint & constr
     return combined_constraint
```

### Comparing `CSET-0.2.0/src/CSET/operators/filters.py` & `CSET-0.3.0/src/CSET/operators/filters.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,41 +14,43 @@
 
 """
 Operators to perform various kind of filtering.
 """
 
 import iris
 import iris.cube
+from typing import Union
 
 
 def filter_cubes(
-    cubelist: iris.cube.CubeList, constraint: iris.Constraint
+    cube: Union[iris.cube.Cube, iris.cube.CubeList],
+    constraint: iris.Constraint,
+    **kwargs,
 ) -> iris.cube.Cube:
     """
     Filters a cubelist down to a single cube based on a constraint.
 
     Arguments
     ---------
-    cubelist: iris.cube.CubeList
-        Cubes to iterate over
+    cube: iris.cube.Cube | iris.cube.CubeList
+        Cube(s) to iterate over
     constraint: iris.Constraint
         Constraint to extract
 
     Returns
     -------
-    cube: iris.cube.Cube
-        Single variable
+    iris.cube.Cube
 
     Raises
     ------
     ValueError
         If the constraint doesn't produce a single cube.
     """
 
-    filtered_cubes = cubelist.extract(constraint)
+    filtered_cubes = cube.extract(constraint)
 
     # Check filtered cubes is a CubeList containing one cube.
     if len(filtered_cubes) == 1:
         return filtered_cubes[0]
     else:
         raise ValueError(
             f"Constraint doesn't produce single cube. {constraint}\n{filtered_cubes}"
```

### Comparing `CSET-0.2.0/src/CSET/operators/misc.py` & `CSET-0.3.0/src/CSET/operators/misc.py`

 * *Files identical despite different names*

### Comparing `CSET-0.2.0/src/CSET/operators/plot.py` & `CSET-0.3.0/src/CSET/operators/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from pathlib import Path
 import iris
 import iris.cube
 import iris.quickplot as qplt
 import matplotlib.pyplot as plt
 
 
-def spatial_contour_plot(cube: iris.cube.Cube, file_path: Path) -> Path:
+def spatial_contour_plot(cube: iris.cube.Cube, file_path: Path, **kwargs) -> Path:
     """
     Plots a spatial variable onto a map.
 
     Parameters
     ----------
     cube: Cube
         An iris cube of the data to plot. It should be 2 dimensional (lat and lon).
```

### Comparing `CSET-0.2.0/src/CSET/operators/read.py` & `CSET-0.3.0/src/CSET/operators/write.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,40 +9,42 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Operators for reading various types of files from disk.
+Operators for writing various types of files to disk.
 """
 
 from pathlib import Path
+from typing import Union
 
 import iris
 import iris.cube
 
 
-def read_cubes(
-    loadpath: Path, constraint: iris.Constraint = None
-) -> iris.cube.CubeList:
+def write_cube_to_nc(
+    cube: Union[iris.cube.Cube, iris.cube.CubeList], file_path: Path, **kwargs
+) -> str:
     """
-    Read operator that takes a path string (can include wildcards), and uses
-    iris to load all the cubes matching stash and return a CubeList object.
+    A write operator that sits after the read operator. This operator expects
+    an iris cube object that will then be passed to MET for further processing.
 
     Arguments
     ---------
-    loadpath: pathlike
-        Path to where .pp/.nc files are located
-    constraint: iris.Constraint or iris.ConstraintCombination, optional
-        Constraints to filter by
+    cube: iris.cube.Cube | iris.cube.CubeList
+        Data to save
+    file_path: Path
+        Path to save the cubes too
 
     Returns
     -------
-    cubes: iris.cube.CubeList
-        Cubes extracted
+    file_path: Path
+        Filepath to saved .nc
     """
 
-    if constraint:
-        return iris.load(loadpath, constraint)
-    else:
-        return iris.load(loadpath)
+    # Ensure that output_file_path is a Path with a .nc suffix
+    file_path = Path(file_path).with_suffix(".nc")
+    # Save the file as nc compliant (iris should handle this)
+    iris.save(cube, file_path)
+    return file_path
```

### Comparing `CSET-0.2.0/src/CSET.egg-info/PKG-INFO` & `CSET-0.3.0/src/CSET.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: CSET
-Version: 0.2.0
-Summary: Convective Scale Evaluation Tool for evaluation and investigation of regional models.
+Version: 0.3.0
+Summary: Toolkit for evaluation and investigation of numerical models for weather and climate applications.
 Author: Met Office, NIWA
 License: Apache-2.0
 Project-URL: Documentation, https://metoffice.github.io/CSET
 Project-URL: Source, https://github.com/MetOffice/CSET
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # CSET
 
-CSET is a tool to aid in evaluating regional model configurations. It aims to
-replace the collection of bespoke scripts littering people’s home directories,
-reducing effort wasted on duplicating already existing code. This centralisation
-of diagnostics should also make evaluations more consistent and comparable.
-Development takes place in the CSET repository on GitHub.
+CSET is a toolkit for evaluation and investigation of numerical models for
+weather and climate applications. It aims to replace the collection of bespoke
+scripts littering people’s home directories, reducing effort wasted on
+duplicating already existing code. This centralisation of diagnostics should
+also make evaluations more consistent and comparable. Development takes place in
+the CSET repository on GitHub.
 
 Please read [the documentation](https://metoffice.github.io/CSET) to learn more
 about CSET, and how to use it.
 
 ## Contributing
 
 Contributions are readily welcomed! To get started with developing CSET visit
-the [Working
-Practices](https://metoffice.github.io/CSET/working-practices/#getting-started)
-section of the documentation.
+the [Contributing](https://metoffice.github.io/CSET/contributing/) section of
+the documentation.
 
 In addition to reading the working practices, the key
 recommendation is early communication. Open an [issue on
 Github](https://github.com/MetOffice/CSET/issues) with your proposed change or
 addition in the design phase, and then others can provide guidance early.
 
 ## Licence
```

