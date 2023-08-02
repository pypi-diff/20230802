# Comparing `tmp/KKMeans-0.0.6.tar.gz` & `tmp/KKMeans-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KKMeans-0.0.6.tar", last modified: Mon Jul 31 23:17:10 2023, max compression
+gzip compressed data, was "KKMeans-0.0.7.tar", last modified: Wed Aug  2 10:33:07 2023, max compression
```

## Comparing `KKMeans-0.0.6.tar` & `KKMeans-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 23:17:10.862546 KKMeans-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-07-31 23:17:10.837993 KKMeans-0.0.6/KKMeans.egg-info/
--rw-rw-rw-   0        0        0      618 2023-07-31 23:17:10.000000 KKMeans-0.0.6/KKMeans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      639 2023-07-31 23:17:10.000000 KKMeans-0.0.6/KKMeans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 23:17:10.000000 KKMeans-0.0.6/KKMeans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-31 23:17:10.000000 KKMeans-0.0.6/KKMeans.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 23:17:10.000000 KKMeans-0.0.6/KKMeans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      618 2023-07-31 23:17:10.862027 KKMeans-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-31 12:26:00.000000 KKMeans-0.0.6/README.md
--rw-rw-rw-   0        0        0     1086 2023-07-31 11:30:04.000000 KKMeans-0.0.6/license.txt
--rw-rw-rw-   0        0        0      521 2023-07-31 23:16:26.000000 KKMeans-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 23:17:10.863053 KKMeans-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1663 2023-07-31 12:13:21.000000 KKMeans-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 23:17:10.815519 KKMeans-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 23:17:10.859978 KKMeans-0.0.6/src/KKMeans/
--rw-rw-rw-   0        0        0   875796 2023-07-31 11:49:59.000000 KKMeans-0.0.6/src/KKMeans/KKMeans.c
--rw-rw-rw-   0        0        0    27233 2023-07-31 11:36:19.000000 KKMeans-0.0.6/src/KKMeans/KKMeans.py
--rw-rw-rw-   0        0        0       28 2023-07-31 23:15:44.000000 KKMeans-0.0.6/src/KKMeans/__init__.py
--rw-rw-rw-   0        0        0  1170842 2023-07-31 23:17:09.000000 KKMeans-0.0.6/src/KKMeans/elkan.c
--rw-rw-rw-   0        0        0     9984 2023-07-31 16:04:53.000000 KKMeans-0.0.6/src/KKMeans/elkan.pyx
--rw-rw-rw-   0        0        0  1182482 2023-07-31 23:17:09.000000 KKMeans-0.0.6/src/KKMeans/kernels.c
--rw-rw-rw-   0        0        0     6892 2023-07-29 08:20:16.000000 KKMeans-0.0.6/src/KKMeans/kernels.pyx
--rw-rw-rw-   0        0        0  1022846 2023-07-29 08:23:01.000000 KKMeans-0.0.6/src/KKMeans/lloyd.c
--rw-rw-rw-   0        0        0     3427 2023-07-29 08:20:16.000000 KKMeans-0.0.6/src/KKMeans/lloyd.pyx
--rw-rw-rw-   0        0        0  1004899 2023-07-31 11:50:00.000000 KKMeans-0.0.6/src/KKMeans/quality.c
--rw-rw-rw-   0        0        0     1966 2023-07-31 11:38:16.000000 KKMeans-0.0.6/src/KKMeans/quality.pyx
--rw-rw-rw-   0        0        0  1091399 2023-07-29 08:23:02.000000 KKMeans-0.0.6/src/KKMeans/utils.c
--rw-rw-rw-   0        0        0     5309 2023-07-29 08:20:16.000000 KKMeans-0.0.6/src/KKMeans/utils.pyx
-drwxrwxrwx   0        0        0        0 2023-07-31 23:17:10.861000 KKMeans-0.0.6/tests/
--rw-rw-rw-   0        0        0     1472 2023-07-31 17:53:20.000000 KKMeans-0.0.6/tests/test_pytest_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:33:07.037694 KKMeans-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-08-02 10:33:07.001921 KKMeans-0.0.7/KKMeans.egg-info/
+-rw-rw-rw-   0        0        0     1171 2023-08-02 10:33:06.000000 KKMeans-0.0.7/KKMeans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      639 2023-08-02 10:33:06.000000 KKMeans-0.0.7/KKMeans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:33:06.000000 KKMeans-0.0.7/KKMeans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-02 10:33:06.000000 KKMeans-0.0.7/KKMeans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 10:33:06.000000 KKMeans-0.0.7/KKMeans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1171 2023-08-02 10:33:07.037180 KKMeans-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-08-01 21:43:50.000000 KKMeans-0.0.7/README.md
+-rw-rw-rw-   0        0        0     1086 2023-07-31 11:30:04.000000 KKMeans-0.0.7/license.txt
+-rw-rw-rw-   0        0        0      521 2023-08-02 10:30:04.000000 KKMeans-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 10:33:07.037694 KKMeans-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1663 2023-07-31 12:13:21.000000 KKMeans-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:33:06.977872 KKMeans-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 10:33:07.029512 KKMeans-0.0.7/src/KKMeans/
+-rw-rw-rw-   0        0        0   875796 2023-08-02 10:32:14.000000 KKMeans-0.0.7/src/KKMeans/KKMeans.c
+-rw-rw-rw-   0        0        0    27233 2023-08-01 21:49:50.000000 KKMeans-0.0.7/src/KKMeans/KKMeans.py
+-rw-rw-rw-   0        0        0      122 2023-08-01 18:06:49.000000 KKMeans-0.0.7/src/KKMeans/__init__.py
+-rw-rw-rw-   0        0        0  1171323 2023-08-02 10:33:04.000000 KKMeans-0.0.7/src/KKMeans/elkan.c
+-rw-rw-rw-   0        0        0    10024 2023-08-02 10:32:48.000000 KKMeans-0.0.7/src/KKMeans/elkan.pyx
+-rw-rw-rw-   0        0        0  1182482 2023-08-02 10:33:05.000000 KKMeans-0.0.7/src/KKMeans/kernels.c
+-rw-rw-rw-   0        0        0     6892 2023-08-01 21:47:36.000000 KKMeans-0.0.7/src/KKMeans/kernels.pyx
+-rw-rw-rw-   0        0        0  1022804 2023-08-02 10:33:05.000000 KKMeans-0.0.7/src/KKMeans/lloyd.c
+-rw-rw-rw-   0        0        0     3427 2023-08-01 21:47:44.000000 KKMeans-0.0.7/src/KKMeans/lloyd.pyx
+-rw-rw-rw-   0        0        0  1004899 2023-07-31 11:50:00.000000 KKMeans-0.0.7/src/KKMeans/quality.c
+-rw-rw-rw-   0        0        0     1966 2023-07-31 11:38:16.000000 KKMeans-0.0.7/src/KKMeans/quality.pyx
+-rw-rw-rw-   0        0        0  1091357 2023-08-02 10:33:06.000000 KKMeans-0.0.7/src/KKMeans/utils.c
+-rw-rw-rw-   0        0        0     5309 2023-08-01 18:03:59.000000 KKMeans-0.0.7/src/KKMeans/utils.pyx
+drwxrwxrwx   0        0        0        0 2023-08-02 10:33:07.035641 KKMeans-0.0.7/tests/
+-rw-rw-rw-   0        0        0     1504 2023-08-01 21:50:30.000000 KKMeans-0.0.7/tests/test_pytest_utils.py
```

### Comparing `KKMeans-0.0.6/KKMeans.egg-info/SOURCES.txt` & `KKMeans-0.0.7/KKMeans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.6/license.txt` & `KKMeans-0.0.7/license.txt`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.6/pyproject.toml` & `KKMeans-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=63", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "KKMeans"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Paul Theis", email="keymailt7@gmail.com" },
 ]
 dependencies = ["numpy>=1.25"]
 description = "https://github.com/bauxn/kernel-kmeans. openMP is not enabled when installing via PiPy"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `KKMeans-0.0.6/setup.py` & `KKMeans-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.6/src/KKMeans/KKMeans.c` & `KKMeans-0.0.7/src/KKMeans/KKMeans.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.6/src/KKMeans/KKMeans.py` & `KKMeans-0.0.7/src/KKMeans/KKMeans.py`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.6/src/KKMeans/elkan.c` & `KKMeans-0.0.7/src/KKMeans/elkan.c`

 * *Files 1% similar despite different names*

```diff
@@ -17368,52 +17368,60 @@
   __PYX_INC_MEMVIEW(&__pyx_v_center_dists, 1);
   __PYX_INC_MEMVIEW(&__pyx_v_inner_sums, 1);
 
   /* "KKMeans/elkan.pyx":47
  * 
  * 
  *     inner_sums_old = inner_sums             # <<<<<<<<<<<<<<
- *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(kernel_matrix, labels, labels_old,
- *                                                           n_clusters, return_inner_new=True)
+ *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(
+ *         kernel_matrix, labels, labels_old,
  */
   __PYX_INC_MEMVIEW(&__pyx_v_inner_sums, 1);
   __pyx_v_inner_sums_old = __pyx_v_inner_sums;
 
   /* "KKMeans/elkan.pyx":48
  * 
  *     inner_sums_old = inner_sums
- *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(kernel_matrix, labels, labels_old,             # <<<<<<<<<<<<<<
- *                                                           n_clusters, return_inner_new=True)
- *     center_dists += _calc_center_dists(inner_sums, inner_sums_mixed, inner_sums_old, sizes, sizes_old)
+ *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(             # <<<<<<<<<<<<<<
+ *         kernel_matrix, labels, labels_old,
+ *         n_clusters, return_inner_new=True)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_calc_inner_sums_mixed); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_kernel_matrix, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
+
+  /* "KKMeans/elkan.pyx":49
+ *     inner_sums_old = inner_sums
+ *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(
+ *         kernel_matrix, labels, labels_old,             # <<<<<<<<<<<<<<
+ *         n_clusters, return_inner_new=True)
+ *     center_dists += _calc_center_dists(
+ */
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_kernel_matrix, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_labels, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_labels, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_labels_old, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_labels_old, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
-  /* "KKMeans/elkan.pyx":49
- *     inner_sums_old = inner_sums
- *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(kernel_matrix, labels, labels_old,
- *                                                           n_clusters, return_inner_new=True)             # <<<<<<<<<<<<<<
- *     center_dists += _calc_center_dists(inner_sums, inner_sums_mixed, inner_sums_old, sizes, sizes_old)
- *     l_bounds = _est_lower_bounds(kernel_matrix, l_bounds, center_dists, labels, sizes, inner_sums)
+  /* "KKMeans/elkan.pyx":50
+ *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(
+ *         kernel_matrix, labels, labels_old,
+ *         n_clusters, return_inner_new=True)             # <<<<<<<<<<<<<<
+ *     center_dists += _calc_center_dists(
+ *         inner_sums, inner_sums_mixed,
  */
-  __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_v_n_clusters); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_v_n_clusters); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
   /* "KKMeans/elkan.pyx":48
  * 
  *     inner_sums_old = inner_sums
- *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(kernel_matrix, labels, labels_old,             # <<<<<<<<<<<<<<
- *                                                           n_clusters, return_inner_new=True)
- *     center_dists += _calc_center_dists(inner_sums, inner_sums_mixed, inner_sums_old, sizes, sizes_old)
+ *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(             # <<<<<<<<<<<<<<
+ *         kernel_matrix, labels, labels_old,
+ *         n_clusters, return_inner_new=True)
  */
   __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_3);
@@ -17422,31 +17430,31 @@
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_6, 3, __pyx_t_5);
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
 
-  /* "KKMeans/elkan.pyx":49
- *     inner_sums_old = inner_sums
- *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(kernel_matrix, labels, labels_old,
- *                                                           n_clusters, return_inner_new=True)             # <<<<<<<<<<<<<<
- *     center_dists += _calc_center_dists(inner_sums, inner_sums_mixed, inner_sums_old, sizes, sizes_old)
- *     l_bounds = _est_lower_bounds(kernel_matrix, l_bounds, center_dists, labels, sizes, inner_sums)
+  /* "KKMeans/elkan.pyx":50
+ *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(
+ *         kernel_matrix, labels, labels_old,
+ *         n_clusters, return_inner_new=True)             # <<<<<<<<<<<<<<
+ *     center_dists += _calc_center_dists(
+ *         inner_sums, inner_sums_mixed,
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return_inner_new, Py_True) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return_inner_new, Py_True) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
 
   /* "KKMeans/elkan.pyx":48
  * 
  *     inner_sums_old = inner_sums
- *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(kernel_matrix, labels, labels_old,             # <<<<<<<<<<<<<<
- *                                                           n_clusters, return_inner_new=True)
- *     center_dists += _calc_center_dists(inner_sums, inner_sums_mixed, inner_sums_old, sizes, sizes_old)
+ *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(             # <<<<<<<<<<<<<<
+ *         kernel_matrix, labels, labels_old,
+ *         n_clusters, return_inner_new=True)
  */
   __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
@@ -17500,32 +17508,48 @@
   __pyx_v_inner_sums_mixed = __pyx_t_5;
   __pyx_t_5 = 0;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_inner_sums, 1);
   __pyx_v_inner_sums = __pyx_t_8;
   __pyx_t_8.memview = NULL;
   __pyx_t_8.data = NULL;
 
-  /* "KKMeans/elkan.pyx":50
- *     inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(kernel_matrix, labels, labels_old,
- *                                                           n_clusters, return_inner_new=True)
- *     center_dists += _calc_center_dists(inner_sums, inner_sums_mixed, inner_sums_old, sizes, sizes_old)             # <<<<<<<<<<<<<<
- *     l_bounds = _est_lower_bounds(kernel_matrix, l_bounds, center_dists, labels, sizes, inner_sums)
- *     return np.asarray(l_bounds), np.asarray(inner_sums), np.asarray(sizes), np.asarray(center_dists)
+  /* "KKMeans/elkan.pyx":51
+ *         kernel_matrix, labels, labels_old,
+ *         n_clusters, return_inner_new=True)
+ *     center_dists += _calc_center_dists(             # <<<<<<<<<<<<<<
+ *         inner_sums, inner_sums_mixed,
+ *         inner_sums_old, sizes, sizes_old)
  */
-  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_center_dists, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_center_dists, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_calc_center_dists); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_calc_center_dists); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_inner_sums, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+
+  /* "KKMeans/elkan.pyx":52
+ *         n_clusters, return_inner_new=True)
+ *     center_dists += _calc_center_dists(
+ *         inner_sums, inner_sums_mixed,             # <<<<<<<<<<<<<<
+ *         inner_sums_old, sizes, sizes_old)
+ *     l_bounds = _est_lower_bounds(
+ */
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_inner_sums, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_inner_sums_old, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
+
+  /* "KKMeans/elkan.pyx":53
+ *     center_dists += _calc_center_dists(
+ *         inner_sums, inner_sums_mixed,
+ *         inner_sums_old, sizes, sizes_old)             # <<<<<<<<<<<<<<
+ *     l_bounds = _est_lower_bounds(
+ *         kernel_matrix, l_bounds,
+ */
+  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_inner_sums_old, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_sizes, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_sizes, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_sizes_old, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_sizes_old, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_10 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -17539,49 +17563,81 @@
     PyObject *__pyx_callargs[6] = {__pyx_t_10, __pyx_t_1, __pyx_v_inner_sums_mixed, __pyx_t_3, __pyx_t_2, __pyx_t_9};
     __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_11, 5+__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 50, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 51, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L1_error)
+
+  /* "KKMeans/elkan.pyx":51
+ *         kernel_matrix, labels, labels_old,
+ *         n_clusters, return_inner_new=True)
+ *     center_dists += _calc_center_dists(             # <<<<<<<<<<<<<<
+ *         inner_sums, inner_sums_mixed,
+ *         inner_sums_old, sizes, sizes_old)
+ */
+  __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_center_dists, 1);
   __pyx_v_center_dists = __pyx_t_12;
   __pyx_t_12.memview = NULL;
   __pyx_t_12.data = NULL;
 
-  /* "KKMeans/elkan.pyx":51
- *                                                           n_clusters, return_inner_new=True)
- *     center_dists += _calc_center_dists(inner_sums, inner_sums_mixed, inner_sums_old, sizes, sizes_old)
- *     l_bounds = _est_lower_bounds(kernel_matrix, l_bounds, center_dists, labels, sizes, inner_sums)             # <<<<<<<<<<<<<<
- *     return np.asarray(l_bounds), np.asarray(inner_sums), np.asarray(sizes), np.asarray(center_dists)
- * 
+  /* "KKMeans/elkan.pyx":54
+ *         inner_sums, inner_sums_mixed,
+ *         inner_sums_old, sizes, sizes_old)
+ *     l_bounds = _est_lower_bounds(             # <<<<<<<<<<<<<<
+ *         kernel_matrix, l_bounds,
+ *         center_dists, labels,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_est_lower_bounds); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_est_lower_bounds); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_kernel_matrix, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
+
+  /* "KKMeans/elkan.pyx":55
+ *         inner_sums_old, sizes, sizes_old)
+ *     l_bounds = _est_lower_bounds(
+ *         kernel_matrix, l_bounds,             # <<<<<<<<<<<<<<
+ *         center_dists, labels,
+ *         sizes, inner_sums)
+ */
+  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_kernel_matrix, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_l_bounds, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_9 = __pyx_memoryview_fromslice(__pyx_v_l_bounds, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_center_dists, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
+
+  /* "KKMeans/elkan.pyx":56
+ *     l_bounds = _est_lower_bounds(
+ *         kernel_matrix, l_bounds,
+ *         center_dists, labels,             # <<<<<<<<<<<<<<
+ *         sizes, inner_sums)
+ *     return np.asarray(l_bounds), np.asarray(inner_sums), np.asarray(sizes), np.asarray(center_dists)
+ */
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_center_dists, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_labels, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_labels, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_sizes, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+
+  /* "KKMeans/elkan.pyx":57
+ *         kernel_matrix, l_bounds,
+ *         center_dists, labels,
+ *         sizes, inner_sums)             # <<<<<<<<<<<<<<
+ *     return np.asarray(l_bounds), np.asarray(inner_sums), np.asarray(sizes), np.asarray(center_dists)
+ * 
+ */
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_sizes, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_10 = __pyx_memoryview_fromslice(__pyx_v_inner_sums, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_10 = __pyx_memoryview_fromslice(__pyx_v_inner_sums, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __pyx_t_13 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_13)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -17597,39 +17653,47 @@
     __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 51, __pyx_L1_error)
+
+  /* "KKMeans/elkan.pyx":54
+ *         inner_sums, inner_sums_mixed,
+ *         inner_sums_old, sizes, sizes_old)
+ *     l_bounds = _est_lower_bounds(             # <<<<<<<<<<<<<<
+ *         kernel_matrix, l_bounds,
+ *         center_dists, labels,
+ */
+  __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_l_bounds, 1);
   __pyx_v_l_bounds = __pyx_t_12;
   __pyx_t_12.memview = NULL;
   __pyx_t_12.data = NULL;
 
-  /* "KKMeans/elkan.pyx":52
- *     center_dists += _calc_center_dists(inner_sums, inner_sums_mixed, inner_sums_old, sizes, sizes_old)
- *     l_bounds = _est_lower_bounds(kernel_matrix, l_bounds, center_dists, labels, sizes, inner_sums)
+  /* "KKMeans/elkan.pyx":58
+ *         center_dists, labels,
+ *         sizes, inner_sums)
  *     return np.asarray(l_bounds), np.asarray(inner_sums), np.asarray(sizes), np.asarray(center_dists)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_l_bounds, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_l_bounds, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_1 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
@@ -17640,24 +17704,24 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_t_6};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_inner_sums, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_inner_sums, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_3 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -17668,24 +17732,24 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_6};
     __pyx_t_10 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 52, __pyx_L1_error)
+    if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_sizes, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_sizes, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_2 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -17696,24 +17760,24 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_6};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_center_dists, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_6 = __pyx_memoryview_fromslice(__pyx_v_center_dists, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_9 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -17724,19 +17788,19 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_6};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_10);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_10);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_1);
@@ -17780,15 +17844,15 @@
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_center_dists, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_inner_sums, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans/elkan.pyx":55
+/* "KKMeans/elkan.pyx":61
  * 
  * 
  * def _est_lower_bounds(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         double[:, ::1] l_bounds,
  */
 
@@ -17846,76 +17910,76 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kernel_matrix)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 61, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_l_bounds)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 61, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_est_lower_bounds", 1, 6, 6, 1); __PYX_ERR(0, 55, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_est_lower_bounds", 1, 6, 6, 1); __PYX_ERR(0, 61, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_center_dists)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 61, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_est_lower_bounds", 1, 6, 6, 2); __PYX_ERR(0, 55, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_est_lower_bounds", 1, 6, 6, 2); __PYX_ERR(0, 61, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 61, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_est_lower_bounds", 1, 6, 6, 3); __PYX_ERR(0, 55, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_est_lower_bounds", 1, 6, 6, 3); __PYX_ERR(0, 61, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sizes)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 61, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_est_lower_bounds", 1, 6, 6, 4); __PYX_ERR(0, 55, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_est_lower_bounds", 1, 6, 6, 4); __PYX_ERR(0, 61, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_inner_sums)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 61, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_est_lower_bounds", 1, 6, 6, 5); __PYX_ERR(0, 55, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_est_lower_bounds", 1, 6, 6, 5); __PYX_ERR(0, 61, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_est_lower_bounds") < 0)) __PYX_ERR(0, 55, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_est_lower_bounds") < 0)) __PYX_ERR(0, 61, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 6)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
       values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
       values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
     }
-    __pyx_v_kernel_matrix = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_kernel_matrix.memview)) __PYX_ERR(0, 56, __pyx_L3_error)
-    __pyx_v_l_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_l_bounds.memview)) __PYX_ERR(0, 57, __pyx_L3_error)
-    __pyx_v_center_dists = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_center_dists.memview)) __PYX_ERR(0, 58, __pyx_L3_error)
-    __pyx_v_labels = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels.memview)) __PYX_ERR(0, 59, __pyx_L3_error)
-    __pyx_v_sizes = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sizes.memview)) __PYX_ERR(0, 60, __pyx_L3_error)
-    __pyx_v_inner_sums = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_inner_sums.memview)) __PYX_ERR(0, 61, __pyx_L3_error)
+    __pyx_v_kernel_matrix = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_kernel_matrix.memview)) __PYX_ERR(0, 62, __pyx_L3_error)
+    __pyx_v_l_bounds = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_l_bounds.memview)) __PYX_ERR(0, 63, __pyx_L3_error)
+    __pyx_v_center_dists = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_center_dists.memview)) __PYX_ERR(0, 64, __pyx_L3_error)
+    __pyx_v_labels = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels.memview)) __PYX_ERR(0, 65, __pyx_L3_error)
+    __pyx_v_sizes = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sizes.memview)) __PYX_ERR(0, 66, __pyx_L3_error)
+    __pyx_v_inner_sums = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_inner_sums.memview)) __PYX_ERR(0, 67, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_est_lower_bounds", 1, 6, 6, __pyx_nargs); __PYX_ERR(0, 55, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_est_lower_bounds", 1, 6, 6, __pyx_nargs); __PYX_ERR(0, 61, __pyx_L3_error)
   __pyx_L3_error:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_kernel_matrix, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_l_bounds, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_center_dists, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_labels, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_sizes, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_inner_sums, 1);
@@ -17960,68 +18024,68 @@
   Py_ssize_t __pyx_t_15;
   PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_est_lower_bounds", 0);
 
-  /* "KKMeans/elkan.pyx":77
+  /* "KKMeans/elkan.pyx":83
  *         double outer_sum
  * 
  *     assert l_bounds.shape[0] == labels.shape[0]             # <<<<<<<<<<<<<<
  *     assert l_bounds.shape[1] == inner_sums.shape[0]
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = ((__pyx_v_l_bounds.shape[0]) == (__pyx_v_labels.shape[0]));
     if (unlikely(!__pyx_t_1)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 77, __pyx_L1_error)
+      __PYX_ERR(0, 83, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 77, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 83, __pyx_L1_error)
   #endif
 
-  /* "KKMeans/elkan.pyx":78
+  /* "KKMeans/elkan.pyx":84
  * 
  *     assert l_bounds.shape[0] == labels.shape[0]
  *     assert l_bounds.shape[1] == inner_sums.shape[0]             # <<<<<<<<<<<<<<
  * 
  *     for i in prange(l_bounds.shape[0], nogil=True):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = ((__pyx_v_l_bounds.shape[1]) == (__pyx_v_inner_sums.shape[0]));
     if (unlikely(!__pyx_t_1)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 78, __pyx_L1_error)
+      __PYX_ERR(0, 84, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 78, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 84, __pyx_L1_error)
   #endif
 
-  /* "KKMeans/elkan.pyx":80
+  /* "KKMeans/elkan.pyx":86
  *     assert l_bounds.shape[1] == inner_sums.shape[0]
  * 
  *     for i in prange(l_bounds.shape[0], nogil=True):             # <<<<<<<<<<<<<<
  *         labels_i = labels[i]
  *         outer_sum = _calc_outer_sum_single(kernel_matrix, i, labels_i, labels)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       _save = NULL;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
-        if (unlikely(!__pyx_v_l_bounds.memview)) { __Pyx_RaiseUnboundMemoryviewSliceNogil("l_bounds"); __PYX_ERR(0, 80, __pyx_L4_error) }
+        if (unlikely(!__pyx_v_l_bounds.memview)) { __Pyx_RaiseUnboundMemoryviewSliceNogil("l_bounds"); __PYX_ERR(0, 86, __pyx_L4_error) }
         __pyx_t_2 = (__pyx_v_l_bounds.shape[0]);
         {
             Py_ssize_t __pyx_parallel_temp0 = ((Py_ssize_t)0xbad0bad0);
             Py_ssize_t __pyx_parallel_temp1 = ((Py_ssize_t)0xbad0bad0);
             Py_ssize_t __pyx_parallel_temp2 = ((Py_ssize_t)0xbad0bad0);
             double __pyx_parallel_temp3 = ((double)__PYX_NAN());
             const char *__pyx_parallel_filename = NULL; int __pyx_parallel_lineno = 0, __pyx_parallel_clineno = 0;
@@ -18055,98 +18119,98 @@
                         {
                             __pyx_v_i = (Py_ssize_t)(0 + 1 * __pyx_t_3);
                             /* Initialize private variables to invalid values */
                             __pyx_v_j = ((Py_ssize_t)0xbad0bad0);
                             __pyx_v_labels_i = ((Py_ssize_t)0xbad0bad0);
                             __pyx_v_outer_sum = ((double)__PYX_NAN());
 
-                            /* "KKMeans/elkan.pyx":81
+                            /* "KKMeans/elkan.pyx":87
  * 
  *     for i in prange(l_bounds.shape[0], nogil=True):
  *         labels_i = labels[i]             # <<<<<<<<<<<<<<
  *         outer_sum = _calc_outer_sum_single(kernel_matrix, i, labels_i, labels)
  *         # updating lower bounds from x to c_x
  */
                             __pyx_t_5 = __pyx_v_i;
                             __pyx_v_labels_i = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_labels.data) + __pyx_t_5)) )));
 
-                            /* "KKMeans/elkan.pyx":82
+                            /* "KKMeans/elkan.pyx":88
  *     for i in prange(l_bounds.shape[0], nogil=True):
  *         labels_i = labels[i]
  *         outer_sum = _calc_outer_sum_single(kernel_matrix, i, labels_i, labels)             # <<<<<<<<<<<<<<
  *         # updating lower bounds from x to c_x
  *         l_bounds[i, labels_i] = (
  */
-                            __pyx_t_6 = __pyx_f_7KKMeans_5elkan__calc_outer_sum_single(__pyx_v_kernel_matrix, __pyx_v_i, __pyx_v_labels_i, __pyx_v_labels, 0); if (unlikely(__pyx_t_6 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 82, __pyx_L8_error)
+                            __pyx_t_6 = __pyx_f_7KKMeans_5elkan__calc_outer_sum_single(__pyx_v_kernel_matrix, __pyx_v_i, __pyx_v_labels_i, __pyx_v_labels, 0); if (unlikely(__pyx_t_6 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 88, __pyx_L8_error)
                             __pyx_v_outer_sum = __pyx_t_6;
 
-                            /* "KKMeans/elkan.pyx":85
+                            /* "KKMeans/elkan.pyx":91
  *         # updating lower bounds from x to c_x
  *         l_bounds[i, labels_i] = (
  *             kernel_matrix[i, i]             # <<<<<<<<<<<<<<
  *             - 2 * outer_sum / sizes[labels_i]
  *             + inner_sums[labels_i] / sizes[labels_i]**2)
  */
                             __pyx_t_5 = __pyx_v_i;
                             __pyx_t_7 = __pyx_v_i;
 
-                            /* "KKMeans/elkan.pyx":86
+                            /* "KKMeans/elkan.pyx":92
  *         l_bounds[i, labels_i] = (
  *             kernel_matrix[i, i]
  *             - 2 * outer_sum / sizes[labels_i]             # <<<<<<<<<<<<<<
  *             + inner_sums[labels_i] / sizes[labels_i]**2)
  *         center_dists[i, labels_i] = 0  # relative movement set to 0
  */
                             __pyx_t_8 = __pyx_v_labels_i;
 
-                            /* "KKMeans/elkan.pyx":87
+                            /* "KKMeans/elkan.pyx":93
  *             kernel_matrix[i, i]
  *             - 2 * outer_sum / sizes[labels_i]
  *             + inner_sums[labels_i] / sizes[labels_i]**2)             # <<<<<<<<<<<<<<
  *         center_dists[i, labels_i] = 0  # relative movement set to 0
  *         for j in range(l_bounds.shape[1]):
  */
                             __pyx_t_9 = __pyx_v_labels_i;
                             __pyx_t_10 = __pyx_v_labels_i;
 
-                            /* "KKMeans/elkan.pyx":84
+                            /* "KKMeans/elkan.pyx":90
  *         outer_sum = _calc_outer_sum_single(kernel_matrix, i, labels_i, labels)
  *         # updating lower bounds from x to c_x
  *         l_bounds[i, labels_i] = (             # <<<<<<<<<<<<<<
  *             kernel_matrix[i, i]
  *             - 2 * outer_sum / sizes[labels_i]
  */
                             __pyx_t_11 = __pyx_v_i;
                             __pyx_t_12 = __pyx_v_labels_i;
                             *((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_l_bounds.data + __pyx_t_11 * __pyx_v_l_bounds.strides[0]) )) + __pyx_t_12)) )) = (((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_kernel_matrix.data + __pyx_t_5 * __pyx_v_kernel_matrix.strides[0]) )) + __pyx_t_7)) ))) - ((2.0 * __pyx_v_outer_sum) / ((double)(*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_sizes.data) + __pyx_t_8)) )))))) + ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_inner_sums.data) + __pyx_t_9)) ))) / ((double)__Pyx_pow_long((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_sizes.data) + __pyx_t_10)) ))), 2))));
 
-                            /* "KKMeans/elkan.pyx":88
+                            /* "KKMeans/elkan.pyx":94
  *             - 2 * outer_sum / sizes[labels_i]
  *             + inner_sums[labels_i] / sizes[labels_i]**2)
  *         center_dists[i, labels_i] = 0  # relative movement set to 0             # <<<<<<<<<<<<<<
  *         for j in range(l_bounds.shape[1]):
  *             if sqrt(l_bounds[i, j]) - center_dists[i, j] <= sqrt(l_bounds[i, labels_i]):
  */
                             __pyx_t_10 = __pyx_v_i;
                             __pyx_t_9 = __pyx_v_labels_i;
                             *((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_center_dists.data + __pyx_t_10 * __pyx_v_center_dists.strides[0]) )) + __pyx_t_9)) )) = 0.0;
 
-                            /* "KKMeans/elkan.pyx":89
+                            /* "KKMeans/elkan.pyx":95
  *             + inner_sums[labels_i] / sizes[labels_i]**2)
  *         center_dists[i, labels_i] = 0  # relative movement set to 0
  *         for j in range(l_bounds.shape[1]):             # <<<<<<<<<<<<<<
  *             if sqrt(l_bounds[i, j]) - center_dists[i, j] <= sqrt(l_bounds[i, labels_i]):
  *                 outer_sum = _calc_outer_sum_single(kernel_matrix, i, j, labels)
  */
                             __pyx_t_13 = (__pyx_v_l_bounds.shape[1]);
                             __pyx_t_14 = __pyx_t_13;
                             for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
                               __pyx_v_j = __pyx_t_15;
 
-                              /* "KKMeans/elkan.pyx":90
+                              /* "KKMeans/elkan.pyx":96
  *         center_dists[i, labels_i] = 0  # relative movement set to 0
  *         for j in range(l_bounds.shape[1]):
  *             if sqrt(l_bounds[i, j]) - center_dists[i, j] <= sqrt(l_bounds[i, labels_i]):             # <<<<<<<<<<<<<<
  *                 outer_sum = _calc_outer_sum_single(kernel_matrix, i, j, labels)
  *                 l_bounds[i, j] = (kernel_matrix[i, i]
  */
                               __pyx_t_9 = __pyx_v_i;
@@ -18154,76 +18218,76 @@
                               __pyx_t_8 = __pyx_v_i;
                               __pyx_t_7 = __pyx_v_j;
                               __pyx_t_5 = __pyx_v_i;
                               __pyx_t_12 = __pyx_v_labels_i;
                               __pyx_t_1 = ((sqrt((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_l_bounds.data + __pyx_t_9 * __pyx_v_l_bounds.strides[0]) )) + __pyx_t_10)) )))) - (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_center_dists.data + __pyx_t_8 * __pyx_v_center_dists.strides[0]) )) + __pyx_t_7)) )))) <= sqrt((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_l_bounds.data + __pyx_t_5 * __pyx_v_l_bounds.strides[0]) )) + __pyx_t_12)) )))));
                               if (__pyx_t_1) {
 
-                                /* "KKMeans/elkan.pyx":91
+                                /* "KKMeans/elkan.pyx":97
  *         for j in range(l_bounds.shape[1]):
  *             if sqrt(l_bounds[i, j]) - center_dists[i, j] <= sqrt(l_bounds[i, labels_i]):
  *                 outer_sum = _calc_outer_sum_single(kernel_matrix, i, j, labels)             # <<<<<<<<<<<<<<
  *                 l_bounds[i, j] = (kernel_matrix[i, i]
  *                                  - 2 * outer_sum / sizes[j]
  */
-                                __pyx_t_6 = __pyx_f_7KKMeans_5elkan__calc_outer_sum_single(__pyx_v_kernel_matrix, __pyx_v_i, __pyx_v_j, __pyx_v_labels, 0); if (unlikely(__pyx_t_6 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 91, __pyx_L8_error)
+                                __pyx_t_6 = __pyx_f_7KKMeans_5elkan__calc_outer_sum_single(__pyx_v_kernel_matrix, __pyx_v_i, __pyx_v_j, __pyx_v_labels, 0); if (unlikely(__pyx_t_6 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 97, __pyx_L8_error)
                                 __pyx_v_outer_sum = __pyx_t_6;
 
-                                /* "KKMeans/elkan.pyx":92
+                                /* "KKMeans/elkan.pyx":98
  *             if sqrt(l_bounds[i, j]) - center_dists[i, j] <= sqrt(l_bounds[i, labels_i]):
  *                 outer_sum = _calc_outer_sum_single(kernel_matrix, i, j, labels)
  *                 l_bounds[i, j] = (kernel_matrix[i, i]             # <<<<<<<<<<<<<<
  *                                  - 2 * outer_sum / sizes[j]
  *                                  + inner_sums[j] / sizes[j]**2)
  */
                                 __pyx_t_12 = __pyx_v_i;
                                 __pyx_t_5 = __pyx_v_i;
 
-                                /* "KKMeans/elkan.pyx":93
+                                /* "KKMeans/elkan.pyx":99
  *                 outer_sum = _calc_outer_sum_single(kernel_matrix, i, j, labels)
  *                 l_bounds[i, j] = (kernel_matrix[i, i]
  *                                  - 2 * outer_sum / sizes[j]             # <<<<<<<<<<<<<<
  *                                  + inner_sums[j] / sizes[j]**2)
  *                 center_dists[i, j] = 0
  */
                                 __pyx_t_7 = __pyx_v_j;
 
-                                /* "KKMeans/elkan.pyx":94
+                                /* "KKMeans/elkan.pyx":100
  *                 l_bounds[i, j] = (kernel_matrix[i, i]
  *                                  - 2 * outer_sum / sizes[j]
  *                                  + inner_sums[j] / sizes[j]**2)             # <<<<<<<<<<<<<<
  *                 center_dists[i, j] = 0
  *     return l_bounds
  */
                                 __pyx_t_8 = __pyx_v_j;
                                 __pyx_t_10 = __pyx_v_j;
 
-                                /* "KKMeans/elkan.pyx":92
+                                /* "KKMeans/elkan.pyx":98
  *             if sqrt(l_bounds[i, j]) - center_dists[i, j] <= sqrt(l_bounds[i, labels_i]):
  *                 outer_sum = _calc_outer_sum_single(kernel_matrix, i, j, labels)
  *                 l_bounds[i, j] = (kernel_matrix[i, i]             # <<<<<<<<<<<<<<
  *                                  - 2 * outer_sum / sizes[j]
  *                                  + inner_sums[j] / sizes[j]**2)
  */
                                 __pyx_t_9 = __pyx_v_i;
                                 __pyx_t_11 = __pyx_v_j;
                                 *((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_l_bounds.data + __pyx_t_9 * __pyx_v_l_bounds.strides[0]) )) + __pyx_t_11)) )) = (((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_kernel_matrix.data + __pyx_t_12 * __pyx_v_kernel_matrix.strides[0]) )) + __pyx_t_5)) ))) - ((2.0 * __pyx_v_outer_sum) / ((double)(*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_sizes.data) + __pyx_t_7)) )))))) + ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_inner_sums.data) + __pyx_t_8)) ))) / ((double)__Pyx_pow_long((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_sizes.data) + __pyx_t_10)) ))), 2))));
 
-                                /* "KKMeans/elkan.pyx":95
+                                /* "KKMeans/elkan.pyx":101
  *                                  - 2 * outer_sum / sizes[j]
  *                                  + inner_sums[j] / sizes[j]**2)
  *                 center_dists[i, j] = 0             # <<<<<<<<<<<<<<
  *     return l_bounds
  * 
  */
                                 __pyx_t_10 = __pyx_v_i;
                                 __pyx_t_8 = __pyx_v_j;
                                 *((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_center_dists.data + __pyx_t_10 * __pyx_v_center_dists.strides[0]) )) + __pyx_t_8)) )) = 0.0;
 
-                                /* "KKMeans/elkan.pyx":90
+                                /* "KKMeans/elkan.pyx":96
  *         center_dists[i, labels_i] = 0  # relative movement set to 0
  *         for j in range(l_bounds.shape[1]):
  *             if sqrt(l_bounds[i, j]) - center_dists[i, j] <= sqrt(l_bounds[i, labels_i]):             # <<<<<<<<<<<<<<
  *                 outer_sum = _calc_outer_sum_single(kernel_matrix, i, j, labels)
  *                 l_bounds[i, j] = (kernel_matrix[i, i]
  */
                               }
@@ -18311,15 +18375,15 @@
             #undef likely
             #undef unlikely
             #define likely(x)   __builtin_expect(!!(x), 1)
             #define unlikely(x) __builtin_expect(!!(x), 0)
         #endif
       }
 
-      /* "KKMeans/elkan.pyx":80
+      /* "KKMeans/elkan.pyx":86
  *     assert l_bounds.shape[1] == inner_sums.shape[0]
  * 
  *     for i in prange(l_bounds.shape[0], nogil=True):             # <<<<<<<<<<<<<<
  *         labels_i = labels[i]
  *         outer_sum = _calc_outer_sum_single(kernel_matrix, i, labels_i, labels)
  */
       /*finally:*/ {
@@ -18337,29 +18401,29 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L5:;
       }
   }
 
-  /* "KKMeans/elkan.pyx":96
+  /* "KKMeans/elkan.pyx":102
  *                                  + inner_sums[j] / sizes[j]**2)
  *                 center_dists[i, j] = 0
  *     return l_bounds             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_16 = __pyx_memoryview_fromslice(__pyx_v_l_bounds, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_16 = __pyx_memoryview_fromslice(__pyx_v_l_bounds, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __pyx_r = __pyx_t_16;
   __pyx_t_16 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans/elkan.pyx":55
+  /* "KKMeans/elkan.pyx":61
  * 
  * 
  * def _est_lower_bounds(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         double[:, ::1] l_bounds,
  */
 
@@ -18370,15 +18434,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans/elkan.pyx":99
+/* "KKMeans/elkan.pyx":105
  * 
  * 
  * def _calc_center_dists(             # <<<<<<<<<<<<<<
  *         double[::1] inner_sums_new,
  *         double[::1] inner_sums_mixed,
  */
 
@@ -18433,67 +18497,67 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_inner_sums_new)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 99, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_inner_sums_mixed)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 99, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_calc_center_dists", 1, 5, 5, 1); __PYX_ERR(0, 99, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calc_center_dists", 1, 5, 5, 1); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_inner_sums_old)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 99, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_calc_center_dists", 1, 5, 5, 2); __PYX_ERR(0, 99, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calc_center_dists", 1, 5, 5, 2); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sizes_new)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 99, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_calc_center_dists", 1, 5, 5, 3); __PYX_ERR(0, 99, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calc_center_dists", 1, 5, 5, 3); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sizes_old)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 99, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_calc_center_dists", 1, 5, 5, 4); __PYX_ERR(0, 99, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calc_center_dists", 1, 5, 5, 4); __PYX_ERR(0, 105, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_calc_center_dists") < 0)) __PYX_ERR(0, 99, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_calc_center_dists") < 0)) __PYX_ERR(0, 105, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 5)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
       values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
     }
-    __pyx_v_inner_sums_new = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_inner_sums_new.memview)) __PYX_ERR(0, 100, __pyx_L3_error)
-    __pyx_v_inner_sums_mixed = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_inner_sums_mixed.memview)) __PYX_ERR(0, 101, __pyx_L3_error)
-    __pyx_v_inner_sums_old = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_inner_sums_old.memview)) __PYX_ERR(0, 102, __pyx_L3_error)
-    __pyx_v_sizes_new = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sizes_new.memview)) __PYX_ERR(0, 103, __pyx_L3_error)
-    __pyx_v_sizes_old = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sizes_old.memview)) __PYX_ERR(0, 104, __pyx_L3_error)
+    __pyx_v_inner_sums_new = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_inner_sums_new.memview)) __PYX_ERR(0, 106, __pyx_L3_error)
+    __pyx_v_inner_sums_mixed = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_inner_sums_mixed.memview)) __PYX_ERR(0, 107, __pyx_L3_error)
+    __pyx_v_inner_sums_old = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_inner_sums_old.memview)) __PYX_ERR(0, 108, __pyx_L3_error)
+    __pyx_v_sizes_new = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sizes_new.memview)) __PYX_ERR(0, 109, __pyx_L3_error)
+    __pyx_v_sizes_old = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sizes_old.memview)) __PYX_ERR(0, 110, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_calc_center_dists", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 99, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_calc_center_dists", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 105, __pyx_L3_error)
   __pyx_L3_error:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_inner_sums_new, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_inner_sums_mixed, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_inner_sums_old, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_sizes_new, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_sizes_old, 1);
   __Pyx_AddTraceback("KKMeans.elkan._calc_center_dists", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -18535,36 +18599,36 @@
   Py_ssize_t __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_calc_center_dists", 0);
 
-  /* "KKMeans/elkan.pyx":117
+  /* "KKMeans/elkan.pyx":123
  *     cdef:
  *         Py_ssize_t i
  *         Py_ssize_t n_clusters = inner_sums_new.shape[0]             # <<<<<<<<<<<<<<
  *         double[::1] dists = np.zeros(n_clusters)
  *         long new_size, old_size
  */
   __pyx_v_n_clusters = (__pyx_v_inner_sums_new.shape[0]);
 
-  /* "KKMeans/elkan.pyx":118
+  /* "KKMeans/elkan.pyx":124
  *         Py_ssize_t i
  *         Py_ssize_t n_clusters = inner_sums_new.shape[0]
  *         double[::1] dists = np.zeros(n_clusters)             # <<<<<<<<<<<<<<
  *         long new_size, old_size
  *         double mixed_sum, new_sum, old_sum
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_n_clusters); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_n_clusters); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -18575,187 +18639,187 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_dists = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
-  /* "KKMeans/elkan.pyx":122
+  /* "KKMeans/elkan.pyx":128
  *         double mixed_sum, new_sum, old_sum
  * 
  *     assert n_clusters == inner_sums_mixed.shape[0]             # <<<<<<<<<<<<<<
  *     assert n_clusters == inner_sums_old.shape[0]
  *     assert n_clusters == sizes_new.shape[0]
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_7 = (__pyx_v_n_clusters == (__pyx_v_inner_sums_mixed.shape[0]));
     if (unlikely(!__pyx_t_7)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 122, __pyx_L1_error)
+      __PYX_ERR(0, 128, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 122, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 128, __pyx_L1_error)
   #endif
 
-  /* "KKMeans/elkan.pyx":123
+  /* "KKMeans/elkan.pyx":129
  * 
  *     assert n_clusters == inner_sums_mixed.shape[0]
  *     assert n_clusters == inner_sums_old.shape[0]             # <<<<<<<<<<<<<<
  *     assert n_clusters == sizes_new.shape[0]
  *     assert n_clusters == sizes_old.shape[0]
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_7 = (__pyx_v_n_clusters == (__pyx_v_inner_sums_old.shape[0]));
     if (unlikely(!__pyx_t_7)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 123, __pyx_L1_error)
+      __PYX_ERR(0, 129, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 123, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 129, __pyx_L1_error)
   #endif
 
-  /* "KKMeans/elkan.pyx":124
+  /* "KKMeans/elkan.pyx":130
  *     assert n_clusters == inner_sums_mixed.shape[0]
  *     assert n_clusters == inner_sums_old.shape[0]
  *     assert n_clusters == sizes_new.shape[0]             # <<<<<<<<<<<<<<
  *     assert n_clusters == sizes_old.shape[0]
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_7 = (__pyx_v_n_clusters == (__pyx_v_sizes_new.shape[0]));
     if (unlikely(!__pyx_t_7)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 124, __pyx_L1_error)
+      __PYX_ERR(0, 130, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 124, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 130, __pyx_L1_error)
   #endif
 
-  /* "KKMeans/elkan.pyx":125
+  /* "KKMeans/elkan.pyx":131
  *     assert n_clusters == inner_sums_old.shape[0]
  *     assert n_clusters == sizes_new.shape[0]
  *     assert n_clusters == sizes_old.shape[0]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(n_clusters):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_7 = (__pyx_v_n_clusters == (__pyx_v_sizes_old.shape[0]));
     if (unlikely(!__pyx_t_7)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 125, __pyx_L1_error)
+      __PYX_ERR(0, 131, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 125, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 131, __pyx_L1_error)
   #endif
 
-  /* "KKMeans/elkan.pyx":127
+  /* "KKMeans/elkan.pyx":133
  *     assert n_clusters == sizes_old.shape[0]
  * 
  *     for i in range(n_clusters):             # <<<<<<<<<<<<<<
  *         new_size = sizes_new[i]
  *         old_size = sizes_old[i]
  */
   __pyx_t_8 = __pyx_v_n_clusters;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "KKMeans/elkan.pyx":128
+    /* "KKMeans/elkan.pyx":134
  * 
  *     for i in range(n_clusters):
  *         new_size = sizes_new[i]             # <<<<<<<<<<<<<<
  *         old_size = sizes_old[i]
  *         mixed_sum = inner_sums_mixed[i]
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_v_new_size = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_sizes_new.data) + __pyx_t_11)) )));
 
-    /* "KKMeans/elkan.pyx":129
+    /* "KKMeans/elkan.pyx":135
  *     for i in range(n_clusters):
  *         new_size = sizes_new[i]
  *         old_size = sizes_old[i]             # <<<<<<<<<<<<<<
  *         mixed_sum = inner_sums_mixed[i]
  *         new_sum = inner_sums_new[i]
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_v_old_size = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_sizes_old.data) + __pyx_t_11)) )));
 
-    /* "KKMeans/elkan.pyx":130
+    /* "KKMeans/elkan.pyx":136
  *         new_size = sizes_new[i]
  *         old_size = sizes_old[i]
  *         mixed_sum = inner_sums_mixed[i]             # <<<<<<<<<<<<<<
  *         new_sum = inner_sums_new[i]
  *         old_sum = inner_sums_old[i]
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_v_mixed_sum = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_inner_sums_mixed.data) + __pyx_t_11)) )));
 
-    /* "KKMeans/elkan.pyx":131
+    /* "KKMeans/elkan.pyx":137
  *         old_size = sizes_old[i]
  *         mixed_sum = inner_sums_mixed[i]
  *         new_sum = inner_sums_new[i]             # <<<<<<<<<<<<<<
  *         old_sum = inner_sums_old[i]
  *         dists[i] = sqrt(new_sum / new_size**2
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_v_new_sum = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_inner_sums_new.data) + __pyx_t_11)) )));
 
-    /* "KKMeans/elkan.pyx":132
+    /* "KKMeans/elkan.pyx":138
  *         mixed_sum = inner_sums_mixed[i]
  *         new_sum = inner_sums_new[i]
  *         old_sum = inner_sums_old[i]             # <<<<<<<<<<<<<<
  *         dists[i] = sqrt(new_sum / new_size**2
  *                         - 2*mixed_sum / (new_size * old_size)
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_v_old_sum = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_inner_sums_old.data) + __pyx_t_11)) )));
 
-    /* "KKMeans/elkan.pyx":133
+    /* "KKMeans/elkan.pyx":139
  *         new_sum = inner_sums_new[i]
  *         old_sum = inner_sums_old[i]
  *         dists[i] = sqrt(new_sum / new_size**2             # <<<<<<<<<<<<<<
  *                         - 2*mixed_sum / (new_size * old_size)
  *                         + old_sum / old_size**2)
  */
     __pyx_t_11 = __pyx_v_i;
     *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_dists.data) + __pyx_t_11)) )) = sqrt((((__pyx_v_new_sum / ((double)__Pyx_pow_long(__pyx_v_new_size, 2))) - ((2.0 * __pyx_v_mixed_sum) / ((double)(__pyx_v_new_size * __pyx_v_old_size)))) + (__pyx_v_old_sum / ((double)__Pyx_pow_long(__pyx_v_old_size, 2)))));
   }
 
-  /* "KKMeans/elkan.pyx":137
+  /* "KKMeans/elkan.pyx":143
  *                         + old_sum / old_size**2)
  * 
  *     return np.asarray(dists)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dists, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dists, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -18766,23 +18830,23 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans/elkan.pyx":99
+  /* "KKMeans/elkan.pyx":105
  * 
  * 
  * def _calc_center_dists(             # <<<<<<<<<<<<<<
  *         double[::1] inner_sums_new,
  *         double[::1] inner_sums_mixed,
  */
 
@@ -18798,15 +18862,15 @@
   __pyx_L0:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_dists, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans/elkan.pyx":142
+/* "KKMeans/elkan.pyx":148
  * 
  * 
  * def _calc_inner_sums_mixed(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         long[::1] labels,
  */
 
@@ -18842,15 +18906,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_calc_inner_sums_mixed (wrapper)", 0);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_kernel_matrix,&__pyx_n_s_labels,&__pyx_n_s_labels_old,&__pyx_n_s_n_clusters,&__pyx_n_s_return_inner_new,0};
     PyObject* values[5] = {0,0,0,0,0};
 
-    /* "KKMeans/elkan.pyx":147
+    /* "KKMeans/elkan.pyx":153
  *         long[::1] labels_old,
  *         long n_clusters,
  *         return_inner_new=True):             # <<<<<<<<<<<<<<
  *     '''
  *     Mathematical helper function
  */
     values[4] = ((PyObject *)((PyObject *)Py_True));
@@ -18870,81 +18934,81 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kernel_matrix)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 148, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 148, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_calc_inner_sums_mixed", 0, 4, 5, 1); __PYX_ERR(0, 142, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calc_inner_sums_mixed", 0, 4, 5, 1); __PYX_ERR(0, 148, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels_old)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 148, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_calc_inner_sums_mixed", 0, 4, 5, 2); __PYX_ERR(0, 142, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calc_inner_sums_mixed", 0, 4, 5, 2); __PYX_ERR(0, 148, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_clusters)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 148, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_calc_inner_sums_mixed", 0, 4, 5, 3); __PYX_ERR(0, 142, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calc_inner_sums_mixed", 0, 4, 5, 3); __PYX_ERR(0, 148, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_return_inner_new);
           if (value) { values[4] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 148, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_calc_inner_sums_mixed") < 0)) __PYX_ERR(0, 142, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_calc_inner_sums_mixed") < 0)) __PYX_ERR(0, 148, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_kernel_matrix = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_kernel_matrix.memview)) __PYX_ERR(0, 143, __pyx_L3_error)
-    __pyx_v_labels = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels.memview)) __PYX_ERR(0, 144, __pyx_L3_error)
-    __pyx_v_labels_old = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels_old.memview)) __PYX_ERR(0, 145, __pyx_L3_error)
-    __pyx_v_n_clusters = __Pyx_PyInt_As_long(values[3]); if (unlikely((__pyx_v_n_clusters == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 146, __pyx_L3_error)
+    __pyx_v_kernel_matrix = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_kernel_matrix.memview)) __PYX_ERR(0, 149, __pyx_L3_error)
+    __pyx_v_labels = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels.memview)) __PYX_ERR(0, 150, __pyx_L3_error)
+    __pyx_v_labels_old = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels_old.memview)) __PYX_ERR(0, 151, __pyx_L3_error)
+    __pyx_v_n_clusters = __Pyx_PyInt_As_long(values[3]); if (unlikely((__pyx_v_n_clusters == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 152, __pyx_L3_error)
     __pyx_v_return_inner_new = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_calc_inner_sums_mixed", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 142, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_calc_inner_sums_mixed", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 148, __pyx_L3_error)
   __pyx_L3_error:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_kernel_matrix, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_labels, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_labels_old, 1);
   __Pyx_AddTraceback("KKMeans.elkan._calc_inner_sums_mixed", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_5elkan_6_calc_inner_sums_mixed(__pyx_self, __pyx_v_kernel_matrix, __pyx_v_labels, __pyx_v_labels_old, __pyx_v_n_clusters, __pyx_v_return_inner_new);
 
-  /* "KKMeans/elkan.pyx":142
+  /* "KKMeans/elkan.pyx":148
  * 
  * 
  * def _calc_inner_sums_mixed(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         long[::1] labels,
  */
 
@@ -18985,40 +19049,40 @@
   Py_ssize_t __pyx_t_18;
   Py_ssize_t __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_calc_inner_sums_mixed", 0);
 
-  /* "KKMeans/elkan.pyx":160
+  /* "KKMeans/elkan.pyx":166
  *     '''
  *     cdef:
  *         Py_ssize_t size = kernel_matrix.shape[0]             # <<<<<<<<<<<<<<
  *         double[:, ::1] sums_mixed = np.zeros((size, n_clusters))
  *         double[:, ::1] sums_new = np.zeros((size, n_clusters))
  */
   __pyx_v_size = (__pyx_v_kernel_matrix.shape[0]);
 
-  /* "KKMeans/elkan.pyx":161
+  /* "KKMeans/elkan.pyx":167
  *     cdef:
  *         Py_ssize_t size = kernel_matrix.shape[0]
  *         double[:, ::1] sums_mixed = np.zeros((size, n_clusters))             # <<<<<<<<<<<<<<
  *         double[:, ::1] sums_new = np.zeros((size, n_clusters))
  *         Py_ssize_t i, j
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
@@ -19035,41 +19099,41 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_5};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_sums_mixed = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "KKMeans/elkan.pyx":162
+  /* "KKMeans/elkan.pyx":168
  *         Py_ssize_t size = kernel_matrix.shape[0]
  *         double[:, ::1] sums_mixed = np.zeros((size, n_clusters))
  *         double[:, ::1] sums_new = np.zeros((size, n_clusters))             # <<<<<<<<<<<<<<
  *         Py_ssize_t i, j
  *         long labels_i
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
@@ -19086,44 +19150,44 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_sums_new = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "KKMeans/elkan.pyx":166
+  /* "KKMeans/elkan.pyx":172
  *         long labels_i
  * 
  *     assert size == kernel_matrix.shape[1]             # <<<<<<<<<<<<<<
  * 
  *     for i in prange(size, nogil=True):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_8 = (__pyx_v_size == (__pyx_v_kernel_matrix.shape[1]));
     if (unlikely(!__pyx_t_8)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 166, __pyx_L1_error)
+      __PYX_ERR(0, 172, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 166, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 172, __pyx_L1_error)
   #endif
 
-  /* "KKMeans/elkan.pyx":168
+  /* "KKMeans/elkan.pyx":174
  *     assert size == kernel_matrix.shape[1]
  * 
  *     for i in prange(size, nogil=True):             # <<<<<<<<<<<<<<
  *         labels_i = labels[i]
  *         for j in range(size):
  */
   {
@@ -19155,96 +19219,96 @@
                     for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_11; __pyx_t_10++){
                         {
                             __pyx_v_i = (Py_ssize_t)(0 + 1 * __pyx_t_10);
                             /* Initialize private variables to invalid values */
                             __pyx_v_j = ((Py_ssize_t)0xbad0bad0);
                             __pyx_v_labels_i = ((long)0xbad0bad0);
 
-                            /* "KKMeans/elkan.pyx":169
+                            /* "KKMeans/elkan.pyx":175
  * 
  *     for i in prange(size, nogil=True):
  *         labels_i = labels[i]             # <<<<<<<<<<<<<<
  *         for j in range(size):
  *             if labels_i == labels[j]:
  */
                             __pyx_t_12 = __pyx_v_i;
                             __pyx_v_labels_i = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_labels.data) + __pyx_t_12)) )));
 
-                            /* "KKMeans/elkan.pyx":170
+                            /* "KKMeans/elkan.pyx":176
  *     for i in prange(size, nogil=True):
  *         labels_i = labels[i]
  *         for j in range(size):             # <<<<<<<<<<<<<<
  *             if labels_i == labels[j]:
  *                 sums_new[i, labels[j]] += kernel_matrix[i, j]
  */
                             __pyx_t_13 = __pyx_v_size;
                             __pyx_t_14 = __pyx_t_13;
                             for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
                               __pyx_v_j = __pyx_t_15;
 
-                              /* "KKMeans/elkan.pyx":171
+                              /* "KKMeans/elkan.pyx":177
  *         labels_i = labels[i]
  *         for j in range(size):
  *             if labels_i == labels[j]:             # <<<<<<<<<<<<<<
  *                 sums_new[i, labels[j]] += kernel_matrix[i, j]
  *             if labels_i == labels_old[j]:
  */
                               __pyx_t_12 = __pyx_v_j;
                               __pyx_t_8 = (__pyx_v_labels_i == (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_labels.data) + __pyx_t_12)) ))));
                               if (__pyx_t_8) {
 
-                                /* "KKMeans/elkan.pyx":172
+                                /* "KKMeans/elkan.pyx":178
  *         for j in range(size):
  *             if labels_i == labels[j]:
  *                 sums_new[i, labels[j]] += kernel_matrix[i, j]             # <<<<<<<<<<<<<<
  *             if labels_i == labels_old[j]:
  *                 sums_mixed[i, labels_old[j]] += kernel_matrix[i, j]
  */
                                 __pyx_t_12 = __pyx_v_i;
                                 __pyx_t_16 = __pyx_v_j;
                                 __pyx_t_17 = __pyx_v_j;
                                 __pyx_t_18 = __pyx_v_i;
                                 __pyx_t_19 = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_labels.data) + __pyx_t_17)) )));
                                 *((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_sums_new.data + __pyx_t_18 * __pyx_v_sums_new.strides[0]) )) + __pyx_t_19)) )) += (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_kernel_matrix.data + __pyx_t_12 * __pyx_v_kernel_matrix.strides[0]) )) + __pyx_t_16)) )));
 
-                                /* "KKMeans/elkan.pyx":171
+                                /* "KKMeans/elkan.pyx":177
  *         labels_i = labels[i]
  *         for j in range(size):
  *             if labels_i == labels[j]:             # <<<<<<<<<<<<<<
  *                 sums_new[i, labels[j]] += kernel_matrix[i, j]
  *             if labels_i == labels_old[j]:
  */
                               }
 
-                              /* "KKMeans/elkan.pyx":173
+                              /* "KKMeans/elkan.pyx":179
  *             if labels_i == labels[j]:
  *                 sums_new[i, labels[j]] += kernel_matrix[i, j]
  *             if labels_i == labels_old[j]:             # <<<<<<<<<<<<<<
  *                 sums_mixed[i, labels_old[j]] += kernel_matrix[i, j]
  *     if return_inner_new:
  */
                               __pyx_t_16 = __pyx_v_j;
                               __pyx_t_8 = (__pyx_v_labels_i == (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_labels_old.data) + __pyx_t_16)) ))));
                               if (__pyx_t_8) {
 
-                                /* "KKMeans/elkan.pyx":174
+                                /* "KKMeans/elkan.pyx":180
  *                 sums_new[i, labels[j]] += kernel_matrix[i, j]
  *             if labels_i == labels_old[j]:
  *                 sums_mixed[i, labels_old[j]] += kernel_matrix[i, j]             # <<<<<<<<<<<<<<
  *     if return_inner_new:
  *         return np.sum(sums_mixed, axis=0), np.sum(sums_new, axis=0)
  */
                                 __pyx_t_16 = __pyx_v_i;
                                 __pyx_t_12 = __pyx_v_j;
                                 __pyx_t_17 = __pyx_v_j;
                                 __pyx_t_19 = __pyx_v_i;
                                 __pyx_t_18 = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_labels_old.data) + __pyx_t_17)) )));
                                 *((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_sums_mixed.data + __pyx_t_19 * __pyx_v_sums_mixed.strides[0]) )) + __pyx_t_18)) )) += (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_kernel_matrix.data + __pyx_t_16 * __pyx_v_kernel_matrix.strides[0]) )) + __pyx_t_12)) )));
 
-                                /* "KKMeans/elkan.pyx":173
+                                /* "KKMeans/elkan.pyx":179
  *             if labels_i == labels[j]:
  *                 sums_new[i, labels[j]] += kernel_matrix[i, j]
  *             if labels_i == labels_old[j]:             # <<<<<<<<<<<<<<
  *                 sums_mixed[i, labels_old[j]] += kernel_matrix[i, j]
  *     if return_inner_new:
  */
                               }
@@ -19258,15 +19322,15 @@
             #undef likely
             #undef unlikely
             #define likely(x)   __builtin_expect(!!(x), 1)
             #define unlikely(x) __builtin_expect(!!(x), 0)
         #endif
       }
 
-      /* "KKMeans/elkan.pyx":168
+      /* "KKMeans/elkan.pyx":174
  *     assert size == kernel_matrix.shape[1]
  * 
  *     for i in prange(size, nogil=True):             # <<<<<<<<<<<<<<
  *         labels_i = labels[i]
  *         for j in range(size):
  */
       /*finally:*/ {
@@ -19277,126 +19341,126 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "KKMeans/elkan.pyx":175
+  /* "KKMeans/elkan.pyx":181
  *             if labels_i == labels_old[j]:
  *                 sums_mixed[i, labels_old[j]] += kernel_matrix[i, j]
  *     if return_inner_new:             # <<<<<<<<<<<<<<
  *         return np.sum(sums_mixed, axis=0), np.sum(sums_new, axis=0)
  *     return np.sum(sums_mixed, axis=0)
  */
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_return_inner_new); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_return_inner_new); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 181, __pyx_L1_error)
   if (__pyx_t_8) {
 
-    /* "KKMeans/elkan.pyx":176
+    /* "KKMeans/elkan.pyx":182
  *                 sums_mixed[i, labels_old[j]] += kernel_matrix[i, j]
  *     if return_inner_new:
  *         return np.sum(sums_mixed, axis=0), np.sum(sums_new, axis=0)             # <<<<<<<<<<<<<<
  *     return np.sum(sums_mixed, axis=0)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sum); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sum); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_sums_mixed, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_sums_mixed, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 176, __pyx_L1_error)
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 176, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_sums_new, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_sums_new, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 176, __pyx_L1_error)
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_3 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "KKMeans/elkan.pyx":175
+    /* "KKMeans/elkan.pyx":181
  *             if labels_i == labels_old[j]:
  *                 sums_mixed[i, labels_old[j]] += kernel_matrix[i, j]
  *     if return_inner_new:             # <<<<<<<<<<<<<<
  *         return np.sum(sums_mixed, axis=0), np.sum(sums_new, axis=0)
  *     return np.sum(sums_mixed, axis=0)
  */
   }
 
-  /* "KKMeans/elkan.pyx":177
+  /* "KKMeans/elkan.pyx":183
  *     if return_inner_new:
  *         return np.sum(sums_mixed, axis=0), np.sum(sums_new, axis=0)
  *     return np.sum(sums_mixed, axis=0)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_sums_mixed, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_sums_mixed, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 177, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans/elkan.pyx":142
+  /* "KKMeans/elkan.pyx":148
  * 
  * 
  * def _calc_inner_sums_mixed(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         long[::1] labels,
  */
 
@@ -19414,15 +19478,15 @@
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_sums_mixed, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_sums_new, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans/elkan.pyx":182
+/* "KKMeans/elkan.pyx":188
  * 
  * 
  * def start_elkan(             # <<<<<<<<<<<<<<
  *         sq_distances,
  *         double[:, ::1] kernel_matrix,
  */
 
@@ -19477,67 +19541,67 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sq_distances)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kernel_matrix)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("start_elkan", 1, 5, 5, 1); __PYX_ERR(0, 182, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("start_elkan", 1, 5, 5, 1); __PYX_ERR(0, 188, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("start_elkan", 1, 5, 5, 2); __PYX_ERR(0, 182, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("start_elkan", 1, 5, 5, 2); __PYX_ERR(0, 188, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_clusters)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("start_elkan", 1, 5, 5, 3); __PYX_ERR(0, 182, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("start_elkan", 1, 5, 5, 3); __PYX_ERR(0, 188, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cluster_sizes)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("start_elkan", 1, 5, 5, 4); __PYX_ERR(0, 182, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("start_elkan", 1, 5, 5, 4); __PYX_ERR(0, 188, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "start_elkan") < 0)) __PYX_ERR(0, 182, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "start_elkan") < 0)) __PYX_ERR(0, 188, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 5)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
       values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
     }
     __pyx_v_sq_distances = values[0];
-    __pyx_v_kernel_matrix = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_kernel_matrix.memview)) __PYX_ERR(0, 184, __pyx_L3_error)
-    __pyx_v_labels = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels.memview)) __PYX_ERR(0, 185, __pyx_L3_error)
-    __pyx_v_n_clusters = __Pyx_PyInt_As_long(values[3]); if (unlikely((__pyx_v_n_clusters == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 186, __pyx_L3_error)
-    __pyx_v_cluster_sizes = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cluster_sizes.memview)) __PYX_ERR(0, 187, __pyx_L3_error)
+    __pyx_v_kernel_matrix = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_kernel_matrix.memview)) __PYX_ERR(0, 190, __pyx_L3_error)
+    __pyx_v_labels = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels.memview)) __PYX_ERR(0, 191, __pyx_L3_error)
+    __pyx_v_n_clusters = __Pyx_PyInt_As_long(values[3]); if (unlikely((__pyx_v_n_clusters == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 192, __pyx_L3_error)
+    __pyx_v_cluster_sizes = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cluster_sizes.memview)) __PYX_ERR(0, 193, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("start_elkan", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 182, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("start_elkan", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 188, __pyx_L3_error)
   __pyx_L3_error:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_kernel_matrix, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_labels, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_cluster_sizes, 1);
   __Pyx_AddTraceback("KKMeans.elkan.start_elkan", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
@@ -19575,62 +19639,62 @@
   Py_ssize_t __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("start_elkan", 0);
   __Pyx_INCREF(__pyx_v_sq_distances);
 
-  /* "KKMeans/elkan.pyx":216
+  /* "KKMeans/elkan.pyx":222
  * 
  * 
  *     sq_distances = np.asarray(sq_distances, dtype=np.double)             # <<<<<<<<<<<<<<
  *     outer_sums, inner_sums = _calc_sums_full(kernel_matrix, labels, n_clusters)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_sq_distances);
   __Pyx_GIVEREF(__pyx_v_sq_distances);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_sq_distances);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 216, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_sq_distances, __pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "KKMeans/elkan.pyx":217
+  /* "KKMeans/elkan.pyx":223
  * 
  *     sq_distances = np.asarray(sq_distances, dtype=np.double)
  *     outer_sums, inner_sums = _calc_sums_full(kernel_matrix, labels, n_clusters)             # <<<<<<<<<<<<<<
  * 
  *     for cluster in range(n_clusters):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_calc_sums_full); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 217, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_calc_sums_full); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_kernel_matrix, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_kernel_matrix, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_labels, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 217, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_labels, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 217, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -19643,198 +19707,198 @@
   {
     PyObject *__pyx_callargs[4] = {__pyx_t_6, __pyx_t_1, __pyx_t_2, __pyx_t_4};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 3+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 217, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   if ((likely(PyTuple_CheckExact(__pyx_t_5))) || (PyList_CheckExact(__pyx_t_5))) {
     PyObject* sequence = __pyx_t_5;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 217, __pyx_L1_error)
+      __PYX_ERR(0, 223, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_3 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_2 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __pyx_t_2 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2);
     index = 0; __pyx_t_3 = __pyx_t_8(__pyx_t_2); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
     index = 1; __pyx_t_4 = __pyx_t_8(__pyx_t_2); if (unlikely(!__pyx_t_4)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_4);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_2), 2) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_2), 2) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
     __pyx_t_8 = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_8 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 217, __pyx_L1_error)
+    __PYX_ERR(0, 223, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_outer_sums = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_inner_sums = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "KKMeans/elkan.pyx":219
+  /* "KKMeans/elkan.pyx":225
  *     outer_sums, inner_sums = _calc_sums_full(kernel_matrix, labels, n_clusters)
  * 
  *     for cluster in range(n_clusters):             # <<<<<<<<<<<<<<
  *         size = cluster_sizes[cluster]
  *         outer_sum = outer_sums[:, cluster]
  */
   __pyx_t_9 = __pyx_v_n_clusters;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_cluster = __pyx_t_11;
 
-    /* "KKMeans/elkan.pyx":220
+    /* "KKMeans/elkan.pyx":226
  * 
  *     for cluster in range(n_clusters):
  *         size = cluster_sizes[cluster]             # <<<<<<<<<<<<<<
  *         outer_sum = outer_sums[:, cluster]
  *         inner_sum = inner_sums[cluster]
  */
     __pyx_t_12 = __pyx_v_cluster;
-    __pyx_t_5 = __Pyx_PyInt_From_long((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_cluster_sizes.data) + __pyx_t_12)) )))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_long((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_cluster_sizes.data) + __pyx_t_12)) )))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_XDECREF_SET(__pyx_v_size, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "KKMeans/elkan.pyx":221
+    /* "KKMeans/elkan.pyx":227
  *     for cluster in range(n_clusters):
  *         size = cluster_sizes[cluster]
  *         outer_sum = outer_sums[:, cluster]             # <<<<<<<<<<<<<<
  *         inner_sum = inner_sums[cluster]
  *         sq_distances[:,  cluster] += (-2 * outer_sum / size
  */
-    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_cluster); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_cluster); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_slice__5);
     __Pyx_GIVEREF(__pyx_slice__5);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_slice__5);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_outer_sums, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_outer_sums, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF_SET(__pyx_v_outer_sum, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "KKMeans/elkan.pyx":222
+    /* "KKMeans/elkan.pyx":228
  *         size = cluster_sizes[cluster]
  *         outer_sum = outer_sums[:, cluster]
  *         inner_sum = inner_sums[cluster]             # <<<<<<<<<<<<<<
  *         sq_distances[:,  cluster] += (-2 * outer_sum / size
  *                                      + inner_sum / size**2)
  */
-    __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_inner_sums, __pyx_v_cluster, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_inner_sums, __pyx_v_cluster, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 228, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_XDECREF_SET(__pyx_v_inner_sum, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "KKMeans/elkan.pyx":223
+    /* "KKMeans/elkan.pyx":229
  *         outer_sum = outer_sums[:, cluster]
  *         inner_sum = inner_sums[cluster]
  *         sq_distances[:,  cluster] += (-2 * outer_sum / size             # <<<<<<<<<<<<<<
  *                                      + inner_sum / size**2)
  *     return np.asarray(sq_distances), np.asarray(inner_sums), np.asarray(cluster_sizes)
  */
-    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_cluster); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_cluster); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_slice__5);
     __Pyx_GIVEREF(__pyx_slice__5);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_slice__5);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_sq_distances, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_sq_distances, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyInt_MultiplyCObj(__pyx_int_neg_2, __pyx_v_outer_sum, -2L, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_MultiplyCObj(__pyx_int_neg_2, __pyx_v_outer_sum, -2L, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_v_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_v_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "KKMeans/elkan.pyx":224
+    /* "KKMeans/elkan.pyx":230
  *         inner_sum = inner_sums[cluster]
  *         sq_distances[:,  cluster] += (-2 * outer_sum / size
  *                                      + inner_sum / size**2)             # <<<<<<<<<<<<<<
  *     return np.asarray(sq_distances), np.asarray(inner_sums), np.asarray(cluster_sizes)
  * 
  */
-    __pyx_t_3 = PyNumber_Power(__pyx_v_size, __pyx_int_2, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Power(__pyx_v_size, __pyx_int_2, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 230, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_v_inner_sum, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_v_inner_sum, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 230, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "KKMeans/elkan.pyx":223
+    /* "KKMeans/elkan.pyx":229
  *         outer_sum = outer_sums[:, cluster]
  *         inner_sum = inner_sums[cluster]
  *         sq_distances[:,  cluster] += (-2 * outer_sum / size             # <<<<<<<<<<<<<<
  *                                      + inner_sum / size**2)
  *     return np.asarray(sq_distances), np.asarray(inner_sums), np.asarray(cluster_sizes)
  */
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely((PyObject_SetItem(__pyx_v_sq_distances, __pyx_t_4, __pyx_t_1) < 0))) __PYX_ERR(0, 223, __pyx_L1_error)
+    if (unlikely((PyObject_SetItem(__pyx_v_sq_distances, __pyx_t_4, __pyx_t_1) < 0))) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
 
-  /* "KKMeans/elkan.pyx":225
+  /* "KKMeans/elkan.pyx":231
  *         sq_distances[:,  cluster] += (-2 * outer_sum / size
  *                                      + inner_sum / size**2)
  *     return np.asarray(sq_distances), np.asarray(inner_sums), np.asarray(cluster_sizes)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
@@ -19845,21 +19909,21 @@
       __pyx_t_7 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_sq_distances};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 225, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_1)) {
@@ -19870,24 +19934,24 @@
       __pyx_t_7 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_inner_sums};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 225, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_cluster_sizes, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_cluster_sizes, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -19898,34 +19962,34 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_1};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 225, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_5);
   __pyx_t_4 = 0;
   __pyx_t_3 = 0;
   __pyx_t_5 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans/elkan.pyx":182
+  /* "KKMeans/elkan.pyx":188
  * 
  * 
  * def start_elkan(             # <<<<<<<<<<<<<<
  *         sq_distances,
  *         double[:, ::1] kernel_matrix,
  */
 
@@ -19947,20 +20011,20 @@
   __Pyx_XDECREF(__pyx_v_inner_sum);
   __Pyx_XDECREF(__pyx_v_sq_distances);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans/elkan.pyx":228
+/* "KKMeans/elkan.pyx":234
  * 
  * 
- * def _calc_sums_full(double[:, ::1] kernel_matrix, long[::1] labels, long n_clusters):             # <<<<<<<<<<<<<<
- *     '''
- *     Mathematical helper function
+ * def _calc_sums_full(             # <<<<<<<<<<<<<<
+ *         double[:, ::1] kernel_matrix,
+ *         long[::1] labels,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7KKMeans_5elkan_11_calc_sums_full(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
@@ -20004,49 +20068,49 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kernel_matrix)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 228, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 234, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 228, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 234, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_calc_sums_full", 1, 3, 3, 1); __PYX_ERR(0, 228, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calc_sums_full", 1, 3, 3, 1); __PYX_ERR(0, 234, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_clusters)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 228, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 234, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_calc_sums_full", 1, 3, 3, 2); __PYX_ERR(0, 228, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calc_sums_full", 1, 3, 3, 2); __PYX_ERR(0, 234, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_calc_sums_full") < 0)) __PYX_ERR(0, 228, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_calc_sums_full") < 0)) __PYX_ERR(0, 234, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
-    __pyx_v_kernel_matrix = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_kernel_matrix.memview)) __PYX_ERR(0, 228, __pyx_L3_error)
-    __pyx_v_labels = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels.memview)) __PYX_ERR(0, 228, __pyx_L3_error)
-    __pyx_v_n_clusters = __Pyx_PyInt_As_long(values[2]); if (unlikely((__pyx_v_n_clusters == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 228, __pyx_L3_error)
+    __pyx_v_kernel_matrix = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_kernel_matrix.memview)) __PYX_ERR(0, 235, __pyx_L3_error)
+    __pyx_v_labels = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels.memview)) __PYX_ERR(0, 236, __pyx_L3_error)
+    __pyx_v_n_clusters = __Pyx_PyInt_As_long(values[2]); if (unlikely((__pyx_v_n_clusters == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 237, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_calc_sums_full", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 228, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_calc_sums_full", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 234, __pyx_L3_error)
   __pyx_L3_error:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_kernel_matrix, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_labels, 1);
   __Pyx_AddTraceback("KKMeans.elkan._calc_sums_full", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -20089,131 +20153,131 @@
   int __pyx_t_17;
   int __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_calc_sums_full", 0);
 
-  /* "KKMeans/elkan.pyx":243
+  /* "KKMeans/elkan.pyx":252
  *     '''
  *     cdef:
  *         Py_ssize_t rows = kernel_matrix.shape[0]             # <<<<<<<<<<<<<<
  *         Py_ssize_t cols = kernel_matrix.shape[1]
  *         double[:, ::1] inner_sum = np.zeros((rows, n_clusters), dtype=np.double)
  */
   __pyx_v_rows = (__pyx_v_kernel_matrix.shape[0]);
 
-  /* "KKMeans/elkan.pyx":244
+  /* "KKMeans/elkan.pyx":253
  *     cdef:
  *         Py_ssize_t rows = kernel_matrix.shape[0]
  *         Py_ssize_t cols = kernel_matrix.shape[1]             # <<<<<<<<<<<<<<
  *         double[:, ::1] inner_sum = np.zeros((rows, n_clusters), dtype=np.double)
  *         double[:, ::1] outer_sum = np.zeros((rows, n_clusters), dtype=np.double)
  */
   __pyx_v_cols = (__pyx_v_kernel_matrix.shape[1]);
 
-  /* "KKMeans/elkan.pyx":245
+  /* "KKMeans/elkan.pyx":254
  *         Py_ssize_t rows = kernel_matrix.shape[0]
  *         Py_ssize_t cols = kernel_matrix.shape[1]
  *         double[:, ::1] inner_sum = np.zeros((rows, n_clusters), dtype=np.double)             # <<<<<<<<<<<<<<
  *         double[:, ::1] outer_sum = np.zeros((rows, n_clusters), dtype=np.double)
  *         Py_ssize_t i,j
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_rows); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_rows); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_n_clusters); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_n_clusters); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_inner_sum = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
-  /* "KKMeans/elkan.pyx":246
+  /* "KKMeans/elkan.pyx":255
  *         Py_ssize_t cols = kernel_matrix.shape[1]
  *         double[:, ::1] inner_sum = np.zeros((rows, n_clusters), dtype=np.double)
  *         double[:, ::1] outer_sum = np.zeros((rows, n_clusters), dtype=np.double)             # <<<<<<<<<<<<<<
  *         Py_ssize_t i,j
  *         int label_i, label_j
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_rows); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_rows); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_n_clusters); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_n_clusters); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_5 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_double); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_double); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_outer_sum = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
-  /* "KKMeans/elkan.pyx":249
+  /* "KKMeans/elkan.pyx":258
  *         Py_ssize_t i,j
  *         int label_i, label_j
  *     for i in prange(rows, nogil=True):             # <<<<<<<<<<<<<<
  *         label_i = labels[i]
  *         for j in range(cols):
  */
   {
@@ -20246,83 +20310,83 @@
                         {
                             __pyx_v_i = (Py_ssize_t)(0 + 1 * __pyx_t_8);
                             /* Initialize private variables to invalid values */
                             __pyx_v_j = ((Py_ssize_t)0xbad0bad0);
                             __pyx_v_label_i = ((int)0xbad0bad0);
                             __pyx_v_label_j = ((int)0xbad0bad0);
 
-                            /* "KKMeans/elkan.pyx":250
+                            /* "KKMeans/elkan.pyx":259
  *         int label_i, label_j
  *     for i in prange(rows, nogil=True):
  *         label_i = labels[i]             # <<<<<<<<<<<<<<
  *         for j in range(cols):
  *             label_j = labels[j]
  */
                             __pyx_t_10 = __pyx_v_i;
                             __pyx_v_label_i = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_labels.data) + __pyx_t_10)) )));
 
-                            /* "KKMeans/elkan.pyx":251
+                            /* "KKMeans/elkan.pyx":260
  *     for i in prange(rows, nogil=True):
  *         label_i = labels[i]
  *         for j in range(cols):             # <<<<<<<<<<<<<<
  *             label_j = labels[j]
  *             outer_sum[i, label_j] += kernel_matrix[i, j]
  */
                             __pyx_t_11 = __pyx_v_cols;
                             __pyx_t_12 = __pyx_t_11;
                             for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
                               __pyx_v_j = __pyx_t_13;
 
-                              /* "KKMeans/elkan.pyx":252
+                              /* "KKMeans/elkan.pyx":261
  *         label_i = labels[i]
  *         for j in range(cols):
  *             label_j = labels[j]             # <<<<<<<<<<<<<<
  *             outer_sum[i, label_j] += kernel_matrix[i, j]
  *             if label_i == label_j:
  */
                               __pyx_t_10 = __pyx_v_j;
                               __pyx_v_label_j = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_labels.data) + __pyx_t_10)) )));
 
-                              /* "KKMeans/elkan.pyx":253
+                              /* "KKMeans/elkan.pyx":262
  *         for j in range(cols):
  *             label_j = labels[j]
  *             outer_sum[i, label_j] += kernel_matrix[i, j]             # <<<<<<<<<<<<<<
  *             if label_i == label_j:
  *                 inner_sum[i, label_j] += kernel_matrix[i, j]
  */
                               __pyx_t_10 = __pyx_v_i;
                               __pyx_t_14 = __pyx_v_j;
                               __pyx_t_15 = __pyx_v_i;
                               __pyx_t_16 = __pyx_v_label_j;
                               *((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_outer_sum.data + __pyx_t_15 * __pyx_v_outer_sum.strides[0]) )) + __pyx_t_16)) )) += (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_kernel_matrix.data + __pyx_t_10 * __pyx_v_kernel_matrix.strides[0]) )) + __pyx_t_14)) )));
 
-                              /* "KKMeans/elkan.pyx":254
+                              /* "KKMeans/elkan.pyx":263
  *             label_j = labels[j]
  *             outer_sum[i, label_j] += kernel_matrix[i, j]
  *             if label_i == label_j:             # <<<<<<<<<<<<<<
  *                 inner_sum[i, label_j] += kernel_matrix[i, j]
  *     return np.asarray(outer_sum), np.sum(inner_sum, axis=0)
  */
                               __pyx_t_17 = (__pyx_v_label_i == __pyx_v_label_j);
                               if (__pyx_t_17) {
 
-                                /* "KKMeans/elkan.pyx":255
+                                /* "KKMeans/elkan.pyx":264
  *             outer_sum[i, label_j] += kernel_matrix[i, j]
  *             if label_i == label_j:
  *                 inner_sum[i, label_j] += kernel_matrix[i, j]             # <<<<<<<<<<<<<<
  *     return np.asarray(outer_sum), np.sum(inner_sum, axis=0)
  * 
  */
                                 __pyx_t_14 = __pyx_v_i;
                                 __pyx_t_10 = __pyx_v_j;
                                 __pyx_t_16 = __pyx_v_i;
                                 __pyx_t_15 = __pyx_v_label_j;
                                 *((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_inner_sum.data + __pyx_t_16 * __pyx_v_inner_sum.strides[0]) )) + __pyx_t_15)) )) += (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_kernel_matrix.data + __pyx_t_14 * __pyx_v_kernel_matrix.strides[0]) )) + __pyx_t_10)) )));
 
-                                /* "KKMeans/elkan.pyx":254
+                                /* "KKMeans/elkan.pyx":263
  *             label_j = labels[j]
  *             outer_sum[i, label_j] += kernel_matrix[i, j]
  *             if label_i == label_j:             # <<<<<<<<<<<<<<
  *                 inner_sum[i, label_j] += kernel_matrix[i, j]
  *     return np.asarray(outer_sum), np.sum(inner_sum, axis=0)
  */
                               }
@@ -20336,15 +20400,15 @@
             #undef likely
             #undef unlikely
             #define likely(x)   __builtin_expect(!!(x), 1)
             #define unlikely(x) __builtin_expect(!!(x), 0)
         #endif
       }
 
-      /* "KKMeans/elkan.pyx":249
+      /* "KKMeans/elkan.pyx":258
  *         Py_ssize_t i,j
  *         int label_i, label_j
  *     for i in prange(rows, nogil=True):             # <<<<<<<<<<<<<<
  *         label_i = labels[i]
  *         for j in range(cols):
  */
       /*finally:*/ {
@@ -20355,28 +20419,28 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "KKMeans/elkan.pyx":256
+  /* "KKMeans/elkan.pyx":265
  *             if label_i == label_j:
  *                 inner_sum[i, label_j] += kernel_matrix[i, j]
  *     return np.asarray(outer_sum), np.sum(inner_sum, axis=0)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_outer_sum, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_outer_sum, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_18 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -20387,56 +20451,56 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_18, 1+__pyx_t_18);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_inner_sum, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_inner_sum, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 256, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 256, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_axis, __pyx_int_0) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_5);
   __pyx_t_1 = 0;
   __pyx_t_5 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans/elkan.pyx":228
+  /* "KKMeans/elkan.pyx":234
  * 
  * 
- * def _calc_sums_full(double[:, ::1] kernel_matrix, long[::1] labels, long n_clusters):             # <<<<<<<<<<<<<<
- *     '''
- *     Mathematical helper function
+ * def _calc_sums_full(             # <<<<<<<<<<<<<<
+ *         double[:, ::1] kernel_matrix,
+ *         long[::1] labels,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -20449,15 +20513,15 @@
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_inner_sum, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_outer_sum, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans/elkan.pyx":259
+/* "KKMeans/elkan.pyx":268
  * 
  * 
  * cpdef double _calc_outer_sum_single(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         long elem_index,
  */
 
@@ -20476,85 +20540,85 @@
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   Py_ssize_t __pyx_t_6;
 
-  /* "KKMeans/elkan.pyx":271
+  /* "KKMeans/elkan.pyx":280
  *     '''
  *     cdef:
  *         double outer_sum = 0.             # <<<<<<<<<<<<<<
  *         Py_ssize_t i
  *         Py_ssize_t size = len(labels)
  */
   __pyx_v_outer_sum = 0.;
 
-  /* "KKMeans/elkan.pyx":273
+  /* "KKMeans/elkan.pyx":282
  *         double outer_sum = 0.
  *         Py_ssize_t i
  *         Py_ssize_t size = len(labels)             # <<<<<<<<<<<<<<
  *     for i in range(size):
  *         if labels[i] == cluster_index:
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_labels); 
   __pyx_v_size = __pyx_t_1;
 
-  /* "KKMeans/elkan.pyx":274
+  /* "KKMeans/elkan.pyx":283
  *         Py_ssize_t i
  *         Py_ssize_t size = len(labels)
  *     for i in range(size):             # <<<<<<<<<<<<<<
  *         if labels[i] == cluster_index:
  *             outer_sum += kernel_matrix[elem_index, i]
  */
   __pyx_t_1 = __pyx_v_size;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "KKMeans/elkan.pyx":275
+    /* "KKMeans/elkan.pyx":284
  *         Py_ssize_t size = len(labels)
  *     for i in range(size):
  *         if labels[i] == cluster_index:             # <<<<<<<<<<<<<<
  *             outer_sum += kernel_matrix[elem_index, i]
  *     return outer_sum
  */
     __pyx_t_4 = __pyx_v_i;
     __pyx_t_5 = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_labels.data) + __pyx_t_4)) ))) == __pyx_v_cluster_index);
     if (__pyx_t_5) {
 
-      /* "KKMeans/elkan.pyx":276
+      /* "KKMeans/elkan.pyx":285
  *     for i in range(size):
  *         if labels[i] == cluster_index:
  *             outer_sum += kernel_matrix[elem_index, i]             # <<<<<<<<<<<<<<
  *     return outer_sum
  */
       __pyx_t_4 = __pyx_v_elem_index;
       __pyx_t_6 = __pyx_v_i;
       __pyx_v_outer_sum = (__pyx_v_outer_sum + (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_kernel_matrix.data + __pyx_t_4 * __pyx_v_kernel_matrix.strides[0]) )) + __pyx_t_6)) ))));
 
-      /* "KKMeans/elkan.pyx":275
+      /* "KKMeans/elkan.pyx":284
  *         Py_ssize_t size = len(labels)
  *     for i in range(size):
  *         if labels[i] == cluster_index:             # <<<<<<<<<<<<<<
  *             outer_sum += kernel_matrix[elem_index, i]
  *     return outer_sum
  */
     }
   }
 
-  /* "KKMeans/elkan.pyx":277
+  /* "KKMeans/elkan.pyx":286
  *         if labels[i] == cluster_index:
  *             outer_sum += kernel_matrix[elem_index, i]
  *     return outer_sum             # <<<<<<<<<<<<<<
  */
   __pyx_r = __pyx_v_outer_sum;
   goto __pyx_L0;
 
-  /* "KKMeans/elkan.pyx":259
+  /* "KKMeans/elkan.pyx":268
  * 
  * 
  * cpdef double _calc_outer_sum_single(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         long elem_index,
  */
 
@@ -20611,58 +20675,58 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kernel_matrix)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 259, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_elem_index)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 259, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_calc_outer_sum_single", 1, 4, 4, 1); __PYX_ERR(0, 259, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calc_outer_sum_single", 1, 4, 4, 1); __PYX_ERR(0, 268, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cluster_index)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 259, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_calc_outer_sum_single", 1, 4, 4, 2); __PYX_ERR(0, 259, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calc_outer_sum_single", 1, 4, 4, 2); __PYX_ERR(0, 268, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 259, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_calc_outer_sum_single", 1, 4, 4, 3); __PYX_ERR(0, 259, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_calc_outer_sum_single", 1, 4, 4, 3); __PYX_ERR(0, 268, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_calc_outer_sum_single") < 0)) __PYX_ERR(0, 259, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_calc_outer_sum_single") < 0)) __PYX_ERR(0, 268, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
-    __pyx_v_kernel_matrix = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_kernel_matrix.memview)) __PYX_ERR(0, 260, __pyx_L3_error)
-    __pyx_v_elem_index = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v_elem_index == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 261, __pyx_L3_error)
-    __pyx_v_cluster_index = __Pyx_PyInt_As_long(values[2]); if (unlikely((__pyx_v_cluster_index == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 262, __pyx_L3_error)
-    __pyx_v_labels = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels.memview)) __PYX_ERR(0, 263, __pyx_L3_error)
+    __pyx_v_kernel_matrix = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_kernel_matrix.memview)) __PYX_ERR(0, 269, __pyx_L3_error)
+    __pyx_v_elem_index = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v_elem_index == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 270, __pyx_L3_error)
+    __pyx_v_cluster_index = __Pyx_PyInt_As_long(values[2]); if (unlikely((__pyx_v_cluster_index == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 271, __pyx_L3_error)
+    __pyx_v_labels = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels.memview)) __PYX_ERR(0, 272, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_calc_outer_sum_single", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 259, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_calc_outer_sum_single", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 268, __pyx_L3_error)
   __pyx_L3_error:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_kernel_matrix, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_labels, 1);
   __Pyx_AddTraceback("KKMeans.elkan._calc_outer_sum_single", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -20681,18 +20745,18 @@
   double __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_calc_outer_sum_single", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_kernel_matrix.memview)) { __Pyx_RaiseUnboundLocalError("kernel_matrix"); __PYX_ERR(0, 259, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_labels.memview)) { __Pyx_RaiseUnboundLocalError("labels"); __PYX_ERR(0, 259, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_f_7KKMeans_5elkan__calc_outer_sum_single(__pyx_v_kernel_matrix, __pyx_v_elem_index, __pyx_v_cluster_index, __pyx_v_labels, 0); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 259, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
+  if (unlikely(!__pyx_v_kernel_matrix.memview)) { __Pyx_RaiseUnboundLocalError("kernel_matrix"); __PYX_ERR(0, 268, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_labels.memview)) { __Pyx_RaiseUnboundLocalError("labels"); __PYX_ERR(0, 268, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_f_7KKMeans_5elkan__calc_outer_sum_single(__pyx_v_kernel_matrix, __pyx_v_elem_index, __pyx_v_cluster_index, __pyx_v_labels, 0); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -21819,16 +21883,16 @@
     {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 77, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 95, __pyx_L1_error)
   __pyx_builtin___import__ = __Pyx_GetBuiltinName(__pyx_n_s_import); if (!__pyx_builtin___import__) __PYX_ERR(1, 100, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 156, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 159, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 408, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 618, __pyx_L1_error)
@@ -21988,88 +22052,88 @@
  *         double[:, ::1] l_bounds,
  */
   __pyx_tuple__20 = PyTuple_Pack(11, __pyx_n_s_kernel_matrix, __pyx_n_s_l_bounds, __pyx_n_s_center_dists, __pyx_n_s_labels, __pyx_n_s_labels_old, __pyx_n_s_sizes, __pyx_n_s_sizes_old, __pyx_n_s_inner_sums, __pyx_n_s_n_clusters, __pyx_n_s_inner_sums_old, __pyx_n_s_inner_sums_mixed); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
   __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(9, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_update_elkan, 4, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 4, __pyx_L1_error)
 
-  /* "KKMeans/elkan.pyx":55
+  /* "KKMeans/elkan.pyx":61
  * 
  * 
  * def _est_lower_bounds(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         double[:, ::1] l_bounds,
  */
-  __pyx_tuple__22 = PyTuple_Pack(10, __pyx_n_s_kernel_matrix, __pyx_n_s_l_bounds, __pyx_n_s_center_dists, __pyx_n_s_labels, __pyx_n_s_sizes, __pyx_n_s_inner_sums, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_labels_i, __pyx_n_s_outer_sum); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(10, __pyx_n_s_kernel_matrix, __pyx_n_s_l_bounds, __pyx_n_s_center_dists, __pyx_n_s_labels, __pyx_n_s_sizes, __pyx_n_s_inner_sums, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_labels_i, __pyx_n_s_outer_sum); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_est_lower_bounds, 55, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_est_lower_bounds, 61, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 61, __pyx_L1_error)
 
-  /* "KKMeans/elkan.pyx":99
+  /* "KKMeans/elkan.pyx":105
  * 
  * 
  * def _calc_center_dists(             # <<<<<<<<<<<<<<
  *         double[::1] inner_sums_new,
  *         double[::1] inner_sums_mixed,
  */
-  __pyx_tuple__24 = PyTuple_Pack(13, __pyx_n_s_inner_sums_new, __pyx_n_s_inner_sums_mixed, __pyx_n_s_inner_sums_old, __pyx_n_s_sizes_new, __pyx_n_s_sizes_old, __pyx_n_s_i, __pyx_n_s_n_clusters, __pyx_n_s_dists, __pyx_n_s_new_size, __pyx_n_s_old_size, __pyx_n_s_mixed_sum, __pyx_n_s_new_sum, __pyx_n_s_old_sum); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(13, __pyx_n_s_inner_sums_new, __pyx_n_s_inner_sums_mixed, __pyx_n_s_inner_sums_old, __pyx_n_s_sizes_new, __pyx_n_s_sizes_old, __pyx_n_s_i, __pyx_n_s_n_clusters, __pyx_n_s_dists, __pyx_n_s_new_size, __pyx_n_s_old_size, __pyx_n_s_mixed_sum, __pyx_n_s_new_sum, __pyx_n_s_old_sum); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_calc_center_dists, 99, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_calc_center_dists, 105, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 105, __pyx_L1_error)
 
-  /* "KKMeans/elkan.pyx":142
+  /* "KKMeans/elkan.pyx":148
  * 
  * 
  * def _calc_inner_sums_mixed(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         long[::1] labels,
  */
-  __pyx_tuple__26 = PyTuple_Pack(11, __pyx_n_s_kernel_matrix, __pyx_n_s_labels, __pyx_n_s_labels_old, __pyx_n_s_n_clusters, __pyx_n_s_return_inner_new, __pyx_n_s_size, __pyx_n_s_sums_mixed, __pyx_n_s_sums_new, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_labels_i); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(11, __pyx_n_s_kernel_matrix, __pyx_n_s_labels, __pyx_n_s_labels_old, __pyx_n_s_n_clusters, __pyx_n_s_return_inner_new, __pyx_n_s_size, __pyx_n_s_sums_mixed, __pyx_n_s_sums_new, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_labels_i); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_calc_inner_sums_mixed, 142, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 142, __pyx_L1_error)
-  __pyx_tuple__28 = PyTuple_Pack(1, ((PyObject *)Py_True)); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_calc_inner_sums_mixed, 148, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(1, ((PyObject *)Py_True)); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
 
-  /* "KKMeans/elkan.pyx":182
+  /* "KKMeans/elkan.pyx":188
  * 
  * 
  * def start_elkan(             # <<<<<<<<<<<<<<
  *         sq_distances,
  *         double[:, ::1] kernel_matrix,
  */
-  __pyx_tuple__29 = PyTuple_Pack(11, __pyx_n_s_sq_distances, __pyx_n_s_kernel_matrix, __pyx_n_s_labels, __pyx_n_s_n_clusters, __pyx_n_s_cluster_sizes, __pyx_n_s_cluster, __pyx_n_s_outer_sums, __pyx_n_s_inner_sums, __pyx_n_s_size, __pyx_n_s_outer_sum, __pyx_n_s_inner_sum); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(11, __pyx_n_s_sq_distances, __pyx_n_s_kernel_matrix, __pyx_n_s_labels, __pyx_n_s_n_clusters, __pyx_n_s_cluster_sizes, __pyx_n_s_cluster, __pyx_n_s_outer_sums, __pyx_n_s_inner_sums, __pyx_n_s_size, __pyx_n_s_outer_sum, __pyx_n_s_inner_sum); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_start_elkan, 182, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_start_elkan, 188, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 188, __pyx_L1_error)
 
-  /* "KKMeans/elkan.pyx":228
+  /* "KKMeans/elkan.pyx":234
  * 
  * 
- * def _calc_sums_full(double[:, ::1] kernel_matrix, long[::1] labels, long n_clusters):             # <<<<<<<<<<<<<<
- *     '''
- *     Mathematical helper function
+ * def _calc_sums_full(             # <<<<<<<<<<<<<<
+ *         double[:, ::1] kernel_matrix,
+ *         long[::1] labels,
  */
-  __pyx_tuple__31 = PyTuple_Pack(11, __pyx_n_s_kernel_matrix, __pyx_n_s_labels, __pyx_n_s_n_clusters, __pyx_n_s_rows, __pyx_n_s_cols, __pyx_n_s_inner_sum, __pyx_n_s_outer_sum, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_label_i, __pyx_n_s_label_j); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(11, __pyx_n_s_kernel_matrix, __pyx_n_s_labels, __pyx_n_s_n_clusters, __pyx_n_s_rows, __pyx_n_s_cols, __pyx_n_s_inner_sum, __pyx_n_s_outer_sum, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_label_i, __pyx_n_s_label_j); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_calc_sums_full, 228, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_calc_sums_full, 234, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 234, __pyx_L1_error)
 
-  /* "KKMeans/elkan.pyx":259
+  /* "KKMeans/elkan.pyx":268
  * 
  * 
  * cpdef double _calc_outer_sum_single(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         long elem_index,
  */
-  __pyx_tuple__33 = PyTuple_Pack(4, __pyx_n_s_kernel_matrix, __pyx_n_s_elem_index, __pyx_n_s_cluster_index, __pyx_n_s_labels); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(4, __pyx_n_s_kernel_matrix, __pyx_n_s_elem_index, __pyx_n_s_cluster_index, __pyx_n_s_labels); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_calc_outer_sum_single, 259, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_elkan_pyx, __pyx_n_s_calc_outer_sum_single, 268, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -23145,85 +23209,85 @@
  *         double[:, ::1] l_bounds,
  */
   __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_1update_elkan, 0, __pyx_n_s_update_elkan, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_update_elkan, __pyx_t_7) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "KKMeans/elkan.pyx":55
+  /* "KKMeans/elkan.pyx":61
  * 
  * 
  * def _est_lower_bounds(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         double[:, ::1] l_bounds,
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_3_est_lower_bounds, 0, __pyx_n_s_est_lower_bounds, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_3_est_lower_bounds, 0, __pyx_n_s_est_lower_bounds, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_est_lower_bounds, __pyx_t_7) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_est_lower_bounds, __pyx_t_7) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "KKMeans/elkan.pyx":99
+  /* "KKMeans/elkan.pyx":105
  * 
  * 
  * def _calc_center_dists(             # <<<<<<<<<<<<<<
  *         double[::1] inner_sums_new,
  *         double[::1] inner_sums_mixed,
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_5_calc_center_dists, 0, __pyx_n_s_calc_center_dists, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_5_calc_center_dists, 0, __pyx_n_s_calc_center_dists, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_center_dists, __pyx_t_7) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_center_dists, __pyx_t_7) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "KKMeans/elkan.pyx":142
+  /* "KKMeans/elkan.pyx":148
  * 
  * 
  * def _calc_inner_sums_mixed(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         long[::1] labels,
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_7_calc_inner_sums_mixed, 0, __pyx_n_s_calc_inner_sums_mixed, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_7_calc_inner_sums_mixed, 0, __pyx_n_s_calc_inner_sums_mixed, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_tuple__28);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_inner_sums_mixed, __pyx_t_7) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_inner_sums_mixed, __pyx_t_7) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "KKMeans/elkan.pyx":182
+  /* "KKMeans/elkan.pyx":188
  * 
  * 
  * def start_elkan(             # <<<<<<<<<<<<<<
  *         sq_distances,
  *         double[:, ::1] kernel_matrix,
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_9start_elkan, 0, __pyx_n_s_start_elkan, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_9start_elkan, 0, __pyx_n_s_start_elkan, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_start_elkan, __pyx_t_7) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_start_elkan, __pyx_t_7) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "KKMeans/elkan.pyx":228
+  /* "KKMeans/elkan.pyx":234
  * 
  * 
- * def _calc_sums_full(double[:, ::1] kernel_matrix, long[::1] labels, long n_clusters):             # <<<<<<<<<<<<<<
- *     '''
- *     Mathematical helper function
+ * def _calc_sums_full(             # <<<<<<<<<<<<<<
+ *         double[:, ::1] kernel_matrix,
+ *         long[::1] labels,
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_11_calc_sums_full, 0, __pyx_n_s_calc_sums_full, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_11_calc_sums_full, 0, __pyx_n_s_calc_sums_full, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_sums_full, __pyx_t_7) < 0) __PYX_ERR(0, 228, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_sums_full, __pyx_t_7) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "KKMeans/elkan.pyx":259
+  /* "KKMeans/elkan.pyx":268
  * 
  * 
  * cpdef double _calc_outer_sum_single(             # <<<<<<<<<<<<<<
  *         double[:, ::1] kernel_matrix,
  *         long elem_index,
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_13_calc_outer_sum_single, 0, __pyx_n_s_calc_outer_sum_single, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_5elkan_13_calc_outer_sum_single, 0, __pyx_n_s_calc_outer_sum_single, NULL, __pyx_n_s_KKMeans_elkan, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_outer_sum_single, __pyx_t_7) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_outer_sum_single, __pyx_t_7) < 0) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "KKMeans/elkan.pyx":1
  * import numpy as np             # <<<<<<<<<<<<<<
  * from cython.parallel import prange
  * from libc.math cimport sqrt
  */
```

### Comparing `KKMeans-0.0.6/src/KKMeans/elkan.pyx` & `KKMeans-0.0.7/src/KKMeans/elkan.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,24 @@
     sizes: ndarray of shape(n_clusters)
     center_dists: ndarray of shape(n_clusters, n_clusters)
         updated center_dists
     '''
 
 
     inner_sums_old = inner_sums
-    inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(kernel_matrix, labels, labels_old, 
-                                                          n_clusters, return_inner_new=True)
-    center_dists += _calc_center_dists(inner_sums, inner_sums_mixed, inner_sums_old, sizes, sizes_old)
-    l_bounds = _est_lower_bounds(kernel_matrix, l_bounds, center_dists, labels, sizes, inner_sums)
+    inner_sums_mixed, inner_sums = _calc_inner_sums_mixed(
+        kernel_matrix, labels, labels_old, 
+        n_clusters, return_inner_new=True)
+    center_dists += _calc_center_dists(
+        inner_sums, inner_sums_mixed, 
+        inner_sums_old, sizes, sizes_old)
+    l_bounds = _est_lower_bounds(
+        kernel_matrix, l_bounds, 
+        center_dists, labels, 
+        sizes, inner_sums)
     return np.asarray(l_bounds), np.asarray(inner_sums), np.asarray(sizes), np.asarray(center_dists)
 
 
 def _est_lower_bounds(
         double[:, ::1] kernel_matrix, 
         double[:, ::1] l_bounds, 
         double[:, ::1] center_dists, 
@@ -221,15 +227,18 @@
         outer_sum = outer_sums[:, cluster]
         inner_sum = inner_sums[cluster] 
         sq_distances[:,  cluster] += (-2 * outer_sum / size 
                                      + inner_sum / size**2)
     return np.asarray(sq_distances), np.asarray(inner_sums), np.asarray(cluster_sizes)
 
 
-def _calc_sums_full(double[:, ::1] kernel_matrix, long[::1] labels, long n_clusters):
+def _calc_sums_full(
+        double[:, ::1] kernel_matrix, 
+        long[::1] labels, 
+        long n_clusters):
     '''
     Mathematical helper function
 
     Returns
     -------
     outer_sums: ndarray of shape(n_samples, n_clusters)
         outer_sums[i, j] == sum(K(data[i], data[x])) for x in cluster j
```

### Comparing `KKMeans-0.0.6/src/KKMeans/kernels.c` & `KKMeans-0.0.7/src/KKMeans/kernels.c`

 * *Files 0% similar despite different names*

```diff
@@ -17115,15 +17115,15 @@
 static PyObject *__pyx_pw_7KKMeans_7kernels_1build_kernel_matrix(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7KKMeans_7kernels_build_kernel_matrix, "\n    wrapper function to build kernel matrix\n\n    Parameters\n    ----------\n    X: ndarray of shape(n_samples, n_features), dtype=np.double\n        data to build kernel matrix upon\n    Y: ndarray of shape(*, n_features), dtype=np.double, optional\n        If None, Y=X. data to compute kernel matrix \n        against, eg kernel_matrix[i,j] = K(X[i], Y[j])\n        Y=X leads to expected behaviour\n    kernel: {\"linear\", \"rbf\", \"gaussian\", \"polynomial\", \"sigmoid\", \"laplacian\"}\n            default=\"linear\"\n    gamma: double, default=1\n        param for kernel\n    c_0: double, default=0\n        param for kernel\n    d: double, default=3\n        param for kernel\n    variance: double, default=1\n        param for gaussian kernel.\n        is passed to rbf with gamma=1/variance\n    \n    Returns\n    -------\n    kernel_matrix: ndarray, dtype=np.double \n        of shape(len(X), len(X)) if Y=None\n        of shape(len(X), len(Y)) else\n    ");
+PyDoc_STRVAR(__pyx_doc_7KKMeans_7kernels_build_kernel_matrix, "\n    wrapper function to build kernel matrix\n\n    Parameters\n    ----------\n    X: ndarray of shape(n_samples, n_features), dtype=np.double\n        data to build kernel matrix from\n    Y: ndarray of shape(*, n_features), dtype=np.double, optional\n        If None, Y=X. data to compute kernel matrix \n        against, eg kernel_matrix[i,j] = K(X[i], Y[j])\n        Y=X leads to expected behaviour\n    kernel: {\"linear\", \"rbf\", \"gaussian\", \"polynomial\", \"sigmoid\", \"laplacian\"}\n            default=\"linear\"\n    gamma: double, default=1\n        param for kernel\n    c_0: double, default=0\n        param for kernel\n    d: double, default=3\n        param for kernel\n    variance: double, default=1\n        param for gaussian kernel.\n        is passed to rbf with gamma=1/variance\n    \n    Returns\n    -------\n    kernel_matrix: ndarray, dtype=np.double \n        of shape(len(X), len(X)) if Y=None\n        of shape(len(X), len(Y)) else\n    ");
 static PyMethodDef __pyx_mdef_7KKMeans_7kernels_1build_kernel_matrix = {"build_kernel_matrix", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7KKMeans_7kernels_1build_kernel_matrix, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7KKMeans_7kernels_build_kernel_matrix};
 static PyObject *__pyx_pw_7KKMeans_7kernels_1build_kernel_matrix(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
```

### Comparing `KKMeans-0.0.6/src/KKMeans/kernels.pyx` & `KKMeans-0.0.7/src/KKMeans/kernels.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def build_kernel_matrix(X, Y=None, kernel="linear", gamma=1, c_0=0, d=3, variance=1):
     '''
     wrapper function to build kernel matrix
 
     Parameters
     ----------
     X: ndarray of shape(n_samples, n_features), dtype=np.double
-        data to build kernel matrix upon
+        data to build kernel matrix from
     Y: ndarray of shape(*, n_features), dtype=np.double, optional
         If None, Y=X. data to compute kernel matrix 
         against, eg kernel_matrix[i,j] = K(X[i], Y[j])
         Y=X leads to expected behaviour
     kernel: {"linear", "rbf", "gaussian", "polynomial", "sigmoid", "laplacian"}
             default="linear"
     gamma: double, default=1
```

### Comparing `KKMeans-0.0.6/src/KKMeans/lloyd.c` & `KKMeans-0.0.7/src/KKMeans/lloyd.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 /* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "extra_compile_args": [
-            "/O2",
-            "-DCYTHON_WITHOUT_ASSERTIONS",
-            "/openmp"
+            "-DCYTHON_WITHOUT_ASSERTIONS"
         ],
         "name": "KKMeans.lloyd",
         "sources": [
             "src/KKMeans/lloyd.pyx"
         ]
     },
     "module_name": "KKMeans.lloyd"
```

### Comparing `KKMeans-0.0.6/src/KKMeans/lloyd.pyx` & `KKMeans-0.0.7/src/KKMeans/lloyd.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.6/src/KKMeans/quality.c` & `KKMeans-0.0.7/src/KKMeans/quality.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.6/src/KKMeans/quality.pyx` & `KKMeans-0.0.7/src/KKMeans/quality.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.6/src/KKMeans/utils.c` & `KKMeans-0.0.7/src/KKMeans/utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 /* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "extra_compile_args": [
-            "/O2",
-            "-DCYTHON_WITHOUT_ASSERTIONS",
-            "/openmp"
+            "-DCYTHON_WITHOUT_ASSERTIONS"
         ],
         "name": "KKMeans.utils",
         "sources": [
             "src/KKMeans/utils.pyx"
         ]
     },
     "module_name": "KKMeans.utils"
```

### Comparing `KKMeans-0.0.6/src/KKMeans/utils.pyx` & `KKMeans-0.0.7/src/KKMeans/utils.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.6/tests/test_pytest_utils.py` & `KKMeans-0.0.7/tests/test_pytest_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 import pytest
 import tests.pytest_utils as pu
 import numpy as np
 from sklearn.neighbors import NearestCentroid
 from sklearn.datasets import make_blobs
 
-@pytest.mark.parametrize("n_samples", [100,1000])
-@pytest.mark.parametrize("n_clusters", [2,10])
+
+@pytest.mark.parametrize("n_samples", [100, 1000])
+@pytest.mark.parametrize("n_clusters", [2, 10])
 @pytest.mark.parametrize("n_features", [1, 100])
 def test_ctrl_centers_linear(n_samples, n_clusters, n_features):
     data, labels = make_blobs(n_samples, n_features, centers=n_clusters)
     ctrl = NearestCentroid()
     ctrl.fit(data, labels)
-    assert np.allclose(pu.ctrl_centers_linear(data, labels, n_clusters, n_features), ctrl.centroids_)
+    assert np.allclose(
+        pu.ctrl_centers_linear(data, labels, n_clusters, n_features), ctrl.centroids_
+    )
+
 
 def test_ctrl_cluster_sizes():
     sizes = np.asarray([10, 100, 1000, 7])
     labels = list()
     for i in range(len(sizes)):
         labels += [i] * sizes[i]
     pu.RNG.shuffle(labels)
     assert all(sizes == pu.ctrl_cluster_sizes(labels, 4))
 
+
 def test_ctrl_outer_sums():
     km = [
-        [0,1, 2],
+        [0, 1, 2],
         [-2, 0, 3],
         [-1, 1, 0],
     ]
     km = np.asarray(km)
     labels = np.asarray([1, 0, 1])
     outer_sums = [
         [1, 2],
         [0, 1],
         [1, -1],
     ]
     assert np.allclose(pu.ctrl_outer_sums(km, labels, 2), outer_sums)
 
+
 def test_ctrl_inner_sums():
     km = [
-        [0,1, 2],
+        [0, 1, 2],
         [-2, 0, 3],
         [-1, 1, 0],
     ]
     km = np.asarray(km)
     labels = [1, 0, 1]
     labels = np.asarray(labels)
-    inner_sums = [0. ,1.]
-    assert np.allclose(pu.ctrl_inner_sums(km, labels, 2), inner_sums)
+    inner_sums = [0.0, 1.0]
+    assert np.allclose(pu.ctrl_inner_sums(km, labels, 2), inner_sums)
```

