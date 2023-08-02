# Comparing `tmp/hiveviewer-0.1.12.tar.gz` & `tmp/hiveviewer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiveviewer-0.1.12.tar", last modified: Mon Jul 31 12:28:12 2023, max compression
+gzip compressed data, was "hiveviewer-0.2.1.tar", last modified: Wed Aug  2 03:45:38 2023, max compression
```

## Comparing `hiveviewer-0.1.12.tar` & `hiveviewer-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.794550 hiveviewer-0.1.12/
--rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.1.12/LICENSE
--rw-r--r--   0 yin        (501) staff       (20)     1127 2023-07-31 12:28:12.794426 hiveviewer-0.1.12/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.1.12/README.md
--rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.1.12/pyproject.toml
--rw-r--r--   0 yin        (501) staff       (20)       38 2023-07-31 12:28:12.794589 hiveviewer-0.1.12/setup.cfg
--rw-r--r--   0 yin        (501) staff       (20)     1007 2023-07-31 12:27:36.000000 hiveviewer-0.1.12/setup.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.789270 hiveviewer-0.1.12/src/
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.790513 hiveviewer-0.1.12/src/hiveviewer/
--rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.1.12/src/hiveviewer/__init__.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.791833 hiveviewer-0.1.12/src/hiveviewer/dataloader/
--rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.1.12/src/hiveviewer/dataloader/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     3169 2023-07-21 04:18:15.000000 hiveviewer-0.1.12/src/hiveviewer/dataloader/base.py
--rw-r--r--   0 yin        (501) staff       (20)      519 2023-07-21 03:59:25.000000 hiveviewer-0.1.12/src/hiveviewer/dataloader/load_csv.py
--rw-r--r--   0 yin        (501) staff       (20)      512 2023-07-21 03:19:27.000000 hiveviewer-0.1.12/src/hiveviewer/dataloader/load_excel.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.792094 hiveviewer-0.1.12/src/hiveviewer/evaluation/
--rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.1.12/src/hiveviewer/evaluation/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     6440 2023-07-31 12:13:52.000000 hiveviewer-0.1.12/src/hiveviewer/evaluation/calculator.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.792574 hiveviewer-0.1.12/src/hiveviewer/optimization/
--rw-r--r--   0 yin        (501) staff       (20)      128 2023-07-19 08:12:07.000000 hiveviewer-0.1.12/src/hiveviewer/optimization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)      770 2023-07-20 10:58:22.000000 hiveviewer-0.1.12/src/hiveviewer/optimization/base.py
--rw-r--r--   0 yin        (501) staff       (20)     5105 2023-07-31 12:24:57.000000 hiveviewer-0.1.12/src/hiveviewer/optimization/profolio_objective.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.793400 hiveviewer-0.1.12/src/hiveviewer/sampling/
--rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.1.12/src/hiveviewer/sampling/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.1.12/src/hiveviewer/sampling/base.py
--rw-r--r--   0 yin        (501) staff       (20)     1394 2023-07-31 03:32:57.000000 hiveviewer-0.1.12/src/hiveviewer/sampling/frequency_sampler.py
--rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.1.12/src/hiveviewer/sampling/gini_sampler.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.794234 hiveviewer-0.1.12/src/hiveviewer/visualization/
--rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.1.12/src/hiveviewer/visualization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.1.12/src/hiveviewer/visualization/lorenz_curve.py
--rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.1.12/src/hiveviewer/visualization/plot_trisurf.py
--rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.1.12/src/hiveviewer/visualization/venn2.py
--rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.1.12/src/hiveviewer/visualization/venn3.py
--rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.1.12/src/hiveviewer/visualization/venn_base.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-07-31 12:28:12.791248 hiveviewer-0.1.12/src/hiveviewer.egg-info/
--rw-r--r--   0 yin        (501) staff       (20)     1127 2023-07-31 12:28:12.000000 hiveviewer-0.1.12/src/hiveviewer.egg-info/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)     1013 2023-07-31 12:28:12.000000 hiveviewer-0.1.12/src/hiveviewer.egg-info/SOURCES.txt
--rw-r--r--   0 yin        (501) staff       (20)        1 2023-07-31 12:28:12.000000 hiveviewer-0.1.12/src/hiveviewer.egg-info/dependency_links.txt
--rw-r--r--   0 yin        (501) staff       (20)       82 2023-07-31 12:28:12.000000 hiveviewer-0.1.12/src/hiveviewer.egg-info/requires.txt
--rw-r--r--   0 yin        (501) staff       (20)       11 2023-07-31 12:28:12.000000 hiveviewer-0.1.12/src/hiveviewer.egg-info/top_level.txt
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.591529 hiveviewer-0.2.1/
+-rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.2.1/LICENSE
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-02 03:45:38.591142 hiveviewer-0.2.1/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.2.1/README.md
+-rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.2.1/pyproject.toml
+-rw-r--r--   0 yin        (501) staff       (20)       38 2023-08-02 03:45:38.591962 hiveviewer-0.2.1/setup.cfg
+-rw-r--r--   0 yin        (501) staff       (20)     1006 2023-08-02 03:41:52.000000 hiveviewer-0.2.1/setup.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.573799 hiveviewer-0.2.1/src/
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.576498 hiveviewer-0.2.1/src/hiveviewer/
+-rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.2.1/src/hiveviewer/__init__.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.581311 hiveviewer-0.2.1/src/hiveviewer/dataloader/
+-rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.2.1/src/hiveviewer/dataloader/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     3169 2023-07-21 04:18:15.000000 hiveviewer-0.2.1/src/hiveviewer/dataloader/base.py
+-rw-r--r--   0 yin        (501) staff       (20)      519 2023-07-21 03:59:25.000000 hiveviewer-0.2.1/src/hiveviewer/dataloader/load_csv.py
+-rw-r--r--   0 yin        (501) staff       (20)      512 2023-07-21 03:19:27.000000 hiveviewer-0.2.1/src/hiveviewer/dataloader/load_excel.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.582363 hiveviewer-0.2.1/src/hiveviewer/evaluation/
+-rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.2.1/src/hiveviewer/evaluation/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     7284 2023-08-02 03:41:50.000000 hiveviewer-0.2.1/src/hiveviewer/evaluation/calculator.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.583391 hiveviewer-0.2.1/src/hiveviewer/optimization/
+-rw-r--r--   0 yin        (501) staff       (20)      128 2023-08-01 02:03:43.000000 hiveviewer-0.2.1/src/hiveviewer/optimization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)      770 2023-08-02 03:43:12.000000 hiveviewer-0.2.1/src/hiveviewer/optimization/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     5826 2023-08-02 03:41:50.000000 hiveviewer-0.2.1/src/hiveviewer/optimization/multiple_objective.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.585956 hiveviewer-0.2.1/src/hiveviewer/sampling/
+-rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.2.1/src/hiveviewer/sampling/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.2.1/src/hiveviewer/sampling/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     1394 2023-07-31 03:32:57.000000 hiveviewer-0.2.1/src/hiveviewer/sampling/frequency_sampler.py
+-rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.2.1/src/hiveviewer/sampling/gini_sampler.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.590246 hiveviewer-0.2.1/src/hiveviewer/visualization/
+-rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.2.1/src/hiveviewer/visualization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.2.1/src/hiveviewer/visualization/lorenz_curve.py
+-rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.2.1/src/hiveviewer/visualization/plot_trisurf.py
+-rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.2.1/src/hiveviewer/visualization/venn2.py
+-rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.2.1/src/hiveviewer/visualization/venn3.py
+-rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.2.1/src/hiveviewer/visualization/venn_base.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-02 03:45:38.578669 hiveviewer-0.2.1/src/hiveviewer.egg-info/
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-02 03:45:38.000000 hiveviewer-0.2.1/src/hiveviewer.egg-info/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)     1013 2023-08-02 03:45:38.000000 hiveviewer-0.2.1/src/hiveviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yin        (501) staff       (20)        1 2023-08-02 03:45:38.000000 hiveviewer-0.2.1/src/hiveviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yin        (501) staff       (20)       82 2023-08-02 03:45:38.000000 hiveviewer-0.2.1/src/hiveviewer.egg-info/requires.txt
+-rw-r--r--   0 yin        (501) staff       (20)       11 2023-08-02 03:45:38.000000 hiveviewer-0.2.1/src/hiveviewer.egg-info/top_level.txt
```

### Comparing `hiveviewer-0.1.12/LICENSE` & `hiveviewer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/PKG-INFO` & `hiveviewer-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.1.12
+Version: 0.2.1
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.1.12/README.md` & `hiveviewer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/setup.py` & `hiveviewer-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "openpyxl",
         "optuna",
     ],
 )
 
 setup(
     name="hiveviewer",
-    version="0.1.12",
+    version="0.2.1",
     author="Yin Cheng",
     author_email="yin.sjtu@gmail.com",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/yinsn/hiveviewer",
     python_requires=">=3.6",
     description="Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.",
```

### Comparing `hiveviewer-0.1.12/src/hiveviewer/dataloader/base.py` & `hiveviewer-0.2.1/src/hiveviewer/dataloader/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/src/hiveviewer/dataloader/load_csv.py` & `hiveviewer-0.2.1/src/hiveviewer/dataloader/load_csv.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/src/hiveviewer/dataloader/load_excel.py` & `hiveviewer-0.2.1/src/hiveviewer/dataloader/load_excel.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/src/hiveviewer/evaluation/calculator.py` & `hiveviewer-0.2.1/src/hiveviewer/evaluation/calculator.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,52 +11,59 @@
 class Calculator:
     """Calculator class for calculating various metrics."""
 
     def __init__(
         self,
         df: pd.DataFrame,
         selected_columns: List[str],
+        equation_type: str = "product",
         weights_for_groups: Optional[pd.Series] = None,
     ) -> None:
         """Initialize Calculator.
 
         :param df: dataframe
         :param selected_columns: selected columns
         :param weights_for_groups: weights for group
         """
         self.df = df
         self.df_len = len(self.df)
+        self.selected_columns = selected_columns
         self.selected_values = self.df[selected_columns].values
+        self.equation_type = equation_type
         if weights_for_groups is None:
             self.weights_for_groups = pd.Series(
                 np.ones(len(self.df)), index=self.df.index
             )
         else:
             self.weights_for_groups = weights_for_groups
 
     def get_overall_score(
         self,
-        powers_for_equation: List[float],
-        first_order_weights: Optional[List[float]] = None,
+        weights_for_equation: List[float],
     ) -> None:
         """Calculate overall score.
 
         :param powers_for_equation: powers for equation
         :param first_order_weights: first order weights
         """
-        if first_order_weights is not None:
+        if len(weights_for_equation) == 2 * len(self.selected_columns):
+            powers_for_equation = weights_for_equation[: len(self.selected_columns)]
+            first_order_weights = weights_for_equation[len(self.selected_columns) :]
             self.df["overall_score"] = np.product(
                 (1 + np.asarray(first_order_weights) * np.asarray(self.selected_values))
                 ** powers_for_equation,
                 axis=1,
             )
-        else:
+        elif self.equation_type == "product":
             self.df["overall_score"] = np.product(
-                self.selected_values**powers_for_equation, axis=1
+                self.selected_values**weights_for_equation, axis=1
             )
+        elif self.equation_type == "sum":
+            weights_array = np.array(weights_for_equation).reshape(-1, 1)
+            self.df["overall_score"] = self.selected_values @ weights_array
 
     def calculate_wuauc(
         self,
         groupby: str,
         weights_for_equation: List,
         weights_for_groups: Optional[pd.Series] = None,
         label_column: str = "label",
@@ -116,33 +123,43 @@
             laplace_smoothing=laplace_smoothing,
         )
         self.score_column = score_column
         self.create_score_columns(
             boundary_dict=self.sampler.sample(), score_column=score_column
         )
 
-    def calculate_wouauc(
+    def calculate_woauc(
         self,
         weights_for_equation: List,
     ) -> List[float]:
         """Calculate weighted ordinal user AUC.
 
         :param weights_for_equation: weights for equation
         :param score_column: score column
         """
         self.get_overall_score(weights_for_equation)
-        wouauc = []
+        woauc = []
         for k, _ in self.sampler.boundary_dict.items():
             paritial_auc = float(
                 roc_auc_score(
                     self.df[f"{self.score_column}_lt_{k}"], self.df["overall_score"]
                 )
             )
-            wouauc.append(paritial_auc)
-        return wouauc
+            woauc.append(paritial_auc)
+        return woauc
+
+    def calculate_log_mse(self, target_column: str) -> float:
+        """Calculate log mean squared error.
+
+        :param target_column: target column
+        """
+        log_true = np.log(self.df[target_column] + 1)
+        log_pred = np.log(self.df["overall_score"] + 1)
+        mse = np.mean((log_true - log_pred) ** 2)
+        return float(mse)
 
     def calculate_portfolio_concentration(
         self, target_column: str, expected_return: Optional[float] = None
     ) -> Tuple[float, float]:
         """Calculate portfolio concentration.
 
         :param target_column: target column
```

### Comparing `hiveviewer-0.1.12/src/hiveviewer/optimization/base.py` & `hiveviewer-0.2.1/src/hiveviewer/optimization/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/src/hiveviewer/optimization/profolio_objective.py` & `hiveviewer-0.2.1/src/hiveviewer/optimization/multiple_objective.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from typing import List, Optional
 
+import numpy as np
 import optuna
 from optuna.trial import Trial
 
 from ..evaluation.calculator import Calculator
 from .base import BaseObjective
 
 
-class ProfolioObjective(BaseObjective):
+class MultipleObjective(BaseObjective):
     """
     This class provides methods to optimize the profolio objective.
     """
 
     def __init__(
         self,
         direction: str,
@@ -54,88 +55,103 @@
         self.logger = optuna.logging.get_logger("optuna")
         self.logger.addHandler(file_handler)
 
     def add_calculator(
         self,
         calculator: Calculator,
         flag: str,
-        hyperparameter: Optional[float],
         target_column: str,
+        hyperparameter: Optional[float] = None,
     ) -> None:
         """Add calculators to the objective.
 
         Args:
             calculator (Calculator): calculator building blocks.
-            flag (str ["wuauc", "profolio"]): type of calculation.
+            flag (str ["wuauc", "profolio", "logmse"]): type of calculation.
             target_column (str): target column to calculate.
         """
         self.calculators.append(calculator)
         self.calculator_flags.append(flag)
         self.target_columns.append(target_column)
-        if hyperparameter:
+        if hyperparameter is not None:
             self.hyperparameters.append(hyperparameter)
         else:
             self.hyperparameters.append(None)
 
     def objective(
         self,
         trial: Trial,
     ) -> float:
         """
         Calculate the objective value.
         """
 
-        weights: List[float] = []
+        power_weights: List[float] = []
         if self.dirichlet:
             for i in range(self.weights_num - 1):
-                weights.append(
-                    trial.suggest_float(f"w{i+1}", 0, max((1 - sum(weights), 0.1)))
+                power_weights.append(
+                    trial.suggest_float(
+                        f"w{i+1}", 0, max((1 - sum(power_weights), 0.1))
+                    )
                 )
-            weights.append(1 - sum(weights))
+            power_weights.append(1 - sum(power_weights))
         else:
             for i in range(self.weights_num):
-                weights.append(trial.suggest_float(f"w{i+1}", 0, 1))
+                power_weights.append(trial.suggest_float(f"w{i+1}", 0, 1))
 
-        if self.first_order:
-            first_order_weights = []
-            for i in range(self.weights_num):
-                first_order_weights.append(
-                    trial.suggest_float(
-                        f"w{self.weights_num+i+1}",
-                        self.first_order_lower_bound,
-                        self.first_order_upper_bound,
-                        log=True,
-                    )
+        first_order_weights: List[float] = []
+        for i in range(self.weights_num):
+            first_order_weights.append(
+                trial.suggest_float(
+                    f"w{self.weights_num+i+1}",
+                    self.first_order_lower_bound,
+                    self.first_order_upper_bound,
+                    log=True,
                 )
-        else:
-            first_order_weights = None
+            )
 
         targets: List[float] = []
         for calculator, flag, hyperparameter, target_column in zip(
             self.calculators,
             self.calculator_flags,
             self.hyperparameters,
             self.target_columns,
         ):
+            weights: List[float] = []
+            if calculator.equation_type == "product":
+                weights = power_weights
+            elif calculator.equation_type == "product" and self.first_order:
+                weights = power_weights + first_order_weights
+            elif calculator.equation_type == "sum":
+                weights = first_order_weights
             calculator.get_overall_score(
-                powers_for_equation=weights,
-                first_order_weights=first_order_weights,
+                weights_for_equation=weights,
             )
             if flag == "profolio":
                 _, concentration = calculator.calculate_portfolio_concentration(
                     target_column=target_column,
                     expected_return=hyperparameter,
                 )
                 targets.append(concentration)
             elif flag == "wuauc":
                 wuauc = calculator.calculate_wuauc(
                     groupby=target_column,
                     weights_for_equation=weights,
                 )
                 targets.append(wuauc)
+            elif flag == "woauc":
+                woauc = calculator.calculate_woauc(
+                    weights_for_equation=weights,
+                )
+                targets.append(sum(woauc))
+            elif flag == "logmse":
+                mse = calculator.calculate_log_mse(
+                    target_column=target_column,
+                )
+                targets.append(mse)
 
         local_vars = {"targets": targets, "sum": sum}
         result = float(eval(self.formula, {"__builtins__": None}, local_vars))
         if self.logger:
             self.logger.info(f"Trial {trial.number} finished with result: {result}")
             self.logger.info(f"targets: {targets}")
             self.logger.info(f"weights: {weights}")
```

### Comparing `hiveviewer-0.1.12/src/hiveviewer/sampling/base.py` & `hiveviewer-0.2.1/src/hiveviewer/sampling/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/src/hiveviewer/sampling/frequency_sampler.py` & `hiveviewer-0.2.1/src/hiveviewer/sampling/frequency_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/src/hiveviewer/sampling/gini_sampler.py` & `hiveviewer-0.2.1/src/hiveviewer/sampling/gini_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/src/hiveviewer/visualization/lorenz_curve.py` & `hiveviewer-0.2.1/src/hiveviewer/visualization/lorenz_curve.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/src/hiveviewer/visualization/plot_trisurf.py` & `hiveviewer-0.2.1/src/hiveviewer/visualization/plot_trisurf.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/src/hiveviewer/visualization/venn2.py` & `hiveviewer-0.2.1/src/hiveviewer/visualization/venn2.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/src/hiveviewer/visualization/venn3.py` & `hiveviewer-0.2.1/src/hiveviewer/visualization/venn3.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/src/hiveviewer/visualization/venn_base.py` & `hiveviewer-0.2.1/src/hiveviewer/visualization/venn_base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.1.12/src/hiveviewer.egg-info/PKG-INFO` & `hiveviewer-0.2.1/src/hiveviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.1.12
+Version: 0.2.1
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.1.12/src/hiveviewer.egg-info/SOURCES.txt` & `hiveviewer-0.2.1/src/hiveviewer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 src/hiveviewer/dataloader/base.py
 src/hiveviewer/dataloader/load_csv.py
 src/hiveviewer/dataloader/load_excel.py
 src/hiveviewer/evaluation/__init__.py
 src/hiveviewer/evaluation/calculator.py
 src/hiveviewer/optimization/__init__.py
 src/hiveviewer/optimization/base.py
-src/hiveviewer/optimization/profolio_objective.py
+src/hiveviewer/optimization/multiple_objective.py
 src/hiveviewer/sampling/__init__.py
 src/hiveviewer/sampling/base.py
 src/hiveviewer/sampling/frequency_sampler.py
 src/hiveviewer/sampling/gini_sampler.py
 src/hiveviewer/visualization/__init__.py
 src/hiveviewer/visualization/lorenz_curve.py
 src/hiveviewer/visualization/plot_trisurf.py
```

