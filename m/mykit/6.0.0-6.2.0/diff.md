# Comparing `tmp/mykit-6.0.0.tar.gz` & `tmp/mykit-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-d53acf6m/mykit-6.0.0.tar", last modified: Wed Jul  5 07:45:50 2023, max compression
+gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-ilfcgbdx/mykit-6.2.0.tar", last modified: Wed Aug  2 13:42:27 2023, max compression
```

## Comparing `mykit-6.0.0.tar` & `mykit-6.2.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-05 07:45:35.000000 mykit-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-05 07:45:50.000000 mykit-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-05 07:45:35.000000 mykit-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit/app/
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit/app/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/app/architecture/eventdriven.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/app/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/app/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit/app/complex/
--rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/app/complex/biplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/app/complex/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/app/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/app/slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit/kit/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/kit/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit/kit/fast_visualizations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit/kit/fast_visualizations/static/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/kit/fast_visualizations/static/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/kit/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit/kit/keycrate/
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/kit/keycrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/kit/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit/kit/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/kit/neuralnet/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/kit/neuralnet/genetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/kit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/kit/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/kit/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/kit/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit/rec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/rec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:35.000000 mykit-6.0.0/mykit/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 07:45:50.000000 mykit-6.0.0/mykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-05 07:45:35.000000 mykit-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 07:45:50.000000 mykit-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-05 07:45:35.000000 mykit-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-02 13:42:20.000000 mykit-6.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-02 13:42:27.000000 mykit-6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-02 13:42:20.000000 mykit-6.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/app/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/architecture/eventdriven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/app/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/complex/biplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/complex/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/kit/fast_visualizations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/kit/fast_visualizations/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/fast_visualizations/static/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/kit/keycrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/keycrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/kit/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/neuralnet/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/neuralnet/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/pLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/rec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/rec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 13:42:21.000000 mykit-6.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-02 13:42:27.000000 mykit-6.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 13:42:20.000000 mykit-6.2.0/setup.py
```

### Comparing `mykit-6.0.0/LICENSE` & `mykit-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/PKG-INFO` & `mykit-6.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 6.0.0
+Version: 6.2.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/mykit/docs
 Project-URL: Report bugs, https://github.com/nvfp/mykit/issues
```

### Comparing `mykit-6.0.0/README.md` & `mykit-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/__init__.py` & `mykit-6.2.0/mykit/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/__main__.py` & `mykit-6.2.0/mykit/__main__.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/app/__init__.py` & `mykit-6.2.0/mykit/app/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/app/architecture/eventdriven.py` & `mykit-6.2.0/mykit/app/architecture/eventdriven.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/app/arrow.py` & `mykit-6.2.0/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/app/button.py` & `mykit-6.2.0/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/app/complex/biplot.py` & `mykit-6.2.0/mykit/app/complex/biplot.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/app/complex/plot.py` & `mykit-6.2.0/mykit/app/complex/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/app/label.py` & `mykit-6.2.0/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/app/slider.py` & `mykit-6.2.0/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/kit/fast_visualizations/static/plot.py` & `mykit-6.2.0/mykit/kit/fast_visualizations/static/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/kit/ffmpeg.py` & `mykit-6.2.0/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/kit/keycrate/__init__.py` & `mykit-6.2.0/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/kit/math.py` & `mykit-6.2.0/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/kit/neuralnet/dense.py` & `mykit-6.2.0/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/kit/neuralnet/genetic.py` & `mykit-6.2.0/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/kit/noise.py` & `mykit-6.2.0/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/kit/path.py` & `mykit-6.2.0/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/kit/time.py` & `mykit-6.2.0/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-6.0.0/mykit/kit/utils.py` & `mykit-6.2.0/mykit/kit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,18 +103,19 @@
 def printer(__msg: str, /) -> None:
     """
     For simple logging needs.
     
     ---
 
     ## Demo
-    >>> printer('INFO: foo')  # [06:15:09] INFO: foo
+    >>> printer('INFO: foo')     # [06:15:09] INFO: foo
     >>> printer('WARNING: bar')  # [06:15:09] WARNING: bar
     """
-    print(f'[{_datetime.datetime.now().strftime("%H:%M:%S")}] {__msg}')
+    T = _datetime.datetime.now().strftime('%H:%M:%S')
+    print(f'[{T}] {__msg}')
 
 def slowprint(__msg: str, /, delay: float = 0.15) -> None:
     """
     For simple logging needs.
     Basically the same as `mykit.kit.utils.printer` but with delay.
 
     ---
@@ -127,15 +128,15 @@
     >>>     slowprint(f'INFO: {i}')
     >>> ## output:
     >>> ## [06:38:32] INFO: 0
     >>> ## [06:38:32] INFO: 1
     >>> ## [06:38:33] INFO: 2
     """
     _time.sleep(delay)
-    print(f'[{_datetime.datetime.now().strftime("%H:%M:%S")}] {__msg}')
+    printer(__msg)
 
 def print_screen(__msg: str, /) -> None:
     """prints message at the bottom of the terminal screen, adapting to terminal's height."""
 
     ## the height of users' terminal
     h = _os.get_terminal_size()[1]
```

### Comparing `mykit-6.0.0/mykit.egg-info/PKG-INFO` & `mykit-6.2.0/mykit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 6.0.0
+Version: 6.2.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/mykit/docs
 Project-URL: Report bugs, https://github.com/nvfp/mykit/issues
```

### Comparing `mykit-6.0.0/mykit.egg-info/SOURCES.txt` & `mykit-6.2.0/mykit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 mykit/app/architecture/eventdriven.py
 mykit/app/complex/biplot.py
 mykit/app/complex/plot.py
 mykit/kit/color.py
 mykit/kit/ffmpeg.py
 mykit/kit/math.py
 mykit/kit/noise.py
+mykit/kit/pLog.py
 mykit/kit/path.py
 mykit/kit/text.py
 mykit/kit/time.py
 mykit/kit/utils.py
 mykit/kit/fast_visualizations/static/plot.py
 mykit/kit/keycrate/__init__.py
 mykit/kit/neuralnet/dense.py
```

### Comparing `mykit-6.0.0/pyproject.toml` & `mykit-6.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "6.0.0"
+version = "6.2.0"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

