# Comparing `tmp/openpile-0.4.0.tar.gz` & `tmp/openpile-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-mvs9863j/openpile-0.4.0.tar", last modified: Sun Jul 30 20:31:00 2023, max compression
+gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-2tc1nr32/openpile-0.5.0.tar", last modified: Wed Aug  2 21:22:58 2023, max compression
```

## Comparing `openpile-0.4.0.tar` & `openpile-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-30 20:30:51.000000 openpile-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-07-30 20:31:00.000000 openpile-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-30 20:30:51.000000 openpile-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-30 20:30:51.000000 openpile-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-30 20:31:00.000000 openpile-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-30 20:30:51.000000 openpile-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)    60358 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/construct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28674 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/core/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/core/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/core/txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    27008 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/soilmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/Hb_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/Mb_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/mt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/py_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/qz_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-07-30 20:30:51.000000 openpile-0.4.0/src/openpile/utils/tz_curves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 20:31:00.000000 openpile-0.4.0/src/openpile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:31:00.000000 openpile-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-07-30 20:30:51.000000 openpile-0.4.0/test/test_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-30 20:30:51.000000 openpile-0.4.0/test/test_pycurves.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-30 20:30:51.000000 openpile-0.4.0/test/test_utils_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:22:58.000000 openpile-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 21:22:49.000000 openpile-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-08-02 21:22:58.000000 openpile-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-08-02 21:22:49.000000 openpile-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-02 21:22:49.000000 openpile-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-02 21:22:58.000000 openpile-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-02 21:22:49.000000 openpile-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:22:58.000000 openpile-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:22:58.000000 openpile-0.5.0/src/openpile/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60358 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/construct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:22:58.000000 openpile-0.5.0/src/openpile/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28674 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/core/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/core/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/core/txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30265 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/soilmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:22:58.000000 openpile-0.5.0/src/openpile/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/utils/Hb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/utils/Mb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/utils/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/utils/mt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/utils/multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/utils/py_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/utils/qz_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-08-02 21:22:49.000000 openpile-0.5.0/src/openpile/utils/tz_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:22:58.000000 openpile-0.5.0/src/openpile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-08-02 21:22:58.000000 openpile-0.5.0/src/openpile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 21:22:58.000000 openpile-0.5.0/src/openpile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:22:58.000000 openpile-0.5.0/src/openpile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:22:58.000000 openpile-0.5.0/src/openpile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-02 21:22:58.000000 openpile-0.5.0/src/openpile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 21:22:58.000000 openpile-0.5.0/src/openpile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:22:58.000000 openpile-0.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-08-02 21:22:49.000000 openpile-0.5.0/test/test_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-08-02 21:22:49.000000 openpile-0.5.0/test/test_pycurves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-02 21:22:49.000000 openpile-0.5.0/test/test_utils_misc.py
```

### Comparing `openpile-0.4.0/LICENSE.txt` & `openpile-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/PKG-INFO` & `openpile-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.4.0
+Version: 0.5.0
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
 Project-URL: Documentation, https://openpile.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/TchilDill/openpile
```

### Comparing `openpile-0.4.0/README.md` & `openpile-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/setup.cfg` & `openpile-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/setup.py` & `openpile-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/src/openpile/analyze.py` & `openpile-0.5.0/src/openpile/analyze.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/src/openpile/calculate.py` & `openpile-0.5.0/src/openpile/calculate.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/src/openpile/construct.py` & `openpile-0.5.0/src/openpile/construct.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/src/openpile/core/kernel.py` & `openpile-0.5.0/src/openpile/core/kernel.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/src/openpile/core/misc.py` & `openpile-0.5.0/src/openpile/core/misc.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/src/openpile/core/txt.py` & `openpile-0.5.0/src/openpile/core/txt.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/src/openpile/core/validation.py` & `openpile-0.5.0/src/openpile/core/validation.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/src/openpile/soilmodels.py` & `openpile-0.5.0/src/openpile/soilmodels.py`

 * *Files 2% similar despite different names*

```diff
@@ -789,7 +789,95 @@
         z_pos = np.append(z_pos, [z_pos[-1] + i * 0.1 for i in range(diff_length_z)])
 
         # calculate m and t vectors (they are all the same for clay)
         t = np.arctan(z_pos.reshape((1, -1)) / (0.5 * D)) * np.ones((output_length, 1))
         m = 1 / 4 * np.pi * D**2 * tz_pos.reshape((1, -1)) * np.ones((output_length, 1))
 
         return t, m
+
+
+@dataclass(config=PydanticConfigFrozen)
+class Reese_weakrock(LateralModel):
+    """A class to establish the Reese weakrock model.
+
+    Parameters
+    ----------
+    Ei: float or list[top_value, bottom_value]
+        Initial modulus of rock [unit: kPa]
+    qu: float or list[top_value, bottom_value]
+        compressive strength of rock [unit: kPa]
+    RQD: float or list[top_value, bottom_value]
+        Rock Quality Designation [unit: %]
+    k: float
+        dimensional constant randing from 0.0005 to 0.00005, by default 0.0005
+    ztop: float
+        absolute depth of top layer elevation with respect to rock surface [m]
+    p_multiplier: float or function taking the depth as argument and returns the multiplier
+        multiplier for p-values
+    y_multiplier: float or function taking the depth as argument and returns the multiplier
+        multiplier for y-values
+
+    """
+
+    #: initial modulus of rock [kPa], if a variation in values, two values can be given.
+    Ei: Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]
+    #: scompressive strength of rock [kPa], if a variation in values, two values can be given.
+    qu: Optional[Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]]
+    #: Rock Quality Designation
+    RQD: confloat(ge=0.0, le=100.0)
+    #: dimnesional constant
+    k: confloat(ge=0.00005, le=0.0005)
+    #: absolute depth of top layer elevation with respect to rock surface [m]
+    ztop: confloat(ge=0.0)
+    #: p-multiplier
+    p_multiplier: Union[Callable[[float], float], confloat(ge=0.0)] = 1.0
+    #: y-multiplier
+    y_multiplier: Union[Callable[[float], float], confloat(gt=0.0)] = 1.0
+
+    # define class variables needed for all soil models
+    m_multiplier = 1.0
+    t_multiplier = 1.0
+
+    spring_signature = np.array([True, False, False, False], dtype=bool)
+
+    def __str__(self):
+        return f"\tReese weakrock\n\tEi = {var_to_str(self.Ei)}kPa\n\tqu = {var_to_str(self.qu)}kPa\n\tRQD = {var_to_str(self.RQD)}%"
+
+    def py_spring_fct(
+        self,
+        sig: float,
+        X: float,
+        layer_height: float,
+        depth_from_top_of_layer: float,
+        D: float,
+        L: float = None,
+        below_water_table: bool = True,
+        ymax: float = 0.0,
+        output_length: int = 15,
+    ):
+        # validation
+        if depth_from_top_of_layer > layer_height:
+            raise ValueError("Spring elevation outside layer")
+
+        # define Ei
+        Ei_t, Ei_b = from_list2x_parse_top_bottom(self.Ei)
+        Ei = Ei_t + (Ei_b - Ei_t) * depth_from_top_of_layer / layer_height
+
+        # define qu
+        qu_t, qu_b = from_list2x_parse_top_bottom(self.qu)
+        qu = qu_t + (qu_b - qu_t) * depth_from_top_of_layer / layer_height
+
+        y, p = py_curves.reese_weakrock(
+            Ei=Ei,
+            xr=(X + self.ztop),
+            RQD=self.RQD,
+            qu=qu,
+            D=D,
+            k=self.k,
+            output_length=output_length,
+        )
+
+        # parse multipliers and apply results
+        y_mult = self.y_multiplier if isinstance(self.y_multiplier, float) else self.y_multiplier(X)
+        p_mult = self.p_multiplier if isinstance(self.p_multiplier, float) else self.p_multiplier(X)
+
+        return y * y_mult, p * p_mult
```

### Comparing `openpile-0.4.0/src/openpile/utils/Hb_curves.py` & `openpile-0.5.0/src/openpile/utils/Hb_curves.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,17 +44,17 @@
         Embedded pile length [unit: m]
     output_length : int, optional
         Number of datapoints in the curve, by default 20
 
     Returns
     -------
     1darray
-        Hb vector [unit: kN]
-    1darray
         y vector [unit: m]
+    1darray
+        Hb vector [unit: kN]
     """
     # correct relative density for decimal value
     Dr = Dr / 100
 
     # Generalised Dunkirk Sand Model parameters
     v_hu1 = 0.5150 + 2.883 * Dr
     v_hu2 = 0.1695 - 0.7018 * Dr
@@ -106,24 +106,17 @@
         Embedded pile length [unit: m]
     output_length : int, optional
         Number of datapoints in the curve, by default 20
 
     Returns
     -------
     1darray
-        Hb vector [unit: kN]
-    1darray
         y vector [unit: m]
-
-    References
-    ----------
-    .. [1] Byrne, B. W., Houlsby, G. T., Burd, H. J., Gavin, K. G., Igoe, D. J. P., Jardine,
-           R. J., Martin, C. M., McAdam, R. A., Potts, D. M., Taborda, D. M. G. & Zdravkovic ́,
-           L. (2020). PISA design model for monopiles for offshore wind turbines: application
-           to a stiff glacial clay till. Géotechnique, https://doi.org/10.1680/ jgeot.18.P.255.
+    1darray
+        Hb vector [unit: kN]
 
     """
 
     # Generalised Dunkirk Sand Model parameters
     v_hu1 = 235.7
     v_hu2 = 0.00
     k_h1 = 2.717
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openpile-0.4.0/src/openpile/utils/Mb_curves.py` & `openpile-0.5.0/src/openpile/utils/Mb_curves.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         Pile length [unit: m]
     output_length : int, optional
         Number of datapoints in the curve, by default 20
 
     Returns
     -------
     1darray
-        Mb vector [unit: kN]
-    1darray
         t vector of length [unit: rad]
+    1darray
+        Mb vector [unit: kN]
 
     """
 
     # Cowden clay parameters
     k_m1 = 0.2146
     k_m2 = -0.002132
     n_m1 = 1.079
@@ -104,17 +104,17 @@
         Embedded pile length [unit: m]
     output_length : int, optional
         Number of datapoints in the curve, by default 20
 
     Returns
     -------
     1darray
-        Mb vector [unit: kN]
-    1darray
         t vector of length [unit: rad]
+    1darray
+        Mb vector [unit: kN]
     """
     # correct relative density for decimal value
     Dr = Dr / 100
 
     # Generalised Dunkirk Sand Model parameters
     k_m1 = 0.3515
     k_m2 = 0.00
```

### Comparing `openpile-0.4.0/src/openpile/utils/graphics.py` & `openpile-0.5.0/src/openpile/utils/graphics.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/src/openpile/utils/misc.py` & `openpile-0.5.0/src/openpile/utils/misc.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/src/openpile/utils/mt_curves.py` & `openpile-0.5.0/src/openpile/utils/mt_curves.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,17 @@
         Pile diameter [unit: m]
     output_length : int, optional
         Number of datapoints in the curve, by default 20
 
     Returns
     -------
     1darray
-        m vector [unit: kN]
-    1darray
         t vector of length [unit: rad]
+    1darray
+        m vector [unit: kN]
 
     """
 
     # Cowden clay parameters
     k_m1 = 1.420
     k_m2 = -0.09643
     n_m1 = 0.00
@@ -103,17 +103,17 @@
         Embedded pile length [unit: m]
     output_length : int, optional
         Number of datapoints in the curve, by default 20
 
     Returns
     -------
     1darray
-        m vector [unit: kN]
-    1darray
         t vector of length [unit: rad]
+    1darray
+        m vector [unit: kN]
     """
     # correct relative density for decimal value
     Dr = Dr / 100
 
     # correct p value
     p = abs(p)
```

### Comparing `openpile-0.4.0/src/openpile/utils/multipliers.py` & `openpile-0.5.0/src/openpile/utils/multipliers.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/src/openpile/utils/py_curves.py` & `openpile-0.5.0/src/openpile/utils/py_curves.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,17 +38,17 @@
         Pile diameter [unit: m]
     output_length : int, optional
         Number of datapoints in the curve, by default 20
 
     Returns
     -------
     1darray
-        p vector [unit: kN/m]
-    1darray
         y vector [unit: m]
+    1darray
+        p vector [unit: kN/m]
 
     """
 
     # # Cowden clay parameters
     v_pu = 241.4
     k_p1 = 10.6
     k_p2 = -1.650
@@ -101,17 +101,17 @@
         Embedded pile length [unit: m]
     output_length : int, optional
         Number of datapoints in the curve, by default 20
 
     Returns
     -------
     1darray
-        p vector [unit: kN/m]
-    1darray
         y vector [unit: m]
+    1darray
+        p vector [unit: kN/m]
     """
     # correct relative density for decimal value
     Dr = Dr / 100
 
     # Generalised Dunkirk Sand Model parameters
     v_pu = 146.1 - 92.11 * Dr
     k_p1 = 8.731 - 0.6982 * Dr
@@ -166,17 +166,17 @@
         maximum value of y, default goes to 99.9% of ultimate resistance
     output_length: int, by default 20
         Number of discrete point along the springs
 
     Returns
     -------
     1darray
-        p vector [unit: kN/m]
-    1darray
         y vector [unit: m]
+    1darray
+        p vector [unit: kN/m]
     """
     # A value - only thing that changes between cyclic or static
     if kind == "static":
         A = max(0.9, 3 - 0.8 * X / D)
     else:
         A = 0.9
 
@@ -270,18 +270,17 @@
         maximum value of y, if null the maximum is calculated such that the whole curve is computed
     output_length: int, by default 20
         Number of discrete point along the springs
 
     Returns
     -------
     1darray
-        p vector [unit: kN/m]
-    1darray
         y vector [unit: m]
-    ---------
+    1darray
+        p vector [unit: kN/m]
     """
     # important variables
     y50 = 2.5 * eps50 * D
     if X == 0.0 or Su == 0:
         Xr = 2.5 * D
     else:
         Xr = max((6 * D) / (sig / X * D / Su + J), 2.5 * D)
@@ -352,7 +351,78 @@
                         p[i] = 0.5 * Pmax * (y[i] / y50) ** 0.33
 
         # modification of initial slope of the curve (DNVGL RP-C203 B.2.2.4)
         if y[i] == 0.1 * y50:
             p[i] = 0.23 * Pmax
 
     return y, p
+
+
+@njit(parallel=True, cache=True)
+def reese_weakrock(
+    Ei: float,
+    qu: float,
+    RQD: float,
+    xr: float,
+    D: float,
+    k: float = 0.0005,
+    output_length=20,
+):
+    """creates the Reese weakrock p-y curve based on the work of Reese (1997) #TODO(ref).
+
+
+    Parameters
+    ----------
+    Ei : float
+        initial modulus of rock [kPa]
+    qu : float
+        compressive strength of rock [kPa]
+    RQD : float
+        Rock Quality Designation [%]
+    xr : float
+        depth from rock surface [m]
+    D : float
+        pile width [m]
+    k : float, optional
+        dimensional constant, randing from 0.0005 to 0.00005, by default 0.0005
+    output_length : int, optional
+        length of output arrays, by default 20
+
+    Returns
+    -------
+    1darray
+        y vector [unit: m]
+    1darray
+        p vector [unit: kN/m]
+
+    """
+
+    # Rqd forced to be within 0 and 100
+    rqd = max(min(100, RQD), 0)
+
+    # determine alpha
+    alpha = 1.0 - 2 / 3 * rqd / 100
+
+    # determine ultimate resistance of rock
+    Pmax = min(5.2 * alpha * qu * D, alpha * qu * D * (1 + 1.4 * xr / D))
+
+    # initial portion of p-y curve
+    Epy_i = Ei * min(500, 100 + 400 * xr / (3 * D))
+
+    # yA & yrm
+    yrm = k * D
+    yA = (Pmax / (2 * (yrm) ** 0.25 * Epy_i)) ** 1.333
+
+    # define y
+    ymax = max(1.05 * yA, (2 * yrm ** (0.25)) ** 4)
+    y = np.linspace(yA, ymax, output_length - 2)
+    y = np.concatenate((np.array([0.0]), y, np.array([1.2 * ymax])))
+
+    # define p
+    p = np.zeros(y.size)
+    for i in range(len(p)):
+        if y[i] <= yA:
+            p[i] = min(Pmax, Epy_i * y[i])
+        else:
+            p[i] = min(Pmax, Pmax / 2 * (y[i] / yrm) ** 0.25)
+
+    return y, p
```

### Comparing `openpile-0.4.0/src/openpile/utils/qz_curves.py` & `openpile-0.5.0/src/openpile/utils/qz_curves.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,17 +35,17 @@
         Pile diameter [unit: m]
     output_length : int, optional
         Number of discrete point along the springs, cannot be lower than 8, by default 8
 
     Returns
     -------
     numpy 1darray
-        Q vector [unit: kPa]
-    numpy 1darray
         z vector [unit: m]
+    numpy 1darray
+        Q vector [unit: kPa]
     """
     # cannot have less than 8
     if output_length < 8:
         output_length = 8
 
     # unit toe reistance [kPa]
     f = misc._Qmax_api_sand(sig, delta)
@@ -97,17 +97,17 @@
         Pile diameter [unit: m]
     output_length : int, optional
         Number of discrete point along the springs, cannot be lower than 8, by default 8
 
     Returns
     -------
     numpy 1darray
-        Q vector [unit: kPa]
-    numpy 1darray
         z vector [unit: m]
+    numpy 1darray
+        Q vector [unit: kPa]
     """
     # cannot have less than 8
     if output_length < 8:
         output_length = 8
 
     # unit toe reistance [kPa]
     f = misc._Qmax_api_clay
```

### Comparing `openpile-0.4.0/src/openpile/utils/tz_curves.py` & `openpile-0.5.0/src/openpile/utils/tz_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/src/openpile.egg-info/PKG-INFO` & `openpile-0.5.0/src/openpile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.4.0
+Version: 0.5.0
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
 Project-URL: Documentation, https://openpile.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/TchilDill/openpile
```

### Comparing `openpile-0.4.0/src/openpile.egg-info/SOURCES.txt` & `openpile-0.5.0/src/openpile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/test/test_construct.py` & `openpile-0.5.0/test/test_construct.py`

 * *Files identical despite different names*

### Comparing `openpile-0.4.0/test/test_pycurves.py` & `openpile-0.5.0/test/test_pycurves.py`

 * *Files 11% similar despite different names*

```diff
@@ -110,7 +110,30 @@
         pu = 0.7185*pmax
     elif xkind=="static":
         pres = pmax
         pu = pmax
     assert m.isclose(p[-1],pres, rel_tol=0.01, abs_tol=0.1)
     assert m.isclose(np.max(p), pu, rel_tol=0.01, abs_tol=0.1)
 
+@pytest.mark.parametrize("xEi",[1,75,200])
+@pytest.mark.parametrize("xqu",[1,75,200])
+@pytest.mark.parametrize("xRQD",[0,25,50,75,100])
+@pytest.mark.parametrize("xxr",[0,5,20])
+@pytest.mark.parametrize("xD",[1,3,6])
+def test_reese_weakrock(xEi, xqu, xRQD, xxr, xD):
+    #create curve
+    y, p = py.reese_weakrock(Ei=xEi, qu=xqu, RQD=xRQD, xr=xxr, D=xD)
+    #helper fct
+    is_sorted = lambda a: np.all(a[:-1] <= a[1:])
+    #check if sorted
+    assert is_sorted(y)
+    #check if origin is (0,0)
+    assert p[0] == 0.0
+    assert y[0] == 0.0
+
+    alpha = 1 - 2/3 * xRQD/100
+    pu = min(alpha * xqu * xD * (1+1.4*xxr/xD), 5.2*alpha*xqu*xD)
+    assert m.isclose(np.max(p), pu, rel_tol=0.01, abs_tol=0.1)
+
+
+
+
```

### Comparing `openpile-0.4.0/test/test_utils_misc.py` & `openpile-0.5.0/test/test_utils_misc.py`

 * *Files identical despite different names*

