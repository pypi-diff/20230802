# Comparing `tmp/ngff_zarr-0.4.5.tar.gz` & `tmp/ngff_zarr-0.4.6.tar.gz`

## Comparing `ngff_zarr-0.4.5.tar` & `ngff_zarr-0.4.6.tar`

### file list

```diff
@@ -1,59 +1,63 @@
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.readthedocs.yaml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.github/workflows/test.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/.gitignore
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/Makefile
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/cli.md
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/conf.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/development.md
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/make.bat
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/requirements.txt
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/_static/favicon.png
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/_static/logo.png
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/__about__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/__init__.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/_array_split.py
--rwxr-xr-x   0        0        0    10939 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/cli.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/cli_input_to_ngff_image.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/config.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/detect_cli_io_backend.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/from_ngff_zarr.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/itk_image_to_ngff_image.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/memory_usage.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/multiscales.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/ngff_image.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/ngff_image_to_itk_image.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/rich_dask_progress.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/task_count.py
--rw-r--r--   0        0        0    13466 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/to_multiscales.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/to_ngff_image.py
--rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/to_ngff_zarr.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/zarr_metadata.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/methods/__init__.py
--rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/methods/_dask_image.py
--rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/methods/_itk.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/methods/_support.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/__init__.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/_data.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_cli_input_to_ngff_image.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_detect_cli_input_backend.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_from_ngff_zarr.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_itk_image_to_ngff_image.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_large_serialization.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_memory_usage.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_ngff_image_scale_factors.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_ngff_image_to_itk_image.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_task_count.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_to_ngff_zarr_dask_image.py
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_to_ngff_zarr_itk.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/LICENSE.txt
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/README.md
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/.readthedocs.yaml
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/docs/.gitignore
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/docs/Makefile
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/docs/cli.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/docs/conf.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/docs/development.md
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/docs/make.bat
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/docs/requirements.txt
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/docs/_static/favicon.png
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/docs/_static/logo.png
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/__about__.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/__init__.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/_array_split.py
+-rwxr-xr-x   0        0        0    12281 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/cli.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/cli_input_to_ngff_image.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/config.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/detect_cli_io_backend.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/from_ngff_zarr.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/itk_image_to_ngff_image.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/memory_usage.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/multiscales.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/ngff_image.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/ngff_image_to_itk_image.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/rich_dask_progress.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/task_count.py
+-rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/to_multiscales.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/to_ngff_image.py
+-rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/to_ngff_zarr.py
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/zarr_metadata.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/methods/__init__.py
+-rw-r--r--   0        0        0    17565 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/methods/_dask_image.py
+-rw-r--r--   0        0        0    18445 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/methods/_itk.py
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/ngff_zarr/methods/_support.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/__init__.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/_data.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/conftest.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/test_cli_input_to_ngff_image.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/test_detect_cli_input_backend.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/test_from_ngff_zarr.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/test_itk_image_to_ngff_image.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/test_large_serialization.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/test_memory_usage.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/test_ngff_image_scale_factors.py
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/test_ngff_image_to_itk_image.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/test_task_count.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/test_to_ngff_zarr_dask_image.py
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/test/test_to_ngff_zarr_itk.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/LICENSE.txt
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/README.md
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 ngff_zarr-0.4.6/PKG-INFO
```

### Comparing `ngff_zarr-0.4.5/.readthedocs.yaml` & `ngff_zarr-0.4.6/.readthedocs.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 build:
   os: ubuntu-22.04
   tools:
     python: "3.11"
 
 # Build documentation in the "docs/" directory with Sphinx
 sphinx:
-   configuration: docs/conf.py
+  configuration: docs/conf.py
 
 # Optionally build your docs in additional formats such as PDF and ePub
 # formats:
 #    - pdf
 #    - epub
 
 # Optional but recommended, declare the Python requirements required
 # to build your documentation
 # See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
 python:
-   install:
-   - requirements: docs/requirements.txt
+  install:
+    - requirements: docs/requirements.txt
```

### Comparing `ngff_zarr-0.4.5/.github/workflows/test.yml` & `ngff_zarr-0.4.6/.github/workflows/test.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 name: Test
 
-on: [push,pull_request]
+on: [push, pull_request]
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       max-parallel: 5
       matrix:
         os: [ubuntu-22.04, windows-2022, macos-12]
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3
         with:
@@ -27,8 +27,8 @@
       - name: Test with pytest
         run: |
           pytest --junitxml=junit/test-results.xml
 
       - name: Publish Test Report
         uses: mikepenz/action-junit-report@v2
         with:
-          report_paths: 'junit/test-results*.xml'
+          report_paths: "junit/test-results*.xml"
```

### Comparing `ngff_zarr-0.4.5/.pytest_cache/v/cache/nodeids` & `ngff_zarr-0.4.6/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.5/docs/Makefile` & `ngff_zarr-0.4.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.5/docs/cli.md` & `ngff_zarr-0.4.6/docs/cli.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # Command Line Interface (CLI)
 
-`ngff-zarr` provides a command line interface to convert a variety of scientific file formats to ome-zarr and inspect and ome-zarr store's contents.
+`ngff-zarr` provides a command line interface to convert a variety of scientific
+file formats to ome-zarr and inspect and ome-zarr store's contents.
 
 ## Installation
 
 To install the command line interface (CLI):
 
 ```shell
 pip install 'ngff-zarr[cli]'
 ```
+
 ## Usage
 
 ### Convert an image file
 
-Convert any scientific image file format supported by either [itk](https://wasm.itk.org/docs/image_formats), [tifffile](https://pypi.org/project/tifffile/), or [imageio](https://imageio.readthedocs.io/en/stable/formats/index.html).
+Convert any scientific image file format supported by either
+[itk](https://wasm.itk.org/docs/image_formats),
+[tifffile](https://pypi.org/project/tifffile/), or
+[imageio](https://imageio.readthedocs.io/en/stable/formats/index.html).
 
 Example:
 
 ```shell
 ngff-zarr -i ./MR-head.nrrd -o ./MR-head.zarr
 ```
 
@@ -53,23 +58,23 @@
 
 ```shell
 ngff-zarr --dims "z" "y" "x" --scale x 1.4 y 1.4 z 2.5 --translation x 6.24 y 360.0 z 332.5 --name LIDC2 -i "series/*.tif"
 ```
 
 ![ngff-zarr metadata](https://i.imgur.com/AecFANr.png)
 
-
 ### Limit memory consumption
 
-Limit memory consumption by passing a rough memory limit in human-readable units, e.g. *8GB* with the `--memory-target` option.
+Limit memory consumption by passing a rough memory limit in human-readable
+units, e.g. _8GB_ with the `--memory-target` option.
 
 ```shell
 ngff-zarr --memory-target 50M -i ./LIDCFull.vtk -o ./LIDCFull.zarr
 ```
 
 ![ngff-zarr memory-target](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExZmQ2NzVmMzU0NDA5ZDcyNzczNTU3MWE2YjczZjY5YmJkNWE4OTRhZSZjdD1n/ODobGeUYQr9wrE9J2s/giphy.gif)
 
 ### More options
 
 ```shell
 ngff-zarr --help
-```
+```
```

### Comparing `ngff_zarr-0.4.5/docs/conf.py` & `ngff_zarr-0.4.6/docs/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 from datetime import date
 
-project = 'ngff-zarr'
-copyright = f'{date.today().year}, NumFOCUS'
-author = 'Matt McCormick'
+project = "ngff-zarr"
+copyright = f"{date.today().year}, NumFOCUS"
+author = "Matt McCormick"
 
 extensions = [
-    'sphinx.ext.autosummary',
-    'autodoc2',
-    'myst_parser',
-    'sphinx.ext.intersphinx',
-    'sphinx_copybutton',
-    'sphinxext.opengraph',
-    'sphinx_design',
+    "sphinx.ext.autosummary",
+    "autodoc2",
+    "myst_parser",
+    "sphinx.ext.intersphinx",
+    "sphinx_copybutton",
+    "sphinxext.opengraph",
+    "sphinx_design",
 ]
 
 myst_enable_extensions = ["colon_fence", "fieldlist"]
 
-templates_path = ['_templates']
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+templates_path = ["_templates"]
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 autodoc2_packages = [
     {
         "path": "../ngff_zarr",
         "exclude_files": ["__about__.py"],
     },
 ]
@@ -37,20 +37,20 @@
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
     "itkwasm": ("https://itkwasm.readthedocs.io/en/latest/", None),
     "dask": ("https://docs.dask.org/en/stable/", None),
 }
 
-html_theme = 'furo'
-html_static_path = ['_static']
+html_theme = "furo"
+html_static_path = ["_static"]
 html_logo = "_static/logo.png"
 html_favicon = "_static/favicon.png"
 html_title = f"{project}"
 
 # Furo options
 html_theme_options = {
     "top_of_page_button": "edit",
     "source_repository": "https://github.com/thewtex/ngff-zarr",
     "source_branch": "main",
     "source_directory": "docs",
-}
+}
```

### Comparing `ngff_zarr-0.4.5/docs/development.md` & `ngff_zarr-0.4.6/docs/development.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # Development
 
 Contributions are welcome and appreciated!
 
-We are glad you are here and appreciate your contribution. Please keep in mind our [community participation guidelines](https://github.com/InsightSoftwareConsortium/ITK/blob/master/CODE_OF_CONDUCT.md).
+We are glad you are here and appreciate your contribution. Please keep in mind
+our
+[community participation guidelines](https://github.com/InsightSoftwareConsortium/ITK/blob/master/CODE_OF_CONDUCT.md).
 
 To run the unit tests:
 
 ```sh
 pip install -e ".[test,dask-image,itk,cli]"
+pre-commit install
 pytest
 ```
 
 ### Updating test data
 
 1. Generate new test data tarball
 
@@ -19,8 +22,9 @@
 cd test/data
 tar cvf ../data.tar baseline input
 gzip -9 ../data.tar
 ```
 
 2. Upload the data to [web3.storage](https://web3.storage)
 
-3. Upload the `test_data_ipfs_cid` (from web3.storage web UI) and `test_data_sha256` (`sh256sum ../data.tar.gz`) variables in *test/_data.py*.
+3. Upload the `test_data_ipfs_cid` (from web3.storage web UI) and
+   `test_data_sha256` (`sh256sum ../data.tar.gz`) variables in _test/\_data.py_.
```

### Comparing `ngff_zarr-0.4.5/docs/index.md` & `ngff_zarr-0.4.6/docs/index.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,60 @@
-ngff-zarr
-=========
+# ngff-zarr
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ngff-zarr.svg)](https://pypi.org/project/ngff-zarr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ngff-zarr.svg)](https://pypi.org/project/ngff-zarr)
 [![Test](https://github.com/thewtex/ngff-zarr/actions/workflows/test.yml/badge.svg)](https://github.com/thewtex/ngff-zarr/actions/workflows/test.yml)
 [![DOI](https://zenodo.org/badge/541840158.svg)](https://zenodo.org/badge/latestdoi/541840158)
 [![Documentation Status](https://readthedocs.org/projects/ngff-zarr/badge/?version=latest)](https://ngff-zarr.readthedocs.io/en/latest/?badge=latest)
 
-A lean and kind Open Microscopy Environment (OME) Next Generation File Format (NGFF) Zarr implementation.
+A lean and kind Open Microscopy Environment (OME) Next Generation File Format
+(NGFF) Zarr implementation.
 
 ## Features
 
 - Minimal dependencies
 - Work with arbitrary Zarr store types
 - Lazy, parallel, and web ready -- no local filesystem required
 - Process extremely large datasets
 - Multiple downscaling methods
 - Supports Python>=3.7
-- Implements version 0.4 of the [OME-Zarr
-NGFF specification](https://github.com/ome/ngff)
+- Implements version 0.4 of the
+  [OME-Zarr NGFF specification](https://github.com/ome/ngff)
 
 ## Installation
 
 ::::{tab-set}
 
 :::{tab-item} System
+
 ```shell
 pip install 'ngff-zarr[cli]'
 ```
+
 :::
 
-:::{tab-item} Browser
-In Pyodide, e.g. the [Pyodide REPL](https://pyodide.org/en/stable/console.html) or [JupyterLite](https://jupyterlite.readthedocs.io/en/latest/try/lab),
+:::{tab-item} Browser In Pyodide, e.g. the
+[Pyodide REPL](https://pyodide.org/en/stable/console.html) or
+[JupyterLite](https://jupyterlite.readthedocs.io/en/latest/try/lab),
 
-```python
+````python
 import micropip
 await micropip.install('ngff-zarr')
 :::
 
 ::::
 
 ```{toctree}
 :hidden:
 :maxdepth: 3
 
 cli.md
 development.md
-```
+````
 
 ```{toctree}
 :hidden:
 :maxdepth: 3
 :caption: 📖 Reference
 
 apidocs/index.rst
-```
+```
```

### Comparing `ngff_zarr-0.4.5/docs/make.bat` & `ngff_zarr-0.4.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.5/docs/_static/favicon.png` & `ngff_zarr-0.4.6/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.5/docs/_static/logo.png` & `ngff_zarr-0.4.6/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.5/ngff_zarr/__init__.py` & `ngff_zarr-0.4.6/ngff_zarr/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-FileCopyrightText: 2022-present Matt McCormick <matt.mccormick@kitware.com>
 #
 # SPDX-License-Identifier: MIT
 
-from .to_ngff_image import to_ngff_image
+from .__about__ import __version__
+from .cli_input_to_ngff_image import cli_input_to_ngff_image
+from .config import config
+from .detect_cli_io_backend import ConversionBackend, detect_cli_io_backend
 from .from_ngff_zarr import from_ngff_zarr
 from .itk_image_to_ngff_image import itk_image_to_ngff_image
-from .ngff_image_to_itk_image import ngff_image_to_itk_image
-from .detect_cli_io_backend import detect_cli_io_backend, ConversionBackend
-from .cli_input_to_ngff_image import cli_input_to_ngff_image
-from .__about__ import __version__
-from .ngff_image import NgffImage
-from .multiscales import Multiscales
 from .memory_usage import memory_usage
+from .methods import Methods
+from .multiscales import Multiscales
+from .ngff_image import NgffImage
+from .ngff_image_to_itk_image import ngff_image_to_itk_image
 from .task_count import task_count
-from .to_multiscales import to_multiscales, Multiscales
+from .to_multiscales import to_multiscales
+from .to_ngff_image import to_ngff_image
 from .to_ngff_zarr import to_ngff_zarr
-from .methods import Methods
-from .config import config
 
 __all__ = [
     "__version__",
     "config",
     "NgffImage",
     "Multiscales",
     "to_ngff_image",
@@ -28,11 +28,12 @@
     "itk_image_to_ngff_image",
     "ngff_image_to_itk_image",
     "memory_usage",
     "task_count",
     "to_multiscales",
     "Methods",
     "to_ngff_zarr",
+    "from_ngff_zarr",
     "detect_cli_io_backend",
     "ConversionBackend",
     "cli_input_to_ngff_image",
 ]
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/_array_split.py` & `ngff_zarr-0.4.6/ngff_zarr/_array_split.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import numpy as np
 import dask.array
+import numpy as np
+
 
 def _array_split(ary, indices_or_sections, axis=0):
     """
     *** From NumPy, adapted for Dask Array's
 
     Split an array into multiple sub-arrays.
 
@@ -32,29 +33,28 @@
     try:
         Ntotal = ary.shape[axis]
     except AttributeError:
         Ntotal = len(ary)
     try:
         # handle array case.
         Nsections = len(indices_or_sections) + 1
-        div_points = [0] + list(indices_or_sections) + [Ntotal]
+        div_points = [0, *list(indices_or_sections), Ntotal]
     except TypeError:
         # indices_or_sections is a scalar, not an array.
         Nsections = int(indices_or_sections)
         if Nsections <= 0:
-            raise ValueError('number sections must be larger than 0.') from None
+            msg = "number sections must be larger than 0."
+            raise ValueError(msg) from None
         Neach_section, extras = divmod(Ntotal, Nsections)
-        section_sizes = ([0] +
-                         extras * [Neach_section+1] +
-                         (Nsections-extras) * [Neach_section])
+        section_sizes = (
+            [0] + extras * [Neach_section + 1] + (Nsections - extras) * [Neach_section]
+        )
         div_points = np.array(section_sizes, dtype=np.intp).cumsum()
 
     sub_arys = []
     sary = dask.array.swapaxes(ary, axis, 0)
     for i in range(Nsections):
         st = div_points[i]
         end = div_points[i + 1]
         sub_arys.append(dask.array.swapaxes(sary[st:end], axis, 0))
 
     return sub_arys
-
-
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/cli.py` & `ngff_zarr-0.4.6/ngff_zarr/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,162 +1,282 @@
 #!/usr/bin/env python
 
 if __name__ == "__main__" and __package__ is None:
     __package__ = "ngff_zarr"
 
-import sys
 import argparse
-from pathlib import Path
 import atexit
 import signal
-import os
+import sys
+from pathlib import Path
 
-from rich.progress import Progress as RichProgress, SpinnerColumn, TimeElapsedColumn, MofNCompleteColumn
+import dask.utils
+import zarr
 from rich.console import Console
-from rich.panel import Panel
 from rich.live import Live
+from rich.panel import Panel
 from rich.pretty import Pretty
+from rich.progress import (
+    MofNCompleteColumn,
+    SpinnerColumn,
+    TimeElapsedColumn,
+)
+from rich.progress import (
+    Progress as RichProgress,
+)
 from rich.spinner import Spinner
 from zarr.storage import DirectoryStore
-import zarr
-import dask.utils
 
-from .ngff_image import NgffImage
-from .to_multiscales import to_multiscales
-from .to_ngff_image import to_ngff_image
-from .to_ngff_zarr import to_ngff_zarr
-from .from_ngff_zarr import from_ngff_zarr
 from .cli_input_to_ngff_image import cli_input_to_ngff_image
-from .ngff_image_to_itk_image import ngff_image_to_itk_image
-from .detect_cli_io_backend import detect_cli_io_backend, ConversionBackend, conversion_backends_values
+from .config import config
+from .detect_cli_io_backend import (
+    ConversionBackend,
+    conversion_backends_values,
+    detect_cli_io_backend,
+)
+from .from_ngff_zarr import from_ngff_zarr
 from .methods import Methods, methods_values
+from .ngff_image_to_itk_image import ngff_image_to_itk_image
 from .rich_dask_progress import NgffProgress, NgffProgressCallback
-from .zarr_metadata import is_dimension_supported, is_unit_supported
-from .config import config
+from .to_multiscales import to_multiscales
+from .to_ngff_image import to_ngff_image
+from .to_ngff_zarr import to_ngff_zarr
+from .zarr_metadata import is_unit_supported
 
-def _multiscales_to_ngff_zarr(live, args, output_store, rich_dask_progress, multiscales):
+
+def _multiscales_to_ngff_zarr(
+    live, args, output_store, rich_dask_progress, multiscales
+):
     if not args.output:
         if args.quiet:
             live.update(Pretty(multiscales))
         else:
-            live.update(Panel(Pretty(multiscales), title="[red]NGFF OME-Zarr", subtitle="[red]information", style="magenta"))
+            live.update(
+                Panel(
+                    Pretty(multiscales),
+                    title="[red]NGFF OME-Zarr",
+                    subtitle="[red]information",
+                    style="magenta",
+                )
+            )
         return
     to_ngff_zarr(output_store, multiscales, progress=rich_dask_progress)
 
-def _ngff_image_to_multiscales(live, ngff_image, args, progress, rich_dask_progress, subtitle, method):
+
+def _ngff_image_to_multiscales(
+    live, ngff_image, args, progress, rich_dask_progress, subtitle, method
+):
     data = ngff_image.data
     if args.dims:
         if len(args.dims) != len(ngff_image.dims):
-            live.console.print(f"[red]Provided number of dims do not match expected: {len(ngff_image.dims)}")
+            live.console.print(
+                f"[red]Provided number of dims do not match expected: {len(ngff_image.dims)}"
+            )
             sys.exit(1)
         ngff_image.dims = args.dims
     if args.scale:
         if len(args.scale) % 2 != 0:
-            live.console.print(f"[red]Provided scales are expected to be dim value pairs")
+            live.console.print(
+                "[red]Provided scales are expected to be dim value pairs"
+            )
             sys.exit(1)
         n_scale_args = len(args.scale) // 2
         for scale in range(n_scale_args):
-            dim = args.scale[scale*2]
-            value = float(args.scale[scale*2+1])
+            dim = args.scale[scale * 2]
+            value = float(args.scale[scale * 2 + 1])
             ngff_image.scale[dim] = value
     if args.translation:
         if len(args.translation) % 2 != 0:
-            live.console.print(f"[red]Provided translations are expected to be dim value pairs")
+            live.console.print(
+                "[red]Provided translations are expected to be dim value pairs"
+            )
             sys.exit(1)
         n_translation_args = len(args.translation) // 2
         for translation in range(n_translation_args):
-            dim = args.translation[translation*2]
-            value = float(args.translation[translation*2+1])
-            ngff_image.translation[dim] = value    
+            dim = args.translation[translation * 2]
+            value = float(args.translation[translation * 2 + 1])
+            ngff_image.translation[dim] = value
     if args.units:
         if len(args.units) % 2 != 0:
-            live.console.print(f"[red]Provided units are expected to be dim value pairs, i.e. \"x\" \"meter\" ...")
+            live.console.print(
+                '[red]Provided units are expected to be dim value pairs, i.e. "x" "meter" ...'
+            )
             sys.exit(1)
-        unit_pairs = {str(args.units[unit*2]).lower(): str(args.units[unit*2+1]).lower()
-                        for unit in range(len(args.units) // 2)}
-        unsupported_units = [value for value in unit_pairs.values() if not is_unit_supported(value)]
+        unit_pairs = {
+            str(args.units[unit * 2]).lower(): str(args.units[unit * 2 + 1]).lower()
+            for unit in range(len(args.units) // 2)
+        }
+        unsupported_units = [
+            value for value in unit_pairs.values() if not is_unit_supported(value)
+        ]
         if any(unsupported_units):
-            live.console.print(f"[red]The following unit(s) were requested but are not supported: {unsupported_units}")
+            live.console.print(
+                f"[red]The following unit(s) were requested but are not supported: {unsupported_units}"
+            )
             sys.exit(1)
         ngff_image.axes_units = unit_pairs
     if args.name:
         ngff_image.name = args.name
 
     # Generate Multiscales
     cache = data.nbytes > config.memory_target
     if not args.output:
         cache = False
     if not args.quiet:
-        live.update(Panel(progress, title="[red]NGFF OME-Zarr", subtitle=subtitle, style="magenta"))
+        live.update(
+            Panel(
+                progress, title="[red]NGFF OME-Zarr", subtitle=subtitle, style="magenta"
+            )
+        )
     chunks = args.chunks
     if chunks is not None:
-        if len(chunks) == 1:
-            chunks = chunks[0]
-        else:
-            chunks = tuple(chunks)
-    multiscales = to_multiscales(ngff_image, method=method, progress=rich_dask_progress, chunks=chunks, cache=cache)
-    return multiscales
+        chunks = chunks[0] if len(chunks) == 1 else tuple(chunks)
+    return to_multiscales(
+        ngff_image,
+        method=method,
+        progress=rich_dask_progress,
+        chunks=chunks,
+        cache=cache,
+    )
 
 
 def main():
-    parser = argparse.ArgumentParser(description='Convert datasets to and from the OME-Zarr Next Generation File Format.')
-    parser.add_argument('-i', '--input', nargs='+', help='Input image(s)', required=True)
-    parser.add_argument('-o', '--output', help='Output image. If not specified just print information to stdout.')
+    parser = argparse.ArgumentParser(
+        description="Convert datasets to and from the OME-Zarr Next Generation File Format."
+    )
+    parser.add_argument(
+        "-i", "--input", nargs="+", help="Input image(s)", required=True
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        help="Output image. If not specified just print information to stdout.",
+    )
 
     metadata_group = parser.add_argument_group("metadata", "Specify output metadata")
-    metadata_group.add_argument('-d', '--dims', nargs='+', help='Ordered OME-Zarr NGFF dimensions from {"t", "z", "y", "x", "c"}', metavar='DIM')
-    metadata_group.add_argument('-u', '--units', nargs='+', help='Ordered OME-Zarr NGFF axes spatial or temporal units', metavar='UNITS')
-    metadata_group.add_argument('-s', '--scale', nargs='+', help='Override scale / spacing for each dimension, e.g. z 4.0 y 1.0 x 1.0', metavar='SCALE')
-    metadata_group.add_argument('-t', '--translation', nargs='+', help='Override translation / origin for each dimension, e.g. z 0.0 y 50.0 x 40.0', metavar='TRANSLATION')
-    metadata_group.add_argument('-n', '--name', help="Image name")
-    metadata_group.add_argument('--output-scale', help="Scale to pick from multiscale input for a single-scale output format", type=int, default=0)
+    metadata_group.add_argument(
+        "-d",
+        "--dims",
+        nargs="+",
+        help='Ordered OME-Zarr NGFF dimensions from {"t", "z", "y", "x", "c"}',
+        metavar="DIM",
+    )
+    metadata_group.add_argument(
+        "-u",
+        "--units",
+        nargs="+",
+        help="Ordered OME-Zarr NGFF axes spatial or temporal units",
+        metavar="UNITS",
+    )
+    metadata_group.add_argument(
+        "-s",
+        "--scale",
+        nargs="+",
+        help="Override scale / spacing for each dimension, e.g. z 4.0 y 1.0 x 1.0",
+        metavar="SCALE",
+    )
+    metadata_group.add_argument(
+        "-t",
+        "--translation",
+        nargs="+",
+        help="Override translation / origin for each dimension, e.g. z 0.0 y 50.0 x 40.0",
+        metavar="TRANSLATION",
+    )
+    metadata_group.add_argument("-n", "--name", help="Image name")
+    metadata_group.add_argument(
+        "--output-scale",
+        help="Scale to pick from multiscale input for a single-scale output format",
+        type=int,
+        default=0,
+    )
 
     processing_group = parser.add_argument_group("processing", "Processing options")
-    processing_group.add_argument('-c', '--chunks', nargs='+', type=int, help='Dask array chunking specification, either a single integer or integer per dimension, e.g. 64 or 8 16 32', metavar='CHUNKS')
-    processing_group.add_argument('-m', '--method', default="dask_image_gaussian", choices=methods_values, help="Downsampling method")
-    processing_group.add_argument('-q', '--quiet', action='store_true', help='Do not display progress information')
-    processing_group.add_argument('-l', '--local-cluster', action='store_true', help='Create a Dask Distributed LocalCluster. Better for large datasets.')
-    processing_group.add_argument('--input-backend', choices=conversion_backends_values, help='Input conversion backend')
-    processing_group.add_argument('--memory-target', help='Memory limit, e.g. 4GB')
-    processing_group.add_argument('--cache-dir', help='Directory to use for caching with large datasets')
+    processing_group.add_argument(
+        "-c",
+        "--chunks",
+        nargs="+",
+        type=int,
+        help="Dask array chunking specification, either a single integer or integer per dimension, e.g. 64 or 8 16 32",
+        metavar="CHUNKS",
+    )
+    processing_group.add_argument(
+        "-m",
+        "--method",
+        default="dask_image_gaussian",
+        choices=methods_values,
+        help="Downsampling method",
+    )
+    processing_group.add_argument(
+        "-q", "--quiet", action="store_true", help="Do not display progress information"
+    )
+    processing_group.add_argument(
+        "-l",
+        "--local-cluster",
+        action="store_true",
+        help="Create a Dask Distributed LocalCluster. Better for large datasets.",
+    )
+    processing_group.add_argument(
+        "--input-backend",
+        choices=conversion_backends_values,
+        help="Input conversion backend",
+    )
+    processing_group.add_argument("--memory-target", help="Memory limit, e.g. 4GB")
+    processing_group.add_argument(
+        "--cache-dir", help="Directory to use for caching with large datasets"
+    )
 
     args = parser.parse_args()
 
     if args.memory_target:
         config.memory_target = dask.utils.parse_bytes(args.memory_target)
 
     if args.cache_dir:
         cache_dir = Path(args.cache_dir).resolve()
         if not cache_dir.exists():
-            os.makedirs(cache_dir)
-        config.cache_store = zarr.storage.DirectoryStore(cache_dir,
-                dimension_separator='/')
+            Path.makedirs(cache_dir, parents=True)
+        config.cache_store = zarr.storage.DirectoryStore(
+            cache_dir, dimension_separator="/"
+        )
 
     console = Console()
-    progress = RichProgress(SpinnerColumn(), MofNCompleteColumn(), TimeElapsedColumn(), *RichProgress.get_default_columns(), transient=False, console=console)
+    progress = RichProgress(
+        SpinnerColumn(),
+        MofNCompleteColumn(),
+        TimeElapsedColumn(),
+        *RichProgress.get_default_columns(),
+        transient=False,
+        console=console,
+    )
     rich_dask_progress = None
 
     # Setup LocalCluster
     if args.local_cluster:
         from dask.distributed import Client, LocalCluster
 
         n_workers = 4
         worker_memory_target = config.memory_target // n_workers
         try:
             import psutil
+
             n_workers = psutil.cpu_count(False) // 2
             worker_memory_target = config.memory_target // n_workers
         except ImportError:
             pass
 
-        cluster = LocalCluster(n_workers=n_workers, memory_target=worker_memory_target, processes=True, threads_per_worker=2)
+        cluster = LocalCluster(
+            n_workers=n_workers,
+            memory_target=worker_memory_target,
+            processes=True,
+            threads_per_worker=2,
+        )
         client = Client(cluster)
 
-        def shutdown_client(sig_id, frame):
+        def shutdown_client(sig_id, frame):  # noqa: ARG001
             client.shutdown()
+
         atexit.register(shutdown_client, None, None)
         signal.signal(signal.SIGTERM, shutdown_client)
         signal.signal(signal.SIGINT, shutdown_client)
 
         if not args.quiet:
             console.log(f"[yellow]Dashboard: [cyan]{client.dashboard_link}")
 
@@ -168,63 +288,87 @@
             rich_dask_progress.register()
 
     # Parse conversion options
     if args.input_backend is None:
         input_backend = detect_cli_io_backend(args.input)
     else:
         input_backend = ConversionBackend(args.input_backend)
-    if args.method is None:
-        method = Methods.ITK_GAUSSIAN
-    else:
-        method = Methods(args.method)
+    method = Methods.ITK_GAUSSIAN if args.method is None else Methods(args.method)
 
     if args.output:
-        output_backend = detect_cli_io_backend([args.output,])
+        output_backend = detect_cli_io_backend(
+            [
+                args.output,
+            ]
+        )
     output_store = None
     if args.output and output_backend is ConversionBackend.NGFF_ZARR:
-        output_store = DirectoryStore(args.output, dimension_separator='/')
+        output_store = DirectoryStore(args.output, dimension_separator="/")
 
     subtitle = "[red]generation"
     if not args.output:
         subtitle = "[red]information"
-    initial = Panel(Spinner('point', text="Loading input..."), title="[red]NGFF OME-Zarr", subtitle=subtitle, style="magenta")
+    initial = Panel(
+        Spinner("point", text="Loading input..."),
+        title="[red]NGFF OME-Zarr",
+        subtitle=subtitle,
+        style="magenta",
+    )
     if args.quiet:
         initial = None
     with Live(initial, console=console) as live:
-        if args.output:
-            if output_backend is ConversionBackend.ITK:
-                import itk
-                ngff_image = cli_input_to_ngff_image(input_backend, args.input, args.output_scale)
-                if isinstance(rich_dask_progress, NgffProgressCallback):
-                    rich_dask_progress.add_callback_task(f"[green]Converting Zarr Array to NumPy Array")
-                itk_image = ngff_image_to_itk_image(ngff_image, wasm=False)
-                itk.imwrite(itk_image, args.output)
-                return
+        if args.output and output_backend is ConversionBackend.ITK:
+            import itk
+
+            ngff_image = cli_input_to_ngff_image(
+                input_backend, args.input, args.output_scale
+            )
+            if isinstance(rich_dask_progress, NgffProgressCallback):
+                rich_dask_progress.add_callback_task(
+                    "[green]Converting Zarr Array to NumPy Array"
+                )
+            itk_image = ngff_image_to_itk_image(ngff_image, wasm=False)
+            itk.imwrite(itk_image, args.output)
+            return
 
         if input_backend is ConversionBackend.NGFF_ZARR:
             store = zarr.storage.DirectoryStore(args.input[0])
             multiscales = from_ngff_zarr(store)
-            _multiscales_to_ngff_zarr(live, args, output_store, rich_dask_progress, multiscales)
+            _multiscales_to_ngff_zarr(
+                live, args, output_store, rich_dask_progress, multiscales
+            )
         elif input_backend is ConversionBackend.TIFFFILE:
             try:
                 import tifffile
-                if len(args.input) == 1:
-                    files = args.input[0]
-                else:
-                    files = args.input
+
+                files = args.input[0] if len(args.input) == 1 else args.input
                 with tifffile.imread(files, aszarr=True) as store:
-                    root = zarr.open(store, mode='r')
+                    root = zarr.open(store, mode="r")
                     ngff_image = to_ngff_image(root)
-                    multiscales = _ngff_image_to_multiscales(live, ngff_image, args, progress, rich_dask_progress, subtitle, method)
-                    _multiscales_to_ngff_zarr(live, args, output_store, rich_dask_progress, multiscales)
+                    multiscales = _ngff_image_to_multiscales(
+                        live,
+                        ngff_image,
+                        args,
+                        progress,
+                        rich_dask_progress,
+                        subtitle,
+                        method,
+                    )
+                    _multiscales_to_ngff_zarr(
+                        live, args, output_store, rich_dask_progress, multiscales
+                    )
             except ImportError:
-                print('[red]Please install the [i]tifffile[/i] package.')
+                sys.stdout.write("[red]Please install the [i]tifffile[/i] package.\n")
                 sys.exit(1)
         else:
             # Generate NgffImage
             ngff_image = cli_input_to_ngff_image(input_backend, args.input)
-            multiscales = _ngff_image_to_multiscales(live, ngff_image, args,
-                    progress, rich_dask_progress, subtitle, method)
-            _multiscales_to_ngff_zarr(live, args, output_store, rich_dask_progress, multiscales)
+            multiscales = _ngff_image_to_multiscales(
+                live, ngff_image, args, progress, rich_dask_progress, subtitle, method
+            )
+            _multiscales_to_ngff_zarr(
+                live, args, output_store, rich_dask_progress, multiscales
+            )
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/cli_input_to_ngff_image.py` & `ngff_zarr-0.4.6/ngff_zarr/cli_input_to_ngff_image.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,76 @@
 import sys
 
-from rich import print
-from dask.array.image import imread as daimread
 import zarr
+from dask.array.image import imread as daimread
+from rich import print
 
 from .detect_cli_io_backend import ConversionBackend
+from .from_ngff_zarr import from_ngff_zarr
+from .itk_image_to_ngff_image import itk_image_to_ngff_image
 from .ngff_image import NgffImage
 from .to_ngff_image import to_ngff_image
-from .itk_image_to_ngff_image import itk_image_to_ngff_image
-from .from_ngff_zarr import from_ngff_zarr
 
-def cli_input_to_ngff_image(backend: ConversionBackend, input, output_scale: int=0) -> NgffImage:
+
+def cli_input_to_ngff_image(
+    backend: ConversionBackend, input, output_scale: int = 0
+) -> NgffImage:
     if backend is ConversionBackend.NGFF_ZARR:
         store = zarr.storage.DirectoryStore(input[0])
         multiscales = from_ngff_zarr(store)
         return multiscales.images[output_scale]
-    elif backend is ConversionBackend.ZARR_ARRAY:
-        arr = zarr.open_array(input[0], mode='r')
+    if backend is ConversionBackend.ZARR_ARRAY:
+        arr = zarr.open_array(input[0], mode="r")
         return to_ngff_image(arr)
-    elif backend is ConversionBackend.ITK:
+    if backend is ConversionBackend.ITK:
         try:
             import itk
         except ImportError:
-            print('[red]Please install the [i]itk-io[/i] package.')
+            print("[red]Please install the [i]itk-io[/i] package.")
             sys.exit(1)
         if len(input) == 1:
-            if '*' in str(input[0]):
+            if "*" in str(input[0]):
+
                 def imread(filename):
                     image = itk.imread(filename)
                     return itk.array_from_image(image)
+
                 da = daimread(str(input[0]), imread=imread)
                 return to_ngff_image(da)
-            else:
-                image = itk.imread(input[0])
-                return itk_image_to_ngff_image(image)
+            image = itk.imread(input[0])
+            return itk_image_to_ngff_image(image)
         image = itk.imread(input)
         return itk_image_to_ngff_image(image)
-    elif backend is ConversionBackend.TIFFFILE:
+    if backend is ConversionBackend.TIFFFILE:
         try:
             import tifffile
         except ImportError:
-            print('[red]Please install the [i]tifffile[/i] package.')
+            print("[red]Please install the [i]tifffile[/i] package.")
             sys.exit(1)
         if len(input) == 1:
             store = tifffile.imread(input[0], aszarr=True)
         else:
             store = tifffile.imread(input, aszarr=True)
-        root = zarr.open(store, mode='r')
+        root = zarr.open(store, mode="r")
         return to_ngff_image(root)
-    elif backend is ConversionBackend.IMAGEIO:
+    if backend is ConversionBackend.IMAGEIO:
         try:
-            import imageio
+            import imageio.v3 as iio
         except ImportError:
-            print('[red]Please install the [i]imageio[/i] package.')
+            print("[red]Please install the [i]imageio[/i] package.")
             sys.exit(1)
-        import imageio.v3 as iio
+
         image = iio.imread(str(input[0]))
 
         ngff_image = to_ngff_image(image)
 
         props = iio.improps(str(input[0]))
         if props.spacing is not None:
-            if len(spacing) == 1:
-                scale = {d: spacing for d in ngff_image.dims}
+            if len(props.spacing) == 1:
+                scale = {d: props.spacing for d in ngff_image.dims}
                 ngff_image.scale = scale
             else:
-                scale = {d: spacing[i] for i, d in enumerate(ngff_image.dims)}
+                scale = {d: props.spacing[i] for i, d in enumerate(ngff_image.dims)}
                 ngff_image.scale = scale
 
         return ngff_image
+    return None
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/config.py` & `ngff_zarr-0.4.6/ngff_zarr/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from dataclasses import dataclass, field
-
 from pathlib import Path
+
+import dask.config
+import zarr
 from platformdirs import user_cache_dir
 from zarr.storage import StoreLike
-import zarr
-import dask.config
 
-if dask.config.get('temporary-directory') is not None:
-    _store_dir = dask.config.get('temporary-directory')
+if dask.config.get("temporary-directory") is not None:
+    _store_dir = dask.config.get("temporary-directory")
 else:
-    _store_dir = Path(user_cache_dir('ngff-zarr'))
+    _store_dir = Path(user_cache_dir("ngff-zarr"))
+
+
 def default_store_factory():
-    return zarr.storage.DirectoryStore(_store_dir, dimension_separator='/')
+    return zarr.storage.DirectoryStore(_store_dir, dimension_separator="/")
+
 
 try:
     import psutil
-    default_memory_target = int(psutil.virtual_memory().available*0.5)
+
+    default_memory_target = int(psutil.virtual_memory().available * 0.5)
 except ImportError:
     default_memory_target = int(1e9)
 
 
 @dataclass
 class NgffZarrConfig:
     # Rough memory target in bytes
     memory_target: int = default_memory_target
     task_target: int = 50000
     cache_store: StoreLike = field(default_factory=default_store_factory)
 
+
 config = NgffZarrConfig()
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/detect_cli_io_backend.py` & `ngff_zarr-0.4.6/ngff_zarr/detect_cli_io_backend.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,75 @@
+import sys
 from enum import Enum
 from pathlib import Path
 from typing import List
 
-conversion_backends = [("NGFF_ZARR", "ngff_zarr"),
-        ("ZARR_ARRAY", "zarr"),
-        ("ITK", "itk"),
-        ("TIFFFILE", "tifffile"),
-        ("IMAGEIO", "imageio")]
+conversion_backends = [
+    ("NGFF_ZARR", "ngff_zarr"),
+    ("ZARR_ARRAY", "zarr"),
+    ("ITK", "itk"),
+    ("TIFFFILE", "tifffile"),
+    ("IMAGEIO", "imageio"),
+]
 conversion_backends_values = [b[1] for b in conversion_backends]
 ConversionBackend = Enum("ConversionBackend", conversion_backends)
 
+
 def detect_cli_io_backend(input: List[str]) -> ConversionBackend:
-    if (Path(input[0]) / '.zarray').exists():
+    if (Path(input[0]) / ".zarray").exists():
         return ConversionBackend.ZARR_ARRAY
 
-    extension = ''.join(Path(input[0]).suffixes).lower()
+    extension = "".join(Path(input[0]).suffixes).lower()
 
-    ngff_zarr_supported_extensions = (
-        '.zarr',
-        )
+    ngff_zarr_supported_extensions = (".zarr",)
     if extension in ngff_zarr_supported_extensions:
         return ConversionBackend.NGFF_ZARR
 
     itk_supported_extensions = (
-            '.bmp',
-            '.dcm',
-            '.gipl',
-            '.hdf5',
-            '.jpg',
-            '.jpeg',
-            '.iwi',
-            '.iwi.cbor',
-            '.lsm',
-            '.mnc',
-            '.mnc.gz',
-            '.mnc2',
-            '.mgh',
-            '.mhz',
-            '.mha',
-            '.mhd',
-            '.mrc',
-            '.nia',
-            '.nii',
-            '.nii.gz',
-            '.hdr',
-            '.nrrd',
-            '.nhdr',
-            '.png',
-            '.pic',
-            '.vtk',
-            '.isq', # Requires pip install itk-ioscanco,
-            '.fdf', # Requires pip install itk-iofdf
-            )
+        ".bmp",
+        ".dcm",
+        ".gipl",
+        ".hdf5",
+        ".jpg",
+        ".jpeg",
+        ".iwi",
+        ".iwi.cbor",
+        ".lsm",
+        ".mnc",
+        ".mnc.gz",
+        ".mnc2",
+        ".mgh",
+        ".mhz",
+        ".mha",
+        ".mhd",
+        ".mrc",
+        ".nia",
+        ".nii",
+        ".nii.gz",
+        ".hdr",
+        ".nrrd",
+        ".nhdr",
+        ".png",
+        ".pic",
+        ".vtk",
+        ".isq",  # Requires pip install itk-ioscanco,
+        ".fdf",  # Requires pip install itk-iofdf
+    )
 
     if extension in itk_supported_extensions:
         return ConversionBackend.ITK
 
     try:
         import tifffile
-        tifffile_supported_extensions = [f".{ext}" for ext in tifffile.TIFF.FILE_EXTENSIONS]
+
+        tifffile_supported_extensions = [
+            f".{ext}" for ext in tifffile.TIFF.FILE_EXTENSIONS
+        ]
         if extension in tifffile_supported_extensions:
             return ConversionBackend.TIFFFILE
     except ImportError:
-        console.log('[red]Please install the [i]tifffile[/i] package')
+        from rich import print
 
-    return ConversionBackend.IMAGEIO
+        print("[red]Please install the [i]tifffile[/i] package")
+        sys.exit(1)
 
+    return ConversionBackend.IMAGEIO
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/from_ngff_zarr.py` & `ngff_zarr-0.4.6/ngff_zarr/from_ngff_zarr.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import Union, Optional
 from collections.abc import MutableMapping
 from pathlib import Path
+from typing import Union
 
-from zarr.storage import BaseStore
-import zarr
 import dask.array
+import zarr
+from zarr.storage import BaseStore
 
-from .to_multiscales import Multiscales
 from .ngff_image import NgffImage
-from .zarr_metadata import Metadata, Axis, Dataset, Scale, Translation
+from .to_multiscales import Multiscales
+from .zarr_metadata import Axis, Dataset, Metadata, Scale, Translation
+
 
 def from_ngff_zarr(
     store: Union[MutableMapping, str, Path, BaseStore],
 ) -> Multiscales:
     """
     Read an OME-Zarr NGFF Multiscales data structure from a Zarr store.
 
@@ -23,50 +24,57 @@
     Returns
     -------
 
     multiscales: multiscale ngff image with dask-chunked arrays for data
 
     """
 
-    root = zarr.open_group(store, mode='r')
+    root = zarr.open_group(store, mode="r")
     metadata = root.attrs["multiscales"][0]
 
     dims = [a["name"] for a in metadata["axes"]]
 
     name = "image"
     if name in metadata:
         name = metadata["name"]
 
-    units = { d: None for d in dims }
+    units = {d: None for d in dims}
     for axis in metadata["axes"]:
-       if "unit" in axis:
-          units[axis["name"]] = axis["unit"]
+        if "unit" in axis:
+            units[axis["name"]] = axis["unit"]
 
     images = []
     datasets = []
     for dataset in metadata["datasets"]:
         data = dask.array.from_zarr(store, component=dataset["path"])
 
-        scale = { d: 1.0 for d in dims }
-        translation = { d: 0.0 for d in dims }
+        scale = {d: 1.0 for d in dims}
+        translation = {d: 0.0 for d in dims}
         coordinateTransformations = []
         for transformation in dataset["coordinateTransformations"]:
-            if 'scale' in transformation:
+            if "scale" in transformation:
                 scale = transformation["scale"]
-                scale = { d: s for d, s in zip(dims, scale)}
+                scale = dict(zip(dims, scale))
                 coordinateTransformations.append(Scale(transformation["scale"]))
-            elif 'translation' in transformation:
+            elif "translation" in transformation:
                 translation = transformation["translation"]
-                translation = { d: t for d, t in zip(dims, translation)}
-                coordinateTransformations.append(Translation(transformation["translation"]))
-        datasets.append(Dataset(path=dataset["path"], coordinateTransformations=coordinateTransformations))
+                translation = dict(zip(dims, translation))
+                coordinateTransformations.append(
+                    Translation(transformation["translation"])
+                )
+        datasets.append(
+            Dataset(
+                path=dataset["path"],
+                coordinateTransformations=coordinateTransformations,
+            )
+        )
 
         ngff_image = NgffImage(data, dims, scale, translation, name, units)
         images.append(ngff_image)
 
     metadata.pop("@type", None)
     axes = [Axis(**axis) for axis in metadata["axes"]]
-    metadata = Metadata(axes=axes, datasets=datasets, name=name, version=metadata["version"])
-
-    multiscales = Multiscales(images, metadata)
+    metadata = Metadata(
+        axes=axes, datasets=datasets, name=name, version=metadata["version"]
+    )
 
-    return multiscales
+    return Multiscales(images, metadata)
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/itk_image_to_ngff_image.py` & `ngff_zarr-0.4.6/ngff_zarr/itk_image_to_ngff_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from dataclasses import asdict
+
 import dask.array
+
 from .ngff_image import NgffImage
-from dataclasses import asdict
 
 
 def itk_image_to_ngff_image(
     itk_image,
     # anatomical_axes: bool = False,
     # axis_names: List[str] = None,
     # axis_units: List[str] = None,
@@ -42,19 +44,22 @@
 
         if isinstance(itk_image, itkwasm.Image):
             image_dict = asdict(itk_image)
     except ImportError:
         pass
 
     if image_dict is None:
-        raise RuntimeError('Could not import itk or itkwasm or input is not itk.Image or itkwasm.Image')
+        msg = (
+            "Could not import itk or itkwasm or input is not itk.Image or itkwasm.Image"
+        )
+        raise RuntimeError(msg)
 
     data = dask.array.from_array(image_dict["data"])
     ndim = data.ndim
-    if ndim == 3 and image_dict['imageType']['components'] > 1:
+    if ndim == 3 and image_dict["imageType"]["components"] > 1:
         dims = ("y", "x", "c")
     elif ndim < 4:
         dims = ("z", "y", "x")[-ndim:]
     elif ndim < 5:
         dims = ("z", "y", "x", "c")
     elif ndim < 6:
         dims = ("t", "z", "y", "x", "c")
@@ -63,9 +68,8 @@
 
     spacing = image_dict["spacing"]
     scale = {dim: spacing[::-1][idx] for idx, dim in enumerate(spatial_dims)}
 
     origin = image_dict["origin"]
     translation = {dim: origin[::-1][idx] for idx, dim in enumerate(spatial_dims)}
 
-    ngff_image = NgffImage(data, dims, scale, translation)
-    return ngff_image
+    return NgffImage(data, dims, scale, translation)
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/multiscales.py` & `ngff_zarr-0.4.6/ngff_zarr/multiscales.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import Union, Optional, Sequence, Mapping, Dict, Tuple, Any, List
 from dataclasses import dataclass
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
+from .methods import Methods
 from .ngff_image import NgffImage
 from .zarr_metadata import Metadata
-from .methods import Methods
+
 
 @dataclass
 class Multiscales:
     images: List[NgffImage]
     metadata: Metadata
     scale_factors: Optional[Sequence[Union[Dict[str, int], int]]] = None
     method: Optional[Methods] = None
@@ -15,8 +16,7 @@
         Union[
             int,
             Tuple[int, ...],
             Tuple[Tuple[int, ...], ...],
             Mapping[Any, Union[None, int, Tuple[int, ...]]],
         ]
     ] = None
-
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/ngff_image_to_itk_image.py` & `ngff_zarr-0.4.6/ngff_zarr/ngff_image_to_itk_image.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,87 @@
-from .ngff_image import NgffImage
 import numpy as np
 
 from .methods._support import _spatial_dims
+from .ngff_image import NgffImage
+
 
 def _dtype_to_component_type(dtype):
-    from itkwasm import IntTypes, FloatTypes
+    from itkwasm import FloatTypes, IntTypes
+
     if dtype == np.uint8:
         return IntTypes.UInt8
-    elif dtype == np.int8:
+    if dtype == np.int8:
         return IntTypes.Int8
-    elif dtype == np.uint16:
+    if dtype == np.uint16:
         return IntTypes.UInt16
-    elif dtype == np.int16:
+    if dtype == np.int16:
         return IntTypes.Int16
-    elif dtype == np.uint32:
+    if dtype == np.uint32:
         return IntTypes.UInt32
-    elif dtype == np.int32:
+    if dtype == np.int32:
         return IntTypes.Int32
-    elif dtype == np.uint64:
+    if dtype == np.uint64:
         return IntTypes.UInt64
-    elif dtype == np.int64:
+    if dtype == np.int64:
         return IntTypes.Int64
-    elif dtype == np.float32:
+    if dtype == np.float32:
         return FloatTypes.Float32
-    elif dtype == np.float64:
+    if dtype == np.float64:
         return FloatTypes.Float64
-    raise ValueError(f"Unsupported dtype {dtype}")
+    msg = f"Unsupported dtype {dtype}"
+    raise ValueError(msg)
+
 
 def ngff_image_to_itk_image(
     ngff_image: NgffImage,
     wasm: bool = True,
-    ):
-
+):
     from itkwasm import IntTypes, PixelTypes
 
     dims = ngff_image.dims
-    if 'z' in dims:
-        dimension = 3
-    else:
-        dimension = 2
+    dimension = 3 if "z" in dims else 2
 
     componentType = _dtype_to_component_type(ngff_image.data.dtype)
 
     components = 1
     pixelType = PixelTypes.Scalar
-    if 'c' in dims:
-        components = ngff_image.data.shape[dims.index('c')]
+    if "c" in dims:
+        components = ngff_image.data.shape[dims.index("c")]
         if components == 3 and componentType == IntTypes.UInt8:
             pixelType = PixelTypes.RGB
         else:
             pixelType = PixelTypes.VariableLengthVector
     imageType = {
-        'dimension': dimension,
-        'componentType': str(componentType),
-        'pixelType': str(pixelType),
-        'components': components
-        }
+        "dimension": dimension,
+        "componentType": str(componentType),
+        "pixelType": str(pixelType),
+        "components": components,
+    }
 
     spatial_dims = [dim for dim in dims if dim in _spatial_dims]
     spatial_dims.sort()
     spacing = [ngff_image.scale[dim] for dim in spatial_dims]
     origin = [ngff_image.translation[dim] for dim in spatial_dims]
     size = [ngff_image.data.shape[dims.index(d)] for d in spatial_dims]
 
     # TODO: reorder as needed
     data = np.asarray(ngff_image.data)
 
     image_dict = {
-            'imageType': imageType,
-            'name': ngff_image.name,
-            'origin': origin,
-            'spacing': spacing,
-            'direction': np.eye(dimension),
-            'size': size,
-            'metadata': {},
-            'data': data,
-            }
+        "imageType": imageType,
+        "name": ngff_image.name,
+        "origin": origin,
+        "spacing": spacing,
+        "direction": np.eye(dimension),
+        "size": size,
+        "metadata": {},
+        "data": data,
+    }
 
     if wasm:
         from itkwasm import Image
-        image = Image(**image_dict)
-        return image
-    else:
-        import itk
-        image = itk.image_from_dict(image_dict)
-        return image
 
+        return Image(**image_dict)
+
+    import itk
+
+    return itk.image_from_dict(image_dict)
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/rich_dask_progress.py` & `ngff_zarr-0.4.6/ngff_zarr/rich_dask_progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Dict, Optional, Set
 
-from rich.progress import TaskID
 from dask.callbacks import Callback
+from rich.progress import TaskID
+
 
 class NgffProgress:
     def __init__(self, rich_progress):
         self.rich = rich_progress
 
     def add_multiscales_task(self, description: str, scales: int):
         self.multiscales_task = self.rich.add_task(description, total=scales)
@@ -15,50 +16,53 @@
 
     def add_cache_task(self, description: str, total: int):
         self.cache_task = self.rich.add_task(description, total=total)
 
     def update_cache_task_completed(self, completed: int):
         self.rich.update(self.cache_task, completed=completed, refresh=True)
 
+
 class NgffProgressCallback(Callback, NgffProgress):
     def __init__(self, rich_progress):
         self.rich = rich_progress
-        self.tasks: Dict[str, Optional[TaskId]] = {}
+        self.tasks: Dict[str, Optional[TaskID]] = {}
         self.hide_after_finished: Set[str] = set()
         self.next_task = None
 
     def add_callback_task(self, description: str):
         self.next_task = description
         self.tasks[self.next_task] = self.rich.add_task(self.next_task)
         self.hide_after_finished.add(self.next_task)
 
     def _start(self, dsk):
         if self.next_task:
             description = self.next_task
-            dsk['ngff_zarr_task'] = description
+            dsk["ngff_zarr_task"] = description
 
     def _start_state(self, dsk, state):
         pass
 
-    def _pretask(self, key, dsk, state):
-        if 'ngff_zarr_task' in dsk:
-            description = dsk['ngff_zarr_task']
+    def _pretask(self, key, dsk, state):  # noqa: ARG002
+        if "ngff_zarr_task" in dsk:
+            description = dsk["ngff_zarr_task"]
             task = self.tasks[description]
             ndone = len(state["finished"])
             ntasks = sum(len(state[k]) for k in ["ready", "waiting", "running"]) + ndone
             self.rich.update(task, total=ntasks, completed=ndone)
 
     def _posttask(self, key, result, dsk, state, worker_id):
         pass
 
     def _finish(self, dsk, state, errored):
-        if 'ngff_zarr_task' in dsk:
-            description = dsk['ngff_zarr_task']
+        if "ngff_zarr_task" in dsk:
+            description = dsk["ngff_zarr_task"]
             task = self.tasks[description]
             if not errored:
                 ndone = len(state["finished"])
-                ntasks = sum(len(state[k]) for k in ["ready", "waiting", "running"]) + ndone
+                ntasks = (
+                    sum(len(state[k]) for k in ["ready", "waiting", "running"]) + ndone
+                )
                 self.rich.update(task, total=ntasks, completed=ndone)
                 if description in self.hide_after_finished:
                     self.rich.update(task, visible=False)
 
             # self.rich.update(task, total=1.0, completed=1.0)
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/to_multiscales.py` & `ngff_zarr-0.4.6/ngff_zarr/to_multiscales.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,61 @@
-from typing import Union, Optional, Sequence, Mapping, Dict, Tuple, Any, List
-from typing_extensions import Literal
-from collections.abc import MutableMapping
-import time
-import shutil
-from pathlib import Path
 import atexit
+import shutil
 import signal
+import time
+from collections.abc import MutableMapping
+from pathlib import Path
+from typing import Any, Dict, Mapping, Optional, Sequence, Tuple, Union
 
-from zarr.core import Array as ZarrArray
-from numpy.typing import ArrayLike
-from dask.array.core import Array as DaskArray
+import dask
 import numpy as np
 import zarr
-import dask
+from dask.array.core import Array as DaskArray
+from numpy.typing import ArrayLike
+from zarr.core import Array as ZarrArray
 
+from .config import config
+from .memory_usage import memory_usage
+from .methods import Methods
 from .methods._dask_image import _downsample_dask_image
-from .methods._itk import _downsample_itk_bin_shrink, _downsample_itk_gaussian, _downsample_itk_label
-from .to_ngff_image import to_ngff_image
-from .ngff_image import NgffImage
+from .methods._itk import (
+    _downsample_itk_bin_shrink,
+    _downsample_itk_gaussian,
+)
+from .methods._support import _spatial_dims
 from .multiscales import Multiscales
-from .zarr_metadata import Metadata, Axis, Translation, Scale, Dataset
-from .methods import Methods
-from .config import config
+from .ngff_image import NgffImage
 from .rich_dask_progress import NgffProgress, NgffProgressCallback
-from .memory_usage import memory_usage
+from .to_ngff_image import to_ngff_image
+from .zarr_metadata import Axis, Dataset, Metadata, Scale, Translation
 
-from .methods._support import _spatial_dims
 
 def _ngff_image_scale_factors(ngff_image, min_length, out_chunks):
-    sizes = { d: s for d, s in zip(ngff_image.dims, ngff_image.data.shape) if d in _spatial_dims }
+    sizes = {
+        d: s
+        for d, s in zip(ngff_image.dims, ngff_image.data.shape)
+        if d in _spatial_dims
+    }
     scale_factors = []
     dims = ngff_image.dims
-    previous = { d: 1 for d in _spatial_dims.intersection(dims) }
+    previous = {d: 1 for d in _spatial_dims.intersection(dims)}
     sizes_array = np.array(list(sizes.values()))
-    sizes = { d: s for d, s in zip(ngff_image.dims, ngff_image.data.shape) if d in _spatial_dims }
-    double_chunks = np.array([2*out_chunks[d] for d in _spatial_dims.intersection(out_chunks)])
+    sizes = {
+        d: s
+        for d, s in zip(ngff_image.dims, ngff_image.data.shape)
+        if d in _spatial_dims
+    }
+    double_chunks = np.array(
+        [2 * out_chunks[d] for d in _spatial_dims.intersection(out_chunks)]
+    )
     while (sizes_array > double_chunks).any():
         max_size = np.array(list(sizes.values())).max()
-        to_skip = { d: sizes[d] <= max_size / 2 for d in previous.keys() }
+        to_skip = {d: sizes[d] <= max_size / 2 for d in previous}
         scale_factor = {}
-        for dim in previous.keys():
+        for dim in previous:
             if to_skip[dim] or sizes[dim] / 2 < out_chunks[dim]:
                 scale_factor[dim] = previous[dim]
                 continue
             scale_factor[dim] = 2 * previous[dim]
 
             sizes[dim] = int(sizes[dim] / 2)
         sizes_array = np.array(list(sizes.values()))
@@ -51,154 +63,175 @@
         # There should be sufficient data in the result for statistics, etc.
         if (np.prod(sizes_array) / min_length) < 2:
             break
         scale_factors.append(scale_factor)
 
     return scale_factors
 
-def _large_image_serialization(image: NgffImage, progress: Optional[Union[NgffProgress, NgffProgressCallback]]):
-    if "z" in image.dims:
-        optimized_chunks = 512
-    else:
-        optimized_chunks = 1024
+
+def _large_image_serialization(
+    image: NgffImage, progress: Optional[Union[NgffProgress, NgffProgressCallback]]
+):
+    optimized_chunks = 512 if "z" in image.dims else 1024
     base_path = f"{image.name}-cache-{time.time()}"
 
     cache_store = config.cache_store
     base_path_removed = False
-    def remove_from_cache_store(sig_id, frame):
+
+    def remove_from_cache_store(sig_id, frame):  # noqa: ARG001
         nonlocal base_path_removed
         if not base_path_removed:
             if isinstance(cache_store, zarr.storage.DirectoryStore):
                 full_path = Path(cache_store.dir_path()) / base_path
                 if full_path.exists():
                     shutil.rmtree(full_path, ignore_errors=True)
             else:
                 zarr.storage.rmdir(cache_store, base_path)
             base_path_removed = True
+
     atexit.register(remove_from_cache_store, None, None)
     signal.signal(signal.SIGTERM, remove_from_cache_store)
     signal.signal(signal.SIGINT, remove_from_cache_store)
 
     data = image.data
 
     dims = list(image.dims)
-    x_index = dims.index('x')
-    y_index = dims.index('y')
+    x_index = dims.index("x")
+    y_index = dims.index("y")
 
     rechunks = {}
     for index, dim in enumerate(dims):
-        if dim == 't':
-            rechunks[index] = 1
-        elif dim == 'c':
+        if dim == "t" or dim == "c":
             rechunks[index] = 1
         else:
             rechunks[index] = min(optimized_chunks, data.shape[index])
 
-    if 'z' in dims:
-        z_index = dims.index('z')
+    if "z" in dims:
+        z_index = dims.index("z")
         slice_bytes = data.dtype.itemsize * data.shape[x_index] * data.shape[y_index]
 
-        slab_slices = min(int(np.ceil(config.memory_target / slice_bytes)), data.shape[z_index])
+        slab_slices = min(
+            int(np.ceil(config.memory_target / slice_bytes)), data.shape[z_index]
+        )
         if optimized_chunks < data.shape[z_index]:
             slab_slices = min(slab_slices, optimized_chunks)
         rechunks[z_index] = slab_slices
 
         path = f"{base_path}/slabs"
         slabs = data.rechunk(rechunks)
 
         chunks = tuple([c[0] for c in slabs.chunks])
-        optimized = dask.array.Array(dask.array.optimize(slabs.__dask_graph__(),
-            slabs.__dask_keys__()), slabs.name,
-            slabs.chunks, meta=slabs)
+        optimized = dask.array.Array(
+            dask.array.optimize(slabs.__dask_graph__(), slabs.__dask_keys__()),
+            slabs.name,
+            slabs.chunks,
+            meta=slabs,
+        )
         zarr_array = zarr.creation.open_array(
             shape=data.shape,
             chunks=chunks,
             dtype=data.dtype,
             store=cache_store,
             path=path,
-            mode='a',
+            mode="a",
+            dimension_separator="/",
         )
 
         n_slabs = int(np.ceil(data.shape[z_index] / slab_slices))
         if progress:
-            progress.add_cache_task(f"[blue]Caching z-slabs", n_slabs)
+            progress.add_cache_task("[blue]Caching z-slabs", n_slabs)
         for slab_index in range(n_slabs):
             if progress:
                 if isinstance(progress, NgffProgressCallback):
-                    progress.add_callback_task(f"[blue]Caching z-slabs {slab_index+1} of {n_slabs}")
-                progress.update_cache_task_completed((slab_index+1))
+                    progress.add_callback_task(
+                        f"[blue]Caching z-slabs {slab_index+1} of {n_slabs}"
+                    )
+                progress.update_cache_task_completed(slab_index + 1)
             region = [slice(data.shape[i]) for i in range(data.ndim)]
-            region[z_index] = slice(slab_index*slab_slices, min((slab_index+1)*slab_slices, data.shape[z_index]))
+            region[z_index] = slice(
+                slab_index * slab_slices,
+                min((slab_index + 1) * slab_slices, data.shape[z_index]),
+            )
             region = tuple(region)
             arr_region = optimized[region]
             dask.array.to_zarr(
                 arr_region,
                 zarr_array,
                 region=region,
                 component=path,
                 overwrite=False,
                 compute=True,
                 return_stored=False,
+                dimension_separator="/",
             )
         data = dask.array.from_zarr(cache_store, component=path)
         if optimized_chunks < data.shape[z_index] and slab_slices < optimized_chunks:
             rechunks[z_index] = optimized_chunks
             data = data.rechunk(rechunks)
             path = f"{base_path}/optimized_chunks"
             chunks = tuple([c[0] for c in optimized.chunks])
             data = data.rechunk(chunks)
             zarr_array = zarr.creation.open_array(
                 shape=data.shape,
                 chunks=chunks,
                 dtype=data.dtype,
                 store=cache_store,
                 path=path,
-                mode='a',
+                mode="a",
+                dimension_separator="/",
             )
             n_slabs = int(np.ceil(data.shape[z_index] / optimized_chunks))
             for slab_index in range(n_slabs):
                 if progress:
                     if isinstance(progress, NgffProgressCallback):
-                        progress.add_callback_task(f"[blue]Caching z-rechunk {slab_index+1} of {n_slabs}")
-                    progress.update_cache_task_completed((slab_index+1))
+                        progress.add_callback_task(
+                            f"[blue]Caching z-rechunk {slab_index+1} of {n_slabs}"
+                        )
+                    progress.update_cache_task_completed(slab_index + 1)
                 region = [slice(data.shape[i]) for i in range(data.ndim)]
-                region[z_index] = slice(slab_index*optimized_chunks, min((slab_index+1)*optimized_chunks, data.shape[z_index]))
+                region[z_index] = slice(
+                    slab_index * optimized_chunks,
+                    min((slab_index + 1) * optimized_chunks, data.shape[z_index]),
+                )
                 region = tuple(region)
                 arr_region = data[region]
                 dask.array.to_zarr(
                     arr_region,
                     zarr_array,
                     region=region,
                     component=path,
                     overwrite=False,
                     compute=True,
                     return_stored=False,
+                    dimension_separator="/",
                 )
             data = dask.array.from_zarr(cache_store, component=path)
         else:
             data = data.rechunk(rechunks)
     else:
         data = data.rechunk(rechunks)
         # TODO: Slab, chunk optimized very large 2D images
-        path = base_path + f"/optimized_chunks"
+        path = base_path + "/optimized_chunks"
         if progress:
-            progress.add_callback_task(f"[blue]Caching optimized chunks")
+            progress.add_callback_task("[blue]Caching optimized chunks")
         dask.array.to_zarr(
             data,
             cache_store,
             component=path,
             overwrite=False,
             compute=True,
             return_stored=False,
+            dimension_separator="/",
         )
         data = dask.array.from_zarr(cache_store, component=path)
 
     image.data = data
     return image
 
+
 def to_multiscales(
     data: Union[NgffImage, ArrayLike, MutableMapping, str, ZarrArray],
     scale_factors: Union[int, Sequence[Union[Dict[str, int], int]]] = 128,
     method: Optional[Methods] = None,
     chunks: Optional[
         Union[
             int,
@@ -234,24 +267,18 @@
     Returns
     -------
 
     multiscales: Multiscales
         NgffImage for each resolution and NGFF multiscales metadata
     """
     image = data
-    if isinstance(data, NgffImage):
-        ngff_image = data
-    else:
-        ngff_image = to_ngff_image(data)
+    ngff_image = data if isinstance(data, NgffImage) else to_ngff_image(data)
 
     # IPFS and visualization friendly default chunks
-    if "z" in ngff_image.dims:
-        default_chunks = 128
-    else:
-        default_chunks = 256
+    default_chunks = 128 if "z" in ngff_image.dims else 256
     default_chunks = {d: default_chunks for d in ngff_image.dims}
     if "t" in ngff_image.dims:
         default_chunks["t"] = 1
     out_chunks = chunks
     if out_chunks is None:
         out_chunks = default_chunks
     elif isinstance(out_chunks, int):
@@ -307,15 +334,16 @@
         if dim in {"x", "y", "z"}:
             axis = Axis(name=dim, type="space", unit=unit)
         elif dim == "c":
             axis = Axis(name=dim, type="channel", unit=unit)
         elif dim == "t":
             axis = Axis(name=dim, type="time", unit=unit)
         else:
-            raise KeyError(f'Dimension identifier is not valid: {dim}')
+            msg = f"Dimension identifier is not valid: {dim}"
+            raise KeyError(msg)
         axes.append(axis)
 
     datasets = []
     for index, image in enumerate(images):
         path = f"scale{index}/{ngff_image.name}"
         scale = []
         for dim in image.dims:
@@ -332,9 +360,8 @@
         coordinateTransformations = [Scale(scale), Translation(translation)]
         dataset = Dataset(
             path=path, coordinateTransformations=coordinateTransformations
         )
         datasets.append(dataset)
     metadata = Metadata(axes=axes, datasets=datasets, name=ngff_image.name)
 
-    multiscales = Multiscales(images, metadata, scale_factors, method, out_chunks)
-    return multiscales
+    return Multiscales(images, metadata, scale_factors, method, out_chunks)
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/to_ngff_image.py` & `ngff_zarr-0.4.6/ngff_zarr/to_ngff_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Union, Optional, Sequence, Hashable, Mapping, Dict, Tuple, Any, List
 from collections.abc import MutableMapping
+from typing import Hashable, Mapping, Optional, Sequence, Union
 
+import dask
+from dask.array.core import Array as DaskArray
 from numpy.typing import ArrayLike
 from zarr.core import Array as ZarrArray
-from dask.array.core import Array as DaskArray
-import dask
 
 from .methods._support import _spatial_dims
 from .ngff_image import NgffImage
-from .zarr_metadata import Units
+from .zarr_metadata import SupportedDims, Units
 
 
 def to_ngff_image(
     data: Union[ArrayLike, MutableMapping, str, ZarrArray],
-    dims: Optional[Sequence[Union["t", "z", "y", "x", "c"]]] = None,
+    dims: Optional[Sequence[SupportedDims]] = None,
     scale: Optional[Union[Mapping[Hashable, float]]] = None,
     translation: Optional[Union[Mapping[Hashable, float]]] = None,
     name: str = "image",
     axes_units: Optional[Mapping[str, Units]] = None,
 ) -> NgffImage:
     """
     Create an image with pixel array and metadata to following the OME-NGFF data model.
@@ -64,31 +64,30 @@
         elif ndim < 6:
             dims = ("t", "z", "y", "x", "c")
         else:
             raise ValueError("Unsupported dimension: " + str(ndim))
     else:
         _supported_dims = {"c", "x", "y", "z", "t"}
         if not set(dims).issubset(_supported_dims):
-            raise ValueError("dims not valid")
+            msg = "dims not valid"
+            raise ValueError(msg)
 
     if scale is None:
         scale = {dim: 1.0 for dim in dims if dim in _spatial_dims}
 
     if translation is None:
         translation = {dim: 0.0 for dim in dims if dim in _spatial_dims}
 
     if not isinstance(data, DaskArray):
         if isinstance(data, (ZarrArray, str, MutableMapping)):
             data = dask.array.from_zarr(data)
         else:
             data = dask.array.from_array(data)
 
-    ngff_image = NgffImage(
+    return NgffImage(
         data=data,
         dims=dims,
         scale=scale,
         translation=translation,
         name=name,
         axes_units=axes_units,
     )
-
-    return ngff_image
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/to_ngff_zarr.py` & `ngff_zarr-0.4.6/ngff_zarr/to_ngff_zarr.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from typing import Union, Optional
 from collections.abc import MutableMapping
-from pathlib import Path, PurePosixPath
 from dataclasses import asdict
-from functools import reduce
+from pathlib import Path, PurePosixPath
+from typing import Optional, Union
 
-from zarr.storage import BaseStore
-import zarr
 import dask.array
 import numpy as np
+import zarr
+from zarr.storage import BaseStore
 
-from .multiscales import Multiscales
-from .to_multiscales import to_multiscales
 from .config import config
-from .rich_dask_progress import NgffProgress, NgffProgressCallback
 from .memory_usage import memory_usage
-from .task_count import task_count
 from .methods._support import _dim_scale_factors
+from .multiscales import Multiscales
+from .rich_dask_progress import NgffProgress, NgffProgressCallback
+from .to_multiscales import to_multiscales
+
 
 def to_ngff_zarr(
     store: Union[MutableMapping, str, Path, BaseStore],
     multiscales: Multiscales,
     overwrite: bool = True,
     chunk_store: Optional[Union[MutableMapping, str, Path, BaseStore]] = None,
     progress: Optional[Union[NgffProgress, NgffProgressCallback]] = None,
@@ -58,31 +57,33 @@
     metadata_dict = asdict(multiscales.metadata)
     metadata_dict["@type"] = "ngff:Image"
     root = zarr.group(store, overwrite=overwrite, chunk_store=chunk_store)
     root.attrs["multiscales"] = [metadata_dict]
 
     nscales = len(multiscales.images)
     if progress:
-        progress.add_multiscales_task(f"[green]Writing scales", nscales)
+        progress.add_multiscales_task("[green]Writing scales", nscales)
     next_image = multiscales.images[0]
     dims = next_image.dims
     previous_dim_factors = {d: 1 for d in dims}
     for index in range(nscales):
         if progress:
-            progress.update_multiscales_task_completed((index+1))
+            progress.update_multiscales_task_completed(index + 1)
         image = next_image
         arr = image.data
         path = multiscales.metadata.datasets[index].path
         array_dims_group = root.create_group(str(PurePosixPath(path).parent))
         array_dims_group.attrs["_ARRAY_DIMENSIONS"] = image.dims
 
         if index > 0 and index < nscales - 1:
-            dim_factors = _dim_scale_factors(dims, multiscales.scale_factors[index], previous_dim_factors)
+            dim_factors = _dim_scale_factors(
+                dims, multiscales.scale_factors[index], previous_dim_factors
+            )
         else:
-            dim_factors = { d: 1 for d in dims }
+            dim_factors = {d: 1 for d in dims}
         previous_dim_factors = dim_factors
 
         if memory_usage(image) > config.memory_target:
             shrink_factors = []
             for dim in dims:
                 if dim in dim_factors:
                     shrink_factors.append(dim_factors[dim])
@@ -92,25 +93,28 @@
             chunks = tuple([c[0] for c in arr.chunks])
             zarr_array = zarr.creation.open_array(
                 shape=arr.shape,
                 chunks=chunks,
                 dtype=arr.dtype,
                 store=store,
                 path=path,
-                mode='a',
+                mode="a",
+                dimension_separator="/",
             )
 
             shape = image.data.shape
-            x_index = dims.index('x')
-            y_index = dims.index('y')
-            if 'z' in dims:
-                z_index = dims.index('z')
+            x_index = dims.index("x")
+            y_index = dims.index("y")
+            if "z" in dims:
+                z_index = dims.index("z")
                 # TODO address, c, t, large 2D
-                slice_bytes = memory_usage(image, {'z'})
-                slab_slices = min(int(np.ceil(config.memory_target / slice_bytes)), arr.shape[z_index])
+                slice_bytes = memory_usage(image, {"z"})
+                slab_slices = min(
+                    int(np.ceil(config.memory_target / slice_bytes)), arr.shape[z_index]
+                )
                 z_chunks = chunks[z_index]
                 slice_planes = False
                 if slab_slices < z_chunks:
                     slab_slices = z_chunks
                     slice_planes = True
                 if slab_slices > arr.shape[z_index]:
                     slab_slices = arr.shape[z_index]
@@ -119,104 +123,166 @@
                 while num_z_splits % shrink_factors[z_index] > 1:
                     num_z_splits += 1
                 num_y_splits = 1
                 num_x_splits = 1
                 regions = []
                 for slab_index in range(num_z_splits):
                     if slice_planes:
-                        plane_bytes = memory_usage(image, {'z', 'y'})
-                        plane_slices = min(int(np.ceil(config.memory_target / plane_bytes)), arr.shape[y_index])
+                        plane_bytes = memory_usage(image, {"z", "y"})
+                        plane_slices = min(
+                            int(np.ceil(config.memory_target / plane_bytes)),
+                            arr.shape[y_index],
+                        )
                         y_chunks = chunks[y_index]
                         slice_strips = False
                         if plane_slices < y_chunks:
                             plane_slices = y_chunks
                             slice_strips = True
                         if plane_slices > arr.shape[y_index]:
                             plane_slices = arr.shape[y_index]
                         plane_slices = int(plane_slices / y_chunks) * y_chunks
                         num_y_splits = int(np.ceil(shape[y_index] / plane_slices))
                         while num_y_splits % shrink_factors[y_index] > 1:
                             num_y_splits += 1
                         if slice_strips:
-                            strip_bytes = memory_usage(image, {'z', 'y', 'x'})
-                            strip_slices = min(int(np.ceil(config.memory_target / strip_bytes)), arr.shape[x_index])
+                            strip_bytes = memory_usage(image, {"z", "y", "x"})
+                            strip_slices = min(
+                                int(np.ceil(config.memory_target / strip_bytes)),
+                                arr.shape[x_index],
+                            )
                             x_chunks = chunks[x_index]
                             strip_slices = max(strip_slices, x_chunks)
                             slice_strips = False
                             if strip_slices > arr.shape[x_index]:
                                 strip_slices = arr.shape[x_index]
                             strip_slices = int(strip_slices / x_chunks) * x_chunks
                             num_x_splits = int(np.ceil(shape[x_index] / strip_slices))
                             while num_x_splits % shrink_factors[x_index] > 1:
                                 num_x_splits += 1
                             for plane_index in range(num_y_splits):
                                 for strip_index in range(num_x_splits):
-                                    region = [slice(arr.shape[i]) for i in range(arr.ndim)]
-                                    region[z_index] = slice(slab_index*z_chunks, min((slab_index+1)*z_chunks, arr.shape[z_index]))
-                                    region[y_index] = slice(plane_index*y_chunks, min((plane_index+1)*y_chunks, arr.shape[y_index]))
-                                    region[x_index] = slice(strip_index*x_chunks, min((strip_index+1)*x_chunks, arr.shape[x_index]))
+                                    region = [
+                                        slice(arr.shape[i]) for i in range(arr.ndim)
+                                    ]
+                                    region[z_index] = slice(
+                                        slab_index * z_chunks,
+                                        min(
+                                            (slab_index + 1) * z_chunks,
+                                            arr.shape[z_index],
+                                        ),
+                                    )
+                                    region[y_index] = slice(
+                                        plane_index * y_chunks,
+                                        min(
+                                            (plane_index + 1) * y_chunks,
+                                            arr.shape[y_index],
+                                        ),
+                                    )
+                                    region[x_index] = slice(
+                                        strip_index * x_chunks,
+                                        min(
+                                            (strip_index + 1) * x_chunks,
+                                            arr.shape[x_index],
+                                        ),
+                                    )
                                     regions.append(tuple(region))
                         else:
                             for plane_index in range(num_y_splits):
                                 region = [slice(arr.shape[i]) for i in range(arr.ndim)]
-                                region[z_index] = slice(slab_index*z_chunks, min((slab_index+1)*z_chunks, arr.shape[z_index]))
-                                region[y_index] = slice(plane_index*y_chunks, min((plane_index+1)*y_chunks, arr.shape[y_index]))
+                                region[z_index] = slice(
+                                    slab_index * z_chunks,
+                                    min(
+                                        (slab_index + 1) * z_chunks, arr.shape[z_index]
+                                    ),
+                                )
+                                region[y_index] = slice(
+                                    plane_index * y_chunks,
+                                    min(
+                                        (plane_index + 1) * y_chunks, arr.shape[y_index]
+                                    ),
+                                )
                                 regions.append(tuple(region))
                     else:
                         region = [slice(arr.shape[i]) for i in range(arr.ndim)]
-                        region[z_index] = slice(slab_index*z_chunks, min((slab_index+1)*z_chunks, arr.shape[z_index]))
+                        region[z_index] = slice(
+                            slab_index * z_chunks,
+                            min((slab_index + 1) * z_chunks, arr.shape[z_index]),
+                        )
                         regions.append(tuple(region))
                 regions = tuple(regions)
                 for region_index, region in enumerate(regions):
                     if isinstance(progress, NgffProgressCallback):
-                        progress.add_callback_task(f"[green]Writing scale {index+1} of {nscales}, region {region_index+1} of {len(regions)}")
+                        progress.add_callback_task(
+                            f"[green]Writing scale {index+1} of {nscales}, region {region_index+1} of {len(regions)}"
+                        )
                     arr_region = arr[region]
-                    optimized = dask.array.Array(dask.array.optimize(arr_region.__dask_graph__(),
-                        arr_region.__dask_keys__()), arr_region.name,
-                        arr_region.chunks, meta=arr_region)
+                    optimized = dask.array.Array(
+                        dask.array.optimize(
+                            arr_region.__dask_graph__(), arr_region.__dask_keys__()
+                        ),
+                        arr_region.name,
+                        arr_region.chunks,
+                        meta=arr_region,
+                    )
                     dask.array.to_zarr(
                         optimized,
                         zarr_array,
                         region=region,
                         component=path,
                         overwrite=False,
                         compute=True,
                         return_stored=False,
+                        dimension_separator="/",
                         **kwargs,
                     )
         else:
             if isinstance(progress, NgffProgressCallback):
-                progress.add_callback_task(f"[green]Writing scale {index+1} of {nscales}")
+                progress.add_callback_task(
+                    f"[green]Writing scale {index+1} of {nscales}"
+                )
             dask.array.to_zarr(
                 arr,
                 store,
                 component=path,
                 overwrite=False,
                 compute=True,
                 return_stored=False,
+                dimension_separator="/",
                 **kwargs,
             )
 
         # Minimize task graph depth
-        if index > 1 and index < nscales - 2 and multiscales.scale_factors and multiscales.method and multiscales.chunks:
+        if (
+            index > 1
+            and index < nscales - 2
+            and multiscales.scale_factors
+            and multiscales.method
+            and multiscales.chunks
+        ):
             image.data = dask.array.from_zarr(store, component=path)
             next_multiscales_factor = multiscales.scale_factors[index]
             if isinstance(next_multiscales_factor, int):
-                next_multiscales_factor = next_multiscales_factor // multiscales.scale_factors[index-1]
+                next_multiscales_factor = (
+                    next_multiscales_factor // multiscales.scale_factors[index - 1]
+                )
             else:
                 updated_factors = {}
                 for d, f in next_multiscales_factor.items():
-                    updated_factors[d] = f // multiscales.scale_factors[index-1][d]
+                    updated_factors[d] = f // multiscales.scale_factors[index - 1][d]
                 next_multiscales_factor = updated_factors
 
-            next_multiscales = to_multiscales(image,
-                scale_factors=[next_multiscales_factor,],
+            next_multiscales = to_multiscales(
+                image,
+                scale_factors=[
+                    next_multiscales_factor,
+                ],
                 method=multiscales.method,
                 chunks=multiscales.chunks,
                 progress=progress,
-                cache=False)
-            multiscales.images[index+1] = next_multiscales.images[1]
+                cache=False,
+            )
+            multiscales.images[index + 1] = next_multiscales.images[1]
             next_image = next_multiscales.images[1]
         elif index < nscales - 1:
-            next_image = multiscales.images[index+1]
+            next_image = multiscales.images[index + 1]
 
     zarr.consolidate_metadata(store)
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/zarr_metadata.py` & `ngff_zarr-0.4.6/ngff_zarr/zarr_metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass, field
-from typing import Union, Optional, List
+from typing import List, Optional, Union
+
 from typing_extensions import Literal
 
 SupportedDims = Union[
     Literal["c"], Literal["x"], Literal["y"], Literal["z"], Literal["t"]
 ]
 
 SpatialDims = Union[Literal["x"], Literal["y"], Literal["z"]]
@@ -59,33 +60,79 @@
     Literal["yoctosecond"],
     Literal["yottasecond"],
     Literal["zeptosecond"],
     Literal["zettasecond"],
 ]
 Units = Union[SpaceUnits, TimeUnits]
 
-supported_dims = ['x','y','z','c','t']
+supported_dims = ["x", "y", "z", "c", "t"]
+
+space_units = [
+    "angstrom",
+    "attometer",
+    "centimeter",
+    "decimeter",
+    "exameter",
+    "femtometer",
+    "foot",
+    "gigameter",
+    "hectometer",
+    "inch",
+    "kilometer",
+    "megameter",
+    "meter",
+    "micrometer",
+    "mile",
+    "millimeter",
+    "nanometer",
+    "parsec",
+    "petameter",
+    "picometer",
+    "terameter",
+    "yard",
+    "yoctometer",
+    "yottameter",
+    "zeptometer",
+    "zettameter",
+]
+
+time_units = [
+    "attosecond",
+    "centisecond",
+    "day",
+    "decisecond",
+    "exasecond",
+    "femtosecond",
+    "gigasecond",
+    "hectosecond",
+    "hour",
+    "kilosecond",
+    "megasecond",
+    "microsecond",
+    "millisecond",
+    "minute",
+    "nanosecond",
+    "petasecond",
+    "picosecond",
+    "second",
+    "terasecond",
+    "yoctosecond",
+    "yottasecond",
+    "zeptosecond",
+    "zettasecond",
+]
 
-space_units = ['angstrom', 'attometer', 'centimeter', 'decimeter', 'exameter',
-                 'femtometer', 'foot', 'gigameter', 'hectometer', 'inch', 'kilometer',
-                 'megameter', 'meter', 'micrometer', 'mile', 'millimeter', 'nanometer',
-                 'parsec', 'petameter', 'picometer', 'terameter', 'yard', 'yoctometer',
-                 'yottameter', 'zeptometer', 'zettameter']
-
-time_units = ['attosecond', 'centisecond', 'day', 'decisecond', 'exasecond', 'femtosecond',
-              'gigasecond', 'hectosecond', 'hour', 'kilosecond', 'megasecond', 'microsecond',
-              'millisecond', 'minute', 'nanosecond', 'petasecond', 'picosecond', 'second',
-              'terasecond', 'yoctosecond', 'yottasecond', 'zeptosecond', 'zettasecond']
 
-def is_dimension_supported(dim:str) -> bool:
-    '''Helper for string validation'''
+def is_dimension_supported(dim: str) -> bool:
+    """Helper for string validation"""
     return dim in supported_dims
 
-def is_unit_supported(unit:str) -> bool:
-    '''Helper for string validation'''
+
+def is_unit_supported(unit: str) -> bool:
+    """Helper for string validation"""
     return (unit in time_units) or (unit in space_units)
 
 
 @dataclass
 class Axis:
     name: SupportedDims
     type: AxesType
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/methods/_dask_image.py` & `ngff_zarr-0.4.6/ngff_zarr/methods/_dask_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from collections import OrderedDict
 
-import numpy as np
 import dask.array
+import numpy as np
 
-from ._support import _align_chunks, _dim_scale_factors, _compute_sigma, _spatial_dims
-from ..ngff_image import NgffImage
+from .._array_split import _array_split
 from ..config import config
 from ..memory_usage import memory_usage
-from .._array_split import _array_split
+from ..ngff_image import NgffImage
+from ._support import _align_chunks, _compute_sigma, _dim_scale_factors, _spatial_dims
 
 
 def _compute_next_scale(previous_image: NgffImage, dim_factors):
     """Helper method to manually compute output image spacing.
 
     previous_image: NgffImage
         The image for which voxel spacings are use to compute spacing for the next scale
@@ -20,15 +20,19 @@
         Shrink ratio along each enumerated axis
 
     result: Dict
         Spacing along each enumerated image axis
         Example {'x': 2.0, 'y': 1.0}
     """
     input_scale = previous_image.scale
-    return {dim: input_scale[dim] * dim_factors[dim] for dim in previous_image.dims if dim in _spatial_dims}
+    return {
+        dim: input_scale[dim] * dim_factors[dim]
+        for dim in previous_image.dims
+        if dim in _spatial_dims
+    }
 
 
 def _compute_next_translation(previous_image, dim_factors):
     """Helper method to manually compute output image physical offset.
         Note that this method does not account for an image direction matrix.
 
     previous_image: NgffImage
@@ -83,18 +87,16 @@
     from dask_image.ndfilters._gaussian import _get_border
 
     truncate = truncate_start
     stddev_step = 0.5  # search by stepping down by 0.5 stddev in each iteration
 
     border = _get_border(previous_image.data, sigma_values, truncate)
     while any(
-        [
-            border_len > image_len
-            for border_len, image_len in zip(border, previous_image.data.shape)
-        ]
+        border_len > image_len
+        for border_len, image_len in zip(border, previous_image.data.shape)
     ):
         truncate = truncate - stddev_step
         if truncate <= 0.0:
             break
         border = _get_border(previous_image.data, sigma_values, truncate)
 
     return truncate
@@ -110,16 +112,20 @@
         ngff_image,
     ]
     previous_image = ngff_image
     dims = ngff_image.dims
     previous_absolute_dim_factors = {d: 1 for d in dims}
     previous_scale_factor = 1
     for scale_factor in scale_factors:
-        dim_factors = _dim_scale_factors(dims, scale_factor, previous_absolute_dim_factors)
-        previous_absolute_dim_factors = {d:v*previous_scale_factor for d, v in dim_factors.items()}
+        dim_factors = _dim_scale_factors(
+            dims, scale_factor, previous_absolute_dim_factors
+        )
+        previous_absolute_dim_factors = {
+            d: v * previous_scale_factor for d, v in dim_factors.items()
+        }
         previous_scale_factor = scale_factor
         previous_image = _align_chunks(previous_image, default_chunks, dim_factors)
 
         shrink_factors = []
         for dim in dims:
             if dim in dim_factors:
                 shrink_factors.append(dim_factors[dim])
@@ -169,43 +175,44 @@
                 mode="nearest",
                 truncate=truncate,
             )
 
         # Construct downsample parameters
         image_dimension = len(shrink_factors)
         transform = np.eye(image_dimension)
-        if label:
-            order = 0
-        else:
-            order = 1
-        depth = [1,]*blurred_array.ndim
+        order = 0 if label else 1
+        depth = [
+            1,
+        ] * blurred_array.ndim
         for dim, shrink_factor in enumerate(shrink_factors):
             transform[dim, dim] = shrink_factor
             depth[dim] = shrink_factor + 1 + order
 
         out_chunks_list = []
         for dim in dims:
             if dim in out_chunks:
                 out_chunks_list.append(out_chunks[dim])
             else:
                 out_chunks_list.append(1)
-        output_chunks=tuple(out_chunks_list)
+        output_chunks = tuple(out_chunks_list)
 
         if memory_usage(previous_image) > config.memory_target:
             chunks = tuple([c[0] for c in blurred_array.chunks])
-            x_index = dims.index('x')
-            y_index = dims.index('y')
+            x_index = dims.index("x")
+            y_index = dims.index("y")
             ndim = blurred_array.ndim
             shape = blurred_array.shape
-            if 'z' in dims:
-                slice_slabs = True
-                z_index = dims.index('z')
+            if "z" in dims:
+                z_index = dims.index("z")
                 # TODD address, c, t, large 2D
-                slice_bytes = memory_usage(previous_image, {'z'})
-                slab_slices = min(int(np.ceil(config.memory_target / slice_bytes)), blurred_array.shape[z_index])
+                slice_bytes = memory_usage(previous_image, {"z"})
+                slab_slices = min(
+                    int(np.ceil(config.memory_target / slice_bytes)),
+                    blurred_array.shape[z_index],
+                )
                 z_chunks = chunks[z_index]
                 slice_planes = False
                 if slab_slices < z_chunks:
                     slab_slices = z_chunks
                     slice_planes = True
                 if slab_slices > blurred_array.shape[z_index]:
                     slab_slices = blurred_array.shape[z_index]
@@ -214,30 +221,35 @@
                 while num_z_splits % shrink_factors[z_index] > 1:
                     num_z_splits += 1
                 num_y_splits = 1
                 num_x_splits = 1
                 regions = OrderedDict()
                 if slice_planes:
                     # TODO
-                    plane_bytes = memory_usage(previous_image, {'z', 'y'})
-                    plane_slices = min(int(np.ceil(config.memory_target / plane_bytes)), shape[y_index])
+                    plane_bytes = memory_usage(previous_image, {"z", "y"})
+                    plane_slices = min(
+                        int(np.ceil(config.memory_target / plane_bytes)), shape[y_index]
+                    )
                     y_chunks = chunks[y_index]
                     slice_strips = False
                     if plane_slices < y_chunks:
                         plane_slices = y_chunks
                         slice_strips = True
                     if plane_slices > shape[y_index]:
                         plane_slices = shape[y_index]
                     plane_slices = int(plane_slices / y_chunks) * y_chunks
                     num_y_splits = int(np.ceil(shape[y_index] / plane_slices))
                     while num_y_splits % shrink_factors[y_index] > 1:
                         num_y_splits += 1
                     if slice_strips:
-                        strip_bytes = memory_usage(previous_image, {'z', 'y', 'x'})
-                        strip_slices = min(int(np.ceil(config.memory_target / strip_bytes)), shape[x_index])
+                        strip_bytes = memory_usage(previous_image, {"z", "y", "x"})
+                        strip_slices = min(
+                            int(np.ceil(config.memory_target / strip_bytes)),
+                            shape[x_index],
+                        )
                         x_chunks = chunks[x_index]
                         strip_slices = max(strip_slices, x_chunks)
                         slice_strips = False
                         if strip_slices > shape[x_index]:
                             strip_slices = shape[x_index]
                         strip_slices = int(strip_slices / x_chunks) * x_chunks
                         num_x_splits = int(np.ceil(shape[x_index] / strip_slices))
@@ -253,77 +265,108 @@
                         z_offset = 0
                         for z_split_index, z_split in enumerate(z_splits):
                             y_offset = 0
                             for y_split_index, y_split in enumerate(z_split):
                                 x_offset = 0
                                 for x_split_index, x_split in enumerate(y_split):
                                     region = [slice(shape[i]) for i in range(ndim)]
-                                    region[z_index] = slice(z_offset, z_offset+x_split.shape[z_index])
-                                    region[y_index] = slice(y_offset, y_offset+x_split.shape[y_index])
-                                    region[x_index] = slice(x_offset, x_offset+x_split.shape[x_index])
-                                    offset = [0,]*ndim
+                                    region[z_index] = slice(
+                                        z_offset, z_offset + x_split.shape[z_index]
+                                    )
+                                    region[y_index] = slice(
+                                        y_offset, y_offset + x_split.shape[y_index]
+                                    )
+                                    region[x_index] = slice(
+                                        x_offset, x_offset + x_split.shape[x_index]
+                                    )
+                                    offset = [
+                                        0,
+                                    ] * ndim
                                     offset[z_index] = z_offset
                                     offset[y_index] = y_offset
                                     offset[x_index] = x_offset
-                                    regions[(z_split_index, y_split_index, x_split_index)] = tuple(region), tuple(offset)
+                                    regions[
+                                        (z_split_index, y_split_index, x_split_index)
+                                    ] = tuple(region), tuple(offset)
                                     x_offset += x_split.shape[x_index]
                                 y_offset += y_split[0].shape[y_index]
                             z_offset += z_split[0][0].shape[z_index]
                     else:
                         z_splits = _array_split(blurred_array, num_z_splits, z_index)
                         for split_index, split in enumerate(z_splits):
                             y_splits = _array_split(split, num_y_splits, y_index)
                             z_splits[split_index] = y_splits
                         z_offset = 0
-                        for z_split_index, z_split in enumerate(splits):
+                        for z_split_index, z_split in enumerate(z_splits):
                             y_offset = 0
                             for y_split_index, y_split in enumerate(z_split):
                                 region = [slice(shape[i]) for i in range(ndim)]
-                                region[z_index] = slice(z_offset, z_offset+y_split.shape[z_index])
-                                region[y_index] = slice(y_offset, y_offset+y_split.shape[y_index])
-                                offset = [0,]*ndim
+                                region[z_index] = slice(
+                                    z_offset, z_offset + y_split.shape[z_index]
+                                )
+                                region[y_index] = slice(
+                                    y_offset, y_offset + y_split.shape[y_index]
+                                )
+                                offset = [
+                                    0,
+                                ] * ndim
                                 offset[z_index] = z_offset
                                 offset[y_index] = y_offset
-                                regions[(z_split_index, y_split_index, 0)] = tuple(region), tuple(offset)
+                                regions[(z_split_index, y_split_index, 0)] = tuple(
+                                    region
+                                ), tuple(offset)
                                 y_offset += y_split.shape[y_index]
                             z_offset += z_split[0].shape[z_index]
                 else:
                     z_splits = _array_split(blurred_array, num_z_splits, z_index)
                     z_offset = 0
                     for split_index, split in enumerate(z_splits):
                         region = [slice(shape[i]) for i in range(ndim)]
-                        region[z_index] = slice(z_offset, z_offset+split.shape[z_index])
-                        offset = [0,]*ndim
+                        region[z_index] = slice(
+                            z_offset, z_offset + split.shape[z_index]
+                        )
+                        offset = [
+                            0,
+                        ] * ndim
                         offset[z_index] = z_offset
                         regions[(split_index, 0, 0)] = tuple(region), tuple(offset)
                         z_offset += split.shape[z_index]
 
-                blurred_region = blurred_array[regions[(0,0,0)][0]]
+                blurred_region = blurred_array[regions[(0, 0, 0)][0]]
                 region_output_shape = [
                     arr_len // shrink_factor
                     for arr_len, shrink_factor in zip(
                         blurred_region.shape, shrink_factors
                     )
                 ]
                 while region_output_shape[z_index] % shrink_factors[z_index] != 0:
                     region_output_shape[z_index] -= 1
                 while region_output_shape[y_index] % shrink_factors[y_index] != 0:
                     region_output_shape[y_index] -= 1
                 while region_output_shape[x_index] % shrink_factors[x_index] != 0:
                     region_output_shape[x_index] -= 1
-                def downscale_region(region, offset):
-                    blurred_region = blurred_array[region]
-                    downscaled_region = dask_image.ndinterp.affine_transform(
+
+                def downscale_region(
+                    region,  # noqa: ARG001
+                    offset,
+                    blurred_array=blurred_array,
+                    transform=transform,
+                    region_output_shape=region_output_shape,
+                    order=order,
+                ):
+                    # TODO: this should be transformed??
+                    # blurred_region = blurred_array[region]
+                    return dask_image.ndinterp.affine_transform(
                         blurred_array,
                         matrix=transform,
                         offset=offset,
                         output_shape=tuple(region_output_shape),  # tzyx order
                         order=order,
                     )
-                    return downscaled_region
+
                 z_splits = []
                 for z_split in range(num_z_splits):
                     y_splits = []
                     for y_split in range(num_y_splits):
                         x_splits = []
                         for x_split in range(num_x_splits):
                             region, offset = regions[(z_split, y_split, x_split)]
@@ -334,15 +377,17 @@
                 output_shape = [
                     arr_len // shrink_factor
                     for arr_len, shrink_factor in zip(
                         blurred_array.shape, shrink_factors
                     )
                 ]
                 # trim
-                downscaled_array = downscaled_array[tuple([slice(output_shape[i]) for i in range(ndim)])]
+                downscaled_array = downscaled_array[
+                    tuple([slice(output_shape[i]) for i in range(ndim)])
+                ]
             else:
                 # Todo: downsample 2D images
                 downscaled_array = dask_image.ndinterp.affine_transform(
                     blurred_array,
                     matrix=transform,
                     order=order,
                     output_shape=output_shape,  # tzyx order
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/methods/_itk.py` & `ngff_zarr-0.4.6/ngff_zarr/methods/_itk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,114 +1,138 @@
 from typing import Tuple
 
 import numpy as np
+from dask.array import concatenate, expand_dims, map_blocks, map_overlap, take
 
-from dask.array import map_blocks, map_overlap, take, concatenate, expand_dims
-
-from ._support import _align_chunks, _dim_scale_factors, _compute_sigma, _spatial_dims
 from ..ngff_image import NgffImage
+from ._support import _align_chunks, _compute_sigma, _dim_scale_factors, _spatial_dims
 
 _image_dims: Tuple[str, str, str, str] = ("x", "y", "z", "t")
 
+
 def _get_block(previous_image: NgffImage, block_index: int):
-    '''Helper method for accessing an enumerated chunk from input'''
+    """Helper method for accessing an enumerated chunk from input"""
     block_shape = [c[block_index] for c in previous_image.data.chunks]
     block = previous_image.data[tuple([slice(0, s) for s in block_shape])]
     # For consistency for now, do not utilize direction until there is standardized support for
     # direction cosines / orientation in OME-NGFF
     # block.attrs.pop("direction", None)
-    if 't' in previous_image.dims:
+    if "t" in previous_image.dims:
         dims = list(previous_image.dims)
-        t_index = dims.index('t')
+        t_index = dims.index("t")
         block = take(block, 0, t_index)
     return block
 
-def _compute_itk_gaussian_kernel_radius(input_size, sigma_values, shrink_factors) -> list:
-    '''Get kernel radius in xyzt directions'''
+
+def _compute_itk_gaussian_kernel_radius(input_size, sigma_values) -> list:
+    """Get kernel radius in xyzt directions"""
     DEFAULT_MAX_KERNEL_WIDTH = 32
     MAX_KERNEL_ERROR = 0.01
     image_dimension = len(input_size)
 
     import itk
 
     # Constrain kernel width to be at most the size of one chunk
     max_kernel_width = min(DEFAULT_MAX_KERNEL_WIDTH, *input_size)
-    variance = [sigma ** 2 for sigma in sigma_values]
+    variance = [sigma**2 for sigma in sigma_values]
 
-    def generate_radius(direction:int) -> int:
-        '''Follow itk.DiscreteGaussianImageFilter procedure to generate directional kernels'''
+    def generate_radius(direction: int) -> int:
+        """Follow itk.DiscreteGaussianImageFilter procedure to generate directional kernels"""
         oper = itk.GaussianOperator[itk.F, image_dimension]()
         oper.SetDirection(direction)
         oper.SetMaximumError(MAX_KERNEL_ERROR)
         oper.SetMaximumKernelWidth(max_kernel_width)
         oper.SetVariance(variance[direction])
         oper.CreateDirectional()
         return oper.GetRadius(direction)
 
     return [generate_radius(dim) for dim in range(image_dimension)]
 
 
-def _itk_blur_and_downsample(image_data, gaussian_filter_name, interpolator_name, shrink_factors, sigma_values, kernel_radius):
-    '''Blur and then downsample a given image chunk'''
+def _itk_blur_and_downsample(
+    image_data,
+    gaussian_filter_name,
+    interpolator_name,
+    shrink_factors,
+    sigma_values,
+    kernel_radius,
+):
+    """Blur and then downsample a given image chunk"""
     import itk
 
     # chunk does not have metadata attached, values are ITK defaults
     image = itk.image_view_from_array(image_data)
     input_origin = itk.origin(image)
 
     # Skip this image block if it has 0 voxels
     block_size = itk.size(image)
-    if(any([block_len == 0 for block_len in block_size])):
+    if any(block_len == 0 for block_len in block_size):
         return None
 
     # Output values are relative to input
     itk_shrink_factors = shrink_factors  # xyzt
     itk_kernel_radius = kernel_radius
-    output_origin = [val + radius for val, radius in zip(input_origin, itk_kernel_radius)]
+    output_origin = [
+        val + radius for val, radius in zip(input_origin, itk_kernel_radius)
+    ]
     output_spacing = [s * f for s, f in zip(itk.spacing(image), itk_shrink_factors)]
-    output_size = [max(0,int((image_len - 2 * radius) / shrink_factor))
-        for image_len, radius, shrink_factor in zip(itk.size(image), itk_kernel_radius, itk_shrink_factors)]
+    output_size = [
+        max(0, int((image_len - 2 * radius) / shrink_factor))
+        for image_len, radius, shrink_factor in zip(
+            itk.size(image), itk_kernel_radius, itk_shrink_factors
+        )
+    ]
 
     # Optionally run accelerated smoothing with itk-vkfft
-    if gaussian_filter_name == 'VkDiscreteGaussianImageFilter':
+    if gaussian_filter_name == "VkDiscreteGaussianImageFilter":
         smoothing_filter_template = itk.VkDiscreteGaussianImageFilter
-    elif gaussian_filter_name == 'DiscreteGaussianImageFilter':
+    elif gaussian_filter_name == "DiscreteGaussianImageFilter":
         smoothing_filter_template = itk.DiscreteGaussianImageFilter
     else:
-        raise ValueError(f'Unsupported gaussian_filter {gaussian_filter_name}')
+        msg = f"Unsupported gaussian_filter {gaussian_filter_name}"
+        raise ValueError(msg)
 
     # Construct pipeline
-    smoothing_filter = smoothing_filter_template.New(image,
-        sigma_array=sigma_values,
-        use_image_spacing=False)
-
-    if interpolator_name == 'LinearInterpolateImageFunction':
-        interpolator_instance = itk.LinearInterpolateImageFunction.New(smoothing_filter.GetOutput())
-    elif interpolator_name == 'LabelImageGaussianInterpolateImageFunction':
-        interpolator_instance = itk.LabelImageGaussianInterpolateImageFunction.New(smoothing_filter.GetOutput())
+    smoothing_filter = smoothing_filter_template.New(
+        image, sigma_array=sigma_values, use_image_spacing=False
+    )
+
+    if interpolator_name == "LinearInterpolateImageFunction":
+        interpolator_instance = itk.LinearInterpolateImageFunction.New(
+            smoothing_filter.GetOutput()
+        )
+    elif interpolator_name == "LabelImageGaussianInterpolateImageFunction":
+        interpolator_instance = itk.LabelImageGaussianInterpolateImageFunction.New(
+            smoothing_filter.GetOutput()
+        )
         # Similar approach as compute_sigma
         # Ref: https://link.springer.com/content/pdf/10.1007/978-3-319-24571-3_81.pdf
         sigma = [s * 0.7355 for s in output_spacing]
         sigma_max = max(sigma)
         interpolator_instance.SetSigma(sigma)
         interpolator_instance.SetAlpha(sigma_max * 2.5)
     else:
-        raise ValueError(f'Unsupported interpolator_name {interpolator_name}')
+        msg = f"Unsupported interpolator_name {interpolator_name}"
+        raise ValueError(msg)
 
-    shrink_filter = itk.ResampleImageFilter.New(smoothing_filter.GetOutput(),
+    shrink_filter = itk.ResampleImageFilter.New(
+        smoothing_filter.GetOutput(),
         interpolator=interpolator_instance,
         size=output_size,
         output_spacing=output_spacing,
-        output_origin=output_origin)
+        output_origin=output_origin,
+    )
     shrink_filter.Update()
 
     return np.asarray(shrink_filter.GetOutput())
 
 
-def _downsample_itk_bin_shrink(ngff_image: NgffImage, default_chunks, out_chunks, scale_factors):
+def _downsample_itk_bin_shrink(
+    ngff_image: NgffImage, default_chunks, out_chunks, scale_factors
+):
     import itk
 
     multiscales = [
         ngff_image,
     ]
     previous_image = ngff_image
     dims = ngff_image.dims
@@ -127,22 +151,18 @@
         # direction cosines / orientation in OME-NGFF
         # block_0.attrs.pop("direction", None)
         block_input = itk.image_from_array(np.ones_like(block_0))
         spacing = [previous_image.scale[d] for d in spatial_dims]
         block_input.SetSpacing(spacing)
         origin = [previous_image.translation[d] for d in spatial_dims]
         block_input.SetOrigin(origin)
-        filt = itk.BinShrinkImageFilter.New(
-            block_input, shrink_factors=shrink_factors
-        )
+        filt = itk.BinShrinkImageFilter.New(block_input, shrink_factors=shrink_factors)
         filt.UpdateOutputInformation()
         block_output = filt.GetOutput()
-        scale = {
-            _image_dims[i]: s for (i, s) in enumerate(block_output.GetSpacing())
-        }
+        scale = {_image_dims[i]: s for (i, s) in enumerate(block_output.GetSpacing())}
         translation = {
             _image_dims[i]: s for (i, s) in enumerate(block_output.GetOrigin())
         }
         dtype = block_output.dtype
         output_chunks = list(previous_image.data.chunks)
         for i, c in enumerate(output_chunks):
             output_chunks[i] = [
@@ -150,20 +170,18 @@
             ] * len(c)
 
         block_neg1 = _get_block(previous_image, -1)
         # block_neg1.attrs.pop("direction", None)
         block_input = itk.image_from_array(np.ones_like(block_neg1))
         block_input.SetSpacing(spacing)
         block_input.SetOrigin(origin)
-        filt = itk.BinShrinkImageFilter.New(
-            block_input, shrink_factors=shrink_factors
-        )
+        filt = itk.BinShrinkImageFilter.New(block_input, shrink_factors=shrink_factors)
         filt.UpdateOutputInformation()
         block_output = filt.GetOutput()
-        for i, c in enumerate(output_chunks):
+        for i in range(len(output_chunks)):
             output_chunks[i][-1] = block_output.shape[i]
             output_chunks[i] = tuple(output_chunks[i])
         output_chunks = tuple(output_chunks)
 
         downscaled_array = map_blocks(
             itk.bin_shrink_image_filter,
             previous_image.data,
@@ -175,32 +193,32 @@
         for dim in dims:
             if dim in out_chunks:
                 out_chunks_list.append(out_chunks[dim])
             else:
                 out_chunks_list.append(1)
         downscaled_array = downscaled_array.rechunk(tuple(out_chunks_list))
 
-        previous_image = NgffImage(
-            downscaled_array, dims, scale, translation
-        )
+        previous_image = NgffImage(downscaled_array, dims, scale, translation)
         multiscales.append(previous_image)
 
     return multiscales
 
 
-def _downsample_itk_gaussian(ngff_image: NgffImage, default_chunks, out_chunks, scale_factors):
+def _downsample_itk_gaussian(
+    ngff_image: NgffImage, default_chunks, out_chunks, scale_factors
+):
     import itk
 
     # Optionally run accelerated smoothing with itk-vkfft
-    if 'VkFFTBackend' in dir(itk):
-        gaussian_filter_name = 'VkDiscreteGaussianImageFilter'
+    if "VkFFTBackend" in dir(itk):
+        gaussian_filter_name = "VkDiscreteGaussianImageFilter"
     else:
-        gaussian_filter_name = 'DiscreteGaussianImageFilter'
+        gaussian_filter_name = "DiscreteGaussianImageFilter"
 
-    interpolator_name = 'LinearInterpolateImageFunction'
+    interpolator_name = "LinearInterpolateImageFunction"
 
     multiscales = [
         ngff_image,
     ]
     previous_image = ngff_image
     dims = ngff_image.dims
     previous_dim_factors = {d: 1 for d in dims}
@@ -223,212 +241,238 @@
         block_0_image = itk.image_from_array(np.ones_like(block_0_input))
         input_spacing = [previous_image.scale[d] for d in spatial_dims]
         block_0_image.SetSpacing(input_spacing)
         input_origin = [previous_image.translation[d] for d in spatial_dims]
         block_0_image.SetOrigin(input_origin)
 
         sigma_values = _compute_sigma(input_spacing, shrink_factors)
-        kernel_radius = _compute_itk_gaussian_kernel_radius(itk.size(block_0_image), sigma_values, shrink_factors)
+        kernel_radius = _compute_itk_gaussian_kernel_radius(
+            itk.size(block_0_image), sigma_values
+        )
 
         # Compute output size and spatial metadata for blocks 0, .., N-2
         filt = itk.BinShrinkImageFilter.New(
             block_0_image, shrink_factors=shrink_factors
         )
         filt.UpdateOutputInformation()
         block_output = filt.GetOutput()
         block_0_output_spacing = block_output.GetSpacing()
         block_0_output_origin = block_output.GetOrigin()
 
-        scale = {
-            _image_dims[i]: s for (i, s) in enumerate(block_0_output_spacing)
-        }
-        translation = {
-            _image_dims[i]: s for (i, s) in enumerate(block_0_output_origin)
-        }
+        scale = {_image_dims[i]: s for (i, s) in enumerate(block_0_output_spacing)}
+        translation = {_image_dims[i]: s for (i, s) in enumerate(block_0_output_origin)}
         dtype = block_output.dtype
 
-        computed_size = [int(block_len / shrink_factor)
-            for block_len, shrink_factor in zip(itk.size(block_0_image), shrink_factors)]
-        assert all([itk.size(block_output)[dim] == computed_size[dim]
-                    for dim in range(block_output.ndim)])
+        computed_size = [
+            int(block_len / shrink_factor)
+            for block_len, shrink_factor in zip(itk.size(block_0_image), shrink_factors)
+        ]
+        assert all(
+            itk.size(block_output)[dim] == computed_size[dim]
+            for dim in range(block_output.ndim)
+        )
         output_chunks = list(previous_image.data.chunks)
-        if 't' in previous_image.dims:
+        if "t" in previous_image.dims:
             dims = list(previous_image.dims)
-            t_index = dims.index('t')
+            t_index = dims.index("t")
             output_chunks.pop(t_index)
         for i, c in enumerate(output_chunks):
             output_chunks[i] = [
                 block_output.shape[i],
             ] * len(c)
         # Compute output size for block N-1
         block_neg1_image = itk.image_from_array(np.ones_like(block_neg1_input))
         block_neg1_image.SetSpacing(input_spacing)
         block_neg1_image.SetOrigin(input_origin)
         filt.SetInput(block_neg1_image)
         filt.UpdateOutputInformation()
         block_output = filt.GetOutput()
-        computed_size = [int(block_len / shrink_factor)
-            for block_len, shrink_factor in zip(itk.size(block_neg1_image), shrink_factors)]
-        assert all([itk.size(block_output)[dim] == computed_size[dim]
-                    for dim in range(block_output.ndim)])
-        for i, c in enumerate(output_chunks):
+        computed_size = [
+            int(block_len / shrink_factor)
+            for block_len, shrink_factor in zip(
+                itk.size(block_neg1_image), shrink_factors
+            )
+        ]
+        assert all(
+            itk.size(block_output)[dim] == computed_size[dim]
+            for dim in range(block_output.ndim)
+        )
+        for i in range(len(output_chunks)):
             output_chunks[i][-1] = block_output.shape[i]
             output_chunks[i] = tuple(output_chunks[i])
         output_chunks = tuple(output_chunks)
 
-        if 't' in previous_image.dims:
+        if "t" in previous_image.dims:
             all_timepoints = []
             for timepoint in range(previous_image.data.shape[t_index]):
                 data = take(previous_image.data, timepoint, t_index)
 
                 downscaled_timepoint = map_overlap(
                     _itk_blur_and_downsample,
                     data,
                     gaussian_filter_name=gaussian_filter_name,
                     interpolator_name=interpolator_name,
                     shrink_factors=shrink_factors,
                     sigma_values=sigma_values,
                     kernel_radius=kernel_radius,
                     dtype=dtype,
-                    depth={dim: radius for dim, radius in enumerate(np.flip(kernel_radius))}, # overlap is in tzyx
-                    boundary='nearest',
+                    depth=dict(enumerate(np.flip(kernel_radius))),  # overlap is in tzyx
+                    boundary="nearest",
                     trim=False,  # Overlapped region is trimmed in blur_and_downsample to output size
                     chunks=output_chunks,
                 )
                 expanded = expand_dims(downscaled_timepoint, t_index)
                 all_timepoints.append(expanded)
             downscaled_array = concatenate(all_timepoints, t_index)
         else:
             data = previous_image.data
             downscaled_array = map_overlap(
-              _itk_blur_and_downsample,
-              data,
-              gaussian_filter_name=gaussian_filter_name,
-              interpolator_name=interpolator_name,
-              shrink_factors=shrink_factors,
-              sigma_values=sigma_values,
-              kernel_radius=kernel_radius,
-              dtype=dtype,
-              depth={dim: radius for dim, radius in enumerate(np.flip(kernel_radius))}, # overlap is in tzyx
-              boundary='nearest',
-              trim=False,  # Overlapped region is trimmed in blur_and_downsample to output size
-              chunks=output_chunks,
+                _itk_blur_and_downsample,
+                data,
+                gaussian_filter_name=gaussian_filter_name,
+                interpolator_name=interpolator_name,
+                shrink_factors=shrink_factors,
+                sigma_values=sigma_values,
+                kernel_radius=kernel_radius,
+                dtype=dtype,
+                depth=dict(enumerate(np.flip(kernel_radius))),  # overlap is in tzyx
+                boundary="nearest",
+                trim=False,  # Overlapped region is trimmed in blur_and_downsample to output size
+                chunks=output_chunks,
             )
 
         out_chunks_list = []
         for dim in dims:
             if dim in out_chunks:
                 out_chunks_list.append(out_chunks[dim])
             else:
                 out_chunks_list.append(1)
         downscaled_array = downscaled_array.rechunk(tuple(out_chunks_list))
 
-        previous_image = NgffImage(
-            downscaled_array, dims, scale, translation
-        )
+        previous_image = NgffImage(downscaled_array, dims, scale, translation)
         multiscales.append(previous_image)
 
     return multiscales
 
-def _downsample_itk_label(current_input, default_chunks, out_chunks, scale_factors, data_objects, image):
-    # Uses the LabelImageGaussianInterpolateImageFunction. More appropriate for integer label images.
-    import itk
-
-    gaussian_filter_name = 'DiscreteGaussianImageFilter'
-    interpolator_name = 'LabelImageGaussianInterpolateImageFunction'
-
-    for factor_index, scale_factor in enumerate(scale_factors):
-        dim_factors = _dim_scale_factors(image.dims, scale_factor)
-        current_input = _align_chunks(current_input, default_chunks, dim_factors)
-
-        shrink_factors = [dim_factors[sf] for sf in _image_dims if sf in dim_factors]
-
-        # Compute metadata for region splitting
-
-        # Blocks 0, ..., N-2 have the same shape
-        block_0_input = _get_block(current_input,0)
-        # Block N-1 may be smaller than preceding blocks
-        block_neg1_input = _get_block(current_input,-1)
-
-        # Compute overlap for Gaussian blurring for all blocks
-        block_0_image = itk.image_from_xarray(block_0_input)
-        input_spacing = itk.spacing(block_0_image)
-        sigma_values = _compute_sigma(input_spacing, shrink_factors)
-        kernel_radius = _compute_itk_gaussian_kernel_radius(itk.size(block_0_image), sigma_values, shrink_factors)
-
-        # Compute output size and spatial metadata for blocks 0, .., N-2
-        filt = itk.BinShrinkImageFilter.New(
-            block_0_image, shrink_factors=shrink_factors
-        )
-        filt.UpdateOutputInformation()
-        block_output = filt.GetOutput()
-        block_0_output_spacing = block_output.GetSpacing()
-        block_0_output_origin = block_output.GetOrigin()
-
-        block_0_scale = {
-            _image_dims[i]: s for (i, s) in enumerate(block_0_output_spacing)
-        }
-        block_0_translation = {
-            _image_dims[i]: s for (i, s) in enumerate(block_0_output_origin)
-        }
-        dtype = block_output.dtype
 
-        computed_size = [int(block_len / shrink_factor)
-            for block_len, shrink_factor in zip(itk.size(block_0_image), shrink_factors)]
-        assert all([itk.size(block_output)[dim] == computed_size[dim]
-                    for dim in range(block_output.ndim)])
-        output_chunks = list(current_input.chunks)
-        for i, c in enumerate(output_chunks):
-            output_chunks[i] = [
-                block_output.shape[i],
-            ] * len(c)
-
-        # Compute output size for block N-1
-        block_neg1_image = itk.image_from_xarray(block_neg1_input)
-        filt.SetInput(block_neg1_image)
-        filt.UpdateOutputInformation()
-        block_output = filt.GetOutput()
-        computed_size = [int(block_len / shrink_factor)
-            for block_len, shrink_factor in zip(itk.size(block_neg1_image), shrink_factors)]
-        assert all([itk.size(block_output)[dim] == computed_size[dim]
-                    for dim in range(block_output.ndim)])
-        for i, c in enumerate(output_chunks):
-            output_chunks[i][-1] = block_output.shape[i]
-            output_chunks[i] = tuple(output_chunks[i])
-        output_chunks = tuple(output_chunks)
-
-        downscaled_array = map_overlap(
-          _itk_blur_and_downsample,
-          current_input.data,
-          gaussian_filter_name=gaussian_filter_name,
-          interpolator_name=interpolator_name,
-          shrink_factors=shrink_factors,
-          sigma_values=sigma_values,
-          kernel_radius=kernel_radius,
-          dtype=dtype,
-          depth={dim: radius for dim, radius in enumerate(np.flip(kernel_radius))}, # overlap is in tzyx
-          boundary='nearest',
-          trim=False   # Overlapped region is trimmed in blur_and_downsample to output size
-        ).compute()
-
-        downscaled = to_spatial_image(
-            downscaled_array,
-            dims=image.dims,
-            scale=block_0_scale,
-            translation=block_0_translation,
-            name=current_input.name,
-            axis_names={
-                d: image.coords[d].attrs.get("long_name", d) for d in image.dims
-            },
-            axis_units={
-                d: image.coords[d].attrs.get("units", "") for d in image.dims
-            },
-            t_coords=image.coords.get("t", None),
-            c_coords=image.coords.get("c", None),
-        )
-        downscaled = downscaled.chunk(out_chunks)
-        data_objects[f"scale{factor_index+1}"] = downscaled.to_dataset(
-            name=image.name, promote_attrs=True
-        )
-        current_input = downscaled
+# todo
+# def _downsample_itk_label(
+#     current_input,
+#     default_chunks,
+#     out_chunks,
+#     scale_factors,
+#     data_objects,
+#     image,
+# ):
+# Uses the LabelImageGaussianInterpolateImageFunction. More appropriate for integer label images.
+# import itk
+
+# gaussian_filter_name = "DiscreteGaussianImageFilter"
+# interpolator_name = "LabelImageGaussianInterpolateImageFunction"
+
+# for _factor_index, scale_factor in enumerate(scale_factors):
+#     dim_factors = _dim_scale_factors(image.dims, scale_factor)
+#     current_input = _align_chunks(current_input, default_chunks, dim_factors)
+
+#     shrink_factors = [dim_factors[sf] for sf in _image_dims if sf in dim_factors]
+
+#     # Compute metadata for region splitting
+
+#     # Blocks 0, ..., N-2 have the same shape
+#     block_0_input = _get_block(current_input, 0)
+#     # Block N-1 may be smaller than preceding blocks
+#     block_neg1_input = _get_block(current_input, -1)
+
+#     # Compute overlap for Gaussian blurring for all blocks
+#     block_0_image = itk.image_from_xarray(block_0_input)
+#     input_spacing = itk.spacing(block_0_image)
+#     sigma_values = _compute_sigma(input_spacing, shrink_factors)
+#     kernel_radius = _compute_itk_gaussian_kernel_radius(
+#         itk.size(block_0_image), sigma_values
+#     )
+
+#     # Compute output size and spatial metadata for blocks 0, .., N-2
+#     filt = itk.BinShrinkImageFilter.New(
+#         block_0_image, shrink_factors=shrink_factors
+#     )
+#     filt.UpdateOutputInformation()
+#     block_output = filt.GetOutput()
+#     block_0_output_spacing = block_output.GetSpacing()
+#     block_0_output_origin = block_output.GetOrigin()
+
+#     block_0_scale = {
+#         _image_dims[i]: s for (i, s) in enumerate(block_0_output_spacing)
+#     }
+#     block_0_translation = {
+#         _image_dims[i]: s for (i, s) in enumerate(block_0_output_origin)
+#     }
+#     dtype = block_output.dtype
+
+#     computed_size = [
+#         int(block_len / shrink_factor)
+#         for block_len, shrink_factor in zip(itk.size(block_0_image), shrink_factors)
+#     ]
+#     assert all(
+#         itk.size(block_output)[dim] == computed_size[dim]
+#         for dim in range(block_output.ndim)
+#     )
+#     output_chunks = list(current_input.chunks)
+#     for i, c in enumerate(output_chunks):
+#         output_chunks[i] = [
+#             block_output.shape[i],
+#         ] * len(c)
+
+#     # Compute output size for block N-1
+#     block_neg1_image = itk.image_from_xarray(block_neg1_input)
+#     filt.SetInput(block_neg1_image)
+#     filt.UpdateOutputInformation()
+#     block_output = filt.GetOutput()
+#     computed_size = [
+#         int(block_len / shrink_factor)
+#         for block_len, shrink_factor in zip(
+#             itk.size(block_neg1_image), shrink_factors
+#         )
+#     ]
+#     assert all(
+#         itk.size(block_output)[dim] == computed_size[dim]
+#         for dim in range(block_output.ndim)
+#     )
+#     for i in range(len(output_chunks)):
+#         output_chunks[i][-1] = block_output.shape[i]
+#         output_chunks[i] = tuple(output_chunks[i])
+#     output_chunks = tuple(output_chunks)
+
+#     downscaled_array = map_overlap(
+#         _itk_blur_and_downsample,
+#         current_input.data,
+#         gaussian_filter_name=gaussian_filter_name,
+#         interpolator_name=interpolator_name,
+#         shrink_factors=shrink_factors,
+#         sigma_values=sigma_values,
+#         kernel_radius=kernel_radius,
+#         dtype=dtype,
+#         depth=dict(enumerate(np.flip(kernel_radius))),  # overlap is in tzyx
+#         boundary="nearest",
+#         trim=False,  # Overlapped region is trimmed in blur_and_downsample to output size
+#     ).compute()
+
+#     # todo
+#     # downscaled = to_spatial_image(
+#     #     downscaled_array,
+#     #     dims=image.dims,
+#     #     scale=block_0_scale,
+#     #     translation=block_0_translation,
+#     #     name=current_input.name,
+#     #     axis_names={
+#     #         d: image.coords[d].attrs.get("long_name", d) for d in image.dims
+#     #     },
+#     #     axis_units={d: image.coords[d].attrs.get("units", "") for d in image.dims},
+#     #     t_coords=image.coords.get("t", None),
+#     #     c_coords=image.coords.get("c", None),
+#     # )
+#     # downscaled = downscaled.chunk(out_chunks)
+#     # data_objects[f"scale{factor_index+1}"] = downscaled.to_dataset(
+#     #     name=image.name, promote_attrs=True
+#     # )
+#     # current_input = downscaled
 
-    return data_objects
+# return data_objects
```

### Comparing `ngff_zarr-0.4.5/ngff_zarr/methods/_support.py` & `ngff_zarr-0.4.6/ngff_zarr/methods/_support.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 _spatial_dims = {"x", "y", "z"}
 
 
 def _dim_scale_factors(dims, scale_factor, previous_dim_factors):
     if isinstance(scale_factor, int):
         result_scale_factors = {
-            dim: int(scale_factor / previous_dim_factors[dim]) for dim in _spatial_dims.intersection(dims)
+            dim: int(scale_factor / previous_dim_factors[dim])
+            for dim in _spatial_dims.intersection(dims)
         }
     else:
-        result_scale_factors = { d:int(scale_factor[d] / previous_dim_factors[d]) for d in scale_factor.keys() }
+        result_scale_factors = {
+            d: int(scale_factor[d] / previous_dim_factors[d]) for d in scale_factor
+        }
     return result_scale_factors
 
 
 def _align_chunks(previous_image, default_chunks, dim_factors):
     block_0_shape = [c[0] for c in previous_image.data.chunks]
 
     rechunk = False
@@ -20,16 +23,18 @@
         dim_index = previous_image.dims.index(dim)
         if block_0_shape[dim_index] % factor:
             aligned_chunks[dim] = block_0_shape[dim_index] * factor
             rechunk = True
         else:
             aligned_chunks[dim] = default_chunks[dim]
     if rechunk:
-        dask_aligned_chunks = { previous_image.dims.index(dim):
-                aligned_chunks[dim] for dim in aligned_chunks.keys() }
+        dask_aligned_chunks = {
+            previous_image.dims.index(dim): aligned_chunks[dim]
+            for dim in aligned_chunks
+        }
         previous_image.data = previous_image.data.rechunk(dask_aligned_chunks)
 
     return previous_image
 
 
 def _compute_sigma(input_spacings, shrink_factors) -> list:
     """Compute Gaussian kernel sigma values for resampling to isotropic spacing.
```

### Comparing `ngff_zarr-0.4.5/test/_data.py` & `ngff_zarr-0.4.6/test/_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Sequence, Dict
+import sys
 from pathlib import Path
 
-import pytest
-import pooch
 import itk
-from zarr.storage import DirectoryStore, MemoryStore
-
+import pooch
+import pytest
 from ngff_zarr import itk_image_to_ngff_image, to_ngff_zarr
+from zarr.storage import DirectoryStore, MemoryStore
 
 test_data_ipfs_cid = "bafybeid6tqv7og52ycwwwmy6wcsdzgh5a7zwyc7fnsguin3st2at35pvs4"
 test_data_sha256 = "2b116ecf57856d0ca7f3f4f0f30fe4a4daa1fbc38d40a41e5c13b3cb836036c3"
 
 
 test_dir = Path(__file__).resolve().parent
 extract_dir = "data"
@@ -21,15 +20,15 @@
     registry={
         "data.tar.gz": f"sha256:{test_data_sha256}",
     },
     retry_if_failed=5,
 )
 
 
-@pytest.fixture
+@pytest.fixture(scope="package")
 def input_images():
     untar = pooch.Untar(extract_dir=extract_dir)
     test_data.fetch("data.tar.gz", processor=untar)
     result = {}
 
     # store = DirectoryStore(
     #     test_data_dir / "input" / "cthead1.zarr", dimension_separator="/"
@@ -38,15 +37,18 @@
     # image_da = image_ds.cthead1
     image = itk.imread(test_data_dir / "input" / "cthead1.png")
     image_ngff = itk_image_to_ngff_image(image)
     result["cthead1"] = image_ngff
 
     result["lung_series"] = test_data_dir / "input" / "lung_series" / "*"
 
-    image = itk.imread(test_data_dir / "input" / "brain_two_components.nrrd", itk.VariableLengthVector[itk.SS])
+    image = itk.imread(
+        test_data_dir / "input" / "brain_two_components.nrrd",
+        itk.VariableLengthVector[itk.SS],
+    )
     image_ngff = itk_image_to_ngff_image(image)
     result["brain_two_components"] = image_ngff
 
     # store = DirectoryStore(
     #     test_data_dir / "input" / "small_head.zarr", dimension_separator="/"
     # )
     # image_ds = xr.open_zarr(store)
@@ -58,38 +60,43 @@
     # )
     # image_ds = xr.open_zarr(store)
     # image_da = image_ds['2th_cthead1']
     # result["2th_cthead1"] = image_da
 
     return result
 
+
 def store_equals(baseline_store, test_store):
     baseline_keys = set(baseline_store.keys())
     test_keys = set(test_store.keys())
     if baseline_keys != test_keys:
-        print('test keys != baseline keys')
-        print('baseline - test:', baseline_keys.difference(test_keys))
-        print('test - baseline:', test_keys.difference(baseline_keys))
+        sys.stderr.write("test keys != baseline keys\n")
+        sys.stderr.write("baseline - test:", baseline_keys.difference(test_keys), "\n")
+        sys.stderr.write("test - baseline:", test_keys.difference(baseline_keys), "\n")
         return False
     for k in baseline_keys:
         if baseline_store[k] != test_store[k]:
-            print(f'test value != baseline value for key {k}')
-            print('baseline:', baseline_store[k])
-            print('test:', test_store[k])
+            sys.stderr.write(f"test value != baseline value for key {k}\n")
+            sys.stderr.write("baseline:", baseline_store[k], "\n")
+            sys.stderr.write("test:", test_store[k], "\n")
             return False
     return True
 
+
 def verify_against_baseline(dataset_name, baseline_name, multiscales):
     baseline_store = DirectoryStore(
-        test_data_dir / f"baseline/{dataset_name}/{baseline_name}", dimension_separator="/"
+        test_data_dir / f"baseline/{dataset_name}/{baseline_name}",
+        dimension_separator="/",
     )
-    test_store =  MemoryStore(dimension_separator='/')
+    test_store = MemoryStore(dimension_separator="/")
     to_ngff_zarr(test_store, multiscales)
     assert store_equals(baseline_store, test_store)
 
+
 def store_new_multiscales(dataset_name, baseline_name, multiscales):
-    '''Helper method for writing output results to disk
-       for later upload as test baseline'''
+    """Helper method for writing output results to disk
+    for later upload as test baseline"""
     store = DirectoryStore(
-        test_data_dir / f"baseline/{dataset_name}/{baseline_name}", dimension_separator="/",
+        test_data_dir / f"baseline/{dataset_name}/{baseline_name}",
+        dimension_separator="/",
     )
     to_ngff_zarr(store, multiscales)
```

### Comparing `ngff_zarr-0.4.5/test/test_from_ngff_zarr.py` & `ngff_zarr-0.4.6/test/test_from_ngff_zarr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-from ngff_zarr import Methods, to_ngff_zarr, from_ngff_zarr, to_multiscales, to_ngff_image
-from zarr.storage import MemoryStore
-
-from ._data import input_images, store_new_multiscales, verify_against_baseline
-
 from dask_image import imread
+from ngff_zarr import (
+    Methods,
+    to_multiscales,
+    to_ngff_image,
+    to_ngff_zarr,
+)
+from zarr.storage import MemoryStore
 
+from ._data import verify_against_baseline
 
 
 def test_gaussian_isotropic_scale_factors(input_images):
     dataset_name = "cthead1"
     image = input_images[dataset_name]
     baseline_name = "2_4/DASK_IMAGE_GAUSSIAN.zarr"
     multiscales = to_multiscales(image, [2, 4], method=Methods.DASK_IMAGE_GAUSSIAN)
     # store_new_multiscales(dataset_name, f'{baseline_name}', multiscales)
     verify_against_baseline(dataset_name, baseline_name, multiscales)
 
 
 def test_from_ngff_zarr(input_images):
     dataset_name = "lung_series"
     data = imread.imread(input_images[dataset_name])
-    image = to_ngff_image(data=data,
-                          dims=('z', 'y', 'x'),
-                          scale={'z': 2.5, 'y': 1.40625, 'x': 1.40625},
-                          translation={'z': 332.5, 'y': 360., 'x': 0.0},
-                          name='LIDC2')
+    image = to_ngff_image(
+        data=data,
+        dims=("z", "y", "x"),
+        scale={"z": 2.5, "y": 1.40625, "x": 1.40625},
+        translation={"z": 332.5, "y": 360.0, "x": 0.0},
+        name="LIDC2",
+    )
     multiscales = to_multiscales(image)
     multiscales.scale_factors = None
     multiscales.method = None
     multiscales.chunks = None
     baseline_name = "from_ngff_zarr"
     # store_new_multiscales(dataset_name, baseline_name, multiscales)
     verify_against_baseline(dataset_name, baseline_name, multiscales)
-    test_store =  MemoryStore(dimension_separator='/')
+    test_store = MemoryStore(dimension_separator="/")
     to_ngff_zarr(test_store, multiscales)
 
-    multiscales_back = from_ngff_zarr(test_store)
+    # multiscales_back = from_ngff_zarr(test_store)
     # verify_against_baseline(dataset_name, baseline_name, multiscales_back)
```

### Comparing `ngff_zarr-0.4.5/test/test_itk_image_to_ngff_image.py` & `ngff_zarr-0.4.6/test/test_itk_image_to_ngff_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,83 @@
-from ngff_zarr import itk_image_to_ngff_image
 import itk
 import itkwasm
 import numpy as np
+from ngff_zarr import itk_image_to_ngff_image
 
-from ._data import input_images, test_data_dir
+from ._data import test_data_dir
 
+rng = np.random.default_rng(12345)
 
-def test_2d_itk_image(input_images):
+
+def test_2d_itk_image(input_images):  # noqa: ARG001
     itk_image = itk.imread(test_data_dir / "input" / "cthead1.png")
     ngff_image = itk_image_to_ngff_image(itk_image)
     assert np.array_equal(np.asarray(itk_image), np.asarray(ngff_image.data))
     assert ngff_image.dims == ("y", "x")
     assert ngff_image.scale["x"] == 1.0
     assert ngff_image.scale["y"] == 1.0
     assert ngff_image.translation["x"] == 0.0
     assert ngff_image.translation["y"] == 0.0
     assert ngff_image.name == "image"
-    assert ngff_image.axes_units == None
+    assert ngff_image.axes_units is None
+
 
-def test_2d_rgb_itk_image(input_images):
-    array = np.random.randint(0, 255, size=(224, 224, 3), dtype=np.uint8)
+def test_2d_rgb_itk_image(input_images):  # noqa: ARG001
+    array = rng.integers(0, 255, size=(224, 224, 3), dtype=np.uint8)
     itk_image = itk.image_from_array(array, is_vector=True)
     ngff_image = itk_image_to_ngff_image(itk_image)
     assert np.array_equal(np.asarray(itk_image), array)
     assert np.array_equal(np.asarray(ngff_image.data), array)
     assert ngff_image.dims == ("y", "x", "c")
     assert ngff_image.scale["x"] == 1.0
     assert ngff_image.scale["y"] == 1.0
     assert ngff_image.translation["x"] == 0.0
     assert ngff_image.translation["y"] == 0.0
     assert ngff_image.name == "image"
-    assert ngff_image.axes_units == None
+    assert ngff_image.axes_units is None
 
-def test_2d_itk_vector_image(input_images):
-    array = np.random.rand(224, 224, 3).astype(dtype=np.float32)
+
+def test_2d_itk_vector_image(input_images):  # noqa: ARG001
+    array = rng.random(size=(224, 224, 3), dtype=np.float32)
     itk_image = itk.image_from_array(array, is_vector=True)
     ngff_image = itk_image_to_ngff_image(itk_image)
     assert np.array_equal(itk.array_from_image(itk_image), array)
     assert np.array_equal(np.asarray(ngff_image.data), array)
     assert ngff_image.dims == ("y", "x", "c")
     assert ngff_image.scale["x"] == 1.0
     assert ngff_image.scale["y"] == 1.0
     assert ngff_image.translation["x"] == 0.0
     assert ngff_image.translation["y"] == 0.0
     assert ngff_image.name == "image"
-    assert ngff_image.axes_units == None
+    assert ngff_image.axes_units is None
+
 
-def test_3d_itk_vector_image(input_images):
-    array = np.random.rand(224, 224, 128, 3).astype(dtype=np.float32)
+def test_3d_itk_vector_image(input_images):  # noqa: ARG001
+    array = rng.random(size=(224, 224, 128, 3), dtype=np.float32)
     itk_image = itk.image_from_array(array, is_vector=True)
     ngff_image = itk_image_to_ngff_image(itk_image)
     assert np.array_equal(itk.array_from_image(itk_image), array)
     assert np.array_equal(np.asarray(ngff_image.data), array)
     assert ngff_image.dims == ("z", "y", "x", "c")
     assert ngff_image.scale["x"] == 1.0
     assert ngff_image.scale["y"] == 1.0
     assert ngff_image.scale["z"] == 1.0
     assert ngff_image.translation["x"] == 0.0
     assert ngff_image.translation["y"] == 0.0
     assert ngff_image.translation["z"] == 0.0
     assert ngff_image.name == "image"
-    assert ngff_image.axes_units == None
+    assert ngff_image.axes_units is None
+
 
-def test_2d_itkwasm_image(input_images):
+def test_2d_itkwasm_image(input_images):  # noqa: ARG001
     itk_image = itk.imread(test_data_dir / "input" / "cthead1.png")
     itk_image_dict = itk.dict_from_image(itk_image)
     itkwasm_image = itkwasm.Image(**itk_image_dict)
     ngff_image = itk_image_to_ngff_image(itkwasm_image)
     assert np.array_equal(np.asarray(itk_image), np.asarray(ngff_image.data))
     assert ngff_image.dims == ("y", "x")
     assert ngff_image.scale["x"] == 1.0
     assert ngff_image.scale["y"] == 1.0
     assert ngff_image.translation["x"] == 0.0
     assert ngff_image.translation["y"] == 0.0
     assert ngff_image.name == "image"
-    assert ngff_image.axes_units == None
+    assert ngff_image.axes_units is None
```

### Comparing `ngff_zarr-0.4.5/test/test_memory_usage.py` & `ngff_zarr-0.4.6/test/test_memory_usage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 import dask.array
 import numpy as np
 import zarr
+from ngff_zarr import (
+    from_ngff_zarr,
+    memory_usage,
+    to_multiscales,
+    to_ngff_image,
+    to_ngff_zarr,
+)
+
+rng = np.random.default_rng(12345)
 
-from ngff_zarr import memory_usage, NgffImage, to_ngff_image, to_multiscales, to_ngff_zarr, from_ngff_zarr
 
 def test_memory_usage():
-    arr = np.random.randint(0, 255, size=(4,4,4), dtype=np.uint8)
+    arr = rng.integers(0, 255, size=(4, 4, 4), dtype=np.uint8)
     arr = dask.array.from_array(arr, chunks=2)
     image = to_ngff_image(arr)
     multiscales = to_multiscales(image, scale_factors=[], chunks=2)
     store = zarr.storage.MemoryStore()
     to_ngff_zarr(store, multiscales)
     multiscales = from_ngff_zarr(store)
 
     image = multiscales.images[0]
     arr = image.data
     assert arr.nbytes == 64
     usage = memory_usage(image)
     assert usage == 64
-    usage = memory_usage(image, {'z'})
+    usage = memory_usage(image, {"z"})
     assert usage == 32
 
     arr1 = arr + 1
     assert arr1.nbytes == 64
     image.data = arr1
     usage = memory_usage(image)
     assert usage == 64
-    usage = memory_usage(image, {'z'})
+    usage = memory_usage(image, {"z"})
     assert usage == 32
```

### Comparing `ngff_zarr-0.4.5/test/test_ngff_image_scale_factors.py` & `ngff_zarr-0.4.6/test/test_ngff_image_scale_factors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-from ngff_zarr.to_ngff_image import to_ngff_image
+import numpy as np
 from ngff_zarr.to_multiscales import _ngff_image_scale_factors
+from ngff_zarr.to_ngff_image import to_ngff_image
+
+rng = np.random.default_rng(12345)
 
-import numpy as np
 
 def test_scale_factors_520_520():
-    array = np.random.uniform(high=100.0, size=(520,520)).astype(np.float32)
+    array = rng.random(size=(520, 520), dtype=np.float32) * 100.0
     image = to_ngff_image(array)
     image.data = image.data.rechunk(64)
-    scale_factors = _ngff_image_scale_factors(image, 64, {'x': 64, 'y': 64})
+    scale_factors = _ngff_image_scale_factors(image, 64, {"x": 64, "y": 64})
     assert len(scale_factors) == 3
-    assert scale_factors[2]['x'] == 8
-    assert scale_factors[2]['y'] == 8
+    assert scale_factors[2]["x"] == 8
+    assert scale_factors[2]["y"] == 8
+
 
 def test_scale_factors_520_530():
-    array = np.random.uniform(high=100.0, size=(520,530)).astype(np.float32)
+    array = rng.random(size=(520, 530), dtype=np.float32) * 100.0
     image = to_ngff_image(array)
     image.data = image.data.rechunk(64)
-    scale_factors = _ngff_image_scale_factors(image, 64, {'x': 64, 'y': 64})
+    scale_factors = _ngff_image_scale_factors(image, 64, {"x": 64, "y": 64})
     assert len(scale_factors) == 3
-    assert scale_factors[2]['x'] == 8
-    assert scale_factors[2]['y'] == 8
+    assert scale_factors[2]["x"] == 8
+    assert scale_factors[2]["y"] == 8
```

### Comparing `ngff_zarr-0.4.5/test/test_ngff_image_to_itk_image.py` & `ngff_zarr-0.4.6/test/test_ngff_image_to_itk_image.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,64 @@
-from ngff_zarr import itk_image_to_ngff_image, ngff_image_to_itk_image
 import itk
 import itkwasm
 import numpy as np
+from ngff_zarr import itk_image_to_ngff_image, ngff_image_to_itk_image
+
+from ._data import test_data_dir
 
-from ._data import input_images, test_data_dir
+rng = np.random.default_rng(12345)
 
 
-def test_2d_itk_image(input_images):
+def test_2d_itk_image(input_images):  # noqa: ARG001
     itk_image = itk.imread(test_data_dir / "input" / "cthead1.png")
     ngff_image = itk_image_to_ngff_image(itk_image)
     itk_image_back = ngff_image_to_itk_image(ngff_image, wasm=False)
     diff = itk.comparison_image_filter(itk_image, itk_image_back)
     assert np.sum(np.asarray(diff)) == 0.0
 
-def test_2d_rgb_itk_image(input_images):
-    array = np.random.randint(0, 255, size=(224, 224, 3), dtype=np.uint8)
+
+def test_2d_rgb_itk_image(input_images):  # noqa: ARG001
+    array = rng.integers(0, 255, size=(224, 224, 3), dtype=np.uint8)
     itk_image = itk.image_from_array(array, is_vector=True)
-    ngff_image = itk_image_to_ngff_image(itk_image)
+    ngff_image = itk_image_to_ngff_image(itk_image)  # noqa: F841
     # Requires fixes for itk
     # itk_image_back = ngff_image_to_itk_image(ngff_image, wasm=False)
     # diff = itk.comparison_image_filter(itk_image, itk_image_back)
     # assert np.sum(np.asarray(diff)) == 0.0
 
-def test_2d_itk_vector_image(input_images):
-    array = np.random.rand(224, 224, 3).astype(dtype=np.float32)
+
+def test_2d_itk_vector_image(input_images):  # noqa: ARG001
+    array = rng.random(size=(224, 224, 3), dtype=np.float32)
     itk_image = itk.image_from_array(array, is_vector=True)
-    ngff_image = itk_image_to_ngff_image(itk_image)
+    ngff_image = itk_image_to_ngff_image(itk_image)  # noqa: F841
     # Requires fixes for itk
     # itk_image_back = ngff_image_to_itk_image(ngff_image, wasm=False)
     # assert np.array_equal(itk.array_from_image(itk_image), itk.array_from_image(itk_image_back))
 
-def test_3d_itk_image(input_images):
-    array = np.random.randint(0, 255, size=(32, 32, 32), dtype=np.uint8)
+
+def test_3d_itk_image(input_images):  # noqa: ARG001
+    array = rng.integers(0, 255, size=(32, 32, 32), dtype=np.uint8)
     itk_image = itk.image_from_array(array, is_vector=False)
     ngff_image = itk_image_to_ngff_image(itk_image)
     itk_image_back = ngff_image_to_itk_image(ngff_image, wasm=False)
     diff = itk.comparison_image_filter(itk_image, itk_image_back)
     assert np.sum(np.asarray(diff)) == 0.0
 
-def test_3d_itk_vector_image(input_images):
-    array = np.random.rand(224, 224, 128, 3).astype(dtype=np.float32)
+
+def test_3d_itk_vector_image(input_images):  # noqa: ARG001
+    array = rng.random(size=(224, 224, 128, 3), dtype=np.float32)
     itk_image = itk.image_from_array(array, is_vector=True)
-    ngff_image = itk_image_to_ngff_image(itk_image)
+    ngff_image = itk_image_to_ngff_image(itk_image)  # noqa: F841
     # Requires fixes for itk
     # itk_image_back = ngff_image_to_itk_image(ngff_image, wasm=False)
     # assert np.array_equal(itk.array_from_image(itk_image), itk.array_from_image(itk_image_back))
 
-def test_2d_itkwasm_image(input_images):
+
+def test_2d_itkwasm_image(input_images):  # noqa: ARG001
     itk_image = itk.imread(test_data_dir / "input" / "cthead1.png")
     itk_image_dict = itk.dict_from_image(itk_image)
     itkwasm_image = itkwasm.Image(**itk_image_dict)
     ngff_image = itk_image_to_ngff_image(itkwasm_image)
     itkwasm_image_back = ngff_image_to_itk_image(ngff_image)
-    assert np.array_equal(np.asarray(itkwasm_image.data), np.asarray(itkwasm_image_back.data))
+    assert np.array_equal(
+        np.asarray(itkwasm_image.data), np.asarray(itkwasm_image_back.data)
+    )
```

### Comparing `ngff_zarr-0.4.5/test/test_task_count.py` & `ngff_zarr-0.4.6/test/test_task_count.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 import dask.array
 import numpy as np
 import zarr
+from ngff_zarr import (
+    from_ngff_zarr,
+    task_count,
+    to_multiscales,
+    to_ngff_image,
+    to_ngff_zarr,
+)
+
+rng = np.random.default_rng(12345)
 
-from ngff_zarr import NgffImage, to_ngff_image, to_multiscales, to_ngff_zarr, from_ngff_zarr, task_count
 
 def test_memory_usage():
-    arr = np.random.randint(0, 255, size=(4,4,4), dtype=np.uint8)
+    arr = rng.integers(0, 255, size=(4, 4, 4), dtype=np.uint8)
     arr = dask.array.from_array(arr, chunks=2)
     image = to_ngff_image(arr)
     multiscales = to_multiscales(image, scale_factors=[], chunks=2)
     store = zarr.storage.MemoryStore()
     to_ngff_zarr(store, multiscales)
     multiscales = from_ngff_zarr(store)
 
     image = multiscales.images[0]
     arr = image.data
     assert len(arr.dask) == 9
     count = task_count(image)
     assert count == 9
-    count = task_count(image, {'z'})
+    count = task_count(image, {"z"})
     assert count == 13
 
     arr1 = arr + 1
     assert len(arr1.dask) == 17
     image.data = arr1
     count = task_count(image)
     assert count == 17
-    count = task_count(image, {'z'})
+    count = task_count(image, {"z"})
     assert count == 21
```

### Comparing `ngff_zarr-0.4.5/test/test_to_ngff_zarr_dask_image.py` & `ngff_zarr-0.4.6/test/test_to_ngff_zarr_itk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-from ngff_zarr import Methods, to_ngff_zarr, to_multiscales
-from zarr.storage import MemoryStore
+from ngff_zarr import Methods, to_multiscales
 
-from ._data import input_images, store_new_multiscales, verify_against_baseline
+from ._data import verify_against_baseline
 
 
-def test_gaussian_isotropic_scale_factors(input_images):
+def test_bin_shrink_isotropic_scale_factors(input_images):
     dataset_name = "cthead1"
     image = input_images[dataset_name]
-    baseline_name = "2_4/DASK_IMAGE_GAUSSIAN.zarr"
-    multiscales = to_multiscales(image, [2, 4], method=Methods.DASK_IMAGE_GAUSSIAN)
+    baseline_name = "2_4/ITK_BIN_SHRINK.zarr"
+    multiscales = to_multiscales(image, [2, 4], method=Methods.ITK_BIN_SHRINK)
     # store_new_multiscales(dataset_name, baseline_name, multiscales)
     verify_against_baseline(dataset_name, baseline_name, multiscales)
 
-    baseline_name = "auto/DASK_IMAGE_GAUSSIAN.zarr"
-    multiscales = to_multiscales(image, method=Methods.DASK_IMAGE_GAUSSIAN)
+    baseline_name = "auto/ITK_BIN_SHRINK.zarr"
+    multiscales = to_multiscales(image, method=Methods.ITK_BIN_SHRINK)
     verify_against_baseline(dataset_name, baseline_name, multiscales)
 
-    dataset_name = "brain_two_components"
+
+def test_gaussian_isotropic_scale_factors(input_images):
+    dataset_name = "cthead1"
     image = input_images[dataset_name]
-    baseline_name = "2_4/DASK_IMAGE_GAUSSIAN.zarr"
-    multiscales = to_multiscales(image, [2, 4], method=Methods.DASK_IMAGE_GAUSSIAN)
+    baseline_name = "2_4/ITK_GAUSSIAN.zarr"
+    multiscales = to_multiscales(image, [2, 4], method=Methods.ITK_GAUSSIAN)
     verify_against_baseline(dataset_name, baseline_name, multiscales)
 
+    baseline_name = "auto/ITK_GAUSSIAN.zarr"
+    multiscales = to_multiscales(image, method=Methods.ITK_GAUSSIAN)
+    verify_against_baseline(dataset_name, baseline_name, multiscales)
+
+
 #     dataset_name = "cthead1"
 #     image = input_images[dataset_name]
 #     baseline_name = "2_3/DASK_IMAGE_GAUSSIAN"
 #     multiscale = to_multiscale(image, [2, 3], method=Methods.DASK_IMAGE_GAUSSIAN)
 #     verify_against_baseline(dataset_name, baseline_name, multiscale)
 
 #     dataset_name = "small_head"
```

### Comparing `ngff_zarr-0.4.5/test/test_to_ngff_zarr_itk.py` & `ngff_zarr-0.4.6/test/test_to_ngff_zarr_dask_image.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-from ngff_zarr import Methods, to_ngff_zarr, to_multiscales
-from zarr.storage import MemoryStore
+from ngff_zarr import Methods, to_multiscales
 
-from ._data import input_images, store_new_multiscales, verify_against_baseline
+from ._data import verify_against_baseline
 
 
-def test_bin_shrink_isotropic_scale_factors(input_images):
+def test_gaussian_isotropic_scale_factors(input_images):
     dataset_name = "cthead1"
     image = input_images[dataset_name]
-    baseline_name = "2_4/ITK_BIN_SHRINK.zarr"
-    multiscales = to_multiscales(image, [2, 4], method=Methods.ITK_BIN_SHRINK)
+    baseline_name = "2_4/DASK_IMAGE_GAUSSIAN.zarr"
+    multiscales = to_multiscales(image, [2, 4], method=Methods.DASK_IMAGE_GAUSSIAN)
     # store_new_multiscales(dataset_name, baseline_name, multiscales)
     verify_against_baseline(dataset_name, baseline_name, multiscales)
 
-    baseline_name = "auto/ITK_BIN_SHRINK.zarr"
-    multiscales = to_multiscales(image, method=Methods.ITK_BIN_SHRINK)
+    baseline_name = "auto/DASK_IMAGE_GAUSSIAN.zarr"
+    multiscales = to_multiscales(image, method=Methods.DASK_IMAGE_GAUSSIAN)
     verify_against_baseline(dataset_name, baseline_name, multiscales)
 
-def test_gaussian_isotropic_scale_factors(input_images):
-    dataset_name = "cthead1"
+    dataset_name = "brain_two_components"
     image = input_images[dataset_name]
-    baseline_name = "2_4/ITK_GAUSSIAN.zarr"
-    multiscales = to_multiscales(image, [2, 4], method=Methods.ITK_GAUSSIAN)
+    baseline_name = "2_4/DASK_IMAGE_GAUSSIAN.zarr"
+    multiscales = to_multiscales(image, [2, 4], method=Methods.DASK_IMAGE_GAUSSIAN)
     verify_against_baseline(dataset_name, baseline_name, multiscales)
 
-    baseline_name = "auto/ITK_GAUSSIAN.zarr"
-    multiscales = to_multiscales(image, method=Methods.ITK_GAUSSIAN)
-    verify_against_baseline(dataset_name, baseline_name, multiscales)
 
 #     dataset_name = "cthead1"
 #     image = input_images[dataset_name]
 #     baseline_name = "2_3/DASK_IMAGE_GAUSSIAN"
 #     multiscale = to_multiscale(image, [2, 3], method=Methods.DASK_IMAGE_GAUSSIAN)
 #     verify_against_baseline(dataset_name, baseline_name, multiscale)
```

### Comparing `ngff_zarr-0.4.5/LICENSE.txt` & `ngff_zarr-0.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.5/README.md` & `ngff_zarr-0.4.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,42 +2,46 @@
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ngff-zarr.svg)](https://pypi.org/project/ngff-zarr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ngff-zarr.svg)](https://pypi.org/project/ngff-zarr)
 [![Test](https://github.com/thewtex/ngff-zarr/actions/workflows/test.yml/badge.svg)](https://github.com/thewtex/ngff-zarr/actions/workflows/test.yml)
 [![DOI](https://zenodo.org/badge/541840158.svg)](https://zenodo.org/badge/latestdoi/541840158)
 [![Documentation Status](https://readthedocs.org/projects/ngff-zarr/badge/?version=latest)](https://ngff-zarr.readthedocs.io/en/latest/?badge=latest)
 
------
+---
 
-A lean and kind Open Microscopy Environment (OME) Next Generation File Format (NGFF) Zarr implementation.
+A lean and kind Open Microscopy Environment (OME) Next Generation File Format
+(NGFF) Zarr implementation.
 
 ## Features
 
 - Minimal dependencies
 - Work with arbitrary Zarr store types
 - Lazy, parallel, and web ready -- no local filesystem required
 - Process extremely large datasets
 - Multiple downscaling methods
 - Supports Python>=3.7
-- Implements version 0.4 of the [OME-Zarr
-NGFF specification](https://github.com/ome/ngff)
+- Implements version 0.4 of the
+  [OME-Zarr NGFF specification](https://github.com/ome/ngff)
 
 ## Installation
 
 To install the command line interface (CLI):
 
 ```console
 pip install 'ngff-zarr[cli]'
 ```
 
 ## Documentation
 
-More information an command line usage, the Python API, library features, and how to contribute can be found in [our documentation](https://ngff-zarr.readthedocs.io/).
+More information an command line usage, the Python API, library features, and
+how to contribute can be found in
+[our documentation](https://ngff-zarr.readthedocs.io/).
 
 ## See also
 
 - [ome-zarr-py](https://github.com/ome/ome-zarr-py)
 - [multiscale-spatial-image](https://github.com/spatial-image/multiscale-spatial-image)
 
 ## License
 
-`ngff-zarr` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`ngff-zarr` is distributed under the terms of the
+[MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `ngff_zarr-0.4.5/PKG-INFO` & `ngff_zarr-0.4.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: ngff-zarr
-Version: 0.4.5
+Version: 0.4.6
+Summary: A lean and kind Open Microscopy Environment (OME) Next Generation File Format (NGFF) Zarr implementation.
 Project-URL: Documentation, https://github.com/thewtex/ngff-zarr#readme
 Project-URL: Issues, https://github.com/thewtex/ngff-zarr/issues
 Project-URL: Source, https://github.com/thewtex/ngff-zarr
+Project-URL: Changelog, https://github.com/thewtex/ngff-zarr/releases
 Author-email: Matt McCormick <matt.mccormick@kitware.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Requires-Dist: dask[array]
 Requires-Dist: numpy
 Requires-Dist: platformdirs
 Requires-Dist: psutil; sys_platform != 'emscripten'
 Requires-Dist: rich
 Requires-Dist: typing-extensions
@@ -37,54 +44,59 @@
 Provides-Extra: itk
 Requires-Dist: itk-filtering>=5.3.0; extra == 'itk'
 Provides-Extra: test
 Requires-Dist: itk-filtering>=5.3.0; extra == 'test'
 Requires-Dist: itk-io>=5.3.0; extra == 'test'
 Requires-Dist: itkwasm; extra == 'test'
 Requires-Dist: pooch; extra == 'test'
-Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pre-commit; extra == 'test'
+Requires-Dist: pytest>=6; extra == 'test'
 Requires-Dist: tifffile; extra == 'test'
 Description-Content-Type: text/markdown
 
 # ngff-zarr
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ngff-zarr.svg)](https://pypi.org/project/ngff-zarr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ngff-zarr.svg)](https://pypi.org/project/ngff-zarr)
 [![Test](https://github.com/thewtex/ngff-zarr/actions/workflows/test.yml/badge.svg)](https://github.com/thewtex/ngff-zarr/actions/workflows/test.yml)
 [![DOI](https://zenodo.org/badge/541840158.svg)](https://zenodo.org/badge/latestdoi/541840158)
 [![Documentation Status](https://readthedocs.org/projects/ngff-zarr/badge/?version=latest)](https://ngff-zarr.readthedocs.io/en/latest/?badge=latest)
 
------
+---
 
-A lean and kind Open Microscopy Environment (OME) Next Generation File Format (NGFF) Zarr implementation.
+A lean and kind Open Microscopy Environment (OME) Next Generation File Format
+(NGFF) Zarr implementation.
 
 ## Features
 
 - Minimal dependencies
 - Work with arbitrary Zarr store types
 - Lazy, parallel, and web ready -- no local filesystem required
 - Process extremely large datasets
 - Multiple downscaling methods
 - Supports Python>=3.7
-- Implements version 0.4 of the [OME-Zarr
-NGFF specification](https://github.com/ome/ngff)
+- Implements version 0.4 of the
+  [OME-Zarr NGFF specification](https://github.com/ome/ngff)
 
 ## Installation
 
 To install the command line interface (CLI):
 
 ```console
 pip install 'ngff-zarr[cli]'
 ```
 
 ## Documentation
 
-More information an command line usage, the Python API, library features, and how to contribute can be found in [our documentation](https://ngff-zarr.readthedocs.io/).
+More information an command line usage, the Python API, library features, and
+how to contribute can be found in
+[our documentation](https://ngff-zarr.readthedocs.io/).
 
 ## See also
 
 - [ome-zarr-py](https://github.com/ome/ome-zarr-py)
 - [multiscale-spatial-image](https://github.com/spatial-image/multiscale-spatial-image)
 
 ## License
 
-`ngff-zarr` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`ngff-zarr` is distributed under the terms of the
+[MIT](https://spdx.org/licenses/MIT.html) license.
```

