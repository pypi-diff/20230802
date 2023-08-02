# Comparing `tmp/PythonicDISORT-0.2.0.tar.gz` & `tmp/PythonicDISORT-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonicDISORT-0.2.0.tar", last modified: Sun Jun 11 09:10:28 2023, max compression
+gzip compressed data, was "PythonicDISORT-0.2.1.tar", last modified: Wed Aug  2 17:41:57 2023, max compression
```

## Comparing `PythonicDISORT-0.2.0.tar` & `PythonicDISORT-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:10:28.626991 PythonicDISORT-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-11 09:10:28.626991 PythonicDISORT-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-11 09:10:01.000000 PythonicDISORT-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-11 09:10:02.000000 PythonicDISORT-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 09:10:28.626991 PythonicDISORT-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:10:28.622991 PythonicDISORT-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:10:28.622991 PythonicDISORT-0.2.0/src/PythonicDISORT/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-11 09:10:02.000000 PythonicDISORT-0.2.0/src/PythonicDISORT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13382 2023-06-11 09:10:02.000000 PythonicDISORT-0.2.0/src/PythonicDISORT/_loop_and_assemble_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-06-11 09:10:02.000000 PythonicDISORT-0.2.0/src/PythonicDISORT/_one_Fourier_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-06-11 09:10:02.000000 PythonicDISORT-0.2.0/src/PythonicDISORT/pydisort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-11 09:10:02.000000 PythonicDISORT-0.2.0/src/PythonicDISORT/subroutines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:10:28.622991 PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-11 09:10:28.000000 PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-11 09:10:28.000000 PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 09:10:28.000000 PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-11 09:10:28.000000 PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-11 09:10:28.000000 PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:41:57.075048 PythonicDISORT-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-08-02 17:41:57.075048 PythonicDISORT-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-08-02 17:41:39.000000 PythonicDISORT-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-02 17:41:40.000000 PythonicDISORT-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:41:57.075048 PythonicDISORT-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:41:57.075048 PythonicDISORT-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:41:57.075048 PythonicDISORT-0.2.1/src/PythonicDISORT/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 17:41:40.000000 PythonicDISORT-0.2.1/src/PythonicDISORT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15679 2023-08-02 17:41:40.000000 PythonicDISORT-0.2.1/src/PythonicDISORT/_loop_and_assemble_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-08-02 17:41:40.000000 PythonicDISORT-0.2.1/src/PythonicDISORT/_one_Fourier_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20916 2023-08-02 17:41:40.000000 PythonicDISORT-0.2.1/src/PythonicDISORT/pydisort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-08-02 17:41:40.000000 PythonicDISORT-0.2.1/src/PythonicDISORT/subroutines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:41:57.075048 PythonicDISORT-0.2.1/src/PythonicDISORT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-08-02 17:41:57.000000 PythonicDISORT-0.2.1/src/PythonicDISORT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 17:41:57.000000 PythonicDISORT-0.2.1/src/PythonicDISORT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:41:57.000000 PythonicDISORT-0.2.1/src/PythonicDISORT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-02 17:41:57.000000 PythonicDISORT-0.2.1/src/PythonicDISORT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 17:41:57.000000 PythonicDISORT-0.2.1/src/PythonicDISORT.egg-info/top_level.txt
```

### Comparing `PythonicDISORT-0.2.0/PKG-INFO` & `PythonicDISORT-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonicDISORT
-Version: 0.2.0
+Version: 0.2.1
 Summary: Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 Author-email: Dion HO Jia Xu <dh3065@columbia.edu>
 Project-URL: Homepage, https://github.com/LDEO-CREW/PythonicDISORT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `PythonicDISORT-0.2.0/README.md` & `PythonicDISORT-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `PythonicDISORT-0.2.0/pyproject.toml` & `PythonicDISORT-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 dependencies = [
   "numpy>=1.17.3",
   "scipy>=1.8.0",
 ]
 name = "PythonicDISORT"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Dion HO Jia Xu", email="dh3065@columbia.edu" },
 ]
 description = "Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PythonicDISORT-0.2.0/src/PythonicDISORT/_loop_and_assemble_results.py` & `PythonicDISORT-0.2.1/src/PythonicDISORT/_loop_and_assemble_results.py`

 * *Files 9% similar despite different names*

```diff
@@ -138,14 +138,16 @@
         # --------------------------------------------------------------------------------------------------------------------------
         
         # Construct the intensity function
         # --------------------------------------------------------------------------------------------------------------------------
         def u(tau, phi, return_Fourier_error=False):
             tau = np.atleast_1d(tau)
             phi = np.atleast_1d(phi)
+            assert np.all(tau >= 0)
+            assert np.all(tau <= tau_arr[-1])
             
             # Atmospheric layer indices
             l = np.argmax(tau[:, None] <= tau_arr[None, :], axis=1)
             scaled_tau_arr_l = scaled_tau_arr_with_0[l + 1]
             scaled_tau_arr_lm1 = scaled_tau_arr_with_0[l]
 
             # Delta-M scaling
@@ -218,25 +220,79 @@
                     )
                 )
                 return intensities, Fourier_error
             else:
                 return intensities
         # --------------------------------------------------------------------------------------------------------------------------
     
+    # Construct u0
+    # --------------------------------------------------------------------------------------------------------------------------
+    def u0(tau):
+        tau = np.atleast_1d(tau)
+        assert np.all(tau >= 0)
+        assert np.all(tau <= tau_arr[-1])
+        
+        # Atmospheric layer indices
+        l = np.argmax(tau[:, None] <= tau_arr[None, :], axis=1)
+        scaled_tau_arr_l = scaled_tau_arr_with_0[l + 1]
+        scaled_tau_arr_lm1 = scaled_tau_arr_with_0[l]
+
+        # Delta-M scaling
+        if np.any(scale_tau != np.ones(NLayers)):
+            tau_dist_from_top = tau_arr[l] - tau
+            scaled_tau_dist_from_top = tau_dist_from_top * scale_tau[l]
+            scaled_tau = scaled_tau_arr_l - scaled_tau_dist_from_top
+        else:
+            scaled_tau = tau
+
+        exponent = np.concatenate(
+            [
+                K_collect_0[l, :N] * (scaled_tau - scaled_tau_arr_lm1)[:, None],
+                K_collect_0[l, N:] * (scaled_tau - scaled_tau_arr_l)[:, None],
+            ],
+            axis=-1,
+        )
+        if I0 > 0:
+            u0 = np.einsum(
+                "tij, tj -> it", GC_collect_0[l, :, :], np.exp(exponent), optimize=True
+            ) + B_collect_0[l, :].T * np.exp(-scaled_tau[None, :] / mu0)
+        else:
+            u0 = np.einsum(
+                "tij, tj -> it", GC_collect_0[l, :, :], np.exp(exponent), optimize=True
+            )
+        
+        # Contribution from particular solution for isotropic internal sources
+        if Nscoeffs > 0:
+            _mathscr_v_contribution = _mathscr_v(
+                tau, l,
+                s_poly_coeffs,
+                Nscoeffs,
+                G_collect_0,
+                K_collect_0,
+                G_inv_collect_0,
+                mu_arr,
+            )
+            u0 += _mathscr_v_contribution
+            
+        return np.squeeze(u0)
+    # --------------------------------------------------------------------------------------------------------------------------
+    
     # Construct the flux functions
     # --------------------------------------------------------------------------------------------------------------------------
     GC_pos = GC_collect_0[:, :N, :]
     GC_neg = GC_collect_0[:, N:, :]
     if I0 > 0:
         B_pos = B_collect_0[:, :N].T
         B_neg = B_collect_0[:, N:].T
 
 
     def flux_up(tau):
         tau = np.atleast_1d(tau)
+        assert np.all(tau >= 0)
+        assert np.all(tau <= tau_arr[-1])
         
         # Atmospheric layer indices
         l = np.argmax(tau[:, None] <= tau_arr[None, :], axis=1)
         scaled_tau_arr_l = scaled_tau_arr_with_0[l + 1]
         scaled_tau_arr_lm1 = scaled_tau_arr_with_0[l]
 
         # Delta-M scaling
@@ -279,14 +335,16 @@
         )
                   
         return np.squeeze(2 * pi * (mu_arr_pos * W) @ u0_pos)[()]
 
 
     def flux_down(tau):
         tau = np.atleast_1d(tau)
+        assert np.all(tau >= 0)
+        assert np.all(tau <= tau_arr[-1])
 
         # Atmospheric layer indices
         l = np.argmax(tau[:, None] <= tau_arr[None, :], axis=1)
         scaled_tau_arr_l = scaled_tau_arr_with_0[l + 1]
         scaled_tau_arr_lm1 = scaled_tau_arr_with_0[l]
 
         # Delta-M scaling
@@ -339,10 +397,10 @@
                 - direct_beam
             )[()],
             np.squeeze(direct_beam)[()],
         )
         # --------------------------------------------------------------------------------------------------------------------------
 
     if only_flux:
-        return flux_up, flux_down
+        return flux_up, flux_down, u0
     else:
-        return flux_up, flux_down, u
+        return flux_up, flux_down, u0, u
```

### Comparing `PythonicDISORT-0.2.0/src/PythonicDISORT/_one_Fourier_mode.py` & `PythonicDISORT-0.2.1/src/PythonicDISORT/_one_Fourier_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from PythonicDISORT.subroutines import _mathscr_v
 import numpy as np
 import scipy as sc
+from warnings import warn
 from math import pi
 
 
 def _one_Fourier_mode(
     m,
     scaled_omega_arr,
     tau_arr,
@@ -41,14 +42,15 @@
     asso_leg_term_neg = asso_leg_term_pos * signs[:, None]
     asso_leg_term_mu0 = sc.special.lpmv(m, ells, -mu0)
     # --------------------------------------------------------------------------------------------------------------------------
     
     # Generate mathscr_D and mathscr_X (BDRF terms)
     # --------------------------------------------------------------------------------------------------------------------------
     # If h_\ell = 0 for all \ell \geq m, then there is no BDRF contribution
+    # We take precautions against overflow and underflow
     if m < NBDRF and np.all(np.isfinite(asso_leg_term_pos[:NBDRF, :])):
         weighted_asso_Leg_coeffs_BDRF = (
             weighted_Leg_coeffs_BDRF[ells[: (NBDRF - m)]] * fac[: (NBDRF - m)]
         )
         mathscr_D_temp = (
             weighted_asso_Leg_coeffs_BDRF[None, :] * asso_leg_term_pos.T[:, :NBDRF]
         )
@@ -74,14 +76,15 @@
         B_collect_m = np.zeros((NLayers, NQuad))
 
     for l in range(NLayers):
         # More setup
         weighted_asso_Leg_coeffs_l = weighted_scaled_Leg_coeffs[l, :][ells] * fac
         scaled_omega_l = scaled_omega_arr[l]
         
+        # We take precautions against overflow and underflow
         if np.any(weighted_asso_Leg_coeffs_l > 0) and np.all(
             np.isfinite(asso_leg_term_pos)
         ):
             # Generate mathscr_D and mathscr_X (BDRF terms)
             # --------------------------------------------------------------------------------------------------------------------------
             D_temp = weighted_asso_Leg_coeffs_l[None, :] * asso_leg_term_pos.T
             D_pos = (scaled_omega_l / 2) * D_temp @ asso_leg_term_pos
@@ -105,14 +108,21 @@
             if I0 > 0:
                 X_tilde = np.concatenate([-M_inv * X_pos, M_inv * X_neg])
             # --------------------------------------------------------------------------------------------------------------------------
 
             # Diagonalization of coefficient matrix
             # --------------------------------------------------------------------------------------------------------------------------
             K_squared, eigenvecs_GpG = np.linalg.eig((alpha - beta) @ (alpha + beta))
+            if m == 0:
+                if np.any(np.isclose(K_squared, 0)):
+                    warn(
+                        "Single-scattering albedo for layer "
+                        + str(l)
+                        + " (counting from 0) is too close to 1. Results may be inaccurate."
+                    )
 
             # Eigenvalues arranged negative then positive, from largest to smallest magnitude
             K = np.concatenate([-np.sqrt(K_squared), np.sqrt(K_squared)])
             eigenvecs_GpG = np.hstack([eigenvecs_GpG, eigenvecs_GpG])
             eigenvecs_GmG = (alpha + beta) @ eigenvecs_GpG / K
 
             # Eigenvector matrix
```

### Comparing `PythonicDISORT-0.2.0/src/PythonicDISORT/pydisort.py` & `PythonicDISORT-0.2.1/src/PythonicDISORT/pydisort.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,19 @@
         All mu (cosine of polar angle) quadrature nodes.
     function
         Flux function with argument tau (type: array) for positive (upward) mu values.
         Returns the diffuse flux magnitudes (type: array).
     function
         Flux function with argument tau (type: array)  for negative (downward) mu values.
         Returns a tuple of the diffuse and direct flux magnitudes respectively (type: (array, array)).
+    function
+        Zeroth Fourier mode of the intensity with argument tau (type: array).
+        Returns an ndarray with axes corresponding to (mu, tau) variation.
+        This function is useful for calculating actinic flux and other quantities of interest
+        but reclassification of delta-scaled flux and other corrections must be done manually.
     function, optional
         Intensity function with arguments (tau, phi, return_Fourier_error=False) of types (array, array, bool).
         Returns an ndarray with axes corresponding to (mu, tau, phi) variation.
         The optional flag `return_Fourier_error` determines whether the function will also return
         the Cauchy / Fourier convergence evaluation (type: float) for the last Fourier term.
 
     """
@@ -114,27 +119,29 @@
     if NLoops is None:
         NLoops = NQuad
     scalar_b_pos = False
     scalar_b_neg = False
     thickness_arr = np.concatenate([[tau_arr[0]], np.diff(tau_arr)])
     Nscoeffs = np.shape(s_poly_coeffs)[1]
     NLeg_all = np.shape(Leg_coeffs_all)[1]
+    N = NQuad // 2
     # --------------------------------------------------------------------------------------------------------------------------
 
     # Input checks
     # --------------------------------------------------------------------------------------------------------------------------
     # Optical depths and thickness must be positive
     assert np.all(tau_arr > 0)
     assert np.all(thickness_arr > 0)
     # Single-scattering albedo must be between 0 and 1, excluding 1
     assert np.all(omega_arr >= 0)
     assert np.all(omega_arr < 1)
     # There must be a positive number of Legendre coefficients each with magnitude <= 1
     # The user must supply at least as many phase function Legendre coefficients as intended for use
     assert NLeg > 0
+    assert np.all(Leg_coeffs_all[:, 0] == 1)
     assert np.all(np.abs(Leg_coeffs_all) <= 1)
     assert np.all(np.abs(Leg_coeffs_BDRF) <= 1)
     assert NLeg <= NLeg_all
     # Ensure that the first dimension of the following inputs corresponds to the number of layers
     assert np.shape(Leg_coeffs_all)[0] == NLayers
     assert len(omega_arr) == NLayers
     if len(f_arr) != 1 or f_arr[0] != 0:
@@ -144,15 +151,14 @@
     # Conditions on the number of quadrature angles (NQuad), Legendre coefficients (NLeg) and loops (NLoops)
     assert NQuad >= 2
     assert NQuad % 2 == 0
     assert NLoops > 0
     assert NLoops <= NLeg
     # Not strictly necessary but there will be tremendous inaccuracies if this is violated
     assert NQuad >= NLeg
-    N = NQuad // 2
     # We require principal angles and a downward incident beam
     assert I0 >= 0
     if I0 > 0:
         assert 0 < mu0 and mu0 <= 1
         assert 0 <= phi0 and phi0 < 2 * pi
     # Ensure that the BC inputs are of the correct shape
     if len(np.atleast_1d(b_pos)) == 1:
@@ -209,15 +215,15 @@
     # --------------------------------------------------------------------------------------------------------------------------
     
     if NT_cor and not only_flux and I0 > 0 and np.any(f_arr > 0) and NLeg < NLeg_all:
         
         ############################### Perform NT corrections on the intensity but not the flux ###################################
         
         # Delta-M scaled solution; no further corrections to the flux
-        flux_up, flux_down, u_star = _loop_and_assemble_results(
+        flux_up, flux_down, u0, u_star = _loop_and_assemble_results(
             scaled_omega_arr,
             tau_arr,
             scaled_tau_arr_with_0,
             mu_arr_pos, mu_arr,
             M_inv, W,
             N, NQuad, NLeg, NLoops,
             NLayers, NBDRF,
@@ -416,15 +422,15 @@
                     u_star_outputs[0] + np.squeeze(NT_corrections),
                     u_star_outputs[1],
                 )
             else:
                 return u_star(tau, phi, False) + np.squeeze(NT_corrections)
         # --------------------------------------------------------------------------------------------------------------------------
 
-        return mu_arr, flux_up, flux_down, u_corrected
+        return mu_arr, flux_up, flux_down, u0, u_corrected
         
     else:
         return (mu_arr,) + _loop_and_assemble_results(
             scaled_omega_arr,
             tau_arr,
             scaled_tau_arr_with_0,
             mu_arr_pos, mu_arr,
```

### Comparing `PythonicDISORT-0.2.0/src/PythonicDISORT/subroutines.py` & `PythonicDISORT-0.2.1/src/PythonicDISORT/subroutines.py`

 * *Files identical despite different names*

### Comparing `PythonicDISORT-0.2.0/src/PythonicDISORT.egg-info/PKG-INFO` & `PythonicDISORT-0.2.1/src/PythonicDISORT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonicDISORT
-Version: 0.2.0
+Version: 0.2.1
 Summary: Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 Author-email: Dion HO Jia Xu <dh3065@columbia.edu>
 Project-URL: Homepage, https://github.com/LDEO-CREW/PythonicDISORT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

