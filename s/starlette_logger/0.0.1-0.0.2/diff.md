# Comparing `tmp/starlette_logger-0.0.1.tar.gz` & `tmp/starlette_logger-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_logger-0.0.1.tar", last modified: Wed Aug  2 09:42:11 2023, max compression
+gzip compressed data, was "starlette_logger-0.0.2.tar", last modified: Wed Aug  2 11:35:17 2023, max compression
```

## Comparing `starlette_logger-0.0.1.tar` & `starlette_logger-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3078 2023-08-02 06:03:28.269331 starlette_logger-0.0.1/.gitignore
--rw-r--r--   0        0        0      171 2023-08-02 09:20:34.865349 starlette_logger-0.0.1/Pipfile
--rw-r--r--   0        0        0     2090 2023-08-02 09:20:35.615830 starlette_logger-0.0.1/Pipfile.lock
--rw-r--r--   0        0        0       75 2023-08-02 06:03:28.269458 starlette_logger-0.0.1/README.md
--rw-r--r--   0        0        0      488 2023-08-02 09:23:16.978523 starlette_logger-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      293 2023-08-02 09:33:55.337819 starlette_logger-0.0.1/starlette_logger/__init__.py
--rw-r--r--   0        0        0     3134 2023-08-02 08:28:11.427297 starlette_logger-0.0.1/starlette_logger/middleware.py
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 starlette_logger-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-08-02 06:03:28.269331 starlette_logger-0.0.2/.gitignore
+-rw-r--r--   0        0        0      171 2023-08-02 09:20:34.865349 starlette_logger-0.0.2/Pipfile
+-rw-r--r--   0        0        0     2090 2023-08-02 09:20:35.615830 starlette_logger-0.0.2/Pipfile.lock
+-rw-r--r--   0        0        0       75 2023-08-02 06:03:28.269458 starlette_logger-0.0.2/README.md
+-rw-r--r--   0        0        0      488 2023-08-02 11:31:48.594446 starlette_logger-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-08-02 11:34:41.374421 starlette_logger-0.0.2/starlette_logger/__init__.py
+-rw-r--r--   0        0        0     3134 2023-08-02 08:28:11.427297 starlette_logger-0.0.2/starlette_logger/middleware.py
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 starlette_logger-0.0.2/PKG-INFO
```

### Comparing `starlette_logger-0.0.1/.gitignore` & `starlette_logger-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `starlette_logger-0.0.1/Pipfile.lock` & `starlette_logger-0.0.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `starlette_logger-0.0.1/starlette_logger/middleware.py` & `starlette_logger-0.0.2/starlette_logger/middleware.py`

 * *Files identical despite different names*

