# Comparing `tmp/ehrapy-0.4.0.tar.gz` & `tmp/ehrapy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehrapy-0.4.0.tar", max compression
+gzip compressed data, was "ehrapy-0.5.0.tar", max compression
```

## Comparing `ehrapy-0.4.0.tar` & `ehrapy-0.5.0.tar`

### file list

```diff
@@ -1,45 +1,51 @@
--rw-r--r--   0        0        0    11310 2023-06-06 12:43:14.081286 ehrapy-0.4.0/LICENSE
--rw-r--r--   0        0        0     2316 2023-06-06 12:43:14.081286 ehrapy-0.4.0/README.md
--rw-r--r--   0        0        0     1539 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/SCANPY_LICENSE
--rw-r--r--   0        0        0      668 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/__init__.py
--rw-r--r--   0        0        0    15880 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/_settings.py
--rw-r--r--   0        0        0      259 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/anndata/__init__.py
--rw-r--r--   0        0        0    35753 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/anndata/anndata_ext.py
--rw-r--r--   0        0        0        0 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/core/__init__.py
--rw-r--r--   0        0        0     1091 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/core/_tool_available.py
--rw-r--r--   0        0        0     2271 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/core/meta_information.py
--rw-r--r--   0        0        0      509 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/data/__init__.py
--rw-r--r--   0        0        0     2283 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/data/_dataloader.py
--rw-r--r--   0        0        0    22780 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/data/_datasets.py
--rw-r--r--   0        0        0      109 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/io/__init__.py
--rw-r--r--   0        0        0    33563 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/io/_read.py
--rw-r--r--   0        0        0      676 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/io/_utility_io.py
--rw-r--r--   0        0        0     3192 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/io/_write.py
--rw-r--r--   0        0        0     6614 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/logging.py
--rw-r--r--   0        0        0      265 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/plot/__init__.py
--rw-r--r--   0        0        0    10390 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/plot/_missingno_pl_api.py
--rw-r--r--   0        0        0     2191 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/plot/_qc.py
--rw-r--r--   0        0        0   101572 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/plot/_scanpy_pl_api.py
--rw-r--r--   0        0        0    10214 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/plot/_survival_analysis.py
--rw-r--r--   0        0        0      795 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/plot/_util.py
--rw-r--r--   0        0        0      855 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/__init__.py
--rw-r--r--   0        0        0    47405 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_data_imputation.py
--rw-r--r--   0        0        0    46268 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_encode.py
--rw-r--r--   0        0        0     2825 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_highly_variable_features.py
--rw-r--r--   0        0        0    16013 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_normalization.py
--rw-r--r--   0        0        0     4299 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_outliers.py
--rw-r--r--   0        0        0    17121 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_quality_control.py
--rw-r--r--   0        0        0    11810 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/_scanpy_pp_api.py
--rw-r--r--   0        0        0    29649 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/preprocessing/laboratory_reference_tables/laposata.tsv
--rw-r--r--   0        0        0        0 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/py.typed
--rw-r--r--   0        0        0      437 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/__init__.py
--rw-r--r--   0        0        0    11546 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/_sa.py
--rw-r--r--   0        0        0    49254 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/_scanpy_tl_api.py
--rw-r--r--   0        0        0        0 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/nlp/__init__.py
--rw-r--r--   0        0        0     3911 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/nlp/_hpo.py
--rw-r--r--   0        0        0    17561 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/nlp/_medcat.py
--rw-r--r--   0        0        0    19793 2023-06-06 12:43:14.117285 ehrapy-0.4.0/ehrapy/tools/nlp/_translators.py
--rw-r--r--   0        0        0        0 2023-06-06 12:43:14.121285 ehrapy-0.4.0/ehrapy/util/__init__.py
--rw-r--r--   0        0        0    14707 2023-06-06 12:43:14.121285 ehrapy-0.4.0/ehrapy/util/_doc_util.py
--rw-r--r--   0        0        0     3791 2023-06-06 12:43:14.121285 ehrapy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 ehrapy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11310 2023-08-02 10:36:30.261629 ehrapy-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2316 2023-08-02 10:36:30.261629 ehrapy-0.5.0/README.md
+-rw-r--r--   0        0        0     1539 2023-08-02 10:36:30.289629 ehrapy-0.5.0/ehrapy/SCANPY_LICENSE
+-rw-r--r--   0        0        0      543 2023-08-02 10:36:30.289629 ehrapy-0.5.0/ehrapy/__init__.py
+-rw-r--r--   0        0        0    15880 2023-08-02 10:36:30.289629 ehrapy-0.5.0/ehrapy/_settings.py
+-rw-r--r--   0        0        0      259 2023-08-02 10:36:30.289629 ehrapy-0.5.0/ehrapy/anndata/__init__.py
+-rw-r--r--   0        0        0    34434 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/anndata/anndata_ext.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/core/__init__.py
+-rw-r--r--   0        0        0     1091 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/core/_tool_available.py
+-rw-r--r--   0        0        0     2271 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/core/meta_information.py
+-rw-r--r--   0        0        0      509 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/data/__init__.py
+-rw-r--r--   0        0        0     3349 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/data/_dataloader.py
+-rw-r--r--   0        0        0    22812 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/data/_datasets.py
+-rw-r--r--   0        0        0      109 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/io/__init__.py
+-rw-r--r--   0        0        0    31558 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/io/_read.py
+-rw-r--r--   0        0        0      676 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/io/_utility_io.py
+-rw-r--r--   0        0        0     3192 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/io/_write.py
+-rw-r--r--   0        0        0     6614 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/logging.py
+-rw-r--r--   0        0        0      327 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/plot/__init__.py
+-rw-r--r--   0        0        0    10390 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/plot/_missingno_pl_api.py
+-rw-r--r--   0        0        0     2191 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/plot/_qc.py
+-rw-r--r--   0        0        0   101572 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/plot/_scanpy_pl_api.py
+-rw-r--r--   0        0        0    10214 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/plot/_survival_analysis.py
+-rw-r--r--   0        0        0      795 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/plot/_util.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/plot/causal_inference/__init__.py
+-rw-r--r--   0        0        0     2630 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/plot/causal_inference/_dowhy.py
+-rw-r--r--   0        0        0      855 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/preprocessing/__init__.py
+-rw-r--r--   0        0        0    47405 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/preprocessing/_data_imputation.py
+-rw-r--r--   0        0        0    39831 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/preprocessing/_encode.py
+-rw-r--r--   0        0        0     2825 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/preprocessing/_highly_variable_features.py
+-rw-r--r--   0        0        0    16226 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/preprocessing/_normalization.py
+-rw-r--r--   0        0        0     4299 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/preprocessing/_outliers.py
+-rw-r--r--   0        0        0    17121 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/preprocessing/_quality_control.py
+-rw-r--r--   0        0        0    11810 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/preprocessing/_scanpy_pp_api.py
+-rw-r--r--   0        0        0    29649 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/preprocessing/laboratory_reference_tables/laposata.tsv
+-rw-r--r--   0        0        0        0 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/py.typed
+-rw-r--r--   0        0        0      449 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/tools/__init__.py
+-rw-r--r--   0        0        0      604 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/tools/_method_options.py
+-rw-r--r--   0        0        0    11546 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/tools/_sa.py
+-rw-r--r--   0        0        0    44404 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/tools/_scanpy_tl_api.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/tools/causal/__init__.py
+-rw-r--r--   0        0        0    13113 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/tools/causal/_dowhy.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/tools/feature_ranking/__init__.py
+-rw-r--r--   0        0        0    17489 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/tools/feature_ranking/_rank_features_groups.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/tools/nlp/__init__.py
+-rw-r--r--   0        0        0    17561 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/tools/nlp/_medcat.py
+-rw-r--r--   0        0        0    19793 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/tools/nlp/_translators.py
+-rw-r--r--   0        0        0        0 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/util/__init__.py
+-rw-r--r--   0        0        0    14707 2023-08-02 10:36:30.293629 ehrapy-0.5.0/ehrapy/util/_doc_util.py
+-rw-r--r--   0        0        0     3634 2023-08-02 10:36:30.297629 ehrapy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4010 1970-01-01 00:00:00.000000 ehrapy-0.5.0/PKG-INFO
```

### Comparing `ehrapy-0.4.0/LICENSE` & `ehrapy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/README.md` & `ehrapy-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/SCANPY_LICENSE` & `ehrapy-0.5.0/ehrapy/SCANPY_LICENSE`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/_settings.py` & `ehrapy-0.5.0/ehrapy/_settings.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/anndata/anndata_ext.py` & `ehrapy-0.5.0/ehrapy/anndata/anndata_ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 import random
 from collections import OrderedDict
 from string import ascii_letters
-from typing import Collection, Iterable, NamedTuple
+from typing import Collection, Iterable, NamedTuple, Sequence
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData, concat
-from mudata import MuData
 from rich import print
 from rich.text import Text
 from rich.tree import Tree
 from scanpy.get import obs_df, rank_genes_groups_df, var_df
 from scipy import sparse
 from scipy.sparse import issparse
 
@@ -313,15 +312,15 @@
         logg.info(f"Added `{cols_not_in_x}` features to `X`.")
     else:
         new_adata = adata
 
     return new_adata
 
 
-def get_column_indices(adata: AnnData, col_names: str | list[str]) -> list[int]:
+def get_column_indices(adata: AnnData, col_names: str | Sequence[str]) -> list[int]:
     """Fetches the column indices in X for a given list of column names
 
     Args:
         adata: :class:`~anndata.AnnData` object
         col_names: Column names to extract the indices for
 
     Returns:
@@ -352,39 +351,35 @@
 
     Returns:
         :class:`~numpy.ndarray` object containing the column values
     """
     return np.take(adata.X, indices, axis=1)
 
 
-def type_overview(
-    data: MuData | AnnData, sort_by: str | None = None, sort_reversed: bool = False
-) -> None:  # pragma: no cover
-    """Prints the current state of an :class:`~anndata.AnnData` or :class:`~mudata.MuData` object in a tree format.
+def type_overview(data: AnnData, sort_by: str | None = None, sort_reversed: bool = False) -> None:  # pragma: no cover
+    """Prints the current state of an :class:`~anndata.AnnData` object in a tree format.
 
     Output could be printed in sorted format by using one of `dtype`, `order`, `num_cats` or `None`, which sorts by data type, lexicographical order,
     number of unique values (excluding NaN's) and unsorted respectively. Note that sorting by `num_cats` only affects
     encoded variables currently and will display unencoded vars unsorted.
 
     Args:
-        data: :class:`~anndata.AnnData` or :class:`~mudata.MuData` object to display
+        data: :class:`~anndata.AnnData` object to display
         sort_by: How the tree output should be sorted. One of `dtype`, `order`, `num_cats` or None (Defaults to None -> unsorted)
         sort_reversed: Whether to sort in reversed order or not
 
     Examples:
         >>> import ehrapy as ep
         >>> adata = ep.dt.mimic_2(encoded=True)
         >>> ep.ad.type_overview(adata)
     """
     if isinstance(data, AnnData):
         _adata_type_overview(data, sort_by, sort_reversed)
-    elif isinstance(data, MuData):
-        _mudata_type_overview(data, sort_by, sort_reversed)
     else:
-        raise ValueError(f"Unable to present object of type {type(data)}. Can only display AnnData or MuData objects!")
+        raise ValueError(f"Unable to present object of type {type(data)}. Can only display AnnData objects!")
 
 
 def _adata_type_overview(
     adata: AnnData, sort_by: str | None = None, sort_reversed: bool = False
 ) -> None:  # pragma: no cover
     """Display the :class:`~anndata.AnnData object in its current state (encoded and unencoded variables, obs)
 
@@ -446,41 +441,14 @@
     if sort_by:
         logg.info(
             "Displaying AnnData object in sorted mode. Note that this might not be the exact same order of the variables in X or var are stored!"
         )
     print(tree)
 
 
-def _mudata_type_overview(
-    mudata: MuData, sort: str | None = None, sort_reversed: bool = False
-) -> None:  # pragma: no cover
-    """Display the :class:`~mudata.MuData object in its current state (:class:`~anndata.AnnData objects with obs, shapes)
-
-    Args:
-        mudata: The :class:`~mudata.MuData object to display
-        sort: Whether to sort output or not
-        sort_reversed: Whether to sort output in reversed order or not
-    """
-    tree = Tree(
-        f"[b green]Variable names for AnnData object with {len(mudata.obs_names)} obs, {len(mudata.var_names)} vars and {len(mudata.mod.keys())} modalities\n",
-        guide_style="underline2 bright_blue",
-    )
-
-    modalities = sorted(list(mudata.mod.keys()), reverse=sort_reversed) if sort else list(mudata.mod.keys())
-    for mod in modalities:
-        branch = tree.add(
-            f"[b green]{mod}: [not b blue]n_vars x n_obs: {mudata.mod[mod].n_vars} x {mudata.mod[mod].n_obs}"
-        )
-        branch.add(
-            f"[blue]obs: [black]{', '.join(f'{_single_quote_string(col_name)}' for col_name in mudata.mod[mod].obs.columns)}"
-        )
-        branch.add(f"[blue]layers: [black]{', '.join(layer for layer in mudata.mod[mod].layers)}\n")
-    print(tree)
-
-
 def _sort_by_order_or_none(adata: AnnData, branch, var_names: list[str]):
     """Add branches to tree for sorting by order or unsorted."""
     var_names_val = list(adata.var_names.values)
     for other_vars in var_names:
         if not other_vars.startswith("ehrapycat"):
             idx = var_names_val.index(other_vars)
             unique_categoricals = pd.unique(adata.X[:, idx : idx + 1].flatten())
@@ -537,30 +505,33 @@
         adata: :class:`~anndata.AnnData` object
 
     Returns:
         List of column numeric column names
     """
     _assert_encoded(adata)
 
-    return adata.uns["numerical_columns"]
+    if "numerical_columns" not in adata.uns_keys():
+        return list(adata.var_names.values)
+    else:
+        return adata.uns["numerical_columns"]
 
 
-def assert_numeric_vars(adata: AnnData, vars: list[str]):
+def assert_numeric_vars(adata: AnnData, vars: Sequence[str]):
     num_vars = get_numeric_vars(adata)
 
     try:
         assert set(vars) <= set(num_vars)
     except AssertionError:
         raise ValueError("Some selected vars are not numeric")
 
 
 def set_numeric_vars(
-    adata: AnnData, values: np.ndarray, vars: list[str] | None = None, copy: bool = False
+    adata: AnnData, values: np.ndarray, vars: Sequence[str] | None = None, copy: bool = False
 ) -> AnnData | None:
-    """Sets the column names for numeric variables in X.
+    """Sets the numeric values in given column names in X.
 
     Args:
         adata: :class:`~anndata.AnnData` object
         values: Matrix containing the replacement values
         vars: List of names of the numeric variables to replace. If `None` they will be detected using :func:`~ehrapy.preprocessing.get_numeric_vars`.
         copy: Whether to return a copy with the normalized data.
 
@@ -571,30 +542,30 @@
 
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
         assert_numeric_vars(adata, vars)
 
     if not np.issubdtype(values.dtype, np.number):
-        raise TypeError(f"values must be numeric (current dtype is {values.dtype})")
+        raise TypeError(f"Values must be numeric (current dtype is {values.dtype})")
 
     n_values = values.shape[1]
 
     if n_values != len(vars):
         raise ValueError(f"Number of values ({n_values}) does not match number of vars ({len(vars)})")
 
     if copy:
         adata = adata.copy()
 
     vars_idx = get_column_indices(adata, vars)
 
     for i in range(n_values):
         adata.X[:, vars_idx[i]] = values[:, i]
 
-    logg.info(f"Column names for numeric variables {vars} were replaced by {values}.")
+    logg.info(f"Values in columns {vars} were replaced by {values}.")
 
     return adata
 
 
 def _update_uns(
     adata: AnnData, moved_columns: list[str], to_x: bool = False
 ) -> tuple[list[str], list[str], list[str] | None]:
@@ -768,15 +739,15 @@
     obsp = dict(array=np.random.random((M, M)), sparse=sparse.random(M, M, format="csr"))
     varp = dict(array=np.random.random((N, N)), sparse=sparse.random(N, N, format="csr"))
 
     def _generate_vstr_recarray(m, n, dtype=None):
         size = m * n
         lengths = np.random.randint(3, 5, size)
         letters = np.array(list(ascii_letters))
-        gen_word = lambda l: "".join(np.random.choice(letters, l))
+        gen_word = lambda w: "".join(np.random.choice(letters, w))
         arr = np.array([gen_word(length) for length in lengths]).reshape(m, n)
 
         return pd.DataFrame(arr, columns=[gen_word(5) for _ in range(n)]).to_records(index=False, column_dtypes=dtype)
 
     uns = dict(
         O_recarray=_generate_vstr_recarray(N, 5),
         nested=dict(
```

### Comparing `ehrapy-0.4.0/ehrapy/core/_tool_available.py` & `ehrapy-0.5.0/ehrapy/core/_tool_available.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/core/meta_information.py` & `ehrapy-0.5.0/ehrapy/core/meta_information.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/data/_datasets.py` & `ehrapy-0.5.0/ehrapy/data/_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,17 +85,17 @@
         >>> import ehrapy as ep
         >>> dfs = ep.dt.mimic_3_demo()
     """
     data = read_csv(
         dataset_path=f"{ehrapy_settings.datasetdir}/ehrapy_mimic_3",
         download_dataset_name="ehrapy_mimic_3",
         backup_url="https://physionet.org/static/published-projects/mimiciii-demo/mimic-iii-clinical-database-demo-1.4.zip",
-        return_mudata=False,
         return_dfs=False if anndata else True,
         columns_obs_only=columns_obs_only,
+        archive_format="zip",
     )
     if encoded:
         if not anndata:
             raise ValueError("Can only encode AnnData objects. Set 'anndata=True' to get AnnData objects.")
         encode(data, autodetect=True)
 
     return data
@@ -627,15 +627,15 @@
     return adata
 
 
 def synthea_1k_sample(
     encoded: bool = False,
     columns_obs_only: list[str] | None = None,
 ) -> AnnData:
-    """Loads the 1K Sample Synthetic Patient Records Data Set
+    """Loads the 1K Sample Synthetic Patient Records Data Set.
 
     More details: https://synthea.mitre.org/downloads
     Preprocessing: TODO: add preprocessing link
 
     Args:
         encoded: Whether to return an already encoded object.
         columns_obs_only: Columns to include in obs only and not X.
@@ -649,13 +649,14 @@
     """
     adata: AnnData = read_fhir(
         dataset_path=f"{ehrapy_settings.datasetdir}/synthea_sample",
         download_dataset_name="synthea_sample",
         backup_url="https://synthetichealth.github.io/synthea-sample-data/downloads/synthea_sample_data_fhir_dstu2_sep2019.zip",
         columns_obs_only=columns_obs_only,
         index_column="id",
+        archive_format="zip",
     )
 
     if encoded:
         return encode(adata, autodetect=True)
 
     return adata
```

### Comparing `ehrapy-0.4.0/ehrapy/io/_read.py` & `ehrapy-0.5.0/ehrapy/io/_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,120 +1,116 @@
 from __future__ import annotations
 
-import shutil
 from pathlib import Path
 from typing import Iterator, Literal
 
 import fhiry.parallel as fp
 import numpy as np
 import pandas as pd
 from _collections import OrderedDict
 from anndata import AnnData
 from anndata import read as read_h5
-from mudata import MuData
 from rich import print
 
 from ehrapy import ehrapy_settings, settings
 from ehrapy.anndata.anndata_ext import df_to_anndata
-from ehrapy.data._dataloader import download
+from ehrapy.data._dataloader import download, remove_archive_extension
 from ehrapy.preprocessing._encode import encode
 
 
 def read_csv(
     dataset_path: Path | str,
     sep: str = ",",
     index_column: dict[str, str | int] | str | int | None = None,
     columns_obs_only: dict[str, list[str]] | list[str] | None = None,
     columns_x_only: dict[str, list[str]] | list[str] | None = None,
     return_dfs: bool = False,
-    return_mudata: bool = False,
     cache: bool = False,
     backup_url: str | None = None,
     download_dataset_name: str | None = None,
+    archive_format: Literal["zip", "tar", "tar.gz", "tgz"] = None,
     **kwargs,
-) -> AnnData | dict[str, AnnData] | MuData:
+) -> AnnData | dict[str, AnnData]:
     """Reads or downloads a desired directory of csv/tsv files or a single csv/tsv file.
 
     Args:
         dataset_path: Path to the file or directory to read.
         sep: Separator in the file. One of either , (comma) or \t (tab). Defaults to , (comma)
         index_column: The index column of obs. Usually the patient visit ID or the patient ID.
         columns_obs_only: These columns will be added to obs only and not X.
         columns_x_only: These columns will be added to X only and all remaining columns to obs.
                         Note that datetime columns will always be added to .obs though.
         return_dfs: Whether to return one or several Pandas DataFrames.
-        return_mudata: Whether to create and return a MuData object.
-                       This is primarily used for complex datasets which require several AnnData files.
         cache: Whether to write to cache when reading or not. Defaults to False .
-        download_dataset_name: Name of the file or directory in case the dataset is downloaded.
-        backup_url: URL to download the data file(s) from if not yet existing.
+        download_dataset_name: Name of the file or directory after download.
+        backup_url: URL to download the data file(s) from, if the dataset is not yet on disk.
+        is_archive: Whether the downloaded file is an archive.
 
     Returns:
-        An :class:`~anndata.AnnData` object, a :class:`~mudata.MuData` object or a dict with an identifier (the filename, without extension)
+        An :class:`~anndata.AnnData` object or a dict with an identifier (the filename, without extension)
         for each :class:`~anndata.AnnData` object in the dict
 
     Examples:
         >>> import ehrapy as ep
         >>> adata = ep.io.read_csv("myfile.csv")
     """
     _check_columns_only_params(columns_obs_only, columns_x_only)
-    file: Path = Path(dataset_path)
-    if not file.exists():
-        file = _get_non_existing_files(file, download_dataset_name, backup_url)
+    dataset_path = Path(dataset_path)
+    if not dataset_path.exists():
+        dataset_path = _get_non_existing_files(dataset_path, download_dataset_name, backup_url, archive_format)
 
     adata = _read_csv(
-        file_path=file,
+        file_path=dataset_path,
         sep=sep,
         index_column=index_column,
         columns_obs_only=columns_obs_only,
         columns_x_only=columns_x_only,
         return_dfs=return_dfs,
-        return_mudata=return_mudata,
         cache=cache,
         **kwargs,
     )
     return adata
 
 
 def _read_csv(
     file_path: Path,
     sep: str,
     index_column: dict[str, str | int] | str | int | None,
     columns_obs_only: dict[str, list[str]] | list[str] | None,
     columns_x_only: dict[str, list[str]] | list[str] | None,
     return_dfs: bool = False,
-    return_mudata: bool = False,
     cache: bool = False,
     **kwargs,
-) -> AnnData | dict[str, AnnData] | MuData:
+) -> AnnData | dict[str, AnnData]:
     """Internal interface of the read_csv method."""
-    if cache and (return_mudata or return_dfs):
-        raise CachingNotSupported("Caching is currently not supported for MuData or Pandas DataFrame objects.")
+    if cache and return_dfs:
+        raise CachingNotSupported("Caching is currently not supported for Pandas DataFrame objects.")
     if return_dfs and (columns_x_only or columns_obs_only):
         raise Warning(
             "Parameters columns_x_only and columns_obs_only are not supported when returning Pandas DataFrames."
         )
+
     path_cache = settings.cachedir / file_path
     # reading from (cache) file is separated in the read_h5ad function
     if cache and (path_cache.is_dir() or path_cache.is_file()):
         raise CacheExistsException(
             f"{path_cache} already exists. Use the read_h5ad function instead to read from cache!"
         )
+
     # If the the file path is a directory, assume it is a dataset with multiple files
     elif file_path.is_dir():
         return _read_from_directory(
             file_path,
             cache,
             path_cache,
             extension=sep,
             index_column=index_column,
             columns_obs_only=columns_obs_only,
             columns_x_only=columns_x_only,
             return_dfs=return_dfs,
-            return_mudata=return_mudata,  # type: ignore
         )
     # input is a single file
     else:
         if sep not in {",", "\t"}:
             raise ValueError("Please provide one of the available separators , or tab")
         adata, columns_obs_only = _do_read_csv(
             file_path, sep, index_column, columns_obs_only, columns_x_only, cache, **kwargs  # type: ignore
@@ -127,15 +123,16 @@
         return adata
 
 
 def read_h5ad(
     dataset_path: Path | str,
     backup_url: str | None = None,
     download_dataset_name: str | None = None,
-) -> AnnData | dict[str, AnnData] | MuData:
+    archive_format: Literal["zip", "tar", "tar.gz", "tgz"] = None,
+) -> AnnData | dict[str, AnnData]:
     """Reads or downloads a desired directory of h5ad files or a single h5ad file.
 
     Args:
         dataset_path: Path to the file or directory to read.
         download_dataset_name: Name of the file or directory in case the dataset is downloaded
         backup_url: URL to download the data file(s) from if not yet existing.
 
@@ -147,15 +144,15 @@
         >>> import ehrapy as ep
         >>> adata = ep.dt.mimic_2(encoded=True)
         >>> ep.io.write("mimic_2.h5ad", adata)
         >>> adata_2 = ep.io.read_h5ad("mimic_2.h5ad")
     """
     file_path: Path = Path(dataset_path)
     if not file_path.exists():
-        file_path = _get_non_existing_files(file_path, download_dataset_name, backup_url)
+        file_path = _get_non_existing_files(file_path, download_dataset_name, backup_url, archive_format=archive_format)
 
     if file_path.is_dir():
         adata = _read_from_directory(file_path, False, None, "h5ad")
     else:
         adata = _do_read_h5ad(file_path)
 
     return adata
@@ -166,29 +163,27 @@
     cache: bool,
     path_cache_dir: Path | None,
     extension: str,
     index_column: dict[str, str | int] | str | int | None = None,
     columns_obs_only: dict[str, list[str]] | list[str] | None = None,
     columns_x_only: dict[str, list[str]] | list[str] | None = None,
     return_dfs: bool = False,
-    return_mudata: bool = False,
 ) -> dict[str, AnnData] | dict[str, pd.DataFrame]:
     """Parse AnnData objects or Pandas DataFrames from a directory containing the data files"""
     if return_dfs:
         dfs = _read_multiple_csv(file_path, sep=extension, return_dfs=True)
         return dfs  # type: ignore
     if extension in {",", "\t"}:
         adata_objects, columns_obs_only = _read_multiple_csv(  # type: ignore
             file_path,
             sep=extension,
             index_column=index_column,
             columns_obs_only=columns_obs_only,
             columns_x_only=columns_x_only,
             return_dfs=False,
-            return_mudata=return_mudata,
         )
         # cache results
         if cache:
             if not path_cache_dir.parent.is_dir():
                 path_cache_dir.parent.mkdir(parents=True)
             path_cache_dir.mkdir()
             return _write_cache_dir(adata_objects, path_cache_dir, columns_obs_only, index_column)  # type: ignore
@@ -202,71 +197,59 @@
 def _read_multiple_csv(  # noqa: N802
     file_path: Path,
     sep: str,
     index_column: dict[str, str | int] | str | int | None = None,
     columns_obs_only: dict[str, list[str]] | list[str] | None = None,
     columns_x_only: dict[str, list[str]] | list[str] | None = None,
     return_dfs: bool = False,
-    return_mudata_object: bool = False,
     cache: bool = False,
     **kwargs,
-) -> tuple[dict[str, AnnData], dict[str, list[str] | None]] | MuData | dict[str, pd.DataFrame]:
+) -> tuple[dict[str, AnnData], dict[str, list[str] | None]] | dict[str, pd.DataFrame]:
     """Read a dataset containing multiple .csv/.tsv files.
 
     Args:
         file_path: File path to the directory containing multiple .csv/.tsv files.
         sep: Either , or \t to determine which files to read.
         index_column: Column names of the index columns for obs
         columns_obs_only: List of columns per file (AnnData object) which should only be stored in .obs, but not in X. Useful for free text annotations.
         columns_x_only: List of columns per file (AnnData object) which should only be stored in .X, but not in obs. Datetime columns will be added to .obs regardless.
         return_dfs: When set to True, return a dictionary of Pandas DataFrames.
-        return_mudata_object: When set to True, return a :class:`~mudata.MuData` object, otherwise a dict of :class:`~anndata.AnnData` objects
         cache: Whether to cache results or not
         kwargs: Keyword arguments for Pandas read_csv
 
     Returns:
-        An :class:`~mudata.MuData` object or a dict mapping the filename (object name) to the corresponding :class:`~anndata.AnnData` object and the columns
+        A Dict mapping the filename (object name) to the corresponding :class:`~anndata.AnnData` object and the columns
         that are obs only for each object
     """
     obs_only_all = {}
-    if not return_mudata_object and not return_dfs:
-        anndata_dict = {}
-    elif return_dfs:
+    if return_dfs:
         df_dict: dict[str, pd.DataFrame] = {}
-    elif return_mudata_object:
-        mudata = None
+    else:
+        anndata_dict = {}
+
     for file in file_path.iterdir():
         if file.is_file() and file.suffix in {".csv", ".tsv"}:
             # slice off the file suffix .csv or .tsv for a clean file name
             file_identifier = file.name[:-4]
             if return_dfs:
                 df = pd.read_csv(file, sep=sep, **kwargs)
                 df_dict[file_identifier] = df
                 continue
 
             index_col, col_obs_only, col_x_only = _extract_index_and_columns_obs_only(
                 file_identifier, index_column, columns_obs_only, columns_x_only
             )
             adata, single_adata_obs_only = _do_read_csv(file, sep, index_col, col_obs_only, col_x_only, cache=cache)
             obs_only_all[file_identifier] = single_adata_obs_only
-            # obs indices have to be unique otherwise updating and working with the MuData object will fail
+            # obs indices have to be unique otherwise updating and working with the object will fail
             if index_col:
                 adata.obs_names_make_unique()
 
-            if return_mudata_object:
-                if not mudata:
-                    mudata = MuData({file_identifier: adata})
-                else:
-                    mudata.mod[file_identifier] = adata
-            else:
-                anndata_dict[file_identifier] = adata
-    if return_mudata_object:
-        mudata.update()
-        return mudata
-    elif return_dfs:
+            anndata_dict[file_identifier] = adata
+    if return_dfs:
         return df_dict
     else:
         return anndata_dict, obs_only_all
 
 
 def _do_read_csv(
     file_path: Path | Iterator[str],
@@ -298,15 +281,15 @@
                 f"for obs only. Using default indices instead and moving [blue]{index_column} [yellow]to column_obs_only."
             )
             index_column = None
         initial_df = pd.read_csv(file_path, delimiter=delimiter, index_col=index_column, **kwargs)
     # in case the index column is misspelled or does not exist
     except ValueError:
         raise IndexNotFoundError(
-            f"Could not create AnnData object while reading file {file_path}. Does index_column named {index_column} "
+            f"Could not create AnnData object while reading file {file_path} . Does index_column named {index_column} "
             f"exist in {file_path}?"
         ) from None
 
     initial_df, columns_obs_only = _prepare_dataframe(initial_df, columns_obs_only, columns_x_only, cache)
 
     return df_to_anndata(initial_df, columns_obs_only), columns_obs_only
 
@@ -355,14 +338,15 @@
     columns_obs_only: list[str] | None = None,
     columns_x_only: list[str] | None = None,
     return_df: bool = False,
     cache: bool = False,
     backup_url: str | None = None,
     index_column: str | int | None = None,
     download_dataset_name: str | None = None,
+    archive_format: Literal["zip", "tar", "tar.gz", "tgz"] = None,
 ) -> pd.DataFrame | AnnData:
     """Reads one or multiple FHIR files using fhiry.
 
     Uses https://github.com/dermatologist/fhiry to read the FHIR file into a Pandas DataFrame
     which is subsequently transformed into an AnnData object.
 
     Args:
@@ -382,15 +366,15 @@
     Examples:
         >>> import ehrapy as ep
         >>> adata = ep.io.read_fhir("/path/to/fhir/resources")
     """
     _check_columns_only_params(columns_obs_only, columns_x_only)
     file_path: Path = Path(dataset_path)
     if not file_path.exists():
-        file_path = _get_non_existing_files(file_path, download_dataset_name, backup_url)
+        file_path = _get_non_existing_files(file_path, download_dataset_name, backup_url, archive_format)
 
     adata = _read_fhir(
         file_path=str(file_path.resolve()),
         format=format,
         index_column=index_column,
         columns_obs_only=columns_obs_only,
         columns_x_only=columns_x_only,
@@ -404,18 +388,18 @@
     file_path: str,
     format: Literal["json", "ndjson"],
     index_column: dict[str, str | int] | str | int | None,
     columns_obs_only: list[str] | None,
     columns_x_only: list[str] | None,
     return_df: bool = False,
     cache: bool = False,
-) -> AnnData | dict[str, AnnData] | MuData:
+) -> AnnData | dict[str, AnnData]:
     """Internal interface of the read_fhir method."""
     if cache and return_df:
-        raise CachingNotSupported("Caching is currently not supported for MuData or Pandas DataFrame objects.")
+        raise CachingNotSupported("Caching is currently not supported for or Pandas DataFrame objects.")
     if return_df and (columns_x_only or columns_obs_only):
         raise Warning(
             "Parameters columns_x_only and columns_obs_only are not supported when returning Pandas DataFrames."
         )
     path_cache = settings.cachedir / file_path
     if cache and (path_cache.is_dir() or path_cache.is_file()):
         raise CacheExistsException(
@@ -441,60 +425,42 @@
         if not path_cache.parent.is_dir():
             path_cache.parent.mkdir(parents=True)
         return _write_cache(adata, path_cache, columns_obs_only)  # type: ignore
 
     return adata
 
 
-def _get_non_existing_files(file: Path, download_dataset_name: str, backup_url: str) -> Path:
-    """Handle non existing files or directories by trying to download from a backup_url and moving them
-    in the correct directory.
-
-    Args:
-        backup_url: Backup URL to lookup for the datafile(s)
+def _get_non_existing_files(
+    dataset_path: Path,
+    download_dataset_name: str,
+    backup_url: str,
+    archive_format: Literal["zip", "tar", "tar.gz", "tgz"] = None,
+) -> Path:
+    """Handle non existing files or directories by trying to download from a backup_url and moving them in the correct directory.
 
     Returns:
-        The file or directory path of the downloaded content
+        The file or directory path of the downloaded content.
     """
-    if backup_url is not None:
-        download_default_name = backup_url.split("/")[-1]
-        download_dataset_name = download_dataset_name or download_default_name
-        # currently supports zip, tar, gztar, bztar, xztar
-        archive_formats, _ = zip(*shutil.get_archive_formats())
-        is_archived = download_default_name[-3:] in archive_formats
-
-    else:
-        raise BackupURLNotProvidedError(
-            f"File or directory {file} does not exist and no backup_url was provided.\n"
+    if backup_url is None and not dataset_path.exists():
+        raise ValueError(
+            f"File or directory {dataset_path} does not exist and no backup_url was provided.\n"
             f"Please provide a backup_url or check whether path is spelled correctly."
         )
     print("[bold yellow]Path or dataset does not yet exist. Attempting to download...")
     download(
         backup_url,
-        output_file_name=download_default_name,
+        output_file_name=download_dataset_name,
         output_path=ehrapy_settings.datasetdir,
-        is_archived=is_archived,
+        archive_format=archive_format,
     )
-    # if archived, remove archive suffix
-    archive_extension = download_default_name[-4:]
-    output_path_name = download_default_name.replace(archive_extension, "") if is_archived else download_default_name
-    output_file_or_dir = ehrapy_settings.datasetdir / output_path_name
-    moved_path = Path(str(output_file_or_dir)[: str(output_file_or_dir).rfind("/") + 1]) / download_dataset_name
-    if moved_path.exists():
-        shutil.move(output_file_or_dir, moved_path)  # type: ignore
-        file = moved_path
-    elif (
-        not moved_path.exists()
-    ):  # some zip files change their name when unzipped. Hence, we look for the latest created file in datasetdir
-        list_of_paths = [path for path in ehrapy_settings.datasetdir.glob("*/") if not path.name.startswith(".")]
-        latest_path = max(list_of_paths, key=lambda path: path.stat().st_ctime)
-        shutil.move(latest_path, moved_path)  # type: ignore
-        file = moved_path
 
-    return file
+    if archive_format:
+        dataset_path = remove_archive_extension(dataset_path)
+
+    return dataset_path
 
 
 def _read_from_cache_dir(cache_dir: Path) -> dict[str, AnnData]:
     """Read AnnData objects from the cache directory."""
     adata_objects = {}
     # read each cache file in the cache directory and store it into a dict
     for cache_file in cache_dir.iterdir():
@@ -591,15 +557,15 @@
     object_type_columns = [col_name for col_name in initial_df.columns if initial_df[col_name].dtype == "object"]
     # if columns_obs_only is None, initialize it as datetime columns need to be included here
     if not columns_obs_only:
         columns_obs_only = []
     no_datetime_object_col = []
     for col in object_type_columns:
         try:
-            pd.to_datetime(initial_df[col])
+            pd.to_datetime(initial_df[col], format="mixed")
             # only add to column_obs_only if not present already to avoid duplicates
             if col not in columns_obs_only:
                 columns_obs_only.append(col)
         except (ValueError, TypeError):
             # we only need to replace NANs on non datetime, non numerical columns since datetime are obs only by default
             no_datetime_object_col.append(col)
     # writing to hd5a files requires non string to be empty in non numerical columns
@@ -767,18 +733,14 @@
             )
 
 
 class IndexNotFoundError(Exception):
     pass
 
 
-class BackupURLNotProvidedError(Exception):
-    pass
-
-
 class CachingNotSupported(Exception):
     pass
 
 
 class ExtensionMissingError(Exception):
     pass
```

### Comparing `ehrapy-0.4.0/ehrapy/io/_utility_io.py` & `ehrapy-0.5.0/ehrapy/io/_utility_io.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/io/_write.py` & `ehrapy-0.5.0/ehrapy/io/_write.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/logging.py` & `ehrapy-0.5.0/ehrapy/logging.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/plot/_missingno_pl_api.py` & `ehrapy-0.5.0/ehrapy/plot/_missingno_pl_api.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/plot/_qc.py` & `ehrapy-0.5.0/ehrapy/plot/_qc.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/plot/_scanpy_pl_api.py` & `ehrapy-0.5.0/ehrapy/plot/_scanpy_pl_api.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/plot/_survival_analysis.py` & `ehrapy-0.5.0/ehrapy/plot/_survival_analysis.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/plot/_util.py` & `ehrapy-0.5.0/ehrapy/plot/_util.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/preprocessing/__init__.py` & `ehrapy-0.5.0/ehrapy/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/preprocessing/_data_imputation.py` & `ehrapy-0.5.0/ehrapy/preprocessing/_data_imputation.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/preprocessing/_encode.py` & `ehrapy-0.5.0/ehrapy/preprocessing/_encode.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from itertools import chain
-from typing import Any, Dict, List
+from typing import Any
 
 import numpy as np
 import pandas as pd
 from _collections import OrderedDict
 from anndata import AnnData
 from category_encoders import CountEncoder, HashingEncoder
-from mudata import MuData
 from rich import print
 from rich.progress import BarColumn, Progress
 from sklearn.preprocessing import LabelEncoder, OneHotEncoder
 
 from ehrapy import logging as logg
 from ehrapy.anndata.anndata_ext import _update_uns
 
 multi_encoding_modes = {"hash_encoding"}
 available_encodings = {"one_hot_encoding", "label_encoding", "count_encoding", *multi_encoding_modes}
 
 
 def encode(
-    data: AnnData | MuData,
+    data: AnnData,
     autodetect: bool | dict = False,
     encodings: dict[str, dict[str, list[str]]] | dict[str, list[str]] | str | None = None,
-) -> AnnData | None:
-    """Encode the initial read :class:`~anndata.AnnData` or :class:`~mudata.MuData` object.
+) -> AnnData:
+    """Encode categoricals of an :class:`~anndata.AnnData` object.
 
     Categorical values could be either passed via parameters or are autodetected on the fly.
     The categorical values are also stored in obs and uns (for keeping the original, unencoded values).
     The current encoding modes for each variable are also stored in uns (`var_to_encoding` key).
     Variable names in var are updated according to the encoding modes used. A variable name starting with `ehrapycat_`
     indicates an encoded column (or part of it).
 
@@ -42,106 +41,76 @@
     Available encodings are:
         1. one_hot_encoding (https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html)
         2. label_encoding (https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.LabelEncoder.html)
         3. count_encoding (https://contrib.scikit-learn.org/category_encoders/count.html)
         4. hash_encoding (https://contrib.scikit-learn.org/category_encoders/hashing.html)
 
     Args:
-        data: The initial :class:`~anndata.AnnData` or :class:`~mudata.MuData` object
+        data: A :class:`~anndata.AnnData` object.
         autodetect: Whether to autodetect categorical values that will be encoded.
-        encodings: Only needed if autodetect set to False (or False for some columns in case of a :class:`~mudata.MuData` object).
-        A dict containing the encoding mode and categorical name for the respective column (for each AnnData object in case of MuData object).
+        encodings: Only needed if autodetect set to False.
+                   A dict containing the encoding mode and categorical name for the respective column
+                   or the specified encoding that will be applied to all columns.
 
     Returns:
-        An :class:`~anndata.AnnData` object with the encoded values in X or None (in case of :class:`~mudata.MuData` object).
+        An :class:`~anndata.AnnData` object with the encoded values in X.
 
     Examples:
         >>> import ehrapy as ep
-        >>> adata = ep.io.read(...)
+        >>> adata = ep.dt.mimic_2()
         >>> # encode all autodetected (non numerical) columns using label encoding
         >>> adata_encoded = ep.pp.encode(adata, autodetect=True)
 
-    # Example using autodetect with non-default encoding mode:
+        # Example using autodetect with non-default encoding mode:
         >>> import ehrapy as ep
-        >>> adata = ep.io.read(...)
-        >>> # encode all autodetected (non numerical) columns using one hot encoding (this only works for single column encoding modes, not hash encoding)
-        >>> adata_encoded = ep.pp.encode(adata, autodetect=True, 'one_hot_encoding')
+        >>> adata = ep.dt.mimic_2()
+        >>> # encode all autodetected (non numerical) columns using one hot encoding
+        >>> adata_encoded = ep.pp.encode(adata, autodetect=True, encodings='one_hot_encoding')
 
-    # Example using custom encodings per columns:
+        # Example using custom encodings per columns:
         >>> import ehrapy as ep
-        >>> adata = ep.io.read(...)
+        >>> adata = ep.dt.mimic_2()
         >>> # encode col1 and col2 using label encoding and encode col3 using one hot encoding
-        >>> adata_encoded = ep.pp.encode(adata, autodetect=False, {'label_encoding': ['col1', 'col2'], 'one_hot_encoding': ['col3']})
+        >>> adata_encoded = ep.pp.encode(adata,
+        >>>                              autodetect=False,
+        >>>                              encodings={'label_encoding': ['col1', 'col2'], 'one_hot_encoding': ['col3']})
     """
     if isinstance(data, AnnData):
         # basic type checking for passed parameters when encoding a single AnnData object
-        if not _check_anndata_input_type(autodetect, encodings):
-            raise EncodingInputValueError
+        _check_anndata_input_type(autodetect, encodings)
         return _encode(adata=data, autodetect=autodetect, encodings=encodings)
-    elif isinstance(data, MuData):
-        # basic type checking for passed parameters when encoding a MuData object (collection of multiple AnnData objects)
-        if not _check_mudata_input_type(autodetect, encodings):
-            raise EncodingInputValueError
-        for adata in data.mod.keys():
-            detect, encodings_modes = _get_mudata_autodetect_options_and_encoding_modes(adata, autodetect, encodings)  # type: ignore
-            # autodetect is set to False, but no encodings were provided; warn and skip this object
-            if not detect and not encodings_modes:
-                print(
-                    f"[bold yellow]Skipped encoding modality {adata}, as autodetect is set to false and no encodings were provided!"
-                )
-            if encodings_modes:
-                data.mod[adata] = _encode(data.mod[adata], detect, encodings_modes)
-            data.update()
-            # no need to return since this references the original MuData object
     else:
-        print(f"[b red]Cannot encode object of type {type(data)}. Can only encode AnnData or MuData objects!")
-        raise ValueError
-    if isinstance(data, AnnData):
-        logg.debug("Encoded the AnnData object.")
-    elif isinstance(data, MuData):
-        logg.debug("Encoded the MuData object.")
-
-    return None
+        raise ValueError(f"Cannot encode object of type {type(data)}. Can only encode AnnData objects!")
 
 
 def undo_encoding(
-    data: AnnData | MuData,
+    data: AnnData,
     columns: str = "all",
 ) -> AnnData | None:
     """Undo the current encodings applied to all columns in X.
 
-    This currently resets the AnnData or MuData object to its initial state.
+    This currently resets the AnnData object to its initial state.
 
     Args:
-        data: The :class:`~anndata.AnnData` or MuData object
+        data: The :class:`~anndata.AnnData` object
         columns: The names of the columns to reset encoding for. Defaults to all columns.
 
     Returns:
-        A (partially) encoding reset :class:`~anndata.AnnData` or MuData object
+        A (partially) encoding reset :class:`~anndata.AnnData`
 
     Examples:
         >>> import ehrapy as ep
         >>> # adata_encoded is an encoded AnnData object
-        >>> adata_undone = ep.encode.undo_encoding(adata_encoded)
+        >>> adata_undone = ep.pp.encode.undo_encoding(adata_encoded)
     """
     if isinstance(data, AnnData):
         return _undo_encoding(data, columns)
-    elif isinstance(data, MuData):
-        for adata in data.mod.keys():
-            reset_adata = _undo_encoding(data.mod[adata], columns)
-            if reset_adata:
-                data.mod[adata] = reset_adata
-        data.update()
     else:
-        print(f"[b red]Cannot decode object of type {type(data)}. Can only decode AnnData or MuData objects!")
+        print(f"[b red]Cannot decode object of type {type(data)}. Can only decode AnnData objects!")
         raise ValueError
-    if isinstance(data, AnnData):
-        logg.debug("Decoded the AnnData object.")
-    elif isinstance(data, MuData):
-        logg.debug("Decoded the MuData object.")
 
     return None
 
 
 def _encode(
     adata: AnnData,
     autodetect: bool | dict = False,
@@ -232,14 +201,17 @@
                 dtype=np.float32,
             )
             encoded_ann_data.uns["var_to_encoding"] = {categorical: encode_mode for categorical in categoricals_names}
             encoded_ann_data.uns["encoding_to_var"] = {encode_mode: categoricals_names}
 
             encoded_ann_data.uns["numerical_columns"] = adata.uns["numerical_columns"].copy()
             encoded_ann_data.uns["non_numerical_columns"] = []
+            encoded_ann_data.uns["encoded_non_numerical_columns"] = [
+                column for column in encoded_ann_data.var_names if column.startswith("ehrapycat_")
+            ]
 
             _add_categoricals_to_obs(adata, encoded_ann_data, categoricals_names)
 
     # user passed categorical values with encoding mode for each of them
     else:
         # Required since this would be deleted through side references
         non_numericals = adata.uns["non_numerical_columns"].copy()
@@ -296,15 +268,17 @@
                     "one_hot_encoding": _one_hot_encoding,
                     "label_encoding": _label_encoding,
                     "count_encoding": _count_encoding,
                     "hash_encoding": _hash_encoding,
                 }
                 progress.update(task, description=f"Running {encoding_mode} ...")
                 # perform the actual encoding
-                encoded_x, encoded_var_names = encode_mode_switcher[encoding_mode](adata, encoded_x, orig_uns_copy, encoded_var_names, encodings[encoding_mode], progress, task)  # type: ignore
+                encoded_x, encoded_var_names = encode_mode_switcher[encoding_mode](
+                    adata, encoded_x, orig_uns_copy, encoded_var_names, encodings[encoding_mode], progress, task  # type: ignore
+                )
                 # update encoding history in uns
                 for categorical in encodings[encoding_mode]:  # type: ignore
                     # multi column encoding modes -> multiple encoded columns
                     if isinstance(categorical, list):
                         for column_name in categorical:
                             var_to_encoding[column_name] = encoding_mode
                     else:
@@ -336,14 +310,17 @@
                 "[bold red]Creation of AnnData object failed. Ensure that you passed all non numerical, "
                 "categorical values for encoding!"
             )
             raise AnnDataCreationError
         updated_num_uns, updated_non_num_uns, _ = _update_uns(adata, categoricals)
         encoded_ann_data.uns["numerical_columns"] = updated_num_uns
         encoded_ann_data.uns["non_numerical_columns"] = updated_non_num_uns
+        encoded_ann_data.uns["encoded_non_numerical_columns"] = [
+            column for column in encoded_ann_data.var_names if column.startswith("ehrapycat_")
+        ]
 
         _add_categoricals_to_obs(adata, encoded_ann_data, categoricals)
 
     logg.debug("Successfully encoded the AnnData object.")
 
     return encoded_ann_data
 
@@ -669,15 +646,15 @@
 ) -> AnnData | None:
     """
     Undo the current encodings applied to all columns in X. This currently resets the AnnData object to its initial state.
 
     Args:
         adata: The AnnData object
         columns: The names of the columns to reset encoding for. Defaults to all columns. This resets the AnnData object to its initial state.
-        suppress_warning: Whether warnings should be suppressed or not (only True if called from a MuData object)
+        suppress_warning: Whether warnings should be suppressed or not.
 
     Returns:
         A (partially) encoding reset AnnData object
     """
     if "var_to_encoding" not in adata.uns.keys():
         if not suppress_warning:
             print("[bold yellow]Calling undo_encoding on unencoded AnnData object.")
@@ -900,144 +877,37 @@
                 new["original_values_categoricals"][var_name] = original.X[::, idx : idx + 1].astype("float")
             else:
                 new["original_values_categoricals"][var_name] = original.X[::, idx : idx + 1].astype("str")
 
     logg.info(f"The original categorical values `{categorical_names}` were added to uns.")
 
 
-def _get_mudata_autodetect_options_and_encoding_modes(
-    identifier: str, autodetect: dict, encodings: dict[str, dict[str, list[str]]]
-) -> tuple[bool, dict | None]:
-    """
-    Extract the index column (if any) and the columns, for obs only (if any) from the given user input.
-
-    This function is only called when dealing with datasets consisting of multiple files (for example MIMIC-III).
-
-    For each file, `index_columns` and `columns_obs_only` can provide three cases:
-        1.) The filename (thus the identifier) is not present as a key and no default key is provided or one or both dicts are empty:
-            --> No index column will be set and/or no columns are obs only (based on user input)
-
-            .. code-block:: python
-                   # some setup code here
-                   ...
-                   # filename
-                   identifier1 = "MyFile"
-                   identifier2 = "MyOtherFile"
-                   # no default key and identifier1 is not in the index or columns_obs_only keys
-                   # -> no index column will be set and no columns will be obs only (except datetime, if any)
-                   index_columns = {"MyOtherFile":["MyOtherColumn1"]}
-                   columns_obs_only = {"MyOtherFile":["MyOtherColumn2"]}
-
-        2.) The filename (thus the identifier) is not present as a key, but default key is provided
-            --> The index column will be set and/or columns will be obs only according to the default key
-
-            .. code-block:: python
-                  # some setup code here
-                   ...
-                   # filename
-                   identifier1 = "MyFile"
-                   identifier2 = "MyOtherFile"
-                   # identifier1 is not in the index or columns_obs_only keys, but default key is set for both
-                   # -> index column will be set using MyColumn1 and column obs only will include MyColumn2
-                   index_columns = {"MyOtherFile":["MyOtherColumn1"], "default": "MyColumn1"}
-                   columns_obs_only = {"MyOtherFile":["MyOtherColumn2"], "default": "MyColumn2"}
-
-        3.) The filename is present as a key
-            --> The index column will be set and/or columns are obs only according to its value
-
-            .. code-block:: python
-                   # some setup code here
-                   ...
-                   # filename
-                   identifier1 = "MyFile"
-                   identifier2 = "MyOtherFile"
-                   # identifier1 is in the index and columns_obs_only keys
-                   # -> index column will be MyColumn1 and columns_obs_only will include MyColumn2 and MyColumn3
-                   index_columns = {"MyFile":["MyColumn1"]}
-                   columns_obs_only = {"MyFile":["MyColumn2", "MyColumn3"]}
-
-    Args:
-        identifier: The name of the file
-        autodetect: A Dictionary of files to autodetected categorical columns
-        encodings: A Dictionary from mapping to columns
-
-    Returns:
-        Index column (if any) and columns obs only (if any) for this specific AnnData object
-    """
-    _autodetect = False
-    _encodings = None
-    # should use autodetect on this object?
-    if identifier in autodetect:
-        _autodetect = autodetect[identifier]
-    elif "default" in autodetect:
-        _autodetect = autodetect["default"]
-
-    # get encodings (if autodetection is not used)
-    if not _autodetect:
-        if identifier in encodings:
-            _encodings = encodings[identifier]
-
-    return _autodetect, _encodings
-
-
 def _check_anndata_input_type(
     autodetect: bool | dict, encodings: dict[str, dict[str, list[str]]] | dict[str, list[str]] | str | None
-) -> bool:
+) -> None:
     """
     Check type of passed parameters, whether they match the requirements to encode an AnnData object or not.
 
     Args:
         autodetect: Whether columns, that should be encoded, should be autodetected or not
 
     Returns:
         Whether they match type requirements or not
     """
     if not isinstance(autodetect, bool):
-        print(
-            f"[bold red]Attempted to encode an AnnData object, but passed parameter for [bold blue]autodetect [bold red]{autodetect} is not a boolean."
-            f"Please provide a boolean value for [bold blue]autodetect [bold red]when encoding a single AnnData object!"
+        raise ValueError(
+            f"Attempted to encode an AnnData object, but passed parameter for autodetect {autodetect} is not a boolean."
+            f"Please provide a boolean value for autodetect when encoding a single AnnData object!"
         )
-        return False
     elif isinstance(encodings, str) and not autodetect:
-        print("[bold red]Passing a string for parameter encodings is only possible when using autodetect=True!")
-        return False
+        raise ValueError("Passing a string for parameter encodings is only possible when using autodetect=True!")
     elif autodetect and not isinstance(encodings, (str, type(None))):
-        print(
-            "[bold red]Setting encode mode when autodetect=True only works by passing a string (encode mode name) or None not {type(encodings)}!"
-        )
-        return False
-
-    return True
-
-
-def _check_mudata_input_type(
-    autodetect: bool | dict, encodings: dict[str, dict[str, list[str]]] | dict[str, list[str]] | str | None
-) -> bool:
-    """Check type of passed parameters, whether they match the requirements to encode a MuData object or not.
-
-    Args:
-        autodetect: Whether columns, that should be encoded, should be autodetected or not
-        encodings: (Different) encoding mode(s) and their columns to be applied on
-
-    Returns:
-        Whether they match type requirements or not
-    """
-    if not isinstance(autodetect, Dict):
-        print(
-            f"[bold red]Tried encoding a MuData object, but passed parameter for [bold blue]autodetect [bold red]{autodetect} is not a dictionary. "
-            f"Please provide a dictionary for [bold blue]autodetect [bold red]when encoding a MuData object!"
-        )
-        return False
-    elif encodings and any(isinstance(column, List) for column in encodings.values()):  # type: ignore
-        print(
-            "[bold red]Encoding a MuData object requires a dictionary passed for every AnnData object, that should be encoded, containing the "
-            "encoding modes and columns, as required for a single AnnData object!"
+        raise ValueError(
+            "[Setting encode mode when autodetect=True only works by passing a string (encode mode name) or None not {type(encodings)}!"
         )
-        return False
-    return True
 
 
 class AlreadyEncodedWarning(UserWarning):
     pass
 
 
 class EncodingInputValueError(ValueError):
```

### Comparing `ehrapy-0.4.0/ehrapy/preprocessing/_highly_variable_features.py` & `ehrapy-0.5.0/ehrapy/preprocessing/_highly_variable_features.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/preprocessing/_normalization.py` & `ehrapy-0.5.0/ehrapy/preprocessing/_normalization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
+from typing import Sequence
+
 import numpy as np
 from anndata import AnnData
 from sklearn.preprocessing import maxabs_scale, minmax_scale, power_transform, quantile_transform, robust_scale, scale
 
 from ehrapy import logging as logg
 from ehrapy.anndata.anndata_ext import (
     _get_column_values,
     assert_numeric_vars,
     get_column_indices,
     get_numeric_vars,
     set_numeric_vars,
 )
 
 
-def scale_norm(adata: AnnData, vars: str | list[str] | None = None, copy: bool = False, **kwargs) -> AnnData | None:
+def scale_norm(adata: AnnData, vars: str | Sequence[str] | None = None, copy: bool = False, **kwargs) -> AnnData | None:
     """Apply scaling normalization.
 
     Functionality is provided by :func:`~sklearn.preprocessing.scale`, see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.scale.html for details.
 
     Args:
         adata: :class:`~anndata.AnnData` object containing X to normalize values in. Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
         vars: List of the names of the numeric variables to normalize.
@@ -27,15 +29,15 @@
         **kwargs: Additional arguments passed to :func:`~sklearn.preprocessing.scale`
 
     Returns:
         :class:`~anndata.AnnData` object with normalized X. Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
     Examples:
         >>> import ehrapy as ep
-        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata = ep.dt.mimic_2(encoded=True)
         >>> adata_norm = ep.pp.scale_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
@@ -53,15 +55,17 @@
     _record_norm(adata, vars, "scale")
 
     logg.debug("Scaling normalization was applied on `X`.")
 
     return adata
 
 
-def minmax_norm(adata: AnnData, vars: str | list[str] | None = None, copy: bool = False, **kwargs) -> AnnData | None:
+def minmax_norm(
+    adata: AnnData, vars: str | Sequence[str] | None = None, copy: bool = False, **kwargs
+) -> AnnData | None:
     """Apply min-max normalization.
 
     Functionality is provided by :func:`~sklearn.preprocessing.minmax_scale`,
     see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.minmax_scale.html for details.
 
     Args:
         adata: :class:`~anndata.AnnData` object containing X to normalize values in.
@@ -73,15 +77,15 @@
 
     Returns:
         :class:`~anndata.AnnData` object with normalized X.
         Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
     Examples:
         >>> import ehrapy as ep
-        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata = ep.dt.mimic_2(encoded=True)
         >>> adata_norm = ep.pp.minmax_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
@@ -99,15 +103,15 @@
     _record_norm(adata, vars, "minmax")
 
     logg.debug("AnnData's `X` was min-max normalized.")
 
     return adata
 
 
-def maxabs_norm(adata: AnnData, vars: str | list[str] | None = None, copy: bool = False) -> AnnData | None:
+def maxabs_norm(adata: AnnData, vars: str | Sequence[str] | None = None, copy: bool = False) -> AnnData | None:
     """Apply max-abs normalization.
 
     Functionality is provided by :func:`~sklearn.preprocessing.maxabs_scale`,
     see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.maxabs_scale.html for details.
 
     Args:
         adata: :class:`~anndata.AnnData` object containing X to normalize values in.
@@ -118,15 +122,15 @@
 
     Returns:
         :class:`~anndata.AnnData` object with normalized X.
         Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
     Examples:
         >>> import ehrapy as ep
-        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata = ep.dt.mimic_2(encoded=True)
         >>> adata_norm = ep.pp.maxabs_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
@@ -145,15 +149,15 @@
 
     logg.debug("AnnData's `X` was max-abs normalized.")
 
     return adata
 
 
 def robust_scale_norm(
-    adata: AnnData, vars: str | list[str] | None = None, copy: bool = False, **kwargs
+    adata: AnnData, vars: str | Sequence[str] | None = None, copy: bool = False, **kwargs
 ) -> AnnData | None:
     """Apply robust scaling normalization.
 
     Functionality is provided by :func:`~sklearn.preprocessing.robust_scale`,
     see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.robust_scale.html for details.
 
     Args:
@@ -166,15 +170,15 @@
 
     Returns:
         :class:`~anndata.AnnData` object with normalized X.
         Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
     Examples:
         >>> import ehrapy as ep
-        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata = ep.dt.mimic_2(encoded=True)
         >>> adata_norm = ep.pp.robust_scale_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
@@ -192,15 +196,17 @@
     _record_norm(adata, vars, "robust_scale")
 
     logg.debug("Robust scaling normalization was applied on AnnData's `X`.")
 
     return adata
 
 
-def quantile_norm(adata: AnnData, vars: str | list[str] | None = None, copy: bool = False, **kwargs) -> AnnData | None:
+def quantile_norm(
+    adata: AnnData, vars: str | Sequence[str] | None = None, copy: bool = False, **kwargs
+) -> AnnData | None:
     """Apply quantile normalization.
 
     Functionality is provided by ~sklearn.preprocessing.quantile_transform,
     see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.quantile_transform.html for details.
 
     Args:
         adata: :class:`~anndata.AnnData` object containing X to normalize values in. Must already be encoded using ~ehrapy.preprocessing.encode.encode.
@@ -211,15 +217,15 @@
 
     Returns:
         :class:`~anndata.AnnData` object with normalized X.
         Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
     Examples:
         >>> import ehrapy as ep
-        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata = ep.dt.mimic_2(encoded=True)
         >>> adata_norm = ep.pp.quantile_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
@@ -237,15 +243,15 @@
     _record_norm(adata, vars, "quantile")
 
     logg.debug("AnnData's `X` was quantile normalized.")
 
     return adata
 
 
-def power_norm(adata: AnnData, vars: str | list[str] | None = None, copy: bool = False, **kwargs) -> AnnData | None:
+def power_norm(adata: AnnData, vars: str | Sequence[str] | None = None, copy: bool = False, **kwargs) -> AnnData | None:
     """Apply power transformation normalization.
 
     Functionality is provided by :func:`~sklearn.preprocessing.power_transform`,
     see https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.power_transform.html for details.
 
     Args:
         adata: :class:`~anndata.AnnData` object containing X to normalize values in.
@@ -257,15 +263,15 @@
 
     Returns:
         :class:`~anndata.AnnData` object with normalized X.
         Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
     Examples:
         >>> import ehrapy as ep
-        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata = ep.dt.mimic_2(encoded=True)
         >>> adata_norm = ep.pp.power_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
@@ -285,15 +291,15 @@
     logg.debug("Power transformation normalization was applied on AnnData's `X`.")
 
     return adata
 
 
 def log_norm(
     adata: AnnData,
-    vars: str | list[str] | None = None,
+    vars: str | Sequence[str] | None = None,
     base: int | float | None = None,
     offset: int | float = 1,
     copy: bool = False,
 ) -> AnnData | None:
     """Apply log normalization.
 
     Computes :math:`x = \\log(x + offset)`, where :math:`log` denotes the natural logarithm
@@ -309,31 +315,34 @@
 
     Returns:
         :class:`~anndata.AnnData` object with normalized X.
         Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
     Examples:
         >>> import ehrapy as ep
-        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata = ep.dt.mimic_2(encoded=True)
         >>> adata_norm = ep.pp.log_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
         assert_numeric_vars(adata, vars)
 
     adata = _prep_adata_norm(adata, copy)
 
-    if sum(np.sum(adata.X < 0, axis=0)) > 0:
+    adata_to_check_for_negatives = adata[:, vars] if vars else adata
+    offset_tmp_applied = adata_to_check_for_negatives.X + offset
+    if np.any(offset_tmp_applied < 0):
         raise ValueError(
-            "Matrix of X contains negative values. "
+            "Matrix X contains negative values. "
             "Undefined behavior for log normalization. "
-            "Please offset negative values with ep.pp.offset_negative_values()."
+            "Please specifiy a higher offset to this function "
+            "or offset negative values with ep.pp.offset_negative_values()."
         )
 
     var_idx = get_column_indices(adata, vars)
     var_values = _get_column_values(adata, var_idx)
 
     if offset == 1:
         np.log1p(var_values, out=var_values)
@@ -349,15 +358,15 @@
     _record_norm(adata, vars, "log")
 
     logg.debug("Log normalization was applied on AnnData's `X`.")
 
     return adata
 
 
-def sqrt_norm(adata: AnnData, vars: str | list[str] | None = None, copy: bool = False) -> AnnData | None:
+def sqrt_norm(adata: AnnData, vars: str | Sequence[str] | None = None, copy: bool = False) -> AnnData | None:
     """Apply square root normalization.
 
     Take the square root of all values.
 
     Args:
         adata: :class:`~anndata.AnnData` object containing X to normalize values in.
                Must already be encoded using :func:`~ehrapy.preprocessing.encode`.
@@ -367,15 +376,15 @@
 
     Returns:
         :class:`~anndata.AnnData` object with normalized X.
         Also stores a record of applied normalizations as a dictionary in adata.uns["normalization"].
 
     Examples:
         >>> import ehrapy as ep
-        >>> adata = ep.data.mimic_2(encoded=True)
+        >>> adata = ep.dt.mimic_2(encoded=True)
         >>> adata_norm = ep.pp.sqrt_norm(adata, copy=True)
     """
     if isinstance(vars, str):
         vars = [vars]
     if vars is None:
         vars = get_numeric_vars(adata)
     else:
@@ -403,15 +412,15 @@
 
     if "raw_norm" not in adata.layers.keys():
         adata.layers["raw_norm"] = adata.X.copy()
 
     return adata
 
 
-def _record_norm(adata: AnnData, vars: list[str], method: str) -> None:
+def _record_norm(adata: AnnData, vars: Sequence[str], method: str) -> None:
     if "normalization" in adata.uns_keys():
         norm_record = adata.uns["normalization"]
     else:
         norm_record = {}
 
     for var in vars:
         if var in norm_record.keys():
@@ -428,29 +437,27 @@
     """Offsets negative values into positive ones with the lowest negative value becoming 0.
 
     This is primarily used to enable the usage of functions such as log_norm that
     do not allow negative values for mathematical or technical reasons.
 
     Args:
         adata: :class:`~anndata.AnnData` object containing X to normalize values in.
-        layer: The layer to
+        layer: The layer to offset.
         copy: Whether to return a modified copy of the AnnData object.
 
     Returns:
         Copy of AnnData object if copy is True.
     """
     if copy:
         adata = adata.copy()
 
-    def _get_minimum(col):
-        min = np.min(col)
-        if min < 0:
-            col = col + abs(min)
-            return col
-
     if layer:
-        adata[layer] = np.apply_along_axis(_get_minimum, 0, adata[layer])
-    else:
-        adata.X = np.apply_along_axis(_get_minimum, 0, adata.X)
+        minimum = np.min(adata[layer])
+        if minimum < 0:
+            adata[layer] = adata[layer] + np.abs(minimum)
+    else:
+        minimum = np.min(adata.X)
+        if minimum < 0:
+            adata.X = adata.X + np.abs(minimum)
 
     if copy:
         return adata
```

### Comparing `ehrapy-0.4.0/ehrapy/preprocessing/_outliers.py` & `ehrapy-0.5.0/ehrapy/preprocessing/_outliers.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/preprocessing/_quality_control.py` & `ehrapy-0.5.0/ehrapy/preprocessing/_quality_control.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/preprocessing/_scanpy_pp_api.py` & `ehrapy-0.5.0/ehrapy/preprocessing/_scanpy_pp_api.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/preprocessing/laboratory_reference_tables/laposata.tsv` & `ehrapy-0.5.0/ehrapy/preprocessing/laboratory_reference_tables/laposata.tsv`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/tools/_sa.py` & `ehrapy-0.5.0/ehrapy/tools/_sa.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/tools/_scanpy_tl_api.py` & `ehrapy-0.5.0/ehrapy/tools/_scanpy_tl_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import scanpy as sc
 from anndata import AnnData
 from leidenalg.VertexPartition import MutableVertexPartition
 from scanpy._utils import AnyRandom
 from scipy.sparse import spmatrix
 
 from ehrapy.preprocessing._scanpy_pp_api import pca  # noqa: E402,F403,F401
+from ehrapy.tools import _method_options
+from ehrapy.tools.feature_ranking._rank_features_groups import rank_features_groups  # noqa: E402,F403,F401
 
 
 def tsne(
     adata: AnnData,
     n_pcs: Optional[int] = None,
     use_rep: Optional[str] = None,
     perplexity: Union[float, int] = 30,
@@ -73,27 +75,24 @@
         random_state=random_state,
         n_jobs=n_jobs,
         copy=copy,
         metric=metric,
     )
 
 
-_InitPos = Literal["paga", "spectral", "random"]
-
-
 def umap(
     adata: AnnData,
     min_dist: float = 0.5,
     spread: float = 1.0,
     n_components: int = 2,
     maxiter: Optional[int] = None,
     alpha: float = 1.0,
     gamma: float = 1.0,
     negative_sample_rate: int = 5,
-    init_pos: Union[_InitPos, np.ndarray, None] = "spectral",
+    init_pos: Union[_method_options._InitPos, np.ndarray, None] = "spectral",
     random_state: AnyRandom = 0,
     a: Optional[float] = None,
     b: Optional[float] = None,
     copy: bool = False,
     method: Literal["umap", "rapids"] = "umap",
     neighbors_key: Optional[str] = None,
 ) -> Optional[AnnData]:  # pragma: no cover
@@ -179,21 +178,17 @@
             method=method,
             neighbors_key=neighbors_key,
         )
     else:
         raise ValueError(f'.uns["{neighbors_key}"] or .uns["neighbors"] were not found. Run `ep.pp.neighbors` first.')
 
 
-_LAYOUTS = ("fr", "drl", "kk", "grid_fr", "lgl", "rt", "rt_circular", "fa")
-_Layout = Literal[_LAYOUTS]  # type: ignore
-
-
 def draw_graph(
     adata: AnnData,
-    layout: _Layout = "fa",
+    layout: _method_options._Layout = "fa",
     init_pos: Union[str, bool, None] = None,
     root: Optional[int] = None,
     random_state: AnyRandom = 0,
     n_jobs: Optional[int] = None,
     adjacency: Optional[spmatrix] = None,
     key_added_ext: Optional[str] = None,
     neighbors_key: Optional[str] = None,
@@ -756,112 +751,14 @@
         labeling_method=labeling_method,
         neighbors_key=neighbors_key,
         inplace=inplace,
         **kwargs,
     )
 
 
-_rank_features_groups_method = Optional[Literal["logreg", "t-test", "wilcoxon", "t-test_overestim_var"]]
-_corr_method = Literal["benjamini-hochberg", "bonferroni"]
-
-
-def rank_features_groups(
-    adata: AnnData,
-    groupby: str,
-    groups: Union[Literal["all"], Iterable[str]] = "all",
-    reference: str = "rest",
-    n_features: Optional[int] = None,
-    rankby_abs: bool = False,
-    pts: bool = False,
-    key_added: Optional[str] = "rank_features_groups",
-    copy: bool = False,
-    method: _rank_features_groups_method = None,
-    corr_method: _corr_method = "benjamini-hochberg",
-    tie_correct: bool = False,
-    layer: Optional[str] = None,
-    **kwds,
-) -> None:  # pragma: no cover
-    """Rank features for characterizing groups.
-
-    Expects logarithmized data.
-
-    Args:
-        adata: Annotated data matrix.
-        groupby: The key of the observations grouping to consider.
-        groups: Subset of groups, e.g. [`'g1'`, `'g2'`, `'g3'`], to which comparison
-                shall be restricted, or `'all'` (default), for all groups.
-        reference: If `'rest'`, compare each group to the union of the rest of the group.
-                   If a group identifier, compare with respect to this group.
-        n_features: The number of features that appear in the returned tables. Defaults to all features.
-        rankby_abs: Rank genes by the absolute value of the score, not by the score.
-                    The returned scores are never the absolute values.
-        pts: Compute the fraction of observations containing the features.
-        key_added: The key in `adata.uns` information is saved to.
-        copy: Whether to return a copy of the AnnData object.
-        method:  The default method is `'t-test'`,
-                 `'t-test_overestim_var'` overestimates variance of each group,
-                 `'wilcoxon'` uses Wilcoxon rank-sum,
-                 `'logreg'` uses logistic regression.
-        corr_method:  p-value correction method.
-                      Used only for `'t-test'`, `'t-test_overestim_var'`, and `'wilcoxon'`.
-        tie_correct: Use tie correction for `'wilcoxon'` scores. Used only for `'wilcoxon'`.
-        layer: Key from `adata.layers` whose value will be used to perform tests on.
-        **kwds: Are passed to test methods. Currently this affects only parameters that
-                are passed to :class:`sklearn.linear_model.LogisticRegression`.
-                For instance, you can pass `penalty='l1'` to try to come up with a
-                minimal set of genes that are good predictors (sparse solution meaning few non-zero fitted coefficients).
-
-    Returns:
-        *names*: structured `np.ndarray` (`.uns['rank_features_groups']`)
-                  Structured array to be indexed by group id storing the gene
-                  names. Ordered according to scores.
-        *scores*: structured `np.ndarray` (`.uns['rank_features_groups']`)
-                  Structured array to be indexed by group id storing the z-score
-                  underlying the computation of a p-value for each gene for each group.
-                  Ordered according to scores.
-        *logfoldchanges*: structured `np.ndarray` (`.uns['rank_features_groups']`)
-                          Structured array to be indexed by group id storing the log2
-                          fold change for each gene for each group. Ordered according to scores.
-                          Only provided if method is 't-test' like.
-                          Note: this is an approximation calculated from mean-log values.
-        *pvals*: structured `np.ndarray` (`.uns['rank_features_groups']`)
-                 p-values.
-        *pvals_adj* : structured `np.ndarray` (`.uns['rank_features_groups']`)
-                      Corrected p-values.
-        *pts*: `pandas.DataFrame` (`.uns['rank_features_groups']`)
-               Fraction of cells expressing the genes for each group.
-        *pts_rest*: `pandas.DataFrame` (`.uns['rank_features_groups']`)
-                    Only if `reference` is set to `'rest'`.
-                    Fraction of observations from the union of the rest of each group containing the features.
-
-     Examples:
-         >>> import ehrapy as ep
-         >>> adata = ep.dt.mimic_2(encoded=True)
-         >>> ep.tl.rank_features_groups(adata, "service_unit")
-         >>> ep.pl.rank_features_groups(adata)
-    """
-    return sc.tl.rank_genes_groups(
-        adata=adata,
-        groupby=groupby,
-        use_raw=False,
-        groups=groups,
-        reference=reference,
-        n_genes=n_features,
-        rankby_abs=rankby_abs,
-        pts=pts,
-        key_added=key_added,
-        copy=copy,
-        method=method,
-        corr_method=corr_method,
-        tie_correct=tie_correct,
-        layer=layer,
-        **kwds,
-    )
-
-
 def filter_rank_features_groups(
     adata: AnnData,
     key="rank_features_groups",
     groupby=None,
     key_added="rank_features_groups_filtered",
     min_in_group_fraction=0.25,
     min_fold_change=1,
@@ -903,23 +800,20 @@
         key_added=key_added,
         min_in_group_fraction=min_in_group_fraction,
         min_fold_change=min_fold_change,
         max_out_group_fraction=max_out_group_fraction,
     )
 
 
-_marker_feature_overlap_methods = Literal["overlap_count", "overlap_coef", "jaccard"]
-
-
 def marker_feature_overlap(
     adata: AnnData,
     reference_markers: Union[Dict[str, set], Dict[str, list]],
     *,
     key: str = "rank_features_groups",
-    method: _marker_feature_overlap_methods = "overlap_count",
+    method: _method_options._marker_feature_overlap_methods = "overlap_count",
     normalize: Optional[Literal["reference", "data"]] = None,
     top_n_markers: Optional[int] = None,
     adj_pval_threshold: Optional[float] = None,
     key_added: str = "feature_overlap",
     inplace: bool = False,
 ):  # pragma: no cover
     """Calculate an overlap score between data-deriven features and provided marker features.
```

### Comparing `ehrapy-0.4.0/ehrapy/tools/nlp/_medcat.py` & `ehrapy-0.5.0/ehrapy/tools/nlp/_medcat.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/tools/nlp/_translators.py` & `ehrapy-0.5.0/ehrapy/tools/nlp/_translators.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/ehrapy/util/_doc_util.py` & `ehrapy-0.5.0/ehrapy/util/_doc_util.py`

 * *Files identical despite different names*

### Comparing `ehrapy-0.4.0/pyproject.toml` & `ehrapy-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,68 +1,63 @@
 [tool.poetry]
 name = "ehrapy"
-version = "0.4.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.5.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Electronic Health Record Analysis with Python."
 authors = ["Lukas Heumos <lukas.heumos@posteo.net>", "Philipp Ehmele <philipp_ehm@protonmail.com>"]
 license = "Apache2.0"
 readme = "README.md"
 homepage = "https://github.com/theislab/ehrapy"
 repository = "https://github.com/theislab/ehrapy"
 documentation = "https://ehrapy.readthedocs.io"
 packages = [
     { include = "ehrapy" },
 ]
 classifiers = [
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.0,<4"
+python = ">=3.9.0,<3.12"
 rich = ">=10.12.0"
 PyYAML = ">=5.4.1"
-questionary = ">=1.10.0"
 requests = ">=2.26.0"
-pandas = "^2.0.1"
-mudata = ">=0.1.1"
-pypi-latest = ">=0.1.1"
 scikit-learn = ">=1.0"
 category_encoders = ">=2.2.2"
-leidenalg = ">=0.8.7"
 deepl = ">=1.2.0"
 pynndescent = ">=0.5.4"
-scanpy = "^1.9.1"
+scanpy = {extras = ["leiden"], version = "^1.9.3"}
 ipython = ">=7.30.1"
 pyhpo = {extras = ["all"], version = ">=3.0.0"}
 deep-translator = ">=1.6.1"
 scikit-learn-intelex = {version = ">=2021.5.3", optional = true}
 medcat = {version = "^1.5.0", optional = true}
-anndata = ">=0.7.8"
 fancyimpute = ">=0.7.0"
 miceforest = ">=5.3.0"
 scikit-misc = ">=0.1.4"
 session-info = ">=1.0.0"
 lifelines = ">=0.27.0"
 missingno = ">=0.5.1"
-thefuzz = {extras = ["speedup"], version = "^0.19.0"}
+thefuzz = {extras = ["speedup"], version = ">=0.19.0"}
 tabulate = ">=0.9.0"
-fhiry = ">=2.1,<4.0"
+fhiry = ">=2.1"
+numba = ">=0.57.1"
+dowhy = ">=0.10"
+
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.2.5"
 coverage = {extras = ["toml"], version = ">=6.0"}
-safety = ">=1.9.0"
 mypy = ">=0.930"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 pre-commit = ">=2.16.0"
-flake8 = ">=4.0.1"
 black = {extras = ["jupyter"], version = ">=21.12b0"}
+flake8 = ">=4.0.1"
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.11.29"
 flake8-docstrings = ">=1.5.0"
 flake8-rst-docstrings = ">=0.2.5"
 pep8-naming = ">=0.12.1"
 pre-commit-hooks = ">=4.0.1"
 Pygments = ">=2.10.0"
@@ -88,18 +83,17 @@
 sphinx-autodoc-typehints = ">=1.12.0"
 sphinx-last-updated-by-git = ">=0.3.0"
 nbsphinx = ">=0.8.7"
 sphinxcontrib-bibtex = ">=2.4.1"
 sphinx-automodapi = ">=0.14"
 nbsphinx-link = ">=1.3.0"
 sphinx-copybutton = ">=0.4.0"
-myst-parser = ">=0.17.0"
+myst-parser = "^1.0.0"
 sphinx-remove-toctrees = ">=0.0.3"
 sphinx-design = ">=0.0.13"
-sphinxext-opengraph = ">=0.6.2"
 sphinx-click = ">=3.0.0"
 furo = ">=2022.3.4"
 sphinx-autodoc-annotation = "^1.0.post1"
 sphinxcontrib-spelling = ">=7.7,<9.0"
 
 [tool.poetry.scripts]
 ehrapy = "ehrapy.__main__:main"
```

### Comparing `ehrapy-0.4.0/PKG-INFO` & `ehrapy-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,48 @@
 Metadata-Version: 2.1
 Name: ehrapy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Electronic Health Record Analysis with Python.
 Home-page: https://github.com/theislab/ehrapy
 License: Apache2.0
 Author: Lukas Heumos
 Author-email: lukas.heumos@posteo.net
-Requires-Python: >=3.8.0,<4
+Requires-Python: >=3.9.0,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: en-core-web-md
 Provides-Extra: medcat
 Provides-Extra: scikit-learn-intelex
 Requires-Dist: PyYAML (>=5.4.1)
-Requires-Dist: anndata (>=0.7.8)
 Requires-Dist: category_encoders (>=2.2.2)
 Requires-Dist: deep-translator (>=1.6.1)
 Requires-Dist: deepl (>=1.2.0)
+Requires-Dist: dowhy (>=0.10)
 Requires-Dist: fancyimpute (>=0.7.0)
-Requires-Dist: fhiry (>=2.1,<4.0)
+Requires-Dist: fhiry (>=2.1)
 Requires-Dist: ipython (>=7.30.1)
-Requires-Dist: leidenalg (>=0.8.7)
 Requires-Dist: lifelines (>=0.27.0)
 Requires-Dist: medcat (>=1.5.0,<2.0.0) ; extra == "medcat"
 Requires-Dist: miceforest (>=5.3.0)
 Requires-Dist: missingno (>=0.5.1)
-Requires-Dist: mudata (>=0.1.1)
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: numba (>=0.57.1)
 Requires-Dist: pyhpo[all] (>=3.0.0)
 Requires-Dist: pynndescent (>=0.5.4)
-Requires-Dist: pypi-latest (>=0.1.1)
-Requires-Dist: questionary (>=1.10.0)
 Requires-Dist: requests (>=2.26.0)
 Requires-Dist: rich (>=10.12.0)
-Requires-Dist: scanpy (>=1.9.1,<2.0.0)
+Requires-Dist: scanpy[leiden] (>=1.9.3,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0)
 Requires-Dist: scikit-learn-intelex (>=2021.5.3) ; extra == "scikit-learn-intelex"
 Requires-Dist: scikit-misc (>=0.1.4)
 Requires-Dist: session-info (>=1.0.0)
 Requires-Dist: tabulate (>=0.9.0)
-Requires-Dist: thefuzz[speedup] (>=0.19.0,<0.20.0)
+Requires-Dist: thefuzz[speedup] (>=0.19.0)
 Project-URL: Documentation, https://ehrapy.readthedocs.io
 Project-URL: Repository, https://github.com/theislab/ehrapy
 Description-Content-Type: text/markdown
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Build](https://github.com/theislab/ehrapy/workflows/Build%20ehrapy%20Package/badge.svg)](https://github.com/theislab/ehrapy/actions?workflow=Package)
 [![Codecov](https://codecov.io/gh/theislab/ehrapy/branch/master/graph/badge.svg)](https://codecov.io/gh/theislab/ehrapy)
```

