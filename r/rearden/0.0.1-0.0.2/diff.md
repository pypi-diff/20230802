# Comparing `tmp/rearden-0.0.1.tar.gz` & `tmp/rearden-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rearden-0.0.1.tar", last modified: Sat Jul 29 17:29:51 2023, max compression
+gzip compressed data, was "rearden-0.0.2.tar", last modified: Wed Aug  2 20:14:09 2023, max compression
```

## Comparing `rearden-0.0.1.tar` & `rearden-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 17:29:51.358087 rearden-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-06-11 09:15:09.000000 rearden-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3097 2023-07-29 17:29:51.358087 rearden-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      639 2023-07-29 16:45:38.000000 rearden-0.0.1/README.md
--rw-rw-rw-   0        0        0     2101 2023-07-29 16:49:44.000000 rearden-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 17:29:51.358087 rearden-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-29 17:29:51.294630 rearden-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 17:29:51.320286 rearden-0.0.1/src/rearden/
--rw-rw-rw-   0        0        0        0 2023-07-22 16:49:08.000000 rearden-0.0.1/src/rearden/__init__.py
--rw-rw-rw-   0        0        0      443 2023-07-29 09:34:59.000000 rearden-0.0.1/src/rearden/decorators.py
--rw-rw-rw-   0        0        0    18926 2023-07-29 09:28:06.000000 rearden-0.0.1/src/rearden/grid_search.py
--rw-rw-rw-   0        0        0     5367 2023-07-29 09:31:37.000000 rearden-0.0.1/src/rearden/preprocessings.py
--rw-rw-rw-   0        0        0     7033 2023-07-29 09:32:45.000000 rearden-0.0.1/src/rearden/time_series.py
--rw-rw-rw-   0        0        0     5078 2023-07-29 09:33:30.000000 rearden-0.0.1/src/rearden/vizualizations.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:29:51.353319 rearden-0.0.1/src/rearden.egg-info/
--rw-rw-rw-   0        0        0     3097 2023-07-29 17:29:51.000000 rearden-0.0.1/src/rearden.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-29 17:29:51.000000 rearden-0.0.1/src/rearden.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 17:29:51.000000 rearden-0.0.1/src/rearden.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      318 2023-07-29 17:29:51.000000 rearden-0.0.1/src/rearden.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 17:29:51.000000 rearden-0.0.1/src/rearden.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 20:14:09.409834 rearden-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-06-11 09:15:09.000000 rearden-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    13206 2023-08-02 20:14:09.408319 rearden-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10748 2023-08-02 20:10:08.000000 rearden-0.0.2/README.md
+-rw-rw-rw-   0        0        0     2101 2023-08-02 19:43:37.000000 rearden-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 20:14:09.409834 rearden-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 20:14:09.343092 rearden-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 20:14:09.369887 rearden-0.0.2/src/rearden/
+-rw-rw-rw-   0        0        0       23 2023-08-02 19:28:03.000000 rearden-0.0.2/src/rearden/__init__.py
+-rw-rw-rw-   0        0        0      443 2023-07-29 09:34:59.000000 rearden-0.0.2/src/rearden/decorators.py
+-rw-rw-rw-   0        0        0    19189 2023-08-02 19:53:30.000000 rearden-0.0.2/src/rearden/grid_search.py
+-rw-rw-rw-   0        0        0     6870 2023-08-02 19:47:36.000000 rearden-0.0.2/src/rearden/preprocessings.py
+-rw-rw-rw-   0        0        0     8037 2023-08-02 19:51:10.000000 rearden-0.0.2/src/rearden/time_series.py
+-rw-rw-rw-   0        0        0     6146 2023-08-02 19:51:10.000000 rearden-0.0.2/src/rearden/vizualizations.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:14:09.404541 rearden-0.0.2/src/rearden.egg-info/
+-rw-rw-rw-   0        0        0    13206 2023-08-02 20:14:09.000000 rearden-0.0.2/src/rearden.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-08-02 20:14:09.000000 rearden-0.0.2/src/rearden.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 20:14:09.000000 rearden-0.0.2/src/rearden.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      318 2023-08-02 20:14:09.000000 rearden-0.0.2/src/rearden.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 20:14:09.000000 rearden-0.0.2/src/rearden.egg-info/top_level.txt
```

### Comparing `rearden-0.0.1/LICENSE.txt` & `rearden-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rearden-0.0.1/pyproject.toml` & `rearden-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rearden"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name="Sergey Polivin", email="s.polivin@gmail.com"},
 ]
 description = "Library of useful data structures for data preprocessing, vizualizations and grid search"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 requires-python = ">=3.7"
```

### Comparing `rearden-0.0.1/src/rearden/grid_search.py` & `rearden-0.0.2/src/rearden/grid_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import (
     Any,
     Iterable,
     Literal,
     Mapping,
     Optional,
     Sequence,
@@ -488,15 +489,17 @@
         # Print out a summary of all classification metrics if metric=None
         classification_stats = classification_report(
             self.eval_target, self.eval_predictions, target_names=target_names
         )
         print(classification_stats)
 
     def plot_confusion_matrix(
-        self, label_names: Optional[Tuple[str]] = None
+        self,
+        label_names: Optional[Tuple[str]] = None,
+        save_fig: bool = False,
     ) -> Any:
         """Plots a confusion matrix."""
         # Verifying if the grid search has been launched
         self._verify_est_fitted()
 
         # Computing predictions on the test set
         self.eval_predictions = self.predict(self.eval_features)
@@ -510,8 +513,15 @@
         disp.plot(cmap=plt.cm.Blues)
 
         # Selecting last estimator name
         model_name = self._model_name
 
         plt.title(f"Confusion matrix ({model_name})")
         plt.tight_layout()
+
+        if save_fig:
+            dir_name = "images/"
+            if os.path.isdir(dir_name) is False:
+                os.makedirs(dir_name)
+            plt.savefig(dir_name + "confusion_matrix.png")
+
         plt.show()
```

### Comparing `rearden-0.0.1/src/rearden/preprocessings.py` & `rearden-0.0.2/src/rearden/preprocessings.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,14 +60,56 @@
     if num_duplicates != 0:
         data.drop_duplicates(inplace=True)
         print(f"{num_duplicates:,} duplicates found and deleted.")
     else:
         print("No duplicates found.")
 
 
+def filter_data(
+    data: pd.DataFrame,
+    column: str,
+    lower_val: int,
+    upper_val: int,
+    display_changes: bool = False,
+) -> pd.DataFrame:
+    """
+    Filters out values in a specific column
+    of a DataFrame.
+
+    Args:
+        data (pd.DataFrame): DataFrame with information on
+            automobile vehicles.
+        column (str): DataFrame column by which filtering
+            should be done.
+        lower_val (int): The lowest value of the filtering
+            region.
+        upper_val (int): The highest value of the filtering
+            region.
+        display_changes (bool, optional): Boolean indicating
+            displaying changes made to the data. Defaults to False.
+
+    Returns:
+        pd.DataFrame: Object with its values in a
+        specific column filtered out according to
+        `lower_val` and `upper_val`.
+    """
+    filtering_indices = data[column].between(lower_val, upper_val)
+    data_filtered = data[filtering_indices].reset_index(drop=True)
+    if display_changes:
+        data_size_new = data_filtered.shape[0]
+        data_size_old = data.shape[0]
+        filtered_num = data_size_old - data_size_new
+        filtered_share = filtered_num / data_size_old
+        print(f"DataFrame size (prior to filtering): {data_size_old:,}")
+        print(f"DataFrame size (after filtering): {data_size_new:,}")
+        print(f"Objects filtered out: {filtered_num:,} ({filtered_share:.1%})")
+
+    return data_filtered
+
+
 def prepare_sets(
     data: pd.DataFrame,
     target_name: str,
     train_share: float,
     test_share: float,
     valid_share: Optional[float] = None,
     random_state: Optional[int] = None,
```

### Comparing `rearden-0.0.1/src/rearden/time_series.py` & `rearden-0.0.2/src/rearden/time_series.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import Any, Optional, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from sklearn.base import BaseEstimator, TransformerMixin
@@ -145,14 +146,18 @@
 
 def plot_time_series(
     data: pd.DataFrame,
     col: str,
     period_start: str,
     period_end: str,
     kind: Optional[str] = None,
+    save_fig: bool = False,
+    figure_dims: Tuple[int] = (8, 10),
+    title_name: str = "title_name",
+    ylabel_name: str = "ylabel_name",
 ) -> Any:
     """Plots time series.
 
     When specifying kind="decomposed", conducts seasonal decomposition
     of the data and outputs graphs of trend, seasonal and residual
     components.
 
@@ -161,60 +166,82 @@
             about taxi orders.
         col (str): DataFrame column containing
             data about taxi orders.
         period_start (str): Time period start.
         period_end (str): Time period end.
         kind (Optional[str], optional): Boolean indicator
             of performing time-series decomposition.
+        save_fig (bool, optional): Boolean indicating saving the figure
+            in a separate directory. Defaults to False.
+        figure_dims (Tuple[int], optional): Dimensions of the figure.
+            Defaults to (8, 10).
+        title_name (str, optional): Title of the plot if kind is None.
+            Defaults to "title_name".
+        ylabel_name (str, optional): Name of the ylabel on the plot.
+            Defaults to "ylabel_name".
     """
     # Plotting decomposed time series
     if kind == "decomposed":
         decomposed = seasonal_decompose(data)
 
-        plt.figure(figsize=(8, 10))
+        plt.figure(figsize=figure_dims)
 
         # Trend component
         plt.subplot(311)
         trend_plot = sns.lineplot(
             data=decomposed.trend[period_start:period_end], ax=plt.gca()
         )
-        trend_plot.set(title="Trend", xlabel="Time period", ylabel="Orders")
+        trend_plot.set(title="Trend", xlabel="Time period", ylabel=ylabel_name)
         plt.xticks(rotation=45)
 
         # Seasonal component
         plt.subplot(312)
         seasonal_plot = sns.lineplot(
             data=decomposed.seasonal[period_start:period_end], ax=plt.gca()
         )
         seasonal_plot.set(
-            title="Seasonality", xlabel="Time period", ylabel="Orders"
+            title="Seasonality", xlabel="Time period", ylabel=ylabel_name
         )
         plt.xticks(rotation=45)
 
         # Residual component
         plt.subplot(313)
         residual_plot = sns.lineplot(
             data=decomposed.resid[period_start:period_end], ax=plt.gca()
         )
         residual_plot.set(
-            title="Residual", xlabel="Time period", ylabel="Orders"
+            title="Residual", xlabel="Time period", ylabel=ylabel_name
         )
         plt.xticks(rotation=45)
 
         plt.tight_layout()
+
+        if save_fig:
+            dir_name = "images/"
+            if os.path.isdir(dir_name) is False:
+                os.makedirs(dir_name)
+            plt.savefig(dir_name + "ts_decomposed.png")
+
         plt.show()
 
         return
 
     # Plotting time series
     full_data_plot = sns.lineplot(
         data=data[period_start:period_end],
         y=col,
         x=data[period_start:period_end].index,
         ax=plt.gca(),
     )
     full_data_plot.set(
-        title="Taxi orders number", xlabel="Time period", ylabel="Orders"
+        title=title_name, xlabel="Time period", ylabel=ylabel_name
     )
     plt.xticks(rotation=45)
     plt.tight_layout()
+
+    if save_fig:
+        dir_name = "images/"
+        if os.path.isdir(dir_name) is False:
+            os.makedirs(dir_name)
+        plt.savefig(dir_name + "ts_plot.png")
+
     plt.show()
```

### Comparing `rearden-0.0.1/src/rearden/vizualizations.py` & `rearden-0.0.2/src/rearden/vizualizations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import Any, Optional, Sequence, Tuple
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
@@ -12,14 +13,15 @@
     title_name: str = "title_name",
     dot_size: int = 150,
     figure_dims: Tuple[int] = (15, 7),
     xticks_fontsize: int = 15,
     yticks_fontsize: int = 12,
     title_fontsize: int = 20,
     ylabel_fontsize: int = 15,
+    save_fig: bool = False,
 ) -> Any:
     """Provides models performance vizualization.
 
     Generates a scatterplot with model names and their
     respective metric values for comparison.
 
     Args:
@@ -37,14 +39,16 @@
             Defaults to 15.
         yticks_fontsize (int, optional): Size of yticks on the plot.
             Defaults to 12.
         title_fontsize (int, optional): Size of the title of the plot.
             Defaults to 20.
         ylabel_fontsize (int, optional): Size of the Y-label.
             Defaults to 15.
+        save_fig (bool, optional): Boolean indicating saving the plot
+            in a separate directory. Defaults to False.
     """
     # Separating scores from a sequence of tuples passed
     _, scores = zip(*results)
     # Joining model names with scores
     names_with_scores = ["%s\n%.4f" % (name, loss) for name, loss in results]
 
     # Making a plot
@@ -58,23 +62,32 @@
     plt.yticks(fontsize=yticks_fontsize)
 
     plt.title(title_name, fontsize=title_fontsize)
     plt.ylabel(metric_name, fontsize=ylabel_fontsize)
 
     plt.tight_layout()
 
+    if save_fig:
+        dir_name = "images/"
+        if os.path.isdir(dir_name) is False:
+            os.makedirs(dir_name)
+        plt.savefig(dir_name + "model_comparison.png")
+
+    plt.show()
+
 
 def plot_corr_heatmap(
     data: pd.DataFrame,
     target_var: Optional[pd.Series] = None,
     annotation: bool = False,
     annot_num_size: Optional[int] = None,
     heatmap_coloring: Optional[Any] = None,
     upper_triangle: bool = False,
     lower_triangle: bool = False,
+    save_fig: bool = False,
 ) -> Any:
     """Plots a heatmap for the correlation matrix.
 
     Args:
         data (pd.DataFrame): DataFrame for which a heatmap needs
             to be plotted.
         target_var (Optional[pd.Series], optional): Vector with a
@@ -86,14 +99,16 @@
             figures inside the plot. Defaults to None.
         heatmap_coloring (Optional[Any], optional): Heatmap colormap.
             Defaults to None.
         upper_triangle (bool, optional): Boolean indicator of displaying
             only the upper triangle of the matrix. Defaults to False.
         lower_triangle (bool, optional): Boolean indicator of displaying
             only the lower triangle of the matrix. Defaults to False.
+        save_fig (bool, optional): Boolean indicating saving the figure
+            in a separate directory. Defaults to False.
     """
     if target_var is not None:
         data = pd.concat([data, target_var], axis=1)
 
     corr_matrix = data.corr()
 
     # Showing upper/lower triangle of a matrix
@@ -113,35 +128,52 @@
         mask=mask,
         annot_kws={"size": annot_num_size},
         cmap=heatmap_coloring,
     )
     corr_heatmap.xaxis.tick_bottom()
     corr_heatmap.yaxis.tick_left()
     corr_heatmap.set(title="Correlation matrix heatmap")
+
+    if save_fig:
+        dir_name = "images/"
+        if os.path.isdir(dir_name) is False:
+            os.makedirs(dir_name)
+        plt.savefig(dir_name + "corr_mat_heatmap.png")
+
     plt.show()
 
 
 def plot_class_structure(
     target_var: pd.Series,
     xlabel_name: str = "xlabel_name",
     ylabel_name: str = "ylabel_name",
     title_name: str = "title_name",
+    save_fig: bool = False,
 ) -> Any:
     """Plots the structure of the target variable.
 
     Args:
         target_var (pd.Series): Target vector.
         xlabel_name (str, optional): Name of the xlabel on the plot.
             Defaults to "xlabel_name".
         ylabel_name (str, optional): Name of the ylabel on the plot.
             Defaults to "ylabel_name".
         title_name (str, optional): Title of the plot.
             Defaults to "title_name".
+        save_fig (bool, optional): Boolean indicating saving the figure
+            in a separate directory. Defaults to False.
     """
     target_var.value_counts(normalize=True).plot(
         kind="bar",
         xlabel=xlabel_name,
         ylabel=ylabel_name,
         title=title_name,
     )
     plt.xticks(rotation=0)
+
+    if save_fig:
+        dir_name = "images/"
+        if os.path.isdir(dir_name) is False:
+            os.makedirs(dir_name)
+        plt.savefig(dir_name + "class_structure.png")
+
     plt.show()
```

