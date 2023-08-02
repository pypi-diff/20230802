# Comparing `tmp/arfs-2.0.3.tar.gz` & `tmp/arfs-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-2.0.3.tar", last modified: Mon Jul 31 14:01:48 2023, max compression
+gzip compressed data, was "arfs-2.0.4.tar", last modified: Wed Aug  2 19:55:11 2023, max compression
```

## Comparing `arfs-2.0.3.tar` & `arfs-2.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 14:01:48.184867 arfs-2.0.3/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-2.0.3/LICENSE.md
--rw-rw-rw-   0        0        0    11944 2023-07-31 14:01:48.185867 arfs-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    11254 2023-07-31 13:58:34.000000 arfs-2.0.3/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1611 2023-07-31 14:01:48.195866 arfs-2.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-31 14:01:47.613867 arfs-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 14:01:47.872867 arfs-2.0.3/src/arfs/
--rw-rw-rw-   0        0        0       92 2023-07-31 13:56:58.000000 arfs-2.0.3/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    87125 2023-07-31 13:46:30.000000 arfs-2.0.3/src/arfs/association.py
--rw-rw-rw-   0        0        0     6829 2023-07-31 13:45:23.000000 arfs-2.0.3/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:01:47.624868 arfs-2.0.3/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2023-07-31 14:01:48.011866 arfs-2.0.3/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-2.0.3/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-2.0.3/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2023-07-31 14:01:48.146866 arfs-2.0.3/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      637 2023-01-06 14:55:48.000000 arfs-2.0.3/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    96187 2023-07-29 17:00:56.000000 arfs-2.0.3/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5398 2023-07-31 13:36:41.000000 arfs-2.0.3/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    22592 2023-07-31 13:36:55.000000 arfs-2.0.3/src/arfs/feature_selection/lasso.py
--rw-rw-rw-   0        0        0    13812 2023-07-31 13:37:06.000000 arfs-2.0.3/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2473 2023-07-31 13:38:21.000000 arfs-2.0.3/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    16052 2023-07-31 13:40:30.000000 arfs-2.0.3/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    15889 2023-07-31 13:42:08.000000 arfs-2.0.3/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    21997 2023-07-31 13:49:08.000000 arfs-2.0.3/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     5788 2023-07-31 13:49:56.000000 arfs-2.0.3/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    38641 2023-07-31 13:53:12.000000 arfs-2.0.3/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15511 2023-07-31 13:53:23.000000 arfs-2.0.3/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    25361 2023-07-31 13:53:40.000000 arfs-2.0.3/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:01:47.987883 arfs-2.0.3/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    11944 2023-07-31 14:01:47.000000 arfs-2.0.3/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2023-07-31 14:01:47.000000 arfs-2.0.3/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 14:01:47.000000 arfs-2.0.3/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-2.0.3/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      573 2023-07-31 14:01:47.000000 arfs-2.0.3/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-31 14:01:47.000000 arfs-2.0.3/src/arfs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 14:01:48.173865 arfs-2.0.3/tests/
--rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-2.0.3/tests/test_allrelevant.py
--rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-2.0.3/tests/test_featselect.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.885490 arfs-2.0.4/
+-rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-2.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0    11944 2023-08-02 19:55:11.892488 arfs-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11254 2023-07-31 13:58:34.000000 arfs-2.0.4/README.md
+-rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-2.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1386 2023-08-02 19:55:11.924489 arfs-2.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.190488 arfs-2.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.402520 arfs-2.0.4/src/arfs/
+-rw-rw-rw-   0        0        0       92 2023-08-02 12:18:39.000000 arfs-2.0.4/src/arfs/__init__.py
+-rw-rw-rw-   0        0        0    87156 2023-08-02 12:10:26.000000 arfs-2.0.4/src/arfs/association.py
+-rw-rw-rw-   0        0        0     6829 2023-07-31 13:45:23.000000 arfs-2.0.4/src/arfs/benchmark.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.193487 arfs-2.0.4/src/arfs/dataset/
+drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.587488 arfs-2.0.4/src/arfs/dataset/data/
+-rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-2.0.4/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-2.0.4/src/arfs/dataset/data/housing.zip
+drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.769494 arfs-2.0.4/src/arfs/feature_selection/
+-rw-rw-rw-   0        0        0      711 2023-08-02 12:10:25.000000 arfs-2.0.4/src/arfs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0    96674 2023-08-02 12:14:27.000000 arfs-2.0.4/src/arfs/feature_selection/allrelevant.py
+-rw-rw-rw-   0        0        0     5398 2023-07-31 13:36:41.000000 arfs-2.0.4/src/arfs/feature_selection/base.py
+-rw-rw-rw-   0        0        0    22557 2023-08-02 12:10:25.000000 arfs-2.0.4/src/arfs/feature_selection/lasso.py
+-rw-rw-rw-   0        0        0    13812 2023-07-31 13:37:06.000000 arfs-2.0.4/src/arfs/feature_selection/mrmr.py
+-rw-rw-rw-   0        0        0     2473 2023-07-31 13:38:21.000000 arfs-2.0.4/src/arfs/feature_selection/summary.py
+-rw-rw-rw-   0        0        0    16052 2023-07-31 13:40:30.000000 arfs-2.0.4/src/arfs/feature_selection/unsupervised.py
+-rw-rw-rw-   0        0        0    15889 2023-07-31 13:42:08.000000 arfs-2.0.4/src/arfs/feature_selection/variable_importance.py
+-rw-rw-rw-   0        0        0    21997 2023-07-31 13:49:08.000000 arfs-2.0.4/src/arfs/gbm.py
+-rw-rw-rw-   0        0        0     5788 2023-08-02 08:27:06.000000 arfs-2.0.4/src/arfs/parallel.py
+-rw-rw-rw-   0        0        0    38523 2023-08-02 12:10:25.000000 arfs-2.0.4/src/arfs/preprocessing.py
+-rw-rw-rw-   0        0        0    15511 2023-07-31 13:53:23.000000 arfs-2.0.4/src/arfs/sampling.py
+-rw-rw-rw-   0        0        0    25361 2023-07-31 13:53:40.000000 arfs-2.0.4/src/arfs/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.554489 arfs-2.0.4/src/arfs.egg-info/
+-rw-rw-rw-   0        0        0    11944 2023-08-02 19:55:11.000000 arfs-2.0.4/src/arfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-08-02 19:55:11.000000 arfs-2.0.4/src/arfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 19:55:11.000000 arfs-2.0.4/src/arfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-2.0.4/src/arfs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      362 2023-08-02 19:55:11.000000 arfs-2.0.4/src/arfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-02 19:55:11.000000 arfs-2.0.4/src/arfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.805487 arfs-2.0.4/tests/
+-rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-2.0.4/tests/test_allrelevant.py
+-rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-2.0.4/tests/test_featselect.py
```

### Comparing `arfs-2.0.3/LICENSE.md` & `arfs-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/PKG-INFO` & `arfs-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 2.0.3
+Version: 2.0.4
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-2.0.3/README.md` & `arfs-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/setup.cfg` & `arfs-2.0.4/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -66,36 +66,22 @@
 00000410: 6673 2e64 6174 6173 6574 2e64 6573 6372  fs.dataset.descr
 00000420: 6970 7469 6f6e 203d 200d 0a09 2a2e 7273  iption = ...*.rs
 00000430: 740d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  t....[options.ex
 00000440: 7472 6173 5f72 6571 7569 7265 5d0d 0a64  tras_require]..d
 00000450: 6f63 7320 3d20 0d0a 0969 7079 6b65 726e  ocs = ...ipykern
 00000460: 656c 0d0a 0969 7079 7468 6f6e 5f67 656e  el...ipython_gen
 00000470: 7574 696c 730d 0a09 7061 6e64 6f63 0d0a  utils...pandoc..
-00000480: 0973 7068 696e 783d 3d37 2e31 2e31 0d0a  .sphinx==7.1.1..
-00000490: 096e 6273 7068 696e 783d 3d30 2e39 2e32  .nbsphinx==0.9.2
-000004a0: 0d0a 0973 7068 696e 782d 6175 746f 646f  ...sphinx-autodo
-000004b0: 632d 7479 7065 6869 6e74 733d 3d31 2e32  c-typehints==1.2
-000004c0: 342e 300d 0a09 7370 6869 6e78 2d63 6f70  4.0...sphinx-cop
-000004d0: 7962 7574 746f 6e3d 3d30 2e35 2e32 0d0a  ybutton==0.5.2..
-000004e0: 0973 7068 696e 782d 7461 6273 3d3d 332e  .sphinx-tabs==3.
-000004f0: 342e 310d 0a09 7370 6869 6e78 6177 6573  4.1...sphinxawes
-00000500: 6f6d 652d 7468 656d 653d 3d34 2e31 2e30  ome-theme==4.1.0
-00000510: 0d0a 0973 7068 696e 7863 6f6e 7472 6962  ...sphinxcontrib
-00000520: 2d61 7070 6c65 6865 6c70 3d3d 312e 302e  -applehelp==1.0.
-00000530: 340d 0a09 7370 6869 6e78 636f 6e74 7269  4...sphinxcontri
-00000540: 622d 6465 7668 656c 703d 3d31 2e30 2e32  b-devhelp==1.0.2
-00000550: 0d0a 0973 7068 696e 7863 6f6e 7472 6962  ...sphinxcontrib
-00000560: 2d68 746d 6c68 656c 703d 3d32 2e30 2e31  -htmlhelp==2.0.1
-00000570: 0d0a 0973 7068 696e 7863 6f6e 7472 6962  ...sphinxcontrib
-00000580: 2d6a 7175 6572 793d 3d34 2e31 0d0a 0973  -jquery==4.1...s
-00000590: 7068 696e 7863 6f6e 7472 6962 2d6a 736d  phinxcontrib-jsm
-000005a0: 6174 683d 3d31 2e30 2e31 0d0a 0973 7068  ath==1.0.1...sph
-000005b0: 696e 7863 6f6e 7472 6962 2d71 7468 656c  inxcontrib-qthel
-000005c0: 703d 3d31 2e30 2e33 0d0a 0973 7068 696e  p==1.0.3...sphin
-000005d0: 7863 6f6e 7472 6962 2d73 6572 6961 6c69  xcontrib-seriali
-000005e0: 7a69 6e67 6874 6d6c 3d3d 312e 312e 350d  zinghtml==1.1.5.
-000005f0: 0a09 6661 7374 7472 6565 7368 6170 0d0a  ..fasttreeshap..
-00000600: 7465 7374 203d 200d 0a09 7079 7465 7374  test = ...pytest
-00000610: 0d0a 0970 7974 6573 742d 636f 760d 0a0d  ...pytest-cov...
-00000620: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000630: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000640: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000480: 0973 7068 696e 783c 372e 302e 300d 0a09  .sphinx<7.0.0...
+00000490: 7370 6869 6e78 6177 6573 6f6d 652d 7468  sphinxawesome-th
+000004a0: 656d 653d 3d34 2e31 2e30 0d0a 096e 6273  eme==4.1.0...nbs
+000004b0: 7068 696e 783d 3d30 2e39 2e32 0d0a 0973  phinx==0.9.2...s
+000004c0: 7068 696e 782d 6175 746f 646f 632d 7479  phinx-autodoc-ty
+000004d0: 7065 6869 6e74 733c 312e 3234 2e30 0d0a  pehints<1.24.0..
+000004e0: 0973 7068 696e 782d 636f 7079 6275 7474  .sphinx-copybutt
+000004f0: 6f6e 3d3d 302e 352e 320d 0a09 7370 6869  on==0.5.2...sphi
+00000500: 6e78 2d74 6162 733d 3d33 2e34 2e31 0d0a  nx-tabs==3.4.1..
+00000510: 0966 6173 7474 7265 6573 6861 700d 0a74  .fasttreeshap..t
+00000520: 6573 7420 3d20 0d0a 0970 7974 6573 740d  est = ...pytest.
+00000530: 0a09 7079 7465 7374 2d63 6f76 0d0a 0d0a  ..pytest-cov....
+00000540: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000550: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000560: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `arfs-2.0.3/src/arfs/association.py` & `arfs-2.0.4/src/arfs/association.py`

 * *Files 1% similar despite different names*

```diff
@@ -1432,15 +1432,16 @@
 
 ################################
 # Association predictor-target
 ################################
 
 
 def f_oneway_weighted(*args):
-    """Calculate the weighted F-statistic for one-way ANOVA (continuous target, categorical predictor).
+    """
+    Calculate the weighted F-statistic for one-way ANOVA (continuous target, categorical predictor).
 
     Parameters
     ----------
     X : array-like of shape (n_samples,)
         The predictor dataframe.
     y : array-like of shape (n_samples,)
         The target vector.
@@ -1451,14 +1452,15 @@
     -------
     float
         The value of the F-statistic.
 
     Notes
     -----
     The F-statistic is calculated as:
+
     .. math::
         F(rf) = \\frac{\\sum_i (\\bar{Y}_{i \\bullet} - \\bar{Y})^2 / (K-1)}{\\sum_i \\sum_k (\\bar{Y}_{ij} - \\bar{Y}_{i\\bullet})^2 / (N - K)}
     """
     # how many levels (predictor)
     n_classes = len(args)
     # convert to float 2-uple d'array
     args = [as_float_array(a) for a in args]
@@ -1663,21 +1665,21 @@
 
     return f_statistic.drop(labels=[target]).sort_values(ascending=False)
 
 
 def f_stat_regression_parallel(
     X, y, sample_weight=None, n_jobs=-1, force_finite=True, handle_na="drop"
 ):
-    """f_stat_regression_parallel computes the weighted explained variance for the provided categorical
-    and numerical predictors using parallelization of the code.
+    """
+    Compute the weighted explained variance for the provided categorical and numerical predictors using parallelization.
 
     Parameters
     ----------
     X : array-like of shape (n_samples, n_features)
-        Predictor dataframe.
+        The predictor dataframe.
     y : array-like of shape (n_samples,)
         The target vector.
     sample_weight : array-like of shape (n_samples,), optional
         The weight vector, by default None.
     n_jobs : int, optional
         The number of cores to use for the computation, by default -1.
     handle_na : str, optional
@@ -1831,15 +1833,16 @@
     X,
     y,
     sample_weight=None,
     n_jobs=-1,
     force_finite=True,
     handle_na="drop",
 ):
-    """Univariate information dependence.
+    """
+    Univariate information dependence.
 
     It ranks features in the same order if all the features are positively correlated with the target.
     Note that it is therefore recommended as a feature selection criterion to identify
     potentially predictive features for a downstream classifier, irrespective of
     the sign of the association with the target variable.
 
     Parameters
@@ -1854,23 +1857,23 @@
         The number of cores to use for the computation, by default -1.
     handle_na : str, optional
         Either drop rows with NaN, fill NaN with 0, or do nothing, by default "drop".
     force_finite : bool, optional
         Whether or not to force the F-statistics and associated p-values to
         be finite. There are two cases where the F-statistic is expected to not
         be finite:
-        - when the target `y` or some features in `X` are constant. In this
-          case, the Pearson's R correlation is not defined leading to obtain
-          `np.nan` values in the F-statistic and p-value. When
-          `force_finite=True`, the F-statistic is set to `0.0` and the
-          associated p-value is set to `1.0`.
-        - when a feature in `X` is perfectly correlated (or
-          anti-correlated) with the target `y`. In this case, the F-statistic
-          is expected to be `np.inf`. When `force_finite=True`, the F-statistic
-          is set to `np.finfo(dtype).max`.
+            - when the target `y` or some features in `X` are constant. In this
+              case, the Pearson's R correlation is not defined leading to obtain
+              `np.nan` values in the F-statistic and p-value. When
+              `force_finite=True`, the F-statistic is set to `0.0` and the
+              associated p-value is set to `1.0`.
+            - when a feature in `X` is perfectly correlated (or
+              anti-correlated) with the target `y`. In this case, the F-statistic
+              is expected to be `np.inf`. When `force_finite=True`, the F-statistic
+              is set to `np.finfo(dtype).max`.
 
     Returns
     -------
     f_statistic : array-like of shape (n_features,)
         F-statistic for each feature.
     """
     if not isinstance(y, pd.Series):
@@ -1904,21 +1907,21 @@
 
     return f_statistic.drop(labels=[target]).sort_values(ascending=False)
 
 
 def f_stat_classification_parallel(
     X, y, sample_weight=None, n_jobs=-1, force_finite=True, handle_na="drop"
 ):
-    """f_stat_classification_parallel computes the weighted ANOVA F-value for the provided categorical
-    and numerical predictors using parallelization of the code.
+    """
+    Compute the weighted ANOVA F-value for the provided categorical and numerical predictors using parallelization.
 
     Parameters
     ----------
     X : array-like of shape (n_samples, n_features)
-        Predictor dataframe.
+        The predictor dataframe.
     y : array-like of shape (n_samples,)
         The target vector.
     sample_weight : array-like of shape (n_samples,), optional
         The weight vector, by default None.
     n_jobs : int, optional
         The number of cores to use for the computation, by default -1.
     handle_na : str, optional
@@ -2106,34 +2109,35 @@
 
 ###############
 # visualization
 ###############
 
 
 def cluster_sq_matrix(sq_matrix, method="ward"):
-    """cluster_sq_matrix applies agglomerative clustering in order to sort
-    a correlation matrix.
+    """
+    Apply agglomerative clustering to sort a square correlation matrix.
 
     Parameters
     ----------
     sq_matrix : pd.DataFrame
-        a square correlation matrix
+        A square correlation matrix.
     method : str, optional
-        linkage method, by default "ward"
+        The linkage method, by default "ward".
 
     Returns
     -------
     pd.DataFrame
-        a sorted square matrix
+        A sorted square matrix.
+
+    Example
+    -------
+    >>> from some_module import association_matrix, cluster_sq_matrix
 
-    Example:
-    --------
     >>> assoc = association_matrix(iris_df, plot=False)
     >>> assoc_clustered = cluster_sq_matrix(assoc, method="complete")
-
     """
     d = sch.distance.pdist(sq_matrix.values)
     L = sch.linkage(d, method=method)
     ind = sch.fcluster(L, 0.5 * d.max(), "distance")
     columns = [sq_matrix.columns.tolist()[i] for i in list((np.argsort(ind)))]
     sq_matrix = sq_matrix.reindex(columns, axis=1)
     sq_matrix = sq_matrix.reindex(columns, axis=0)
```

### Comparing `arfs-2.0.3/src/arfs/benchmark.py` & `arfs-2.0.4/src/arfs/benchmark.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-2.0.4/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/src/arfs/dataset/data/housing.zip` & `arfs-2.0.4/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/src/arfs/feature_selection/__init__.py` & `arfs-2.0.4/src/arfs/feature_selection/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from .allrelevant import Leshy, BoostAGroota, GrootCV
 from .unsupervised import (
     MissingValueThreshold,
     UniqueValuesThreshold,
     CardinalityThreshold,
     CollinearityThreshold,
 )
+
+from .lasso import LassoFeatureSelection
 from .variable_importance import VariableImportance
 from .summary import make_fs_summary
 from .mrmr import MinRedundancyMaxRelevance
 
 __all__ = [
     "BaseThresholdSelector",
     "MissingValueThreshold",
@@ -17,8 +19,9 @@
     "CollinearityThreshold",
     "VariableImportance",
     "make_fs_summary",
     "Leshy",
     "BoostAGroota",
     "GrootCV",
     "MinRedundancyMaxRelevance",
+    "LassoFeatureSelection",
 ]
```

### Comparing `arfs-2.0.3/src/arfs/feature_selection/allrelevant.py` & `arfs-2.0.4/src/arfs/feature_selection/allrelevant.py`

 * *Files 3% similar despite different names*

```diff
@@ -949,67 +949,66 @@
             _iter += 1
             pbar.update(1)
 
         pbar.close()
         return dec_reg, sha_max_history, imp_history, imp_sha_max
 
     def _calculate_support(self, confirmed, tentative, n_feat):
-        """Calculates the feature support arrays for the BorutaPy feature selection algorithm.
+        """
+        Calculate the feature support arrays.
 
         Parameters
         ----------
-        confirmed : array-like of shape (n_features,)
+        confirmed : array-like of shape (n_confirmed,)
             Indices of confirmed features.
-
-        tentative : array-like of shape (n_features,)
+        tentative : array-like of shape (n_tentative,)
             Indices of tentative features.
-
         n_feat : int
-            Number of features in the dataset.
+            Total number of features.
 
         Returns
         -------
         None
-            The function only sets the following class attributes:
-
-            n_features_ : int
-                Number of confirmed features.
-
-            support_ : ndarray of bool, shape (n_features,)
-                Boolean array representing the confirmed features.
-
-            support_weak_ : ndarray of bool, shape (n_features,)
-                Boolean array representing the tentative features.
-
-        Notes
-        -----
-        - The function modifies the following class attributes:
-            * self.n_features_
-            * self.support_
-            * self.support_weak_
-        - If self.keep_weak is True, the support_weak_ is also added to the support_.
+            The function populates the following class attributes:
+            - n_features_ : int
+                Number of selected features.
+            - support_ : ndarray of shape (n_feat,)
+                Boolean array indicating the selected features.
+            - support_weak_ : ndarray of shape (n_feat,)
+                Boolean array indicating the tentatively selected features.
         """
         # basic result variables
         self.n_features_ = confirmed.shape[0]
         self.support_ = np.zeros(n_feat, dtype=bool)
         self.support_weak_ = np.zeros(n_feat, dtype=bool)
         self.support_[confirmed] = 1
         self.support_weak_ = np.zeros(n_feat, dtype=bool)
         self.support_weak_[tentative] = 1
         if self.keep_weak:
             self.support_[tentative] = 1
 
     def _calculate_absolute_ranking(self):
         """
-        Calculates the absolute ranking of the features based on their mean importance.
+        Compute feature importance scores using SHAP values.
 
-        Returns:
+        Parameters
+        ----------
+        new_x_tr : numpy.ndarray
+            The training dataset after being processed.
+        shap_matrix : numpy.ndarray
+            The matrix containing SHAP values computed by a LightGBM model.
+        param : dict
+            A dictionary containing the parameters for a LightGBM model.
+        objective : str
+            The objective function of the LightGBM model.
+
+        Returns
         -------
-        None
-            The function updates the `ranking_absolutes_` attribute of the instance with the absolute ranking.
+        list
+            A list of tuples containing feature names and their corresponding importance scores.
         """
         vimp_df = pd.DataFrame(self.imp_real_hist, columns=self.feature_names_in_)
         self.ranking_absolutes_ = list(
             vimp_df.mean().sort_values(ascending=False).index
         )
 
     def _calculate_relative_ranking(self, n_feat, tentative, confirmed, imp_history):
@@ -1058,35 +1057,29 @@
             self.ranking_[not_selected] = ranks
         else:
             # all are selected, thus we set feature supports to True
             self.support_ = np.ones(n_feat, dtype=bool)
 
     def _print_result(self, dec_reg, _iter, start_time):
         """
-        Calculate the feature support arrays.
+        Print the results of feature selection.
 
         Parameters
         ----------
-        confirmed : array-like of shape (n_confirmed,)
-            Indices of confirmed features.
-        tentative : array-like of shape (n_tentative,)
-            Indices of tentative features.
-        n_feat : int
-            Total number of features.
+        dec_reg : bool
+            Decision on whether to proceed with another round of feature selection.
+        _iter : int
+            Current iteration number.
+        start_time : float
+            Time when the feature selection process started.
 
         Returns
         -------
         None
-            The function populates the following class attributes:
-            - n_features_ : int
-                Number of selected features.
-            - support_ : ndarray of shape (n_feat,)
-                Boolean array indicating the selected features.
-            - support_weak_ : ndarray of shape (n_feat,)
-                Boolean array indicating the tentatively selected features.
+            The function prints the relevant results and running time.
         """
         if self.verbose > 0:
             self._print_results(dec_reg, _iter, 1)
         self.running_time = time.time() - start_time
         hours, rem = divmod(self.running_time, 3600)
         minutes, seconds = divmod(rem, 60)
         print(
@@ -1283,14 +1276,19 @@
         each iteration if the exact same columns are passed to the selection methods.
 
     Returns
     -------
     shap_imp : array
         The SHAP importance array.
     """
+    try:
+        from fasttreeshap import TreeExplainer as FastTreeExplainer
+    except ImportError:
+        ImportError("fasttreeshap is not installed")
+    
     # Clone the estimator to avoid modifying the original one
     estimator = clone(estimator)
 
     # Split the data into train and test sets and fit the model
     model, X_tt, y_tt, w_tt = _split_fit_estimator(
         estimator, X, y, sample_weight=sample_weight, cat_feature=cat_feature
     )
@@ -1413,69 +1411,70 @@
 
 ###################################
 #
 # BoostAGroota
 #
 ###################################
 class BoostAGroota(SelectorMixin, BaseEstimator):  # (object):
-    """BoostARoota becomes BoostAGroota, I'm Groot. BoostAGroota is an all relevant
-    feature selection method, while most other are minimal optimal;
-    this means it tries to find all features carrying
-    information usable for prediction, rather than finding a possibly compact
+    """
+    BoostAGroota is an all-relevant feature selection method, while most others are minimal optimal.
+    It tries to find all features carrying information usable for prediction, rather than finding a possibly compact
     subset of features on which some estimator has a minimal error.
-    Why bother with all relevant feature selection?
+
+    Why bother with all-relevant feature selection?
     When you try to understand the phenomenon that made your data, you should
     care about all factors that contribute to it, not just the bluntest signs
-    of it in context of your methodology (minimal optimal set of features
+    of it in the context of your methodology (minimal optimal set of features
     by definition depends on your estimator choice).
+
     Parameters
     ----------
-    estimator : sklear estimator
-        the model to train, lightGBM recommended, see the reduce lightgbm method
+    estimator : scikit-learn estimator
+        The model to train, lightGBM recommended, see the reduce lightgbm method.
     cutoff : float
-        the value by which the max of shadow imp is divided, to compare to real importance
+        The value by which the max of shadow imp is divided, to compare to real importance.
     iters : int (>0)
         The number of iterations to average for the feature importance (on the same split),
-        to reduce the variance
+        to reduce the variance.
     max_rounds : int (>0)
-        The number of times the core BoostARoota algorithm will run.
-        Each round eliminates more and more features
+        The number of times the core BoostAGroota algorithm will run.
+        Each round eliminates more and more features.
     delta : float (0 < delta <= 1)
-        Stopping criteria for whether another round is started
+        Stopping criteria for whether another round is started.
     silent : bool
-        Set to True if don't want to see the BoostARoota output printed.
+        Set to True if you don't want to see the BoostAGroota output printed.
     importance : str, default='shap'
-        the kind of feature importance to use. Possible values: 'shap' (Shapley values),
-        'pimp' (permutation importance) and 'native' (Gini/impurity)
+        The kind of feature importance to use. Possible values: 'shap' (Shapley values),
+        'pimp' (permutation importance), and 'native' (Gini/impurity).
+
     Attributes
     ----------
     selected_features_ : list of str
-        the list of columns to keep
+        The list of columns to keep.
     ranking_ : array of shape [n_features]
         The feature ranking, such that ``ranking_[i]`` corresponds to the
         ranking position of the i-th feature. Selected (i.e., estimated
-        best) features are assigned rank 1 and tentative features are assigned
+        best) features are assigned rank 1, and tentative features are assigned
         rank 2.
     ranking_absolutes_ : array of shape [n_features]
-        The absolute feature ranking as ordered by selection process. It does not guarantee
-        that this order is correct for all models. For a model agnostic ranking, see the
-        the attribute ``ranking``
+        The absolute feature ranking as ordered by the selection process. It does not guarantee
+        that this order is correct for all models. For a model-agnostic ranking, see the
+        attribute ``ranking``.
     sha_cutoff_df : dataframe
-        feature importance of the real+shadow predictors over iterations
+        Feature importance of the real+shadow predictors over iterations.
     mean_shadow : float
-        the threshold below which the predictors are rejected
+        The threshold below which the predictors are rejected.
+
     Examples
     --------
     >>> X = df[filtered_features].copy()
     >>> y = df['target'].copy()
     >>> w = df['weight'].copy()
-    >>>
-    >>> model = LGBMRegressor(n_jobs=-1, n_estimators=100, objective='rmse',
-    >>>                       random_state=42, verbose=0)
-    >>> feat_selector = BoostAGroota(est=model, cutoff=1, iters=10, max_rounds=10, delta=0.1, importance='shap')
+    >>> model = LGBMRegressor(n_jobs=-1, n_estimators=100, objective='rmse', random_state=42, verbose=0)
+    >>> feat_selector = BoostAGroota(estimator=model, cutoff=1, iters=10, max_rounds=10, delta=0.1, importance='shap')
     >>> feat_selector.fit(X, y, sample_weight=None)
     >>> print(feat_selector.selected_features_)
     >>> feat_selector.plot_importance(n_feat_per_inch=5)
     """
 
     def __init__(
         self,
@@ -1708,15 +1707,16 @@
     n_iterations,
     delta,
     silent,
     weight,
     imp_kind,
     cat_feature,
 ):
-    """Private function, reduce the number of predictors using a sklearn estimator
+    """
+    Private function, reduce the number of predictors using a sklearn estimator
 
     Parameters
     ----------
     x : pd.DataFrame
         the dataframe to create shadow features on
     y : pd.Series
         the target
@@ -1818,47 +1818,51 @@
 
     return criteria, real_vars["feature"], df, mean_shadow
 
 
 def _boostaroota(
     X, y, estimator, cutoff, iters, max_rounds, delta, silent, weight, imp
 ):
-    """Private function, reduce the number of predictors using a sklearn estimator
+    """
+    Private function, reduces the number of predictors using a sklearn estimator.
+
     Parameters
+    ----------
     x : pd.DataFrame
-        the dataframe to create shadow features on
+        The dataframe to create shadow features on.
     y : pd.Series
-        the target
-    estimator : sklear estimator
-        the model to train, lightGBM recommended, see the reduce lightgbm method
+        The target.
+    estimator : scikit-learn estimator
+        The model to train, lightGBM recommended, see the reduce lightgbm method.
     cutoff : float
-        the value by which the max of shadow imp is divided, to compare to real importance
+        The value by which the max of shadow imp is divided, to compare to real importance.
     iters : int (>0)
         The number of iterations to average for the feature importances (on the same split),
-        to reduce the variance
+        to reduce the variance.
     max_rounds : int (>0)
         The number of times the core BoostARoota algorithm will run.
-        Each round eliminates more and more features
+        Each round eliminates more and more features.
     delta : float (0 < delta <= 1)
-        Stopping criteria for whether another round is started
+        Stopping criteria for whether another round is started.
     silent : bool
-        Set to True if don't want to see the BoostARoota output printed.
-        Will still show any errors or warnings that may occur
-    weight : pd.series
-        sample_weight, if any
+        Set to True if you don't want to see the BoostARoota output printed.
+        Will still show any errors or warnings that may occur.
+    weight : pd.Series, optional
+        Sample weights, if any.
+
     Returns
     -------
     crit : bool
-        if the criteria has been reached or not
-    keep_vars : pd.dataframe
-        feature importance of the real predictors over iter
+        If the criteria have been reached or not.
+    keep_vars : pd.DataFrame
+        Feature importance of the real predictors over iterations.
     df_vimp : pd.DataFrame
-        feature importance of the real+shadow predictors over iter
+        Feature importance of the real+shadow predictors over iterations.
     mean_shadow : float
-        the feature importance threshold, to reject or not the predictors
+        The feature importance threshold to reject or not the predictors.
     """
     start_time = time.time()
     new_x = X.copy()
 
     # extract the categorical names for the first time, store it for next iterations
     # In the below while loop this list will be update only once some of the predictors
     # are removed. This way the encoding is done only every predictors update and not
@@ -1912,75 +1916,80 @@
 #
 # GrootCV
 #
 ###################################
 
 
 class GrootCV(SelectorMixin, BaseEstimator):
-    """A shuffled copy of the predictors matrix is added (shadows) to the original set of predictors.
+    """
+    GrootCV is a feature selection method based on cross-validation with lightGBM.
+
+    A shuffled copy of the predictors matrix is added (shadows) to the original set of predictors.
     The lightGBM is fitted using repeated cross-validation, the feature importance
     is extracted each time and averaged to smooth out the noise.
-    If the feature importance is larger than the average shadow feature importance then the predictors
-    are rejected, the others are kept.
-    - Cross-validated feature importance to smooth out the noise, based on lightGBM only
-      (which is, most of the time, the fastest and more accurate Boosting).
-    - the feature importance is derived using SHAP importance
-    - Taking the max of median of the shadow var. imp over folds otherwise not enough conservative and
-      it improves the convergence (needs less evaluation to find a threshold)
-    - Not based on a given percentage of cols needed to be deleted
-    - Plot method for var. imp
+    If the feature importance is larger than the average shadow feature importance then the predictors are rejected, the others are kept.
+        - Cross-validated feature importance to smooth out the noise, based on lightGBM only
+          (which is, most of the time, the fastest and more accurate Boosting).
+        - the feature importance is derived using SHAP importance
+        - Taking the max of median of the shadow var. imp over folds otherwise not enough conservative and
+          it improves the convergence (needs less evaluation to find a threshold)
+        - Not based on a given percentage of cols needed to be deleted
+        - Plot method for var. imp
 
     Parameters
     ----------
-    objective: str
-        the lightGBM objective
-    cutoff: float
-        the value by which the max of shadow imp is divided, to compare to real importance
-    n_folds: int, default=5
-        the number of folds for the cross-val
-    n_iter: int, default=5
-        the number of times the cross-validation is repeated
-    silent: bool, default=False
-        print out details or not
-    rf: bool, default=False
-        the lightGBM implementation of the random forest
-    fastshap: bool, default=True
-        enable or not the fasttreeshap (LinkedIn) implementation of the shap values
-    lgbm_params: dict, Optional
-        the parameters to pass to the lightGBM algorithm (python API). Note that some of
-        those parameters will be overridden by the algorithm. Namely:
-        objective, verbose, is_balanced
-    n_jobs: int, default 0
-        0 means default number of threads in OpenMP
-        for the best speed, set this to the number of real CPU cores, not the number of threads
-
+    objective : str or callable, default=None
+        The objective function to use in lightGBM. If None, it uses the objective specified in `lgbm_params`.
+    cutoff : float, default=1
+        The value by which the max of shadow imp is divided, to compare to real importance.
+    n_folds : int, default=5
+        The number of folds for cross-validation.
+    n_iter : int, default=5
+        The number of iterations to average for the feature importance (on the same split), to reduce variance.
+    silent : bool, default=True
+        Set to True if you don't want to see the GrootCV output printed.
+    rf : bool, default=False
+        If True, use random forest for calculating feature importances; otherwise, use lightGBM.
+    fastshap : bool, default=False
+        If True, use fastSHAP for calculating feature importances; otherwise, use SHAP.
+    n_jobs : int, default=0
+        The number of jobs to run in parallel. If 0, no parallelism is used.
+    lgbm_params : dict, default=None
+        The parameters for the lightGBM model.
 
     Attributes
     ----------
-    selected_features_: list of str
-        the list of columns to keep
-    ranking_ : array of shape [n_features]
-        The feature ranking, such that ``ranking_[i]`` corresponds to the
-        ranking position of the i-th feature. Selected (i.e., estimated
-        best) features are assigned rank 1 and tentative features are assigned
-        rank 2.
-    ranking_absolutes_ : array of shape [n_features]
-        The absolute feature ranking as ordered by selection process. It does not guarantee
-        that this order is correct for all models. For a model agnostic ranking, see the
-        the attribute ``ranking``
-    cv_df: dataframe
-        the statistics of the feature importance over the different repeats of the X-val
-    sha_cutoff: float
-        the threshold below which the predictors are rejected
+    selected_features_ : ndarray
+        The list of columns to keep as selected features.
+    cv_df : pd.DataFrame
+        DataFrame containing feature importance values for each fold and iteration.
+    sha_cutoff : float
+        The threshold below which the predictors are rejected.
+    ranking_absolutes_ : list
+        The absolute feature ranking as ordered by the selection process.
+    ranking_ : ndarray
+        The feature ranking, where 2 corresponds to selected features and 1 to tentative features.
+
+    Methods
+    -------
+    fit(X, y, sample_weight=None)
+        Fit the GrootCV on the input data.
+    transform(X)
+        Apply the fitted GrootCV on new data.
+    plot_importance(n_feat_per_inch=5)
+        Plot the feature importance of the fitted GrootCV.
+
+    Warnings
+    --------
+    If `sha_cutoff` is None, you should apply the fit method first.
     Examples
     -------
     >>> X = df[filtered_features].copy()
     >>> y = df['target'].copy()
     >>> w = df['weight'].copy()
-    >>>
     >>> feat_selector = arfsgroot.GrootCV(objective='rmse', cutoff = 1, n_folds=5, n_iter=5)
     >>> feat_selector.fit(X, y, sample_weight=None)
     >>> feat_selector.plot_importance(n_feat_per_inch=5)
     """
 
     def __init__(
         self,
@@ -2010,29 +2019,30 @@
 
         # Throw errors if the inputted parameters don't meet the necessary criteria
         # Ensure parameters meet necessary criteria
         if cutoff <= 0 or n_iter <= 0 or n_folds <= 0:
             raise ValueError("cutoff, n_iter, and n_folds should be greater than 0.")
 
     def fit(self, X, y, sample_weight=None):
-        """Fit the GrootCV transformer with the provided estimator.
+        """
+        Fit the GrootCV on the input data.
 
         Parameters
         ----------
-        X : pd.DataFrame
-            the predictors matrix
-        y : pd.Series
-            the target
-        sample_weight : pd.Series, optional
-            sample weights, if any
+        X : pd.DataFrame of shape (n_samples, n_features)
+            The predictor dataframe.
+        y : array-like of shape (n_samples,)
+            The target vector.
+        sample_weight : array-like of shape (n_samples,), optional
+            The weight vector, by default None.
 
         Returns
         -------
-        self : GrootCV
-            fitted estimator
+        self : object
+            Returns self.
         """
 
         if not isinstance(X, pd.DataFrame):
             raise TypeError("X is not a pandas DataFrame")
 
         self.feature_names_in_ = X.columns.to_numpy()
         y = pd.Series(y) if not isinstance(y, pd.Series) else y
@@ -2077,34 +2087,48 @@
 
     def _get_support_mask(self):
         check_is_fitted(self)
 
         return self.support_
 
     def transform(self, X):
+        """
+        Apply the fitted GrootCV on new data.
+
+        Parameters
+        ----------
+        X : pd.DataFrame of shape (n_samples, n_features)
+            The predictor dataframe.
+
+        Returns
+        -------
+        X_selected : pd.DataFrame of shape (n_samples, n_selected_features)
+            The selected features from the input dataframe.
+        """
         if not isinstance(X, pd.DataFrame):
             raise TypeError("X is not a dataframe")
         return X[self.selected_features_]
 
     def _more_tags(self):
         return {"allow_nan": True, "requires_y": True}
 
     @mpl.rc_context(PLT_PARAMS)
     def plot_importance(self, n_feat_per_inch=5):
-        """Boxplot of the variable importance, ordered by magnitude
-        The max shadow variable importance illustrated by the dashed line.
-        Requires to apply the fit method first.
+        """
+        Plot the feature importance of the fitted GrootCV.
+
         Parameters
         ----------
         n_feat_per_inch : int, default=5
-            number of features to plot per inch (for scaling the figure)
+            The number of features per inch in the plot.
+
         Returns
         -------
-        fig : plt.figure
-            the matplotlib figure object containing the boxplot
+        fig : matplotlib.figure.Figure or None
+            The matplotlib figure containing the plot or None if no feature is selected.
         """
 
         if self.sha_cutoff is None:
             raise ValueError("Apply fit method first")
 
         b_df = self.cv_df.T.copy()
         b_df.columns = b_df.iloc[0]
@@ -2511,30 +2535,29 @@
     else:
         shap_matrix = bst.predict(X_train, pred_contrib=True)
 
     return bst, shap_matrix, bst.best_iteration
 
 
 def _compute_importance(new_x_tr, shap_matrix, param, objective, fastshap):
-    """
-    Compute feature importance scores using SHAP values.
+    """Compute feature importance scores using SHAP values.
 
-    Parameters:
-    -----------
+    Parameters
+    ----------
     new_x_tr : numpy.ndarray
         The training dataset after being processed.
     shap_matrix : numpy.ndarray
         The matrix containing SHAP values computed by a LightGBM model.
     param : dict
         A dictionary containing the parameters for a LightGBM model.
     objective : str
         The objective function of the LightGBM model.
 
-    Returns:
-    --------
+    Returns
+    -------
     list
         A list of tuples containing feature names and their corresponding importance scores.
     """
     if fastshap:
         if objective == "softmax":
             shap_matrix = np.abs(np.concatenate(shap_matrix, axis=1))
         shap_imp = np.mean(np.abs(shap_matrix), axis=0)
```

### Comparing `arfs-2.0.3/src/arfs/feature_selection/base.py` & `arfs-2.0.4/src/arfs/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/src/arfs/feature_selection/lasso.py` & `arfs-2.0.4/src/arfs/feature_selection/lasso.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,25 +85,25 @@
         Parameters
         ----------
         family :
             The distributional assumption of the model.
         link:
             the GLM link function
         alpha :
-            The penalty weight. If a scalar, the same penalty weight applies to all variables in the model. 
+            The penalty weight. If a scalar, the same penalty weight applies to all variables in the model.
             If a vector, it must have the same length as params, and contains a penalty weight for each coefficient.
         L1_wt :
-            The `L1_wt` parameter represents the weight of the L1 penalty term in the model and 
-            should be within the range 0 to 1. A value of 0 corresponds to ridge regression, 
-            while a value of 1 corresponds to lasso regression. However, for obtaining statistics, 
-            `L1_wt` should be set to a value greater than 0. If it is set to 0.0, statsmodels returns 
-            a ridge regularized wrapper without refitting the model, making the statistics unavailable 
-            and breaking the class. Nevertheless, you can set `L1_wt` to a very small value, such as 1e-9, 
+            The `L1_wt` parameter represents the weight of the L1 penalty term in the model and
+            should be within the range 0 to 1. A value of 0 corresponds to ridge regression,
+            while a value of 1 corresponds to lasso regression. However, for obtaining statistics,
+            `L1_wt` should be set to a value greater than 0. If it is set to 0.0, statsmodels returns
+            a ridge regularized wrapper without refitting the model, making the statistics unavailable
+            and breaking the class. Nevertheless, you can set `L1_wt` to a very small value, such as 1e-9,
             to obtain close-to-ridge behavior while still obtaining the necessary statistics.
-            
+
         fit_intercept :
             Whether to fit an intercept term in the model.
         """
         self.family = family
         self.link = link
         self.alpha = alpha
         self.L1_wt = L1_wt
@@ -153,21 +153,21 @@
             Sample weights.
 
         Returns
         -------
         self : object
             Returns self.
         """
-        
+
         # see the if kwargs.get("L1_wt", 1) == 0 condition in
         # https://www.statsmodels.org/dev/_modules/statsmodels/genmod/generalized_linear_model.html#GLM.fit_regularized
         # workaround to get the statistics
         if self.alpha == 0.0:
             self.alpha = 1e-9
-        
+
         if not isinstance(X, pd.DataFrame):
             X = pd.DataFrame(X)
             X.columns = [f"pred_{i}" for i in range(X.shape[1])]
 
         if self.fit_intercept:
             X = sm.add_constant(X)
             X = X.rename(columns={"const": "Intercept"})
```

### Comparing `arfs-2.0.3/src/arfs/feature_selection/mrmr.py` & `arfs-2.0.4/src/arfs/feature_selection/mrmr.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/src/arfs/feature_selection/summary.py` & `arfs-2.0.4/src/arfs/feature_selection/summary.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/src/arfs/feature_selection/unsupervised.py` & `arfs-2.0.4/src/arfs/feature_selection/unsupervised.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/src/arfs/feature_selection/variable_importance.py` & `arfs-2.0.4/src/arfs/feature_selection/variable_importance.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/src/arfs/gbm.py` & `arfs-2.0.4/src/arfs/gbm.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/src/arfs/parallel.py` & `arfs-2.0.4/src/arfs/parallel.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/src/arfs/preprocessing.py` & `arfs-2.0.4/src/arfs/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from .gbm import GradientBoosting
 from .utils import create_dtype_dict
 
 
 # fix random seed for reproducibility
 np.random.seed(7)
 
+
 class OrdinalEncoderPandas(OrdinalEncoder):
     # class OrdinalEncoderPandas(BaseEstimator, TransformerMixin):
     """Encode categorical features as an integer array and returns a pandas DF.
     The features are converted to ordinal integers. This results in
     a single column of integers (0 to n_categories - 1) per feature.
     Read more in the scikit-learn OrdinalEncoder documentation
 
@@ -387,18 +388,19 @@
         # Map is faster than replace
     if return_cat:
         df.loc[:, non_num_cols] = df.loc[:, non_num_cols].astype("category")
     return df, cat_var_df, inv_mapper, mapper
 
 
 class TreeDiscretizer(BaseEstimator, TransformerMixin):
-    """The purpose of the function is to discretize continuous and/or categorical data, returning a pandas DataFrame.
-    It is designed to support regression and binary classification tasks. Discretization, also known as quantization or binning,
-    allows for the partitioning of continuous features into discrete values. In certain datasets with continuous attributes,
-    discretization can be beneficial as it transforms the dataset into one with only nominal attributes.
+    """
+    Discretize continuous and/or categorical data using univariate regularized trees, returning a pandas DataFrame.
+    The TreeDiscretizer is designed to support regression and binary classification tasks.
+    Discretization, also known as quantization or binning, allows for the partitioning of continuous features into discrete values.
+    In certain datasets with continuous attributes, discretization can be beneficial as it transforms the dataset into one with only nominal attributes.
     Additionally, for categorical predictors, grouping levels can help reduce overfitting and create meaningful clusters.
 
     By encoding discretized features, a model can become more expressive while maintaining interpretability.
     For example, preprocessing with a discretizer can introduce nonlinearity to linear models.
     For more advanced possibilities, particularly smooth ones, you can refer to the section on generating polynomial features.
     The TreeDiscretizer function utilizes univariate regularized trees, with one tree per column to be binned.
     It finds the optimal partition and returns numerical intervals for numerical continuous columns and pd.Categorical for categorical columns.
@@ -498,30 +500,30 @@
         self.bin_upper_bound_dic = {}
         self.cat_bin_dict = {}
         self.tree_imputer = {}
         self.ordinal_encoder_dic = {}
         self.cat_features = None
 
     def fit(self, X, y, sample_weight=None):
-        """Fit the discretizer on `X`.
+        """
+        Fit the TreeDiscretizer on the input data.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
-            Input data with shape (n_samples, n_features), where `n_samples` is the number of samples and
-            `n_features` is the number of features.
+            The predictor dataframe.
         y : array-like of shape (n_samples,)
-            Target for internally fitting the tree(s).
+            The target vector.
         sample_weight : array-like of shape (n_samples,), optional
-            Sample weight (e.g., exposure) if any.
+            The weight vector, by default None.
 
         Returns
         -------
-        X : pd.DataFrame
-            DataFrame with the binned and grouped columns.
+        self : object
+            Returns self.
         """
         X = X.copy()
 
         if not isinstance(X, pd.DataFrame):
             X = pd.DataFrame(X)
             X.columns = [f"pred_{i}" for i in range(X.shape[1])]
 
@@ -636,15 +638,16 @@
                 ]
 
             del tree
 
         return self
 
     def transform(self, X):
-        """Apply the discretizer on `X`. Only the columns with more than n_bins_max unique values will be transformed.
+        """
+        Apply the discretizer on `X`. Only the columns with more than n_bins_max unique values will be transformed.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             Input data with shape (n_samples, n_features), where `n_samples` is the number of samples and
             `n_features` is the number of features.
 
@@ -686,15 +689,16 @@
 
                     if not self.num_bins_as_category:
                         X[col] = X[col].astype(IntervalDtype())
         return X
 
 
 def highlight_discarded(s):
-    """highlight X in red and V in green.
+    """
+    highlight X in red and V in green.
 
     Parameters
     ----------
     s : np.arrays
 
     Returns
     -------
```

### Comparing `arfs-2.0.3/src/arfs/sampling.py` & `arfs-2.0.4/src/arfs/sampling.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/src/arfs/utils.py` & `arfs-2.0.4/src/arfs/utils.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/src/arfs.egg-info/PKG-INFO` & `arfs-2.0.4/src/arfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arfs
-Version: 2.0.3
+Version: 2.0.4
 Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
 Author: ThomasBury
 Author-email: bury.thomas@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ThomasBury/arfs
 Project-URL: Source, https://github.com/ThomasBury/arfs
 Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
```

### Comparing `arfs-2.0.3/src/arfs.egg-info/SOURCES.txt` & `arfs-2.0.4/src/arfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/tests/test_allrelevant.py` & `arfs-2.0.4/tests/test_allrelevant.py`

 * *Files identical despite different names*

### Comparing `arfs-2.0.3/tests/test_featselect.py` & `arfs-2.0.4/tests/test_featselect.py`

 * *Files identical despite different names*

