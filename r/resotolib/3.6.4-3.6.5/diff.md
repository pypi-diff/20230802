# Comparing `tmp/resotolib-3.6.4.tar.gz` & `tmp/resotolib-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotolib-3.6.4.tar", last modified: Mon Jul 24 18:36:20 2023, max compression
+gzip compressed data, was "resotolib-3.6.5.tar", last modified: Wed Aug  2 19:23:55 2023, max compression
```

## Comparing `resotolib-3.6.4.tar` & `resotolib-3.6.5.tar`

### file list

```diff
@@ -1,89 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.822485 resotolib-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 18:30:36.000000 resotolib-3.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-24 18:36:20.822485 resotolib-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-24 18:30:36.000000 resotolib-3.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-24 18:30:36.000000 resotolib-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.806484 resotolib-3.6.4/resotolib/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.806484 resotolib-3.6.4/resotolib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/asynchronous/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.806484 resotolib-3.6.4/resotolib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/asynchronous/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    40301 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.806484 resotolib-3.6.4/resotolib/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/durations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.806484 resotolib-3.6.4/resotolib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)    27774 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.810484 resotolib-3.6.4/resotolib/log/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    23779 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.810484 resotolib-3.6.4/resotolib/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.814484 resotolib-3.6.4/resotolib/web/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-24 18:30:36.000000 resotolib-3.6.4/resotolib/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.806484 resotolib-3.6.4/resotolib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-24 18:36:20.000000 resotolib-3.6.4/resotolib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-24 18:36:20.000000 resotolib-3.6.4/resotolib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:36:20.000000 resotolib-3.6.4/resotolib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:31:45.000000 resotolib-3.6.4/resotolib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-24 18:36:20.000000 resotolib-3.6.4/resotolib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 18:36:20.000000 resotolib-3.6.4/resotolib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 18:36:20.822485 resotolib-3.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:36:20.822485 resotolib-3.6.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    16198 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-24 18:30:36.000000 resotolib-3.6.4/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:55.406823 resotolib-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 19:17:20.000000 resotolib-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-02 19:23:55.406823 resotolib-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-02 19:17:20.000000 resotolib-3.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-02 19:17:20.000000 resotolib-3.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:55.390822 resotolib-3.6.5/resotolib/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:55.394822 resotolib-3.6.5/resotolib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/asynchronous/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:55.394822 resotolib-3.6.5/resotolib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40301 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:55.398822 resotolib-3.6.5/resotolib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:55.398822 resotolib-3.6.5/resotolib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    28059 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:55.398822 resotolib-3.6.5/resotolib/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23779 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:55.398822 resotolib-3.6.5/resotolib/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:55.406823 resotolib-3.6.5/resotolib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-08-02 19:17:20.000000 resotolib-3.6.5/resotolib/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:55.394822 resotolib-3.6.5/resotolib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-02 19:23:55.000000 resotolib-3.6.5/resotolib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-02 19:23:55.000000 resotolib-3.6.5/resotolib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:23:55.000000 resotolib-3.6.5/resotolib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:18:39.000000 resotolib-3.6.5/resotolib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-02 19:23:55.000000 resotolib-3.6.5/resotolib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 19:23:55.000000 resotolib-3.6.5/resotolib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-02 19:23:55.406823 resotolib-3.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:23:55.406823 resotolib-3.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16198 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-08-02 19:17:20.000000 resotolib-3.6.5/test/test_x509.py
```

### Comparing `resotolib-3.6.4/PKG-INFO` & `resotolib-3.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto common library.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotolib
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotolib-3.6.4/README.md` & `resotolib-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/pyproject.toml` & `resotolib-3.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotolib"
-version = "3.6.4"
+version = "3.6.5"
 authors = [{name="Some Engineering Inc."}]
 description = "Resoto common library."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
```

### Comparing `resotolib-3.6.4/resotolib/args.py` & `resotolib-3.6.5/resotolib/args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/asynchronous/utils.py` & `resotolib-3.6.5/resotolib/asynchronous/utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/asynchronous/web/runner.py` & `resotolib-3.6.5/resotolib/asynchronous/web/runner.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/asynchronous/web/ws_handler.py` & `resotolib-3.6.5/resotolib/asynchronous/web/ws_handler.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/baseplugin.py` & `resotolib-3.6.5/resotolib/baseplugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/baseresources.py` & `resotolib-3.6.5/resotolib/baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/config.py` & `resotolib-3.6.5/resotolib/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/core/__init__.py` & `resotolib-3.6.5/resotolib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/core/actions.py` & `resotolib-3.6.5/resotolib/core/actions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/core/ca.py` & `resotolib-3.6.5/resotolib/core/ca.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/core/config.py` & `resotolib-3.6.5/resotolib/core/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/core/custom_command.py` & `resotolib-3.6.5/resotolib/core/custom_command.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/core/events.py` & `resotolib-3.6.5/resotolib/core/events.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/core/model_check.py` & `resotolib-3.6.5/resotolib/core/model_check.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/core/model_export.py` & `resotolib-3.6.5/resotolib/core/model_export.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/core/progress.py` & `resotolib-3.6.5/resotolib/core/progress.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/core/search.py` & `resotolib-3.6.5/resotolib/core/search.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/core/tasks.py` & `resotolib-3.6.5/resotolib/core/tasks.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/durations.py` & `resotolib-3.6.5/resotolib/durations.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/event.py` & `resotolib-3.6.5/resotolib/event.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/graph/__init__.py` & `resotolib-3.6.5/resotolib/graph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     def merge(self, graph: Graph, skip_deferred_edges: bool = False) -> None:
         """Merge another graph into ourselves
 
         If the other graph has a graph.root an edge will be created between
         it and our own graph root.
         """
         if isinstance(self.root, BaseResource) and isinstance(getattr(graph, "root", None), BaseResource):
-            log.debug(f"Merging graph of {graph.root.rtdname} into graph of {self.root.rtdname}")  # type: ignore
+            log.debug(f"Merging graph of {graph.root.kdname} into graph of {self.root.kdname}")  # type: ignore
             self.add_edge(self.root, graph.root)  # type: ignore
         else:
             log.warning("Merging graphs with no valid roots")
 
         try:
             self._log_edge_creation = False
             self.update(edges=graph.edges, nodes=graph.nodes)
@@ -183,29 +183,26 @@
             key = EdgeKey(src=src, dst=dst, edge_type=edge_type)
 
         if self.has_edge(src, dst, key=key):
             log.debug(f"Edge from {src} to {dst} already exists in graph")
             return None
         return_key = super().add_edge(src, dst, key=key, **attr)
         if self._log_edge_creation and isinstance(src, BaseResource) and isinstance(dst, BaseResource):
-            log.debug(f"Added edge from {src.rtdname} to {dst.rtdname} (type: {edge_type.value})")
+            log.debug(f"Added edge from {src.kdname} to {dst.kdname} (type: {edge_type.value})")
             try:
                 src.successor_added(dst, self)
             except Exception:
                 log.exception(
-                    (f"Unhandled exception while telling {src.rtdname}" f" that {dst.rtdname} was added as a successor")
+                    (f"Unhandled exception while telling {src.kdname}" f" that {dst.kdname} was added as a successor")
                 )
             try:
                 dst.predecessor_added(src, self)
             except Exception:
                 log.exception(
-                    (
-                        f"Unhandled exception while telling {dst.rtdname}"
-                        f" that {src.rtdname} was added as a predecessor"
-                    )
+                    (f"Unhandled exception while telling {dst.kdname}" f" that {src.kdname} was added as a predecessor")
                 )
         return return_key  # type: ignore
 
     def add_deferred_edge(self, src: NodeSelector, dst: NodeSelector, edge_type: EdgeType = EdgeType.default) -> None:
         self.deferred_edges.append((src, dst, edge_type))
 
     def remove_node(self, node: BaseResource) -> None:
@@ -409,46 +406,56 @@
 
 
 @lru_cache(maxsize=4096)  # Only resolve types once per type
 def resolve_type(clazz: Type[Any]) -> None:
     resolve_types(clazz)  # type: ignore
 
 
-def validate_dataclass(node: BaseResource) -> None:
+def validate_dataclass(node: BaseResource) -> bool:
     resolve_type(type(node))  # make sure all type annotations are resolved
     for field in fields(type(node)):
         value = getattr(node, field.name)
         try:
             check_type(value, field.type)
-        except TypeError:
-            log.exception(
-                f"In {node.rtdname} expected {field.name}"
+        except Exception:
+            log.error(
+                f"In {node.kdname} expected {field.name}"
                 f" type {field.type} ({type(field.type)})"
                 f" for value {value} ({type(value)})"
             )
+            return False
+    return True
 
 
 def validate_graph_dataclasses_and_nodes(graph: Graph) -> None:
     log.debug("Validating attribute types of all graph dataclasses")
     node_chksums = {}
+    invalid_nodes = []
     for node in graph.nodes:
         if isinstance(node, BaseResource):
-            validate_dataclass(node)
+            try:
+                if not validate_dataclass(node):
+                    invalid_nodes.append(node)
+            except Exception:
+                log.error(f"Failed to validate dataclass {node.kdname}")
             if node.chksum not in node_chksums:
                 node_chksums[node.chksum] = node
             else:
                 log.error(
-                    f"Duplicate checksum {node.chksum} for node {node.rtdname} in graph!\n"
+                    f"Duplicate checksum {node.chksum} for node {node.kdname} in graph!\n"
                     f"Previous node: {get_resource_attributes(node_chksums[node.chksum])}\n"
-                    f"Previous predecessor nodes: {[n.rtdname for n in node_chksums[node.chksum].predecessors()]}\n"
-                    f"Previous successor nodes: {[n.rtdname for n in node_chksums[node.chksum].successors()]}\n"
+                    f"Previous predecessor nodes: {[n.kdname for n in node_chksums[node.chksum].predecessors()]}\n"
+                    f"Previous successor nodes: {[n.kdname for n in node_chksums[node.chksum].successors()]}\n"
                     f"New node: {get_resource_attributes(node)}\n"
-                    f"New predecessor nodes: {[n.rtdname for n in node.predecessors()]}\n"
-                    f"New successor nodes: {[n.rtdname for n in node.successors()]}\n"
+                    f"New predecessor nodes: {[n.kdname for n in node.predecessors()]}\n"
+                    f"New successor nodes: {[n.kdname for n in node.successors()]}\n"
                 )
+    for node in invalid_nodes:
+        log.error(f"Removing invalid node {node.kdname} from graph")
+        graph.remove_node(node)
 
 
 def update_graph_ref(graph: Graph) -> None:
     for node in graph.nodes:
         if isinstance(node, BaseResource):
             node._graph = graph
 
@@ -588,21 +595,21 @@
 
     def export_graph(self) -> None:
         with self.export_lock:
             start_time = time()
             for node in self.graph.nodes:
                 node_dict = node_to_dict(node)
                 if isinstance(node, self.graph_merge_kind):
-                    log.debug(f"Replacing sub graph below {node.rtdname}")
+                    log.debug(f"Replacing sub graph below {node.kdname}")
                     if "metadata" not in node_dict or not isinstance(node_dict["metadata"], dict):
                         node_dict["metadata"] = {}
                     node_dict["metadata"]["replace"] = True
                     self.found_replace_node = True
                 if isinstance(node, BaseAccount):
-                    log.debug(f"Setting export time on {node.rtdname}")
+                    log.debug(f"Setting export time on {node.kdname}")
                     if "metadata" not in node_dict or not isinstance(node_dict["metadata"], dict):
                         node_dict["metadata"] = {}
                     node_dict["metadata"]["exported_at"] = utc_str()
                 node_json = to_json_str(node_dict) + "\n"
                 self.tempfile.write(node_json.encode())
                 self.total_lines += 1
             elapsed_nodes = time() - start_time
```

### Comparing `resotolib-3.6.4/resotolib/graph/graph_extensions.py` & `resotolib-3.6.5/resotolib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/json.py` & `resotolib-3.6.5/resotolib/json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/json_bender.py` & `resotolib-3.6.5/resotolib/json_bender.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/jwt.py` & `resotolib-3.6.5/resotolib/jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/lock.py` & `resotolib-3.6.5/resotolib/lock.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/logger.py` & `resotolib-3.6.5/resotolib/logger.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/parse_util.py` & `resotolib-3.6.5/resotolib/parse_util.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/proc.py` & `resotolib-3.6.5/resotolib/proc.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/threading.py` & `resotolib-3.6.5/resotolib/threading.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/tree.py` & `resotolib-3.6.5/resotolib/tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/utils.py` & `resotolib-3.6.5/resotolib/utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/web/__init__.py` & `resotolib-3.6.5/resotolib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/web/metrics.py` & `resotolib-3.6.5/resotolib/web/metrics.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/web/static/android-chrome-192x192.png` & `resotolib-3.6.5/resotolib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/web/static/android-chrome-512x512.png` & `resotolib-3.6.5/resotolib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/web/static/apple-touch-icon.png` & `resotolib-3.6.5/resotolib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/web/static/favicon-16x16.png` & `resotolib-3.6.5/resotolib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/web/static/favicon-32x32.png` & `resotolib-3.6.5/resotolib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/web/static/index.html` & `resotolib-3.6.5/resotolib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/web/static/mstile-150x150.png` & `resotolib-3.6.5/resotolib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/web/static/picnic.min.css` & `resotolib-3.6.5/resotolib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib/x509.py` & `resotolib-3.6.5/resotolib/x509.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/resotolib.egg-info/PKG-INFO` & `resotolib-3.6.5/resotolib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.6.4
+Version: 3.6.5
 Summary: Resoto common library.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotolib
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotolib-3.6.4/resotolib.egg-info/SOURCES.txt` & `resotolib-3.6.5/resotolib.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 resotolib.egg-info/dependency_links.txt
 resotolib.egg-info/not-zip-safe
 resotolib.egg-info/requires.txt
 resotolib.egg-info/top_level.txt
 resotolib/asynchronous/__init__.py
 resotolib/asynchronous/utils.py
 resotolib/asynchronous/web/__init__.py
-resotolib/asynchronous/web/auth.py
 resotolib/asynchronous/web/runner.py
 resotolib/asynchronous/web/ws_handler.py
 resotolib/core/__init__.py
 resotolib/core/actions.py
 resotolib/core/ca.py
 resotolib/core/config.py
 resotolib/core/custom_command.py
```

### Comparing `resotolib-3.6.4/test/test_args.py` & `resotolib-3.6.5/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/test/test_baseresources.py` & `resotolib-3.6.5/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/test/test_config.py` & `resotolib-3.6.5/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/test/test_graph.py` & `resotolib-3.6.5/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/test/test_graph_extensions.py` & `resotolib-3.6.5/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/test/test_json.py` & `resotolib-3.6.5/test/test_json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/test/test_jwt.py` & `resotolib-3.6.5/test/test_jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/test/test_plugin.py` & `resotolib-3.6.5/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/test/test_tree.py` & `resotolib-3.6.5/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/test/test_utils.py` & `resotolib-3.6.5/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/test/test_web.py` & `resotolib-3.6.5/test/test_web.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.6.4/test/test_x509.py` & `resotolib-3.6.5/test/test_x509.py`

 * *Files identical despite different names*

