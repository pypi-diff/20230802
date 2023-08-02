# Comparing `tmp/jinjanator_plugin_ansible-23.2.0.tar.gz` & `tmp/jinjanator_plugin_ansible-23.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jul 24 20:11:46 2023, max compression
+gzip compressed data, last modified: Wed Aug  2 18:54:54 2023, max compression
```

## Comparing `jinjanator_plugin_ansible-23.2.0.tar` & `jinjanator_plugin_ansible-23.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1430 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     2817 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/src/jinjanator_plugin_ansible/__init__.py
--rw-r--r--   0        0        0     1405 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/src/jinjanator_plugin_ansible/plugin.py
--rw-r--r--   0        0        0        0 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/src/jinjanator_plugin_ansible/py.typed
--rw-r--r--   0        0        0      967 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/tests/test_plugin.py
--rw-r--r--   0        0        0       32 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/LICENSE
--rw-r--r--   0        0        0     6477 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/pyproject.toml
--rw-r--r--   0        0        0     2125 2023-07-24 20:11:46.000000 jinjanator_plugin_ansible-23.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1725 2023-08-02 18:54:54.000000 jinjanator_plugin_ansible-23.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2817 2023-08-02 18:54:54.000000 jinjanator_plugin_ansible-23.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 18:54:54.000000 jinjanator_plugin_ansible-23.3.0/src/jinjanator_plugin_ansible/__init__.py
+-rw-r--r--   0        0        0     1612 2023-08-02 18:54:54.000000 jinjanator_plugin_ansible-23.3.0/src/jinjanator_plugin_ansible/plugin.py
+-rw-r--r--   0        0        0        0 2023-08-02 18:54:54.000000 jinjanator_plugin_ansible-23.3.0/src/jinjanator_plugin_ansible/py.typed
+-rw-r--r--   0        0        0      638 2023-08-02 18:54:54.000000 jinjanator_plugin_ansible-23.3.0/tests/test_plugin.py
+-rw-r--r--   0        0        0       32 2023-08-02 18:54:54.000000 jinjanator_plugin_ansible-23.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2023-08-02 18:54:54.000000 jinjanator_plugin_ansible-23.3.0/LICENSE
+-rw-r--r--   0        0        0     6343 2023-08-02 18:54:54.000000 jinjanator_plugin_ansible-23.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1857 2023-08-02 18:54:54.000000 jinjanator_plugin_ansible-23.3.0/PKG-INFO
```

### Comparing `jinjanator_plugin_ansible-23.2.0/CHANGELOG.md` & `jinjanator_plugin_ansible-23.3.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,37 +11,45 @@
 The **second number** is incremented with each release, starting at 1
 for each year.
 
 The **third number** is when we need to start branches for older
 releases (only for emergencies).
 
 Committed changes for the next release can be found in the ["changelog.d"
-directory](https://github.com/kpfleming/jinjanator/tree/main/changelog.d)
+directory](https://github.com/kpfleming/jinjanator-plugin-ansible/tree/main/changelog.d)
 in the project repository.
 
 <!--
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 
-See https://github.com/kpfleming/jinjanator/blob/main/.github/CONTRIBUTING.md#changelog for details.
+See https://github.com/kpfleming/jinjanator-plugin-ansible/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
-## [23.2.0](https://github.com/kpfleming/jinjanator/tree/23.2.0) - 2023-07-24
+## [23.3.0](https://github.com/kpfleming/jinjanator-plugin-ansible/tree/23.3.0) - 2023-08-02
+
+### Backwards-incompatible Changes
+
+- Updated to plugins API 23.4.
+  [#4](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/4)
+
+
+## [23.2.0](https://github.com/kpfleming/jinjanator-plugin-ansible/tree/23.2.0) - 2023-07-24
 
 ### Backwards-incompatible Changes
 
 - Increased minimum Python version to 3.9 to ensure Ansible compatibility.
   [#1](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/1)
 
 
 ### Additions
 
 - Add remaining filters and tests from the base Ansible collection.
   [#1](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/1)
 
 
-## [23.1.0](https://github.com/kpfleming/jinjanator/tree/23.1.0) - 2023-07-24
+## [23.1.0](https://github.com/kpfleming/jinjanator-plugin-ansible/tree/23.1.0) - 2023-07-24
 
 Initial release!
```

### Comparing `jinjanator_plugin_ansible-23.2.0/README.md` & `jinjanator_plugin_ansible-23.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jinjanator_plugin_ansible-23.2.0/src/jinjanator_plugin_ansible/plugin.py` & `jinjanator_plugin_ansible-23.3.0/src/jinjanator_plugin_ansible/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from __future__ import annotations
 
+import importlib
+
 from typing import cast
 
 import ansible.plugins.filter.core as filter_core  # type: ignore[import]
 import ansible.plugins.filter.mathstuff as filter_mathstuff  # type: ignore[import]
 import ansible.plugins.filter.urls as filter_urls  # type: ignore[import]
 import ansible.plugins.filter.urlsplit as filter_urlsplit  # type: ignore[import]
 import ansible.plugins.test.core as test_core  # type: ignore[import]
 import ansible.plugins.test.files as test_files  # type: ignore[import]
 import ansible.plugins.test.mathstuff as test_mathstuff  # type: ignore[import]
 import ansible.plugins.test.uri as test_uri  # type: ignore[import]
 
 from jinjanator_plugins import (
     Filters,
+    Identity,
     Tests,
     plugin_filters_hook,
+    plugin_identity_hook,
     plugin_tests_hook,
 )
 
 
+@plugin_identity_hook
+def plugin_identities() -> Identity:
+    return f"ansible (using ansible-core {importlib.metadata.version('ansible-core')})"
+
+
 @plugin_filters_hook
 def plugin_filters() -> Filters:
     return cast(
         Filters,
         {
             **filter_core.FilterModule().filters(),
             **filter_mathstuff.FilterModule().filters(),
```

### Comparing `jinjanator_plugin_ansible-23.2.0/LICENSE` & `jinjanator_plugin_ansible-23.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjanator_plugin_ansible-23.2.0/pyproject.toml` & `jinjanator_plugin_ansible-23.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ]
 dynamic = [
   "readme",
   "version",
 ]
 dependencies = [
   "ansible-core",
-  "jinjanator-plugins==23.1.*",
+  "jinjanator-plugins==23.4.*",
 ]
 [project.urls]
 "Bug Tracker" = "https://github.com/kpfleming/jinjanator-plugin-ansible/issues"
 "Homepage" = "https://github.com/kpfleming/jinjanator-plugin-ansible"
 [project.entry-points.jinjanator]
 ansible = "jinjanator_plugin_ansible.plugin"
 
@@ -45,17 +45,19 @@
 skip-install = true
 dependencies = [
   "towncrier",
 ]
 
 [tool.hatch.envs.changelog.scripts]
 draft = [
+  "rm -f changelog.d/*~",
   "towncrier build --version main --draft",
 ]
 release = [
+  "rm -f changelog.d/*~",
   "towncrier build --yes --version {args}",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build]
@@ -77,17 +79,15 @@
 ]
 
 [tool.hatch.envs.default]
 python = "3.11"
 
 [tool.hatch.envs.lint]
 dependencies = [
-    "attrs", # needed for type-checking tests
     "black",
-    "jinjanator", # needed for type-checking tests
     "ruff",
     "mypy",
     "pytest", # needed for type-checking tests
 ]
 
 [tool.hatch.envs.lint.scripts]
 lint = [
@@ -105,15 +105,14 @@
      "shellcheck workflow-support/*.sh",
 ]
 
 [tool.hatch.envs.ci]
 dependencies = [
     "attrs",
     "coverage[toml]",
-    "jinjanator",
     "pytest",
     "pytest-cov",
     "pytest-icdiff",
 ]
 
 [[tool.hatch.envs.ci.matrix]]
 python = [
@@ -122,18 +121,16 @@
 "3.11",
 "3.12",
 ]
 
 [tool.hatch.envs.ci.scripts]
 ci = [
     "rm -f .coverage",
-    # run tests
-    "pytest --verbose --cov-append  --cov-branch --cov-fail-under=100 --cov=jinjanator_plugin_ansible",
-    # produce a coverage report with 'missing' lines indicated
-    "coverage report -m",
+    "pytest --verbose --cov-append  --cov-branch --cov=jinjanator_plugin_ansible",
+    "coverage report --show-missing --fail-under=100",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
```

### Comparing `jinjanator_plugin_ansible-23.2.0/PKG-INFO` & `jinjanator_plugin_ansible-23.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjanator-plugin-ansible
-Version: 23.2.0
+Version: 23.3.0
 Summary: Plugin which provides Ansible filters and tests to the Jinjanator tool
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator-plugin-ansible/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator-plugin-ansible
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>
 License: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Requires-Dist: ansible-core
-Requires-Dist: jinjanator-plugins==23.1.*
+Requires-Dist: jinjanator-plugins==23.4.*
 Description-Content-Type: text/markdown
 
 # *jinjanator-plugin-ansible*: Makes Ansible's filters and tests available in Jinjanator
 
 
 
 This plugin makes all of the filters and tests from the Ansible 'core'
@@ -41,19 +41,13 @@
 
 The Ansible filters and tests can be used in templates using the same
 names that would be used if the template was rendered by Ansible
 itself.
 ## Release Information
 ### Backwards-incompatible Changes
 
-- Increased minimum Python version to 3.9 to ensure Ansible compatibility.
-  [[#1](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/1)](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/1)
-
-
-### Additions
-
-- Add remaining filters and tests from the base Ansible collection.
-  [[#1](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/1)](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/1)
+- Updated to plugins API 23.4.
+  [[#4](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/4)](https://github.com/kpfleming/jinjanator-plugin-ansible/issues/4)
 
 
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator-plugin-ansible/blob/main/CHANGELOG.md)
```

