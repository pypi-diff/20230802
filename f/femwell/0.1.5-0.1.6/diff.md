# Comparing `tmp/femwell-0.1.5.tar.gz` & `tmp/femwell-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femwell-0.1.5.tar", max compression
+gzip compressed data, was "femwell-0.1.6.tar", max compression
```

## Comparing `femwell-0.1.5.tar` & `femwell-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-07-20 21:59:40.301303 femwell-0.1.5/LICENSE
--rw-r--r--   0        0        0     2480 2023-07-20 21:59:40.301303 femwell-0.1.5/README.md
--rw-r--r--   0        0        0      255 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/__init__.py
--rw-r--r--   0        0        0     3080 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/culomb.py
--rw-r--r--   0        0        0    10175 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/eme.py.bak
--rw-r--r--   0        0        0        0 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/examples/__init__.py
--rw-r--r--   0        0        0     4820 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/examples/coplanar_waveguide.py
--rw-r--r--   0        0        0     5762 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/fefd.py
--rw-r--r--   0        0        0     3173 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/fefd_2d.py
--rw-r--r--   0        0        0     1304 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/fiber.py
--rw-r--r--   0        0        0     1782 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/laplace.py
--rw-r--r--   0        0        0    20309 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/maxwell/waveguide.py
--rw-r--r--   0        0        0      224 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mesh/__init__.py
--rw-r--r--   0        0        0    26893 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mesh/mesh.py
--rw-r--r--   0        0        0     7900 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mesh/meshtracker.py
--rw-r--r--   0        0        0     9318 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mesh/slice.py
--rw-r--r--   0        0        0    21359 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mesh.py
--rw-r--r--   0        0        0     1033 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mode_solver_1d.py
--rw-r--r--   0        0        0     2922 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mode_solver_2d_periodic.py
--rw-r--r--   0        0        0     6950 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mode_solver_2d_periodic_quadratic.py
--rw-r--r--   0        0        0     4224 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mode_solver_inplane.py
--rw-r--r--   0        0        0     1243 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/mode_solver_schrodinger.py
--rw-r--r--   0        0        0     8799 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/pn_analytical.py
--rw-r--r--   0        0        0     6453 2023-07-20 21:59:40.305303 femwell-0.1.5/femwell/solver.py
--rw-r--r--   0        0        0     5897 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/tcad.py
--rw-r--r--   0        0        0     2820 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/tests/test_mesh.py
--rw-r--r--   0        0        0     5880 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/thermal.py
--rw-r--r--   0        0        0     8803 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/thermal_transient.py
--rw-r--r--   0        0        0     2655 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/utils.py
--rw-r--r--   0        0        0     1123 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/visualization.py
--rw-r--r--   0        0        0     2089 2023-07-20 21:59:40.309303 femwell-0.1.5/femwell/waveguide.py
--rw-r--r--   0        0        0      974 2023-07-20 21:59:53.825421 femwell-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 femwell-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-02 20:15:24.370494 femwell-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2480 2023-08-02 20:15:24.370494 femwell-0.1.6/README.md
+-rw-r--r--   0        0        0      255 2023-08-02 20:15:24.370494 femwell-0.1.6/femwell/__init__.py
+-rw-r--r--   0        0        0     3080 2023-08-02 20:15:24.370494 femwell-0.1.6/femwell/culomb.py
+-rw-r--r--   0        0        0    10175 2023-08-02 20:15:24.370494 femwell-0.1.6/femwell/eme.py.bak
+-rw-r--r--   0        0        0        0 2023-08-02 20:15:24.370494 femwell-0.1.6/femwell/examples/__init__.py
+-rw-r--r--   0        0        0     4820 2023-08-02 20:15:24.370494 femwell-0.1.6/femwell/examples/coplanar_waveguide.py
+-rw-r--r--   0        0        0     5763 2023-08-02 20:15:24.370494 femwell-0.1.6/femwell/fefd.py
+-rw-r--r--   0        0        0     3172 2023-08-02 20:15:24.370494 femwell-0.1.6/femwell/fefd_2d.py
+-rw-r--r--   0        0        0     1304 2023-08-02 20:15:24.370494 femwell-0.1.6/femwell/fiber.py
+-rw-r--r--   0        0        0     1782 2023-08-02 20:15:24.370494 femwell-0.1.6/femwell/laplace.py
+-rw-r--r--   0        0        0    20309 2023-08-02 20:15:24.370494 femwell-0.1.6/femwell/maxwell/waveguide.py
+-rw-r--r--   0        0        0      224 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/mesh/__init__.py
+-rw-r--r--   0        0        0    26893 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/mesh/mesh.py
+-rw-r--r--   0        0        0     7900 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/mesh/meshtracker.py
+-rw-r--r--   0        0        0     9318 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/mesh/slice.py
+-rw-r--r--   0        0        0    21359 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/mesh.py
+-rw-r--r--   0        0        0     1033 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/mode_solver_1d.py
+-rw-r--r--   0        0        0     2922 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/mode_solver_2d_periodic.py
+-rw-r--r--   0        0        0     6950 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/mode_solver_2d_periodic_quadratic.py
+-rw-r--r--   0        0        0     4225 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/mode_solver_inplane.py
+-rw-r--r--   0        0        0     1243 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/mode_solver_schrodinger.py
+-rw-r--r--   0        0        0     8799 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/pn_analytical.py
+-rw-r--r--   0        0        0     6453 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/solver.py
+-rw-r--r--   0        0        0     5897 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/tcad.py
+-rw-r--r--   0        0        0     2820 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/tests/test_mesh.py
+-rw-r--r--   0        0        0     5880 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/thermal.py
+-rw-r--r--   0        0        0     8803 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/thermal_transient.py
+-rw-r--r--   0        0        0     2655 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/utils.py
+-rw-r--r--   0        0        0     1123 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/visualization.py
+-rw-r--r--   0        0        0     2089 2023-08-02 20:15:24.374493 femwell-0.1.6/femwell/waveguide.py
+-rw-r--r--   0        0        0     1844 2023-08-02 20:15:35.870523 femwell-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 femwell-0.1.6/PKG-INFO
```

### Comparing `femwell-0.1.5/LICENSE` & `femwell-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/README.md` & `femwell-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/culomb.py` & `femwell-0.1.6/femwell/culomb.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/eme.py.bak` & `femwell-0.1.6/femwell/eme.py.bak`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/examples/coplanar_waveguide.py` & `femwell-0.1.6/femwell/examples/coplanar_waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/fefd.py` & `femwell-0.1.6/femwell/fefd.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     A = lhs.assemble(basis_source_1d, epsilon=basis0_source.interpolate(epsilon))
     B = rhs.assemble(basis_source_1d)
 
     from skfem.utils import solver_eigen_scipy_sym
 
     lams, xs = solve(
         *condense(A, B, I=basis_source_1d.get_dofs(facets="source")),
-        solver=solver_eigen_scipy_sym(sigma=3.55**2, which="LM")
+        solver=solver_eigen_scipy_sym(sigma=3.55**2, which="LM"),
     )
 
     # xs[:,0] = xs[:,0]*0+1
     x0 = basis_source.project(
         (
             np.array(
                 (
```

### Comparing `femwell-0.1.5/femwell/fefd_2d.py` & `femwell-0.1.6/femwell/fefd_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,38 +27,38 @@
 epsilon_r = basis0.zeros(dtype=complex) + 1
 dofs = basis0.get_dofs(elements="waveguide2")  # *(x[1]>.5))
 epsilon_r[dofs] = 1.5**2
 basis0.plot(epsilon_r.real).show()
 # dofs = basis0.get_dofs(elements=lambda x: (x[0] > 6))  # *(x[1]>.5))
 # epsilon_r[dofs] = 1**2
 dofs = basis0.get_dofs(elements=lambda x: x[0] > 7)
-epsilon_r[dofs] += basis0.project(lambda x: np.maximum(0, x[0] - 7) ** 2 * 0.007j, dtype=complex)[
+epsilon_r[dofs] += basis0.project(lambda x: np.maximum(0, x[0] - 7) ** 2 * 0.07j, dtype=complex)[
     dofs
 ]
 basis0.plot(epsilon_r.imag, shading="gouraud", colorbar=True)
 plt.show()
 input_basis = basis.boundary(lambda x: x[0] == np.min(x[0]))
 line1_basis = basis.boundary("line1")
 line2_basis = basis.boundary("line2")
 
 mu_r = 1
-k0 = 6
+k0 = 4
 
 
 def h_m(y, b, m):
     return np.sqrt((1 if m == 0 else 2) / b) * np.sin(m * np.pi * y / b)
 
 
 def gamma_m(b, m):
     return np.sqrt((m * np.pi / b) ** 2 - k0**2, dtype=complex)
 
 
 @BilinearForm(dtype=complex)
 def maxwell(u, v, w):
-    return 0.5 * (1 / w.epsilon_r * inner(grad(u), grad(v))) - k0**2 * inner(u, v)
+    return 0.5 * (1 / w.epsilon_r * inner(grad(u), grad(v)) - k0**2 * inner(u, v))
 
 
 @BilinearForm(dtype=complex)
 def input_form(u, v, w):
     return 0.5 * inner(
         u,
         np.sum([h_m(w.x[1], 1, m) * gamma_m(1, m) * inner(h_m(w.x[1], 1, m), v) for m in range(3)]),
```

### Comparing `femwell-0.1.5/femwell/fiber.py` & `femwell-0.1.6/femwell/fiber.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/laplace.py` & `femwell-0.1.6/femwell/laplace.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/maxwell/waveguide.py` & `femwell-0.1.6/femwell/maxwell/waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/mesh/mesh.py` & `femwell-0.1.6/femwell/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/mesh/meshtracker.py` & `femwell-0.1.6/femwell/mesh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/mesh/slice.py` & `femwell-0.1.6/femwell/mesh/slice.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/mesh.py` & `femwell-0.1.6/femwell/mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/mode_solver_1d.py` & `femwell-0.1.6/femwell/mode_solver_1d.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/mode_solver_2d_periodic.py` & `femwell-0.1.6/femwell/mode_solver_2d_periodic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/mode_solver_2d_periodic_quadratic.py` & `femwell-0.1.6/femwell/mode_solver_2d_periodic_quadratic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/mode_solver_inplane.py` & `femwell-0.1.6/femwell/mode_solver_inplane.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         FacetBasis(basis.mesh, basis.elem, facets="top"),
         FacetBasis(basis.mesh, basis.elem, facets="bottom"),
     ]
     D2 = asm(penalty, fbases, fbases, phase=1)
 
     lams, xs = solve(
         *condense(A + D1, B, D=basis.get_dofs(["top", "bottom"]), x=basis.zeros(dtype=complex)),
-        solver=solver_slepc(k=num_modes, which="LR", sigma=10)
+        solver=solver_slepc(k=num_modes, which="LR", sigma=10),
     )
 
     return np.sqrt(lams), basis, xs
 
 
 if __name__ == "__main__":
     from collections import OrderedDict
```

### Comparing `femwell-0.1.5/femwell/mode_solver_schrodinger.py` & `femwell-0.1.6/femwell/mode_solver_schrodinger.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/pn_analytical.py` & `femwell-0.1.6/femwell/pn_analytical.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/solver.py` & `femwell-0.1.6/femwell/solver.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/tcad.py` & `femwell-0.1.6/femwell/tcad.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/tests/test_mesh.py` & `femwell-0.1.6/femwell/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/thermal.py` & `femwell-0.1.6/femwell/thermal.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/thermal_transient.py` & `femwell-0.1.6/femwell/thermal_transient.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/utils.py` & `femwell-0.1.6/femwell/utils.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/visualization.py` & `femwell-0.1.6/femwell/visualization.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/femwell/waveguide.py` & `femwell-0.1.6/femwell/waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.5/pyproject.toml` & `femwell-0.1.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,50 @@
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "femwell"
+version = "0.0.1"
+authors = [
+    {name = "Helge Gehring"},
+]
+description = "Mode solver for photonic and electric waveguides based on FEM"
+keywords = [
+    "integrated photonics",
+    "silicon photonics",
+    "mode solving",
+    "finite element analysis"
+]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Science/Research",
+    "Programming Language :: Python :: 3",
+    "Topic :: Scientific/Engineering"
+]
+license = {file = "LICENSE"}
+readme = "README.md"
+
+requires-python = ">=3.8"
+
+dependencies = [
+    "scikit-fem>=8.1.0",
+    "gmsh",
+    "pygmsh",
+    "matplotlib",
+    "shapely>=2.0.0"
+]
+
+[project.urls]
+Homepage = "https://github.com/HelgeGehring/femwell"
+Documentation = "https://HelgeGehring.github.io/femwell/"
+
 [tool.poetry]
 name = "femwell"
-version = "0.1.5"
+version = "0.1.6"
 authors = ["Helge Gehring"]
 description = "Mode solver for photonic and electric waveguides based on FEM"
 homepage = "https://github.com/HelgeGehring/femwell"
 keywords = [
     "integrated photonics",
     "silicon photonics",
     "mode solving",
```

### Comparing `femwell-0.1.5/PKG-INFO` & `femwell-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femwell
-Version: 0.1.5
+Version: 0.1.6
 Summary: Mode solver for photonic and electric waveguides based on FEM
 Home-page: https://github.com/HelgeGehring/femwell
 License: GPLv3
 Keywords: integrated photonics,silicon photonics,mode solving,finite element analysis
 Author: Helge Gehring
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
```

