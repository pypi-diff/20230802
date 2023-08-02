# Comparing `tmp/bcirisktools-0.3.5.tar.gz` & `tmp/bcirisktools-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcirisktools-0.3.5.tar", last modified: Fri Jul 14 16:10:34 2023, max compression
+gzip compressed data, was "bcirisktools-0.4.tar", last modified: Wed Aug  2 19:04:32 2023, max compression
```

## Comparing `bcirisktools-0.3.5.tar` & `bcirisktools-0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-07-14 16:10:34.751000 bcirisktools-0.3.5/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2022-10-12 10:00:20.000000 bcirisktools-0.3.5/LICENCE
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-07-14 16:10:34.744000 bcirisktools-0.3.5/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2022-12-02 15:48:25.000000 bcirisktools-0.3.5/README.md
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-07-14 16:10:34.604000 bcirisktools-0.3.5/bcirisktools/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      308 2023-03-02 03:02:45.000000 bcirisktools-0.3.5/bcirisktools/__init__.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5638 2023-06-06 19:27:22.000000 bcirisktools-0.3.5/bcirisktools/input_filters.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-03-02 03:02:45.000000 bcirisktools-0.3.5/bcirisktools/metrics_bci.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-03-02 03:02:45.000000 bcirisktools-0.3.5/bcirisktools/modeling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    10038 2023-07-14 16:08:21.000000 bcirisktools-0.3.5/bcirisktools/shapley_report.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5783 2023-05-09 16:19:37.000000 bcirisktools-0.3.5/bcirisktools/stability.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    19187 2023-05-09 13:13:17.000000 bcirisktools-0.3.5/bcirisktools/tree_crt.py
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-07-14 16:10:34.725000 bcirisktools-0.3.5/bcirisktools.egg-info/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-07-14 16:10:34.000000 bcirisktools-0.3.5/bcirisktools.egg-info/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      410 2023-07-14 16:10:34.000000 bcirisktools-0.3.5/bcirisktools.egg-info/SOURCES.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-07-14 16:10:34.000000 bcirisktools-0.3.5/bcirisktools.egg-info/dependency_links.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-07-14 16:10:34.000000 bcirisktools-0.3.5/bcirisktools.egg-info/requires.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-07-14 16:10:34.000000 bcirisktools-0.3.5/bcirisktools.egg-info/top_level.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-03-02 03:02:45.000000 bcirisktools-0.3.5/pyproject.toml
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-07-14 16:10:34.755000 bcirisktools-0.3.5/setup.cfg
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1018 2023-07-14 16:09:16.000000 bcirisktools-0.3.5/setup.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:04:32.457000 bcirisktools-0.4/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2023-07-27 13:56:43.000000 bcirisktools-0.4/LICENCE
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      571 2023-08-02 19:04:32.450000 bcirisktools-0.4/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2023-07-27 13:56:43.000000 bcirisktools-0.4/README.md
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:04:32.339000 bcirisktools-0.4/bcirisktools/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      308 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/__init__.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/input_filters.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/metrics_bci.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/modeling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    16808 2023-08-02 19:01:12.000000 bcirisktools-0.4/bcirisktools/profiling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     9991 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/shapley_report.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     5705 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/stability.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/tree_crt.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:04:32.430000 bcirisktools-0.4/bcirisktools.egg-info/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      571 2023-08-02 19:04:31.000000 bcirisktools-0.4/bcirisktools.egg-info/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      436 2023-08-02 19:04:31.000000 bcirisktools-0.4/bcirisktools.egg-info/SOURCES.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-08-02 19:04:31.000000 bcirisktools-0.4/bcirisktools.egg-info/dependency_links.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-08-02 19:04:31.000000 bcirisktools-0.4/bcirisktools.egg-info/requires.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-08-02 19:04:31.000000 bcirisktools-0.4/bcirisktools.egg-info/top_level.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-07-27 13:56:43.000000 bcirisktools-0.4/pyproject.toml
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-08-02 19:04:32.464000 bcirisktools-0.4/setup.cfg
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1016 2023-08-02 19:04:18.000000 bcirisktools-0.4/setup.py
```

### Comparing `bcirisktools-0.3.5/LICENCE` & `bcirisktools-0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.5/PKG-INFO` & `bcirisktools-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.3.5
+Version: 0.4
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.3.5/README.md` & `bcirisktools-0.4/README.md`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.5/bcirisktools/metrics_bci.py` & `bcirisktools-0.4/bcirisktools/metrics_bci.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.5/bcirisktools/modeling.py` & `bcirisktools-0.4/bcirisktools/modeling.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.5/bcirisktools/shapley_report.py` & `bcirisktools-0.4/bcirisktools/shapley_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,22 @@
 
 class GenerateReport:
     def __init__(
         self,
         x,
         y,
         params,
-        min_value=-9999,
         report_name="report",
         model=None,
         name="model",
         order_by="Mean Shapley",
         rng=0,
     ):
         self.name_report = name
         self.order_by = order_by
-        self.min_value = min_value
         # initializate creating values for the analysis
         if model is None:
             self.X_train, self.X_test, self.y_train, self.y_test = train_test_split(
                 x, y, test_size=0.2, random_state=rng
             )
         else:
             self.X_train = x
@@ -83,22 +81,21 @@
             self.predVar, columns=["Features", "Group", "ROC", "KS", "DIV"]
         )
         self.predVar = self.predVar.loc[
             (self.predVar["KS"] > 0.01) & (self.predVar["ROC"] > 0.501), :
         ]
         self.variables_univariate = self.predVar["Features"]
 
-    def _plot_shaps(self, study_var, x_label="", shap_nulls=False):
+    def _plot_shaps(self, study_var, x_label="", min_value=-99999, shap_nulls=False):
         if shap_nulls:
-            cond = self.X_train[study_var].values >= self.min_value
-            shaps_values = self.shap_values.values[... , -1][cond]
+            cond = self.X_train[study_var].values > -99999
+            shaps_values = self.shap_values.values[cond]
             inputs_x = self.X_train[cond]
         else:
-            
-            shaps_values = self.shap_values.values[... , -1]
+            shaps_values = self.shap_values.values
             inputs_x = self.X_train
 
         shap.dependence_plot(
             study_var,
             shaps_values,
             inputs_x,
             xmin="percentile(0.5)",
@@ -122,15 +119,15 @@
         # Univariate analysis
         print("/------------------------------------------------------/")
         print("Initializing univariate analysis...")
         print("/------------------------------------------------------/")
         self._univariate_analysis()
 
         # Redefine data
-        self.X_train = self.X_train
+        self.X_train = self.X_train[self.variables_univariate]
 
         # Get Shapley values
         print("\n/------------------------------------------------------/")
         print("Calculating Shapley values...")
         print("/------------------------------------------------------/")
         if self.model is None:
             self.dtrain = xgb.DMatrix(self.X_train, label=self.y_train)
@@ -138,15 +135,15 @@
         explainer = shap.TreeExplainer(self.model)
         self.shap_values = explainer(self.X_train)
 
         var_names = self.shap_values.feature_names
         var_shap = np.abs(self.shap_values.values).mean(axis=0)
 
         self.df_shap = pd.DataFrame(
-            zip(var_names, var_shap[:, -1]), columns=["Features", "Mean Shapley"]
+            zip(var_names, var_shap), columns=["Features", "Mean Shapley"]
         )
         self.df_shap = self.df_shap.sort_values(
             by="Mean Shapley", ascending=False
         ).reset_index(drop=True)
         self.df_shap_top = self.df_shap.head(10)
 
         # Final Dataframe
@@ -173,16 +170,16 @@
 
         # Get plots
         print("Generating Shapley plots...")
         print("/------------------------------------------------------/")
         for idx, var in enumerate(self.df_shap["Features"]):
             sys.stdout.write(f"\rVariable analyzed: {var} [{idx+1}]")
             try:
-                self._plot_shaps(var, "", shap_nulls=False)
-                self._plot_shaps(var, "", shap_nulls=True)
+                self._plot_shaps(var, "", -99999, shap_nulls=False)
+                self._plot_shaps(var, "", -99999, shap_nulls=True)
             except:
                 sys.stdout.write(f"\rVariable not analyzed: {var} [{idx+1}]")
 
         # Generate report
         print("\n/------------------------------------------------------/")
         print("Generating Html Report...")
         print("/------------------------------------------------------/")
@@ -292,8 +289,8 @@
 
         html_string = html_string + "</body></html>"
         f = open(f"./{self.report_name}.html", "w")
         f.write(html_string)
         f.close()
 
         # Removemos la carpeta temporal de plots
-        shutil.rmtree(mypath)
+        shutil.rmtree(mypath)
```

### Comparing `bcirisktools-0.3.5/bcirisktools/stability.py` & `bcirisktools-0.4/bcirisktools/stability.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             expected = df_feat.iloc[:, i] + 10e-20
             df_out.iloc[:, i + 1] = (actual - expected) * np.log(actual / expected)
 
         # Preparamos salida y append
         df_out = df_out.drop(columns=df_feat.columns[0])
         df_out = pd.DataFrame(df_out.sum()).rename(columns={0: a_variable}).T
         df_out["cuantil"] = quantiles
-        df_append = pd.concat([df_append, df_out], axis=0)
+        df_append = df_append.append(df_out)
 
     # Semaforo de estabilidad
     df_append["status"] = "🟢"
     df_append["status_2"] = "low"
 
     cond1 = (df_append.iloc[:, :-3] >= 0.1) & (df_append.iloc[:, :-3] < 0.2)
     cond1 = cond1.any(axis=1)
@@ -136,25 +136,23 @@
         # Preparamos salida y append para la mean
         df_feat_mean = (
             df_feat_mean.dropna()[["period", "diff_%"]]
             .rename(columns={"diff_%": a_variable})
             .set_index("period")
             .T
         )
-        df_append_mean = pd.concat([df_append_mean, df_feat_mean], axis=0)
+        df_append_mean = df_append_mean.append(df_feat_mean)
 
         # Preparamos salida y append para la std
         df_feat_std = df_feat_std.set_index("period").T
-        df_append_std = pd.concat([df_append_std, df_feat_std], axis=0)
+        df_append_std = df_append_std.append(df_feat_std)
 
         # generamos info de nulls
         a = df_feat_nulls.groupby("period").agg({"bool": "count"})
         b = df_feat_nulls.groupby("period").agg({"bool": "sum"})
         df_feat_nulls = (b * 100 / a).rename(columns={"bool": a_variable})
 
         # Preparamos salida de nulos
         df_feat_nulls = df_feat_nulls.T
-        df_append_nulls = pd.concat(
-            [df_append_nulls, df_feat_nulls], axis=0
-        )
+        df_append_nulls = df_append_nulls.append(df_feat_nulls)
 
     return df_append_mean, df_append_std, df_append_nulls
```

### Comparing `bcirisktools-0.3.5/bcirisktools/tree_crt.py` & `bcirisktools-0.4/bcirisktools/tree_crt.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,21 +337,17 @@
     # otra el BadRate
     for i, feature in enumerate(summaries.keys()):
         # Utilizamos los resumenes y re-ordenamos según las variables categoricas.
         summary = summaries[feature].copy()
 
         # summary = summaries[feature]
         IV = summary.iloc[-1, :]["IV"]
-        try:
-            df_all = df_all.append(
-                {"Variable": feature, "Information Value": IV}, ignore_index=True
-            ) 
-        except:
-            pd_new_row = pd.DataFrame({"Variable": [feature], "Information Value": [IV]})
-            df_all = pd.concat([df_all,pd_new_row], axis=0).reset_index(drop=True)
+        df_all = df_all.append(
+            {"Variable": feature, "Information Value": IV}, ignore_index=True
+        )
 
         fig1 = px.bar(
             summary.iloc[:-1, :], x="Categoria", y="%BadRate", hover_data=["Categoria"]
         )
         fig2 = px.bar(
             summary.iloc[:-1, :], x="Categoria", y="WoE", hover_data=["Categoria"]
         )
```

### Comparing `bcirisktools-0.3.5/bcirisktools.egg-info/PKG-INFO` & `bcirisktools-0.4/bcirisktools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.3.5
+Version: 0.4
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.3.5/setup.py` & `bcirisktools-0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.3.5"
+VERSION = "0.4"
 DESCRIPTION = "BCI risks tools"
 LONG_DESCRIPTION = "A package that compiles different risk tools used by BCI bank."
 
 # Setting up
 setup(
     name="bcirisktools",
     version=VERSION,
```

