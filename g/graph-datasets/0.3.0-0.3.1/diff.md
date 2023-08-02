# Comparing `tmp/graph_datasets-0.3.0.tar.gz` & `tmp/graph_datasets-0.3.1.tar.gz`

## Comparing `graph_datasets-0.3.0.tar` & `graph_datasets-0.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.editorconfig
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.pylintrc
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/requirements-dev.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/requirements.txt
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/cuda.sh
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/docs.sh
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/install-cpu.sh
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/install-dev.sh
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/install.sh
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/nb.sh
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/table_maker.sh
--rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/configs/nb.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.github/workflows/release.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.vscode/extensions.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/demos/demo.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/Makefile
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/conf.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/make.bat
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/rst/data_info.rst
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/rst/graph_datasets.datasets.rst
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/rst/graph_datasets.utils.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/rst/load_data.rst
--rw-r--r--   0        0        0     9985 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/rst/table.rst
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/scripts/table_maker.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/tpls/module.rst_t
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/tpls/package.rst_t
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/tpls/toc.rst_t
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/__init__.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/data_info.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/load_data.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/__init__.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/cola.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/critical.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/dgl.py
--rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/linkx.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/ogb.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/pyg.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/sdcn.py
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/utils/__init__.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/utils/statistics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/tests/statistics.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/LICENSE
--rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/README.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.editorconfig
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.pylintrc
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/requirements-dev.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/requirements.txt
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.ci/cuda.sh
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.ci/docs.sh
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.ci/install-cpu.sh
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.ci/install-dev.sh
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.ci/install.sh
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.ci/nb.sh
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.ci/table_maker.sh
+-rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.ci/configs/nb.py
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/demos/demo.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/Makefile
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/conf.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/make.bat
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/rst/data_info.rst
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/rst/graph_datasets.datasets.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/rst/graph_datasets.utils.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/rst/load_data.rst
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/rst/table.rst
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/scripts/table_maker.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/tpls/module.rst_t
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/tpls/package.rst_t
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/docs/tpls/toc.rst_t
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/__init__.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/data_info.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/load_data.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/datasets/__init__.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/datasets/cola.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/datasets/critical.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/datasets/dgl.py
+-rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/datasets/linkx.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/datasets/ogb.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/datasets/pyg.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/datasets/sdcn.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/utils/__init__.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/graph_datasets/utils/statistics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/tests/statistics.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/README.md
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 graph_datasets-0.3.1/PKG-INFO
```

### Comparing `graph_datasets-0.3.0/.pre-commit-config.yaml` & `graph_datasets-0.3.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
           - id: check-yaml
           - id: end-of-file-fixer
     # -   repo: git@github.com:asottile/reorder_python_imports
     - repo: https://github.com/asottile/reorder_python_imports
       rev: v3.9.0
       hooks:
           - id: reorder-python-imports
+            exclude: ^docs/
     - repo: local
       hooks:
           - id: black
             name: black
             entry: black
             language: system
             types: [python]
@@ -37,8 +38,12 @@
             types: [python]
             exclude: ^docs/
           - id: mdformat
             name: mdformat
             entry: mdformat
             language: system
             types: [markdown]
-            exclude: ^CHANGELOG.md
+            exclude: |
+                (?x)^(
+                    CHANGELOG.md|
+                    README.md
+                )$
```

### Comparing `graph_datasets-0.3.0/.pylintrc` & `graph_datasets-0.3.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/CHANGELOG.md` & `graph_datasets-0.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.3.1 (2023-08-02)
+
+### Fix
+
+* fix: update toml settings and several val names &amp; configs ([`2e101d2`](https://github.com/galogm/graph_datasets/commit/2e101d2b3a018c08d99374e6b0ee67c5cca706ea))
+
+
 ## v0.3.0 (2023-08-02)
 
 ### Chore
 
 * chore: remove build command, add github environment and activate env ([`b7e4009`](https://github.com/galogm/graph_datasets/commit/b7e4009c4d9a90ca74211348af7c31d375d2b76d))
 
 * chore: update actions ([`7afbb7b`](https://github.com/galogm/graph_datasets/commit/7afbb7b20bc149f8c31945cd2b40fc42d4a84cea))
```

### Comparing `graph_datasets-0.3.0/.ci/cuda.sh` & `graph_datasets-0.3.1/.ci/cuda.sh`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/.ci/install-cpu.sh` & `graph_datasets-0.3.1/.ci/install-cpu.sh`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/.ci/install.sh` & `graph_datasets-0.3.1/.ci/install.sh`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/.ci/configs/nb.py` & `graph_datasets-0.3.1/.ci/configs/nb.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/.github/workflows/release.yml` & `graph_datasets-0.3.1/.github/workflows/release.yml`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,16 @@
           fetch-depth: 0
       - uses: actions/setup-python@v4
         with:
             python-version: '3.7.16'
 
       - name: Set user info
         run: |
-          git config --local user.name "github-actions"
-          git config --local user.email "action@github.com"
+          git config user.name "github-actions[bot]"
+          git config user.email "41898282+github-actions[bot]@users.noreply.github.com"
 
       # This action uses Python Semantic Release v8
       - name: Python Semantic Release
         id: release
         uses: python-semantic-release/python-semantic-release@v8.0.0
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `graph_datasets-0.3.0/docs/Makefile` & `graph_datasets-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/docs/conf.py` & `graph_datasets-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/docs/index.rst` & `graph_datasets-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/docs/make.bat` & `graph_datasets-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/docs/rst/graph_datasets.datasets.rst` & `graph_datasets-0.3.1/docs/rst/graph_datasets.datasets.rst`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/docs/rst/table.rst` & `graph_datasets-0.3.1/docs/rst/table.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 statistics
 ===========
 +-----+----------+-------------+-----------+--------+-------------+------------+
-| idx |  source  |   dataset   |  n_nodes  | n_feat |   n_edges   | n_clusters |
+| idx |  source  |   dataset   |  n_nodes  | n_feats |   n_edges   | n_clusters |
 +=====+==========+=============+===========+========+=============+============+
 |   1 |   pyg    |    cora     |     2,708 |  1,433 |      10,556 |          7 |
 +-----+----------+-------------+-----------+--------+-------------+------------+
 |   2 |   pyg    |  citeseer   |     3,327 |  3,703 |       9,104 |          6 |
 +-----+----------+-------------+-----------+--------+-------------+------------+
 |   3 |   pyg    |   pubmed    |    19,717 |    500 |      88,648 |          3 |
 +-----+----------+-------------+-----------+--------+-------------+------------+
@@ -118,8 +118,8 @@
 |     |          |   ratings   |           |        |             |            |
 +-----+----------+-------------+-----------+--------+-------------+------------+
 |  55 | critical | minesweeper |    10,000 |      7 |      78,804 |          2 |
 +-----+----------+-------------+-----------+--------+-------------+------------+
 |  56 | critical |  tolokers   |    11,758 |     10 |   1,038,000 |          2 |
 +-----+----------+-------------+-----------+--------+-------------+------------+
 |  57 | critical |  questions  |    48,921 |    301 |     307,080 |          2 |
-+-----+----------+-------------+-----------+--------+-------------+------------+
++-----+----------+-------------+-----------+--------+-------------+------------+
```

### Comparing `graph_datasets-0.3.0/docs/scripts/table_maker.py` & `graph_datasets-0.3.1/docs/scripts/table_maker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Dataset Statistics
 """
 # pylint:disable=duplicate-code,line-too-long
 import re
 
-from texttable import Texttable
 import pandas as pd
+from texttable import Texttable
 
 from graph_datasets import load_data
 from graph_datasets.data_info import DATASETS
 from graph_datasets.utils import format_value
 
 idx = 0
 
@@ -19,36 +19,36 @@
         directory="./data",
         source=_source,
         verbosity=1,
     )
 
     global idx
     idx = idx + 1
-    n_nodes, n_feat = graph.ndata["feat"].shape
+    n_nodes, n_feats = graph.ndata["feat"].shape
     tbody.append(
         [
             idx,
             source,
             dataset,
             format_value(n_nodes),
-            format_value(n_feat),
+            format_value(n_feats),
             format_value(graph.num_edges()),
             format_value(n_clusters),
         ]
     )
 
 
 if __name__ == "__main__":
     table = Texttable()
     thead = [
         'idx',
         'source',
         'dataset',
         'n_nodes',
-        'n_feat',
+        'n_feats',
         'n_edges',
         'n_clusters',
     ]
     tbody = []
     table.set_cols_dtype(['i', 't', 't', 'i', 'i', 'i', 'i'])
     table.set_cols_align(['r', 'c', 'c', 'r', 'r', 'r', 'r'])
     for source, datasets in DATASETS.items():
```

### Comparing `graph_datasets-0.3.0/docs/tpls/package.rst_t` & `graph_datasets-0.3.1/docs/tpls/package.rst_t`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/graph_datasets/data_info.py` & `graph_datasets-0.3.1/graph_datasets/data_info.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/graph_datasets/load_data.py` & `graph_datasets-0.3.1/graph_datasets/load_data.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/graph_datasets/datasets/cola.py` & `graph_datasets-0.3.1/graph_datasets/datasets/cola.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/graph_datasets/datasets/critical.py` & `graph_datasets-0.3.1/graph_datasets/datasets/critical.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/graph_datasets/datasets/dgl.py` & `graph_datasets-0.3.1/graph_datasets/datasets/dgl.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/graph_datasets/datasets/linkx.py` & `graph_datasets-0.3.1/graph_datasets/datasets/linkx.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/graph_datasets/datasets/ogb.py` & `graph_datasets-0.3.1/graph_datasets/datasets/ogb.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/graph_datasets/datasets/pyg.py` & `graph_datasets-0.3.1/graph_datasets/datasets/pyg.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/graph_datasets/datasets/sdcn.py` & `graph_datasets-0.3.1/graph_datasets/datasets/sdcn.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/graph_datasets/utils/__init__.py` & `graph_datasets-0.3.1/graph_datasets/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/graph_datasets/utils/statistics.py` & `graph_datasets-0.3.1/graph_datasets/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/tests/statistics.py` & `graph_datasets-0.3.1/tests/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 
 def main():
     display_order = {
         "src": 1,
         "ds": 2,
         "n_nodes": 3,
-        "n_feat": 4,
+        "n_feats": 4,
         "n_edges": 5,
         "n_clusters": 6,
         "eh_1h": 7,
         "nh_1h": 8,
         "lh_1h": 9,
         "ie_1h": 10,
         "bn_1h": 11,
@@ -159,15 +159,15 @@
                 source=source,
             )
 
             dic = {}
 
             dic["ds"] = dataset
             dic["src"] = source
-            dic["n_nodes"], dic["n_feat"] = graph.ndata["feat"].shape
+            dic["n_nodes"], dic["n_feats"] = graph.ndata["feat"].shape
             dic["n_edges"] = graph.num_edges()
             dic["n_clusters"] = n_clusters
 
             dic.update(statistics(graph, labels, dataset_name=dataset, h_1=False, h_2=True))
 
             csv2file(
                 target_path="results/stat.csv",
```

### Comparing `graph_datasets-0.3.0/.gitignore` & `graph_datasets-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/LICENSE` & `graph_datasets-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.3.0/README.md` & `graph_datasets-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ```bash
 # see installation logs in logs/install.log
 $ nohup bash scripts/install.sh > logs/install.log &
 ``` -->
 
 <!-- Statistics begins -->
 ## Statistics
-|   idx | source   | dataset         | n_nodes   | n_feat   | n_edges     |   n_clusters |
+|   idx | source   | dataset         | n_nodes   | n_feats   | n_edges     |   n_clusters |
 |------:|:---------|:----------------|:----------|:---------|:------------|-------------:|
 |     1 | pyg      | cora            | 2,708     | 1,433    | 10,556      |            7 |
 |     2 | pyg      | citeseer        | 3,327     | 3,703    | 9,104       |            6 |
 |     3 | pyg      | pubmed          | 19,717    | 500      | 88,648      |            3 |
 |     4 | pyg      | corafull        | 19,793    | 8,710    | 126,842     |           70 |
 |     5 | pyg      | reddit          | 232,965   | 602      | 114,615,892 |           41 |
 |     6 | pyg      | chameleon       | 2,277     | 2,325    | 62,742      |            5 |
@@ -102,8 +102,8 @@
 |    55 | critical | minesweeper     | 10,000    | 7        | 78,804      |            2 |
 |    56 | critical | tolokers        | 11,758    | 10       | 1,038,000   |            2 |
 |    57 | critical | questions       | 48,921    | 301      | 307,080     |            2 |
 <!-- Statistics ends -->
 
 ## Requirements
 
-See in `requirements-dev.txt` and `requirements.txt`.
+See [requirements-dev.txt](./requirements-dev.txt) and [requirements.txt](./requirements.txt).
```

### Comparing `graph_datasets-0.3.0/pyproject.toml` & `graph_datasets-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "graph_datasets"
-version = "0.3.0"
+version = "0.3.1"
 authors = [{ name = "galo.gm", email = "galo.gm.work@gmail.com" }]
 keywords = ["graph", "datasets"]
 description = "Load graph datasets."
 readme = "README.md"
-license = "MIT"
+license = {file = "LICENSE"}
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
@@ -47,8 +47,7 @@
 line-length = 100
 
 [tool.semantic_release]
 version_variables = ["graph_datasets/__init__.py:__version__"]
 version_toml = ["pyproject.toml:project.version"]
 major_on_zero = false
 changelog_file = "CHANGELOG.md"
-# build_command = "python -m build"
```

