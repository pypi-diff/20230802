# Comparing `tmp/polywrap_client_config_builder-0.1.0a35.tar.gz` & `tmp/polywrap_client_config_builder-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_client_config_builder-0.1.0a35.tar", max compression
+gzip compressed data, was "polywrap_client_config_builder-0.1.0b2.tar", max compression
```

## Comparing `polywrap_client_config_builder-0.1.0a35.tar` & `polywrap_client_config_builder-0.1.0b2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1410 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/README.md
--rw-r--r--   0        0        0      138 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/__init__.py
--rw-r--r--   0        0        0      309 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/__init__.py
--rw-r--r--   0        0        0      995 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/base_configure.py
--rw-r--r--   0        0        0     2702 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/env_configure.py
--rw-r--r--   0        0        0     2120 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/interface_configure.py
--rw-r--r--   0        0        0     1628 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/package_configure.py
--rw-r--r--   0        0        0     1645 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/redirect_configure.py
--rw-r--r--   0        0        0      965 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/resolver_configure.py
--rw-r--r--   0        0        0     1607 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/wrapper_configure.py
--rw-r--r--   0        0        0     4240 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/polywrap_client_config_builder.py
--rw-r--r--   0        0        0        0 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/py.typed
--rw-r--r--   0        0        0      164 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/types/__init__.py
--rw-r--r--   0        0        0      613 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/types/build_options.py
--rw-r--r--   0        0        0     1154 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/types/builder_config.py
--rw-r--r--   0        0        0     6256 2023-06-28 13:05:20.144193 polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/types/client_config_builder.py
--rw-r--r--   0        0        0     1108 2023-06-28 13:14:43.177375 polywrap_client_config_builder-0.1.0a35/pyproject.toml
--rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 polywrap_client_config_builder-0.1.0a35/PKG-INFO
+-rw-r--r--   0        0        0     1410 2023-06-19 11:17:54.180341 polywrap_client_config_builder-0.1.0b2/README.md
+-rw-r--r--   0        0        0      138 2023-06-15 11:56:46.943179 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/__init__.py
+-rw-r--r--   0        0        0      309 2023-04-10 13:52:54.284350 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/__init__.py
+-rw-r--r--   0        0        0      995 2023-06-15 11:56:46.943257 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/base_configure.py
+-rw-r--r--   0        0        0     2702 2023-06-15 11:56:46.944351 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/env_configure.py
+-rw-r--r--   0        0        0     2120 2023-06-15 11:56:46.943464 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/interface_configure.py
+-rw-r--r--   0        0        0     1628 2023-06-15 11:56:46.944103 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/package_configure.py
+-rw-r--r--   0        0        0     1645 2023-06-15 11:56:46.944236 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/redirect_configure.py
+-rw-r--r--   0        0        0      965 2023-06-15 11:56:46.943869 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/resolver_configure.py
+-rw-r--r--   0        0        0     1607 2023-06-15 11:56:46.944424 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/wrapper_configure.py
+-rw-r--r--   0        0        0     4240 2023-06-15 11:56:46.944542 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/polywrap_client_config_builder.py
+-rw-r--r--   0        0        0        0 2023-04-10 13:52:54.287664 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/py.typed
+-rw-r--r--   0        0        0      164 2023-04-10 13:52:54.289047 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/types/__init__.py
+-rw-r--r--   0        0        0      613 2023-06-15 11:56:46.944680 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/types/build_options.py
+-rw-r--r--   0        0        0     1154 2023-06-15 11:56:46.944876 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/types/builder_config.py
+-rw-r--r--   0        0        0     6256 2023-06-15 11:56:46.945602 polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/types/client_config_builder.py
+-rw-r--r--   0        0        0     1056 2023-08-02 15:58:45.091561 polywrap_client_config_builder-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 polywrap_client_config_builder-0.1.0b2/setup.py
+-rw-r--r--   0        0        0     1868 1970-01-01 00:00:00.000000 polywrap_client_config_builder-0.1.0b2/PKG-INFO
```

### Comparing `polywrap_client_config_builder-0.1.0a35/README.md` & `polywrap_client_config_builder-0.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/base_configure.py` & `polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/base_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/env_configure.py` & `polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/env_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/interface_configure.py` & `polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/interface_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/package_configure.py` & `polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/package_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/redirect_configure.py` & `polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/redirect_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/resolver_configure.py` & `polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/resolver_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/configures/wrapper_configure.py` & `polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/configures/wrapper_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/polywrap_client_config_builder.py` & `polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/polywrap_client_config_builder.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/types/build_options.py` & `polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/types/build_options.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/types/builder_config.py` & `polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/types/builder_config.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a35/polywrap_client_config_builder/types/client_config_builder.py` & `polywrap_client_config_builder-0.1.0b2/polywrap_client_config_builder/types/client_config_builder.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a35/pyproject.toml` & `polywrap_client_config_builder-0.1.0b2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-client-config-builder"
-version = "0.1.0a35"
+version = "0.1.0b2"
 description = ""
 authors = ["Media <media@polywrap.io>", "Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-uri-resolvers = "^0.1.0a35"
-polywrap-core = "^0.1.0a35"
+polywrap-uri-resolvers = "^0.1.0b2"
+polywrap-core = "^0.1.0b2"
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
-pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 isort = "^5.10.1"
 pyright = "^1.1.275"
@@ -34,15 +33,14 @@
 [tool.black]
 target-version = ["py310"]
 
 [tool.pyright]
 # default
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
 testpaths = [
     "tests"
 ]
 
 [tool.pylint]
 disable = [
     "unnecessary-ellipsis",
```

### Comparing `polywrap_client_config_builder-0.1.0a35/PKG-INFO` & `polywrap_client_config_builder-0.1.0b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: polywrap-client-config-builder
-Version: 0.1.0a35
+Version: 0.1.0b2
 Summary: 
 Author: Media
 Author-email: media@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-core (>=0.1.0a35,<0.2.0)
-Requires-Dist: polywrap-uri-resolvers (>=0.1.0a35,<0.2.0)
+Requires-Dist: polywrap-core (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-uri-resolvers (>=0.1.0b2,<0.2.0)
 Description-Content-Type: text/markdown
 
 # polywrap-client-config-builder
 
 A utility class for building the PolywrapClient config. 
 
 Supports building configs using method chaining or imperatively.
```

