# Comparing `tmp/zq-tools-1.0.1.tar.gz` & `tmp/zq-tools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zq-tools-1.0.1.tar", last modified: Thu Jul 20 10:30:19 2023, max compression
+gzip compressed data, was "zq-tools-1.0.2.tar", last modified: Wed Aug  2 03:39:00 2023, max compression
```

## Comparing `zq-tools-1.0.1.tar` & `zq-tools-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:30:19.260483 zq-tools-1.0.1/
--rw-r--r--   0 togo      (1000) togo      (1000)     3069 2023-07-20 10:30:19.260483 zq-tools-1.0.1/PKG-INFO
--rw-r--r--   0 togo      (1000) togo      (1000)     2736 2023-07-20 10:30:08.000000 zq-tools-1.0.1/README.md
--rw-r--r--   0 togo      (1000) togo      (1000)       38 2023-07-20 10:30:19.260483 zq-tools-1.0.1/setup.cfg
--rw-r--r--   0 togo      (1000) togo      (1000)      622 2023-07-20 10:30:12.000000 zq-tools-1.0.1/setup.py
-drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:30:19.250483 zq-tools-1.0.1/test/
--rw-r--r--   0 togo      (1000) togo      (1000)      256 2023-07-20 10:09:20.000000 zq-tools-1.0.1/test/test_zq_logger.py
--rw-r--r--   0 togo      (1000) togo      (1000)     1051 2023-07-20 09:54:35.000000 zq-tools-1.0.1/test/test_zq_tracing.py
-drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:30:19.260483 zq-tools-1.0.1/zq_tools/
--rw-r--r--   0 togo      (1000) togo      (1000)      187 2023-07-20 09:54:35.000000 zq-tools-1.0.1/zq_tools/__init__.py
--rw-r--r--   0 togo      (1000) togo      (1000)      830 2023-07-20 09:54:35.000000 zq-tools-1.0.1/zq_tools/zq_cycle.py
--rw-r--r--   0 togo      (1000) togo      (1000)     4596 2023-07-20 09:54:35.000000 zq-tools-1.0.1/zq_tools/zq_decorator.py
--rw-r--r--   0 togo      (1000) togo      (1000)      520 2023-07-20 09:54:35.000000 zq-tools-1.0.1/zq_tools/zq_files.py
--rw-r--r--   0 togo      (1000) togo      (1000)     8517 2023-07-20 10:29:03.000000 zq-tools-1.0.1/zq_tools/zq_logger.py
--rw-r--r--   0 togo      (1000) togo      (1000)     5227 2023-07-20 09:54:35.000000 zq-tools-1.0.1/zq_tools/zq_tracing.py
-drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-07-20 10:30:19.260483 zq-tools-1.0.1/zq_tools.egg-info/
--rw-r--r--   0 togo      (1000) togo      (1000)     3069 2023-07-20 10:30:19.000000 zq-tools-1.0.1/zq_tools.egg-info/PKG-INFO
--rw-r--r--   0 togo      (1000) togo      (1000)      357 2023-07-20 10:30:19.000000 zq-tools-1.0.1/zq_tools.egg-info/SOURCES.txt
--rw-r--r--   0 togo      (1000) togo      (1000)        1 2023-07-20 10:30:19.000000 zq-tools-1.0.1/zq_tools.egg-info/dependency_links.txt
--rw-r--r--   0 togo      (1000) togo      (1000)       23 2023-07-20 10:30:19.000000 zq-tools-1.0.1/zq_tools.egg-info/requires.txt
--rw-r--r--   0 togo      (1000) togo      (1000)        9 2023-07-20 10:30:19.000000 zq-tools-1.0.1/zq_tools.egg-info/top_level.txt
+drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-08-02 03:39:00.108540 zq-tools-1.0.2/
+-rw-r--r--   0 togo      (1000) togo      (1000)     3040 2023-08-02 03:39:00.108540 zq-tools-1.0.2/PKG-INFO
+-rw-r--r--   0 togo      (1000) togo      (1000)     2707 2023-08-02 03:37:45.000000 zq-tools-1.0.2/README.md
+-rw-r--r--   0 togo      (1000) togo      (1000)       38 2023-08-02 03:39:00.108540 zq-tools-1.0.2/setup.cfg
+-rw-r--r--   0 togo      (1000) togo      (1000)      622 2023-08-02 03:38:09.000000 zq-tools-1.0.2/setup.py
+drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-08-02 03:39:00.108540 zq-tools-1.0.2/test/
+-rw-r--r--   0 togo      (1000) togo      (1000)       91 2023-08-02 02:47:40.000000 zq-tools-1.0.2/test/test_zq_logger.py
+-rw-r--r--   0 togo      (1000) togo      (1000)     1051 2023-08-02 02:47:40.000000 zq-tools-1.0.2/test/test_zq_tracing.py
+drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-08-02 03:39:00.108540 zq-tools-1.0.2/zq_tools/
+-rw-r--r--   0 togo      (1000) togo      (1000)      187 2023-08-02 02:47:40.000000 zq-tools-1.0.2/zq_tools/__init__.py
+-rw-r--r--   0 togo      (1000) togo      (1000)      830 2023-08-02 02:47:40.000000 zq-tools-1.0.2/zq_tools/zq_cycle.py
+-rw-r--r--   0 togo      (1000) togo      (1000)     4596 2023-08-02 02:47:40.000000 zq-tools-1.0.2/zq_tools/zq_decorator.py
+-rw-r--r--   0 togo      (1000) togo      (1000)      520 2023-08-02 02:47:40.000000 zq-tools-1.0.2/zq_tools/zq_files.py
+-rw-r--r--   0 togo      (1000) togo      (1000)     9290 2023-08-02 03:35:41.000000 zq-tools-1.0.2/zq_tools/zq_logger.py
+-rw-r--r--   0 togo      (1000) togo      (1000)     5227 2023-08-02 02:47:40.000000 zq-tools-1.0.2/zq_tools/zq_tracing.py
+drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-08-02 03:39:00.108540 zq-tools-1.0.2/zq_tools.egg-info/
+-rw-r--r--   0 togo      (1000) togo      (1000)     3040 2023-08-02 03:39:00.000000 zq-tools-1.0.2/zq_tools.egg-info/PKG-INFO
+-rw-r--r--   0 togo      (1000) togo      (1000)      357 2023-08-02 03:39:00.000000 zq-tools-1.0.2/zq_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 togo      (1000) togo      (1000)        1 2023-08-02 03:39:00.000000 zq-tools-1.0.2/zq_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 togo      (1000) togo      (1000)       23 2023-08-02 03:39:00.000000 zq-tools-1.0.2/zq_tools.egg-info/requires.txt
+-rw-r--r--   0 togo      (1000) togo      (1000)        9 2023-08-02 03:39:00.000000 zq-tools-1.0.2/zq_tools.egg-info/top_level.txt
```

### Comparing `zq-tools-1.0.1/PKG-INFO` & `zq-tools-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-tools
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of tools for zzqq2199
 Author: zzqq2199
 Author-email: zhouquanjs@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -19,15 +19,15 @@
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
-- 1.0.1: make `zq_logger` support print to screen and file with different levels
+- 1.0.2: Fine grained control of different handlers
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
 - 0.9.4: fix bug: `zq_decorator.time_it(sync)`
 - 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
 - 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
```

### Comparing `zq-tools-1.0.1/README.md` & `zq-tools-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
-- 1.0.1: make `zq_logger` support print to screen and file with different levels
+- 1.0.2: Fine grained control of different handlers
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
 - 0.9.4: fix bug: `zq_decorator.time_it(sync)`
 - 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
 - 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
```

### Comparing `zq-tools-1.0.1/setup.py` & `zq-tools-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="zq-tools",
-    version="1.0.1",
+    version="1.0.2",
     author="zzqq2199",
     author_email="zhouquanjs@qq.com",
     description="A collection of tools for zzqq2199",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["zq_tools"],
     classifiers=[
```

### Comparing `zq-tools-1.0.1/test/test_zq_tracing.py` & `zq-tools-1.0.2/test/test_zq_tracing.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.1/zq_tools/zq_cycle.py` & `zq-tools-1.0.2/zq_tools/zq_cycle.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.1/zq_tools/zq_decorator.py` & `zq-tools-1.0.2/zq_tools/zq_decorator.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.1/zq_tools/zq_files.py` & `zq-tools-1.0.2/zq_tools/zq_files.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.1/zq_tools/zq_logger.py` & `zq-tools-1.0.2/zq_tools/zq_logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,28 +27,39 @@
     ]
     def __init__(self, name):
         super(ZQ_Logger, self).__init__(name)
         self.tag = ""
         self.print_thread = False
         self.print_level = True
         self.rank = 0
-        self.log_files = dict()
+        self.name2handler = dict()
+        logging.Logger.setLevel(self, logging.DEBUG)
+
         
-    def add_log_file(self, log_file:str, level:int=logging.DEBUG):
-        # file handler follows same level control behavior as console handler
-        if log_file in self.log_files: return
-        if log_file in self.log_files:
-            handler = self.log_files[log_file]
-            handler.setLevel(level)
-            return
+    def add_log_file(self, log_file:str, name:str=""):
+        if not name: name = log_file
+        if name in self.name2handler: return
         handler = logging.FileHandler(log_file)
-        handler.setLevel(level)
-        self.log_files[log_file] = handler
+        self.name2handler[name] = handler
         self.addHandler(handler)
         self.reset_format()
+
+    def set_level_for_handler(self, name:str, level:int):
+        if name not in self.name2handler: return
+        handler: logging.Handler = self.name2handler[name]
+        handler.setLevel(level)
+        
+    def set_level_for_all(self, level:int):
+        for name in self.name2handler:
+            handler: logging.Handler = self.name2handler[name]
+            handler.setLevel(level)
+    
+    def setLevel(self, *args, **kwargs):
+        print(f"Warn: `setLevel` is not supported, use `set_level_for_all` instead")
+        
         
         
     def generate_fmt(self)->logging.StreamHandler:
         thread_fmt = "" if not self.print_thread else "[%(threadName)s] "
         level_fmt = "" if not self.print_level else " [%(levelname)s]"
         basic_fmt = f'[%(asctime)s.%(msecs)03d] {thread_fmt}"%(pathname)s", line %(lineno)d{level_fmt}:{self.tag} %(message)s'
         date_fmt = "%Y-%m-%d %H:%M:%S"
@@ -87,21 +98,21 @@
         self._log(self.PRANK, color(msg), args, **kwargs)
     def debug(self, msg:str, color:str='',*args, **kwargs):
         '''print with rank. If color is not specified, use the color format corresponding to the rank'''
         if not self.isEnabledFor(self.DEBUG): return
         color = getattr(cf, color) if color else self.default_color
         self._log(self.DEBUG, color(msg), args, **kwargs)
     def info(self, msg:str, *args, **kwargs):
-        self._log(logging.INFO, cf.green(msg), args, kwargs)
+        if self.isEnabledFor(logging.INFO): self._log(logging.INFO, cf.green(msg), args, kwargs)
     def warn(self, msg:str, *args, **kwargs):
-        self._log(logging.WARN, cf.yellow(msg), args, kwargs)
+        if self.isEnabledFor(logging.WARN): self._log(logging.WARN, cf.yellow(msg), args, kwargs)
     def error(self, msg:str, *args, **kwargs):
-        self._log(logging.ERROR, cf.red(msg), args, kwargs)
+        if self.isEnabledFor(logging.ERROR): self._log(logging.ERROR, cf.red(msg), args, kwargs)
     def fatal(self, msg:str, *args, **kwargs):
-        self._log(logging.FATAL, cf.bold_red(msg), args, kwargs)
+        if self.isEnabledFor(logging.FATAL): self._log(logging.FATAL, cf.bold_red(msg), args, kwargs)
 
     def prank_root(self, msg:str, color:str='', root=0, *args, **kwargs):
         '''print with rank. If color is not specified, use the color format corresponding to the rank'''
         if self.rank != root: return
         if not self.isEnabledFor(self.PRANK): return
         color = getattr(cf, color) if color else self.default_color
         self._log(self.PRANK, color(msg), args, **kwargs)
@@ -109,90 +120,91 @@
         '''print with rank. If color is not specified, use the color format corresponding to the rank'''
         if self.rank != root: return
         if not self.isEnabledFor(self.DEBUG): return
         color = getattr(cf, color) if color else self.default_color
         self._log(self.DEBUG, color(msg), args, **kwargs)
     def info_root(self, msg:str, root=0, *args, **kwargs):
         if self.rank != root: return
-        self._log(logging.INFO, cf.green(msg), args, kwargs)
+        if self.isEnabledFor(logging.INFO): self._log(logging.INFO, cf.green(msg), args, kwargs)
     def warn_root(self, msg:str, root=0, *args, **kwargs):
         if self.rank != root: return
-        self._log(logging.WARN, cf.yellow(msg), args, kwargs)
+        if self.isEnabledFor(logging.WARN): self._log(logging.WARN, cf.yellow(msg), args, kwargs)
     def error_root(self, msg:str, root=0, *args, **kwargs):
         if self.rank != root: return
-        self._log(logging.ERROR, cf.red(msg), args, kwargs)
+        if self.isEnabledFor(logging.ERROR): self._log(logging.ERROR, cf.red(msg), args, kwargs)
     def fatal_root(self, msg:str, root=0, *args, **kwargs):
         if self.rank != root: return
-        self._log(logging.FATAL, cf.bold_red(msg), args, kwargs)
+        if self.isEnabledFor(logging.FATAL): self._log(logging.FATAL, cf.bold_red(msg), args, kwargs)
         
     warning = warn
     critical = fatal
     warning_root = warn_root
     critical_root = fatal_root
     
 def get_level_from_env(logger_name:str, default_level="info"):
     level = default_level if logger_name not in os.environ else os.environ[logger_name]
+    level = level.lower()
     level2num = {
         "debug": logging.DEBUG,
         "info": logging.INFO,
         "warn": logging.WARN,
         "warning": logging.WARN,
         "error": logging.ERROR,
         "fatal": logging.FATAL,
         "critical": logging.FATAL,
     }
     if level in level2num: return level2num[level]
     print(f"Unknown level {level} for logger {logger_name}, use default level {default_level}")
     return level2num[default_level]
 
     
-    
 
 def get_logger(logger_name="Z_LEVEL",
                enable_console = True)->ZQ_Logger:
     if logger_name in allocated_loggers: return allocated_loggers[logger_name]
     # why need to call `setLoggerClass` twice? refer to the issue: https://bugs.python.org/issue37258
     logging.setLoggerClass(ZQ_Logger)
-    logger = logging.getLogger(logger_name)
+    logger:ZQ_Logger = logging.getLogger(logger_name)
     logging.setLoggerClass(logging.Logger)
-    logger.setLevel(logging.DEBUG)
     # Initilize level from environment. If not specified, use INFO
     if enable_console:
-        console_handler = logging.StreamHandler()
-        console_handler.setLevel(get_level_from_env(logger_name))
-        logger.addHandler(console_handler)
+        streamHandler = logging.StreamHandler()
+        name = logger_name
+        logger.name2handler[name] = streamHandler
+        streamHandler.setLevel(get_level_from_env(logger_name))
+        logger.addHandler(streamHandler)
     logger.reset_format()
     allocated_loggers[logger_name] = logger
     return logger
 
 default_logger = get_logger()
 
 
 if __name__ == '__main__':
     def test_environ():
         print(f'{"="*20} test environ {"="*20}')
         logger1 = get_logger("logger1")
         logger1.debug("this message should not be printed due to default initilizing level is INFO")
-        logger1.setLevel(logger1.DEBUG)
-        logger1.debug("this message should be printed due to call `setLevel`")
+        logger1.set_level_for_all(logger1.DEBUG)
+        logger1.debug("this message should be printed due to call `set_level_for_all`")
         os.environ['logger2'] = "debug"
         logger2 = get_logger("logger2")
         logger2.debug("this message should be printed due to env `logger` is set to `debug`")
     
     def test_log_file():
         print(f'{"="*20} test log file {"="*20}')
         # recommend to use `ANSI Color` extention to view log file in VSCode
         logger = get_logger("test_log_file")
         logger.add_log_file("demo.log")
-        logger.info(f"this message should be printed to both console and file {logger.log_files}")
+        logger.info(f"this message should be printed to both console and file {logger.name2handler.keys()}")
         
     def test_ranks():
         print(f'{"="*20} test ranks {"="*20}')
         logger=get_logger("test_ranks")
-        logger.setLevel(logger.DEBUG)
+        logger.set_level_for_handler("test_ranks", logger.DEBUG)
         logger.debug_root("printed due to default rank is 0 and default style is plain")
         logger.debug_root("NOT printed due to default rank is 0", root=2)
         for rank in range(8):
             logger.set_rank(rank)
             logger.debug(f"style of rank {rank}")
 
     def test_styles():
```

### Comparing `zq-tools-1.0.1/zq_tools/zq_tracing.py` & `zq-tools-1.0.2/zq_tools/zq_tracing.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.1/zq_tools.egg-info/PKG-INFO` & `zq-tools-1.0.2/zq_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-tools
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of tools for zzqq2199
 Author: zzqq2199
 Author-email: zhouquanjs@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -19,15 +19,15 @@
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
-- 1.0.1: make `zq_logger` support print to screen and file with different levels
+- 1.0.2: Fine grained control of different handlers
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
 - 0.9.4: fix bug: `zq_decorator.time_it(sync)`
 - 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
 - 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
```

