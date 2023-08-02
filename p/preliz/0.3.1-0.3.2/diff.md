# Comparing `tmp/preliz-0.3.1.tar.gz` & `tmp/preliz-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preliz-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "preliz-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `preliz-0.3.1.tar` & `preliz-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     3712 2023-07-08 12:03:31.873032 preliz-0.3.1/README.md
--rw-r--r--   0        0        0      649 2023-07-08 12:03:32.033036 preliz-0.3.1/preliz/__init__.py
--rw-r--r--   0        0        0     1037 2023-07-08 12:03:32.033036 preliz-0.3.1/preliz/distributions/__init__.py
--rw-r--r--   0        0        0    89186 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/distributions/continuous.py
--rw-r--r--   0        0        0    14095 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/distributions/continuous_multivariate.py
--rw-r--r--   0        0        0    43519 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/distributions/discrete.py
--rw-r--r--   0        0        0    19949 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/distributions/distributions.py
--rw-r--r--   0        0        0     6516 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/distributions/distributions_multivariate.py
--rw-r--r--   0        0        0       64 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/internal/__init__.py
--rw-r--r--   0        0        0     4659 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/internal/distribution_helper.py
--rw-r--r--   0        0        0     8770 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/internal/optimization.py
--rw-r--r--   0        0        0     3043 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/internal/parser.py
--rw-r--r--   0        0        0    15583 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/internal/plot_helper.py
--rw-r--r--   0        0        0     8168 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/internal/plot_helper_multivariate.py
--rw-r--r--   0        0        0      114 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/predictive/__init__.py
--rw-r--r--   0        0        0    14107 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/predictive/ppa.py
--rw-r--r--   0        0        0     1345 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/predictive/predictive_sliders.py
--rw-r--r--   0        0        0     1946 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/check_inside_notebook.ipynb
--rw-r--r--   0        0        0     1799 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/plot_interactive.ipynb
--rw-r--r--   0        0        0     2244 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/predictive_sliders.ipynb
--rw-r--r--   0        0        0     1472 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/roulette.ipynb
--rw-r--r--   0        0        0     7434 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_distributions.py
--rw-r--r--   0        0        0      626 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_helper.py
--rw-r--r--   0        0        0      338 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_internals.py
--rw-r--r--   0        0        0     6634 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_maxent.py
--rw-r--r--   0        0        0     2919 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_mle.py
--rw-r--r--   0        0        0     2828 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_plots.py
--rw-r--r--   0        0        0      115 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_predictive_sliders.py
--rw-r--r--   0        0        0     3483 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_quartile.py
--rw-r--r--   0        0        0      906 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/tests/test_roulette.py
--rw-r--r--   0        0        0      164 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/unidimensional/__init__.py
--rw-r--r--   0        0        0     3898 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/unidimensional/maxent.py
--rw-r--r--   0        0        0     1681 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/unidimensional/mle.py
--rw-r--r--   0        0        0     3214 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/unidimensional/quartile.py
--rw-r--r--   0        0        0     9633 2023-07-08 12:03:32.037036 preliz-0.3.1/preliz/unidimensional/roulette.py
--rw-r--r--   0        0        0     1393 2023-07-08 12:03:32.037036 preliz-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 preliz-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3712 2023-08-02 19:34:52.997219 preliz-0.3.2/README.md
+-rw-r--r--   0        0        0      649 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/__init__.py
+-rw-r--r--   0        0        0     1037 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/distributions/__init__.py
+-rw-r--r--   0        0        0    89183 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/distributions/continuous.py
+-rw-r--r--   0        0        0    14095 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/distributions/continuous_multivariate.py
+-rw-r--r--   0        0        0    43519 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/distributions/discrete.py
+-rw-r--r--   0        0        0    20075 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/distributions/distributions.py
+-rw-r--r--   0        0        0     6516 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/distributions/distributions_multivariate.py
+-rw-r--r--   0        0        0       64 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/internal/__init__.py
+-rw-r--r--   0        0        0     4659 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/internal/distribution_helper.py
+-rw-r--r--   0        0        0     8770 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/internal/optimization.py
+-rw-r--r--   0        0        0     3043 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/internal/parser.py
+-rw-r--r--   0        0        0    15617 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/internal/plot_helper.py
+-rw-r--r--   0        0        0     8168 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/internal/plot_helper_multivariate.py
+-rw-r--r--   0        0        0      114 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/predictive/__init__.py
+-rw-r--r--   0        0        0    14145 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/predictive/ppa.py
+-rw-r--r--   0        0        0     1383 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/predictive/predictive_sliders.py
+-rw-r--r--   0        0        0     1946 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/tests/check_inside_notebook.ipynb
+-rw-r--r--   0        0        0     1799 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/tests/plot_interactive.ipynb
+-rw-r--r--   0        0        0     2244 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/tests/predictive_sliders.ipynb
+-rw-r--r--   0        0        0     1472 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/tests/roulette.ipynb
+-rw-r--r--   0        0        0     7434 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/tests/test_distributions.py
+-rw-r--r--   0        0        0      626 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/tests/test_helper.py
+-rw-r--r--   0        0        0      338 2023-08-02 19:34:53.173220 preliz-0.3.2/preliz/tests/test_internals.py
+-rw-r--r--   0        0        0     6634 2023-08-02 19:34:53.177221 preliz-0.3.2/preliz/tests/test_maxent.py
+-rw-r--r--   0        0        0     2919 2023-08-02 19:34:53.177221 preliz-0.3.2/preliz/tests/test_mle.py
+-rw-r--r--   0        0        0     2828 2023-08-02 19:34:53.177221 preliz-0.3.2/preliz/tests/test_plots.py
+-rw-r--r--   0        0        0      115 2023-08-02 19:34:53.177221 preliz-0.3.2/preliz/tests/test_predictive_sliders.py
+-rw-r--r--   0        0        0     3483 2023-08-02 19:34:53.177221 preliz-0.3.2/preliz/tests/test_quartile.py
+-rw-r--r--   0        0        0      906 2023-08-02 19:34:53.177221 preliz-0.3.2/preliz/tests/test_roulette.py
+-rw-r--r--   0        0        0      164 2023-08-02 19:34:53.177221 preliz-0.3.2/preliz/unidimensional/__init__.py
+-rw-r--r--   0        0        0     3898 2023-08-02 19:34:53.177221 preliz-0.3.2/preliz/unidimensional/maxent.py
+-rw-r--r--   0        0        0     1681 2023-08-02 19:34:53.177221 preliz-0.3.2/preliz/unidimensional/mle.py
+-rw-r--r--   0        0        0     3212 2023-08-02 19:34:53.177221 preliz-0.3.2/preliz/unidimensional/quartile.py
+-rw-r--r--   0        0        0     9670 2023-08-02 19:34:53.177221 preliz-0.3.2/preliz/unidimensional/roulette.py
+-rw-r--r--   0        0        0     1393 2023-08-02 19:34:53.177221 preliz-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 preliz-0.3.2/PKG-INFO
```

### Comparing `preliz-0.3.1/README.md` & `preliz-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/__init__.py` & `preliz-0.3.2/preliz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .distributions import *
 from .predictive import *
 from .unidimensional import *
 
 
 __all__ = ["maxent", "mle", "ppa", "roulette", "quartile"]
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 _log = logging.getLogger("preliz")
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
```

### Comparing `preliz-0.3.1/preliz/distributions/__init__.py` & `preliz-0.3.2/preliz/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/distributions/continuous.py` & `preliz-0.3.2/preliz/distributions/continuous.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     def _parametrization(self, alpha=None, beta=None, mu=None, sigma=None, kappa=None):
         if (
             any_not_none(alpha, beta)
             and any_not_none(mu, sigma, kappa)
             or all_not_none(sigma, kappa)
         ):
             raise ValueError(
-                "Incompatible parametrization. Either use alpha " "and beta, or mu and sigma."
+                "Incompatible parametrization. Either use alpha and beta, or mu and sigma."
             )
 
         self.param_names = ("alpha", "beta")
         self.params_support = ((eps, np.inf), (eps, np.inf))
 
         if any_not_none(mu, sigma):
             self.mu = mu
```

### Comparing `preliz-0.3.1/preliz/distributions/continuous_multivariate.py` & `preliz-0.3.2/preliz/distributions/continuous_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/distributions/discrete.py` & `preliz-0.3.2/preliz/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/distributions/distributions.py` & `preliz-0.3.2/preliz/distributions/distributions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Parent classes for all families.
 """
 # pylint: disable=no-member
 import warnings
 from collections import namedtuple
 
-from ipywidgets import interactive
+try:
+    from ipywidgets import interactive
+except ImportError:
+    pass
 import numpy as np
 
 from ..internal.plot_helper import (
     plot_pdfpmf,
     plot_cdf,
     plot_ppf,
     get_slider,
@@ -436,15 +439,15 @@
         check_inside_notebook()
 
         if valid_scalar_params(self, check_frozen=False):
             args = dict(zip(self.param_names, self.params))
         else:
             args = init_vals[self.__class__.__name__]
 
-        self.__init__(**args)
+        self.__init__(**args)  # pylint: disable=unnecessary-dunder-call
 
         if fixed_lim is not None:
             warnings.warn(
                 "The 'fixed_lim' parameter will be deprecated. Use 'xy_lim' instead.",
                 FutureWarning,
             )
             xy_lim = fixed_lim
@@ -478,15 +481,17 @@
 
         def plot(**args):  # pylint: disable=inconsistent-return-statements
             if self.__class__.__name__ == "Categorical":
                 values = list(args.values())
                 args = {list(args.keys())[0].split("_")[0]: values}
                 if np.sum(values) > 1:
                     return None
-            self.__init__(**args)
+
+            self.__init__(**args)  # pylint: disable=unnecessary-dunder-call
+
             if kind == "pdf":
                 ax = self.plot_pdf(
                     legend=False,
                     pointinterval=pointinterval,
                     interval=interval,
                     levels=levels,
                     figsize=figsize,
```

### Comparing `preliz-0.3.1/preliz/distributions/distributions_multivariate.py` & `preliz-0.3.2/preliz/distributions/distributions_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/internal/distribution_helper.py` & `preliz-0.3.2/preliz/internal/distribution_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/internal/optimization.py` & `preliz-0.3.2/preliz/internal/optimization.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/internal/parser.py` & `preliz-0.3.2/preliz/internal/parser.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/internal/plot_helper.py` & `preliz-0.3.2/preliz/internal/plot_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import inspect
 import logging
 import traceback
 import sys
 
 from IPython import get_ipython
-from ipywidgets import FloatSlider, IntSlider
+
+try:
+    from ipywidgets import FloatSlider, IntSlider
+except ImportError:
+    pass
 from arviz import plot_kde, plot_ecdf, hdi
 from arviz.stats.density_utils import _kde_linear
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import _pylab_helpers, get_backend
 from matplotlib.ticker import MaxNLocator
 from scipy.interpolate import interp1d, PchipInterpolator
@@ -233,15 +237,15 @@
 def side_legend(ax):
     bbox = ax.get_position()
     ax.set_position([bbox.x0, bbox.y0, bbox.width, bbox.height])
     ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
 
 
 def repr_to_matplotlib(distribution):
-    string = distribution.__repr__()
+    string = repr(distribution)
     string = string.replace("\x1b[1m", r"$\bf{")
     string = string.replace("\x1b[0m", "}$")
     return string
 
 
 def get_moments(dist, moments):
     names = {
```

### Comparing `preliz-0.3.1/preliz/internal/plot_helper_multivariate.py` & `preliz-0.3.2/preliz/internal/plot_helper_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/predictive/ppa.py` & `preliz-0.3.2/preliz/predictive/ppa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Prior predictive check assistant."""
 
 import logging
 from random import shuffle
 from sys import modules
 
-import ipywidgets as widgets
+try:
+    import ipywidgets as widgets
+except ImportError:
+    pass
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.spatial import KDTree
 
 
 from ..internal.plot_helper import (
     check_inside_notebook,
```

### Comparing `preliz-0.3.1/preliz/predictive/predictive_sliders.py` & `preliz-0.3.2/preliz/predictive/predictive_sliders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from ipywidgets import interactive
+try:
+    from ipywidgets import interactive
+except ImportError:
+    pass
 from preliz.internal.parser import inspect_source, parse_function_for_pred_sliders
 from preliz.internal.plot_helper import get_sliders, plot_decorator
 
 
 def predictive_sliders(fmodel, samples=50, kind_plot="kde"):
     """
     Create sliders and plot a set of samples returned by a function relating one or more
```

### Comparing `preliz-0.3.1/preliz/tests/check_inside_notebook.ipynb` & `preliz-0.3.2/preliz/tests/check_inside_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/tests/plot_interactive.ipynb` & `preliz-0.3.2/preliz/tests/plot_interactive.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/tests/predictive_sliders.ipynb` & `preliz-0.3.2/preliz/tests/predictive_sliders.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/tests/roulette.ipynb` & `preliz-0.3.2/preliz/tests/roulette.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/tests/test_distributions.py` & `preliz-0.3.2/preliz/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/tests/test_helper.py` & `preliz-0.3.2/preliz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/tests/test_maxent.py` & `preliz-0.3.2/preliz/tests/test_maxent.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/tests/test_mle.py` & `preliz-0.3.2/preliz/tests/test_mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/tests/test_plots.py` & `preliz-0.3.2/preliz/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/tests/test_quartile.py` & `preliz-0.3.2/preliz/tests/test_quartile.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/tests/test_roulette.py` & `preliz-0.3.2/preliz/tests/test_roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/unidimensional/maxent.py` & `preliz-0.3.2/preliz/unidimensional/maxent.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/unidimensional/mle.py` & `preliz-0.3.2/preliz/unidimensional/mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/preliz/unidimensional/quartile.py` & `preliz-0.3.2/preliz/unidimensional/quartile.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     opt = optimize_quartile(distribution, (q1, q2, q3), none_idx, fixed)
 
     r_error, _ = relative_error(distribution, q1, q3, 0.5)
 
     if r_error > 0.01:
         _log.info(
-            "The expected masses are 0.25, 0.5, 0.75\n" "The computed ones are: %.2g, %.2g, %.2g",
+            "The expected masses are 0.25, 0.5, 0.75\n The computed ones are: %.2g, %.2g, %.2g",
             *distribution.cdf([q1, q2, q3])
         )
 
     if plot:
         ax = distribution.plot_pdf(**plot_kwargs)
         if plot_kwargs.get("pointinterval"):
             cid = -4
```

### Comparing `preliz-0.3.1/preliz/unidimensional/roulette.py` & `preliz-0.3.2/preliz/unidimensional/roulette.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from math import ceil, floor
 
 
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import patches
 
-
-import ipywidgets as widgets
+try:
+    import ipywidgets as widgets
+except ImportError:
+    pass
 from ..internal.optimization import fit_to_ecdf, get_distributions
 from ..internal.plot_helper import check_inside_notebook
 
 
 def roulette(x_min=0, x_max=10, nrows=10, ncols=10, figsize=None):
     """
     Prior elicitation for 1D distribution using the roulette method.
```

### Comparing `preliz-0.3.1/pyproject.toml` & `preliz-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `preliz-0.3.1/PKG-INFO` & `preliz-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preliz
-Version: 0.3.1
+Version: 0.3.2
 Summary: The place for all your prior elicitation needs.
 Author-email: ArviZ team <arviz.devs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: Apache Software License
```

