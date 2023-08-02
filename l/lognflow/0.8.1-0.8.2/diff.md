# Comparing `tmp/lognflow-0.8.1.tar.gz` & `tmp/lognflow-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.8.1.tar", last modified: Wed Jul 26 05:02:09 2023, max compression
+gzip compressed data, was "lognflow-0.8.2.tar", last modified: Wed Aug  2 09:53:57 2023, max compression
```

## Comparing `lognflow-0.8.1.tar` & `lognflow-0.8.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:02:09.138044 lognflow-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-26 05:01:56.000000 lognflow-0.8.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-26 05:01:56.000000 lognflow-0.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-26 05:01:56.000000 lognflow-0.8.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-26 05:01:56.000000 lognflow-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-26 05:01:56.000000 lognflow-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-07-26 05:02:09.138044 lognflow-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-26 05:01:56.000000 lognflow-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:02:09.130044 lognflow-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:02:09.130044 lognflow-0.8.1/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-26 05:01:56.000000 lognflow-0.8.1/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63990 2023-07-26 05:01:56.000000 lognflow-0.8.1/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-26 05:01:56.000000 lognflow-0.8.1/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-26 05:01:56.000000 lognflow-0.8.1/lognflow/printprogress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-26 05:01:56.000000 lognflow-0.8.1/lognflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:02:09.134044 lognflow-0.8.1/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-07-26 05:02:09.000000 lognflow-0.8.1/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-26 05:02:09.000000 lognflow-0.8.1/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:02:09.000000 lognflow-0.8.1/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:02:08.000000 lognflow-0.8.1/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 05:02:09.000000 lognflow-0.8.1/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 05:02:09.000000 lognflow-0.8.1/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-26 05:02:09.138044 lognflow-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-26 05:01:56.000000 lognflow-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:02:09.138044 lognflow-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-26 05:01:56.000000 lognflow-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-26 05:01:56.000000 lognflow-0.8.1/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-26 05:01:56.000000 lognflow-0.8.1/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-26 05:01:56.000000 lognflow-0.8.1/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:53:57.167273 lognflow-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 09:53:47.000000 lognflow-0.8.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-02 09:53:47.000000 lognflow-0.8.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-02 09:53:47.000000 lognflow-0.8.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-02 09:53:47.000000 lognflow-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-02 09:53:47.000000 lognflow-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-08-02 09:53:57.167273 lognflow-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-02 09:53:47.000000 lognflow-0.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:53:57.163273 lognflow-0.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:53:57.163273 lognflow-0.8.2/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-02 09:53:47.000000 lognflow-0.8.2/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62870 2023-08-02 09:53:47.000000 lognflow-0.8.2/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-08-02 09:53:47.000000 lognflow-0.8.2/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-08-02 09:53:47.000000 lognflow-0.8.2/lognflow/printprogress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 09:53:47.000000 lognflow-0.8.2/lognflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:53:57.163273 lognflow-0.8.2/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-08-02 09:53:57.000000 lognflow-0.8.2/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-02 09:53:57.000000 lognflow-0.8.2/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:53:57.000000 lognflow-0.8.2/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:53:56.000000 lognflow-0.8.2/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 09:53:57.000000 lognflow-0.8.2/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 09:53:57.000000 lognflow-0.8.2/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 09:53:57.167273 lognflow-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-02 09:53:47.000000 lognflow-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:53:57.167273 lognflow-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 09:53:47.000000 lognflow-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-08-02 09:53:47.000000 lognflow-0.8.2/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-08-02 09:53:47.000000 lognflow-0.8.2/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-02 09:53:47.000000 lognflow-0.8.2/tests/test_printprogress.py
```

### Comparing `lognflow-0.8.1/CONTRIBUTING.rst` & `lognflow-0.8.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.1/HISTORY.rst` & `lognflow-0.8.2/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -122,8 +122,17 @@
 * logger.save and savez are set to be identical to log_single.
 * logged.load is set to be identical to get_single.
 * utils.py is added to contain all misc functions.
 * replace_all added to utils
 
 0.8.1 (2023-07-26)
 ------------------
-* a bug fixed in log_var
+* a bug fixed in log_var
+
+0.8.2 (2023-08-01)
+------------------
+* the word save_as is now replaced with suffix as is in pathlib
+* all loggers can take the suffix as the extension in the parameter_name
+
+0.8.3 (2023-08-20)
+-----------------
+* time_tag is automatically disabled if extension is given, unless overwriting
```

### Comparing `lognflow-0.8.1/LICENSE` & `lognflow-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.1/PKG-INFO` & `lognflow-0.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.8.1
+Version: 0.8.2
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -216,7 +216,16 @@
 * logged.load is set to be identical to get_single.
 * utils.py is added to contain all misc functions.
 * replace_all added to utils
 
 0.8.1 (2023-07-26)
 ------------------
 * a bug fixed in log_var
+
+0.8.2 (2023-08-01)
+------------------
+* the word save_as is now replaced with suffix as is in pathlib
+* all loggers can take the suffix as the extension in the parameter_name
+
+0.8.3 (2023-08-20)
+-----------------
+* time_tag is automatically disabled if extension is given, unless overwriting
```

### Comparing `lognflow-0.8.1/README.rst` & `lognflow-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.1/docs/Makefile` & `lognflow-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.1/docs/conf.py` & `lognflow-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.1/docs/installation.rst` & `lognflow-0.8.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.1/docs/make.bat` & `lognflow-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.1/lognflow/lognflow.py` & `lognflow-0.8.2/lognflow/lognflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 @dataclass
 class varinlog:
     data_array        : np.ndarray      
     time_array        : np.ndarray    
     curr_index        : int
     file_start_time   : float          
-    save_as           : str
+    suffix           : str
     log_counter_limit : int
 
 @dataclass
 class textinlog:
     to_be_logged        : str   
     log_fpath           : pathlib.Path         
     log_size_limit      : int 
@@ -131,18 +131,18 @@
     """
     
     def __init__(self, 
                  logs_root        : pathlib.Path = None,
                  log_dir          : pathlib.Path = None,
                  log_dir_prefix   : str          = None,
                  log_dir_suffix   : str          = None,
+                 time_tag         : bool         = True,
                  print_text       : bool         = True,
                  main_log_name    : str          = 'main_log',
-                 log_flush_period : int          = 10,
-                 time_tag         : bool         = True):
+                 log_flush_period : int          = 10):
         self._init_time = time.time()
         self.time_tag = time_tag
         self.log_dir_prefix = log_dir_prefix
         self.log_dir_suffix = log_dir_suffix
         
         if(log_dir is None):
             if(logs_root is None):
@@ -185,15 +185,15 @@
         self._single_var_call_cnt = 0
 
         self.log_name = main_log_name
         self.log_flush_period = log_flush_period
         self.save = self.log_single
     
     def savez(self, *args, **kwargs):
-        kwargs['save_as'] = 'npz'
+        kwargs['suffix'] = 'npz'
         return self.save(*args, **kwargs)
         
     @property
     def time_stamp(self):
         """ Current time stamp
             Gives the time after the start of the lognflow
         """
@@ -251,15 +251,15 @@
             self.log_text(None, 'Could not rename the log_dir from:')
             self.log_text(None, f'{self.log_dir.name}')
             self.log_text(None, 'into:')
             self.log_text(None, f'{new_name}')
             self.log_text(None, 'Most probably a file was open.')
         return self.log_dir
     
-    def _prepare_param_dir(self, parameter_name: str):
+    def _param_dir_name_suffix(self, parameter_name: str, suffix: str = None):
         
         assert isinstance(parameter_name, str), \
             f'The parameter name {parameter_name} is not a string.' \
             + f' It is of type {type(parameter_name)}.' \
             + 'Perhaps you forgot to pass the name of the variable first.'
         parameter_name = ''.join(
             [_ for _ in repr(repr_raw(parameter_name))  if _ != '\''])
@@ -270,49 +270,71 @@
         param_dir = self.log_dir /  parameter_name
         
         if(parameter_name[-1] == '/'):
             param_name = ''
         else:
             param_name = param_dir.name
             param_dir = param_dir.parent
-        if(not param_dir.is_dir()):
-            self.log_text(self.log_name,
-                          f'Creating directory: {param_dir.absolute()}')
-            param_dir.mkdir(parents = True, exist_ok = True)
-        return(param_dir, param_name)
+        
+        if(suffix == 'mat'):
+            if(len(param_name) == 0):
+                param_name = param_dir.name            
+        
+        if(suffix is None):
+            param_name_split = param_name.split('.')
+            if len(param_name_split) > 1:
+                param_suffix = param_name_split[-1]
+                #Here you can check if it is a valid extention
+                param_name = '.'.join(param_name_split[:-1])
+            else:
+                param_suffix = None
+        else:
+            param_suffix = suffix
+            param_name_split = param_name.split('.')
+            if len(param_name_split) > 1:
+                fname_suffix = param_name_split[-1]
+                if fname_suffix == param_suffix:
+                    param_name = '.'.join(param_name_split[:-1])
+    
+        return(param_dir, param_name, param_suffix)
 
     def _get_fpath(self, param_dir: pathlib.Path, param_name: str, 
-                   save_as: str, time_tag: bool = None) -> pathlib.Path:
+                   suffix: str, time_tag: bool = None) -> pathlib.Path:
         
         time_tag = self.time_tag if (time_tag is None) else time_tag
         
-        if(save_as == 'mat'):
-            if(len(param_name) == 0):
-                param_name = param_dir.name
+        if(not param_dir.is_dir()):
+            self.log_text(self.log_name,
+                          f'Creating directory: {param_dir.absolute()}')
+            param_dir.mkdir(parents = True, exist_ok = True)
         
         if(len(param_name) > 0):
             fname = f'{param_name}'
             if(time_tag):
                 fname += f'_{self.time_stamp:>6.6f}'
         else:
             fname = f'{self.time_stamp:>6.6f}'
         
-        return(param_dir / f'{fname}.{save_as}')
+        fpath = param_dir / f'{fname}.{suffix}'
+        
+        return fpath
         
-    def _log_text_handler(self, log_name = None, 
+    def _log_text_handler(self, log_name: str, 
                          log_size_limit: int = int(1e+7),
                          time_tag: bool = None,
                          log_flush_period = None,
-                         save_as = 'txt'):
+                         suffix = None):
         
         if (log_flush_period is None):
             log_flush_period = self.log_flush_period
-            
-        param_dir, param_name = self._prepare_param_dir(log_name)
-        fpath = self._get_fpath(param_dir, param_name, save_as, time_tag)
+        param_dir, param_name, suffix = self._param_dir_name_suffix(
+            log_name, suffix)
+        if suffix is None:
+            suffix = 'txt'
+        fpath = self._get_fpath(param_dir, param_name, suffix, time_tag)
         self._loggers_dict[log_name] = textinlog(
             to_be_logged=[],      
             log_fpath=fpath,         
             log_size_limit=log_size_limit,    
             log_size=0,          
             last_log_flush_time=0,
             log_flush_period=log_flush_period)  
@@ -328,14 +350,15 @@
             In later versions, a timer will be used to call it automatically.
             :param flush:
                 force the flush regardless of when the last time was.
                 default: False
             :type flush: bool
         """
         log_name = self.log_name if (log_name is None) else log_name
+        
         curr_textinlog = self._loggers_dict[log_name]
         
         if((self.time_stamp - curr_textinlog.last_log_flush_time \
                                            > curr_textinlog.log_flush_period)
            | flush):
             
             with open(curr_textinlog.log_fpath, 'a+') as f:
@@ -351,15 +374,15 @@
                  print_text = None,
                  log_size_limit: int = int(1e+7),
                  time_tag: bool = None,
                  log_flush_period: int = None,
                  flush = False,
                  end = '\n',
                  new_file = False,
-                 save_as = None):
+                 suffix = None):
         """ log a string into a text file
             You can shose a name for the log and give the text to put in it.
             Also you can pass a small numpy array. You can ask it to put time
             stamp in the log and in the log file name, you can disable
             printing the text. You can set the log size limit to split it into
             another file with a new time stamp.
             
@@ -386,43 +409,34 @@
                    force flush into the log file
             :param end: str
                    The last charachter for this call.
             :param new_file: bool
                    if a new file is needed. If time_tag is True, it will make
                    a new file with a new name that has a time tag. If False,
                    it closees the current text file and overwrites on it.
-            :param save_as: str
-                   save_as is the suffix of the text file.
+            :param suffix: str
+                   suffix is the extension of the file name.
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
         log_flush_period = self.log_flush_period \
             if (log_flush_period is None) else log_flush_period
-        
         log_name = self.log_name if (log_name is None) else log_name
 
-        if(save_as is None):
-            log_name_split = log_name.split('.')
-            if len(log_name_split) > 1:
-                save_as = log_name_split[-1]
-                log_name = '.'.join(log_name_split)
-        else:
-            save_as = 'txt'
+        if ( (not (log_name in self._loggers_dict)) or new_file):
+            self._log_text_handler(log_name, 
+                                   log_size_limit = log_size_limit,
+                                   time_tag = time_tag,
+                                   suffix = suffix)
 
         if((print_text is None) | (print_text is True)):
             print_text = self._print_text
         if(print_text):
             if(log_time_stamp):
                 print(f'T:{self.time_stamp:>6.6f}| ', end='')
             print(to_be_logged, end = end)
-        
-        if ( (not (log_name in self._loggers_dict)) or new_file):
-            self._log_text_handler(log_name, 
-                                   log_size_limit = log_size_limit,
-                                   time_tag = time_tag,
-                                   save_as = save_as)
 
         curr_textinlog = self._loggers_dict[log_name]
         _logger = []
         if(log_time_stamp):
             _time_str = f'T:{self.time_stamp:>6.6f}| '
             _logger.append(_time_str)
         if(isinstance(to_be_logged, list)):
@@ -444,25 +458,26 @@
         curr_textinlog.log_size += log_size
         
         self.log_text_flush(log_name, flush)        
 
         if(log_size >= curr_textinlog.log_size_limit):
             self._log_text_handler(log_name, 
                                    log_size_limit = curr_textinlog.log_size_limit,
-                                   time_tag = curr_textinlog.time_tag)
+                                   time_tag = curr_textinlog.time_tag,
+                                   suffix = suffix)
             curr_textinlog = self._loggers_dict[log_name]
         return curr_textinlog.log_fpath
                         
 
     def _get_log_counter_limit(self, param, log_size_limit):
         cnt_limit = int(log_size_limit/(param.size*param.itemsize))
         return cnt_limit
 
     def log_var(self, parameter_name: str, parameter_value, 
-                save_as = None, log_size_limit: int = int(1e+7)):
+                suffix = None, log_size_limit: int = int(1e+7)):
         """log a numpy array in buffer then dump
             It can be the case that we need to take snapshots of a numpy array
             over time. The size of the array would not change and this is hoing
             to happen frequently.
             This log_ver makes a buffer in RAM and keeps many instances of the
             array along with their time stamp and then when the size of the 
             array reaches a threhshold flushes it into HDD with a file that
@@ -473,42 +488,38 @@
             
             :param parameter_name: str
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
             :param parameter_value: np.array
                     An np array whose size doesn't change
-            :param save_as: str
+            :param suffix: str
                     can be 'npz' or 'txt' which will save it as text.
             :param log_size_limit: int
                     log_size_limit in bytes, default: 1e+7.
                     
         """
         try:
             _ = parameter_value.shape
         except:
             parameter_value = np.array([parameter_value])
         
-        if(save_as is None):
-            parameter_name_split = parameter_name.split('.')
-            if len(parameter_name_split) > 1:
-                save_as = parameter_name_split[-1]
-                parameter_name = '.'.join(parameter_name_split)
-        else:
-            save_as = 'npz'
+        _, parameter_name, suffix = self._param_dir_name_suffix(parameter_name, suffix)
+        if(suffix is None):
+            suffix = 'npz'
         
         log_counter_limit = self._get_log_counter_limit(\
             parameter_value, log_size_limit)
 
         if(parameter_name in self._vars_dict):
             _var = self._vars_dict[parameter_name]
             data_array, time_array, curr_index, \
-                file_start_time, save_as, log_counter_limit = \
+                file_start_time, suffix, log_counter_limit = \
                 (_var.data_array, _var.time_array, _var.curr_index, \
-                    _var.file_start_time, _var.save_as, _var.log_counter_limit)
+                    _var.file_start_time, _var.suffix, _var.log_counter_limit)
             curr_index += 1
         else:
             file_start_time = self.time_stamp
             curr_index = 0
 
         if(curr_index >= log_counter_limit):
             self.log_var_flush(parameter_name)
@@ -535,33 +546,33 @@
                 f'from {data_array[curr_index].shape} '\
                 f'to {parameter_value.shape}. Coppying from the last time.')
             data_array[curr_index] = data_array[curr_index - 1]
         self._vars_dict[parameter_name] = varinlog(data_array, 
                                                    time_array, 
                                                    curr_index,
                                                    file_start_time,
-                                                   save_as,
+                                                   suffix,
                                                    log_counter_limit)
 
     def log_var_flush(self, parameter_name: str):
         """ Flush the buffered numpy arrays
             If you have been using log_ver, this will flush all the buffered
             arrays. It is called using log_size_limit for a variable and als
             when the code that made the logger ends.
             :param parameter_name: str
                 examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
         """
-        param_dir, param_name = self._prepare_param_dir(parameter_name)
+        param_dir, param_name, _ = self._param_dir_name_suffix(parameter_name)
         
         _var = self._vars_dict[parameter_name]
         _var_data_array = _var.data_array[_var.time_array > 0]
         _var_time_array = _var.time_array[_var.time_array > 0]
-        if((_var.save_as == 'npz') | (_var.save_as == 'npy')):
+        if((_var.suffix == 'npz') | (_var.suffix == 'npy')):
             fpath = param_dir / f'{param_name}_{_var.file_start_time}.npz'
             np.savez(fpath,
                 time_array = _var_time_array,
                 data_array = _var_data_array)
         else:
             fpath = param_dir / f'{param_name}_time_{_var.file_start_time}.txt'
             np.savetxt(fpath, _var_time_array)
@@ -587,15 +598,15 @@
         _var = self._vars_dict[parameter_name]
         data_array = _var.data_array[_var.time_array>0].copy()
         time_array = _var.time_array[_var.time_array>0].copy()
         return(time_array, data_array)
 
     def log_single(self, parameter_name: str, 
                          parameter_value,
-                         save_as = None,
+                         suffix = None,
                          mat_field = None,
                          time_tag: bool = None):
         """log a single variable
             The most frequently used function would probably be this one.
             
             if you call the logger object as a function and give it a parameter
             name and something to be logged, the __call__ referes to this
@@ -605,59 +616,51 @@
                     examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
                     path like name such as myscript/myvar.
             :param parameter_value: np.array
                     Could be anything and np.save will be used. If it is a
                     dictionary, np.savez will be used. As you may know, np.save
                     can save all pickalables.
-            :param save_as: str
+            :param suffix: str
                     can be 'npz', 'npy', 'mat', 'torch' for pytorch models
                     or 'txt' or anything else which will save it as text.
                     This includes 'json', 'pdb', or ...
             :param mat_field: str
                     when saving as 'mat' file, the field can be set.
                     otherwise it will be the parameter_name
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
 
-        if(save_as is None):
-            parameter_name_split = parameter_name.split('.')
-            if len(parameter_name_split) > 1:
-                save_as = parameter_name_split[-1]
-                #YOU CAN CHECK IF IT IS LEGITEMATE EXTENSION
-                parameter_name = '.'.join(parameter_name_split)
-            elif isinstance(parameter_value, (np.ndarray, int, float)):
-                save_as = 'npy'
+        param_dir, param_name, suffix = self._param_dir_name_suffix(parameter_name, suffix)
+        if(suffix is None):
+            if isinstance(parameter_value, (np.ndarray, int, float)):
+                suffix = 'npy'
             elif (isinstance(parameter_value, dict)):
-                save_as = 'npz'
+                suffix = 'npz'
             else:
-                save_as = 'txt'
-        save_as = save_as.strip()
-        save_as = save_as.strip('.')
-
-        param_dir, param_name = self._prepare_param_dir(parameter_name)
-        fpath = self._get_fpath(param_dir, param_name, save_as, time_tag)
+                suffix = 'txt'
+        fpath = self._get_fpath(param_dir, param_name, suffix, time_tag)
         
         try:
-            if(save_as == 'npy'):
+            if(suffix == 'npy'):
                 np.save(fpath, parameter_value)
-            elif(save_as == 'npz'):
+            elif(suffix == 'npz'):
                 np.savez(fpath, **parameter_value)
-            elif((save_as == 'tif') | (save_as == 'tiff')):
+            elif((suffix == 'tif') | (suffix == 'tiff')):
                 from tifffile import imwrite
                 imwrite(fpath, parameter_value)
-            elif(save_as == 'mat'):
+            elif(suffix == 'mat'):
                 from scipy.io import savemat
                 if(mat_field is None):
                     mat_field = param_name
                 savemat(fpath, {f'{mat_field}':parameter_value})
-            elif(save_as == 'torch'):
+            elif(suffix == 'torch'):
                 from torch import save as torch_save
                 torch_save(parameter_value.state_dict(), fpath)
             else:
                 with open(fpath,'a') as fdata: 
                     fdata.write(str(parameter_value))
         except:
             fpath = None
@@ -677,15 +680,16 @@
                     path like name such as myscript/myvar.
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
-        param_dir, param_name = self._prepare_param_dir(parameter_name)
+        param_dir, param_name, image_format = \
+            self._param_dir_name_suffix(parameter_name, image_format)
         fpath = self._get_fpath(param_dir, param_name, image_format, time_tag)
         
         try:
             plt.savefig(fpath, format=image_format, dpi=dpi)
             if(close_plt):
                 plt.close()
             return fpath
@@ -1180,16 +1184,15 @@
             :param list_of_stacks
                     list_of_stacks would include arrays iteratable by their
                     first dimension.
             :param borders: float
                     borders between tiles will be filled with this variable
                     default: np.nan
         """        
-        if (not isinstance(list_of_stacks, list)):
-            list_of_stacks = [list_of_stacks]
+        list_of_stacks = list(list_of_stacks)
         for cnt, stack in enumerate(list_of_stacks):
             stack = self._handle_images_stack(stack, borders = borders)
             if(stack is None):
                 return
             list_of_stacks[cnt] = stack
         return(list_of_stacks)
 
@@ -1424,15 +1427,16 @@
                     n_f x n_r x n_c or n_f x n_r x n_c x 3
                     stack[cnt] needs to be plotable by plt.imshow()
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
-        param_dir, param_name = self._prepare_param_dir(parameter_name)
+        param_dir, param_name, _ = self._param_dir_name_suffix(parameter_name, 
+                                                               'gif')
         fpath = self._get_fpath(param_dir, param_name, 'gif', time_tag)
 
         fig, ax = plt.subplots()
         ims = []
         for img in stack:    
             im = ax.imshow(img, animated=True)
             plt.xticks([]),plt.yticks([])
@@ -1441,45 +1445,14 @@
             fig, ims, interval = interval, blit = blit,
             repeat_delay = repeat_delay)
 
         ani.save(fpath, dpi = dpi, 
                  writer = animation.PillowWriter(fps=int(1000/interval)))
         return fpath
 
-    def replace_time_with_index(self, var_name):
-        """ index in file names
-            lognflow uses time stamps to make new log files for a variable.
-            That is done by putting time stamp after the name of the variable.
-            This function changes all of the time stamps, sorted ascendingly,
-            by indices.
-            
-            :param var_name:
-                variable name
-        """
-        var_dir = self.log_dir / var_name
-        if(var_dir.is_dir()):
-            var_fname = None
-            flist = list(var_dir.glob(f'*.*'))
-        else:
-            var_fname = var_dir.name
-            var_dir = var_dir.parent
-            flist = list(var_dir.glob(f'{var_fname}_*.*'))
-        if flist:
-            flist.sort()
-            fcnt_width = len(str(len(flist)))
-            for fcnt, fpath in enumerate(flist):
-                # self.log_text(None, f'Changing {flist[fcnt].name}')
-                fname_new = ''
-                if(var_fname is not None):
-                    fname_new = var_fname + '_'
-                fname_new += f'{fcnt:0{fcnt_width}d}' + flist[fcnt].suffix
-                fpath_new = flist[fcnt].parent / fname_new
-                # self.log_text(None, f'To {fpath_new.name}')
-                flist[fcnt].rename(fpath_new)
-                
     def flush_all(self):
         for log_name in list(self._loggers_dict):
             self.log_text_flush(log_name, flush = True)
         for parameter_name in list(self._vars_dict):
             self.log_var_flush(parameter_name)
 
     def __call__(self, *args, **kwargs):
```

### Comparing `lognflow-0.8.1/lognflow/logviewer.py` & `lognflow-0.8.2/lognflow/logviewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -308,12 +308,43 @@
         flist_A_new = [parent_A / (common_stem + suffix_A) \
                           for common_stem in common_stems]
         flist_B_new = [parent_B / (common_stem + suffix_B) \
                           for common_stem in common_stems]
 
         return(flist_A_new, flist_B_new)
     
+    def replace_time_with_index(self, var_name):
+        """ index in file names
+            lognflow uses time stamps to make new log files for a variable.
+            That is done by putting time stamp after the name of the variable.
+            This function changes all of the time stamps, sorted ascendingly,
+            by indices.
+            
+            :param var_name:
+                variable name
+        """
+        var_dir = self.log_dir / var_name
+        if(var_dir.is_dir()):
+            var_fname = None
+            flist = list(var_dir.glob(f'*.*'))
+        else:
+            var_fname = var_dir.name
+            var_dir = var_dir.parent
+            flist = list(var_dir.glob(f'{var_fname}_*.*'))
+        if flist:
+            flist.sort()
+            fcnt_width = len(str(len(flist)))
+            for fcnt, fpath in enumerate(flist):
+                # self.log_text(None, f'Changing {flist[fcnt].name}')
+                fname_new = ''
+                if(var_fname is not None):
+                    fname_new = var_fname + '_'
+                fname_new += f'{fcnt:0{fcnt_width}d}' + flist[fcnt].suffix
+                fpath_new = flist[fcnt].parent / fname_new
+                # self.log_text(None, f'To {fpath_new.name}')
+                flist[fcnt].rename(fpath_new)
+    
     def __repr__(self):
         return f'{self.log_dir}'
 
     def __bool__(self):
         return self.log_dir.is_dir()
```

### Comparing `lognflow-0.8.1/lognflow/printprogress.py` & `lognflow-0.8.2/lognflow/printprogress.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.1/lognflow/utils.py` & `lognflow-0.8.2/lognflow/utils.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.1/lognflow.egg-info/PKG-INFO` & `lognflow-0.8.2/lognflow.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.8.1
+Version: 0.8.2
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -216,7 +216,16 @@
 * logged.load is set to be identical to get_single.
 * utils.py is added to contain all misc functions.
 * replace_all added to utils
 
 0.8.1 (2023-07-26)
 ------------------
 * a bug fixed in log_var
+
+0.8.2 (2023-08-01)
+------------------
+* the word save_as is now replaced with suffix as is in pathlib
+* all loggers can take the suffix as the extension in the parameter_name
+
+0.8.3 (2023-08-20)
+-----------------
+* time_tag is automatically disabled if extension is given, unless overwriting
```

### Comparing `lognflow-0.8.1/lognflow.egg-info/SOURCES.txt` & `lognflow-0.8.2/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.1/setup.py` & `lognflow-0.8.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.8.1'
+__version__ = '0.8.2'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.8.1/tests/test_lognflow.py` & `lognflow-0.8.2/tests/test_lognflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,36 +27,36 @@
     # assert 'GitHub' in BeautifulSoup(response.content).title.string
 
 def test_lognflow_conflict_in_names():
     logger = lognflow(temp_dir)
     logger('This is a test for conflict in names')
     logger1 = lognflow(logger.log_dir)
     logger2 = lognflow(logger.log_dir)
-    print(logger1.log_dir)
-    print(logger2.log_dir)
+    logger1(logger1.log_dir)
+    logger2(logger2.log_dir)
 
 def test_log_text():
-    logger = lognflow(temp_dir)
+    logger = lognflow(temp_dir, print_text = False)
     logger('This is a test for log_text')    
-    for _ in range(1000000):
+    for _ in range(10000):
         logger(f'{_}')
 
-    logger.log_text('not_main_script',
+    logger.log_text('not_main_script1.pdb',
            'This is a new log file for another script')
-    logger.log_text('not_main_script',
+    logger.log_text('not_main_script2.test',
                     'For other log files you need to mention the log_name')
     logger.log_text('not_main_script3',
-           'This is a new log file for another script')
-    logger.log_text('not_main_script4',
+           'This is a new log file for another script', suffix = 'io')
+    logger.log_text('test.to\not_main_script4.top',
                     'For other log files you need to mention the log_name')
-    logger.log_text('not_main_script',
+    logger.log_text('not_main_script2',
            'This is a new log file for another script')
-    logger.log_text('not_main_script',
+    logger.log_text('not_main_script2.test',
                     'For other log files you need to mention the log_name')
-    for _ in range(1000000):
+    for _ in range(10000):
         logger(f'{_}')
 
 def test_logger():
     ''' test the logger call funciton
         when lognflow object is made, you can call it.
         If it is called with a string as input, it will log that into the
         main_log text file.
@@ -69,20 +69,20 @@
 
     a = 20
     b = np.array([34])
     c = 'asdf'
     
     logger(a)
     logger.log_single('a', a)
-    logger.log_single('aa', a, save_as = 'txt', time_tag = False)
+    logger.log_single('aa', a, suffix = 'txt', time_tag = False)
     logger(b)
     logger.log_single('b', b)
-    logger.log_single('bb', b, save_as = 'txt', time_tag = False)
+    logger.log_single('bb', b, suffix = 'txt', time_tag = False)
     logger(c)
-    logger.log_single('test/c', c, save_as = 'txt')
+    logger.log_single('test/c', c, suffix = 'txt')
 
 def test_log_flush_period():
     logger = lognflow(temp_dir, log_flush_period = 30)
     logger('This is a test for lognflow and log_var')    
     
     time_time = time.time()
     for _ in range(20):
@@ -93,21 +93,20 @@
         
 
     logger.log_text('not_main_script',
            'This is a new log file for another script')
     logger.log_text('not_main_script',
                     'For other log files you need to mention the log_name')
 
-
 def test_log_var():
     logger = lognflow(temp_dir)
     logger('This is a test for lognflow and log_var')    
 
     for _ in range(1000):
-        logger.log_var('vars/vec/v', np.random.rand(10000))
+        logger.log_var('vars/vec/v.to.txt', np.random.rand(10000))
         
 def test_log_var_without_time_stamp():
     logger = lognflow(temp_dir)
     logger('This is a test for lognflow and log_var')    
 
     for _ in range(10):
         logger.log_single('vars/vec/v', np.random.rand(10000), 
@@ -120,19 +119,21 @@
     logger.log_animation('var1',var1)
 
 def test_log_single():
     var1 = np.random.rand(100)
     
     logger = lognflow(temp_dir)
     logger('This is a test for log_single')    
-    logger.log_single('var1',var1)
+    logger.log_single('var1/var1.txt', var1)
+    logger.log_single('var1/var1.npy', var1)
     a_dict = dict({'str_var': 'This is a string',
                    'var1': var1})
     logger.log_single('a_dict', a_dict)
-    logger.log_single('a_dict', a_dict, save_as = 'txt')
+    logger.log_single('a_dict.txt', a_dict)
+    logger.log_single('a_dict2', a_dict, suffix = 'txt')
 
 def test_log_plot():
     var1 = np.random.rand(100)
     var2 = 3 + np.random.rand(100)
     var3 = 6 + np.random.rand(100)
     
     logger = lognflow(temp_dir)
@@ -264,17 +265,17 @@
     logger.rename(logger.log_dir.name + '_new_name')
     logger('This is another test for test_rename')
     
 def test_log_single_text():
     logger = lognflow(temp_dir)
     logger('This is a test for test_log_single_text', flush = True)
     var = 2
-    logger.log_single('text_log\a\t/\b/\b//\\/b', 'hello\n', save_as='txt', time_tag = False)
-    logger.log_single('text_log\a', 'bye\n', save_as='json', time_tag = False)
-    logger.log_single('text_log\a', var, save_as='pdb', time_tag = False)
+    logger.log_single('text_log\a\t/\b/\b//\\/b', 'hello\n', suffix='txt', time_tag = False)
+    logger.log_single('text_log\a', 'bye\n', suffix='json', time_tag = False)
+    logger.log_single('text_log\a', var, suffix='pdb', time_tag = False)
     
 def test_log_imshow_complex():
     logger = lognflow(temp_dir)
     logger('This is a test for test_log_imshow_complex', flush = True)
     
     mat = np.random.rand(100, 100) + 10 * 1j * np.random.rand(100, 100)
     
@@ -292,43 +293,43 @@
     logged = logviewer(logger.log_dir, logger)
 
     data_in, flist = logged.get_stack_of_files(
         'test_param', return_data=True, return_flist=True)
     
     logger(flist)
 
-    logger.replace_time_with_index('test_param')
+    logger.logged.replace_time_with_index('test_param')
     
     data_out, flist = logged.get_stack_of_files(
         'test_param', return_data=True, return_flist=True)
     
     logger(flist)
     
     logger(data_in)
     logger(data_out)
     
 if __name__ == '__main__':
     
     #-----IF RUN BY PYTHON------#
     temp_dir = select_directory()
     #---------------------------#
+    test_log_single()
+    test_log_var()
+    test_log_text()
     test_log_single_text()
     test_log_imshow_complex()
     test_log_imshow()
-    test_log_text()
     test_log_surface()
-    test_log_single()
     test_lognflow_conflict_in_names()
     test_rename()
     test_log_plot()
     test_prepare_stack_of_images()
     test_logger()
     test_log_flush_period()
     test_log_var_without_time_stamp()
-    test_log_var()
     test_log_animation()
     test_log_hist()
     test_log_scatter3()
     test_log_plt()
     test_log_hexbin()
     test_log_canvas()
     test_log_confusion_matrix()
```

### Comparing `lognflow-0.8.1/tests/test_logviewer.py` & `lognflow-0.8.2/tests/test_logviewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         'A/', return_data=False, return_flist=True)
     flist_B = logged.get_stack_of_files(
         'B/', return_data=False, return_flist=True)
     
     logger(flist_A)
     logger(flist_B)
     
-    logger.replace_time_with_index('A/')
-    logger.replace_time_with_index('B/')
+    logger.logged.replace_time_with_index('A/')
+    logger.logged.replace_time_with_index('B/')
     
     stack_A = logged.get_stack_of_files('A/', return_data = True, return_flist = False)
     stack_B = logged.get_stack_of_files('B/', return_data = True, return_flist = False)
 
     logger(stack_A.shape)
     logger(stack_B.shape)
     
@@ -90,18 +90,18 @@
         _ = logger._loggers_dict['main_log'].log_size
         logger('Size of the log file in bytes is: ' \
                + f'{_}')
 
 def test_text_to_object():
     logger = lognflow(temp_dir, time_tag = False)
     test_list = ['asdf', 1243, "dd"]
-    logger.log_single('test_list', test_list, save_as = 'txt')
+    logger.log_single('test_list', test_list, suffix = 'txt')
     
     test_dict = {"one": "asdf", 'two': 1243, 'thre': "dd"}
-    logger.log_single('test_dict', test_dict, save_as = 'txt')
+    logger.log_single('test_dict', test_dict, suffix = 'txt')
     
     logged = logviewer(logger.log_dir)
     flist = logged.get_stack_of_files('*')
     print(flist)
     for file_name_input in flist:
         print('='*60)
         print(f'file name: {file_name_input}')
```

### Comparing `lognflow-0.8.1/tests/test_printprogress.py` & `lognflow-0.8.2/tests/test_printprogress.py`

 * *Files identical despite different names*

