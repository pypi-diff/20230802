# Comparing `tmp/GTC-1.4.0.tar.gz` & `tmp/GTC-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GTC-1.4.0.tar", last modified: Mon Jul 18 23:46:02 2022, max compression
+gzip compressed data, was "GTC-1.4.1.tar", last modified: Wed Aug  2 04:12:59 2023, max compression
```

## Comparing `GTC-1.4.0.tar` & `GTC-1.4.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2022-07-18 23:46:02.895777 GTC-1.4.0/
--rw-rw-rw-   0        0        0       70 2020-12-23 20:56:03.000000 GTC-1.4.0/AUTHORS.rst
-drwxrwxrwx   0        0        0        0 2022-07-18 23:46:02.864542 GTC-1.4.0/GTC/
--rw-rw-rw-   0        0        0     6603 2021-01-14 23:37:50.000000 GTC-1.4.0/GTC/LU.py
--rw-rw-rw-   0        0        0     2950 2022-07-18 23:32:24.000000 GTC-1.4.0/GTC/__init__.py
--rw-rw-rw-   0        0        0    25673 2021-09-14 20:21:20.000000 GTC-1.4.0/GTC/archive.py
--rw-rw-rw-   0        0        0     5303 2022-04-18 21:15:23.000000 GTC-1.4.0/GTC/context.py
--rw-rw-rw-   0        0        0    40146 2022-07-18 23:31:33.000000 GTC-1.4.0/GTC/core.py
--rw-rw-rw-   0        0        0    26240 2022-07-18 23:31:33.000000 GTC-1.4.0/GTC/formatting.py
--rw-rw-rw-   0        0        0    15908 2022-04-18 21:15:23.000000 GTC-1.4.0/GTC/function.py
--rw-rw-rw-   0        0        0     6891 2021-01-14 23:37:50.000000 GTC-1.4.0/GTC/json_format.py
--rw-rw-rw-   0        0        0   158298 2022-07-18 23:31:33.000000 GTC-1.4.0/GTC/lib.py
--rw-rw-rw-   0        0        0    12039 2021-01-14 23:37:50.000000 GTC-1.4.0/GTC/linear_algebra.py
--rw-rw-rw-   0        0        0     5986 2022-07-18 23:31:33.000000 GTC-1.4.0/GTC/named_tuples.py
--rw-rw-rw-   0        0        0     1177 2021-09-14 20:21:20.000000 GTC-1.4.0/GTC/nodes.py
--rw-rw-rw-   0        0        0     6190 2021-05-13 22:40:45.000000 GTC-1.4.0/GTC/persistence.py
--rw-rw-rw-   0        0        0    37947 2022-07-18 23:31:33.000000 GTC-1.4.0/GTC/reporting.py
--rw-rw-rw-   0        0        0    49010 2022-04-18 21:15:23.000000 GTC-1.4.0/GTC/type_a.py
--rw-rw-rw-   0        0        0    37097 2022-04-18 21:15:23.000000 GTC-1.4.0/GTC/type_b.py
--rw-rw-rw-   0        0        0    33151 2022-07-18 23:31:33.000000 GTC-1.4.0/GTC/uncertain_array.py
--rw-rw-rw-   0        0        0    15416 2020-12-23 20:56:03.000000 GTC-1.4.0/GTC/vector.py
-drwxrwxrwx   0        0        0        0 2022-07-18 23:46:02.864542 GTC-1.4.0/GTC.egg-info/
--rw-rw-rw-   0        0        0     3770 2022-07-18 23:46:02.000000 GTC-1.4.0/GTC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1019 2022-07-18 23:46:02.000000 GTC-1.4.0/GTC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-18 23:46:02.000000 GTC-1.4.0/GTC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2022-07-18 23:46:02.000000 GTC-1.4.0/GTC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-07-18 23:46:02.000000 GTC-1.4.0/GTC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1125 2022-04-18 21:15:23.000000 GTC-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     3770 2022-07-18 23:46:02.895777 GTC-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2623 2022-04-18 21:15:23.000000 GTC-1.4.0/README.rst
--rw-rw-rw-   0        0        0      562 2022-07-18 23:46:02.895777 GTC-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     4876 2022-04-18 21:15:23.000000 GTC-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-18 23:46:02.895777 GTC-1.4.0/test/
--rw-rw-rw-   0        0        0     9418 2021-01-14 23:37:51.000000 GTC-1.4.0/test/test_LU.py
--rw-rw-rw-   0        0        0     1646 2022-04-18 21:15:23.000000 GTC-1.4.0/test/test_context.py
--rw-rw-rw-   0        0        0    19046 2021-09-14 20:21:20.000000 GTC-1.4.0/test/test_core.py
--rw-rw-rw-   0        0        0     4242 2021-05-13 22:40:45.000000 GTC-1.4.0/test/test_files_v_1_3_3.py
--rw-rw-rw-   0        0        0     4716 2021-09-14 20:21:20.000000 GTC-1.4.0/test/test_files_v_1_3_5.py
--rw-rw-rw-   0        0        0    51268 2022-04-18 21:15:23.000000 GTC-1.4.0/test/test_fitting.py
--rw-rw-rw-   0        0        0   121045 2022-07-18 23:31:33.000000 GTC-1.4.0/test/test_formatting.py
--rw-rw-rw-   0        0        0     9114 2021-01-14 23:37:51.000000 GTC-1.4.0/test/test_function.py
--rw-rw-rw-   0        0        0     2120 2021-06-29 21:51:54.000000 GTC-1.4.0/test/test_implicit.py
--rw-rw-rw-   0        0        0    54437 2022-04-18 21:15:23.000000 GTC-1.4.0/test/test_persistence.py
--rw-rw-rw-   0        0        0     9476 2021-09-14 20:21:20.000000 GTC-1.4.0/test/test_persistence_json.py
--rw-rw-rw-   0        0        0    24690 2022-07-18 23:31:33.000000 GTC-1.4.0/test/test_reporting.py
--rw-rw-rw-   0        0        0     9705 2021-01-14 23:40:23.000000 GTC-1.4.0/test/test_second_order_mul.py
--rw-rw-rw-   0        0        0    11422 2022-04-18 21:15:23.000000 GTC-1.4.0/test/test_sensitivity.py
--rw-rw-rw-   0        0        0    44908 2022-04-18 21:15:23.000000 GTC-1.4.0/test/test_type_a.py
--rw-rw-rw-   0        0        0   178090 2022-07-18 23:31:33.000000 GTC-1.4.0/test/test_uncertain_array.py
--rw-rw-rw-   0        0        0    93200 2022-07-18 23:31:33.000000 GTC-1.4.0/test/test_uncertain_complex.py
--rw-rw-rw-   0        0        0    14857 2020-12-23 20:56:04.000000 GTC-1.4.0/test/test_uncertain_complex_dof.py
--rw-rw-rw-   0        0        0    76359 2022-07-18 23:31:33.000000 GTC-1.4.0/test/test_uncertain_real.py
--rw-rw-rw-   0        0        0    12408 2020-12-23 20:56:04.000000 GTC-1.4.0/test/test_uncertain_real_dof.py
--rw-rw-rw-   0        0        0     7673 2020-12-23 20:56:04.000000 GTC-1.4.0/test/test_vector.py
--rw-rw-rw-   0        0        0     3604 2020-12-23 20:56:04.000000 GTC-1.4.0/test/testing_tools.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:12:59.664657 GTC-1.4.1/
+-rw-rw-rw-   0        0        0       70 2020-07-18 05:08:40.000000 GTC-1.4.1/AUTHORS.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 04:12:59.604650 GTC-1.4.1/GTC/
+-rw-rw-rw-   0        0        0     6603 2020-07-18 05:08:40.000000 GTC-1.4.1/GTC/LU.py
+-rw-rw-rw-   0        0        0     2950 2023-08-02 04:09:19.000000 GTC-1.4.1/GTC/__init__.py
+-rw-rw-rw-   0        0        0    25673 2022-02-11 03:41:11.000000 GTC-1.4.1/GTC/archive.py
+-rw-rw-rw-   0        0        0     5303 2022-02-24 01:02:02.000000 GTC-1.4.1/GTC/context.py
+-rw-rw-rw-   0        0        0    40146 2022-08-05 06:24:22.000000 GTC-1.4.1/GTC/core.py
+-rw-rw-rw-   0        0        0    26240 2022-08-05 06:24:22.000000 GTC-1.4.1/GTC/formatting.py
+-rw-rw-rw-   0        0        0    15908 2022-04-01 03:42:17.000000 GTC-1.4.1/GTC/function.py
+-rw-rw-rw-   0        0        0     6891 2020-09-18 05:29:37.000000 GTC-1.4.1/GTC/json_format.py
+-rw-rw-rw-   0        0        0   158298 2022-08-05 06:24:22.000000 GTC-1.4.1/GTC/lib.py
+-rw-rw-rw-   0        0        0    12039 2020-07-18 05:08:40.000000 GTC-1.4.1/GTC/linear_algebra.py
+-rw-rw-rw-   0        0        0     5986 2022-08-05 06:24:22.000000 GTC-1.4.1/GTC/named_tuples.py
+-rw-rw-rw-   0        0        0     1177 2022-02-11 03:41:11.000000 GTC-1.4.1/GTC/nodes.py
+-rw-rw-rw-   0        0        0     6190 2022-02-11 03:41:11.000000 GTC-1.4.1/GTC/persistence.py
+-rw-rw-rw-   0        0        0    37949 2023-08-02 04:06:58.000000 GTC-1.4.1/GTC/reporting.py
+-rw-rw-rw-   0        0        0    51161 2023-08-02 04:06:58.000000 GTC-1.4.1/GTC/type_a.py
+-rw-rw-rw-   0        0        0    37097 2022-04-01 03:42:17.000000 GTC-1.4.1/GTC/type_b.py
+-rw-rw-rw-   0        0        0    33151 2022-08-05 06:24:22.000000 GTC-1.4.1/GTC/uncertain_array.py
+-rw-rw-rw-   0        0        0    15416 2020-07-18 05:08:40.000000 GTC-1.4.1/GTC/vector.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:12:59.624649 GTC-1.4.1/GTC.egg-info/
+-rw-rw-rw-   0        0        0     3818 2023-08-02 04:12:59.000000 GTC-1.4.1/GTC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1019 2023-08-02 04:12:59.000000 GTC-1.4.1/GTC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 04:12:59.000000 GTC-1.4.1/GTC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-08-02 04:12:59.000000 GTC-1.4.1/GTC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-02 04:12:59.000000 GTC-1.4.1/GTC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1125 2023-08-02 04:06:58.000000 GTC-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0     3818 2023-08-02 04:12:59.664657 GTC-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2623 2023-08-02 04:06:58.000000 GTC-1.4.1/README.rst
+-rw-rw-rw-   0        0        0      562 2023-08-02 04:12:59.664657 GTC-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     4997 2023-08-02 04:06:58.000000 GTC-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:12:59.654649 GTC-1.4.1/test/
+-rw-rw-rw-   0        0        0     9418 2020-07-18 05:08:40.000000 GTC-1.4.1/test/test_LU.py
+-rw-rw-rw-   0        0        0     1646 2022-02-24 01:02:02.000000 GTC-1.4.1/test/test_context.py
+-rw-rw-rw-   0        0        0    19046 2022-02-11 03:41:11.000000 GTC-1.4.1/test/test_core.py
+-rw-rw-rw-   0        0        0     4242 2022-02-11 03:41:11.000000 GTC-1.4.1/test/test_files_v_1_3_3.py
+-rw-rw-rw-   0        0        0     4716 2022-02-11 03:41:11.000000 GTC-1.4.1/test/test_files_v_1_3_5.py
+-rw-rw-rw-   0        0        0    52344 2023-08-02 04:06:58.000000 GTC-1.4.1/test/test_fitting.py
+-rw-rw-rw-   0        0        0   121045 2022-08-05 06:24:22.000000 GTC-1.4.1/test/test_formatting.py
+-rw-rw-rw-   0        0        0     9114 2020-07-18 05:08:40.000000 GTC-1.4.1/test/test_function.py
+-rw-rw-rw-   0        0        0     2120 2022-02-11 03:41:11.000000 GTC-1.4.1/test/test_implicit.py
+-rw-rw-rw-   0        0        0    54437 2022-02-24 01:02:02.000000 GTC-1.4.1/test/test_persistence.py
+-rw-rw-rw-   0        0        0     9476 2022-02-11 03:41:11.000000 GTC-1.4.1/test/test_persistence_json.py
+-rw-rw-rw-   0        0        0    24690 2022-08-05 06:24:22.000000 GTC-1.4.1/test/test_reporting.py
+-rw-rw-rw-   0        0        0     9705 2022-02-11 03:41:11.000000 GTC-1.4.1/test/test_second_order_mul.py
+-rw-rw-rw-   0        0        0    11422 2022-04-01 03:42:17.000000 GTC-1.4.1/test/test_sensitivity.py
+-rw-rw-rw-   0        0        0    44908 2022-04-01 03:42:17.000000 GTC-1.4.1/test/test_type_a.py
+-rw-rw-rw-   0        0        0   178090 2023-08-02 04:03:41.000000 GTC-1.4.1/test/test_uncertain_array.py
+-rw-rw-rw-   0        0        0    93200 2022-08-05 06:24:22.000000 GTC-1.4.1/test/test_uncertain_complex.py
+-rw-rw-rw-   0        0        0    14857 2020-07-18 05:08:40.000000 GTC-1.4.1/test/test_uncertain_complex_dof.py
+-rw-rw-rw-   0        0        0    76359 2022-08-05 06:24:22.000000 GTC-1.4.1/test/test_uncertain_real.py
+-rw-rw-rw-   0        0        0    12408 2020-07-18 05:08:40.000000 GTC-1.4.1/test/test_uncertain_real_dof.py
+-rw-rw-rw-   0        0        0     7673 2020-07-18 05:08:40.000000 GTC-1.4.1/test/test_vector.py
+-rw-rw-rw-   0        0        0     3604 2020-07-18 05:08:40.000000 GTC-1.4.1/test/testing_tools.py
```

### Comparing `GTC-1.4.0/GTC/LU.py` & `GTC-1.4.1/GTC/LU.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/__init__.py` & `GTC-1.4.1/GTC/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,14 @@
         'GTC 2.0 will require Python 3.7, or above. '
         'Please update your version of Python.' % sys.version_info[:2],
         DeprecationWarning,
         stacklevel=2
     )
     del warnings
 #----------------------------------------------------------------------------
-version = "1.4.0"
+version = "1.4.1"
 
-copyright = """Copyright (c) 2022, \
+copyright = """Copyright (c) 2023, \
 Measurement Standards Laboratory of New Zealand"""
 
 from .core import *
 from .formatting import *
```

### Comparing `GTC-1.4.0/GTC/archive.py` & `GTC-1.4.1/GTC/archive.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/context.py` & `GTC-1.4.1/GTC/context.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/core.py` & `GTC-1.4.1/GTC/core.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/formatting.py` & `GTC-1.4.1/GTC/formatting.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/function.py` & `GTC-1.4.1/GTC/function.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/json_format.py` & `GTC-1.4.1/GTC/json_format.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/lib.py` & `GTC-1.4.1/GTC/lib.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/linear_algebra.py` & `GTC-1.4.1/GTC/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/named_tuples.py` & `GTC-1.4.1/GTC/named_tuples.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/nodes.py` & `GTC-1.4.1/GTC/nodes.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/persistence.py` & `GTC-1.4.1/GTC/persistence.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/reporting.py` & `GTC-1.4.1/GTC/reporting.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     Evaluates a number of degrees-of-freedom given a coverage 
     factor for an elliptical uncertainty region with coverage 
     probability ``p`` based on the F-distribution.
     
     **Example**::
 
         >>> reporting.k2_to_dof(2.6,95)
-        34.35788424389927
+        34.3578842438992...
         
     """
     if k2 <= 0:
         raise RuntimeError( "invalid k:  {}".format(k2) ) 
     if p <= 0 or p >= 100:
         raise RuntimeError( "invalid p: {}".format(p) )
     else:
```

### Comparing `GTC-1.4.0/GTC/type_a.py` & `GTC-1.4.1/GTC/type_a.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 Merging uncertain components
 ----------------------------
     *   :func:`merge` combines results from a type-A and type-B analysis 
         of the same data. 
  
 .. note::
 
-    Many functions in :mod:`type_a` treat  data as pure numbers. 
+    Many functions in :mod:`type_a` treat data as pure numbers. 
     Sequences of uncertain numbers can be passed to these 
     functions, but only the uncertain-number values will be used.
     
-    :func:`merge` is provided so that the results of 
-    type-A and type-B analyses on the same data can be 
-    combined. 
+    :func:`merge` is provided so that the results of type-A 
+    and type-B analyses on the same data can be combined. 
+    
 
 Module contents
 ---------------
 
 """
 from __future__ import division
 
@@ -135,15 +135,15 @@
 '''
         return header + LineFit.__str__(self)
 
     def x_from_y(self,yseq,x_label=None,y_label=None):
         """Estimate the stimulus ``x`` corresponding to the responses in ``yseq``
 
         :arg yseq: a sequence of ``y`` observations 
-        :arg x_label: a label for the return uncertain number `x` 
+        :arg x_label: a label for the return uncertain number ``x`` 
         :arg y_label: a label for the estimate of `y` based on ``yseq`` 
 
         .. note::
             When ``x_label`` is defined, the uncertain number returned will be 
             declared an intermediate result (using :func:`~.result`)
 
         **Example** ::
@@ -156,16 +156,16 @@
             >>> fit = type_a.line_fit(x_data,y_data)
             
             >>> x0 = fit.x_from_y( [0.0712, 0.0716] )            
             >>> x0
             ureal(0.2601659751037...,0.01784461112558...,13.0)
 
         """
-        df = self._N - 2       
         a, b = self._a_b
+        df = a.df
 
         p = len(yseq)
         y = math.fsum( yseq ) / p
         
         y = ureal(
             y,
             math.sqrt( self._ssr/df/p ),
@@ -204,15 +204,15 @@
 
         .. note::
             When ``y_label`` is defined, the uncertain number returned will be 
             declared an intermediate result (using :func:`~.result`)
         
         """
         a, b = self._a_b   
-        df = self._N - 2
+        df = a.df 
         
         u = math.sqrt( self._ssr/df )
         
         noise = ureal(
             0,u,df,label=s_label,independent=False
         )
         
@@ -254,16 +254,16 @@
         :arg y_label: a label for the estimate of `y` based on ``yseq``
 
         .. note::
             When ``x_label`` is defined, the uncertain number returned will be 
             declared an intermediate result (using :func:`~.result`)
 
         """
-        df = self._N - 2       
         a, b = self._a_b
+        df = a.df 
         
         p = len(yseq)
         y = math.fsum( yseq ) / p
         
         y = ureal(
             y,
             s_y * math.sqrt( self._ssr/df/p ),
@@ -308,15 +308,15 @@
         
         .. note::
             When ``y_label`` is defined, the uncertain number returned will be 
             declared an intermediate result (using :func:`~.result`)
 
         """
         a, b = self._a_b   
-        df = self._N - 2
+        df = a.df 
         
         u = math.sqrt( s_y*self._ssr/df )
         
         noise = ureal(0,u,df,label=s_label)
 
         append_real_ensemble(a,noise)
                   
@@ -361,22 +361,23 @@
         
         .. note::
             When ``x_label`` is defined, the uncertain number returned will be 
             declared an intermediate result (using :func:`~.result`)
 
         """
         a, b = self._a_b
+        df = a.df
         
         p = len(y_data)
         y = math.fsum( y_data ) / p
         
         y = ureal(
             y,
             u_y_data / math.sqrt( p ),
-            inf,
+            df,
             label=y_label,
             independent=False
         )            
 
         append_real_ensemble(a,y)
 
         if abs(b) < 1E-15:
@@ -409,15 +410,15 @@
         
         .. note::
             When ``y_label`` is defined, the uncertain number returned will be 
             declared an intermediate result (using :func:`~.result`)
 
         """
         a, b = self._a_b   
-        df = self.N - 2
+        df = a.df 
         
         noise = ureal(0,s_y,df,label=s_label)
 
         append_real_ensemble(a,noise)
                   
         if y_label is None:
             y = a + b*x + noise
@@ -426,16 +427,14 @@
         
         return y
         
 #-----------------------------------------------------------------------------------------
 def line_fit(x,y,label=None):
     """Return a least-squares straight-line fit to the data
      
-    .. versionadded:: 1.2
-    
     :arg x:     sequence of stimulus data (independent-variable)  
     :arg y:     sequence of response data (dependent-variable)  
     :arg label: suffix to label the uncertain numbers `a` and `b`
 
     :returns:   an object containing regression results
     :rtype:     :class:`.LineFitOLS`
 
@@ -451,15 +450,17 @@
         ureal(4.8138888888888...,4.8862063121833...,7)
         >>> b
         ureal(9.4083333333333...,0.8683016476563...,7)
 
         >>> y_p = a + b*5.5
         >>> dof(y_p)
         7.0
-            
+ 
+    .. versionadded:: 1.2    
+ 
     """
     N = len(x)
     df = N-2
     if df <= 0 or N != len(y):
         raise RuntimeError(
             "Invalid sequences: len({!r}), len({!r})".format(x,y)
         )
@@ -538,88 +539,113 @@
     
     f = lambda x_i,y_i,u_y_i: ((y_i - a_ - b_*x_i)/u_y_i)**2 
     ssr =  math.fsum( f(x_i,y_i,u_y_i) for x_i,y_i,u_y_i in izip(x,y,u_y) )
 
     return a_,b_,siga,sigb,r_ab,ssr,N
 
 #-----------------------------------------------------------------------------------------
-def line_fit_wls(x,y,u_y,label=None):
+def line_fit_wls(x,y,u_y,dof=None,label=None):
     """Return a weighted least-squares straight-line fit
     
-    .. versionadded:: 1.2
-     
     :arg x:     sequence of stimulus data (independent-variable)  
     :arg y:     sequence of response data (dependent-variable)  
     :arg u_y:   sequence of uncertainties in the response data 
+    :arg dof:   degrees of freedom
     :arg label: suffix to label the uncertain numbers `a` and `b`
 
     :returns:   an object containing regression results
     :rtype:     :class:`.LineFitWLS`
+    
+    The optional argument ``dof`` can be used to choose the number of 
+    degrees of freedom attributed to the uncertain numbers
+    returned for the slope and intercept. By default, infinite degrees 
+    of freedom is used, because weighting is provided for the 
+    ``y`` data suggesting that the dispersion is known. 
 
     **Example**::
     
         >>> x = [1,2,3,4,5,6]
         >>> y = [3.2, 4.3, 7.6, 8.6, 11.7, 12.8]
         >>> u_y = [0.5,0.5,0.5,1.0,1.0,1.0]
         
         >>> fit = type_a.line_fit_wls(x,y,u_y)
         >>> fit.a_b     
          InterceptSlope(a=ureal(0.8852320675105...,0.5297081435088...,inf),
          b=ureal(2.056962025316...,0.177892016741...,inf))
-        
+
+    .. versionchanged:: 1.4.1 ``dof`` keyword argument added
+    .. versionadded:: 1.2
+     
     """
     N = len(x)
     if N-2 <= 0 or N != len(y) or N != len(u_y):
         raise RuntimeError(
             "Invalid sequences: len({!r}), len({!r}), len({!r})".format(x,y,u_y)
         )
         
     x = value_seq(x)
     y = value_seq(y)
 
     a_,b_,siga,sigb,r_ab,ssr,N = _line_fit_wls(x,y,u_y)
     
+    if dof is None:
+        df = inf 
+    else:
+        if isinstance(dof,numbers.Number) and dof > 0:
+            df = dof
+        else:
+            raise RuntimeError( 
+                "{!r} is an invalid degrees of freedom".format(dof) 
+            )
+    
     a = ureal(
         a_,
         siga,
-        inf,
+        df,
         label='a_{}'.format(label) if label is not None else None,
         independent=False
     )
     b = ureal(
         b_,
         sigb,
-        inf,
+        df,
         label='b_{}'.format(label) if label is not None else None,
         independent=False
-    )
-    
+    )    
+
+    real_ensemble( (a,b), df )
     a.set_correlation(r_ab,b)
 
     return LineFitWLS(a,b,ssr,N)
 
 #-----------------------------------------------------------------------------------------
-def line_fit_rwls(x,y,s_y,label=None):
+def line_fit_rwls(x,y,s_y,dof=None,label=None):
     """Return a relative weighted least-squares straight-line fit
     
-    .. versionadded:: 1.2
-    
     The ``s_y`` values are used to scale variability in the ``y`` data.
     It is assumed that the standard deviation of each ``y`` value is 
     proportional to the corresponding ``s_y`` scale factor.
     The unknown common factor in the uncertainties is estimated from the residuals.
     
     :arg x:     sequence of stimulus data (independent-variable)  
     :arg y:     sequence of response data (dependent-variable)  
     :arg s_y:   sequence of scale factors
+    :arg dof:   degrees of freedom
     :arg label: suffix to label the uncertain numbers `a` and `b`
 
     :returns:   an object containing regression results
     :rtype:     :class:`.LineFitRWLS`
 
+    The optional argument ``dof`` can be used to choose the number of 
+    degrees of freedom attributed to the uncertain numbers
+    returned for the slope and intercept. By default, the degrees 
+    of freedom is N - 2, where N is the length of the data sequence.
+    However, when the elements of ``s_y`` are not all equal this 
+    value will be too high. The argument may be set as appropriate.
+    
     **Example**::
 
         >>> x = [1,2,3,4,5,6]
         >>> y = [3.014,5.225,7.004,9.061,11.201,12.762]
         >>> s_y = [0.2,0.2,0.2,0.4,0.4,0.4]
         >>> fit = type_a.line_fit_rwls(x,y,s_y)
         >>> a, b = fit.a_b
@@ -630,19 +656,31 @@
         <BLANKLINE>
           Intercept: 1.14(12)
           Slope: 1.973(41)
           Correlation: -0.87
           Sum of the squared residuals: 1.3395217958...
           Number of points: 6
         <BLANKLINE>
-          
+ 
+    .. versionchanged:: 1.4.1 ``dof`` keyword argument added
+    .. versionadded:: 1.2
+        
     """
     N = len(x)
-    df = N-2
-    if df <= 0 or N != len(y) or N != len(s_y):
+    if dof is None:
+        df = N-2 
+    else:
+        if isinstance(dof,numbers.Number) and dof > 0:
+            df = dof
+        else:
+            raise RuntimeError( 
+                "{!r} is an invalid degrees of freedom".format(dof) 
+            )
+    
+    if N != len(y) or N != len(s_y):
         raise RuntimeError(
             "Invalid sequences: len({!r}), len({!r}), len({!r})".format(x,y,s_y)
         )
         
     x = value_seq(x)
     y = value_seq(y)
     
@@ -670,32 +708,37 @@
     real_ensemble( (a,b), df )
     a.set_correlation(r_ab,b)
 
     return LineFitRWLS(a,b,ssr,N)
     
 #--------------------------------------------------------------------
 #
-def line_fit_wtls(x,y,u_x,u_y,a0_b0=None,r_xy=None,label=None):
+def line_fit_wtls(x,y,u_x,u_y,a0_b0=None,r_xy=None,dof=None,label=None):
     """Return a total least-squares straight-line fit 
     
-    .. versionadded:: 1.2
-
     :arg x:     sequence of independent-variable data
     :arg y:     sequence of dependent-variable data 
     :arg u_x:   sequence of uncertainties in ``x``
     :arg u_y:   sequence of uncertainties in ``y``
     :arg a0_b0: a pair of initial estimates for the intercept and slope
     :arg r_xy:  correlation between x-y pairs
+    :arg dof:   degrees of freedom
     :arg label: suffix labeling the uncertain numbers `a` and `b`
 
     :returns:   an object containing the fitting results
     :rtype:     :class:`.LineFitWTLS`
 
     The optional argument ``a_b`` can be used to provide a pair 
     of initial estimates for the intercept and slope. 
+    
+    The optional argument ``dof`` can be used to choose the number of 
+    degrees of freedom attributed to the uncertain numbers
+    returned for the slope and intercept. By default, the degrees 
+    of freedom are infinite, because weighting is provided for the ``x``
+    and ``y`` data suggesting that the dispersion is known. 
 
     Based on paper by M Krystek and M Anton,
     *Meas. Sci. Technol.* **22** (2011) 035101 (9pp)
     
     **Example**::
 
         # Pearson-York test data see, e.g., 
@@ -709,22 +752,34 @@
         # standard uncertainties required for weighting
         >>> ux=[1./math.sqrt(wx_i) for wx_i in wx ]
         >>> uy=[1./math.sqrt(wy_i) for wy_i in wy ]
 
         >>> result = ta.line_fit_wtls(x,y,ux,uy)
         >>> intercept, slope = result.a_b
         >>> intercept
-        ureal(5.47991018...,0.29193349...,8)
+        ureal(5.47991018...,0.29193349...,inf)
         >>> slope
-        ureal(-0.48053339...,0.057616740...,8)
-    
+        ureal(-0.48053339...,0.057616740...,inf)
+
+    .. versionchanged:: 1.4.1 ``dof`` keyword argument added
+    .. versionadded:: 1.2    
+
     """
     N = len(x)
-    df = N-2
-    if df <= 0 or N != len(y):
+    if dof is None:
+        df = inf 
+    else:
+        if isinstance(dof,numbers.Number) and dof > 0:
+            df = dof
+        else:
+            raise RuntimeError( 
+                "{!r} is an invalid degrees of freedom".format(dof) 
+            )
+    
+    if N != len(y):
         raise RuntimeError(
             "Invalid sequences: len({!r}), len({!r})".format(x,y)
         )
     if N != len(u_x) or N != len(u_y):
         raise RuntimeError(
             "Invalid sequences: len({!r}), len({!r})".format(u_x,u_y)
         )
```

### Comparing `GTC-1.4.0/GTC/type_b.py` & `GTC-1.4.1/GTC/type_b.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/uncertain_array.py` & `GTC-1.4.1/GTC/uncertain_array.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC/vector.py` & `GTC-1.4.1/GTC/vector.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/GTC.egg-info/PKG-INFO` & `GTC-1.4.1/GTC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GTC
-Version: 1.4.0
+Version: 1.4.1
 Summary: The GUM Tree Calculator for Python
 Home-page: https://github.com/MSLNZ/GTC
 Author: Measurement Standards Laboratory of New Zealand
 Author-email: info@measurement.govt.nz
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 License-File: AUTHORS.rst
 
@@ -88,21 +89,19 @@
 * `scipy <https://www.scipy.org/>`_
 
 Documentation
 =============
 
 The documentation for **GTC** can be found `here <https://gtc.readthedocs.io/en/stable/>`_.
 
-.. |docs| image:: https://readthedocs.org/projects/gtc/badge/?version=stable
+.. |docs| image:: https://readthedocs.org/projects/gtc/badge/?version=latest
     :target: https://gtc.readthedocs.io/en/stable/
     :alt: Documentation Status
 
 .. |github tests| image:: https://github.com/MSLNZ/GTC/actions/workflows/run-tests.yml/badge.svg
    :target: https://github.com/MSLNZ/GTC/actions/workflows/run-tests.yml
 
 .. |pypi| image:: https://badge.fury.io/py/GTC.svg
     :target: https://badge.fury.io/py/GTC
 
 .. |zenodo| image:: https://zenodo.org/badge/147150740.svg
    :target: https://zenodo.org/badge/latestdoi/147150740
-
-
```

### Comparing `GTC-1.4.0/GTC.egg-info/SOURCES.txt` & `GTC-1.4.1/GTC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/LICENSE` & `GTC-1.4.1/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Measurement Standards Laboratory of New Zealand
+Copyright (c) 2023 Measurement Standards Laboratory of New Zealand
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `GTC-1.4.0/PKG-INFO` & `GTC-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GTC
-Version: 1.4.0
+Version: 1.4.1
 Summary: The GUM Tree Calculator for Python
 Home-page: https://github.com/MSLNZ/GTC
 Author: Measurement Standards Laboratory of New Zealand
 Author-email: info@measurement.govt.nz
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 License-File: AUTHORS.rst
 
@@ -88,21 +89,19 @@
 * `scipy <https://www.scipy.org/>`_
 
 Documentation
 =============
 
 The documentation for **GTC** can be found `here <https://gtc.readthedocs.io/en/stable/>`_.
 
-.. |docs| image:: https://readthedocs.org/projects/gtc/badge/?version=stable
+.. |docs| image:: https://readthedocs.org/projects/gtc/badge/?version=latest
     :target: https://gtc.readthedocs.io/en/stable/
     :alt: Documentation Status
 
 .. |github tests| image:: https://github.com/MSLNZ/GTC/actions/workflows/run-tests.yml/badge.svg
    :target: https://github.com/MSLNZ/GTC/actions/workflows/run-tests.yml
 
 .. |pypi| image:: https://badge.fury.io/py/GTC.svg
     :target: https://badge.fury.io/py/GTC
 
 .. |zenodo| image:: https://zenodo.org/badge/147150740.svg
    :target: https://zenodo.org/badge/latestdoi/147150740
-
-
```

### Comparing `GTC-1.4.0/README.rst` & `GTC-1.4.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 * `scipy <https://www.scipy.org/>`_
 
 Documentation
 =============
 
 The documentation for **GTC** can be found `here <https://gtc.readthedocs.io/en/stable/>`_.
 
-.. |docs| image:: https://readthedocs.org/projects/gtc/badge/?version=stable
+.. |docs| image:: https://readthedocs.org/projects/gtc/badge/?version=latest
     :target: https://gtc.readthedocs.io/en/stable/
     :alt: Documentation Status
 
 .. |github tests| image:: https://github.com/MSLNZ/GTC/actions/workflows/run-tests.yml/badge.svg
    :target: https://github.com/MSLNZ/GTC/actions/workflows/run-tests.yml
 
 .. |pypi| image:: https://badge.fury.io/py/GTC.svg
```

### Comparing `GTC-1.4.0/setup.cfg` & `GTC-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/setup.py` & `GTC-1.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,16 +96,16 @@
 ]
 tests_require = [
     'pytest>=4.4',  # >=4.4 to support the "-p conftest" option
     'pytest-cov',
 ]
 
 docs_require = [
-    'sphinx',
-    'sphinx_rtd_theme',
+    'sphinx>2',  # >2 required for ReadTheDocs
+    'sphinx-rtd-theme>0.5',  # >0.5 required for ReadTheDocs
 ]
 
 testing = {'test', 'tests', 'pytest'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if testing else []
 
 needs_sphinx = {'doc', 'docs', 'apidoc', 'apidocs', 'build_sphinx'}.intersection(sys.argv)
 sphinx = docs_require + install_requires if needs_sphinx else []
@@ -132,14 +132,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development',
         'Topic :: Scientific/Engineering',
     ],
     setup_requires=sphinx + pytest_runner,
     tests_require=tests_require,
     install_requires=install_requires,
     extras_require={'tests': tests_require, 'docs': docs_require},
```

### Comparing `GTC-1.4.0/test/test_LU.py` & `GTC-1.4.1/test/test_LU.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_context.py` & `GTC-1.4.1/test/test_context.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_core.py` & `GTC-1.4.1/test/test_core.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_files_v_1_3_3.py` & `GTC-1.4.1/test/test_files_v_1_3_3.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_files_v_1_3_5.py` & `GTC-1.4.1/test/test_files_v_1_3_5.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_fitting.py` & `GTC-1.4.1/test/test_fitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,24 @@
         self.assertTrue( equivalent(a.x,1.13754,1E-5))
         self.assertTrue( equivalent(b.x,1.97264,1E-5))
         self.assertTrue( equivalent(a.u,0.12261,1E-5))
         self.assertTrue( equivalent(b.u,0.04118,1E-5))
         self.assertTrue( equivalent(a.u*b.u*a.get_correlation(b),-0.004408553,1E-5))
         self.assertEqual(a.df,len(x)-2)
         self.assertEqual(b.df,len(x)-2)
+        
+        # Try to set a number of degrees of freedom
+        fit = type_a.line_fit_rwls(x,y,u_y,dof=4)
+        a, b = fit.a_b
+        self.assertEqual(a.df,4)
+        self.assertEqual(b.df,4)
  
+        # Try to set an illegal number of degrees of freedom
+        self.assertRaises(RuntimeError,type_a.line_fit_rwls,x,y,u_y,dof=0)
+
     def test_type_b(self):
         """
         We can treat the problem above as type-B. In that
         case, the y uncertainties are the weights. We do 
         not expect the same uncertainties. 
         
         The R commands are:
@@ -272,14 +281,23 @@
 
         x0 = fit.x_from_y([10.5],0.5)
         self.assertTrue( not x0.is_intermediate )
         self.assertTrue( equivalent(x0.x,4.913,TOL) )
         self.assertTrue( equivalent(x0.u,0.322,TOL) )
         self.assertEqual( x0.df,inf )
 
+        # Try to set a number of degrees of freedom
+        fit = type_a.line_fit_wls(x,y,u_y,dof=4)
+        a, b = fit.a_b
+        self.assertEqual(a.df,4)
+        self.assertEqual(b.df,4)
+ 
+        # Try to set an illegal number of degrees of freedom
+        self.assertRaises(RuntimeError,type_a.line_fit_wls,x,y,u_y,dof=0)
+
     def test_iso28037_wls2(self):
         """ ISO/TS 28037:2010, p 14
 
         Better numbers using R:
         
             fit <- lm(y~x,wieghts=w)
             fit.sum <- summary(fit)
@@ -1174,14 +1192,27 @@
         self.assertTrue( equivalent(a.x,0.5788,TOL) )
         self.assertTrue( equivalent(a.u,0.4764,TOL) )  # This is the critical case for TOL
         self.assertTrue( equivalent(b.x,2.1597,TOL) )
         self.assertTrue( equivalent(b.u,0.1355,TOL) )
         self.assertTrue( equivalent(a.get_correlation(b)*b.u*a.u,-0.0577,TOL) )
         self.assertTrue( equivalent(fit.ssr,2.743,TOL) )
   
+        # Test with finite degrees of freedom
+        fit = type_a.line_fit_wtls(x, y, u_x=[u_x]*6, u_y=u_y, dof=4)
+        a, b = fit.a_b
+        self.assertEqual(a.df,4)
+        self.assertEqual(b.df,4)
+        
+        self.assertRaises(
+            RuntimeError,
+            type_a.line_fit_wtls, 
+            x, y, u_x=[u_x]*6, u_y=u_y, 
+            dof=0
+        )
+        
     def test_Lybanon_fn(self):
         """
         Test the WTLS method on the Pearson-York data.
         This does not test the correlations between x-y pairs.
         The the a and b uncertainty values come from
         A H Kalantar, Meas Sci Technol. 3 (1992) 1113
```

### Comparing `GTC-1.4.0/test/test_formatting.py` & `GTC-1.4.1/test/test_formatting.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_function.py` & `GTC-1.4.1/test/test_function.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_implicit.py` & `GTC-1.4.1/test/test_implicit.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_persistence.py` & `GTC-1.4.1/test/test_persistence.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_persistence_json.py` & `GTC-1.4.1/test/test_persistence_json.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_reporting.py` & `GTC-1.4.1/test/test_reporting.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_second_order_mul.py` & `GTC-1.4.1/test/test_second_order_mul.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_sensitivity.py` & `GTC-1.4.1/test/test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_type_a.py` & `GTC-1.4.1/test/test_type_a.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_uncertain_array.py` & `GTC-1.4.1/test/test_uncertain_array.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_uncertain_complex.py` & `GTC-1.4.1/test/test_uncertain_complex.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_uncertain_complex_dof.py` & `GTC-1.4.1/test/test_uncertain_complex_dof.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_uncertain_real.py` & `GTC-1.4.1/test/test_uncertain_real.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_uncertain_real_dof.py` & `GTC-1.4.1/test/test_uncertain_real_dof.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/test_vector.py` & `GTC-1.4.1/test/test_vector.py`

 * *Files identical despite different names*

### Comparing `GTC-1.4.0/test/testing_tools.py` & `GTC-1.4.1/test/testing_tools.py`

 * *Files identical despite different names*

