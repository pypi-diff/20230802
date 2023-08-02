# Comparing `tmp/polywrap_core-0.1.0b1.tar.gz` & `tmp/polywrap_core-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_core-0.1.0b1.tar", max compression
+gzip compressed data, was "polywrap_core-0.1.0b2.tar", max compression
```

## Comparing `polywrap_core-0.1.0b1.tar` & `polywrap_core-0.1.0b2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      132 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/py.typed
--rw-r--r--   0        0        0      589 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/__init__.py
--rw-r--r--   0        0        0      147 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/clean_resolution_step.py
--rw-r--r--   0        0        0     2292 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/client.py
--rw-r--r--   0        0        0      869 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/config.py
--rw-r--r--   0        0        0     3980 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/errors.py
--rw-r--r--   0        0        0      560 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/file_reader.py
--rw-r--r--   0        0        0     1847 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/invocable.py
--rw-r--r--   0        0        0      859 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/invoke_options.py
--rw-r--r--   0        0        0     1716 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/invoker.py
--rw-r--r--   0        0        0      411 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/invoker_client.py
--rw-r--r--   0        0        0     5822 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri.py
--rw-r--r--   0        0        0      553 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_package.py
--rw-r--r--   0        0        0      837 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_package_wrapper.py
--rw-r--r--   0        0        0     3668 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_resolution_context.py
--rw-r--r--   0        0        0      822 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_resolution_step.py
--rw-r--r--   0        0        0      989 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_resolver.py
--rw-r--r--   0        0        0      752 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_resolver_handler.py
--rw-r--r--   0        0        0      458 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/uri_wrapper.py
--rw-r--r--   0        0        0      936 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/wrap_package.py
--rw-r--r--   0        0        0      866 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/types/wrapper.py
--rw-r--r--   0        0        0      204 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/utils/__init__.py
--rw-r--r--   0        0        0     2343 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/utils/build_clean_uri_history.py
--rw-r--r--   0        0        0      712 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/utils/get_env_from_resolution_path.py
--rw-r--r--   0        0        0     1980 2023-08-01 17:46:03.391535 polywrap_core-0.1.0b1/polywrap_core/utils/get_implementations.py
--rw-r--r--   0        0        0     1059 2023-08-01 17:50:15.331996 polywrap_core-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 polywrap_core-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0      132 2023-05-23 15:20:42.240042 polywrap_core-0.1.0b2/polywrap_core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 13:52:54.296012 polywrap_core-0.1.0b2/polywrap_core/py.typed
+-rw-r--r--   0        0        0      589 2023-06-15 11:56:46.962185 polywrap_core-0.1.0b2/polywrap_core/types/__init__.py
+-rw-r--r--   0        0        0      147 2023-06-15 11:56:46.962431 polywrap_core-0.1.0b2/polywrap_core/types/clean_resolution_step.py
+-rw-r--r--   0        0        0     2292 2023-06-15 11:56:46.961280 polywrap_core-0.1.0b2/polywrap_core/types/client.py
+-rw-r--r--   0        0        0      869 2023-06-15 11:56:46.962445 polywrap_core-0.1.0b2/polywrap_core/types/config.py
+-rw-r--r--   0        0        0     3980 2023-06-15 11:56:46.961912 polywrap_core-0.1.0b2/polywrap_core/types/errors.py
+-rw-r--r--   0        0        0      560 2023-06-15 11:56:46.962613 polywrap_core-0.1.0b2/polywrap_core/types/file_reader.py
+-rw-r--r--   0        0        0     1847 2023-06-15 11:56:46.963012 polywrap_core-0.1.0b2/polywrap_core/types/invocable.py
+-rw-r--r--   0        0        0      859 2023-06-15 11:56:46.963218 polywrap_core-0.1.0b2/polywrap_core/types/invoke_options.py
+-rw-r--r--   0        0        0     1716 2023-06-15 11:56:46.972006 polywrap_core-0.1.0b2/polywrap_core/types/invoker.py
+-rw-r--r--   0        0        0      411 2023-06-15 11:56:46.963881 polywrap_core-0.1.0b2/polywrap_core/types/invoker_client.py
+-rw-r--r--   0        0        0     5822 2023-06-15 11:56:46.964069 polywrap_core-0.1.0b2/polywrap_core/types/uri.py
+-rw-r--r--   0        0        0      553 2023-06-15 11:56:46.963416 polywrap_core-0.1.0b2/polywrap_core/types/uri_package.py
+-rw-r--r--   0        0        0      837 2023-06-15 11:56:46.963642 polywrap_core-0.1.0b2/polywrap_core/types/uri_package_wrapper.py
+-rw-r--r--   0        0        0     3668 2023-06-15 11:56:46.963738 polywrap_core-0.1.0b2/polywrap_core/types/uri_resolution_context.py
+-rw-r--r--   0        0        0      822 2023-06-15 11:56:46.963811 polywrap_core-0.1.0b2/polywrap_core/types/uri_resolution_step.py
+-rw-r--r--   0        0        0      989 2023-06-15 11:56:46.963953 polywrap_core-0.1.0b2/polywrap_core/types/uri_resolver.py
+-rw-r--r--   0        0        0      752 2023-06-15 11:56:46.964860 polywrap_core-0.1.0b2/polywrap_core/types/uri_resolver_handler.py
+-rw-r--r--   0        0        0      458 2023-06-15 11:56:46.964214 polywrap_core-0.1.0b2/polywrap_core/types/uri_wrapper.py
+-rw-r--r--   0        0        0      936 2023-06-15 11:56:46.964607 polywrap_core-0.1.0b2/polywrap_core/types/wrap_package.py
+-rw-r--r--   0        0        0      866 2023-06-15 11:56:46.965486 polywrap_core-0.1.0b2/polywrap_core/types/wrapper.py
+-rw-r--r--   0        0        0      204 2023-06-15 11:56:46.965606 polywrap_core-0.1.0b2/polywrap_core/utils/__init__.py
+-rw-r--r--   0        0        0     2343 2023-07-29 15:12:42.183287 polywrap_core-0.1.0b2/polywrap_core/utils/build_clean_uri_history.py
+-rw-r--r--   0        0        0      712 2023-06-15 11:56:46.964726 polywrap_core-0.1.0b2/polywrap_core/utils/get_env_from_resolution_path.py
+-rw-r--r--   0        0        0     1980 2023-06-15 11:56:46.968067 polywrap_core-0.1.0b2/polywrap_core/utils/get_implementations.py
+-rw-r--r--   0        0        0     1059 2023-08-02 15:38:25.477608 polywrap_core-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 polywrap_core-0.1.0b2/setup.py
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 polywrap_core-0.1.0b2/PKG-INFO
```

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/__init__.py` & `polywrap_core-0.1.0b2/polywrap_core/types/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/client.py` & `polywrap_core-0.1.0b2/polywrap_core/types/client.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/config.py` & `polywrap_core-0.1.0b2/polywrap_core/types/config.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/errors.py` & `polywrap_core-0.1.0b2/polywrap_core/types/errors.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/file_reader.py` & `polywrap_core-0.1.0b2/polywrap_core/types/file_reader.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/invocable.py` & `polywrap_core-0.1.0b2/polywrap_core/types/invocable.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/invoke_options.py` & `polywrap_core-0.1.0b2/polywrap_core/types/invoke_options.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/invoker.py` & `polywrap_core-0.1.0b2/polywrap_core/types/invoker.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/uri.py` & `polywrap_core-0.1.0b2/polywrap_core/types/uri.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/uri_package.py` & `polywrap_core-0.1.0b2/polywrap_core/types/uri_package.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/uri_package_wrapper.py` & `polywrap_core-0.1.0b2/polywrap_core/types/uri_package_wrapper.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/uri_resolution_context.py` & `polywrap_core-0.1.0b2/polywrap_core/types/uri_resolution_context.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/uri_resolution_step.py` & `polywrap_core-0.1.0b2/polywrap_core/types/uri_resolution_step.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/uri_resolver.py` & `polywrap_core-0.1.0b2/polywrap_core/types/uri_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/uri_resolver_handler.py` & `polywrap_core-0.1.0b2/polywrap_core/types/uri_resolver_handler.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/wrap_package.py` & `polywrap_core-0.1.0b2/polywrap_core/types/wrap_package.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/types/wrapper.py` & `polywrap_core-0.1.0b2/polywrap_core/types/wrapper.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/utils/build_clean_uri_history.py` & `polywrap_core-0.1.0b2/polywrap_core/utils/build_clean_uri_history.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/utils/get_env_from_resolution_path.py` & `polywrap_core-0.1.0b2/polywrap_core/utils/get_env_from_resolution_path.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/polywrap_core/utils/get_implementations.py` & `polywrap_core-0.1.0b2/polywrap_core/utils/get_implementations.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0b1/pyproject.toml` & `polywrap_core-0.1.0b2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-core"
-version = "0.1.0b1"
+version = "0.1.0b2"
 description = ""
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-msgpack = "^0.1.0b1"
-polywrap-manifest = "^0.1.0b1"
+polywrap-msgpack = "^0.1.0b2"
+polywrap-manifest = "^0.1.0b2"
 
 [tool.poetry.group.dev.dependencies]
 pycln = "^2.1.3"
 pytest = "^7.1.2"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
```

