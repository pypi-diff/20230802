# Comparing `tmp/ambient_package_update-23.7.3.tar.gz` & `tmp/ambient_package_update-23.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_package_update-23.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ambient_package_update-23.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ambient_package_update-23.7.3.tar` & `ambient_package_update-23.7.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient_package_update-23.7.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient_package_update-23.7.3/.gitignore
--rw-r--r--   0        0        0      905 2023-08-02 13:38:41.991309 ambient_package_update-23.7.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1682 2023-08-02 13:45:44.559296 ambient_package_update-23.7.3/CHANGES.md
--rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient_package_update-23.7.3/LICENSE.md
--rw-r--r--   0        0        0     4642 2023-08-02 13:45:44.546686 ambient_package_update-23.7.3/README.md
--rw-r--r--   0        0        0       93 2023-08-02 13:40:21.905102 ambient_package_update-23.7.3/ambient_package_update/__init__.py
--rw-r--r--   0        0        0     3773 2023-05-22 13:32:26.216194 ambient_package_update-23.7.3/ambient_package_update/cli.py
--rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient_package_update-23.7.3/ambient_package_update/metadata/__init__.py
--rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient_package_update-23.7.3/ambient_package_update/metadata/author.py
--rw-r--r--   0        0        0      454 2023-05-09 16:06:49.855781 ambient_package_update-23.7.3/ambient_package_update/metadata/constants.py
--rw-r--r--   0        0        0      592 2023-05-10 08:37:32.317360 ambient_package_update-23.7.3/ambient_package_update/metadata/package.py
--rw-r--r--   0        0        0      192 2023-05-22 13:32:26.216194 ambient_package_update-23.7.3/ambient_package_update/metadata/readme.py
--rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient_package_update-23.7.3/ambient_package_update/metadata/ruff_ignored_inspection.py
--rw-r--r--   0        0        0       82 2023-05-22 13:32:26.216194 ambient_package_update-23.7.3/ambient_package_update/templates/.coveragerc.tpl
--rw-r--r--   0        0        0      288 2023-05-22 13:32:26.216194 ambient_package_update-23.7.3/ambient_package_update/templates/.editorconfig.tpl
--rw-r--r--   0        0        0     1784 2023-05-22 13:32:26.216194 ambient_package_update-23.7.3/ambient_package_update/templates/.github/workflows/ci.yml.tpl
--rw-r--r--   0        0        0      904 2023-07-25 07:49:48.645779 ambient_package_update-23.7.3/ambient_package_update/templates/.pre-commit-config.yaml.tpl
--rw-r--r--   0        0        0      551 2023-05-22 13:32:26.216194 ambient_package_update-23.7.3/ambient_package_update/templates/.readthedocs.yml.tpl
--rw-r--r--   0        0        0     1121 2023-05-22 13:32:26.216194 ambient_package_update-23.7.3/ambient_package_update/templates/LICENSE.md.tpl
--rw-r--r--   0        0        0      137 2023-05-22 13:32:26.216194 ambient_package_update-23.7.3/ambient_package_update/templates/MANIFEST.in.tpl
--rw-r--r--   0        0        0     5394 2023-08-02 13:46:57.670710 ambient_package_update-23.7.3/ambient_package_update/templates/README.md.tpl
--rw-r--r--   0        0        0      654 2023-05-22 13:32:26.216194 ambient_package_update-23.7.3/ambient_package_update/templates/docs/Makefile.tpl
--rw-r--r--   0        0        0     2847 2023-05-22 13:32:26.216194 ambient_package_update-23.7.3/ambient_package_update/templates/docs/conf.py.tpl
--rw-r--r--   0        0        0      795 2023-05-22 13:32:26.216194 ambient_package_update-23.7.3/ambient_package_update/templates/docs/make.bat.tpl
--rw-r--r--   0        0        0     3726 2023-07-25 12:26:56.740200 ambient_package_update-23.7.3/ambient_package_update/templates/pyproject.toml.tpl
--rw-r--r--   0        0        0       56 2023-05-22 13:32:26.216194 ambient_package_update-23.7.3/ambient_package_update/templates/pytest.init.tpl
--rw-r--r--   0        0        0       50 2023-05-22 13:32:26.231832 ambient_package_update-23.7.3/ambient_package_update/templates/scripts/publish_to_pypi.ps1.tpl
--rw-r--r--   0        0        0       50 2023-05-22 13:32:26.231832 ambient_package_update-23.7.3/ambient_package_update/templates/scripts/publish_to_pypi.sh.tpl
--rw-r--r--   0        0        0       69 2023-05-22 13:32:26.231832 ambient_package_update-23.7.3/ambient_package_update/templates/setup.cfg.tpl
--rw-r--r--   0        0        0     2549 2023-07-25 08:59:34.407282 ambient_package_update-23.7.3/pyproject.toml
--rw-r--r--   0        0        0     1741 2023-08-02 13:41:51.817423 ambient_package_update-23.7.3/requirements.txt
--rw-r--r--   0        0        0       50 2023-05-10 08:28:40.436182 ambient_package_update-23.7.3/scripts/unix/publish_to_pypi.sh
--rw-r--r--   0        0        0      566 2023-05-09 08:09:25.681131 ambient_package_update-23.7.3/scripts/unix/setup_venv_unix.sh
--rw-r--r--   0        0        0       50 2023-05-10 08:28:40.436182 ambient_package_update-23.7.3/scripts/windows/publish_to_pypi.ps1
--rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient_package_update-23.7.3/scripts/windows/setup_venv.ps1
--rw-r--r--   0        0        0     5789 1970-01-01 00:00:00.000000 ambient_package_update-23.7.3/PKG-INFO
+-rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient_package_update-23.7.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient_package_update-23.7.4/.gitignore
+-rw-r--r--   0        0        0      905 2023-08-02 13:38:41.991309 ambient_package_update-23.7.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1738 2023-08-02 13:49:32.466055 ambient_package_update-23.7.4/CHANGES.md
+-rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient_package_update-23.7.4/LICENSE.md
+-rw-r--r--   0        0        0     4519 2023-08-02 13:49:03.698717 ambient_package_update-23.7.4/README.md
+-rw-r--r--   0        0        0       93 2023-08-02 13:49:32.466055 ambient_package_update-23.7.4/ambient_package_update/__init__.py
+-rw-r--r--   0        0        0     3773 2023-05-22 13:32:26.216194 ambient_package_update-23.7.4/ambient_package_update/cli.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient_package_update-23.7.4/ambient_package_update/metadata/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient_package_update-23.7.4/ambient_package_update/metadata/author.py
+-rw-r--r--   0        0        0      454 2023-05-09 16:06:49.855781 ambient_package_update-23.7.4/ambient_package_update/metadata/constants.py
+-rw-r--r--   0        0        0      592 2023-05-10 08:37:32.317360 ambient_package_update-23.7.4/ambient_package_update/metadata/package.py
+-rw-r--r--   0        0        0      192 2023-05-22 13:32:26.216194 ambient_package_update-23.7.4/ambient_package_update/metadata/readme.py
+-rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient_package_update-23.7.4/ambient_package_update/metadata/ruff_ignored_inspection.py
+-rw-r--r--   0        0        0       82 2023-05-22 13:32:26.216194 ambient_package_update-23.7.4/ambient_package_update/templates/.coveragerc.tpl
+-rw-r--r--   0        0        0      288 2023-05-22 13:32:26.216194 ambient_package_update-23.7.4/ambient_package_update/templates/.editorconfig.tpl
+-rw-r--r--   0        0        0     1784 2023-05-22 13:32:26.216194 ambient_package_update-23.7.4/ambient_package_update/templates/.github/workflows/ci.yml.tpl
+-rw-r--r--   0        0        0      904 2023-07-25 07:49:48.645779 ambient_package_update-23.7.4/ambient_package_update/templates/.pre-commit-config.yaml.tpl
+-rw-r--r--   0        0        0      551 2023-05-22 13:32:26.216194 ambient_package_update-23.7.4/ambient_package_update/templates/.readthedocs.yml.tpl
+-rw-r--r--   0        0        0     1121 2023-05-22 13:32:26.216194 ambient_package_update-23.7.4/ambient_package_update/templates/LICENSE.md.tpl
+-rw-r--r--   0        0        0      137 2023-05-22 13:32:26.216194 ambient_package_update-23.7.4/ambient_package_update/templates/MANIFEST.in.tpl
+-rw-r--r--   0        0        0     5243 2023-08-02 13:49:03.698717 ambient_package_update-23.7.4/ambient_package_update/templates/README.md.tpl
+-rw-r--r--   0        0        0      654 2023-05-22 13:32:26.216194 ambient_package_update-23.7.4/ambient_package_update/templates/docs/Makefile.tpl
+-rw-r--r--   0        0        0     2847 2023-05-22 13:32:26.216194 ambient_package_update-23.7.4/ambient_package_update/templates/docs/conf.py.tpl
+-rw-r--r--   0        0        0      795 2023-05-22 13:32:26.216194 ambient_package_update-23.7.4/ambient_package_update/templates/docs/make.bat.tpl
+-rw-r--r--   0        0        0     3726 2023-07-25 12:26:56.740200 ambient_package_update-23.7.4/ambient_package_update/templates/pyproject.toml.tpl
+-rw-r--r--   0        0        0       56 2023-05-22 13:32:26.216194 ambient_package_update-23.7.4/ambient_package_update/templates/pytest.init.tpl
+-rw-r--r--   0        0        0       50 2023-05-22 13:32:26.231832 ambient_package_update-23.7.4/ambient_package_update/templates/scripts/publish_to_pypi.ps1.tpl
+-rw-r--r--   0        0        0       50 2023-05-22 13:32:26.231832 ambient_package_update-23.7.4/ambient_package_update/templates/scripts/publish_to_pypi.sh.tpl
+-rw-r--r--   0        0        0       69 2023-05-22 13:32:26.231832 ambient_package_update-23.7.4/ambient_package_update/templates/setup.cfg.tpl
+-rw-r--r--   0        0        0     2549 2023-07-25 08:59:34.407282 ambient_package_update-23.7.4/pyproject.toml
+-rw-r--r--   0        0        0     1741 2023-08-02 13:41:51.817423 ambient_package_update-23.7.4/requirements.txt
+-rw-r--r--   0        0        0       50 2023-05-10 08:28:40.436182 ambient_package_update-23.7.4/scripts/unix/publish_to_pypi.sh
+-rw-r--r--   0        0        0      566 2023-05-09 08:09:25.681131 ambient_package_update-23.7.4/scripts/unix/setup_venv_unix.sh
+-rw-r--r--   0        0        0       50 2023-05-10 08:28:40.436182 ambient_package_update-23.7.4/scripts/windows/publish_to_pypi.ps1
+-rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient_package_update-23.7.4/scripts/windows/setup_venv.ps1
+-rw-r--r--   0        0        0     5667 1970-01-01 00:00:00.000000 ambient_package_update-23.7.4/PKG-INFO
```

### Comparing `ambient_package_update-23.7.3/.gitignore` & `ambient_package_update-23.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/.pre-commit-config.yaml` & `ambient_package_update-23.7.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/CHANGES.md` & `ambient_package_update-23.7.4/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+**23.7.4 (2023-08-02)**
+* Removed duplicated badges
+
 **23.7.3 (2023-08-02)**
 * Updated linters
 * Updated readme to show that this is a general purpose package
 * Added PyPI badge to rendered readme
 
 * **23.7.2 (2023-07-25)**
 * Bugfix with supported Django versions
```

### Comparing `ambient_package_update-23.7.3/LICENSE.md` & `ambient_package_update-23.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/README.md` & `ambient_package_update-23.7.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-[![pypi](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://pypi.python.org/pypi/ambient-package-update/)
-[![Downloads](https://pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
 [![PyPI release](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://img.shields.io/pypi/v/ambient-package-update.svg)
+[![Downloads](https://pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
 
 # Ambient Package Update
 
 This repository will help keep all Python packages following a certain basic structure tidy and up-to-date. It's being 
 maintained by [Ambient Digital](https://ambient.digital). 
 
 This package will render all required configuration and installation files for your target package.
```

### Comparing `ambient_package_update-23.7.3/ambient_package_update/cli.py` & `ambient_package_update-23.7.4/ambient_package_update/cli.py`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/ambient_package_update/metadata/package.py` & `ambient_package_update-23.7.4/ambient_package_update/metadata/package.py`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/ambient_package_update/templates/.github/workflows/ci.yml.tpl` & `ambient_package_update-23.7.4/ambient_package_update/templates/.github/workflows/ci.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/ambient_package_update/templates/.pre-commit-config.yaml.tpl` & `ambient_package_update-23.7.4/ambient_package_update/templates/.pre-commit-config.yaml.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/ambient_package_update/templates/.readthedocs.yml.tpl` & `ambient_package_update-23.7.4/ambient_package_update/templates/.readthedocs.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/ambient_package_update/templates/LICENSE.md.tpl` & `ambient_package_update-23.7.4/ambient_package_update/templates/LICENSE.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/ambient_package_update/templates/README.md.tpl` & `ambient_package_update-23.7.4/ambient_package_update/templates/README.md.tpl`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-[![pypi](https://img.shields.io/pypi/v/{{ package_name|replace("_", "-") }}.svg)](https://pypi.python.org/pypi/{{ package_name|replace("_", "-") }}/)
+[![PyPI release](https://img.shields.io/pypi/v/{{ package_name|replace("_", "-") }}.svg)](https://img.shields.io/pypi/v/{{ package_name|replace("_", "-") }}.svg)
 [![Downloads](https://pepy.tech/badge/{{ package_name|replace("_", "-") }})](https://pepy.tech/project/{{ package_name|replace("_", "-") }})
 [![Documentation Status](https://readthedocs.org/projects/{{ package_name|replace("_", "-") }}/badge/?version=latest)](https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/?badge=latest)
-[![PyPI release](https://img.shields.io/pypi/v/{{ package_name|replace("_", "-") }}.svg)](https://img.shields.io/pypi/v/{{ package_name|replace("_", "-") }}.svg)
 
 {{ readme_content.tagline }}
 
 * [PyPI](https://pypi.org/project/{{ package_name|replace("_", "-") }}/)
 * [GitHub](https://github.com/ambient-innovation/{{ package_name|replace("_", "-") }})
 * [Full documentation](https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/index.html)
 * Creator & Maintainer: [Ambient Digital](https://ambient.digital)
```

### Comparing `ambient_package_update-23.7.3/ambient_package_update/templates/docs/Makefile.tpl` & `ambient_package_update-23.7.4/ambient_package_update/templates/docs/Makefile.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/ambient_package_update/templates/docs/conf.py.tpl` & `ambient_package_update-23.7.4/ambient_package_update/templates/docs/conf.py.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/ambient_package_update/templates/docs/make.bat.tpl` & `ambient_package_update-23.7.4/ambient_package_update/templates/docs/make.bat.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/ambient_package_update/templates/pyproject.toml.tpl` & `ambient_package_update-23.7.4/ambient_package_update/templates/pyproject.toml.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/pyproject.toml` & `ambient_package_update-23.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/requirements.txt` & `ambient_package_update-23.7.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/scripts/unix/setup_venv_unix.sh` & `ambient_package_update-23.7.4/scripts/unix/setup_venv_unix.sh`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.3/PKG-INFO` & `ambient_package_update-23.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-package-update
-Version: 23.7.3
+Version: 23.7.4
 Summary: Ambient package update tool for clean and swift maintenance
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -22,17 +22,16 @@
 Requires-Dist: black~=23.7
 Project-URL: Bugtracker, https://github.com/ambient-innovation/ambient-package-update/issues
 Project-URL: Changelog, https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md
 Project-URL: Documentation, https://github.com/ambient-innovation/ambient-package-update/blob/master/README.md
 Project-URL: Homepage, https://github.com/ambient-innovation/ambient-package-update/
 Project-URL: Maintained by, https://ambient.digital/
 
-[![pypi](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://pypi.python.org/pypi/ambient-package-update/)
-[![Downloads](https://pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
 [![PyPI release](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://img.shields.io/pypi/v/ambient-package-update.svg)
+[![Downloads](https://pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
 
 # Ambient Package Update
 
 This repository will help keep all Python packages following a certain basic structure tidy and up-to-date. It's being 
 maintained by [Ambient Digital](https://ambient.digital). 
 
 This package will render all required configuration and installation files for your target package.
```

