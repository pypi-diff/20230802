# Comparing `tmp/mistree-1.2.1.tar.gz` & `tmp/mistree-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistree-1.2.1.tar", last modified: Mon Mar 27 13:26:03 2023, max compression
+gzip compressed data, was "mistree-1.2.2.tar", last modified: Wed Aug  2 18:43:12 2023, max compression
```

## Comparing `mistree-1.2.1.tar` & `mistree-1.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 krishna    (501) staff       (20)        0 2023-03-27 13:26:03.146764 mistree-1.2.1/
--rw-r--r--   0 krishna    (501) staff       (20)     1058 2023-03-27 13:12:44.000000 mistree-1.2.1/LICENSE.txt
--rw-r--r--   0 krishna    (501) staff       (20)     6229 2023-03-27 13:26:03.146259 mistree-1.2.1/PKG-INFO
--rw-r--r--   0 krishna    (501) staff       (20)     4997 2023-03-27 13:12:44.000000 mistree-1.2.1/README.md
-drwxr-xr-x   0 krishna    (501) staff       (20)        0 2023-03-27 13:26:03.133637 mistree-1.2.1/mistree/
--rw-r--r--   0 krishna    (501) staff       (20)     1947 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/__init__.py
-drwxr-xr-x   0 krishna    (501) staff       (20)        0 2023-03-27 13:26:03.136354 mistree-1.2.1/mistree/coordinates/
--rw-r--r--   0 krishna    (501) staff       (20)      283 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/coordinates/__init__.py
--rw-r--r--   0 krishna    (501) staff       (20)     4728 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/coordinates/coordinate_utility.py
-drwxr-xr-x   0 krishna    (501) staff       (20)        0 2023-03-27 13:26:03.138065 mistree-1.2.1/mistree/levy_flight/
--rw-r--r--   0 krishna    (501) staff       (20)      134 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/levy_flight/__init__.py
--rw-r--r--   0 krishna    (501) staff       (20)     6523 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/levy_flight/levy_flight.py
--rw-r--r--   0 krishna    (501) staff       (20)     4863 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/levy_flight/utility_random_walk.f90
-drwxr-xr-x   0 krishna    (501) staff       (20)        0 2023-03-27 13:26:03.145516 mistree-1.2.1/mistree/mst/
--rw-r--r--   0 krishna    (501) staff       (20)     1211 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/__init__.py
--rw-r--r--   0 krishna    (501) staff       (20)    16855 2023-03-27 13:24:24.000000 mistree-1.2.1/mistree/mst/branches.py
--rw-r--r--   0 krishna    (501) staff       (20)     3096 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/construct.py
--rw-r--r--   0 krishna    (501) staff       (20)     2428 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/density.py
--rw-r--r--   0 krishna    (501) staff       (20)    26081 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/get_mst_class.py
--rw-r--r--   0 krishna    (501) staff       (20)     1300 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/graph.py
--rw-r--r--   0 krishna    (501) staff       (20)     9334 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/hist_mst.py
--rw-r--r--   0 krishna    (501) staff       (20)     1778 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/partition.py
--rw-r--r--   0 krishna    (501) staff       (20)    37454 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/plot_mst.py
--rw-r--r--   0 krishna    (501) staff       (20)     2443 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/scale_cut.py
--rw-r--r--   0 krishna    (501) staff       (20)     1911 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/stats.py
--rw-r--r--   0 krishna    (501) staff       (20)     1194 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/tomo.py
--rw-r--r--   0 krishna    (501) staff       (20)     6880 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/utility_density.f90
--rw-r--r--   0 krishna    (501) staff       (20)     1296 2023-03-27 13:12:44.000000 mistree-1.2.1/mistree/mst/utility_mst.f90
-drwxr-xr-x   0 krishna    (501) staff       (20)        0 2023-03-27 13:26:03.135463 mistree-1.2.1/mistree.egg-info/
--rw-r--r--   0 krishna    (501) staff       (20)     6229 2023-03-27 13:26:03.000000 mistree-1.2.1/mistree.egg-info/PKG-INFO
--rw-r--r--   0 krishna    (501) staff       (20)      734 2023-03-27 13:26:03.000000 mistree-1.2.1/mistree.egg-info/SOURCES.txt
--rw-r--r--   0 krishna    (501) staff       (20)        1 2023-03-27 13:26:03.000000 mistree-1.2.1/mistree.egg-info/dependency_links.txt
--rw-r--r--   0 krishna    (501) staff       (20)       36 2023-03-27 13:26:03.000000 mistree-1.2.1/mistree.egg-info/requires.txt
--rw-r--r--   0 krishna    (501) staff       (20)        8 2023-03-27 13:26:03.000000 mistree-1.2.1/mistree.egg-info/top_level.txt
--rw-r--r--   0 krishna    (501) staff       (20)       38 2023-03-27 13:26:03.146944 mistree-1.2.1/setup.cfg
--rw-r--r--   0 krishna    (501) staff       (20)     2488 2023-03-27 13:24:24.000000 mistree-1.2.1/setup.py
+drwxr-xr-x   0 krishna    (501) staff       (20)        0 2023-08-02 18:43:12.353937 mistree-1.2.2/
+-rw-r--r--   0 krishna    (501) staff       (20)     1058 2023-03-27 13:12:44.000000 mistree-1.2.2/LICENSE.txt
+-rw-r--r--   0 krishna    (501) staff       (20)     6279 2023-08-02 18:43:12.353495 mistree-1.2.2/PKG-INFO
+-rw-r--r--   0 krishna    (501) staff       (20)     4997 2023-08-02 18:37:54.000000 mistree-1.2.2/README.md
+drwxr-xr-x   0 krishna    (501) staff       (20)        0 2023-08-02 18:43:12.339372 mistree-1.2.2/mistree/
+-rw-r--r--   0 krishna    (501) staff       (20)     1947 2023-03-27 13:12:44.000000 mistree-1.2.2/mistree/__init__.py
+drwxr-xr-x   0 krishna    (501) staff       (20)        0 2023-08-02 18:43:12.342879 mistree-1.2.2/mistree/coordinates/
+-rw-r--r--   0 krishna    (501) staff       (20)      283 2023-03-27 13:12:44.000000 mistree-1.2.2/mistree/coordinates/__init__.py
+-rw-r--r--   0 krishna    (501) staff       (20)     4728 2023-08-02 18:37:54.000000 mistree-1.2.2/mistree/coordinates/coordinate_utility.py
+drwxr-xr-x   0 krishna    (501) staff       (20)        0 2023-08-02 18:43:12.344660 mistree-1.2.2/mistree/levy_flight/
+-rw-r--r--   0 krishna    (501) staff       (20)      134 2023-03-27 13:12:44.000000 mistree-1.2.2/mistree/levy_flight/__init__.py
+-rw-r--r--   0 krishna    (501) staff       (20)     6523 2023-08-02 18:37:54.000000 mistree-1.2.2/mistree/levy_flight/levy_flight.py
+-rw-r--r--   0 krishna    (501) staff       (20)     4863 2023-03-27 13:12:44.000000 mistree-1.2.2/mistree/levy_flight/utility_random_walk.f90
+drwxr-xr-x   0 krishna    (501) staff       (20)        0 2023-08-02 18:43:12.352843 mistree-1.2.2/mistree/mst/
+-rw-r--r--   0 krishna    (501) staff       (20)     1211 2023-03-27 13:12:44.000000 mistree-1.2.2/mistree/mst/__init__.py
+-rw-r--r--   0 krishna    (501) staff       (20)    16879 2023-08-02 18:37:54.000000 mistree-1.2.2/mistree/mst/branches.py
+-rw-r--r--   0 krishna    (501) staff       (20)     3096 2023-08-02 18:37:54.000000 mistree-1.2.2/mistree/mst/construct.py
+-rw-r--r--   0 krishna    (501) staff       (20)     2428 2023-08-02 18:37:54.000000 mistree-1.2.2/mistree/mst/density.py
+-rw-r--r--   0 krishna    (501) staff       (20)    26077 2023-08-02 18:37:54.000000 mistree-1.2.2/mistree/mst/get_mst_class.py
+-rw-r--r--   0 krishna    (501) staff       (20)     1300 2023-03-27 13:12:44.000000 mistree-1.2.2/mistree/mst/graph.py
+-rw-r--r--   0 krishna    (501) staff       (20)     9334 2023-03-27 13:12:44.000000 mistree-1.2.2/mistree/mst/hist_mst.py
+-rw-r--r--   0 krishna    (501) staff       (20)     1778 2023-03-27 13:12:44.000000 mistree-1.2.2/mistree/mst/partition.py
+-rw-r--r--   0 krishna    (501) staff       (20)    37454 2023-08-02 17:17:31.000000 mistree-1.2.2/mistree/mst/plot_mst.py
+-rw-r--r--   0 krishna    (501) staff       (20)     2443 2023-08-02 17:17:37.000000 mistree-1.2.2/mistree/mst/scale_cut.py
+-rw-r--r--   0 krishna    (501) staff       (20)     1911 2023-03-27 13:12:44.000000 mistree-1.2.2/mistree/mst/stats.py
+-rw-r--r--   0 krishna    (501) staff       (20)     1194 2023-08-02 17:18:17.000000 mistree-1.2.2/mistree/mst/tomo.py
+-rw-r--r--   0 krishna    (501) staff       (20)     6880 2023-03-27 13:12:44.000000 mistree-1.2.2/mistree/mst/utility_density.f90
+-rw-r--r--   0 krishna    (501) staff       (20)     1296 2023-03-27 13:12:44.000000 mistree-1.2.2/mistree/mst/utility_mst.f90
+drwxr-xr-x   0 krishna    (501) staff       (20)        0 2023-08-02 18:43:12.341739 mistree-1.2.2/mistree.egg-info/
+-rw-r--r--   0 krishna    (501) staff       (20)     6279 2023-08-02 18:43:12.000000 mistree-1.2.2/mistree.egg-info/PKG-INFO
+-rw-r--r--   0 krishna    (501) staff       (20)      734 2023-08-02 18:43:12.000000 mistree-1.2.2/mistree.egg-info/SOURCES.txt
+-rw-r--r--   0 krishna    (501) staff       (20)        1 2023-08-02 18:43:12.000000 mistree-1.2.2/mistree.egg-info/dependency_links.txt
+-rw-r--r--   0 krishna    (501) staff       (20)       36 2023-08-02 18:43:12.000000 mistree-1.2.2/mistree.egg-info/requires.txt
+-rw-r--r--   0 krishna    (501) staff       (20)        8 2023-08-02 18:43:12.000000 mistree-1.2.2/mistree.egg-info/top_level.txt
+-rw-r--r--   0 krishna    (501) staff       (20)       38 2023-08-02 18:43:12.354080 mistree-1.2.2/setup.cfg
+-rw-r--r--   0 krishna    (501) staff       (20)     2537 2023-08-02 18:37:54.000000 mistree-1.2.2/setup.py
```

### Comparing `mistree-1.2.1/LICENSE.txt` & `mistree-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/PKG-INFO` & `mistree-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistree
-Version: 1.2.1
+Version: 1.2.2
 Summary: A python package for constructing and analysing the minimum spanning tree
 Home-page: https://knaidoo29.github.io/mistreedoc/
 Author: Krishna Naidoo
 Author-email: krishna.naidoo.11@ucl.ac.uk
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,28 +13,29 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Fortran
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MiSTree
 
 Author:         Krishna Naidoo                          
-Version:        1.2.0                               
+Version:        1.2.2                               
 Homepage:       https://github.com/knaidoo29/mistree    
 Documentation:  https://knaidoo29.github.io/mistreedoc/
 
 [![Build Status](https://travis-ci.org/knaidoo29/mistree.svg?branch=master)](https://travis-ci.org/knaidoo29/mistree) [![codecov](https://codecov.io/gh/knaidoo29/mistree/branch/master/graph/badge.svg)](https://codecov.io/gh/knaidoo29/mistree) [![PyPI version](https://badge.fury.io/py/mistree.svg)](https://badge.fury.io/py/mistree) [![status](https://joss.theoj.org/papers/461d79e9e5faf21029c0a7b1c928be28/status.svg)](https://joss.theoj.org/papers/461d79e9e5faf21029c0a7b1c928be28) [![DOI](https://zenodo.org/badge/170473458.svg)](https://zenodo.org/badge/latestdoi/170473458) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/knaidoo29/mistree/master?filepath=tutorials%2Fnotebooks%2F)
 [![ascl](https://img.shields.io/badge/ascl-1910.016-blue.svg?colorB=262255)](http://ascl.net/1910.016)
 
 ## Introduction
```

### Comparing `mistree-1.2.1/README.md` & `mistree-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MiSTree
 
 Author:         Krishna Naidoo                          
-Version:        1.2.0                               
+Version:        1.2.2                               
 Homepage:       https://github.com/knaidoo29/mistree    
 Documentation:  https://knaidoo29.github.io/mistreedoc/
 
 [![Build Status](https://travis-ci.org/knaidoo29/mistree.svg?branch=master)](https://travis-ci.org/knaidoo29/mistree) [![codecov](https://codecov.io/gh/knaidoo29/mistree/branch/master/graph/badge.svg)](https://codecov.io/gh/knaidoo29/mistree) [![PyPI version](https://badge.fury.io/py/mistree.svg)](https://badge.fury.io/py/mistree) [![status](https://joss.theoj.org/papers/461d79e9e5faf21029c0a7b1c928be28/status.svg)](https://joss.theoj.org/papers/461d79e9e5faf21029c0a7b1c928be28) [![DOI](https://zenodo.org/badge/170473458.svg)](https://zenodo.org/badge/latestdoi/170473458) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/knaidoo29/mistree/master?filepath=tutorials%2Fnotebooks%2F)
 [![ascl](https://img.shields.io/badge/ascl-1910.016-blue.svg?colorB=262255)](http://ascl.net/1910.016)
 
 ## Introduction
```

### Comparing `mistree-1.2.1/mistree/__init__.py` & `mistree-1.2.2/mistree/__init__.py`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/mistree/coordinates/coordinate_utility.py` & `mistree-1.2.2/mistree/coordinates/coordinate_utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         Units of phi and theta given in either 'degrees' or 'radians'.
 
     Returns
     -------
     x, y, z : array
         cartesian coordinates.
     """
-    if np.isscalar(phi) is True:
+    if np.isscalar(phi) == True:
         return spherical_2_cartesian(1., phi, theta, units=units)
     else:
         return spherical_2_cartesian(np.ones(len(phi)), phi, theta, units=units)
 
 
 def celestial_2_unit_sphere(ra, dec, units='degrees', output='both'):
     """Project coordinates on a sphere into cartesian coordinates on a unit sphere.
@@ -123,15 +123,15 @@
     Returns
     -------
     phi, theta : array
         'spherical': spherical polar coordinates.
     x, y, z : array
         'cartesian': cartesian coordinates.
     """
-    if np.isscalar(ra) is True:
+    if np.isscalar(ra) == True:
         return celestial_2_cartesian(1., ra, dec, units=units, output=output)
     else:
         return celestial_2_cartesian(np.ones(len(ra)), ra, dec, units=units, output=output)
 
 
 def perpendicular_distance_2_angle(distance):
     """Converts distances on a unit sphere to angular distances projected across a unit sphere.
```

### Comparing `mistree-1.2.1/mistree/levy_flight/levy_flight.py` & `mistree-1.2.2/mistree/levy_flight/levy_flight.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     _steps : array
         Random step sizes.
     _x_start, _y_start, _z_start : float
         Starting position of the distribution.
     """
     _u = np.random.uniform(0., 1., size - 1)
     _steps = t_0 / (1. - _u) ** (1. / alpha)
-    if periodic is False:
+    if periodic == False:
         box_size = None
     if mode == '2D':
         x, y = get_random_flight(_steps, mode='2D', box_size=box_size)
         return x, y
     elif mode == '3D':
         x, y, z = get_random_flight(_steps, mode='3D', box_size=box_size)
         return x, y, z
@@ -171,15 +171,15 @@
         gamma = alpha*((1.-beta)/beta)*((t_0-t_s)/t_0)
     else:
         pass
     _u = np.random.uniform(0., 1., size - 1)
     _steps = (t_0 - t_s) * (_u / beta) ** (1. / gamma) + t_s
     condition = np.where(_u >= beta)[0]
     _steps[condition] = t_0*(1.+((beta-_u[condition])/(1.-beta)))**(-1./alpha)
-    if periodic is False:
+    if periodic == False:
         box_size = None
     if mode == '2D':
         x, y = get_random_flight(_steps, mode='2D', box_size=box_size)
         return x, y
     elif mode == '3D':
         x, y, z = get_random_flight(_steps, mode='3D', box_size=box_size)
         return x, y, z
```

### Comparing `mistree-1.2.1/mistree/levy_flight/utility_random_walk.f90` & `mistree-1.2.2/mistree/levy_flight/utility_random_walk.f90`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/mistree/mst/__init__.py` & `mistree-1.2.2/mistree/mst/__init__.py`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/mistree/mst/branches.py` & `mistree-1.2.2/mistree/mst/branches.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                                                 np.ndarray.tolist(np.ndarray.flatten(np.array(_twig)))
                         done = 1.
                     else:
                         check_end[condition] = 0.
                         _twig.append(index_branch_end[condition])
                         done = 1.
                         mask_end[condition] = False
-                        branch_index.append(np.ndarray.tolist(np.ndarray.flatten(np.array(_twig))))
+                        branch_index.append(np.ndarray.tolist(np.ndarray.flatten(np.array(_twig, dtype=object))))
                 else:
                     if len(condition) == 1:
                         check_mid[condition] = 0.
                         _twig.append(index_branch_mid[condition])
                         if index_branch_mid1[condition] == node_index:
                             node_index = index_branch_mid2[condition]
                         elif index_branch_mid2[condition] == node_index:
@@ -132,15 +132,15 @@
             mask_mid = mask_mid[mask_mid]
             count = count + 1
             item = 0
         else:
             count = count + 1
             item = item + 1
     branch_index_rejected = branch_index_rejected + np.ndarray.tolist(np.ndarray.flatten(np.array(index_branch_mid)))
-    branch_index = [np.ndarray.tolist(np.hstack(np.array(branch_index[i]))) for i in range(0, len(branch_index))]
+    branch_index = [np.ndarray.tolist(np.hstack(np.array(branch_index[i], dtype=object))) for i in range(0, len(branch_index))]
     if len(branch_index_rejected) != 0:
         branch_index_rejected = np.ndarray.tolist(np.hstack(np.array(branch_index_rejected)))
     return branch_index, branch_index_rejected
 
 
 def get_branch_index_sub_divide(sub_divisions, edge_index, edge_degree, box_size=None, edge_x=None, edge_y=None,
                                 edge_z=None, phi=None, theta=None, edge_phi=None, edge_theta=None,
@@ -185,15 +185,15 @@
     if mode == 'Euclidean':
         x_min, x_max, y_min, y_max = np.min(edge_x), np.max(edge_x), np.min(edge_y), np.max(edge_y)
         dx, dy = (x_max - x_min) / float(sub_divisions), (y_max - y_min) / float(sub_divisions)
         xx = np.arange(x_min, x_max + dx, dx)
         yy = np.arange(y_min, y_max + dy, dy)
         xx_mid = 0.5 * (xx[1:len(xx)] + xx[0:len(xx) - 1])
         yy_mid = 0.5 * (yy[1:len(yy)] + yy[0:len(yy) - 1])
-        if two_dimension is True:
+        if two_dimension == True:
             x_div, y_div = np.meshgrid(xx_mid, yy_mid, indexing='ij')
             x_div = np.ndarray.flatten(x_div)
             y_div = np.ndarray.flatten(y_div)
         else:
             z_min, z_max = np.min(edge_z), np.max(edge_z)
             dz = (z_max - z_min) / float(sub_divisions)
             zz = np.arange(z_min, z_max + dz, dz)
@@ -217,19 +217,19 @@
     if mode == 'Euclidean':
         length = len(x_div)
         total_mask = np.ones(len(edge_x[0]))
     else:
         length = len(phi_div)
         total_mask = np.ones(len(edge_phi[0]))
     for k in range(0, length):
-        if mode == 'Euclidean' and two_dimension is True:
+        if mode == 'Euclidean' and two_dimension == True:
             xd, yd = x_div[k], y_div[k]
             condition = np.where((total_mask == 1.) & ((edge_x[0] >= xd - dx / 2.) | (edge_x[0] <= xd + dx / 2.) |
                                  (edge_y[0] >= yd - dx / 2.) | (edge_y[0] <= yd + dx / 2.)))[0]
-        elif mode == 'Euclidean' and two_dimension is False:
+        elif mode == 'Euclidean' and two_dimension == False:
             xd, yd, zd = x_div[k], y_div[k], z_div[k]
             condition = np.where((total_mask == 1.) & ((edge_x[0] >= xd - dx / 2.) | (edge_x[0] <= xd + dx / 2.) |
                                  (edge_y[0] >= yd - dx / 2.) | (edge_y[0] < yd + dx / 2.) | (edge_z[0] >= zd - dx / 2.)
                                  & (edge_z[0] <= zd + dx / 2.)))[0]
         else:
             pd, td = phi_div[k], theta_div[k]
             condition = np.where((total_mask == 1.) & ((edge_phi[0] >= pd - dphi / 2.) | (edge_phi[0] <= pd + dphi / 2.)
@@ -237,15 +237,15 @@
         edge_degree_cut = np.array([edge_degree[0][condition], edge_degree[1][condition]])
         edge_index_cut = np.array([edge_index[0][condition], edge_index[1][condition]])
         branch_index_cut, branch_index_rejected_cut = \
             get_branch_index(edge_index_cut, edge_degree_cut, branch_cutting_frequency=branch_cutting_frequency)
         branch_index_cut_corrected = [np.ndarray.tolist(condition[i]) for i in branch_index_cut]
         branch_index_total = branch_index_total + branch_index_cut_corrected
         total_mask[[item for sublist in branch_index_total for item in sublist]] = 0.
-        if len(branch_index_rejected_cut) is not 0:
+        if len(branch_index_rejected_cut) != 0:
             branch_index_rejected_total = branch_index_rejected_total + \
                                           np.ndarray.tolist(condition[branch_index_rejected_cut])
         total_mask[branch_index_rejected_total] = 0.
     branch_index_rejected_total = np.array(branch_index_rejected_total)
     branch_index_rejected_total = np.unique(branch_index_rejected_total)
     if len(branch_index_rejected_total) == 0:
         pass
```

### Comparing `mistree-1.2.1/mistree/mst/construct.py` & `mistree-1.2.2/mistree/mst/construct.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,48 +32,48 @@
     edge_x, edge_y, edge_z : array
         The positional coordinates of the ends of each edge.
     edge_index : array
         The node index of the ends of each edge.
     num_removed_edges : int, optional
         Number of removed edges. Only given and applicable if scale_cut_length is given.
     """
-    if two_dimensions is True:
+    if two_dimensions == True:
         vertices = np.array([x, y]).T
     else:
         vertices = np.array([x, y, z]).T
     if scale_cut_length != 0.:
-        if two_dimensions is True:
+        if two_dimensions == True:
             x, y, k_nearest_neighbour_graph, num_removed_edges = \
                 scale_cut.k_nearest_neighbour_scale_cut(x, y, scale_cut_length, k_neighbours)
         else:
             x, y, z, k_nearest_neighbour_graph, num_removed_edges = \
                 scale_cut.k_nearest_neighbour_scale_cut(x, y, scale_cut_length, k_neighbours, z=z)
     else:
         k_nearest_neighbour_graph = kneighbors_graph(vertices, n_neighbors=k_neighbours, mode='distance')
-    if is_tomo is True:
+    if is_tomo == True:
         k_nearest_neighbour_graph = tomo.convert_tomo_knn_length2angle(k_nearest_neighbour_graph, len(x))
     tree = minimum_spanning_tree(k_nearest_neighbour_graph, overwrite=True)
     tree = tree.tocoo()
     edge_length = tree.data
     index1 = tree.row
     index2 = tree.col
     x1 = x[index1]
     x2 = x[index2]
     edge_x = np.array([x1, x2])
     y1 = y[index1]
     y2 = y[index2]
     edge_y = np.array([y1, y2])
-    if two_dimensions is False:
+    if two_dimensions == False:
         z1 = z[index1]
         z2 = z[index2]
         edge_z = np.array([z1, z2])
     edge_index = np.array([index1, index2])
     if scale_cut_length == 0.:
-        if two_dimensions is True:
+        if two_dimensions == True:
             return edge_length, edge_x, edge_y, edge_index
         else:
             return edge_length, edge_x, edge_y, edge_z, edge_index
     else:
-        if two_dimensions is True:
+        if two_dimensions == True:
             return edge_length, edge_x, edge_y, edge_index, num_removed_edges
         else:
             return edge_length, edge_x, edge_y, edge_z, edge_index, num_removed_edges
```

### Comparing `mistree-1.2.1/mistree/mst/density.py` & `mistree-1.2.2/mistree/mst/density.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,24 +40,24 @@
     condition = np.where(xx < box_size)[0]
     xx = xx[condition]
     length = len(condition)
     if mode == '2D':
         x_div, y_div = np.meshgrid(xx, xx, indexing='ij')
         x_div, y_div = np.ndarray.flatten(x_div), np.ndarray.flatten(y_div)
         mean_param = utility_density.get_param_2d(x_param, y_param, param, dx, length, len(x_div), len(x_param))
-        if get_density is True:
+        if get_density == True:
             counts = utility_density.get_counts_2d(x, y, dx, length, len(x_div), len(x))
             density = counts / np.mean(counts)
             return mean_param, density
         else:
             return mean_param
     else:
         x_div, y_div, z_div = np.meshgrid(xx, xx, xx, indexing='ij')
         x_div, y_div, z_div = np.ndarray.flatten(x_div), np.ndarray.flatten(y_div), np.ndarray.flatten(z_div)
         mean_param = utility_density.get_param_3d(x_param, y_param, z_param, param, dx, length, len(x_div),
                                                   len(x_param))
-        if get_density is True:
+        if get_density == True:
             counts = utility_density.get_counts_3d(x, y, z, dx, length, len(x_div), len(x))
             density = counts / np.mean(counts)
             return mean_param, density
         else:
             return mean_param
```

### Comparing `mistree-1.2.1/mistree/mst/get_mst_class.py` & `mistree-1.2.2/mistree/mst/get_mst_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             else:
                 self._mode = 'spherical polar'
         elif self.ra is not None and self.dec is not None:
             if self.r is None:
                 self._mode = 'tomographic celestial'
             else:
                 self._mode = 'spherical polar celestial'
-        if do_print is True:
+        if do_print == True:
             print('MST mode: ', self._mode, ' coordinates')
         self.k_neighbours = 20
         self.edge_length = None
         self.edge_x = None
         self.edge_y = None
         self.edge_z = None
         self.edge_phi = None
@@ -190,35 +190,35 @@
         ----------
         box_size : float, optional
             The size of the '2D' or '3D' box.
         sub_divisions : int, optional
             The number of divisions used to divide the data set in each axis. Used for speeding up the branch
             finding algorithm when using many points (> 100000).
         """
-        if sub_divisions is 1:
+        if sub_divisions == 1:
             branch_index, rejected_branch_index = branches.get_branch_index(self.edge_index, self.edge_degree)
         else:
-            if self._mode is '2D':
+            if self._mode == '2D':
                 branch_index, rejected_branch_index = \
                     branches.get_branch_index_sub_divide(sub_divisions, self.edge_index, self.edge_degree,
                                                          box_size=box_size, edge_x=self.edge_x, edge_y=self.edge_y,
                                                          mode='Euclidean', two_dimension=True)
-            elif self._mode is '3D':
+            elif self._mode == '3D':
                 branch_index, rejected_branch_index = \
                     branches.get_branch_index_sub_divide(sub_divisions, self.edge_index, self.edge_degree,
                                                          box_size=box_size, edge_x=self.edge_x, edge_y=self.edge_y,
                                                          edge_z=self.edge_z, mode='Euclidean', two_dimension=False)
             else:
                 branch_index, rejected_branch_index = \
                     branches.get_branch_index_sub_divide(sub_divisions, self.edge_index, self.edge_degree,
                                                          box_size=None, phi=self.phi, theta=self.theta,
                                                          edge_phi=self.edge_phi, edge_theta=self.edge_theta, mode='spherical')
         self.branch_index = branch_index
-        if len(rejected_branch_index) is not 0:
-            if self.do_print is True:
+        if len(rejected_branch_index) != 0:
+            if self.do_print == True:
                 print(str(float(len(rejected_branch_index))) + ' branches were incompleted.')
         branch_length = [np.sum(self.edge_length[i]) for i in branch_index]
         self.branch_length = np.array(branch_length)
 
     def get_branch_edge_count(self):
         """Finds the number of edges included in each branch."""
         branch_edge_count = [float(len(i)) for i in self.branch_index]
@@ -308,15 +308,15 @@
             The shape of branches in the MST.
         edge_index : array, optional
             A 2 dimensional array, where the first nested array shows the indexes for the nodes
             on one end of the edge and the second shows the other node.
         branch_index : list, optional
             A list of branches, where each branch is given as a list of the indexes of the member edges.
         """
-        if include_index is True:
+        if include_index == True:
             return self.degree, self.edge_length, self.branch_length, self.branch_shape, self.edge_index, \
                    self.branch_index
         else:
             return self.degree, self.edge_length, self.branch_length, self.branch_shape
 
     def _get_stats(self, include_index=False, sub_divisions=1, k_neighbours=None, scale_cut_length=0.):
         """Computes the MST and outputs the statistics.
@@ -454,15 +454,15 @@
                     self.__init__(phi=all_phi[group_indices], theta=all_theta[group_indices], r=all_r[group_indices])
                 elif self._mode == 'tomographic celestial':
                     self.__init__(ra=all_ra[group_indices], dec=all_dec[group_indices])
                 elif self._mode == 'spherical polar celestial':
                     self.__init__(ra=all_ra[group_indices], dec=all_dec[group_indices], r=all_r[group_indices])
                 else:
                     pass
-                if include_index is False:
+                if include_index == False:
                     _degree, _edge_length , _branch_length, _branch_shape = \
                         self._get_stats(sub_divisions=sub_divisions, k_neighbours=k_neighbours, scale_cut_length=scale_cut_length)
                 else:
                     _degree, _edge_length , _branch_length, _branch_shape, _edge_index, _branch_index = \
                         self._get_stats(include_index=True, sub_divisions=sub_divisions, k_neighbours=k_neighbours, scale_cut_length=scale_cut_length)
                 if i == 0:
                     degree = _degree
@@ -470,18 +470,18 @@
                     branch_length = _branch_length
                     branch_shape = _branch_shape
                 else:
                     degree = np.concatenate([degree, _degree])
                     edge_length = np.concatenate([edge_length, _edge_length])
                     branch_length = np.concatenate([branch_length, _branch_length])
                     branch_shape = np.concatenate([branch_shape, _branch_shape])
-                if include_index is True:
+                if include_index == True:
                     edge_index.append(_edge_index)
                     branch_index.append(_branch_index)
-            if include_index is True:
+            if include_index == True:
                 return degree, edge_length, branch_length, branch_shape, edge_index, branch_index, groups
             else:
                 return degree, edge_length, branch_length, branch_shape
             if self._mode == '2D':
                 self.x = all_x
                 self.y = all_y
             elif self._mode == '3D':
```

### Comparing `mistree-1.2.1/mistree/mst/graph.py` & `mistree-1.2.2/mistree/mst/graph.py`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/mistree/mst/hist_mst.py` & `mistree-1.2.2/mistree/mst/hist_mst.py`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/mistree/mst/partition.py` & `mistree-1.2.2/mistree/mst/partition.py`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/mistree/mst/plot_mst.py` & `mistree-1.2.2/mistree/mst/plot_mst.py`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/mistree/mst/scale_cut.py` & `mistree-1.2.2/mistree/mst/scale_cut.py`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/mistree/mst/stats.py` & `mistree-1.2.2/mistree/mst/stats.py`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/mistree/mst/tomo.py` & `mistree-1.2.2/mistree/mst/tomo.py`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/mistree/mst/utility_density.f90` & `mistree-1.2.2/mistree/mst/utility_density.f90`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/mistree/mst/utility_mst.f90` & `mistree-1.2.2/mistree/mst/utility_mst.f90`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/mistree.egg-info/PKG-INFO` & `mistree-1.2.2/mistree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistree
-Version: 1.2.1
+Version: 1.2.2
 Summary: A python package for constructing and analysing the minimum spanning tree
 Home-page: https://knaidoo29.github.io/mistreedoc/
 Author: Krishna Naidoo
 Author-email: krishna.naidoo.11@ucl.ac.uk
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,28 +13,29 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Fortran
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MiSTree
 
 Author:         Krishna Naidoo                          
-Version:        1.2.0                               
+Version:        1.2.2                               
 Homepage:       https://github.com/knaidoo29/mistree    
 Documentation:  https://knaidoo29.github.io/mistreedoc/
 
 [![Build Status](https://travis-ci.org/knaidoo29/mistree.svg?branch=master)](https://travis-ci.org/knaidoo29/mistree) [![codecov](https://codecov.io/gh/knaidoo29/mistree/branch/master/graph/badge.svg)](https://codecov.io/gh/knaidoo29/mistree) [![PyPI version](https://badge.fury.io/py/mistree.svg)](https://badge.fury.io/py/mistree) [![status](https://joss.theoj.org/papers/461d79e9e5faf21029c0a7b1c928be28/status.svg)](https://joss.theoj.org/papers/461d79e9e5faf21029c0a7b1c928be28) [![DOI](https://zenodo.org/badge/170473458.svg)](https://zenodo.org/badge/latestdoi/170473458) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/knaidoo29/mistree/master?filepath=tutorials%2Fnotebooks%2F)
 [![ascl](https://img.shields.io/badge/ascl-1910.016-blue.svg?colorB=262255)](http://ascl.net/1910.016)
 
 ## Introduction
```

### Comparing `mistree-1.2.1/mistree.egg-info/SOURCES.txt` & `mistree-1.2.2/mistree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mistree-1.2.1/setup.py` & `mistree-1.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  sources = ['mistree/levy_flight/utility_random_walk.f90'])
 ext2 = Extension(name = 'mistree.mst.utility_density',
                  sources = ['mistree/mst/utility_density.f90'])
 ext3 = Extension(name = 'mistree.mst.utility_mst',
                  sources = ['mistree/mst/utility_mst.f90'])
 
 setup(name = 'mistree',
-      version = '1.2.1',
+      version = '1.2.2',
       description       = "A python package for constructing and analysing the minimum spanning tree",
       long_description  = long_description,
       long_description_content_type = 'text/markdown',
       url               = 'https://knaidoo29.github.io/mistreedoc/',
       author            = "Krishna Naidoo",
       author_email      = "krishna.naidoo.11@ucl.ac.uk",
       license='MIT',
@@ -44,14 +44,15 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Fortran',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Astronomy',
         'Topic :: Scientific/Engineering :: Physics',
         'Topic :: Scientific/Engineering :: Visualization',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Scientific/Engineering :: Mathematics',
       ],
```

