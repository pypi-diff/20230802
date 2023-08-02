# Comparing `tmp/thztools-0.0.5.tar.gz` & `tmp/thztools-0.2.0.dev0.tar.gz`

## Comparing `thztools-0.0.5.tar` & `thztools-0.2.0.dev0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 thztools-0.0.5/.DS_Store
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 thztools-0.0.5/.gitattributes
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 thztools-0.0.5/simulation-example.ipynb
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/other.xml
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/thztools.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 thztools-0.0.5/.vscode/settings.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/coverage_html.js
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e___init___py.html
--rw-r--r--   0        0        0    46109 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e_common_py.html
--rw-r--r--   0        0        0    32102 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e_diff_tools_py.html
--rw-r--r--   0        0        0    87482 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e_messages_py.html
--rw-r--r--   0        0        0   139772 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e_pytest_plugin_py.html
--rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_36ede29a3be77d5b___init___py.html
--rw-r--r--   0        0        0    35110 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_36ede29a3be77d5b__util_py.html
--rw-r--r--   0        0        0   321235 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_36ede29a3be77d5b_thztools_py.html
--rw-r--r--   0        0        0    43443 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_8491cb1bc6f6c073_consistency_test_py.html
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_8491cb1bc6f6c073_test_pytest_py.html
--rw-r--r--   0        0        0    20570 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_e963af3fa267a6d4__jb_pytest_runner_py.html
--rw-r--r--   0        0        0   107696 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_e963af3fa267a6d4__jb_runner_tools_py.html
--rw-r--r--   0        0        0    34575 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_e963af3fa267a6d4__jb_serial_tree_manager_py.html
--rw-r--r--   0        0        0    42146 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_e963af3fa267a6d4__jb_utils_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/favicon_32.png
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/keybd_open.png
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/style.css
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 thztools-0.0.5/src/thztools/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 thztools-0.0.5/src/thztools/__about__.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 thztools-0.0.5/src/thztools/__init__.py
--rw-r--r--   0        0        0    18256 2020-02-02 00:00:00.000000 thztools-0.0.5/src/thztools/thztools.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 thztools-0.0.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.0.5/LICENSE
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 thztools-0.0.5/README.md
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 thztools-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 thztools-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.DS_Store
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.gitattributes
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/simulation-example.ipynb
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/modules.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/other.xml
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/thztools.iml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.vscode/settings.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/coverage_html.js
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e___init___py.html
+-rw-r--r--   0        0        0    46109 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_common_py.html
+-rw-r--r--   0        0        0    32102 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_diff_tools_py.html
+-rw-r--r--   0        0        0    87482 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_messages_py.html
+-rw-r--r--   0        0        0   139772 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_pytest_plugin_py.html
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_36ede29a3be77d5b___init___py.html
+-rw-r--r--   0        0        0    35110 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_36ede29a3be77d5b__util_py.html
+-rw-r--r--   0        0        0   321235 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_36ede29a3be77d5b_thztools_py.html
+-rw-r--r--   0        0        0    43443 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_8491cb1bc6f6c073_consistency_test_py.html
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_8491cb1bc6f6c073_test_pytest_py.html
+-rw-r--r--   0        0        0    20570 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_pytest_runner_py.html
+-rw-r--r--   0        0        0   107696 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_runner_tools_py.html
+-rw-r--r--   0        0        0    34575 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_serial_tree_manager_py.html
+-rw-r--r--   0        0        0    42146 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_utils_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/favicon_32.png
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/keybd_open.png
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/style.css
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/src/thztools/.DS_Store
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/src/thztools/__about__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/src/thztools/__init__.py
+-rw-r--r--   0        0        0    17989 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/src/thztools/thztools.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/LICENSE
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/README.md
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/PKG-INFO
```

### Comparing `thztools-0.0.5/simulation-example.ipynb` & `thztools-0.2.0.dev0/simulation-example.ipynb`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/.idea/thztools.iml` & `thztools-0.2.0.dev0/.idea/thztools.iml`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/.idea/inspectionProfiles/Project_Default.xml` & `thztools-0.2.0.dev0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/coverage_html.js` & `thztools-0.2.0.dev0/htmlReport/coverage_html.js`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e___init___py.html` & `thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e___init___py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e_common_py.html` & `thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_common_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e_diff_tools_py.html` & `thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_diff_tools_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e_messages_py.html` & `thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_messages_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e_pytest_plugin_py.html` & `thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_pytest_plugin_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_36ede29a3be77d5b___init___py.html` & `thztools-0.2.0.dev0/htmlReport/d_36ede29a3be77d5b___init___py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_36ede29a3be77d5b__util_py.html` & `thztools-0.2.0.dev0/htmlReport/d_36ede29a3be77d5b__util_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_36ede29a3be77d5b_thztools_py.html` & `thztools-0.2.0.dev0/htmlReport/d_36ede29a3be77d5b_thztools_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_8491cb1bc6f6c073_consistency_test_py.html` & `thztools-0.2.0.dev0/htmlReport/d_8491cb1bc6f6c073_consistency_test_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_8491cb1bc6f6c073_test_pytest_py.html` & `thztools-0.2.0.dev0/htmlReport/d_8491cb1bc6f6c073_test_pytest_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_e963af3fa267a6d4__jb_pytest_runner_py.html` & `thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_pytest_runner_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_e963af3fa267a6d4__jb_runner_tools_py.html` & `thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_runner_tools_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_e963af3fa267a6d4__jb_serial_tree_manager_py.html` & `thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_serial_tree_manager_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/d_e963af3fa267a6d4__jb_utils_py.html` & `thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_utils_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/favicon_32.png` & `thztools-0.2.0.dev0/htmlReport/favicon_32.png`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/index.html` & `thztools-0.2.0.dev0/htmlReport/index.html`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/keybd_closed.png` & `thztools-0.2.0.dev0/htmlReport/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/keybd_open.png` & `thztools-0.2.0.dev0/htmlReport/keybd_open.png`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/status.json` & `thztools-0.2.0.dev0/htmlReport/status.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/htmlReport/style.css` & `thztools-0.2.0.dev0/htmlReport/style.css`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/src/thztools/.DS_Store` & `thztools-0.2.0.dev0/src/thztools/.DS_Store`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/src/thztools/thztools.py` & `thztools-0.2.0.dev0/src/thztools/thztools.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,39 +4,15 @@
 
 import numpy as np
 import scipy.linalg as la
 from numpy.fft import irfft, rfft, rfftfreq
 from numpy.typing import ArrayLike
 from scipy.optimize import minimize
 
-
-def fftfreq(n, ts):
-    """Computes the positive and negative frequencies sampled in the FFT.
-
-    Parameters
-    ----------
-    n : int
-        Number of time samples
-    ts: float
-        Sampling time
-
-    Returns
-    -------
-    f : ndarray
-        Frequency vector (1/``ts``) of length n containing the sample
-        frequencies.
-    """
-
-    if n % 2 == 1:
-        f = np.fft.fftfreq(n, ts)
-    else:
-        f = np.fft.fftfreq(n, ts)
-        f[int(n / 2)] = -f[int(n / 2)]
-
-    return f
+NUM_NOISE_PARAMETERS = 3
 
 
 def noisevar(sigma: ArrayLike, mu: ArrayLike, ts: float) -> ArrayLike:
     r"""
     Compute the time-domain noise variance.
 
     Parameters
@@ -224,16 +200,16 @@
             raise ValueError(msg)
 
     f = rfftfreq(n, ts)
     w = 2 * np.pi * f
     phase = np.expand_dims(eta, axis=eta.ndim) * w
 
     xadj = np.fft.irfft(
-        np.fft.rfft(x) * np.exp(1j * phase), n=n
-    ) / np.expand_dims(a, axis=a.ndim)
+        np.fft.rfft(x) * np.exp(-1j * phase), n=n
+    ) * np.expand_dims(a, axis=a.ndim)
 
     if x.ndim > 1:
         if axis != -1:
             xadj = np.moveaxis(xadj, -1, axis)
 
     return xadj
 
@@ -544,15 +520,16 @@
     measurements of ``mu``.
 
     Parameters
     ----------
     x : ndarray
         Data array.
     v0 : ndarray, optional
-        Initial guess, noise model parameters with size (3,).
+        Initial guess, noise model parameters with size (3,), expressed as
+        variance amplitudes.
     mu0 : ndarray, optional
         Initial guess, signal vector with size (n,).
     a0 : ndarray, optional
         Initial guess, amplitude vector with size (m,).
     eta0 : ndarray, optional
         Initial guess, delay vector with size (m,).
     ts : float, optional
@@ -567,15 +544,15 @@
         Delay vector.
 
     Returns
     --------
     p : dict
         Output parameter dictionary containing:
             var : ndarray
-                Log of noise parameters
+                Noise parameters, expressed as variance amplitudes.
             mu : ndarray
                 Signal vector.
             a : ndarray
                 Amplitude vector.
             eta : ndarray
                 Delay vector.
     fval : float
@@ -600,16 +577,19 @@
     except ValueError:
         print("Data array x must be 2D.")
 
     if v0 is None:
         v0 = np.mean(np.var(x, 1)) * np.array([1, 1, 1])
     else:
         v0 = np.asarray(v0)
-        if v0.size != 3:
-            msg = "Noise parameter array logv must have 3 elements."
+        if v0.size != NUM_NOISE_PARAMETERS:
+            msg = (
+                "Noise parameter array logv must have "
+                f"{NUM_NOISE_PARAMETERS} elements."
+            )
             raise ValueError(msg)
 
     if mu0 is None:
         mu0 = np.mean(x, 1)
     else:
         mu0 = np.asarray(mu0)
         if mu0.size != n:
@@ -716,25 +696,26 @@
             "mu": np.array([]),
             "a": np.array([]),
             "eta": np.array([]),
         },
     }
     err = np.sqrt(np.diag(out.hess_inv))
     if not fix_v:
+        # Propagate error from log(V) to V
         diagnostic["err"]["var"] = np.sqrt(
-            np.diag(np.diag(p["var"]) * out.hess_inv[0:3, 0:3])
-            * np.diag(p["var"])
+            np.diag(np.diag(p["var"]) @ out.hess_inv[0:3, 0:3])
+            @ np.diag(p["var"])
         )
         err = err[3:]
 
     if not fix_mu:
         diagnostic["err"]["mu"] = err[:n]
         err = err[n:]
 
     if not fix_a:
         diagnostic["err"]["a"] = np.concatenate(([0], err[: m - 1]))
         err = err[m - 1 :]
 
     if not fix_eta:
         diagnostic["err"]["eta"] = np.concatenate(([0], err[: m - 1]))
 
-    return [p, out.fun, diagnostic]
+    return p, out.fun, diagnostic
```

### Comparing `thztools-0.0.5/.gitignore` & `thztools-0.2.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/LICENSE` & `thztools-0.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/README.md` & `thztools-0.2.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/pyproject.toml` & `thztools-0.2.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thztools-0.0.5/PKG-INFO` & `thztools-0.2.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: THzTools
-Version: 0.0.5
+Version: 0.2.0.dev0
 Summary: Tools for terahertz time-domain spectroscopy (THz-TDS)
 Project-URL: Documentation, https://dodge-research-group.github.io/thztools/
 Project-URL: Issues, https://github.com/dodge-research-group/thztools/issues
 Project-URL: Source, https://github.com/dodge-research-group/thztools
 Author-email: Steve Dodge <jsdodge@sfu.ca>, Santiago Higuera Quintero <s.higuera@uniandes.edu.co>, Jonathan Posada <jonathan.posada1@udea.edu.co>
 Maintainer-email: Steve Dodge <jsdodge@sfu.ca>
 License-Expression: MIT
```

