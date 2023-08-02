# Comparing `tmp/aiida_ssh2win-0.1.0.tar.gz` & `tmp/aiida_ssh2win-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_ssh2win-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_ssh2win-0.1.0a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_ssh2win-0.1.0.tar` & `aiida_ssh2win-0.1.0a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0      195 2023-07-26 14:18:00.369274 aiida_ssh2win-0.1.0/.github/install_aiida_github.sh
--rw-r--r--   0        0        0     2011 2023-07-26 14:18:00.369274 aiida_ssh2win-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      760 2023-07-26 14:18:00.369274 aiida_ssh2win-0.1.0/.github/workflows/publish-on-pypi.yml
--rw-r--r--   0        0        0      115 2023-07-26 14:18:00.329274 aiida_ssh2win-0.1.0/.gitignore
--rw-r--r--   0        0        0     1388 2023-07-27 08:25:47.746890 aiida_ssh2win-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      121 2023-07-26 14:18:00.333274 aiida_ssh2win-0.1.0/.readthedocs.yml
--rw-r--r--   0        0        0     1072 2023-07-26 14:18:00.333274 aiida_ssh2win-0.1.0/LICENSE
--rw-r--r--   0        0        0     3095 2023-07-27 08:29:34.867917 aiida_ssh2win-0.1.0/README.md
--rw-r--r--   0        0        0      121 2023-08-02 14:06:46.826410 aiida_ssh2win-0.1.0/aiida_ssh2win/__init__.py
--rw-r--r--   0        0        0     2131 2023-07-27 08:29:15.460171 aiida_ssh2win-0.1.0/aiida_ssh2win/transport.py
--rw-r--r--   0        0        0      488 2023-07-26 14:18:00.317274 aiida_ssh2win-0.1.0/conftest.py
--rw-r--r--   0        0        0        7 2023-07-26 14:18:00.337274 aiida_ssh2win-0.1.0/docs/.gitignore
--rwxr-xr-x   0        0        0     1554 2023-07-26 14:18:00.337274 aiida_ssh2win-0.1.0/docs/Makefile
--rwxr-xr-x   0        0        0     7573 2023-07-26 14:18:00.345274 aiida_ssh2win-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0     2996 2023-07-26 14:18:00.349274 aiida_ssh2win-0.1.0/docs/source/developer_guide/index.rst
--rw-r--r--   0        0        0    76300 2023-07-26 14:18:00.357274 aiida_ssh2win-0.1.0/docs/source/images/AiiDA_transparent_logo.png
--rwxr-xr-x   0        0        0     1258 2023-07-26 14:18:00.345274 aiida_ssh2win-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0      627 2023-07-27 08:29:15.464171 aiida_ssh2win-0.1.0/docs/source/user_guide/get_started.rst
--rw-r--r--   0        0        0       94 2023-07-26 14:18:00.361274 aiida_ssh2win-0.1.0/docs/source/user_guide/index.rst
--rw-r--r--   0        0        0      243 2023-07-26 14:18:00.361274 aiida_ssh2win-0.1.0/docs/source/user_guide/tutorial.rst
--rw-r--r--   0        0        0     2864 2023-08-02 14:03:51.960676 aiida_ssh2win-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      215 2023-07-26 14:18:00.385273 aiida_ssh2win-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      117 2023-07-27 08:26:44.462148 aiida_ssh2win-0.1.0/tests/test_transport.py
--rw-r--r--   0        0        0     4462 1970-01-01 00:00:00.000000 aiida_ssh2win-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0      195 2023-07-26 14:18:00.369274 aiida_ssh2win-0.1.0a0/.github/install_aiida_github.sh
+-rw-r--r--   0        0        0     2011 2023-07-26 14:18:00.369274 aiida_ssh2win-0.1.0a0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      760 2023-07-26 14:18:00.369274 aiida_ssh2win-0.1.0a0/.github/workflows/publish-on-pypi.yml
+-rw-r--r--   0        0        0      115 2023-07-26 14:18:00.329274 aiida_ssh2win-0.1.0a0/.gitignore
+-rw-r--r--   0        0        0     1388 2023-07-27 08:25:47.746890 aiida_ssh2win-0.1.0a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      121 2023-07-26 14:18:00.333274 aiida_ssh2win-0.1.0a0/.readthedocs.yml
+-rw-r--r--   0        0        0     1072 2023-07-26 14:18:00.333274 aiida_ssh2win-0.1.0a0/LICENSE
+-rw-r--r--   0        0        0     3095 2023-07-27 08:29:34.867917 aiida_ssh2win-0.1.0a0/README.md
+-rw-r--r--   0        0        0      123 2023-07-26 14:18:00.373273 aiida_ssh2win-0.1.0a0/aiida_ssh2win/__init__.py
+-rw-r--r--   0        0        0     2131 2023-07-27 08:29:15.460171 aiida_ssh2win-0.1.0a0/aiida_ssh2win/transport.py
+-rw-r--r--   0        0        0      488 2023-07-26 14:18:00.317274 aiida_ssh2win-0.1.0a0/conftest.py
+-rw-r--r--   0        0        0        7 2023-07-26 14:18:00.337274 aiida_ssh2win-0.1.0a0/docs/.gitignore
+-rwxr-xr-x   0        0        0     1554 2023-07-26 14:18:00.337274 aiida_ssh2win-0.1.0a0/docs/Makefile
+-rwxr-xr-x   0        0        0     7573 2023-07-26 14:18:00.345274 aiida_ssh2win-0.1.0a0/docs/source/conf.py
+-rw-r--r--   0        0        0     2996 2023-07-26 14:18:00.349274 aiida_ssh2win-0.1.0a0/docs/source/developer_guide/index.rst
+-rw-r--r--   0        0        0    76300 2023-07-26 14:18:00.357274 aiida_ssh2win-0.1.0a0/docs/source/images/AiiDA_transparent_logo.png
+-rwxr-xr-x   0        0        0     1258 2023-07-26 14:18:00.345274 aiida_ssh2win-0.1.0a0/docs/source/index.rst
+-rw-r--r--   0        0        0      627 2023-07-27 08:29:15.464171 aiida_ssh2win-0.1.0a0/docs/source/user_guide/get_started.rst
+-rw-r--r--   0        0        0       94 2023-07-26 14:18:00.361274 aiida_ssh2win-0.1.0a0/docs/source/user_guide/index.rst
+-rw-r--r--   0        0        0      243 2023-07-26 14:18:00.361274 aiida_ssh2win-0.1.0a0/docs/source/user_guide/tutorial.rst
+-rw-r--r--   0        0        0     2881 2023-07-27 08:29:15.464171 aiida_ssh2win-0.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0      215 2023-07-26 14:18:00.385273 aiida_ssh2win-0.1.0a0/tests/__init__.py
+-rw-r--r--   0        0        0      117 2023-07-27 08:26:44.462148 aiida_ssh2win-0.1.0a0/tests/test_transport.py
+-rw-r--r--   0        0        0     4490 1970-01-01 00:00:00.000000 aiida_ssh2win-0.1.0a0/PKG-INFO
```

### Comparing `aiida_ssh2win-0.1.0/.github/workflows/ci.yml` & `aiida_ssh2win-0.1.0a0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida_ssh2win-0.1.0/.github/workflows/publish-on-pypi.yml` & `aiida_ssh2win-0.1.0a0/.github/workflows/publish-on-pypi.yml`

 * *Files identical despite different names*

### Comparing `aiida_ssh2win-0.1.0/.pre-commit-config.yaml` & `aiida_ssh2win-0.1.0a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida_ssh2win-0.1.0/LICENSE` & `aiida_ssh2win-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_ssh2win-0.1.0/README.md` & `aiida_ssh2win-0.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aiida_ssh2win-0.1.0/aiida_ssh2win/transport.py` & `aiida_ssh2win-0.1.0a0/aiida_ssh2win/transport.py`

 * *Files identical despite different names*

### Comparing `aiida_ssh2win-0.1.0/docs/Makefile` & `aiida_ssh2win-0.1.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida_ssh2win-0.1.0/docs/source/conf.py` & `aiida_ssh2win-0.1.0a0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aiida_ssh2win-0.1.0/docs/source/developer_guide/index.rst` & `aiida_ssh2win-0.1.0a0/docs/source/developer_guide/index.rst`

 * *Files identical despite different names*

### Comparing `aiida_ssh2win-0.1.0/docs/source/images/AiiDA_transparent_logo.png` & `aiida_ssh2win-0.1.0a0/docs/source/images/AiiDA_transparent_logo.png`

 * *Files identical despite different names*

### Comparing `aiida_ssh2win-0.1.0/docs/source/index.rst` & `aiida_ssh2win-0.1.0a0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aiida_ssh2win-0.1.0/docs/source/user_guide/get_started.rst` & `aiida_ssh2win-0.1.0a0/docs/source/user_guide/get_started.rst`

 * *Files identical despite different names*

### Comparing `aiida_ssh2win-0.1.0/pyproject.toml` & `aiida_ssh2win-0.1.0a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "Development Status :: 3 - Alpha",
     "Framework :: AiiDA"
 ]
 keywords = ["aiida", "plugin"]
 requires-python = ">=3.7"
 dependencies = [
     "aiida-core>=2.0,<3",
+    "voluptuous"
 ]
 
 [project.urls]
 Source = "https://github.com/edan-bainglass/aiida-ssh2win"
 
 [project.optional-dependencies]
 testing = [
```

### Comparing `aiida_ssh2win-0.1.0/PKG-INFO` & `aiida_ssh2win-0.1.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: aiida-ssh2win
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: A transport plugin allowing AiiDA to run calculations on Windows machines.
 Keywords: aiida,plugin
 Author-email: Edan Bainglass <edan.bainglass@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AiiDA
 Requires-Dist: aiida-core>=2.0,<3
+Requires-Dist: voluptuous
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinxcontrib-contentui ; extra == "docs"
 Requires-Dist: sphinxcontrib-details-directive ; extra == "docs"
 Requires-Dist: furo ; extra == "docs"
 Requires-Dist: markupsafe<2.1 ; extra == "docs"
 Requires-Dist: pre-commit~=2.2 ; extra == "pre-commit"
 Requires-Dist: flake8~=6.0 ; extra == "pre-commit"
```

