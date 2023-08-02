# Comparing `tmp/hiveviewer-0.2.1.tar.gz` & `tmp/hiveviewer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiveviewer-0.2.1.tar", last modified: Wed Aug  2 03:45:38 2023, max compression
+gzip compressed data, was "hiveviewer-0.2.2.tar", last modified: Wed Aug  2 04:47:02 2023, max compression
```

## Comparing `hiveviewer-0.2.1.tar` & `hiveviewer-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.591529 hiveviewer-0.2.1/
--rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.2.1/LICENSE
--rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-02 03:45:38.591142 hiveviewer-0.2.1/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.2.1/README.md
--rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.2.1/pyproject.toml
--rw-r--r--   0 yin        (501) staff       (20)       38 2023-08-02 03:45:38.591962 hiveviewer-0.2.1/setup.cfg
--rw-r--r--   0 yin        (501) staff       (20)     1006 2023-08-02 03:41:52.000000 hiveviewer-0.2.1/setup.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.573799 hiveviewer-0.2.1/src/
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.576498 hiveviewer-0.2.1/src/hiveviewer/
--rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.2.1/src/hiveviewer/__init__.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.581311 hiveviewer-0.2.1/src/hiveviewer/dataloader/
--rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.2.1/src/hiveviewer/dataloader/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     3169 2023-07-21 04:18:15.000000 hiveviewer-0.2.1/src/hiveviewer/dataloader/base.py
--rw-r--r--   0 yin        (501) staff       (20)      519 2023-07-21 03:59:25.000000 hiveviewer-0.2.1/src/hiveviewer/dataloader/load_csv.py
--rw-r--r--   0 yin        (501) staff       (20)      512 2023-07-21 03:19:27.000000 hiveviewer-0.2.1/src/hiveviewer/dataloader/load_excel.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.582363 hiveviewer-0.2.1/src/hiveviewer/evaluation/
--rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.2.1/src/hiveviewer/evaluation/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     7284 2023-08-02 03:41:50.000000 hiveviewer-0.2.1/src/hiveviewer/evaluation/calculator.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.583391 hiveviewer-0.2.1/src/hiveviewer/optimization/
--rw-r--r--   0 yin        (501) staff       (20)      128 2023-08-01 02:03:43.000000 hiveviewer-0.2.1/src/hiveviewer/optimization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)      770 2023-08-02 03:43:12.000000 hiveviewer-0.2.1/src/hiveviewer/optimization/base.py
--rw-r--r--   0 yin        (501) staff       (20)     5826 2023-08-02 03:41:50.000000 hiveviewer-0.2.1/src/hiveviewer/optimization/multiple_objective.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.585956 hiveviewer-0.2.1/src/hiveviewer/sampling/
--rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.2.1/src/hiveviewer/sampling/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.2.1/src/hiveviewer/sampling/base.py
--rw-r--r--   0 yin        (501) staff       (20)     1394 2023-07-31 03:32:57.000000 hiveviewer-0.2.1/src/hiveviewer/sampling/frequency_sampler.py
--rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.2.1/src/hiveviewer/sampling/gini_sampler.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.590246 hiveviewer-0.2.1/src/hiveviewer/visualization/
--rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.2.1/src/hiveviewer/visualization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.2.1/src/hiveviewer/visualization/lorenz_curve.py
--rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.2.1/src/hiveviewer/visualization/plot_trisurf.py
--rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.2.1/src/hiveviewer/visualization/venn2.py
--rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.2.1/src/hiveviewer/visualization/venn3.py
--rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.2.1/src/hiveviewer/visualization/venn_base.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.578669 hiveviewer-0.2.1/src/hiveviewer.egg-info/
--rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-02 03:45:38.000000 hiveviewer-0.2.1/src/hiveviewer.egg-info/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)     1013 2023-08-02 03:45:38.000000 hiveviewer-0.2.1/src/hiveviewer.egg-info/SOURCES.txt
--rw-r--r--   0 yin        (501) staff       (20)        1 2023-08-02 03:45:38.000000 hiveviewer-0.2.1/src/hiveviewer.egg-info/dependency_links.txt
--rw-r--r--   0 yin        (501) staff       (20)       82 2023-08-02 03:45:38.000000 hiveviewer-0.2.1/src/hiveviewer.egg-info/requires.txt
--rw-r--r--   0 yin        (501) staff       (20)       11 2023-08-02 03:45:38.000000 hiveviewer-0.2.1/src/hiveviewer.egg-info/top_level.txt
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.455361 hiveviewer-0.2.2/
+-rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.2.2/LICENSE
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-02 04:47:02.455192 hiveviewer-0.2.2/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.2.2/README.md
+-rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.2.2/pyproject.toml
+-rw-r--r--   0 yin        (501) staff       (20)       38 2023-08-02 04:47:02.455411 hiveviewer-0.2.2/setup.cfg
+-rw-r--r--   0 yin        (501) staff       (20)     1006 2023-08-02 04:45:55.000000 hiveviewer-0.2.2/setup.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.445181 hiveviewer-0.2.2/src/
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.446833 hiveviewer-0.2.2/src/hiveviewer/
+-rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.2.2/src/hiveviewer/__init__.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.449201 hiveviewer-0.2.2/src/hiveviewer/dataloader/
+-rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.2.2/src/hiveviewer/dataloader/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     3169 2023-07-21 04:18:15.000000 hiveviewer-0.2.2/src/hiveviewer/dataloader/base.py
+-rw-r--r--   0 yin        (501) staff       (20)      519 2023-07-21 03:59:25.000000 hiveviewer-0.2.2/src/hiveviewer/dataloader/load_csv.py
+-rw-r--r--   0 yin        (501) staff       (20)      512 2023-07-21 03:19:27.000000 hiveviewer-0.2.2/src/hiveviewer/dataloader/load_excel.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.449954 hiveviewer-0.2.2/src/hiveviewer/evaluation/
+-rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.2.2/src/hiveviewer/evaluation/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     7284 2023-08-02 03:41:50.000000 hiveviewer-0.2.2/src/hiveviewer/evaluation/calculator.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.450938 hiveviewer-0.2.2/src/hiveviewer/optimization/
+-rw-r--r--   0 yin        (501) staff       (20)      128 2023-08-01 02:03:43.000000 hiveviewer-0.2.2/src/hiveviewer/optimization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)      770 2023-08-02 03:43:12.000000 hiveviewer-0.2.2/src/hiveviewer/optimization/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     5984 2023-08-02 04:46:32.000000 hiveviewer-0.2.2/src/hiveviewer/optimization/multiple_objective.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.452759 hiveviewer-0.2.2/src/hiveviewer/sampling/
+-rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.2.2/src/hiveviewer/sampling/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.2.2/src/hiveviewer/sampling/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     1394 2023-07-31 03:32:57.000000 hiveviewer-0.2.2/src/hiveviewer/sampling/frequency_sampler.py
+-rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.2.2/src/hiveviewer/sampling/gini_sampler.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.454831 hiveviewer-0.2.2/src/hiveviewer/visualization/
+-rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.2.2/src/hiveviewer/visualization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.2.2/src/hiveviewer/visualization/lorenz_curve.py
+-rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.2.2/src/hiveviewer/visualization/plot_trisurf.py
+-rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.2.2/src/hiveviewer/visualization/venn2.py
+-rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.2.2/src/hiveviewer/visualization/venn3.py
+-rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.2.2/src/hiveviewer/visualization/venn_base.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 04:47:02.447924 hiveviewer-0.2.2/src/hiveviewer.egg-info/
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-02 04:47:02.000000 hiveviewer-0.2.2/src/hiveviewer.egg-info/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)     1013 2023-08-02 04:47:02.000000 hiveviewer-0.2.2/src/hiveviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yin        (501) staff       (20)        1 2023-08-02 04:47:02.000000 hiveviewer-0.2.2/src/hiveviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yin        (501) staff       (20)       82 2023-08-02 04:47:02.000000 hiveviewer-0.2.2/src/hiveviewer.egg-info/requires.txt
+-rw-r--r--   0 yin        (501) staff       (20)       11 2023-08-02 04:47:02.000000 hiveviewer-0.2.2/src/hiveviewer.egg-info/top_level.txt
```

### Comparing `hiveviewer-0.2.1/LICENSE` & `hiveviewer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/PKG-INFO` & `hiveviewer-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.2.1
+Version: 0.2.2
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.2.1/README.md` & `hiveviewer-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/setup.py` & `hiveviewer-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "openpyxl",
         "optuna",
     ],
 )
 
 setup(
     name="hiveviewer",
-    version="0.2.1",
+    version="0.2.2",
     author="Yin Cheng",
     author_email="yin.sjtu@gmail.com",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/yinsn/hiveviewer",
     python_requires=">=3.6",
     description="Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.",
```

### Comparing `hiveviewer-0.2.1/src/hiveviewer/dataloader/base.py` & `hiveviewer-0.2.2/src/hiveviewer/dataloader/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer/dataloader/load_csv.py` & `hiveviewer-0.2.2/src/hiveviewer/dataloader/load_csv.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer/dataloader/load_excel.py` & `hiveviewer-0.2.2/src/hiveviewer/dataloader/load_excel.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer/evaluation/calculator.py` & `hiveviewer-0.2.2/src/hiveviewer/evaluation/calculator.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer/optimization/base.py` & `hiveviewer-0.2.2/src/hiveviewer/optimization/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer/optimization/multiple_objective.py` & `hiveviewer-0.2.2/src/hiveviewer/optimization/multiple_objective.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     """
 
     def __init__(
         self,
         direction: str,
         weights_num: int,
         formula: str,
+        power: bool = False,
         first_order: bool = False,
         first_order_lower_bound: float = 1e-3,
         first_order_upper_bound: float = 1e6,
         dirichlet: bool = True,
         log_file: Optional[str] = None,
     ) -> None:
         """
@@ -37,14 +38,15 @@
         super().__init__(direction, formula, first_order, dirichlet)
         self.calculators: List[Calculator] = []
         self.calculator_flags: List[str] = []
         self.hyperparameters: List[Optional[float]] = []
         self.target_columns: List[str] = []
         self.weights_num = weights_num
         self.formula = formula
+        self.power = power
         self.first_order = first_order
         self.first_order_lower_bound = first_order_lower_bound
         self.first_order_upper_bound = first_order_upper_bound
         self.dirichlet = dirichlet
         if log_file:
             self.build_logger(log_file)
 
@@ -80,50 +82,52 @@
     def objective(
         self,
         trial: Trial,
     ) -> float:
         """
         Calculate the objective value.
         """
-
         power_weights: List[float] = []
-        if self.dirichlet:
-            for i in range(self.weights_num - 1):
-                power_weights.append(
-                    trial.suggest_float(
-                        f"w{i+1}", 0, max((1 - sum(power_weights), 0.1))
+        first_order_weights: List[float] = []
+
+        if self.power:
+            if self.dirichlet:
+                for i in range(self.weights_num - 1):
+                    power_weights.append(
+                        trial.suggest_float(
+                            f"w_po_{i+1}", 0, max((1 - sum(power_weights), 0.1))
+                        )
                     )
-                )
-            power_weights.append(1 - sum(power_weights))
-        else:
-            for i in range(self.weights_num):
-                power_weights.append(trial.suggest_float(f"w{i+1}", 0, 1))
+                power_weights.append(1 - sum(power_weights))
+            else:
+                for i in range(self.weights_num):
+                    power_weights.append(trial.suggest_float(f"w{i+1}", 0, 1))
 
-        first_order_weights: List[float] = []
-        for i in range(self.weights_num):
-            first_order_weights.append(
-                trial.suggest_float(
-                    f"w{self.weights_num+i+1}",
-                    self.first_order_lower_bound,
-                    self.first_order_upper_bound,
-                    log=True,
+        if self.first_order:
+            for i in range(self.weights_num):
+                first_order_weights.append(
+                    trial.suggest_float(
+                        f"w_fo_{i+1}",
+                        self.first_order_lower_bound,
+                        self.first_order_upper_bound,
+                        log=True,
+                    )
                 )
-            )
 
         targets: List[float] = []
         for calculator, flag, hyperparameter, target_column in zip(
             self.calculators,
             self.calculator_flags,
             self.hyperparameters,
             self.target_columns,
         ):
             weights: List[float] = []
-            if calculator.equation_type == "product":
+            if not (self.first_order):
                 weights = power_weights
-            elif calculator.equation_type == "product" and self.first_order:
+            elif calculator.equation_type == "product" and self.power:
                 weights = power_weights + first_order_weights
             elif calculator.equation_type == "sum":
                 weights = first_order_weights
             calculator.get_overall_score(
                 weights_for_equation=weights,
             )
             if flag == "profolio":
```

### Comparing `hiveviewer-0.2.1/src/hiveviewer/sampling/base.py` & `hiveviewer-0.2.2/src/hiveviewer/sampling/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer/sampling/frequency_sampler.py` & `hiveviewer-0.2.2/src/hiveviewer/sampling/frequency_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer/sampling/gini_sampler.py` & `hiveviewer-0.2.2/src/hiveviewer/sampling/gini_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer/visualization/lorenz_curve.py` & `hiveviewer-0.2.2/src/hiveviewer/visualization/lorenz_curve.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer/visualization/plot_trisurf.py` & `hiveviewer-0.2.2/src/hiveviewer/visualization/plot_trisurf.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer/visualization/venn2.py` & `hiveviewer-0.2.2/src/hiveviewer/visualization/venn2.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer/visualization/venn3.py` & `hiveviewer-0.2.2/src/hiveviewer/visualization/venn3.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer/visualization/venn_base.py` & `hiveviewer-0.2.2/src/hiveviewer/visualization/venn_base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.1/src/hiveviewer.egg-info/PKG-INFO` & `hiveviewer-0.2.2/src/hiveviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.2.1
+Version: 0.2.2
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.2.1/src/hiveviewer.egg-info/SOURCES.txt` & `hiveviewer-0.2.2/src/hiveviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

