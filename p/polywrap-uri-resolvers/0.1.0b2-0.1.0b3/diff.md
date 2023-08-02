# Comparing `tmp/polywrap_uri_resolvers-0.1.0b2.tar.gz` & `tmp/polywrap_uri_resolvers-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_uri_resolvers-0.1.0b2.tar", max compression
+gzip compressed data, was "polywrap_uri_resolvers-0.1.0b3.tar", max compression
```

## Comparing `polywrap_uri_resolvers-0.1.0b2.tar` & `polywrap_uri_resolvers-0.1.0b3.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0       93 2023-04-10 13:52:54.342594 polywrap_uri_resolvers-0.1.0b2/README.md
--rw-r--r--   0        0        0      131 2023-06-15 11:56:46.982059 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/__init__.py
--rw-r--r--   0        0        0     1980 2023-06-15 11:56:46.982524 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/errors.py
--rw-r--r--   0        0        0        0 2023-04-10 13:52:54.326957 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/py.typed
--rw-r--r--   0        0        0      298 2023-04-10 13:52:54.328968 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/__init__.py
--rw-r--r--   0        0        0      101 2023-04-10 13:52:54.329278 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/abc/__init__.py
--rw-r--r--   0        0        0     2378 2023-06-15 11:56:46.983147 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/abc/resolver_with_history.py
--rw-r--r--   0        0        0      151 2023-06-15 11:56:46.983296 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/aggregator/__init__.py
--rw-r--r--   0        0        0     1623 2023-06-15 11:56:46.983503 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/aggregator/uri_resolver_aggregator.py
--rw-r--r--   0        0        0     2840 2023-06-15 11:56:46.983657 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/aggregator/uri_resolver_aggregator_base.py
--rw-r--r--   0        0        0      103 2023-06-15 11:56:46.983036 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/cache/__init__.py
--rw-r--r--   0        0        0     3656 2023-06-15 11:56:46.983826 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/cache/resolution_result_cache_resolver.py
--rw-r--r--   0        0        0      188 2023-04-10 13:52:54.331148 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/extensions/__init__.py
--rw-r--r--   0        0        0     2663 2023-07-29 15:58:48.636657 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/extensions/extendable_uri_resolver.py
--rw-r--r--   0        0        0     5385 2023-07-29 18:30:33.455938 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/extensions/extension_wrapper_uri_resolver.py
--rw-r--r--   0        0        0     1967 2023-06-15 11:56:46.984478 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/extensions/uri_resolver_extension_file_reader.py
--rw-r--r--   0        0        0      155 2023-04-10 13:52:54.333069 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/__init__.py
--rw-r--r--   0        0        0     1661 2023-06-15 11:56:46.984806 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/base_resolver.py
--rw-r--r--   0        0        0     2135 2023-06-15 11:56:46.985062 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/fs_resolver.py
--rw-r--r--   0        0        0     3090 2023-06-15 11:56:46.984952 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/package_to_wrapper_resolver.py
--rw-r--r--   0        0        0     1095 2023-06-15 11:56:46.985272 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/redirect_resolver.py
--rw-r--r--   0        0        0      145 2023-06-15 11:56:46.984651 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache/__init__.py
--rw-r--r--   0        0        0      824 2023-06-15 11:56:46.985191 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache/in_memory_wrapper_cache.py
--rw-r--r--   0        0        0      637 2023-06-15 11:56:46.985930 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache/wrapper_cache.py
--rw-r--r--   0        0        0     4105 2023-06-15 11:56:46.986127 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache_resolver.py
--rw-r--r--   0        0        0       88 2023-06-15 11:56:46.986375 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/package/__init__.py
--rw-r--r--   0        0        0     1925 2023-06-15 11:56:46.986539 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/package/package_resolver.py
--rw-r--r--   0        0        0      102 2023-04-10 13:52:54.335857 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/recursive/__init__.py
--rw-r--r--   0        0        0     1917 2023-07-29 07:48:46.288231 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/recursive/recursive_resolver.py
--rw-r--r--   0        0        0       90 2023-04-10 13:52:54.334522 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/redirect/__init__.py
--rw-r--r--   0        0        0     2065 2023-06-15 11:56:46.986230 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/redirect/redirect_resolver.py
--rw-r--r--   0        0        0       96 2023-04-10 13:52:54.334715 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/static/__init__.py
--rw-r--r--   0        0        0     2006 2023-06-15 11:56:46.987796 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/static/static_resolver.py
--rw-r--r--   0        0        0       88 2023-04-10 13:52:54.337533 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/wrapper/__init__.py
--rw-r--r--   0        0        0     1582 2023-06-15 11:56:46.987208 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/wrapper/wrapper_resolver.py
--rw-r--r--   0        0        0      139 2023-06-15 11:56:46.990058 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/types/__init__.py
--rw-r--r--   0        0        0       98 2023-06-15 11:56:46.987347 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/types/cache/__init__.py
--rw-r--r--   0        0        0      165 2023-06-15 11:56:46.988442 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/types/cache/resolution_result_cache/__init__.py
--rw-r--r--   0        0        0     1196 2023-06-15 11:56:46.991393 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/types/cache/resolution_result_cache/in_memory_resolution_result_cache.py
--rw-r--r--   0        0        0      923 2023-06-15 11:56:46.988720 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/types/cache/resolution_result_cache/resolution_result_cache.py
--rw-r--r--   0        0        0      307 2023-06-15 11:56:46.990354 polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/types/static_resolver_like.py
--rw-r--r--   0        0        0     1354 2023-08-02 15:57:38.305519 polywrap_uri_resolvers-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polywrap_uri_resolvers-0.1.0b2/setup.py
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 polywrap_uri_resolvers-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0       93 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/README.md
+-rw-r--r--   0        0        0      131 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/__init__.py
+-rw-r--r--   0        0        0     1980 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/errors.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/py.typed
+-rw-r--r--   0        0        0      298 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/__init__.py
+-rw-r--r--   0        0        0      101 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/abc/__init__.py
+-rw-r--r--   0        0        0     2378 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/abc/resolver_with_history.py
+-rw-r--r--   0        0        0      151 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/aggregator/__init__.py
+-rw-r--r--   0        0        0     1623 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/aggregator/uri_resolver_aggregator.py
+-rw-r--r--   0        0        0     2840 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/aggregator/uri_resolver_aggregator_base.py
+-rw-r--r--   0        0        0      103 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/cache/__init__.py
+-rw-r--r--   0        0        0     3656 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/cache/resolution_result_cache_resolver.py
+-rw-r--r--   0        0        0      188 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/extensions/__init__.py
+-rw-r--r--   0        0        0     2663 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/extensions/extendable_uri_resolver.py
+-rw-r--r--   0        0        0     5385 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/extensions/extension_wrapper_uri_resolver.py
+-rw-r--r--   0        0        0     1967 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/extensions/uri_resolver_extension_file_reader.py
+-rw-r--r--   0        0        0      155 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/__init__.py
+-rw-r--r--   0        0        0     1661 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/base_resolver.py
+-rw-r--r--   0        0        0     2135 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/fs_resolver.py
+-rw-r--r--   0        0        0     3090 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/package_to_wrapper_resolver.py
+-rw-r--r--   0        0        0     1095 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/redirect_resolver.py
+-rw-r--r--   0        0        0      145 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache/__init__.py
+-rw-r--r--   0        0        0      824 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache/in_memory_wrapper_cache.py
+-rw-r--r--   0        0        0      637 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache/wrapper_cache.py
+-rw-r--r--   0        0        0     4105 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache_resolver.py
+-rw-r--r--   0        0        0       88 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/package/__init__.py
+-rw-r--r--   0        0        0     1925 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/package/package_resolver.py
+-rw-r--r--   0        0        0      102 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/recursive/__init__.py
+-rw-r--r--   0        0        0     1917 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/recursive/recursive_resolver.py
+-rw-r--r--   0        0        0       90 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/redirect/__init__.py
+-rw-r--r--   0        0        0     2065 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/redirect/redirect_resolver.py
+-rw-r--r--   0        0        0       96 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/static/__init__.py
+-rw-r--r--   0        0        0     2006 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/static/static_resolver.py
+-rw-r--r--   0        0        0       88 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/wrapper/__init__.py
+-rw-r--r--   0        0        0     1582 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/wrapper/wrapper_resolver.py
+-rw-r--r--   0        0        0      139 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/types/__init__.py
+-rw-r--r--   0        0        0       98 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/types/cache/__init__.py
+-rw-r--r--   0        0        0      165 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/types/cache/resolution_result_cache/__init__.py
+-rw-r--r--   0        0        0     1196 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/types/cache/resolution_result_cache/in_memory_resolution_result_cache.py
+-rw-r--r--   0        0        0      923 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/types/cache/resolution_result_cache/resolution_result_cache.py
+-rw-r--r--   0        0        0      307 2023-08-02 16:06:36.163338 polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/types/static_resolver_like.py
+-rw-r--r--   0        0        0     1354 2023-08-02 16:17:54.991842 polywrap_uri_resolvers-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 polywrap_uri_resolvers-0.1.0b3/PKG-INFO
```

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/errors.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/errors.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/abc/resolver_with_history.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/abc/resolver_with_history.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/aggregator/uri_resolver_aggregator.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/aggregator/uri_resolver_aggregator.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/aggregator/uri_resolver_aggregator_base.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/aggregator/uri_resolver_aggregator_base.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/cache/resolution_result_cache_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/cache/resolution_result_cache_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/extensions/extendable_uri_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/extensions/extendable_uri_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/extensions/extension_wrapper_uri_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/extensions/extension_wrapper_uri_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/extensions/uri_resolver_extension_file_reader.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/extensions/uri_resolver_extension_file_reader.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/base_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/base_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/fs_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/fs_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/package_to_wrapper_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/package_to_wrapper_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/redirect_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/redirect_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache/in_memory_wrapper_cache.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache/in_memory_wrapper_cache.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache/wrapper_cache.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache/wrapper_cache.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/legacy/wrapper_cache_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/package/package_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/package/package_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/recursive/recursive_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/recursive/recursive_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/redirect/redirect_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/redirect/redirect_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/static/static_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/static/static_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/resolvers/wrapper/wrapper_resolver.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/resolvers/wrapper/wrapper_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/types/cache/resolution_result_cache/in_memory_resolution_result_cache.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/types/cache/resolution_result_cache/in_memory_resolution_result_cache.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/polywrap_uri_resolvers/types/cache/resolution_result_cache/resolution_result_cache.py` & `polywrap_uri_resolvers-0.1.0b3/polywrap_uri_resolvers/types/cache/resolution_result_cache/resolution_result_cache.py`

 * *Files identical despite different names*

### Comparing `polywrap_uri_resolvers-0.1.0b2/pyproject.toml` & `polywrap_uri_resolvers-0.1.0b3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-uri-resolvers"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = ""
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-wasm = "^0.1.0b2"
-polywrap-core = "^0.1.0b2"
+polywrap-wasm = "^0.1.0b3"
+polywrap-core = "^0.1.0b3"
 
 [tool.poetry.group.dev.dependencies]
 pycln = "^2.1.3"
 polywrap-client = {path = "../polywrap-client", develop = true}
 polywrap-plugin = {path = "../polywrap-plugin", develop = true}
 polywrap-test-cases = {path = "../polywrap-test-cases", develop = true}
 pytest = "^7.1.2"
```

### Comparing `polywrap_uri_resolvers-0.1.0b2/PKG-INFO` & `polywrap_uri_resolvers-0.1.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: polywrap-uri-resolvers
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: 
 Author: Cesar
 Author-email: cesar@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-core (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-wasm (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-core (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-wasm (>=0.1.0b3,<0.2.0)
 Description-Content-Type: text/markdown
 
 # polywrap-uri-resolvers
 
 URI resolvers to customize URI resolution in the Polywrap Client.
```

