# Comparing `tmp/hatch_docstring_description-1.0.tar.gz` & `tmp/hatch_docstring_description-1.0.1.tar.gz`

## Comparing `hatch_docstring_description-1.0.tar` & `hatch_docstring_description-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/.github/workflows/pub.yml
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/.vscode/settings.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/src/hatch_docstring_description/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/src/hatch_docstring_description/hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/src/hatch_docstring_description/py.typed
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/src/hatch_docstring_description/read_description.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/tests/test_basic.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/.gitignore
--rw-r--r--   0        0        0    34893 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/LICENSE.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/README.md
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/pyproject.toml
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/.github/workflows/pub.yml
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/.vscode/launch.json
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/src/hatch_docstring_description/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/src/hatch_docstring_description/hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/src/hatch_docstring_description/py.typed
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/src/hatch_docstring_description/read_description.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/tests/test_basic.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/.gitignore
+-rw-r--r--   0        0        0    34893 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/README.rst
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/PKG-INFO
```

### Comparing `hatch_docstring_description-1.0/.github/workflows/ci.yml` & `hatch_docstring_description-1.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `hatch_docstring_description-1.0/src/hatch_docstring_description/read_description.py` & `hatch_docstring_description-1.0.1/src/hatch_docstring_description/read_description.py`

 * *Files identical despite different names*

### Comparing `hatch_docstring_description-1.0/tests/test_basic.py` & `hatch_docstring_description-1.0.1/tests/test_basic.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 
 import pytest
 from hatchling.metadata.core import ProjectMetadata
+from hatchling.plugin.manager import PluginManager
 
 from hatch_docstring_description.read_description import ReadDescriptionHook
 
 # TODO: should hatch support single file modules? "mypkg.py", "src/mypkg.py"
 
 
 @pytest.fixture(params=["mypkg/__init__.py", "src/mypkg/__init__.py"])
@@ -18,7 +19,14 @@
 
 
 def test_basic(tmp_path, basic_project):
     hook = ReadDescriptionHook(tmp_path, {})
     metadata = ProjectMetadata(tmp_path, None).config["project"]
     hook.update(metadata)
     assert metadata["description"] == "A docstring."
+
+
+def test_load_plugin():
+    pm = PluginManager()
+    pm.metadata_hook.collect(include_third_party=True)
+    plugin = pm.manager.get_plugin("docstring-description")
+    assert plugin.hatch_register_metadata() is ReadDescriptionHook
```

### Comparing `hatch_docstring_description-1.0/LICENSE.md` & `hatch_docstring_description-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hatch_docstring_description-1.0/pyproject.toml` & `hatch_docstring_description-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-docstring-description"
 dynamic = ["version", "description"]
-readme = "README.md"
+readme = "README.rst"
 requires-python = ">=3.9"
 license = "GPL-3.0-or-later"
 authors = [
   { name = "Philipp A.", email = "flying-sheep@web.de" },
 ]
 # urls.Documentation = "https://github.com/flying-sheep/hatch-docstring-description#readme"
 urls.Issues = "https://github.com/flying-sheep/hatch-docstring-description/issues"
@@ -19,15 +19,15 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Framework :: Hatch",
 ]
 dependencies = ["hatchling"]
 
 [project.entry-points.hatch]
-aws = "hatch_docstring_description.hooks"
+docstring-description = "hatch_docstring_description.hooks"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
```

### Comparing `hatch_docstring_description-1.0/PKG-INFO` & `hatch_docstring_description-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 Metadata-Version: 2.1
 Name: hatch-docstring-description
-Version: 1.0
+Version: 1.0.1
 Project-URL: Issues, https://github.com/flying-sheep/hatch-docstring-description/issues
 Project-URL: Source, https://github.com/flying-sheep/hatch-docstring-description
 Author-email: "Philipp A." <flying-sheep@web.de>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Hatch
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: hatchling
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 
-# hatch-docstring-description
+hatch-docstring-description
+===========================
 
-[![PyPI - Version](https://img.shields.io/pypi/v/hatch-docstring-description.svg)](https://pypi.org/project/hatch-docstring-description)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hatch-docstring-description.svg)](https://pypi.org/project/hatch-docstring-description)
-[![Coverage](https://codecov.io/github/flying-sheep/hatch-docstring-description/branch/main/graph/badge.svg?token=FZCw1cXSTL)](https://codecov.io/github/flying-sheep/hatch-docstring-description)
+|PyPI Version| |PyPI Python Version| |Coverage|
 
+Usage
 -----
 
-**Table of Contents**
+#. Include it as a plugin to your ``pyproject.toml``:
 
-- [Installation](#installation)
-- [License](#license)
+   .. code:: toml
 
-## Installation
+      [build-system]
+      requires = ["hatchling", "hatch-docstring-description"]
+      build-backend = "hatchling.build"
 
-```console
-pip install hatch-docstring-description
-```
+#. Mark your ``description`` field as ``dynamic``:
 
-## License
+   .. code:: toml
 
-`hatch-docstring-description` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+      [project]
+      dynamic = ["description"]
+
+License
+-------
+
+``hatch-docstring-description`` is distributed under the terms of the `GPL 3 (or later)`_ license.
+
+
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/hatch-docstring-description.svg
+   :target: https://pypi.org/project/hatch-docstring-description
+.. |PyPI Python Version| image:: https://img.shields.io/pypi/pyversions/hatch-docstring-description.svg
+   :target: https://pypi.org/project/hatch-docstring-description
+.. |Coverage| image:: https://codecov.io/github/flying-sheep/hatch-docstring-description/branch/main/graph/badge.svg?token=FZCw1cXSTL
+   :target: https://codecov.io/github/flying-sheep/hatch-docstring-description
+
+.. _GPL 3 (or later): https://spdx.org/licenses/GPL-3.0-or-later.html
```

