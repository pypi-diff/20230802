# Comparing `tmp/pollenflug-0.2.2.tar.gz` & `tmp/pollenflug-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollenflug-0.2.2.tar", max compression
+gzip compressed data, was "pollenflug-0.2.3.tar", max compression
```

## Comparing `pollenflug-0.2.2.tar` & `pollenflug-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-03 15:05:18.704873 pollenflug-0.2.2/LICENSE
--rw-r--r--   0        0        0     1279 2023-06-03 15:05:18.704873 pollenflug-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-06-03 15:05:18.708873 pollenflug-0.2.2/pollenflug/lib/__init__.py
--rw-r--r--   0        0        0     1323 2023-06-03 15:05:18.708873 pollenflug-0.2.2/pollenflug/lib/color.py
--rw-r--r--   0        0        0      682 2023-06-03 15:05:18.708873 pollenflug-0.2.2/pollenflug/lib/consts.py
--rw-r--r--   0        0        0     3948 2023-06-03 15:05:18.708873 pollenflug-0.2.2/pollenflug/lib/functions.py
--rwxr-xr-x   0        0        0     2526 2023-06-03 15:05:18.708873 pollenflug-0.2.2/pollenflug/pollenflug.py
--rw-r--r--   0        0        0     1127 2023-06-03 15:05:18.708873 pollenflug-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 pollenflug-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-02 08:04:38.452343 pollenflug-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1279 2023-08-02 08:04:38.452343 pollenflug-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 08:04:38.452343 pollenflug-0.2.3/pollenflug/lib/__init__.py
+-rw-r--r--   0        0        0     1323 2023-08-02 08:04:38.452343 pollenflug-0.2.3/pollenflug/lib/color.py
+-rw-r--r--   0        0        0      682 2023-08-02 08:04:38.452343 pollenflug-0.2.3/pollenflug/lib/consts.py
+-rw-r--r--   0        0        0     3948 2023-08-02 08:04:38.452343 pollenflug-0.2.3/pollenflug/lib/functions.py
+-rwxr-xr-x   0        0        0     2526 2023-08-02 08:04:38.452343 pollenflug-0.2.3/pollenflug/pollenflug.py
+-rw-r--r--   0        0        0     1128 2023-08-02 08:04:38.452343 pollenflug-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 pollenflug-0.2.3/PKG-INFO
```

### Comparing `pollenflug-0.2.2/LICENSE` & `pollenflug-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pollenflug-0.2.2/README.md` & `pollenflug-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pollenflug-0.2.2/pollenflug/lib/color.py` & `pollenflug-0.2.3/pollenflug/lib/color.py`

 * *Files identical despite different names*

### Comparing `pollenflug-0.2.2/pollenflug/lib/consts.py` & `pollenflug-0.2.3/pollenflug/lib/consts.py`

 * *Files identical despite different names*

### Comparing `pollenflug-0.2.2/pollenflug/lib/functions.py` & `pollenflug-0.2.3/pollenflug/lib/functions.py`

 * *Files identical despite different names*

### Comparing `pollenflug-0.2.2/pollenflug/pollenflug.py` & `pollenflug-0.2.3/pollenflug/pollenflug.py`

 * *Files identical despite different names*

### Comparing `pollenflug-0.2.2/pyproject.toml` & `pollenflug-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pollenflug"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
 	"Bader Zaidan <python@zaidan.tech>"
 ]
 description = "CLI allergy forecast tool"
 readme = "README.md"
 homepage = "https://github.com/BaderSZ/pollenflug"
 repository = "https://github.com/BaderSZ/pollenflug"
@@ -35,8 +35,8 @@
 
 [tool.bandit]
 exclude_dirs = [".venv","dist","config",]
 skips = ["B101"]
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pollenflug-0.2.2/PKG-INFO` & `pollenflug-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollenflug
-Version: 0.2.2
+Version: 0.2.3
 Summary: CLI allergy forecast tool
 Home-page: https://github.com/BaderSZ/pollenflug
 License: GGPL-3.0-or-later
 Author: Bader Zaidan
 Author-email: python@zaidan.tech
 Requires-Python: >=3.7,<4
 Classifier: Environment :: Console
```

