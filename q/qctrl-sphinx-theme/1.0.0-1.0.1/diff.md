# Comparing `tmp/qctrl_sphinx_theme-1.0.0.tar.gz` & `tmp/qctrl_sphinx_theme-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_sphinx_theme-1.0.0.tar", max compression
+gzip compressed data, was "qctrl_sphinx_theme-1.0.1.tar", max compression
```

## Comparing `qctrl_sphinx_theme-1.0.0.tar` & `qctrl_sphinx_theme-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    36653 2023-07-30 22:36:01.884897 qctrl_sphinx_theme-1.0.0/LICENSE
--rw-r--r--   0        0        0     1061 2023-07-30 22:36:01.884897 qctrl_sphinx_theme-1.0.0/README.md
--rw-r--r--   0        0        0     2175 2023-07-30 22:36:23.373118 qctrl_sphinx_theme-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1370 2023-07-30 22:36:23.381118 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/__init__.py
--rw-r--r--   0        0        0      467 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/breadcrumbs.html
--rw-r--r--   0        0        0        0 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/footer.html
--rw-r--r--   0        0        0     3347 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/layout.html
--rw-r--r--   0        0        0       78 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/searchbox.html
--rw-r--r--   0        0        0    17409 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/css/docsearch.css
--rw-r--r--   0        0        0     8860 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/css/qctrlsphinxtheme.css
--rw-r--r--   0        0        0     5430 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/favicon.ico
--rw-r--r--   0        0        0    26880 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon-180.png
--rw-r--r--   0        0        0    29759 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon-192.png
--rw-r--r--   0        0        0   122791 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon-512.png
--rw-r--r--   0        0        0     9545 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon.svg
--rw-r--r--   0        0        0    10694 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-logo.svg
--rw-r--r--   0        0        0   317604 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/social/image.jpg
--rw-r--r--   0        0        0     3209 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/js/qctrlsphinxtheme.js_t
--rw-r--r--   0        0        0      609 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/manifest.webmanifest
--rw-r--r--   0        0        0     1985 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/pygments.css
--rw-r--r--   0        0        0      251 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/theme.conf
--rw-r--r--   0        0        0     3222 1970-01-01 00:00:00.000000 qctrl_sphinx_theme-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-08-02 02:43:57.591461 qctrl_sphinx_theme-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1273 2023-08-02 02:43:57.591461 qctrl_sphinx_theme-1.0.1/README.md
+-rw-r--r--   0        0        0     2175 2023-08-02 02:44:16.783686 qctrl_sphinx_theme-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1369 2023-08-02 02:44:16.791686 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/__init__.py
+-rw-r--r--   0        0        0      467 2023-08-02 02:43:57.591461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/breadcrumbs.html
+-rw-r--r--   0        0        0        0 2023-08-02 02:43:57.591461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/footer.html
+-rw-r--r--   0        0        0     3347 2023-08-02 02:43:57.591461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/layout.html
+-rw-r--r--   0        0        0       78 2023-08-02 02:43:57.591461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/searchbox.html
+-rw-r--r--   0        0        0    17409 2023-08-02 02:43:57.591461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/css/docsearch.css
+-rw-r--r--   0        0        0     8860 2023-08-02 02:43:57.591461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/css/qctrlsphinxtheme.css
+-rw-r--r--   0        0        0     5430 2023-08-02 02:43:57.591461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/favicon.ico
+-rw-r--r--   0        0        0    26880 2023-08-02 02:43:57.591461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/img/q-ctrl-icon-180.png
+-rw-r--r--   0        0        0    29759 2023-08-02 02:43:57.591461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/img/q-ctrl-icon-192.png
+-rw-r--r--   0        0        0   122791 2023-08-02 02:43:57.595461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/img/q-ctrl-icon-512.png
+-rw-r--r--   0        0        0     9545 2023-08-02 02:43:57.595461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/img/q-ctrl-icon.svg
+-rw-r--r--   0        0        0    10694 2023-08-02 02:43:57.595461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/img/q-ctrl-logo.svg
+-rw-r--r--   0        0        0   317604 2023-08-02 02:43:57.595461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/img/social/image.jpg
+-rw-r--r--   0        0        0     3209 2023-08-02 02:43:57.595461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/js/qctrlsphinxtheme.js_t
+-rw-r--r--   0        0        0      609 2023-08-02 02:43:57.595461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/manifest.webmanifest
+-rw-r--r--   0        0        0     1985 2023-08-02 02:43:57.595461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/pygments.css
+-rw-r--r--   0        0        0      251 2023-08-02 02:43:57.595461 qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/theme.conf
+-rw-r--r--   0        0        0     3434 1970-01-01 00:00:00.000000 qctrl_sphinx_theme-1.0.1/PKG-INFO
```

### Comparing `qctrl_sphinx_theme-1.0.0/LICENSE` & `qctrl_sphinx_theme-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/pyproject.toml` & `qctrl_sphinx_theme-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-sphinx-theme"
-version = "1.0.0"
+version = "1.0.1"
 description = "Q-CTRL Sphinx Theme"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
```

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/__init__.py` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 """Q-CTRL Sphinx Theme"""
 import os
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __author__ = "Q-CTRL <support@q-ctrl.com>"
 
 # See https://www.sphinx-doc.org/en/master/development/theming.html#distribute-your-theme-as-a-python-package
 def setup(app):
     app.add_html_theme(
         "qctrl_sphinx_theme", os.path.abspath(os.path.dirname(__file__))
     )
 
-def get_environment_options():
+def get_html_theme_options():
     """
     Check each DocSearch and Segment theme option for an available
     environment variable and, if one exists, set it.
     """
     variables = [
         "DOCSEARCH_API_KEY",
         "DOCSEARCH_APP_ID",
```

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/layout.html` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/layout.html`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/css/docsearch.css` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/css/docsearch.css`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/css/qctrlsphinxtheme.css` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/css/qctrlsphinxtheme.css`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/favicon.ico` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon-180.png` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/img/q-ctrl-icon-180.png`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon-192.png` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/img/q-ctrl-icon-192.png`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon-512.png` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/img/q-ctrl-icon-512.png`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon.svg` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/img/q-ctrl-icon.svg`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-logo.svg` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/img/q-ctrl-logo.svg`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/social/image.jpg` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/img/social/image.jpg`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/js/qctrlsphinxtheme.js_t` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/js/qctrlsphinxtheme.js_t`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/manifest.webmanifest` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/pygments.css` & `qctrl_sphinx_theme-1.0.1/qctrlsphinxtheme/static/pygments.css`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-1.0.0/PKG-INFO` & `qctrl_sphinx_theme-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-sphinx-theme
-Version: 1.0.0
+Version: 1.0.1
 Summary: Q-CTRL Sphinx Theme
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -58,13 +58,23 @@
 [tool.poetry.dev-dependencies]
 qctrl-sphinx-theme = "~1.0.0"
 ```
 1. Add the following to `docs/conf.py` (this sets the Q-CTRL Sphinx Theme as the theme for your documentation):
   ```python
   html_theme = "qctrl_sphinx_theme"
   ```
-1. Update (or create) the `html_theme_options` dictionary in `docs/conf.py` using `qctrlsphinxtheme.get_environment_options` (this checks each DocSearch and Segment theme option for an available environment variable and, if one exists, sets it). For example:
+1. Update (or create) the `html_theme_options` dictionary in `docs/conf.py` using `qctrlsphinxtheme.get_html_theme_options` (this checks each DocSearch and Segment theme option for an available environment variable and, if one exists, sets it). For example:
+
+To update an `html_theme_options` dictionary:
+
+  ```python
+  from qctrlsphinxtheme import get_html_theme_options
+  html_theme_options.update(get_html_theme_options())
+  ```
+
+To create a `html_theme_options` dictionary:
+
   ```python
-  from qctrlsphinxtheme import get_environment_options
-  html_theme_options.update(get_environment_options())
+  from qctrlsphinxtheme import get_html_theme_options
+  html_theme_options = get_html_theme_options()
   ```
```

