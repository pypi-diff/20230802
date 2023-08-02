# Comparing `tmp/bs_python_utils-0.4.1.tar.gz` & `tmp/bs_python_utils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_python_utils-0.4.1.tar", max compression
+gzip compressed data, was "bs_python_utils-0.4.2.tar", max compression
```

## Comparing `bs_python_utils-0.4.1.tar` & `bs_python_utils-0.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.4.1/LICENSE
--rw-r--r--   0        0        0     1864 2023-07-23 13:08:22.221938 bs_python_utils-0.4.1/README.md
--rw-r--r--   0        0        0     1799 2023-07-21 20:34:46.059698 bs_python_utils-0.4.1/bs_python_utils/Timer.py
--rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.4.1/bs_python_utils/__init__.py
--rw-r--r--   0        0        0     9089 2023-07-23 13:06:12.931194 bs_python_utils-0.4.1/bs_python_utils/bivariate_quantiles.py
--rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.859499 bs_python_utils-0.4.1/bs_python_utils/bs_altair.py
--rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.4.1/bs_python_utils/bs_logging.py
--rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.4.1/bs_python_utils/bs_mathstr.py
--rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.4.1/bs_python_utils/bs_mem.py
--rw-r--r--   0        0        0    15009 2023-07-21 21:46:32.207754 bs_python_utils-0.4.1/bs_python_utils/bs_opt.py
--rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.4.1/bs_python_utils/bs_plots.py
--rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.4.1/bs_python_utils/bs_seaborn.py
--rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.302214 bs_python_utils-0.4.1/bs_python_utils/bs_sparse_gaussian.py
--rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.4.1/bs_python_utils/bsmplutils.py
--rw-r--r--   0        0        0    33587 2023-07-22 22:16:47.975748 bs_python_utils-0.4.1/bs_python_utils/bsnputils.py
--rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.4.1/bs_python_utils/bssputils.py
--rw-r--r--   0        0        0    15438 2023-07-21 21:58:00.037774 bs_python_utils-0.4.1/bs_python_utils/bsstats.py
--rw-r--r--   0        0        0     9471 2023-05-08 18:43:13.753098 bs_python_utils-0.4.1/bs_python_utils/bsutils.py
--rw-r--r--   0        0        0    14016 2023-06-20 20:58:35.000000 bs_python_utils-0.4.1/bs_python_utils/chebyshev.py
--rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.4.1/bs_python_utils/distance_covariances.py
--rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.733299 bs_python_utils-0.4.1/bs_python_utils/example_opt.py
--rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.344134 bs_python_utils-0.4.1/bs_python_utils/examples_altair.py
--rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.733372 bs_python_utils-0.4.1/bs_python_utils/examples_distance_covariances.py
--rw-r--r--   0        0        0      552 2023-04-24 22:36:28.733335 bs_python_utils-0.4.1/bs_python_utils/examples_mem.py
--rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.4.1/bs_python_utils/examples_seaborn.py
--rw-r--r--   0        0        0      786 2023-04-24 22:36:28.733292 bs_python_utils-0.4.1/bs_python_utils/examples_sklearn.py
--rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.4.1/bs_python_utils/pandas_utils.py
--rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.4.1/bs_python_utils/sklearn_utils.py
--rw-r--r--   0        0        0     1890 2023-07-23 13:07:41.282800 bs_python_utils-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2876 1970-01-01 00:00:00.000000 bs_python_utils-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-25 18:18:48.273804 bs_python_utils-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1909 2023-08-02 17:45:46.755089 bs_python_utils-0.4.2/README.md
+-rw-r--r--   0        0        0     1799 2023-07-25 18:18:48.274334 bs_python_utils-0.4.2/bs_python_utils/Timer.py
+-rw-r--r--   0        0        0        0 2023-07-25 18:18:48.274376 bs_python_utils-0.4.2/bs_python_utils/__init__.py
+-rw-r--r--   0        0        0     9123 2023-08-02 17:29:19.470519 bs_python_utils-0.4.2/bs_python_utils/bivariate_quantiles.py
+-rw-r--r--   0        0        0    28473 2023-07-25 18:18:48.274727 bs_python_utils-0.4.2/bs_python_utils/bs_altair.py
+-rw-r--r--   0        0        0     2976 2023-07-25 18:18:48.274839 bs_python_utils-0.4.2/bs_python_utils/bs_logging.py
+-rw-r--r--   0        0        0     3577 2023-07-25 18:18:48.274920 bs_python_utils-0.4.2/bs_python_utils/bs_mathstr.py
+-rw-r--r--   0        0        0     4338 2023-07-25 18:18:48.275009 bs_python_utils-0.4.2/bs_python_utils/bs_mem.py
+-rw-r--r--   0        0        0    15009 2023-07-25 18:18:48.275181 bs_python_utils-0.4.2/bs_python_utils/bs_opt.py
+-rw-r--r--   0        0        0       36 2023-07-25 18:18:48.275258 bs_python_utils-0.4.2/bs_python_utils/bs_plots.py
+-rw-r--r--   0        0        0     4507 2023-07-25 18:18:48.275357 bs_python_utils-0.4.2/bs_python_utils/bs_seaborn.py
+-rw-r--r--   0        0        0     2201 2023-08-02 17:22:32.496441 bs_python_utils-0.4.2/bs_python_utils/bs_sparse_gaussian.py
+-rw-r--r--   0        0        0      905 2023-07-25 18:18:48.275517 bs_python_utils-0.4.2/bs_python_utils/bsmplutils.py
+-rw-r--r--   0        0        0    33587 2023-07-25 18:18:48.275734 bs_python_utils-0.4.2/bs_python_utils/bsnputils.py
+-rw-r--r--   0        0        0     2132 2023-07-25 18:18:48.275838 bs_python_utils-0.4.2/bs_python_utils/bssputils.py
+-rw-r--r--   0        0        0    14053 2023-08-02 17:44:39.345131 bs_python_utils-0.4.2/bs_python_utils/bsstats.py
+-rw-r--r--   0        0        0     9471 2023-07-25 18:18:48.276116 bs_python_utils-0.4.2/bs_python_utils/bsutils.py
+-rw-r--r--   0        0        0    14016 2023-07-25 18:18:48.276224 bs_python_utils-0.4.2/bs_python_utils/chebyshev.py
+-rw-r--r--   0        0        0     7801 2023-07-25 18:18:48.276337 bs_python_utils-0.4.2/bs_python_utils/distance_covariances.py
+-rw-r--r--   0        0        0     1350 2023-07-25 18:18:48.276417 bs_python_utils-0.4.2/bs_python_utils/example_opt.py
+-rw-r--r--   0        0        0     3833 2023-07-25 18:18:48.276493 bs_python_utils-0.4.2/bs_python_utils/examples_altair.py
+-rw-r--r--   0        0        0     1013 2023-07-25 18:18:48.276564 bs_python_utils-0.4.2/bs_python_utils/examples_distance_covariances.py
+-rw-r--r--   0        0        0      552 2023-07-25 18:18:48.276629 bs_python_utils-0.4.2/bs_python_utils/examples_mem.py
+-rw-r--r--   0        0        0      771 2023-07-25 18:18:48.276695 bs_python_utils-0.4.2/bs_python_utils/examples_seaborn.py
+-rw-r--r--   0        0        0      786 2023-07-25 18:18:48.276775 bs_python_utils-0.4.2/bs_python_utils/examples_sklearn.py
+-rw-r--r--   0        0        0     7426 2023-07-25 18:18:48.276867 bs_python_utils-0.4.2/bs_python_utils/pandas_utils.py
+-rw-r--r--   0        0        0     1872 2023-07-25 18:18:48.276931 bs_python_utils-0.4.2/bs_python_utils/sklearn_utils.py
+-rw-r--r--   0        0        0     1890 2023-08-02 17:23:55.728156 bs_python_utils-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 bs_python_utils-0.4.2/PKG-INFO
```

### Comparing `bs_python_utils-0.4.1/LICENSE` & `bs_python_utils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/README.md` & `bs_python_utils-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 My Python utilities.
 
 -   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 -   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
-
+#### 0.4.2 (August 2, 2023)
+Updated the docs.
 #### 0.4.1 (July 23, 2023)
 Only print if verbose in bivariate quantiles.
 #### 0.4 (July 22, 2023)
 Added bivariate quantiles and ranks à la optimal transportation.
 #### 0.3 (July 21, 2023)
 Added in Numpy utils a function to set upper and lower triangle to a scalar;
 and `minimize_free` in `bs_opt`.
```

### Comparing `bs_python_utils-0.4.1/bs_python_utils/Timer.py` & `bs_python_utils-0.4.2/bs_python_utils/Timer.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bivariate_quantiles.py` & `bs_python_utils-0.4.2/bs_python_utils/bivariate_quantiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
     vstar1[sort_order] = vstar1_sorted
 
     return vstar1
 
 
 def bivariate_quantiles(
     y: np.ndarray, u: np.ndarray, n_nodes: int = 32, verbose: bool = False
-):
+) -> np.ndarray:
     """computes the bivariate quantiles of `y` at the quantiles `u`
 
     Args:
         y: the observations, an `(n, 2)` matrix
         u: the quantiles at which to compute the bivariate quantiles,
             an `(m, 2)` matrix
         n_nodes: the number of nodes to use for the quadrature
@@ -267,15 +267,17 @@
     Returns:
         an `(m, 2)` matrix of bivariate quantiles
     """
     v = solve_for_v_(y, n_nodes, verbose)
     return bivariate_quantiles_v(y, u, v)
 
 
-def bivariate_ranks(y: np.ndarray, n_nodes: int = 32, verbose: bool = False):
+def bivariate_ranks(
+    y: np.ndarray, n_nodes: int = 32, verbose: bool = False
+) -> np.ndarray:
     """computes the bivariate ranks of `y`
 
     Args:
         y: the observations, an `(n, 2)` matrix
         n_nodes: the number of nodes to use for the quadrature
         verbose: if `True`, print some information
```

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bs_altair.py` & `bs_python_utils-0.4.2/bs_python_utils/bs_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bs_logging.py` & `bs_python_utils-0.4.2/bs_python_utils/bs_logging.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bs_mathstr.py` & `bs_python_utils-0.4.2/bs_python_utils/bs_mathstr.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bs_mem.py` & `bs_python_utils-0.4.2/bs_python_utils/bs_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bs_opt.py` & `bs_python_utils-0.4.2/bs_python_utils/bs_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bs_seaborn.py` & `bs_python_utils-0.4.2/bs_python_utils/bs_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bs_sparse_gaussian.py` & `bs_python_utils-0.4.2/bs_python_utils/bs_sparse_gaussian.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 """
-sets up sparse integration over a Gaussian
+Sets up sparse integration over a Gaussian, given text files that contain rescaled Gauss-Hermite nodes and weights.
+
+These files must be named `GHsparseGrid{ndims}prec{iprec}.txt`, where `ndims` is the number of dimensions of integration 
+and `iprec` is a precision level that must be 9, 13, or (most precise) 17. The file must have `(ndims+1) columns, 
+with the weights in the first column.
+
+The nodes and weights are rescaled so that `f(nodes) @ weights` approximates `Ef(X)` for `X` an `N(0,I)` variable.
 """
 from pathlib import Path
 
 import numpy as np
 
 from bs_python_utils.bsnputils import TwoArrays
 from bs_python_utils.bsutils import bs_error_abort
@@ -11,19 +17,20 @@
 
 def setup_sparse_gaussian(
     ndims: int, iprec: int, GHsparsedir: str | None = None
 ) -> TwoArrays:
     """
     get nodes and weights for sparse integration Ef(X) with X = N(0,1) in `ndims` dimensions
 
-    usage: nodes, weights = setup_sparse_gaussian(mdims, iprec); intf = f(nodes) @ weights
+    usage: nodes, weights = setup_sparse_gaussian(mdims, iprec); integral_f = f(nodes) @ weights
 
     Args:
         ndims: number of dimensions (1 to 5)
         iprec: precision (must be 9, 13, or 17)
+        GHsparsedir: the name of a directory that contains nodes and weights
 
     Returns:
         a pair of  arrays `nodes` and `weights`;
         `nodes` has `ndims`-1 columns and `weights` is a vector
     """
     GHdir = (
         Path.home() / "Dropbox" / "GHsparseGrids"
@@ -32,16 +39,24 @@
     )
     if iprec not in [9, 13, 17]:
         bs_error_abort(
             f"We only do sparse integration with precision 9, 13, or 17, not {iprec}"
         )
 
     if ndims in [1, 2, 3, 4, 5]:
+        if not GHdir.exists():
+            bs_error_abort("I did not find the directory with the nodes/weights files.")
         grid = np.loadtxt(GHdir / f"GHsparseGrid{ndims}prec{iprec}.txt")
-        weights = grid[:, 0]
-        nodes = grid[:, 1:]
+
+        print(f"{grid.shape=}")
+        if ndims == 1:
+            weights = grid[:, 0]
+            nodes = grid[:, 1]
+        else:
+            weights = grid[:, 0]
+            nodes = grid[:, 1:]
         return nodes, weights
     else:
         bs_error_abort(
             f"We only do sparse integration in one to five dimensions, not {ndims}"
         )
         return np.zeros(1), np.zeros(1)  # for mypy
```

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bsmplutils.py` & `bs_python_utils-0.4.2/bs_python_utils/bsmplutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bsnputils.py` & `bs_python_utils-0.4.2/bs_python_utils/bsnputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bssputils.py` & `bs_python_utils-0.4.2/bs_python_utils/bssputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bsstats.py` & `bs_python_utils-0.4.2/bs_python_utils/bsstats.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from statsmodels.nonparametric._kernel_base import EstimatorSettings
 from statsmodels.nonparametric.kernel_regression import KernelReg
 
 from bs_python_utils.bsnputils import (
     check_matrix,
     check_vector,
     check_vector_or_matrix,
-    make_lexico_grid,
 )
 from bs_python_utils.bssputils import spline_reg
 from bs_python_utils.bsutils import bs_error_abort
 
 
 @dataclass
 class TslsResults:
@@ -412,41 +411,7 @@
         else:  # multivariate
             means_x = np.mean(x_obs, 0)
             cov_mat = np.cov(x_obs.T)
             f_x = bs_multivariate_normal_pdf(x_points, means_x, cov_mat)
         if weights is not None:
             f_x *= weights / np.mean(weights)
     return cast(np.ndarray, f_x)
-
-
-def estimate_densities_at_quantiles(
-    X: np.ndarray, qtiles: np.ndarray
-) -> tuple[np.ndarray, np.ndarray] | tuple[np.ndarray, np.ndarray, np.ndarray]:
-    """estimate densities of margins at prespecified quantiles (Silverman rule)
-    and the joint density at each vector of these quantiles
-
-    Args:
-        X: `n`-vector or `(n, nx)`-matrix
-        qtiles: vector of `nq` numbers between 0 and 1
-
-    Returns: 
-        if `X` is a matrix, the `({nq}^{nx}, {nx})` matrices of estimated margin densities \
-     and the `{nq}^{nx}` vector of the joint density on the lexicographic grid of quantiles;
-        if `X` is a vector, the `nq`-vector of the density at the quantiles, twice
-    """
-    ndims_X = check_vector_or_matrix(X, "estimate_densities_")
-    if ndims_X == 1:
-        f_X = estimate_pdf(X, np.quantile(X, qtiles))
-        return f_X, f_X
-    else:
-        nx = X.shape[1]
-        nq = qtiles.size
-        f_X_k = np.zeros((nq, nx))
-        nodes_mat = np.zeros((nq, nx))
-        for i_x in range(nx):
-            X_ix = X[:, i_x]
-            nodes_mat[:, i_x] = np.quantile(X_ix, qtiles)
-            f_X_k[:, i_x] = estimate_pdf(X_ix, nodes_mat[:, i_x])
-        f_margins = make_lexico_grid(f_X_k)
-        values_X = make_lexico_grid(nodes_mat)
-        f_X = estimate_pdf(X, values_X)  # joint density
-        return f_margins, f_X, values_X
```

### Comparing `bs_python_utils-0.4.1/bs_python_utils/bsutils.py` & `bs_python_utils-0.4.2/bs_python_utils/bsutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/chebyshev.py` & `bs_python_utils-0.4.2/bs_python_utils/chebyshev.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/distance_covariances.py` & `bs_python_utils-0.4.2/bs_python_utils/distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/example_opt.py` & `bs_python_utils-0.4.2/bs_python_utils/example_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/examples_altair.py` & `bs_python_utils-0.4.2/bs_python_utils/examples_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/examples_distance_covariances.py` & `bs_python_utils-0.4.2/bs_python_utils/examples_distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/examples_mem.py` & `bs_python_utils-0.4.2/bs_python_utils/examples_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/examples_seaborn.py` & `bs_python_utils-0.4.2/bs_python_utils/examples_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/examples_sklearn.py` & `bs_python_utils-0.4.2/bs_python_utils/examples_sklearn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/pandas_utils.py` & `bs_python_utils-0.4.2/bs_python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/bs_python_utils/sklearn_utils.py` & `bs_python_utils-0.4.2/bs_python_utils/sklearn_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.1/pyproject.toml` & `bs_python_utils-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs_python_utils"
-version = "0.4.1"
+version = "0.4.2"
 description = "my Python utilities"
 authors = ["Bernard Salanie <bsalanie@columbia.edu>"]
 repository = "https://github.com/bsalanie/bs-python-utils"
 documentation = "https://bsalanie.github.io/bs-python-utils/"
 readme = "README.md"
 packages = [
   {include = "bs_python_utils"}
```

### Comparing `bs_python_utils-0.4.1/PKG-INFO` & `bs_python_utils-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-python-utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: my Python utilities
 Home-page: https://github.com/bsalanie/bs-python-utils
 Author: Bernard Salanie
 Author-email: bsalanie@columbia.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -33,15 +33,16 @@
 
 My Python utilities.
 
 -   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 -   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
-
+#### 0.4.2 (August 2, 2023)
+Updated the docs.
 #### 0.4.1 (July 23, 2023)
 Only print if verbose in bivariate quantiles.
 #### 0.4 (July 22, 2023)
 Added bivariate quantiles and ranks à la optimal transportation.
 #### 0.3 (July 21, 2023)
 Added in Numpy utils a function to set upper and lower triangle to a scalar;
 and `minimize_free` in `bs_opt`.
```

