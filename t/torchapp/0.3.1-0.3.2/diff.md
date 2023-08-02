# Comparing `tmp/torchapp-0.3.1.tar.gz` & `tmp/torchapp-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchapp-0.3.1.tar", max compression
+gzip compressed data, was "torchapp-0.3.2.tar", max compression
```

## Comparing `torchapp-0.3.1.tar` & `torchapp-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11345 2023-07-21 01:01:15.382093 torchapp-0.3.1/LICENSE
--rw-r--r--   0        0        0     6537 2023-07-21 01:01:15.382093 torchapp-0.3.1/README.rst
--rw-r--r--   0        0        0     2142 2023-07-21 01:01:15.386093 torchapp-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       82 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/__init__.py
--rw-r--r--   0        0        0    33403 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/apps.py
--rw-r--r--   0        0        0     2141 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/bibtex/fastai.bib
--rw-r--r--   0        0        0      633 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/bibtex/mlflow.bib
--rw-r--r--   0        0        0      426 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/bibtex/optuna.bib
--rw-r--r--   0        0        0      470 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/bibtex/skopt.bib
--rw-r--r--   0        0        0      244 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/bibtex/torchapp.bib
--rw-r--r--   0        0        0      185 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/bibtex/wandb.bib
--rw-r--r--   0        0        0      420 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/blocks.py
--rw-r--r--   0        0        0       84 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/callbacks/__init__.py
--rw-r--r--   0        0        0     4116 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/callbacks/mlflow.py
--rw-r--r--   0        0        0      717 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/callbacks/wandb.py
--rw-r--r--   0        0        0     1937 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/citations.py
--rw-r--r--   0        0        0     2215 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/download.py
--rw-r--r--   0        0        0     1904 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/enums.py
--rw-r--r--   0        0        0        0 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/__init__.py
--rw-r--r--   0        0        0    12563 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/diffusion.py
--rw-r--r--   0        0        0     6750 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/image_classifier.py
--rw-r--r--   0        0        0      738 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/iris.bib
--rw-r--r--   0        0        0     1512 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/iris.py
--rwxr-xr-x   0        0        0     1809 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/logistic_regression.py
--rw-r--r--   0        0        0     1053 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/examples/mlp.py
--rw-r--r--   0        0        0     2435 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/main.py
--rw-r--r--   0        0        0      638 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/metrics.py
--rw-r--r--   0        0        0     1161 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/params.py
--rw-r--r--   0        0        0    15279 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/testing.py
--rw-r--r--   0        0        0        0 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/tuning/__init__.py
--rw-r--r--   0        0        0     2763 2023-07-21 01:01:15.390093 torchapp-0.3.1/torchapp/tuning/optuna.py
--rw-r--r--   0        0        0     5376 2023-07-21 01:01:15.394093 torchapp-0.3.1/torchapp/tuning/skopt.py
--rw-r--r--   0        0        0     3794 2023-07-21 01:01:15.394093 torchapp-0.3.1/torchapp/tuning/wandb.py
--rw-r--r--   0        0        0     3704 2023-07-21 01:01:15.394093 torchapp-0.3.1/torchapp/util.py
--rw-r--r--   0        0        0     3384 2023-07-21 01:01:15.394093 torchapp-0.3.1/torchapp/vision.py
--rw-r--r--   0        0        0     8479 1970-01-01 00:00:00.000000 torchapp-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-08-02 01:47:15.130976 torchapp-0.3.2/LICENSE
+-rw-r--r--   0        0        0     6537 2023-08-02 01:47:15.130976 torchapp-0.3.2/README.rst
+-rw-r--r--   0        0        0     2142 2023-08-02 01:47:15.134976 torchapp-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/__init__.py
+-rw-r--r--   0        0        0    33403 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/apps.py
+-rw-r--r--   0        0        0     2141 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/bibtex/fastai.bib
+-rw-r--r--   0        0        0      633 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/bibtex/mlflow.bib
+-rw-r--r--   0        0        0      426 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/bibtex/optuna.bib
+-rw-r--r--   0        0        0      470 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/bibtex/skopt.bib
+-rw-r--r--   0        0        0      244 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/bibtex/torchapp.bib
+-rw-r--r--   0        0        0      185 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/bibtex/wandb.bib
+-rw-r--r--   0        0        0      420 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/blocks.py
+-rw-r--r--   0        0        0       84 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/callbacks/__init__.py
+-rw-r--r--   0        0        0     4116 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/callbacks/mlflow.py
+-rw-r--r--   0        0        0      717 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/callbacks/wandb.py
+-rw-r--r--   0        0        0     1937 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/citations.py
+-rw-r--r--   0        0        0     2215 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/download.py
+-rw-r--r--   0        0        0     1904 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/enums.py
+-rw-r--r--   0        0        0        0 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/__init__.py
+-rw-r--r--   0        0        0    12563 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/diffusion.py
+-rw-r--r--   0        0        0     6750 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/image_classifier.py
+-rw-r--r--   0        0        0      738 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/iris.bib
+-rw-r--r--   0        0        0     1512 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/iris.py
+-rwxr-xr-x   0        0        0     1809 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/logistic_regression.py
+-rw-r--r--   0        0        0     1053 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/examples/mlp.py
+-rw-r--r--   0        0        0     2435 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/main.py
+-rw-r--r--   0        0        0      638 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/metrics.py
+-rw-r--r--   0        0        0     1161 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/params.py
+-rw-r--r--   0        0        0    15534 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/testing.py
+-rw-r--r--   0        0        0        0 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/tuning/__init__.py
+-rw-r--r--   0        0        0     2763 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/tuning/optuna.py
+-rw-r--r--   0        0        0     5376 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/tuning/skopt.py
+-rw-r--r--   0        0        0     3794 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/tuning/wandb.py
+-rw-r--r--   0        0        0     3704 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/util.py
+-rw-r--r--   0        0        0     3384 2023-08-02 01:47:15.138976 torchapp-0.3.2/torchapp/vision.py
+-rw-r--r--   0        0        0     8479 1970-01-01 00:00:00.000000 torchapp-0.3.2/PKG-INFO
```

### Comparing `torchapp-0.3.1/LICENSE` & `torchapp-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/README.rst` & `torchapp-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/pyproject.toml` & `torchapp-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torchapp"
-version = "0.3.1"
+version = "0.3.2"
 description = "A wrapper for fastai projects to create easy command-line inferfaces and manage hyper-parameter tuning."
 authors = ["Robert Turnbull <robert.turnbull@unimelb.edu.au>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/rbturnbull/torchapp"
 documentation = "https://rbturnbull.github.io/torchapp/"
 homepage = "https://github.com/rbturnbull/torchapp"
```

### Comparing `torchapp-0.3.1/torchapp/apps.py` & `torchapp-0.3.2/torchapp/apps.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/bibtex/fastai.bib` & `torchapp-0.3.2/torchapp/bibtex/fastai.bib`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/bibtex/mlflow.bib` & `torchapp-0.3.2/torchapp/bibtex/mlflow.bib`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/callbacks/mlflow.py` & `torchapp-0.3.2/torchapp/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/callbacks/wandb.py` & `torchapp-0.3.2/torchapp/callbacks/wandb.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/citations.py` & `torchapp-0.3.2/torchapp/citations.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/download.py` & `torchapp-0.3.2/torchapp/download.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/enums.py` & `torchapp-0.3.2/torchapp/enums.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/examples/diffusion.py` & `torchapp-0.3.2/torchapp/examples/diffusion.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/examples/image_classifier.py` & `torchapp-0.3.2/torchapp/examples/image_classifier.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/examples/iris.bib` & `torchapp-0.3.2/torchapp/examples/iris.bib`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/examples/iris.py` & `torchapp-0.3.2/torchapp/examples/iris.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/examples/logistic_regression.py` & `torchapp-0.3.2/torchapp/examples/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/examples/mlp.py` & `torchapp-0.3.2/torchapp/examples/mlp.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/main.py` & `torchapp-0.3.2/torchapp/main.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/metrics.py` & `torchapp-0.3.2/torchapp/metrics.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/params.py` & `torchapp-0.3.2/torchapp/params.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/testing.py` & `torchapp-0.3.2/torchapp/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,14 +165,21 @@
         if not self.expected_base:
             module = importlib.import_module(self.__module__)
             self.expected_base = Path(module.__file__).parent / "expected"
 
         self.expected_base = Path(self.expected_base)
         return self.expected_base
 
+    def test_cli_version(self):
+        app = self.get_app()
+        runner = CliRunner()
+        result = runner.invoke(app.cli(), "--version")
+        assert result.exit_code == 0
+        assert re.match(r"^(\d+\.)?(\d+\.)?(\*|\d+)$", result.stdout)
+
     def get_expected_dir(self) -> Path:
         """
         Returns the path to the directory where the expected files.
 
         It creates the directory if it doesn't already exist.
         """
         expected_dir = self.get_expected_base() / self.__class__.__name__
@@ -395,7 +402,9 @@
             result = runner.invoke(app.cli(), params)
             output = dict(
                 stdout=literal(result.stdout),
                 exit_code=result.exit_code,
             )
 
             assert_output(file, interactive, params, output, expected_output, regenerate=regenerate)
+
+
```

### Comparing `torchapp-0.3.1/torchapp/tuning/optuna.py` & `torchapp-0.3.2/torchapp/tuning/optuna.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/tuning/skopt.py` & `torchapp-0.3.2/torchapp/tuning/skopt.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/tuning/wandb.py` & `torchapp-0.3.2/torchapp/tuning/wandb.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/util.py` & `torchapp-0.3.2/torchapp/util.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/torchapp/vision.py` & `torchapp-0.3.2/torchapp/vision.py`

 * *Files identical despite different names*

### Comparing `torchapp-0.3.1/PKG-INFO` & `torchapp-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchapp
-Version: 0.3.1
+Version: 0.3.2
 Summary: A wrapper for fastai projects to create easy command-line inferfaces and manage hyper-parameter tuning.
 Home-page: https://github.com/rbturnbull/torchapp
 License: Apache-2.0
 Keywords: fastai,pytorch,deep learning,command-line interface
 Author: Robert Turnbull
 Author-email: robert.turnbull@unimelb.edu.au
 Requires-Python: >=3.8,<3.12
```

