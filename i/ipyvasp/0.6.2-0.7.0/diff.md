# Comparing `tmp/ipyvasp-0.6.2.tar.gz` & `tmp/ipyvasp-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyvasp-0.6.2.tar", last modified: Wed Jul 26 19:37:55 2023, max compression
+gzip compressed data, was "ipyvasp-0.7.0.tar", last modified: Wed Aug  2 18:34:56 2023, max compression
```

## Comparing `ipyvasp-0.6.2.tar` & `ipyvasp-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 19:37:55.096475 ipyvasp-0.6.2/
--rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.6.2/LICENSE
--rw-rw-rw-   0        0        0     1862 2023-07-26 19:37:55.095475 ipyvasp-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 19:37:55.066924 ipyvasp-0.6.2/ipyvasp/
--rw-rw-rw-   0        0        0     1838 2023-07-24 19:58:23.000000 ipyvasp-0.6.2/ipyvasp/__init__.py
--rw-rw-rw-   0        0        0      216 2023-07-04 22:54:12.000000 ipyvasp-0.6.2/ipyvasp/__main__.py
--rw-rw-rw-   0        0        0    37503 2023-07-02 21:24:03.000000 ipyvasp-0.6.2/ipyvasp/_enplots.py
--rw-rw-rw-   0        0        0    97706 2023-07-26 19:34:10.000000 ipyvasp-0.6.2/ipyvasp/_lattice.py
--rw-rw-rw-   0        0        0       23 2023-07-26 19:37:09.000000 ipyvasp-0.6.2/ipyvasp/_version.py
--rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.6.2/ipyvasp/bsdos.py
--rw-rw-rw-   0        0        0     3866 2023-07-26 16:58:27.000000 ipyvasp-0.6.2/ipyvasp/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:37:55.094497 ipyvasp-0.6.2/ipyvasp/core/
--rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.6.2/ipyvasp/core/__init__.py
--rw-rw-rw-   0        0        0    37726 2023-07-02 17:25:50.000000 ipyvasp-0.6.2/ipyvasp/core/parser.py
--rw-rw-rw-   0        0        0    34192 2023-07-24 20:25:24.000000 ipyvasp-0.6.2/ipyvasp/core/plot_toolkit.py
--rw-rw-rw-   0        0        0    30507 2023-07-24 19:55:30.000000 ipyvasp-0.6.2/ipyvasp/core/serializer.py
--rw-rw-rw-   0        0        0    14743 2023-07-04 17:24:40.000000 ipyvasp-0.6.2/ipyvasp/core/spatial_toolkit.py
--rw-rw-rw-   0        0        0    19335 2023-07-02 18:12:36.000000 ipyvasp-0.6.2/ipyvasp/evals_dataframe.py
--rw-rw-rw-   0        0        0    23229 2023-07-26 18:04:39.000000 ipyvasp-0.6.2/ipyvasp/lattice.py
--rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.6.2/ipyvasp/misc.py
--rw-rw-rw-   0        0        0    11406 2023-07-02 18:28:53.000000 ipyvasp-0.6.2/ipyvasp/potential.py
--rw-rw-rw-   0        0        0    15225 2023-07-10 18:26:17.000000 ipyvasp-0.6.2/ipyvasp/utils.py
--rw-rw-rw-   0        0        0    44823 2023-07-01 01:09:38.000000 ipyvasp-0.6.2/ipyvasp/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:37:55.089394 ipyvasp-0.6.2/ipyvasp.egg-info/
--rw-rw-rw-   0        0        0     1862 2023-07-26 19:37:54.000000 ipyvasp-0.6.2/ipyvasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      601 2023-07-26 19:37:54.000000 ipyvasp-0.6.2/ipyvasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 19:37:54.000000 ipyvasp-0.6.2/ipyvasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-26 19:37:54.000000 ipyvasp-0.6.2/ipyvasp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      203 2023-07-26 19:37:54.000000 ipyvasp-0.6.2/ipyvasp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 19:37:54.000000 ipyvasp-0.6.2/ipyvasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 19:37:55.096475 ipyvasp-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     3840 2023-07-04 22:57:57.000000 ipyvasp-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 18:34:56.814476 ipyvasp-0.7.0/
+-rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     1862 2023-08-02 18:34:56.814476 ipyvasp-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 18:34:56.760526 ipyvasp-0.7.0/ipyvasp/
+-rw-rw-rw-   0        0        0     1838 2023-07-24 19:58:23.000000 ipyvasp-0.7.0/ipyvasp/__init__.py
+-rw-rw-rw-   0        0        0      216 2023-07-04 22:54:12.000000 ipyvasp-0.7.0/ipyvasp/__main__.py
+-rw-rw-rw-   0        0        0    37503 2023-07-02 21:24:03.000000 ipyvasp-0.7.0/ipyvasp/_enplots.py
+-rw-rw-rw-   0        0        0    99401 2023-08-02 17:22:12.000000 ipyvasp-0.7.0/ipyvasp/_lattice.py
+-rw-rw-rw-   0        0        0       23 2023-08-02 18:33:50.000000 ipyvasp-0.7.0/ipyvasp/_version.py
+-rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.7.0/ipyvasp/bsdos.py
+-rw-rw-rw-   0        0        0     3866 2023-07-26 16:58:27.000000 ipyvasp-0.7.0/ipyvasp/cli.py
+drwxrwxrwx   0        0        0        0 2023-08-02 18:34:56.812882 ipyvasp-0.7.0/ipyvasp/core/
+-rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.7.0/ipyvasp/core/__init__.py
+-rw-rw-rw-   0        0        0    37726 2023-07-02 17:25:50.000000 ipyvasp-0.7.0/ipyvasp/core/parser.py
+-rw-rw-rw-   0        0        0    34226 2023-08-02 18:12:09.000000 ipyvasp-0.7.0/ipyvasp/core/plot_toolkit.py
+-rw-rw-rw-   0        0        0    31902 2023-08-02 15:44:21.000000 ipyvasp-0.7.0/ipyvasp/core/serializer.py
+-rw-rw-rw-   0        0        0    14744 2023-07-27 15:28:24.000000 ipyvasp-0.7.0/ipyvasp/core/spatial_toolkit.py
+-rw-rw-rw-   0        0        0    19335 2023-07-02 18:12:36.000000 ipyvasp-0.7.0/ipyvasp/evals_dataframe.py
+-rw-rw-rw-   0        0        0    23959 2023-08-02 18:08:13.000000 ipyvasp-0.7.0/ipyvasp/lattice.py
+-rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.7.0/ipyvasp/misc.py
+-rw-rw-rw-   0        0        0    11406 2023-07-02 18:28:53.000000 ipyvasp-0.7.0/ipyvasp/potential.py
+-rw-rw-rw-   0        0        0    15225 2023-07-10 18:26:17.000000 ipyvasp-0.7.0/ipyvasp/utils.py
+-rw-rw-rw-   0        0        0    44823 2023-07-01 01:09:38.000000 ipyvasp-0.7.0/ipyvasp/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-02 18:34:56.801177 ipyvasp-0.7.0/ipyvasp.egg-info/
+-rw-rw-rw-   0        0        0     1862 2023-08-02 18:34:56.000000 ipyvasp-0.7.0/ipyvasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2023-08-02 18:34:56.000000 ipyvasp-0.7.0/ipyvasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 18:34:56.000000 ipyvasp-0.7.0/ipyvasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-08-02 18:34:56.000000 ipyvasp-0.7.0/ipyvasp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      203 2023-08-02 18:34:56.000000 ipyvasp-0.7.0/ipyvasp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 18:34:56.000000 ipyvasp-0.7.0/ipyvasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 18:34:56.814476 ipyvasp-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     3840 2023-07-04 22:57:57.000000 ipyvasp-0.7.0/setup.py
```

### Comparing `ipyvasp-0.6.2/LICENSE` & `ipyvasp-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/PKG-INFO` & `ipyvasp-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvasp
-Version: 0.6.2
+Version: 0.7.0
 Summary: A processing tool for VASP DFT input/output processing in Jupyter Notebook.
 Home-page: https://github.com/massgh/ipyvasp
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyvasp/issues
 Keywords: Jupyter,Widgets,IPython,VASP,DFT
```

### Comparing `ipyvasp-0.6.2/README.md` & `ipyvasp-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/ipyvasp/__init__.py` & `ipyvasp-0.7.0/ipyvasp/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/ipyvasp/_enplots.py` & `ipyvasp-0.7.0/ipyvasp/_enplots.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/ipyvasp/_lattice.py` & `ipyvasp-0.7.0/ipyvasp/_lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1417,14 +1417,17 @@
 # Cell
 def _fix_sites(poscar_data, tol=1e-2, eqv_sites=False, translate=None):
     """Add equivalent sites to make a full data shape of lattice. Returns same data after fixing.
     It should not be exposed mostly be used in visualizations"""
     pos = (
         poscar_data.positions.copy()
     )  # We can also do poscar_data.copy().positions that copies all contents.
+    if hasattr(poscar_data.metadata, "origin"):
+        pos = pos + poscar_data.metadata.origin  # Move towards origin of basis
+
     labels = np.array(poscar_data.labels)  # We need to store equivalent labels as well
     out_dict = poscar_data.to_dict()  # For output
 
     if translate and isinstance(translate, (int, np.integer, float)):
         pos = pos + (translate - int(translate))  # Only translate in 0 - 1
     elif translate and len(translate) == 3:
         txyz = np.array([translate])
@@ -1483,14 +1486,17 @@
                 "lab": np.hstack([vlabs, *slab]),
                 "inds": np.hstack([inds, *sinds]),
             }
             new_dict[k]["range"] = range(start, start + len(new_dict[k]["pos"]))
             start += len(new_dict[k]["pos"])
 
         out_dict["positions"] = np.vstack([new_dict[k]["pos"] for k in new_dict.keys()])
+        if hasattr(poscar_data.metadata, "origin"):
+            out_dict["positions"] -= poscar_data.metadata.origin  # origin given by user
+
         out_dict["metadata"]["eqv_labels"] = np.hstack(
             [new_dict[k]["lab"] for k in new_dict.keys()]
         )
 
         out_dict["metadata"]["eqv_indices"] = np.hstack(
             [new_dict[k]["inds"] for k in new_dict.keys()]
         )
@@ -1870,18 +1876,22 @@
         )
 
     if (colors is None) or len(colors) != len(uelems.keys()):
         colors = [_atom_colors[elem] for elem in uelems.keys()]
 
     # Before doing other stuff, create something for legend.
     for (k, v), c, s in zip(uelems.items(), colors, sizes):
-        ax.scatter([], [], s=s, color=c, label=k)  # Works both for 3D and 2D.
+        ax.scatter(
+            [], [], s=s, color=c, label=k, **site_kws
+        )  # Works both for 3D and 2D.
 
     # Now change colors and sizes to whole array size
-    colors = np.array([colors[i] for i, vs in enumerate(uelems.values()) for v in vs])
+    colors = np.array(
+        [mplc.to_rgb(colors[i]) for i, vs in enumerate(uelems.values()) for v in vs]
+    )
     sizes = np.array([sizes[i] for i, vs in enumerate(uelems.values()) for v in vs])
 
     if sites:
         colors = colors[sites]
         sizes = sizes[sites]
 
     if np.any(pairs):
@@ -1921,16 +1931,17 @@
         )
         if fmt_label:
             for i, coord in enumerate(coords):
                 lab, textkws = fmt_label(labels[i]), {}
                 if isinstance(lab, (list, tuple)):
                     lab, textkws = lab
                 ax.text(*coord, lab, **textkws)
-        # Set aspect to same as data.
-        ax.set_box_aspect(np.ptp(bz_data.vertices, axis=0))
+        # Set aspect to same as data if cell plotted
+        if plot_cell:
+            ax.set_box_aspect(np.ptp(bz_data.vertices, axis=0))
 
     elif plane in "xyzxzyx":
         site_kws = {**dict(alpha=0.7, zorder=3), **site_kws}
         (iz,) = [i for i in range(3) if i not in (ix, iy)]
         zorder = coords[:, iz].argsort()
         if plane in "yxzy":  # Left handed
             zorder = zorder[::-1]
@@ -2082,21 +2093,23 @@
     ----------
     scale : tuple
         Tuple of three values along (a,b,c) vectors. int or float values. If number of sites are not as expected in output,
         tweak `tol` instead of `scale`. You can put a minus sign with `tol` to get more sites and plus sign to reduce sites.
     tol : float
         It is used such that site positions are blow `1 - tol`, as 1 belongs to next cell, not previous one.
 
-
     .. note::
         ``scale = (2,2,2)`` enlarges a cell and next operation of ``(1/2,1/2,1/2)`` should bring original cell back.
 
     .. warning::
-        A POSCAR scaled with Non-integer values should only be used for visualization purposes, Not for any other opration such as making supercells, joining POSCARs.
+        A POSCAR scaled with Non-integer values should only be used for visualization purposes, Not for any other opration such as making supercells, joining POSCARs etc.
     """
+    if not isinstance(scale, (tuple, list)) or len(scale) != 3:
+        raise ValueError("scale must be a tuple of three values.")
+
     ii, jj, kk = np.ceil(scale).astype(int)  # Need int for joining.
 
     if tuple(scale) == (1, 1, 1):  # No need to scale.
         return poscar_data
 
     if ii >= 2:
         poscar_data = repeat_poscar(poscar_data, ii, direction="a")
@@ -2114,14 +2127,15 @@
 
     # Get clip fraction
     fi, fj, fk = scale[0] / ii, scale[1] / jj, scale[2] / kk
 
     # Clip at end according to scale, change length of basis as fractions.
     pos = poscar_data.positions.copy() / np.array([fi, fj, fk])  # rescale for clip
     basis = poscar_data.basis.copy()
+
     for i, f in zip(range(3), [fi, fj, fk]):
         basis[i] = f * basis[i]  # Basis rescale for clip
 
     new_poscar["basis"] = basis
     new_poscar["metadata"]["scale"] = np.linalg.norm(basis[0])
     new_poscar["metadata"]["comment"] = f"Modified by ipyvasp"
 
@@ -2161,14 +2175,36 @@
     p_dict["basis"] = rot.apply(
         p_dict["basis"]
     )  # Rotate basis so that they are transpose
     p_dict["metadata"]["comment"] = f"Modified by ipyvasp"
     return serializer.PoscarData(p_dict)
 
 
+def set_origin(poscar_data, origin):
+    """Set origin of POSCAR sites to a given position in fractional coordinates.
+    The following example demonstrates the use of this function.
+
+    >>> import ipyvasp as ipv
+    >>> poscar = ipv.POSCAR("POSCAR")
+    >>> ax = poscar.splot_cell() # plot original cell
+    >>> poscar_shifted = poscar.scale((3,3,3)).set_origin((1/3,1/3,1/3))
+    >>> poscar_shifted.splot_lattice(ax=ax, plot_cell=False) # displays sites around original cell
+
+    .. warning::
+        The shifted origin will be used in all subsequent operations such as joining, rotating, writing etc.
+        You must know what you are doing after setting origin. It is recommended to use this function only for visualization purposes.
+    """
+    if not isinstance(origin, (tuple, list, np.ndarray)) or len(origin) != 3:
+        raise ValueError("origin must be a list, tuple or numpy array of length 3.")
+    new_poscar = poscar_data.to_dict()
+    new_poscar["positions"] = poscar_data.positions - np.array(origin)
+    new_poscar["metadata"]["origin"] = origin  # need this info in fixing sites
+    return serializer.PoscarData(new_poscar)
+
+
 def set_zdir(poscar_data, hkl, phi=0):
     """Set z-direction of POSCAR along a given hkl direction and returns new data.
 
     Parameters
     ----------
     hkl : tuple
         (h,k,l) of the direction along which z-direction is to be set.
@@ -2577,7 +2613,8 @@
     "View a POSCAR in a jupyter notebook. kwargs are passed to splot_lattice. After setting a view, you can do view.f(**view.kwargs) to get same plot in a cell."
 
     def view(elev=30, azim=30, roll=0):
         ax = splot_lattice(poscar_data, **kwargs)
         ax.view_init(elev=elev, azim=azim, roll=roll)
 
     return interactive(view, elev=(0, 180), azim=(0, 360), roll=(0, 360))
+
```

### Comparing `ipyvasp-0.6.2/ipyvasp/bsdos.py` & `ipyvasp-0.7.0/ipyvasp/bsdos.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/ipyvasp/cli.py` & `ipyvasp-0.7.0/ipyvasp/cli.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/ipyvasp/core/parser.py` & `ipyvasp-0.7.0/ipyvasp/core/parser.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/ipyvasp/core/plot_toolkit.py` & `ipyvasp-0.7.0/ipyvasp/core/plot_toolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1015,12 +1015,12 @@
 
     fig_widget.data = []  # Clear previous data
     if template is not None:
         fig.layout.template = template  # will make white flash if not done before
 
     fig_widget.layout = fig.layout
 
-    with fig_widget.batch_animate():
+    with fig_widget.batch_animate(0):  # Disable animation to speed up
         for data in fig.data:
             fig_widget.add_trace(data)
 
     return fig_widget
```

### Comparing `ipyvasp-0.6.2/ipyvasp/core/serializer.py` & `ipyvasp-0.7.0/ipyvasp/core/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,20 @@
     "CellData",
 ]
 
 import json, re
 import pickle
 import inspect
 from collections import namedtuple
+from itertools import product
 from copy import deepcopy
 from pathlib import Path
 
 import numpy as np
+from scipy.spatial import KDTree
 
 from .spatial_toolkit import (
     angle_deg,
     to_basis,
     to_R3,
     kpoints2bz,
     order,
@@ -308,14 +310,42 @@
             self.metadata, "eqv_labels"
         ):  # If eqv_labels are present, return them
             return self.metadata.eqv_labels
         return np.array(
             [f"{k} {v - vs.start + 1}" for k, vs in self.types.items() for v in vs]
         )
 
+    def get_neighbors(self, k=5):
+        """Get the k nearest neighbors of each atom (including itself) in the lattice.
+        Returns array (N, k) of indices of atoms. The first index is the atom itself.
+
+
+        >>> import ipyvasp as ipv
+        >>> data = ipv.POSCAR('POSCAR').data # Assume 8 atoms
+        >>> knn = data.get_neighbors(5) # or .get_knn, Array of shape (8, 5) with indices of neighbors
+        >>> data.labels[knn] # Array of shape (8, 5) with labels of neighbors
+        >>> data.positions[knn] # Array of shape (8, 5, 3) with positions of neighbors
+        >>> data.labels[knn[0]] # Array of shape (5,) with labels of neighbors of first atom including itself
+        """
+        if not isinstance(k, int):
+            raise ValueError("k must be an integer to include that many neighbors")
+
+        # To take care of periodic boundary conditions, we need to replicate the atoms in the lattice
+        ps = np.vstack(
+            [self.positions + tr for tr in product([0, 1, -1], [0, 1, -1], [0, 1, -1])]
+        )
+        cs = to_R3(self.basis, ps)
+        tree = KDTree(cs)
+        _, inn = tree.query(cs, k=k)
+        return inn % len(
+            self.positions
+        )  # to get the index of the atom in the original list
+
+    get_knn = get_neighbors  # important alias
+
     def get_distance(self, atom1, atom2):
         """
         Returns the distance between two atoms.
         Provide atom1 and atom2 as strings such as get_distance('Ga', 'As') to get a mimimal distance between two types
         or as a dict with a single key as get_distance({'Ga':0}, {'As':0}) to get distance between specific atoms,
         or mixed as get_distance('Ga', {'As':0}) to get minimum distance between a type and a specific atom.
         """
```

### Comparing `ipyvasp-0.6.2/ipyvasp/core/spatial_toolkit.py` & `ipyvasp-0.7.0/ipyvasp/core/spatial_toolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
 def kpoints2bz(bz_data, kpoints, shift=0, keep_geomerty=False):
     """Brings KPOINTS inside BZ. Applies `to_R3` only if BZ is primitive.
 
     Parameters
     ----------
     bz_data : Output of get_bz().
     kpoints : array_like
-        List or array of KPOINTS to transorm into BZ or R3.
+        List or array of KPOINTS to transform into BZ or R3.
     shift : float
         This value is added to kpoints before any other operation, single number of list of 3 numbers for each direction.
     keep_geomerty : bool
         If True, returns kpoints in R3 with `shift` applied, keeping the neighbors in order, else kpoints adopt the shape of BZ.
         This is useful when you already created cartesian kpoints mesh and want to collect their fractional coordinates back to cartesian.
     """
     kpoints = np.array(kpoints) + shift
```

### Comparing `ipyvasp-0.6.2/ipyvasp/evals_dataframe.py` & `ipyvasp-0.7.0/ipyvasp/evals_dataframe.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/ipyvasp/lattice.py` & `ipyvasp-0.7.0/ipyvasp/lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import numpy as np
 from pandas.io.clipboard import clipboard_get, clipboard_set
 import matplotlib.colors as mcolors
 
 
 from .core import serializer
 from .core import spatial_toolkit as stk
+from .core.plot_toolkit import iplot2widget
 from .utils import _sig_kwargs, _sub_doc
 from . import _lattice as plat
 from ._lattice import (
     periodic_table,
     get_kpath,
     get_kmesh,
     splot_bz,
@@ -191,14 +192,15 @@
         view.gui_style = "NGL"
     return view
 
 
 class POSCAR:
     _cb_instance = {}  # Loads last clipboard data if not changed
     _mp_instance = {}  # Loads last mp data if not changed
+    _update_kws = {}  # kwargs to pass to auto update figurewidget
 
     def __init__(self, path=None, content=None, data=None):
         """
         POSCAR class to contain data and related methods, data is PoscarData, json/tuple file/string.
         Do not use `data` yourself, it's for operations on poscar.
 
         Parameters
@@ -284,14 +286,23 @@
 
     def view_kpath(self):
         "Initialize a KpathWidget instance to view kpath for current POSCAR, and you can select others too."
         from .widgets import KpathWidget
 
         return KpathWidget(path=str(self.path.parent), glob=self.path.name)
 
+    @_sig_kwargs(plat.iplot_lattice, ("poscar_data",))
+    def view_widegt(self, **kwargs):
+        self.__class__._update_kws = kwargs  # attach to class, not self
+        return iplot2widget(self.iplot_lattice(**kwargs))
+
+    def update_widget(self, handle):
+        "Update widget (if shown in notebook) after some operation on POSCAR with `handle` returned by `view_widget`"
+        iplot2widget(self.iplot_lattice(**self._update_kws), fig_widget=handle)
+
     @classmethod
     def from_file(cls, path):
         "Load data from POSCAR file"
         return cls(path=path)
 
     @classmethod
     def from_string(cls, content):
@@ -525,14 +536,18 @@
         )
 
     @_sub_doc(plat.scale_poscar)
     @_sig_kwargs(plat.scale_poscar, ("poscar_data",))
     def scale(self, scale=(1, 1, 1), **kwargs):
         return self.__class__(data=plat.scale_poscar(self.data, scale, **kwargs))
 
+    @_sub_doc(plat.set_origin)
+    def set_origin(self, origin):
+        return self.__class__(data=plat.set_origin(self.data, origin=origin))
+
     @_sub_doc(plat.rotate_poscar)
     def rotate(self, angle_deg, axis_vec):
         return self.__class__(
             data=plat.rotate_poscar(self.data, angle_deg=angle_deg, axis_vec=axis_vec)
         )
 
     @_sub_doc(plat.set_zdir)
```

### Comparing `ipyvasp-0.6.2/ipyvasp/misc.py` & `ipyvasp-0.7.0/ipyvasp/misc.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/ipyvasp/potential.py` & `ipyvasp-0.7.0/ipyvasp/potential.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/ipyvasp/utils.py` & `ipyvasp-0.7.0/ipyvasp/utils.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/ipyvasp/widgets.py` & `ipyvasp-0.7.0/ipyvasp/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/ipyvasp.egg-info/PKG-INFO` & `ipyvasp-0.7.0/ipyvasp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvasp
-Version: 0.6.2
+Version: 0.7.0
 Summary: A processing tool for VASP DFT input/output processing in Jupyter Notebook.
 Home-page: https://github.com/massgh/ipyvasp
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyvasp/issues
 Keywords: Jupyter,Widgets,IPython,VASP,DFT
```

### Comparing `ipyvasp-0.6.2/ipyvasp.egg-info/SOURCES.txt` & `ipyvasp-0.7.0/ipyvasp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.2/setup.py` & `ipyvasp-0.7.0/setup.py`

 * *Files identical despite different names*

