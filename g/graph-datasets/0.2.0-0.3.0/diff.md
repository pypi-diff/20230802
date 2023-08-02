# Comparing `tmp/graph_datasets-0.2.0.tar.gz` & `tmp/graph_datasets-0.3.0.tar.gz`

## Comparing `graph_datasets-0.2.0.tar` & `graph_datasets-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,50 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.editorconfig
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.pylintrc
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/=1.1.0
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/requirements-dev.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/requirements.txt
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.ci/cuda.sh
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.ci/docs.sh
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.ci/install-dev.sh
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.ci/install.sh
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.ci/nb.sh
--rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.ci/configs/nb.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.vscode/extensions.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/demos/demo.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/Makefile
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/conf.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/make.bat
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/rst/data_info.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/rst/load_data.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/rst/src.utils.rst
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/tpls/module.rst_t
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/tpls/package.rst_t
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/tpls/toc.rst_t
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/graph_datasets/__init__.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/graph_datasets/data_info.py
--rw-r--r--   0        0        0    28138 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/graph_datasets/load_data.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/graph_datasets/utils/__init__.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/graph_datasets/utils/statistics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/tests/statistics.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/LICENSE
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/README.md
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.editorconfig
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.pylintrc
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/requirements-dev.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/requirements.txt
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/cuda.sh
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/docs.sh
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/install-cpu.sh
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/install-dev.sh
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/install.sh
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/nb.sh
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/table_maker.sh
+-rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.ci/configs/nb.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/demos/demo.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/rst/data_info.rst
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/rst/graph_datasets.datasets.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/rst/graph_datasets.utils.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/rst/load_data.rst
+-rw-r--r--   0        0        0     9985 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/rst/table.rst
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/scripts/table_maker.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/tpls/module.rst_t
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/tpls/package.rst_t
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/docs/tpls/toc.rst_t
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/__init__.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/data_info.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/load_data.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/__init__.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/cola.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/critical.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/dgl.py
+-rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/linkx.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/ogb.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/pyg.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/datasets/sdcn.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/utils/__init__.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/graph_datasets/utils/statistics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/tests/statistics.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/README.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 graph_datasets-0.3.0/PKG-INFO
```

### Comparing `graph_datasets-0.2.0/.pre-commit-config.yaml` & `graph_datasets-0.3.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -18,38 +18,27 @@
     - repo: local
       hooks:
           - id: black
             name: black
             entry: black
             language: system
             types: [python]
-            exclude: |
-                (?x)^(
-                    docs/*
-                )$
+            exclude: ^docs/
+            verbose: true
           - id: yapf
             name: yapf
             entry: yapf -r -i
             language: system
             types: [python]
-            exclude: |
-                (?x)^(
-                    docs/*
-                )$
+            exclude: ^docs/
           - id: pylint
             name: pylint
             entry: pylint
             language: system
             types: [python]
-            exclude: |
-                (?x)^(
-                    docs/*
-                )$
+            exclude: ^docs/
           - id: mdformat
             name: mdformat
             entry: mdformat
             language: system
             types: [markdown]
-            exclude: |
-                (?x)^(
-                    CHANGELOG.md
-                )$
+            exclude: ^CHANGELOG.md
```

### Comparing `graph_datasets-0.2.0/.pylintrc` & `graph_datasets-0.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.2.0/.ci/cuda.sh` & `graph_datasets-0.3.0/.ci/cuda.sh`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.2.0/.ci/install.sh` & `graph_datasets-0.3.0/.ci/install.sh`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 source .venv/bin/activate
 
 # # update pip
 # python -m pip install -U pip
 
 # # torch cuda 11.3
-python -m pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu113
+python -m pip install torch==1.10.2 torchvision torchaudio --index-url https://download.pytorch.org/whl/cu113
 
 # dgl cuda 11.3
 # add a source if prefered: -i https://pypi.tuna.tsinghua.edu.cn/simple/
-python -m pip install dgl>=1.1.0 -f https://data.dgl.ai/wheels/cu113/repo.html
+python -m pip install dgl==1.1.0 -f https://data.dgl.ai/wheels/cu113/repo.html
 python -m pip install dglgo -f https://data.dgl.ai/wheels-test/repo.html
 
 # install requirements
 # add a source if prefered: -i https://pypi.tuna.tsinghua.edu.cn/simple/
 python -m pip install -r requirements.txt
 
 echo install requirements successfully!
```

### Comparing `graph_datasets-0.2.0/.ci/configs/nb.py` & `graph_datasets-0.3.0/.ci/configs/nb.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.2.0/docs/Makefile` & `graph_datasets-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.2.0/docs/conf.py` & `graph_datasets-0.3.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 sys.path.insert(0, os.path.abspath('../'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'Graph Datasets'
-copyright = '2023, EAGLE-Lab, ZJU'
-author = 'Ming GU'
+copyright = '2023, EAGLE-Lab, Zhejiang University'
+author = 'Galo.gm'
 
 # The full version, including alpha/beta/rc tags
 release = '0.0.1'
 
 
 # -- General configuration ---------------------------------------------------
```

### Comparing `graph_datasets-0.2.0/docs/make.bat` & `graph_datasets-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.2.0/docs/tpls/package.rst_t` & `graph_datasets-0.3.0/docs/tpls/package.rst_t`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.2.0/graph_datasets/data_info.py` & `graph_datasets-0.3.0/graph_datasets/data_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Data source information.
 """
 # pylint:disable=duplicate-code
-import os
-
 #: Default directory for data saving.
-DEFAULT_DATA_DIR = os.path.abspath("./data")
+DEFAULT_DATA_DIR = "./data"
 
 #: Downloading url of datasets in paper
 #: `SDCN <https://github.com/bdy9527/SDCN>`_.
 SDCN_URL = "https://github.com/bdy9527/SDCN/blob/da6bb007b7"
 
 #: Downloading url of datasets in paper
 #: `CoLA <https://github.com/GRAND-Lab/CoLA>`_.
@@ -24,14 +22,19 @@
     "wiki_views": "1p5DlVHrnFgYm3VsNIzahSsvCD424AyvP",  # Wiki 1.9M
     "wiki_edges": "14X7FlkjrlUgmnsYtPwdh-gGuFla4yb5u",  # Wiki 1.9M
     "wiki_features": "1ySNspxbK-snNoAZM7oxiWGvOnTRdSyEK",  # Wiki 1.9M
     "twitch-gamer_feat": "1fA9VIIEI8N0L27MSQfcBzJgRQLvSbrvR",
     "twitch-gamer_edges": "1XLETC6dG3lVl7kDmytEJ52hvDMVdxnZ0",
 }
 
+#: Downloading url of datasets in paper
+#: `A Critical Look at the Evaluation of GNNs Under Heterophily:
+#: Are We Really Making Progress?* <https://openreview.net/pdf?id=tJbbQfw-5wv>`_.
+CRITICAL_URL = "https://github.com/yandex-research/heterophilous-graphs/blob/a431395/data"
+
 #: Supported datasets of pyG.
 #:
 #: NOTE: main difference of dgl and pyG datasets
 #: - dgl has self-loops while pyG removes them.
 #: - dgl row normalizes features while pyG does not.
 PYG_DATASETS = [
     "cora",
@@ -106,15 +109,27 @@
     "deezer-europe",
     "Amherst41",
     "Cornell5",
     "Johns Hopkins55",
     "Reed98",
 ]
 
+#: Datasets in paper
+#: `A Critical Look at the Evaluation of GNNs Under Heterophily:
+#: Are We Really Making Progress?* <https://openreview.net/pdf?id=tJbbQfw-5wv>`_.
+CRITICAL_DATASETS = [
+    "roman-empire",
+    "amazon-ratings",
+    "minesweeper",
+    "tolokers",
+    "questions",
+]
+
 DATASETS = {
     "pyg": PYG_DATASETS,
     "dgl": DGL_DATASETS,
     "ogb": OGB_DATASETS,
     "sdcn": SDCN_DATASETS,
     "cola": COLA_DATASETS,
     "linkx": LINKX_DATASETS,
+    "critical": CRITICAL_DATASETS,
 }
```

### Comparing `graph_datasets-0.2.0/graph_datasets/utils/__init__.py` & `graph_datasets-0.3.0/graph_datasets/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,14 +53,61 @@
         table.set_cols_valign(cols_valign)
     if cols_dtype is not None:
         table.set_cols_dtype(cols_dtype)
     table.add_rows(params)
 
     print(table.draw())
 
+    return table.draw()
+
+
+def download_tip(info: Dict) -> None:
+    """Tips for Downloading datasets
+
+    Args:
+        data_file (str): filepath.
+        url (str): url for downloading.
+    """
+    info["Tip"] = "If the download fails, \
+use the 'Download URL' to download manually and move the file to the 'Save Path'."
+
+    tab_printer(info)
+
+
+def print_dataset_info(
+    dataset_name: str,
+    n_nodes: int,
+    n_edges: int,
+    n_feats: int,
+    n_clusters: int,
+    self_loops: int = None,
+    is_directed: bool = None,
+    thead: List[str] = None,
+) -> None:
+    dic = {
+        "NumNodes": n_nodes,
+        "NumEdges": n_edges,
+        "NumFeats": n_feats,
+        "NumClasses": n_clusters,
+        "Self-loops": self_loops,
+        "Directed": is_directed,
+    }
+
+    if self_loops is None:
+        dic.pop("Self-loops")
+    if is_directed is None:
+        dic.pop("Directed")
+
+    tab_printer(
+        dic,
+        thead=["Dataset", dataset_name] if thead is None else thead,
+        cols_align=["c", "r"],
+        sort=False,
+    )
+
 
 def bar_progress(current, total, _):
     """create this bar_progress method which is invoked automatically from wget"""
     progress_message = f"Downloading: {current / total * 100}% [{current} / {total}] bytes"
     sys.stdout.write("\r" + progress_message)
     sys.stdout.flush()
 
@@ -82,14 +129,14 @@
     if not quiet:
         info = {
             "File": file_name if file_name is not None else os.path.basename(output),
             "Drive ID": gid,
             "Download URL": f"https://drive.google.com/uc?id={gid}",
             "Save Path": output,
         }
-        tab_printer(info)
+        download_tip(info)
 
     gdown.download(
         id=gid,
         output=output,
         quiet=quiet,
     )
```

### Comparing `graph_datasets-0.2.0/graph_datasets/utils/statistics.py` & `graph_datasets-0.3.0/graph_datasets/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.2.0/tests/statistics.py` & `graph_datasets-0.3.0/tests/statistics.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.2.0/.gitignore` & `graph_datasets-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.2.0/LICENSE` & `graph_datasets-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.2.0/pyproject.toml` & `graph_datasets-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "graph_datasets"
-version = "0.2.0"
+version = "0.3.0"
 authors = [{ name = "galo.gm", email = "galo.gm.work@gmail.com" }]
 keywords = ["graph", "datasets"]
 description = "Load graph datasets."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.7"
 classifiers = [
@@ -43,12 +43,12 @@
 
 [tool.yapfignore]
 
 [tool.black]
 line-length = 100
 
 [tool.semantic_release]
-version_variable = ["graph_datasets/__init__.py:__version__"]
-version_toml = "pyproject.toml:project.version"
+version_variables = ["graph_datasets/__init__.py:__version__"]
+version_toml = ["pyproject.toml:project.version"]
 major_on_zero = false
 changelog_file = "CHANGELOG.md"
-build_command = "python -m build"
+# build_command = "python -m build"
```

