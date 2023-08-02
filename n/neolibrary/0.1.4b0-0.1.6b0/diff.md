# Comparing `tmp/neolibrary-0.1.4b0.tar.gz` & `tmp/neolibrary-0.1.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neolibrary-0.1.4b0.tar", max compression
+gzip compressed data, was "neolibrary-0.1.6b0.tar", max compression
```

## Comparing `neolibrary-0.1.4b0.tar` & `neolibrary-0.1.6b0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/LICENSE
--rw-r--r--   0        0        0      448 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/README.md
--rw-r--r--   0        0        0      445 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/src/neolibrary/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/src/neolibrary/monitoring/__init__.py
--rw-r--r--   0        0        0      770 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/src/neolibrary/monitoring/config/config.py
--rw-r--r--   0        0        0     3518 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/src/neolibrary/monitoring/logger.py
--rw-r--r--   0        0        0      714 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/src/neolibrary/utils.py
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 neolibrary-0.1.4b0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-02 12:08:53.618984 neolibrary-0.1.6b0/LICENSE
+-rw-r--r--   0        0        0     3562 2023-08-02 12:08:53.618984 neolibrary-0.1.6b0/README.md
+-rw-r--r--   0        0        0      592 2023-08-02 12:08:53.622984 neolibrary-0.1.6b0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 12:08:53.622984 neolibrary-0.1.6b0/src/neolibrary/__init__.py
+-rw-r--r--   0        0        0      696 2023-08-02 12:08:53.622984 neolibrary-0.1.6b0/src/neolibrary/decorators.py
+-rw-r--r--   0        0        0        0 2023-08-02 12:08:53.622984 neolibrary-0.1.6b0/src/neolibrary/monitoring/__init__.py
+-rw-r--r--   0        0        0      769 2023-08-02 12:08:53.622984 neolibrary-0.1.6b0/src/neolibrary/monitoring/config/config.py
+-rw-r--r--   0        0        0     8376 2023-08-02 12:08:53.622984 neolibrary-0.1.6b0/src/neolibrary/monitoring/logger.py
+-rw-r--r--   0        0        0      143 2023-08-02 12:08:53.622984 neolibrary-0.1.6b0/src/neolibrary/preproc.py
+-rw-r--r--   0        0        0     5388 2023-08-02 12:08:53.622984 neolibrary-0.1.6b0/src/neolibrary/utils.py
+-rw-r--r--   0        0        0     4200 1970-01-01 00:00:00.000000 neolibrary-0.1.6b0/PKG-INFO
```

### Comparing `neolibrary-0.1.4b0/LICENSE` & `neolibrary-0.1.6b0/LICENSE`

 * *Files identical despite different names*

### Comparing `neolibrary-0.1.4b0/src/neolibrary/monitoring/config/config.py` & `neolibrary-0.1.6b0/src/neolibrary/monitoring/config/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 ROOT = os.getcwd()
 
 SUCCESS = 15
 FAIL = 16
 PIPE = 17
 LOG_LEVEL = logging.INFO
 LOG_LEVEL_E = logging.WARNING
-LOGFORMAT = "%(log_color)s%(asctime) s%(reset)s |%(log_color)s %(filename)s:%(name)s%(reset)s |%(log_color)s%(levelname)-8s%(reset)s | %(log_color)s%(message)s%(reset)s | level=%(levelname)s%(reset)s"
-LOGFORMAT_ERROR = "%(log_color)s%(asctime)s %(reset)s | %(log_color)s %(filename)s:%(name)s%(reset)s | %(log_color)s%(levelname)-8s%(reset)s | %(log_color)s%(message)s%(reset)s | level=%(levelname)s%(reset)s"
+LOGFORMAT = '%(log_color)s%(asctime) s%(reset)s |%(log_color)s %(filename)s:%(name)s%(reset)s |%(log_color)s%(levelname)-8s%(reset)s | %(log_color)s%(message)s%(reset)s | level=%(levelname)s%(reset)s'
+LOGFORMAT_ERROR = '%(log_color)s%(asctime)s %(reset)s | %(log_color)s %(filename)s:%(name)s%(reset)s | %(log_color)s%(levelname)-8s%(reset)s | %(log_color)s%(message)s%(reset)s | level=%(levelname)s%(reset)s'
 
 LOG_COLORS = {
-    "DEBUG": "white,bg_black",
-    "INFO": "cyan",
-    "WARNING": "yellow",
-    "ERROR": "red",
-    "CRITICAL": "red,bg_black",
-    "SUCCESS": "bold_green",
-    "FAIL": "white,bg_black",
-    "PIPE": "green",
-}
+    'DEBUG': 'white,bg_black',
+    'INFO': 'cyan',
+    'WARNING': 'yellow',
+    'ERROR': 'red',
+    'CRITICAL': 'red,bg_black',
+    'SUCCESS': 'bold_green',
+    'FAIL': 'white,bg_black',
+    'PIPE': 'green',
+}
```

### Comparing `neolibrary-0.1.4b0/src/neolibrary/utils.py` & `neolibrary-0.1.6b0/src/neolibrary/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Callable
 from functools import wraps
 from time import time
-from neolibrary.monitoring.logger import NeoLogger
+from typing import Callable
 
-logger = NeoLogger(__name__).get_logger()
+from neolibrary.monitoring.logger import NeoLogger
 
+log = NeoLogger(__name__)
 
 
 def timer(orig_func: Callable):
     """This is custom timer decorator.
     Parameters
     ----------
     orig_func : object
@@ -21,11 +21,11 @@
     """
 
     @wraps(orig_func)
     def wrapper(*args, **kwargs):
         t1 = time()
         result = orig_func(*args, **kwargs)
         t2 = time() - t1
-        logger.info('Runtime for {}: {} sec'.format(orig_func.__name__, t2))
+        log.info('Runtime for {}: {} sec'.format(orig_func.__name__, t2))
         return result
 
-    return wrapper
+    return wrapper
```

