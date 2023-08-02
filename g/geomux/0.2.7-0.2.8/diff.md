# Comparing `tmp/geomux-0.2.7.tar.gz` & `tmp/geomux-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomux-0.2.7.tar", max compression
+gzip compressed data, was "geomux-0.2.8.tar", max compression
```

## Comparing `geomux-0.2.7.tar` & `geomux-0.2.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-06 16:28:36.932248 geomux-0.2.7/LICENSE
--rw-r--r--   0        0        0     3282 2023-07-06 15:32:39.788448 geomux-0.2.7/README.md
--rw-r--r--   0        0        0       71 2023-07-06 15:32:39.815115 geomux-0.2.7/geomux/__init__.py
--rw-r--r--   0        0        0     2482 2023-07-06 15:32:39.815115 geomux-0.2.7/geomux/__main__.py
--rw-r--r--   0        0        0    10177 2023-07-06 15:32:39.815115 geomux-0.2.7/geomux/geomux.py
--rw-r--r--   0        0        0     1005 2023-07-06 15:32:39.815115 geomux-0.2.7/geomux/utils.py
--rw-r--r--   0        0        0      555 2023-07-06 16:45:20.486254 geomux-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3943 1970-01-01 00:00:00.000000 geomux-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-31 23:43:33.396033 geomux-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3282 2023-07-31 23:43:33.396150 geomux-0.2.8/README.md
+-rw-r--r--   0        0        0      225 2023-07-31 23:43:33.429956 geomux-0.2.8/geomux/__init__.py
+-rw-r--r--   0        0        0     2569 2023-07-31 23:43:33.430040 geomux-0.2.8/geomux/__main__.py
+-rw-r--r--   0        0        0    14350 2023-07-31 23:43:33.430169 geomux-0.2.8/geomux/geomux.py
+-rw-r--r--   0        0        0     1005 2023-07-31 23:43:33.430246 geomux-0.2.8/geomux/utils.py
+-rw-r--r--   0        0        0      555 2023-08-02 16:51:08.933561 geomux-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3943 1970-01-01 00:00:00.000000 geomux-0.2.8/PKG-INFO
```

### Comparing `geomux-0.2.7/LICENSE` & `geomux-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `geomux-0.2.7/README.md` & `geomux-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `geomux-0.2.7/geomux/__main__.py` & `geomux-0.2.8/geomux/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,21 +29,29 @@
         type=int,
         required=False,
         default=100,
         help="minimum number of cells to consider a guide (default=100)",
     )
     parser.add_argument(
         "-t",
-        "--threshold",
+        "--pvalue_threshold",
         type=float,
         required=False,
         default=0.05,
         help="Pvalue threshold to use after pvalue correction (default=0.05)",
     )
     parser.add_argument(
+        "-T",
+        "--lor_threshold",
+        type=float,
+        required=False,
+        default=10.0,
+        help="Log odds ratio threshold to use (default=10.0)",
+    )
+    parser.add_argument(
         "-C",
         "--correction",
         type=str,
         required=False,
         default="bh",
         help="Pvalue correction method to use (default=bh)",
     )
@@ -51,21 +59,14 @@
         "-j",
         "--n_jobs",
         type=int,
         required=False,
         default=1,
         help="Number of jobs to use when calculating hypergeometric distributions (default=1)",
     )
-    parser.add_argument(
-        "-q",
-        "--quiet",
-        action="store_true",
-        required=False,
-        help="Suppress progress messages",
-    )
     args = parser.parse_args()
     return args
 
 
 def main_cli():
     args = get_args()
 
@@ -81,16 +82,18 @@
         matrix,
         cell_names=matrix.index.values,
         guide_names=matrix.columns.values,
         min_umi=args.min_umi,
         min_cells=args.min_cells,
         n_jobs=args.n_jobs,
         method=args.correction,
-        verbose=not args.quiet,
     )
     gx.test()
-    assignments = gx.assignments(threshold=args.threshold)
+    assignments = gx.assignments(
+        pvalue_threshold=args.pvalue_threshold,
+        lor_threshold=args.lor_threshold,
+    )
 
     if not args.output:
         assignments.to_csv(sys.stdout, sep="\t", index=False)
     else:
         assignments.to_csv(args.output, sep="\t", index=False)
```

### Comparing `geomux-0.2.7/geomux/utils.py` & `geomux-0.2.8/geomux/utils.py`

 * *Files identical despite different names*

### Comparing `geomux-0.2.7/pyproject.toml` & `geomux-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geomux"
-version = "0.2.7"
+version = "0.2.8"
 description = "A tool to assign identifiers to cell barcodes"
 authors = ["Noam Teyssier"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 geomux = 'geomux.__main__:main_cli'
```

### Comparing `geomux-0.2.7/PKG-INFO` & `geomux-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomux
-Version: 0.2.7
+Version: 0.2.8
 Summary: A tool to assign identifiers to cell barcodes
 License: MIT
 Author: Noam Teyssier
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

