# Comparing `tmp/wise-pizza-0.1.9.tar.gz` & `tmp/wise-pizza-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wise-pizza-0.1.9.tar", last modified: Tue Jun 27 13:41:34 2023, max compression
+gzip compressed data, was "wise-pizza-0.2.0.tar", last modified: Wed Aug  2 09:03:02 2023, max compression
```

## Comparing `wise-pizza-0.1.9.tar` & `wise-pizza-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:41:34.163817 wise-pizza-0.1.9/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/LICENSE
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-27 13:41:34.163297 wise-pizza-0.1.9/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/README.md
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      220 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/pyproject.toml
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-06-27 13:41:34.163955 wise-pizza-0.1.9/setup.cfg
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-06-27 13:41:09.000000 wise-pizza-0.1.9/setup.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:41:34.133784 wise-pizza-0.1.9/tests/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7047 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/tests/test_fit.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:41:34.140942 wise-pizza-0.1.9/wise_pizza/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      118 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/__init__.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    11407 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/explain.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/find_alpha.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4745 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/make_matrix.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     9197 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/plotting.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      518 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/segment_data.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/slicer.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/solver.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-06-27 13:33:37.000000 wise-pizza-0.1.9/wise_pizza/utils.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-06-27 13:41:34.162560 wise-pizza-0.1.9/wise_pizza.egg-info/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-06-27 13:41:34.000000 wise-pizza-0.1.9/wise_pizza.egg-info/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      436 2023-06-27 13:41:34.000000 wise-pizza-0.1.9/wise_pizza.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-06-27 13:41:34.000000 wise-pizza-0.1.9/wise_pizza.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-06-27 13:41:34.000000 wise-pizza-0.1.9/wise_pizza.egg-info/requires.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-06-27 13:41:34.000000 wise-pizza-0.1.9/wise_pizza.egg-info/top_level.txt
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-08-02 09:03:02.472283 wise-pizza-0.2.0/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-08-02 08:30:31.000000 wise-pizza-0.2.0/LICENSE
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-08-02 09:03:02.472020 wise-pizza-0.2.0/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5678 2023-08-02 08:30:31.000000 wise-pizza-0.2.0/README.md
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      220 2023-08-02 08:30:31.000000 wise-pizza-0.2.0/pyproject.toml
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-08-02 09:03:02.472342 wise-pizza-0.2.0/setup.cfg
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-08-02 09:02:21.000000 wise-pizza-0.2.0/setup.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-08-02 09:03:02.464380 wise-pizza-0.2.0/wise_pizza/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      118 2023-08-02 08:30:31.000000 wise-pizza-0.2.0/wise_pizza/__init__.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    11448 2023-08-02 08:37:59.000000 wise-pizza-0.2.0/wise_pizza/explain.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-08-02 08:30:31.000000 wise-pizza-0.2.0/wise_pizza/find_alpha.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4745 2023-08-02 08:30:31.000000 wise-pizza-0.2.0/wise_pizza/make_matrix.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     9290 2023-08-02 08:39:55.000000 wise-pizza-0.2.0/wise_pizza/plotting.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      518 2023-08-02 08:30:31.000000 wise-pizza-0.2.0/wise_pizza/segment_data.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-08-02 08:30:31.000000 wise-pizza-0.2.0/wise_pizza/slicer.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-08-02 08:30:31.000000 wise-pizza-0.2.0/wise_pizza/solver.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-08-02 08:30:31.000000 wise-pizza-0.2.0/wise_pizza/utils.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-08-02 09:03:02.471633 wise-pizza-0.2.0/wise_pizza.egg-info/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6204 2023-08-02 09:03:02.000000 wise-pizza-0.2.0/wise_pizza.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-08-02 09:03:02.000000 wise-pizza-0.2.0/wise_pizza.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-08-02 09:03:02.000000 wise-pizza-0.2.0/wise_pizza.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-08-02 09:03:02.000000 wise-pizza-0.2.0/wise_pizza.egg-info/requires.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-08-02 09:03:02.000000 wise-pizza-0.2.0/wise_pizza.egg-info/top_level.txt
```

### Comparing `wise-pizza-0.1.9/LICENSE` & `wise-pizza-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.9/PKG-INFO` & `wise-pizza-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.9
+Version: 0.2.0
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wise-pizza-0.1.9/README.md` & `wise-pizza-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.9/setup.py` & `wise-pizza-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="wise-pizza",
-    version="0.1.9",
+    version="0.2.0",
     description="A library to find and visualise the most interesting slices in multidimensional data",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Wise",
     url='https://github.com/transferwise/wise-pizza',
     classifiers=[
         'Programming Language :: Python :: 3 :: Only',
```

### Comparing `wise-pizza-0.1.9/wise_pizza/explain.py` & `wise-pizza-0.2.0/wise_pizza/explain.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,12 +300,12 @@
     )
 
     for s in sf.segments:
         s["naive_avg"] += average
         s["total"] += average * s["seg_size"]
     # print(average)
     sf.reg.intercept_ = average
-    sf.plot = lambda plot_is_static=False, width=2000, height=500: plot_segments(
-        sf, plot_is_static=plot_is_static, width=width, height=height
+    sf.plot = lambda plot_is_static=False, width=2000, height=500, return_fig=False: plot_segments(
+        sf, plot_is_static=plot_is_static, width=width, height=height, return_fig=return_fig
     )
     sf.task = "levels"
     return sf
```

### Comparing `wise-pizza-0.1.9/wise_pizza/find_alpha.py` & `wise-pizza-0.2.0/wise_pizza/find_alpha.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.9/wise_pizza/make_matrix.py` & `wise-pizza-0.2.0/wise_pizza/make_matrix.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.9/wise_pizza/plotting.py` & `wise-pizza-0.2.0/wise_pizza/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 
 
 def plot_segments(
     sf: SliceFinder,
     plot_is_static: bool = False,
     width: int = 2000,
     height: int = 500,
+    return_fig: bool = False
 ):
     """
     Plot segments for explain_levels
     @param sf: SliceFinder
     @param plot_is_static: static (True) or dynamic (False) plotly result
     @param width: parameter to modify the final width of the plot
     @param height: parameter to modify the final height of the plot
@@ -206,15 +207,18 @@
         # Display the static image in the Jupyter notebook
         return Image(
             image_bytes,
             height=height + len(sf.segment_labels) * 30,
             width=width + len(sf.segment_labels) * 30,
         )
     else:
-        fig.show()
+        if return_fig:
+            return fig
+        else:
+            fig.show()
 
 
 def waterfall_args(sf: SliceFinder):
     """
     Waterfall plot arguments
     @param sf: SliceFinder
     """
```

### Comparing `wise-pizza-0.1.9/wise_pizza/segment_data.py` & `wise-pizza-0.2.0/wise_pizza/segment_data.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.9/wise_pizza/slicer.py` & `wise-pizza-0.2.0/wise_pizza/slicer.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.9/wise_pizza/solver.py` & `wise-pizza-0.2.0/wise_pizza/solver.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.9/wise_pizza/utils.py` & `wise-pizza-0.2.0/wise_pizza/utils.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.9/wise_pizza.egg-info/PKG-INFO` & `wise-pizza-0.2.0/wise_pizza.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.9
+Version: 0.2.0
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

