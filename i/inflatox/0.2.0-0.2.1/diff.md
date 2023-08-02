# Comparing `tmp/inflatox-0.2.0-cp37-abi3-win_amd64.whl.zip` & `tmp/inflatox-0.2.1-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 344796 bytes, number of entries: 11
--rw-r--r--  4.6 unx     5170 b- defN 23-Jul-21 17:38 inflatox-0.2.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jul-21 17:38 inflatox-0.2.0.dist-info/WHEEL
--rw-r--r--  4.6 unx    14114 b- defN 23-Jul-21 17:38 inflatox-0.2.0.dist-info/license_files/LICENSE-EN.txt
--rw-r--r--  4.6 unx   377429 b- defN 23-Jul-21 17:38 inflatox-0.2.0.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx    11416 b- defN 23-Jul-21 17:38 inflatox/compiler.py
--rw-r--r--  4.6 unx     8656 b- defN 23-Jul-21 17:38 inflatox/consistency_conditions.py
--rw-r--r--  4.6 unx    20784 b- defN 23-Jul-21 17:38 inflatox/symbolic.py
--rw-r--r--  4.6 unx      908 b- defN 23-Jul-21 17:38 inflatox/version.py
--rw-r--r--  4.6 unx     1189 b- defN 23-Jul-21 17:38 inflatox/__init__.py
--rwxr-xr-x  4.6 unx   495616 b- defN 23-Jul-21 17:38 inflatox/libinflx_rs.pyd
--rw-r--r--  4.6 unx      910 b- defN 23-Jul-21 17:38 inflatox-0.2.0.dist-info/RECORD
-11 files, 936286 bytes uncompressed, 343272 bytes compressed:  63.3%
+Zip file size: 344785 bytes, number of entries: 11
+-rw-r--r--  4.6 unx     5170 b- defN 23-Aug-02 16:22 inflatox-0.2.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Aug-02 16:22 inflatox-0.2.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx    14114 b- defN 23-Aug-02 16:22 inflatox-0.2.1.dist-info/license_files/LICENSE-EN.txt
+-rw-r--r--  4.6 unx   377429 b- defN 23-Aug-02 16:22 inflatox-0.2.1.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx    11416 b- defN 23-Aug-02 16:22 inflatox/compiler.py
+-rw-r--r--  4.6 unx     8612 b- defN 23-Aug-02 16:22 inflatox/consistency_conditions.py
+-rw-r--r--  4.6 unx    20784 b- defN 23-Aug-02 16:22 inflatox/symbolic.py
+-rw-r--r--  4.6 unx      908 b- defN 23-Aug-02 16:22 inflatox/version.py
+-rw-r--r--  4.6 unx     1189 b- defN 23-Aug-02 16:22 inflatox/__init__.py
+-rwxr-xr-x  4.6 unx   495616 b- defN 23-Aug-02 16:22 inflatox/libinflx_rs.pyd
+-rw-r--r--  4.6 unx      910 b- defN 23-Aug-02 16:22 inflatox-0.2.1.dist-info/RECORD
+11 files, 936242 bytes uncompressed, 343261 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,17 +1,17 @@
-Filename: inflatox-0.2.0.dist-info/METADATA
+Filename: inflatox-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: inflatox-0.2.0.dist-info/WHEEL
+Filename: inflatox-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: inflatox-0.2.0.dist-info/license_files/LICENSE-EN.txt
+Filename: inflatox-0.2.1.dist-info/license_files/LICENSE-EN.txt
 Comment: 
 
-Filename: inflatox-0.2.0.dist-info/license_files/LICENSE.md
+Filename: inflatox-0.2.1.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: inflatox/compiler.py
 Comment: 
 
 Filename: inflatox/consistency_conditions.py
 Comment: 
@@ -24,11 +24,11 @@
 
 Filename: inflatox/__init__.py
 Comment: 
 
 Filename: inflatox/libinflx_rs.pyd
 Comment: 
 
-Filename: inflatox-0.2.0.dist-info/RECORD
+Filename: inflatox-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inflatox/consistency_conditions.py

```diff
@@ -35,71 +35,71 @@
   into the Rust API or C ABI.
   """
 
   def __init__(self, compiled_artifact: CompilationArtifact):
     self.artifact = compiled_artifact
     self.dylib = open_inflx_dylib(compiled_artifact.shared_object_path)
     
-  def calc_V(self, x: np.array, args: np.array) -> float:
+  def calc_V(self, x: np.ndarray, args: np.ndarray) -> float:
     """calculates the scalar potential at field-space coordinates `x` with
     model-specific parameters `args`.
 
     ### Args
-    - `x` (`np.array`): field-space coordinates at which to calculate
-    - `args` (`np.array`): values of the model-dependent parameters. See
+    - `x` (`np.ndarray`): field-space coordinates at which to calculate
+    - `args` (`np.ndarray`): values of the model-dependent parameters. See
     `CompilationArtifact.print_sym_lookup_table()` for an overview of which
     sympy symbols were mapped to which args index.
 
     ### Returns
       `float`: Value of scalar potential with parameters `args` at coordinates `x`.
     """
     return self.dylib.potential(x, args)
   
   def calc_V_array(self,
-    args: list[float] | np.ndarray[float],
-    start: list[float] | np.ndarray[float],
-    stop: list[float] | np.ndarray[float],
+    args: list[float] | np.ndarray,
+    start: list[float] | np.ndarray,
+    stop: list[float] | np.ndarray,
     N: list[int] | None = None
-  ) -> np.ndarray[float]:
+  ) -> np.ndarray:
     """constructs an array of field space coordinates and fills it with the
     value of the scalar potential at those field space coordinates.
     The start and stop values of each axis in field-space can be specified with
     the `start` and `stop` arguments. The number of samples along each axis can
     be set with the `N` argument. It defaults to `8000` per axis.
 
     ### Args
-    - `args` (`list[float] | np.ndarray[float]`): values of the model-dependent
+    - `args` (`list[float] | np.ndarray`): values of the model-dependent
     parameters. See `CompilationArtifact.print_sym_lookup_table()` for an
     overview of which sympy symbols were mapped to which args index.
-    - `start` (`list[float] | np.ndarray[float]`): list of minimum values for
+    - `start` (`list[float] | np.ndarray`): list of minimum values for
     each axis of the to-be-constructed array in field space.
-    - `stop` (`list[float] | np.ndarray[float]`): list of maximum values for each
+    - `stop` (`list[float] | np.ndarray`): list of maximum values for each
     axis of the to-be-constructed array in field space.
     - `N` (`list[int] | None`, optional): _description_. list of the number of
     samples along each axis in field space. If set to `None`, 8000 samples will
     be used along each axis.
 
     ### Returns
-    `np.ndarray[float]`: value of scalar potential at specified field-space
+    `np.ndarray`: value of scalar potential at specified field-space
     coordinates
     """
     n_fields = self.artifact.n_fields
     start_stop = np.array([[start, stop] for (start, stop) in zip(start, stop)])
     N = N if N is not None else np.array([8000 for _ in range(n_fields)])
     x = np.zeros(N)
     self.dylib.potential_array(x, args, start_stop)
     return x
   
-  def calc_H(self, x: np.array, args: np.array) -> np.array:
+  def calc_H(self, x: np.ndarray, args: np.ndarray) -> np.ndarray:
     """calculates the projected covariant Hesse matrix at field-space
     coordinates `x` with model-specific parameters `args`.
 
     ### Args
-    - `x` (`np.array`): field-space coordinates at which to calculate
-    - `args` (`np.array`): values of the model-dependent parameters. See
+    - `x` (`np.ndarray`): field-space coordinates at which to calculate
+    - `args` (`np.ndarray`): values of the model-dependent parameters. See
     `CompilationArtifact.print_sym_lookup_table()` for an overview of which
     sympy symbols were mapped to which args index.
 
     ### Returns
     `np.ndarray`: Components of the projected covariant hesse matrix with
       parameters `args` at coordinates `x`.
     """
@@ -124,22 +124,22 @@
   with the appropriate methods. For more info, see the `.evaluate()` method.
   """
   
   def __init__(self, compiled_artifact: CompilationArtifact):
     super().__init__(compiled_artifact)
     
   def evaluate(self,
-    args: np.ndarray[float],
+    args: np.ndarray,
     x0_start: float,
     x0_stop: float,
     x1_start: float,
     x1_stop: float,
     N_x0: int = 10_000,
     N_x1: int = 10_000
-  ) -> np.ndarray[float]:
+  ) -> np.ndarray:
     """Evaluates the potential consistency condition from Anguelova and Lazaroiu
     2022 paper (`arXiv:2210.00031v2`) for rapid-turn, slow-roll (RTSL)
     inflationary models.
     
     In their paper, the authors claim that RTSL models must satisfy a consistency
     condition:
       3V (V_vv)^2 = (V_vw)^2 V_ww
@@ -155,36 +155,36 @@
       out = lhs / rhs - 1
     The field-space region to be investigated is specified with the arguments of
     this function.
 
     ### Args
     General: See `CompilationArtifact.print_sym_lookup_table()` for an overview
     of which sympy symbols were mapped to which arguments (args) and fields (x).
-    - `args` (`np.array`): values of the model-dependent parameters. 
+    - `args` (`np.ndarray`): values of the model-dependent parameters. 
     - `x0_start` (`float`): minimum value of first field `x[0]`.
     - `x0_stop` (`float`): maximum value of first field `x[0]`.
     - `x1_start` (`float`): minimum value of second field `x[1]`.
     - `y_stop` (`float`): maximum value of second field `x[1]`.
     - `N_x` (`int`, optional): number of steps along `x[0]` axis. Defaults to 10_000.
     - `x1_stop` (`int`, optional): number of steps along `x[1]` axis. Defaults to 10_000.
 
     ### Returns
-    `np.array`: Quotient of left-hand side and right-hand side of
+    `np.ndarray`: Quotient of left-hand side and right-hand side of
     Anguelova & Lazaroiu consistency condition, minus one.
       
     ### Example
     Run and plot the consistency condition
     ```python
     from inflatox.consistency_conditions import AnguelovaLazaroiuCondition
     from matplotlib import pyplot as plt
     anguelova = AnguelovaLazaroiuCondition(comp_artifact)
 
     #calculate condition
-    args = np.array([3.4e-10, 5e-16, 2.5e-3, 1.0])
-    x = np.array([2.0, 2.0])
+    args = np.ndarray([3.4e-10, 5e-16, 2.5e-3, 1.0])
+    x = np.ndarray([2.0, 2.0])
     extent = (-1e-3, 1e-3, -1e-3, 1e-3)
     array = anguelova.evaluate(args, *extent)
     
     #plot result
     plt.imshow(array, extent=extent)
     plt.colorbar()
     plt.show()
```

## Comparing `inflatox-0.2.0.dist-info/METADATA` & `inflatox-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inflatox
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: cffi
 Requires-Dist: numpy >1
 Requires-Dist: sympy >1
 Requires-Dist: joblib >1
 Requires-Dist: einsteinpy >=0.4
```

## Comparing `inflatox-0.2.0.dist-info/license_files/LICENSE-EN.txt` & `inflatox-0.2.1.dist-info/license_files/LICENSE-EN.txt`

 * *Files identical despite different names*

## Comparing `inflatox-0.2.0.dist-info/license_files/LICENSE.md` & `inflatox-0.2.1.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

## Comparing `inflatox-0.2.0.dist-info/RECORD` & `inflatox-0.2.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-inflatox-0.2.0.dist-info/METADATA,sha256=LmZLc9Hc7IBabNup4jGAOPBkMzt30I54SQN8So8bG7U,5170
-inflatox-0.2.0.dist-info/WHEEL,sha256=EOMNtrT_gKkmhndb21X5-Kx7YThUf3BfKaagKjbmQiw,94
-inflatox-0.2.0.dist-info/license_files/LICENSE-EN.txt,sha256=Aif1zk6wdAUTw1KYZpRUC_cXUeVECcTDwYncAOS1DFI,14114
-inflatox-0.2.0.dist-info/license_files/LICENSE.md,sha256=KmidoWBnFWjACK_7WlJKWKoQmwzCzFjn5L5V0wPtcyQ,377429
+inflatox-0.2.1.dist-info/METADATA,sha256=6Kl75ZX_ca4XktQDsusKEFLBrSKV8t79zFqd5x-bjBI,5170
+inflatox-0.2.1.dist-info/WHEEL,sha256=EOMNtrT_gKkmhndb21X5-Kx7YThUf3BfKaagKjbmQiw,94
+inflatox-0.2.1.dist-info/license_files/LICENSE-EN.txt,sha256=Aif1zk6wdAUTw1KYZpRUC_cXUeVECcTDwYncAOS1DFI,14114
+inflatox-0.2.1.dist-info/license_files/LICENSE.md,sha256=KmidoWBnFWjACK_7WlJKWKoQmwzCzFjn5L5V0wPtcyQ,377429
 inflatox/compiler.py,sha256=D2gXrIYCIwh85h6R1q9S6gY-1APb1EQugateyB7Uo6Y,11416
-inflatox/consistency_conditions.py,sha256=oIvGdB37Inf0TUVv5jKp5aUQIxOdT4vrSG2CEL88Ofg,8656
+inflatox/consistency_conditions.py,sha256=P650fyWYj4UGpyE-Zomk-gdIgIIxU1L3_Gani7EIUP0,8612
 inflatox/symbolic.py,sha256=iLv2oTsGvfxy53qURfRx2cSu8thsIxSXB6ks0vekJDw,20784
 inflatox/version.py,sha256=bgjvalwat8dCu27o6K_wuVg7hnihc6tjA5N-QgMwsek,908
 inflatox/__init__.py,sha256=pKHxt6-PAv5teetfVStAAFPkY1CY1H8cqcsR0sIl-5U,1189
-inflatox/libinflx_rs.pyd,sha256=y3Lv8zVC0jqwOsc1qMoK_uZwxGEdSHPyNXJxOtVO42M,495616
-inflatox-0.2.0.dist-info/RECORD,,
+inflatox/libinflx_rs.pyd,sha256=3G8682NIaL9N-9sCU4GUifT1cCUIzpmxof70hy7g8fA,495616
+inflatox-0.2.1.dist-info/RECORD,,
```

