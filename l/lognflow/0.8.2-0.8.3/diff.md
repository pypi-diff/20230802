# Comparing `tmp/lognflow-0.8.2.tar.gz` & `tmp/lognflow-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.8.2.tar", last modified: Wed Aug  2 09:53:57 2023, max compression
+gzip compressed data, was "lognflow-0.8.3.tar", last modified: Wed Aug  2 11:53:47 2023, max compression
```

## Comparing `lognflow-0.8.2.tar` & `lognflow-0.8.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:53:57.167273 lognflow-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 09:53:47.000000 lognflow-0.8.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-02 09:53:47.000000 lognflow-0.8.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-02 09:53:47.000000 lognflow-0.8.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-02 09:53:47.000000 lognflow-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-02 09:53:47.000000 lognflow-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-08-02 09:53:57.167273 lognflow-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-02 09:53:47.000000 lognflow-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:53:57.163273 lognflow-0.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 09:53:47.000000 lognflow-0.8.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:53:57.163273 lognflow-0.8.2/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-02 09:53:47.000000 lognflow-0.8.2/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62870 2023-08-02 09:53:47.000000 lognflow-0.8.2/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-08-02 09:53:47.000000 lognflow-0.8.2/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-08-02 09:53:47.000000 lognflow-0.8.2/lognflow/printprogress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 09:53:47.000000 lognflow-0.8.2/lognflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:53:57.163273 lognflow-0.8.2/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-08-02 09:53:57.000000 lognflow-0.8.2/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-02 09:53:57.000000 lognflow-0.8.2/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:53:57.000000 lognflow-0.8.2/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:53:56.000000 lognflow-0.8.2/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 09:53:57.000000 lognflow-0.8.2/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 09:53:57.000000 lognflow-0.8.2/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 09:53:57.167273 lognflow-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-02 09:53:47.000000 lognflow-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:53:57.167273 lognflow-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 09:53:47.000000 lognflow-0.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-08-02 09:53:47.000000 lognflow-0.8.2/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-08-02 09:53:47.000000 lognflow-0.8.2/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-02 09:53:47.000000 lognflow-0.8.2/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:53:47.523294 lognflow-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 11:53:32.000000 lognflow-0.8.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-02 11:53:32.000000 lognflow-0.8.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-08-02 11:53:32.000000 lognflow-0.8.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-02 11:53:32.000000 lognflow-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-02 11:53:32.000000 lognflow-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-08-02 11:53:47.523294 lognflow-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-02 11:53:32.000000 lognflow-0.8.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:53:47.519294 lognflow-0.8.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 11:53:32.000000 lognflow-0.8.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:53:47.519294 lognflow-0.8.3/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-02 11:53:32.000000 lognflow-0.8.3/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62863 2023-08-02 11:53:32.000000 lognflow-0.8.3/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-08-02 11:53:32.000000 lognflow-0.8.3/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-08-02 11:53:32.000000 lognflow-0.8.3/lognflow/printprogress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 11:53:32.000000 lognflow-0.8.3/lognflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:53:47.519294 lognflow-0.8.3/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-08-02 11:53:47.000000 lognflow-0.8.3/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-02 11:53:47.000000 lognflow-0.8.3/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:53:47.000000 lognflow-0.8.3/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:53:47.000000 lognflow-0.8.3/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 11:53:47.000000 lognflow-0.8.3/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 11:53:47.000000 lognflow-0.8.3/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 11:53:47.523294 lognflow-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-02 11:53:32.000000 lognflow-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:53:47.523294 lognflow-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 11:53:32.000000 lognflow-0.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-08-02 11:53:32.000000 lognflow-0.8.3/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-08-02 11:53:32.000000 lognflow-0.8.3/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-02 11:53:32.000000 lognflow-0.8.3/tests/test_printprogress.py
```

### Comparing `lognflow-0.8.2/CONTRIBUTING.rst` & `lognflow-0.8.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/HISTORY.rst` & `lognflow-0.8.3/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 * utils.py is added to contain all misc functions.
 * replace_all added to utils
 
 0.8.1 (2023-07-26)
 ------------------
 * a bug fixed in log_var
 
-0.8.2 (2023-08-01)
+0.8.2 (2023-08-02)
 ------------------
 * the word save_as is now replaced with suffix as is in pathlib
 * all loggers can take the suffix as the extension in the parameter_name
 
-0.8.3 (2023-08-20)
+0.8.3 (2023-08-02)
 -----------------
-* time_tag is automatically disabled if extension is given, unless overwriting
+* critical bug fixed in log_var to support v0.8.2
```

### Comparing `lognflow-0.8.2/LICENSE` & `lognflow-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/PKG-INFO` & `lognflow-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.8.2
+Version: 0.8.3
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -217,15 +217,15 @@
 * utils.py is added to contain all misc functions.
 * replace_all added to utils
 
 0.8.1 (2023-07-26)
 ------------------
 * a bug fixed in log_var
 
-0.8.2 (2023-08-01)
+0.8.2 (2023-08-02)
 ------------------
 * the word save_as is now replaced with suffix as is in pathlib
 * all loggers can take the suffix as the extension in the parameter_name
 
-0.8.3 (2023-08-20)
+0.8.3 (2023-08-02)
 -----------------
-* time_tag is automatically disabled if extension is given, unless overwriting
+* critical bug fixed in log_var to support v0.8.2
```

### Comparing `lognflow-0.8.2/README.rst` & `lognflow-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/docs/Makefile` & `lognflow-0.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/docs/conf.py` & `lognflow-0.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/docs/installation.rst` & `lognflow-0.8.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/docs/make.bat` & `lognflow-0.8.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/lognflow/lognflow.py` & `lognflow-0.8.3/lognflow/lognflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
                     
         """
         try:
             _ = parameter_value.shape
         except:
             parameter_value = np.array([parameter_value])
         
-        _, parameter_name, suffix = self._param_dir_name_suffix(parameter_name, suffix)
+        _, _, suffix = self._param_dir_name_suffix(parameter_name, suffix)
         if(suffix is None):
             suffix = 'npz'
         
         log_counter_limit = self._get_log_counter_limit(\
             parameter_value, log_size_limit)
 
         if(parameter_name in self._vars_dict):
@@ -538,15 +538,15 @@
                 self.log_name,
                 f'current index {curr_index} cannot be used in the logger')
         if(parameter_value.shape == data_array[curr_index].shape):
             data_array[curr_index] = parameter_value
         else:
             self.log_text(
                 self.log_name,
-                f'Shape of variable {parameter_name} cannot change '\
+                f'Shape of variable {parameter_name} cannot change shape '\
                 f'from {data_array[curr_index].shape} '\
                 f'to {parameter_value.shape}. Coppying from the last time.')
             data_array[curr_index] = data_array[curr_index - 1]
         self._vars_dict[parameter_name] = varinlog(data_array, 
                                                    time_array, 
                                                    curr_index,
                                                    file_start_time,
```

### Comparing `lognflow-0.8.2/lognflow/logviewer.py` & `lognflow-0.8.3/lognflow/logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/lognflow/printprogress.py` & `lognflow-0.8.3/lognflow/printprogress.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/lognflow/utils.py` & `lognflow-0.8.3/lognflow/utils.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/lognflow.egg-info/PKG-INFO` & `lognflow-0.8.3/lognflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.8.2
+Version: 0.8.3
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -217,15 +217,15 @@
 * utils.py is added to contain all misc functions.
 * replace_all added to utils
 
 0.8.1 (2023-07-26)
 ------------------
 * a bug fixed in log_var
 
-0.8.2 (2023-08-01)
+0.8.2 (2023-08-02)
 ------------------
 * the word save_as is now replaced with suffix as is in pathlib
 * all loggers can take the suffix as the extension in the parameter_name
 
-0.8.3 (2023-08-20)
+0.8.3 (2023-08-02)
 -----------------
-* time_tag is automatically disabled if extension is given, unless overwriting
+* critical bug fixed in log_var to support v0.8.2
```

### Comparing `lognflow-0.8.2/lognflow.egg-info/SOURCES.txt` & `lognflow-0.8.3/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/setup.py` & `lognflow-0.8.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.8.2'
+__version__ = '0.8.3'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.8.2/tests/test_lognflow.py` & `lognflow-0.8.3/tests/test_lognflow.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/tests/test_logviewer.py` & `lognflow-0.8.3/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.2/tests/test_printprogress.py` & `lognflow-0.8.3/tests/test_printprogress.py`

 * *Files identical despite different names*

