# Comparing `tmp/iohub-0.1.0.dev3.tar.gz` & `tmp/iohub-0.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iohub-0.1.0.dev3.tar", last modified: Fri Apr 14 23:56:56 2023, max compression
+gzip compressed data, was "iohub-0.1.0.dev4.tar", last modified: Wed Aug  2 17:26:13 2023, max compression
```

## Comparing `iohub-0.1.0.dev3.tar` & `iohub-0.1.0.dev4.tar`

### file list

```diff
@@ -1,80 +1,95 @@
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.688852 iohub-0.1.0.dev3/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      236 2023-01-19 20:11:04.000000 iohub-0.1.0.dev3/.git-blame-ignore-revs
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.675019 iohub-0.1.0.dev3/.github/
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.678495 iohub-0.1.0.dev3/.github/workflows/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     1076 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/.github/workflows/docs.yml
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     2458 2023-04-13 18:36:42.000000 iohub-0.1.0.dev3/.github/workflows/pr.yml
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      686 2023-04-14 16:32:14.000000 iohub-0.1.0.dev3/.github/workflows/test.yml
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     2017 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/.gitignore
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     4644 2023-03-10 22:18:16.000000 iohub-0.1.0.dev3/CONTRIBUTING.md
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     1530 2022-11-23 00:26:00.000000 iohub-0.1.0.dev3/LICENSE
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     4800 2023-04-14 23:56:56.688959 iohub-0.1.0.dev3/PKG-INFO
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     3686 2023-04-14 20:16:19.000000 iohub-0.1.0.dev3/README.md
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.678694 iohub-0.1.0.dev3/docs/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      895 2023-04-14 22:51:34.000000 iohub-0.1.0.dev3/docs/Makefile
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.679054 iohub-0.1.0.dev3/docs/source/
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.680412 iohub-0.1.0.dev3/docs/source/api/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      263 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/docs/source/api/mm_converter.rst
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      178 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/docs/source/api/mm_ometiff_reader.rst
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      127 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/docs/source/api/mm_reader.rst
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      180 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/docs/source/api/mm_sequence_reader.rst
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      139 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/docs/source/api/ndtiff.rst
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      336 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/docs/source/api/ngff.rst
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      138 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/docs/source/api/upti.rst
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     5491 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/docs/source/conf.py
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.680637 iohub-0.1.0.dev3/docs/source/contact_us/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      584 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/docs/source/contact_us/github.rst
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.681056 iohub-0.1.0.dev3/docs/source/getting_started/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      136 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/docs/source/getting_started/install.rst
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      964 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/docs/source/getting_started/why.rst
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     1312 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/docs/source/index.rst
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.681780 iohub-0.1.0.dev3/examples/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     1277 2023-03-14 18:23:48.000000 iohub-0.1.0.dev3/examples/large_array_ome_zarr.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     1923 2023-03-14 18:19:10.000000 iohub-0.1.0.dev3/examples/multi_fov_hcs_ome_zarr.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     2344 2023-03-14 18:19:10.000000 iohub-0.1.0.dev3/examples/single_fov_ome_zarr.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     1282 2023-03-11 06:11:41.000000 iohub-0.1.0.dev3/examples/tiled_ome_zarr.py
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.684471 iohub-0.1.0.dev3/iohub/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      254 2023-03-28 20:30:52.000000 iohub-0.1.0.dev3/iohub/__init__.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      173 2023-04-14 23:56:56.000000 iohub-0.1.0.dev3/iohub/_version.py
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.686108 iohub-0.1.0.dev3/iohub/cli/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)        0 2023-02-13 22:14:11.000000 iohub-0.1.0.dev3/iohub/cli/__init__.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     2131 2023-03-28 20:30:52.000000 iohub-0.1.0.dev3/iohub/cli/cli.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)    12705 2023-04-05 21:24:46.000000 iohub-0.1.0.dev3/iohub/convert.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     3323 2023-04-05 04:05:16.000000 iohub-0.1.0.dev3/iohub/display_utils.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)    11894 2023-04-13 18:25:43.000000 iohub-0.1.0.dev3/iohub/multipagetiff.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     6289 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/iohub/ndtiff.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)    46532 2023-04-14 23:54:02.000000 iohub-0.1.0.dev3/iohub/ngff.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)    11920 2023-04-05 04:05:16.000000 iohub-0.1.0.dev3/iohub/ngff_meta.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)    10069 2023-04-05 21:24:46.000000 iohub-0.1.0.dev3/iohub/reader.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     2737 2023-04-14 16:32:14.000000 iohub-0.1.0.dev3/iohub/reader_base.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)    14147 2023-03-24 17:48:02.000000 iohub-0.1.0.dev3/iohub/singlepagetiff.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     6646 2023-04-05 21:24:46.000000 iohub-0.1.0.dev3/iohub/upti.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)    10611 2023-03-31 16:46:58.000000 iohub-0.1.0.dev3/iohub/zarrfile.py
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.685759 iohub-0.1.0.dev3/iohub.egg-info/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     4800 2023-04-14 23:56:56.000000 iohub-0.1.0.dev3/iohub.egg-info/PKG-INFO
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     1513 2023-04-14 23:56:56.000000 iohub-0.1.0.dev3/iohub.egg-info/SOURCES.txt
--rw-r--r--   0 ziwen.liu   (503) staff       (20)        1 2023-04-14 23:56:56.000000 iohub-0.1.0.dev3/iohub.egg-info/dependency_links.txt
--rw-r--r--   0 ziwen.liu   (503) staff       (20)       44 2023-04-14 23:56:56.000000 iohub-0.1.0.dev3/iohub.egg-info/entry_points.txt
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      340 2023-04-14 23:56:56.000000 iohub-0.1.0.dev3/iohub.egg-info/requires.txt
--rw-r--r--   0 ziwen.liu   (503) staff       (20)        6 2023-04-14 23:56:56.000000 iohub-0.1.0.dev3/iohub.egg-info/top_level.txt
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      241 2022-11-28 23:06:14.000000 iohub-0.1.0.dev3/pyproject.toml
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     1488 2023-04-14 23:56:56.689375 iohub-0.1.0.dev3/setup.cfg
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      105 2023-02-13 22:14:11.000000 iohub-0.1.0.dev3/setup.py
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.686888 iohub-0.1.0.dev3/tests/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)        0 2023-03-28 20:30:52.000000 iohub-0.1.0.dev3/tests/__init__.py
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.687258 iohub-0.1.0.dev3/tests/cli/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)        0 2023-03-14 18:20:52.000000 iohub-0.1.0.dev3/tests/cli/__init__.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     2872 2023-03-28 20:30:52.000000 iohub-0.1.0.dev3/tests/cli/test_cli.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     6255 2023-03-06 18:43:50.000000 iohub-0.1.0.dev3/tests/conftest.py
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.687594 iohub-0.1.0.dev3/tests/ngff/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)        0 2023-02-15 04:46:37.000000 iohub-0.1.0.dev3/tests/ngff/__init__.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)    18044 2023-03-28 20:30:52.000000 iohub-0.1.0.dev3/tests/ngff/test_ngff.py
-drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-04-14 23:56:56.688693 iohub-0.1.0.dev3/tests/reader/
--rw-r--r--   0 ziwen.liu   (503) staff       (20)        0 2022-11-23 00:24:00.000000 iohub-0.1.0.dev3/tests/reader/__init__.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     5022 2023-02-15 04:46:37.000000 iohub-0.1.0.dev3/tests/reader/test_multipagetiff.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     2128 2023-03-10 22:18:16.000000 iohub-0.1.0.dev3/tests/reader/test_pycromanager.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)    11402 2023-03-28 20:30:52.000000 iohub-0.1.0.dev3/tests/reader/test_reader.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     5136 2023-02-15 04:46:37.000000 iohub-0.1.0.dev3/tests/reader/test_singlepagetiff.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     2761 2023-03-28 20:30:52.000000 iohub-0.1.0.dev3/tests/reader/test_zarrfile.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)     4503 2023-03-28 20:30:52.000000 iohub-0.1.0.dev3/tests/test_converter.py
--rw-r--r--   0 ziwen.liu   (503) staff       (20)      699 2023-04-05 04:05:16.000000 iohub-0.1.0.dev3/tests/test_display_utils.py
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.055181 iohub-0.1.0.dev4/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      237 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/.git-blame-ignore-revs
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.037625 iohub-0.1.0.dev4/.github/
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.041887 iohub-0.1.0.dev4/.github/workflows/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     1429 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/.github/workflows/docs.yml
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     2971 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/.github/workflows/pr.yml
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      686 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/.github/workflows/test.yml
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     2037 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/.gitignore
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      919 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/.pre-commit-config.yaml
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     5586 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/CONTRIBUTING.md
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     1530 2022-11-23 00:26:00.000000 iohub-0.1.0.dev4/LICENSE
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     4839 2023-08-02 17:26:13.055301 iohub-0.1.0.dev4/PKG-INFO
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     3710 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/README.md
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.042348 iohub-0.1.0.dev4/docs/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     1150 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/docs/Makefile
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.043641 iohub-0.1.0.dev4/docs/examples/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)       76 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/docs/examples/README.rst
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     2040 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/docs/examples/run_coordinate_transform.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     1326 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/docs/examples/run_large_array_ome_zarr.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     1959 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/docs/examples/run_multi_fov_hcs_ome_zarr.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     2367 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/docs/examples/run_single_fov_ome_zarr.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     1510 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/docs/examples/run_tiled_ome_zarr.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     1280 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/docs/examples/run_view_clearcontrol_dataset.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      241 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/docs/gh-pages-redirect.html
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.044534 iohub-0.1.0.dev4/docs/source/
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.044728 iohub-0.1.0.dev4/docs/source/_static/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)       78 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/docs/source/_static/switcher.json
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.046297 iohub-0.1.0.dev4/docs/source/api/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      181 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/docs/source/api/clearcontrol.rst
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      262 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/docs/source/api/mm_converter.rst
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      164 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/docs/source/api/mm_ometiff_reader.rst
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      119 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/docs/source/api/mm_reader.rst
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      166 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/docs/source/api/mm_sequence_reader.rst
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      124 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/docs/source/api/ndtiff.rst
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      457 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/docs/source/api/ngff.rst
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      124 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/docs/source/api/upti.rst
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      261 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/docs/source/api.rst
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     6768 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/docs/source/conf.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      542 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/docs/source/contact_us.rst
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     1455 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/docs/source/getting_started.rst
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      745 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/docs/source/index.rst
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.050397 iohub-0.1.0.dev4/iohub/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      254 2023-07-27 17:29:16.000000 iohub-0.1.0.dev4/iohub/__init__.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      173 2023-08-02 17:26:12.000000 iohub-0.1.0.dev4/iohub/_version.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)    14340 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/iohub/clearcontrol.py
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.051935 iohub-0.1.0.dev4/iohub/cli/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)        0 2023-02-13 22:14:11.000000 iohub-0.1.0.dev4/iohub/cli/__init__.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     2516 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/iohub/cli/cli.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)    16014 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/iohub/convert.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     3429 2023-08-02 16:49:29.000000 iohub-0.1.0.dev4/iohub/display_utils.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     6173 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/iohub/fov.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)    13589 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/iohub/multipagetiff.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     6180 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/iohub/ndtiff.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)    52803 2023-08-02 16:49:29.000000 iohub-0.1.0.dev4/iohub/ngff.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)    11871 2023-07-12 00:40:30.000000 iohub-0.1.0.dev4/iohub/ngff_meta.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)    10138 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/iohub/reader.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     2724 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/iohub/reader_base.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)    14147 2023-05-03 18:14:50.000000 iohub-0.1.0.dev4/iohub/singlepagetiff.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     6646 2023-05-03 18:14:50.000000 iohub-0.1.0.dev4/iohub/upti.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)    10611 2023-05-03 18:14:50.000000 iohub-0.1.0.dev4/iohub/zarrfile.py
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.051569 iohub-0.1.0.dev4/iohub.egg-info/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     4839 2023-08-02 17:26:12.000000 iohub-0.1.0.dev4/iohub.egg-info/PKG-INFO
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     1904 2023-08-02 17:26:13.000000 iohub-0.1.0.dev4/iohub.egg-info/SOURCES.txt
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)        1 2023-08-02 17:26:12.000000 iohub-0.1.0.dev4/iohub.egg-info/dependency_links.txt
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)       44 2023-08-02 17:26:12.000000 iohub-0.1.0.dev4/iohub.egg-info/entry_points.txt
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      416 2023-08-02 17:26:12.000000 iohub-0.1.0.dev4/iohub.egg-info/requires.txt
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)        6 2023-08-02 17:26:12.000000 iohub-0.1.0.dev4/iohub.egg-info/top_level.txt
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      289 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/pyproject.toml
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     1585 2023-08-02 17:26:13.055700 iohub-0.1.0.dev4/setup.cfg
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)       99 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/setup.py
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.052663 iohub-0.1.0.dev4/tests/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)        0 2023-03-28 20:30:52.000000 iohub-0.1.0.dev4/tests/__init__.py
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.052819 iohub-0.1.0.dev4/tests/clearcontrol/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     2183 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/tests/clearcontrol/test_clearcontrol.py
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.053123 iohub-0.1.0.dev4/tests/cli/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)        0 2023-05-03 18:14:50.000000 iohub-0.1.0.dev4/tests/cli/__init__.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     3264 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/tests/cli/test_cli.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     6255 2023-08-02 16:49:29.000000 iohub-0.1.0.dev4/tests/conftest.py
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.053310 iohub-0.1.0.dev4/tests/fov/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     1971 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/tests/fov/test_fov.py
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.053673 iohub-0.1.0.dev4/tests/ngff/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)        0 2023-02-15 04:46:37.000000 iohub-0.1.0.dev4/tests/ngff/__init__.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)    22754 2023-08-02 16:49:29.000000 iohub-0.1.0.dev4/tests/ngff/test_ngff.py
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.054002 iohub-0.1.0.dev4/tests/pyramid/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)        0 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/tests/pyramid/__init__.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     2195 2023-06-22 22:22:31.000000 iohub-0.1.0.dev4/tests/pyramid/test_pyramid.py
+drwxr-xr-x   0 ziwen.liu   (503) staff       (20)        0 2023-08-02 17:26:13.055036 iohub-0.1.0.dev4/tests/reader/
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)        0 2022-11-23 00:24:00.000000 iohub-0.1.0.dev4/tests/reader/__init__.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     5022 2023-02-15 04:46:37.000000 iohub-0.1.0.dev4/tests/reader/test_multipagetiff.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     2128 2023-05-03 18:14:50.000000 iohub-0.1.0.dev4/tests/reader/test_pycromanager.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)    11402 2023-05-03 18:14:50.000000 iohub-0.1.0.dev4/tests/reader/test_reader.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     5136 2023-02-15 04:46:37.000000 iohub-0.1.0.dev4/tests/reader/test_singlepagetiff.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     2761 2023-05-03 18:14:50.000000 iohub-0.1.0.dev4/tests/reader/test_zarrfile.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)     6764 2023-08-02 16:49:33.000000 iohub-0.1.0.dev4/tests/test_converter.py
+-rw-r--r--   0 ziwen.liu   (503) staff       (20)      819 2023-08-02 16:49:29.000000 iohub-0.1.0.dev4/tests/test_display_utils.py
```

### Comparing `iohub-0.1.0.dev3/.github/workflows/pr.yml` & `iohub-0.1.0.dev4/.github/workflows/pr.yml`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 jobs:
   style:
     name: Style Check
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: [ '3.10' ]
+        python-version: ["3.10"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
@@ -34,15 +34,15 @@
 
   lint:
     name: Lint Check
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: [ '3.10' ]
+        python-version: ["3.10"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
@@ -57,15 +57,15 @@
 
   isort:
     name: isort Check
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: [ '3.10' ]
+        python-version: ["3.10"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
@@ -73,31 +73,51 @@
         run: |
           python -m pip install --upgrade pip
           pip install isort
       - name: Check code with isort
         run: |
           isort --check iohub
 
-
   tests:
     needs: [style, lint, isort]
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.9', '3.10', '3.11']
+        python-version: ["3.9", "3.10", "3.11"]
 
     steps:
-    - uses: actions/checkout@v3
+      - uses: actions/checkout@v3
+
+      - uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install ".[dev]"
 
-    - uses: actions/setup-python@v4
-      with:
-        python-version: ${{ matrix.python-version }}
-
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install ".[dev]"
-
-    - name: Test with pytest
-      run: |
-        pytest -v
-        pytest --cov=./ --cov-report=xml
+      - name: Test with pytest
+        run: |
+          pytest -v --cov=./ --cov-report=xml
+
+  # this checks that docs build and examples run
+  # but does not deploy to GH Pages
+  docs:
+    needs: [style, lint, isort]
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+
+      - uses: actions/setup-python@v4
+        with:
+          python-version: "3.10"
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install ".[doc]"
+
+      - name: Test docs build
+        working-directory: ./docs
+        run: |
+          make build
```

### Comparing `iohub-0.1.0.dev3/.github/workflows/test.yml` & `iohub-0.1.0.dev4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `iohub-0.1.0.dev3/.gitignore` & `iohub-0.1.0.dev4/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Binary image files.
 *.tif[f]
 *.jp[e]g
 *.zar[r]
-*.json
 
 # pycharm IDE
 .idea
 .DS_Store
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
@@ -77,14 +76,15 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+docs/source/auto_examples/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `iohub-0.1.0.dev3/CONTRIBUTING.md` & `iohub-0.1.0.dev4/CONTRIBUTING.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ## Getting started
 
 Please read the [README](./README.md) for an overview of the project,
 and how you can install and use the package.
 
 ## Issues
 
-We use [issues](https://github.com/czbiohub/iohub/issues) to track
+We use [issues](https://github.com/czbiohub-sf/iohub/issues) to track
 bug reports, feature requests, and provide user support.
 
 Before opening a new issue, please first search existing issues (including closed ones),
 to see if there is an existing discussion about it.
 
 ### Bug report
 
@@ -44,27 +44,27 @@
 - (Optional) what are the alternatives?
 
 ### Prioritization
 
 As is the case with any software project, possible improvements vastly out number the community's capacity.
 We use releases as a reference to focus the effort on near-term priorities.
 PRs within the scope of the next release will receive more attention.
-A list of planned release milestones can be found [here](https://github.com/czbiohub/iohub/milestones).
+A list of planned release milestones can be found [here](https://github.com/czbiohub-sf/iohub/milestones).
 
 ### Documentation change
 
 If you find that any documentation in this project is incomplete, inaccurate, or ambiguous,
 please open an issue.
 We welcome contributions to the documentation from users,
 particularly user guides that we can collaboratively edit.
 
 ## Making changes
 
 Any change made to the `main` branch or release maintenance branches
-need to be proposed in a [pull request](https://github.com/czbiohub/iohub/pulls) (PR).
+need to be proposed in a [pull request](https://github.com/czbiohub-sf/iohub/pulls) (PR).
 
 If there is an issue that can be addressed by the PR, please reference it.
 
 If there is not a relevant issue, please either open an issue first,
 or describe the bug fixed or feature implemented in the PR.
 
 ### Setting up development environment
@@ -81,44 +81,58 @@
 ```
 
 If you have push permission to the repository,
 clone the repository (the code blocks below are shell commands):
 
 ```sh
 cd # to the directory you want to work in
-git clone https://github.com/czbiohub/iohub.git
+git clone https://github.com/czbiohub-sf/iohub.git
 ```
 
 Otherwise, you can follow [these instructions](https://docs.github.com/en/get-started/quickstart/fork-a-repo)
-to [fork](https://github.com/czbiohub/iohub/fork) the repository.
+to [fork](https://github.com/czbiohub-sf/iohub/fork) the repository.
 
 Then install the package in editable mode with the development dependencies:
 
 ```sh
 cd iohub/ # or the renamed project root directory
 pip install -e ".[dev]"
 ```
 
 Then make the changes and [track them with Git](https://docs.github.com/en/get-started/using-git/about-git#example-contribute-to-an-existing-repository).
 
+### Developing documentation
 
-### Building documentation locally
+#### Building the HTML version locally
 
 Inside `/docs` folder
 
 ```shell
 pip install "/PATH/TO/iohub[doc]"
 make clean && make build
 ```
 
 Generated HTML documentation can be found in
 the ``build/html`` directory. Open ``build/html/index.html`` to view the home
 page for the documentation.
 
+#### Writing examples
 
+Example scripts in the `docs/examples` directory
+are automatically compiled to RST with `sphinx-gallery`
+in the `docs/source/auto_examples` directory.
+Files that start with `run_` in the file name
+are executed during the build,
+and output (stdout, matplotlib plot) are rendered in HTML.
+
+They can also be executed as plain Python scripts
+or interactive code blocks in some IDEs (VS Code, PyCharm, Spyder etc.).
+
+See the syntax documentation
+[here](https://sphinx-gallery.github.io/stable/syntax.html).
 
 ### Testing
 
 If you made code changes, make sure that there are also tests for them!
 Local test runs and coverage check can be invoked by:
 
 ```sh
@@ -129,11 +143,16 @@
 `iohub` uses [Hypothesis](https://hypothesis.readthedocs.io/en/latest/index.html)
 together with [pytest](https://docs.pytest.org/).
 See [this paper](https://conference.scipy.org/proceedings/scipy2020/zac_hatfield-dodds.html)
 for how this can reveal more bugs.
 
 ### Code style
 
-We use [black](https://black.readthedocs.io/en/stable/) to format our code.
-Black installed with `iohub` should automatically use the [settings](./pyproject.toml) in the repository.
+We use [pre-commit](https://pre-commit.com/) to sort imports with [isort](https://github.com/PyCQA/isort), format code with [black](https://black.readthedocs.io/en/stable/), and lint with [flake8](https://github.com/PyCQA/flake8) automatically prior to each commit. To minimize test errors when submitting pull requests, please install pre-commit in your environment as follows:
+
+```bash
+pre-commit install
+```
+
+When these packages are executed within the project root directory, they should automatically use the [project settings](./pyproject.toml).
 
 [NumPy style docstrings](https://numpydoc.readthedocs.io/en/latest/format.html) are used for API documentation.
```

### Comparing `iohub-0.1.0.dev3/LICENSE` & `iohub-0.1.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `iohub-0.1.0.dev3/PKG-INFO` & `iohub-0.1.0.dev4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: iohub
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: N-dimensional bioimaging data I/O with OME metadata in Python
-Home-page: https://github.com/czbiohub/iohub
+Home-page: https://github.com/czbiohub-sf/iohub
 Author: CZ Biohub and iohub contributors
 Author-email: iohub@czbiohub.org
 License: BSD 3-Clause License
-Project-URL: Bug Tracker, https://github.com/czbiohub/iohub/issues
-Project-URL: Documentation, https://czbiohub.github.io/iohub
-Project-URL: Source Code, https://github.com/czbiohub/iohub
-Project-URL: User Support, https://github.com/czbiohub/iohub/issues
+Project-URL: Bug Tracker, https://github.com/czbiohub-sf/iohub/issues
+Project-URL: Documentation, https://czbiohub-sf.github.io/iohub
+Project-URL: Source Code, https://github.com/czbiohub-sf/iohub
+Project-URL: User Support, https://github.com/czbiohub-sf/iohub/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Operating System :: Microsoft :: Windows
@@ -34,31 +34,31 @@
 ## Supported formats
 
 ### Read
 
 - OME-Zarr ([OME-NGFF v0.4](https://ngff.openmicroscopy.org/0.4/))
 - Micro-Manager TIFF sequence, OME-TIFF (MMStack), and NDTiff datasets
 - Custom data formats generated by Biohub microscopes
-  - Supported: Falcon (PTI)
-  - WIP: Mantis, Dragonfly, Dorado
+  - Supported: Falcon (PTI), Dorado (ClearControl)
+  - WIP: Mantis, Dragonfly
   - TBA: DaXi
 
 ### Write
 
 - OME-Zarr
 - Multi-page TIFF stacks organized in a directory hierarchy that mimics OME-NGFF (WIP)
 
 ## Quick start
 
 ### Installation
 
 Install iohub with pip:
 
 ```sh
-git clone https://github.com/czbiohub/iohub.git
+git clone https://github.com/czbiohub-sf/iohub.git
 pip install /path/to/iohub
 ```
 
 > For more details about installation, see the [related section in the contribution guide](CONTRIBUTING.md#setting-up-developing-environment).
 
 ### Command-line interface
 
@@ -106,16 +106,16 @@
     )  # creates fov with the same path
     new_fov["0"] = raw_data.max(axis=1).reshape(
         (1, 1, 1, *raw_data.shape[2:])
     )  # max projection along Z axis and prepend dims to 5D
     dataset.print_tree()  # checks that new data has been written
 ```
 
-For more about API usage, refer to the [documentation](https://czbiohub.github.io/iohub/)
-and the [example scripts](https://github.com/czbiohub/iohub/tree/main/examples).
+For more about API usage, refer to the [documentation](https://czbiohub-sf.github.io/iohub/)
+and the [example scripts](https://github.com/czbiohub-sf/iohub/tree/main/examples).
 
 ### Reading Micro-Manager TIFF data
 
 Read a directory containing a TIFF dataset:
 
 ```py
 from iohub import read_micromanager
@@ -125,17 +125,17 @@
 ```
 
 ## Why iohub?
 
 This project is inspired by the existing Python libraries for bioimaging data I/O,
 including [ome-zarr-py](https://github.com/ome/ome-zarr-py), [tifffile](https://github.com/cgohlke/tifffile) and [aicsimageio](https://github.com/AllenCellModeling/aicsimageio).
 They support some of the most widely adopted and/or promising formats in microscopy,
-such as OME-Zarr and OME-Tiff.
+such as OME-Zarr and OME-TIFF.
 
 iohub bridges the gaps among them with the following features:
 
 - Efficient reading of data in various TIFF-based formats produced by the Micro-Manager/Pycro-Manager acquisition stack.
-- Efficient and customizable conversion of data and metadata from Tiff to OME-Zarr.
+- Efficient and customizable conversion of data and metadata from TIFF to OME-Zarr.
 - Pythonic and atomic access of OME-Zarr data with parallelized analysis in mind.
 - OME-Zarr metadata is automatically constructed and updated for writing,
 and verified against the specification when reading.
 - Adherence to the latest OME-NGFF specification (v0.4) whenever possible.
```

### Comparing `iohub-0.1.0.dev3/README.md` & `iohub-0.1.0.dev4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 ## Supported formats
 
 ### Read
 
 - OME-Zarr ([OME-NGFF v0.4](https://ngff.openmicroscopy.org/0.4/))
 - Micro-Manager TIFF sequence, OME-TIFF (MMStack), and NDTiff datasets
 - Custom data formats generated by Biohub microscopes
-  - Supported: Falcon (PTI)
-  - WIP: Mantis, Dragonfly, Dorado
+  - Supported: Falcon (PTI), Dorado (ClearControl)
+  - WIP: Mantis, Dragonfly
   - TBA: DaXi
 
 ### Write
 
 - OME-Zarr
 - Multi-page TIFF stacks organized in a directory hierarchy that mimics OME-NGFF (WIP)
 
 ## Quick start
 
 ### Installation
 
 Install iohub with pip:
 
 ```sh
-git clone https://github.com/czbiohub/iohub.git
+git clone https://github.com/czbiohub-sf/iohub.git
 pip install /path/to/iohub
 ```
 
 > For more details about installation, see the [related section in the contribution guide](CONTRIBUTING.md#setting-up-developing-environment).
 
 ### Command-line interface
 
@@ -79,16 +79,16 @@
     )  # creates fov with the same path
     new_fov["0"] = raw_data.max(axis=1).reshape(
         (1, 1, 1, *raw_data.shape[2:])
     )  # max projection along Z axis and prepend dims to 5D
     dataset.print_tree()  # checks that new data has been written
 ```
 
-For more about API usage, refer to the [documentation](https://czbiohub.github.io/iohub/)
-and the [example scripts](https://github.com/czbiohub/iohub/tree/main/examples).
+For more about API usage, refer to the [documentation](https://czbiohub-sf.github.io/iohub/)
+and the [example scripts](https://github.com/czbiohub-sf/iohub/tree/main/examples).
 
 ### Reading Micro-Manager TIFF data
 
 Read a directory containing a TIFF dataset:
 
 ```py
 from iohub import read_micromanager
@@ -98,17 +98,17 @@
 ```
 
 ## Why iohub?
 
 This project is inspired by the existing Python libraries for bioimaging data I/O,
 including [ome-zarr-py](https://github.com/ome/ome-zarr-py), [tifffile](https://github.com/cgohlke/tifffile) and [aicsimageio](https://github.com/AllenCellModeling/aicsimageio).
 They support some of the most widely adopted and/or promising formats in microscopy,
-such as OME-Zarr and OME-Tiff.
+such as OME-Zarr and OME-TIFF.
 
 iohub bridges the gaps among them with the following features:
 
 - Efficient reading of data in various TIFF-based formats produced by the Micro-Manager/Pycro-Manager acquisition stack.
-- Efficient and customizable conversion of data and metadata from Tiff to OME-Zarr.
+- Efficient and customizable conversion of data and metadata from TIFF to OME-Zarr.
 - Pythonic and atomic access of OME-Zarr data with parallelized analysis in mind.
 - OME-Zarr metadata is automatically constructed and updated for writing,
 and verified against the specification when reading.
 - Adherence to the latest OME-NGFF specification (v0.4) whenever possible.
```

### Comparing `iohub-0.1.0.dev3/docs/Makefile` & `iohub-0.1.0.dev4/docs/Makefile`

 * *Files 24% similar despite different names*

```diff
@@ -9,22 +9,31 @@
 ALLSPHINXOPTS   = -d $(BUILDDIR)/doctrees $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) source
 # the i18n builder cannot share the environment and doctrees with the others
 I18NSPHINXOPTS  = $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) source
 
 .PHONY: help clean build publish
 
 help:
-	@echo "Please use \`make <target>' where <target> is one of"
-	@echo "  html       to make standalone HTML files"
+	@echo "Build iohub HTML documentation."
+	@echo
+	@echo "Usage: make COMMAND"
+	@echo
+	@echo "Commands:"
+	@echo "build\tBuild from current source code"
+	@echo "publish\tBuild multiple versions for publishing"
+	@echo "clean\tRemove all built files"
+	@echo "help\tShow this message and quit"
 
 clean:
 	-rm -rf $(BUILDDIR)/*
+	-rm -rf source/auto_examples/*
 
 build:
 	$(SPHINXBUILD) -b html $(ALLSPHINXOPTS) $(BUILDDIR)/html
 	@echo
 	@echo "Build finished. The HTML pages are in $(BUILDDIR)/html."
 
 publish:
 	sphinx-multiversion source build/html
+	cp gh-pages-redirect.html build/html/index.html
 	@echo
 	@echo "Build finished. The HTML pages are in $(BUILDDIR)/html."
```

### Comparing `iohub-0.1.0.dev3/docs/source/conf.py` & `iohub-0.1.0.dev4/docs/source/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*- coding: utf-8 -*-
 
 
 import os
 
-# -- General configuration -----------------------------------------------------
+# Add any Sphinx extension module names, as strings. They can be extensions
+# coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+import sys
+
+import importlib_metadata
+
+# -- General configuration ----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
-# Add any Sphinx extension module names here, as strings. They can be extensions
-# coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-import sys
-
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath("../../"))
 
 source_dir = os.path.dirname(__file__)
@@ -28,38 +30,55 @@
     "sphinx.ext.intersphinx",
     "sphinx.ext.autosummary",
     "sphinx.ext.extlinks",
     "sphinx.ext.viewcode",
     "sphinx_copybutton",
     "numpydoc",
     "sphinx_multiversion",
+    "sphinx_sitemap",
+    "sphinx_gallery.gen_gallery",
 ]
 
+# default url is a dummy for local build
+html_baseurl = os.environ.get(
+    "GITHUB_PAGES_URL", f"file://{os.path.dirname(source_dir)}/build/html/"
+)
+sitemap_locales = ["en"]
+sitemap_url_scheme = "{link}"
 
 numpydoc_show_class_members = True
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ["_templates"]
 
 # Disabling generation of docs on different branches to use tags only
-# smv_branch_whitelist = None
-# smv_tag_whitelist = r'^v\d+\.\d+\.\d+$'
+smv_tag_whitelist = r"^v\d+\.\d+\.\d+$"
+smv_branch_whitelist = r"^main$"
+smv_latest_version = r"^main$"
 
 # The suffix of source filenames.
 source_suffix = ".rst"
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "iohub"
 copyright = "2023. Chan Zuckerberg Biohub. All rights reserved"
+release = importlib_metadata.version("iohub")
+
+json_url = f"{html_baseurl}/main/_static/switcher.json"
+if "dev" in release or "rc" in release:
+    # json_url = "_static/switcher.json"
+    version_match = "latest"
+else:
+    version_match = release
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
@@ -67,15 +86,15 @@
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = []
 
-# The reST default role (used for this markup: `text`) to use for all documents.
+# The reST default role (used for this markup `text`) to use for all documents.
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
@@ -88,58 +107,72 @@
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "default"
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
 
-# -- Options for HTML output ---------------------------------------------------
+# -- Options for HTML output --------------------------------------------------
 
-html_theme = "sphinx_rtd_theme"
+html_theme = "pydata_sphinx_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-# html_theme_options = {"logo_only": True}
+html_theme_options = {
+    "show_toc_level": 2,
+    "switcher": {
+        "json_url": json_url,
+        "version_match": version_match,
+    },
+    "navbar_end": ["theme-switcher", "version-switcher", "navbar-icon-links"],
+}
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-# html_title = None
+html_title = "iohub"
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 # html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 # html_logo = "resources/1.png"
 
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-# html_favicon = None
+# emoji favicon code adapted from:
+# https://twitter.com/LeaVerou/status/1241619866475474946
+html_favicon = (
+    "data:image/svg+xml,"
+    "<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22>"
+    r"<text y=%22.9em%22 font-size=%2290%22>💾</text>"
+    "</svg>"
+)
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-# html_static_path = ["_static"]
+html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 # html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
 # html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-# html_sidebars = {}
+html_sidebars = {"**": ["sidebar-nav-bs"]}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
 # html_additional_pages = {}
 
 # If false, no module index is generated.
 # html_domain_indices = True
@@ -167,7 +200,17 @@
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 # html_file_suffix = None
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "iohubdoc"
 
 numpydoc_show_class_members = False
+
+# sphinx-gallery config
+sphinx_gallery_conf = {
+    "examples_dirs": "../examples",
+    "gallery_dirs": "auto_examples",
+    "download_all_examples": False,
+    "filename_pattern": "/run_",
+    "min_reported_time": 2,
+    "show_signature": False,
+}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iohub-0.1.0.dev3/docs/source/contact_us/github.rst` & `iohub-0.1.0.dev4/docs/source/contact_us.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-================================
-Report a bug/Request a feature
-================================
+Contact Us
+==========
 
 If you would like to report a bug, request a feature, or communicate any related problem,
 please create an issue on our
-`GitHub repository <https://github.com/czbiohub/iohub>`_
+`GitHub repository <https://github.com/czbiohub-sf/iohub>`_
 if there is not an existing issue on the topic.
-
 You can also track pull-requests, milestones and our plans on our repository.
+
+Contributing
+------------
+
 Feel free to participate in discussions and contribute,
 but do not forget to read our
-`contributing guidelines <https://github.com/czbiohub/iohub/blob/main/CONTRIBUTING.md>`_ first.
+`contributing guidelines <https://github.com/czbiohub-sf/iohub/blob/main/CONTRIBUTING.md>`_ first.
```

### Comparing `iohub-0.1.0.dev3/examples/large_array_ome_zarr.py` & `iohub-0.1.0.dev4/docs/examples/run_large_array_ome_zarr.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-# %%
-# RUNNING THE FOLLOWING CODE WILL WRITE A LARGE FILE
-# This script shows how to store a larger-than-RAM array to a OME-Zarr dataset.
-# The same methods works for HCS datasets too.
-# It can be run as a plain Python script,
-# or as interactive cells in some IDEs.
-
+"""
+Writing a Large Array
+=====================
+
+This script shows how to store a larger-than-RAM array to a OME-Zarr dataset.
+The same method works for HCS datasets too.
+"""
 
+# %%
+# .. warning:: Executing this example will write a large file.
+#     Modify the store path manually.
 import numpy as np
 from tqdm import tqdm
 
 from iohub.ngff import open_ome_zarr
 
-# %%
-# FIXME: set Zarr store path here
 store_path = ""
 
 # %%
-# shape and data type of the large array
-# this array is about 10 GB, each time point is about 100 MB
-# it may not be actually larger than RAM but enough for demo
-# monitor the memory usage of python when the following runs
-# and it should take significantly less than 10 GB
+# Shape and data type of the large array
+# this array is about 10 GB, each time point is about 100 MB.
+# It may not be actually larger than RAM but enough for demo.
+# Monitor the memory usage of Python when the following runs
+# and it should take significantly less than 10 GB.
 shape = (100, 2, 25, 1024, 1024)
 dtype = np.uint16
 
 
 # %%
-# store this array by looping through the time points
+# .. note:: This will not run if the Zarr store path is not set above
+#
+# Store this array by looping through the time points
 if store_path:
     with open_ome_zarr(
         store_path, layout="fov", mode="w-", channel_names=["DAPI", "GFP"]
     ) as dataset:
         img = dataset.create_zeros(
             name="0",
             shape=shape,
```

### Comparing `iohub-0.1.0.dev3/examples/multi_fov_hcs_ome_zarr.py` & `iohub-0.1.0.dev4/docs/examples/run_multi_fov_hcs_ome_zarr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,30 @@
+"""
+Multi-FOV HCS OME-Zarr
+======================
+
+This script writes a high content screening (HCS) OME-Zarr dataset
+with a single FOV and a single scaling level per well,
+and adds an extra well-position to an existing dataset.
+"""
+
 # %%
-# This script writes a high content screening (HCS) OME-Zarr dataset
-# with a single FOV and a single scaling level per well,
-# and adds an extra well-position to an existing dataset.
-# It can be run as a plain Python script, or as interactive cells in some IDEs.
 
-import tempfile
+import os
+from tempfile import TemporaryDirectory
 
 import numpy as np
 
 from iohub.ngff import open_ome_zarr
 
 # %%
 # Set storage path
 
-store_path = f"{tempfile.gettempdir()}/hcs.zarr"
+tmp_dir = TemporaryDirectory()
+store_path = os.path.join(tmp_dir.name, "hcs.zarr")
 print("Zarr store path", store_path)
 
 # %%
 # Write 5D data to multiple wells.
 # Integer path names will be automatically converted to strings.
 # While the NGFF specification (and iohub) allows for arbitrary names,
 # the ome-zarr-py library and the napari-ome-zarr viewer
@@ -56,8 +63,11 @@
         position["0"][:, 3] = np.random.randint(
             0, np.iinfo(np.uint16).max, size=(5, 2, 32, 32), dtype=np.uint16
         )
     dataset.print_tree()
 
 # %%
 # Try viewing the images with napari-ome-zarr
-print("Zarr store path", store_path)
+
+# %%
+# Clean up
+tmp_dir.cleanup()
```

### Comparing `iohub-0.1.0.dev3/examples/single_fov_ome_zarr.py` & `iohub-0.1.0.dev4/docs/examples/run_single_fov_ome_zarr.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-# %%
-# This script shows how to create a single-FOV, single-scale OME-Zarr dataset,
-# read data in read-only mode,
-# append an extra time point to an existing dataset,
-# and adding a new channel to an existing dataset.
-# It can be run as a plain Python script,
-# or as interactive cells in some IDEs.
+"""
+Single-FOV OME-Zarr
+===================
+
+This script shows how to create a single-FOV, single-scale OME-Zarr dataset,
+read data in read-only mode,
+append an extra time point to an existing dataset,
+and adding a new channel to an existing dataset.
+"""
 
-import tempfile
+# %%
+import os
+from tempfile import TemporaryDirectory
 
 import numpy as np
 
 from iohub.ngff import open_ome_zarr
 
 # %%
 # Set storage path
-
-store_path = f"{tempfile.gettempdir()}/ome.zarr"
+tmp_dir = TemporaryDirectory()
+store_path = os.path.join(tmp_dir.name, "ome.zarr")
 print("Zarr store path", store_path)
 
 # %%
 # Write 5D data to a new Zarr store
 
 tczyx = np.random.randint(
     0, np.iinfo(np.uint16).max, size=(5, 2, 3, 32, 32), dtype=np.uint16
@@ -87,8 +91,11 @@
     dataset.update_channel("Renamed", target="img", data=new_tzyx)
 
 # Close the dataset
 dataset.close()
 
 # %%
 # Try viewing the images with napari-ome-zarr
-print("Zarr store path", store_path)
+
+# %%
+# Clean up
+tmp_dir.cleanup()
```

### Comparing `iohub-0.1.0.dev3/examples/tiled_ome_zarr.py` & `iohub-0.1.0.dev4/docs/examples/run_tiled_ome_zarr.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-# %%
-# This script shows how to create a tiled single-resolution OME-Zarr dataset,
-# make a tiles grid, and write data.
+"""
+Tiled OME-Zarr
+==============
+
+This script shows how to create a tiled single-resolution OME-Zarr dataset,
+make a tiles grid, and write data.
+"""
 
+# %%
 import os
+from tempfile import TemporaryDirectory
 
 import numpy as np
 
 from iohub.ngff import open_ome_zarr
 
 # %%
 # Set storage path
-
-store_path = f'{os.path.expanduser("~/")}ome.zarr'
+tmp_dir = TemporaryDirectory()
+store_path = os.path.join(tmp_dir.name, "tiled.zarr")
+print("Zarr store path", store_path)
 
 # %%
 # Write 5D data to a new Zarr store
 
 # define grid (rows, columns)
 grid_shape = (2, 3)
 # define tile shape (5D array)
 tile_shape = (5, 2, 3, 32, 32)
 
 
 with open_ome_zarr(
     store_path, layout="tiled", mode="a", channel_names=["DAPI", "GFP"]
 ) as dataset:
+    dtype = np.uint16
     tiles = dataset.make_tiles(
-        "tiled_raw", grid_shape=grid_shape, tile_shape=tile_shape
+        "tiled_raw", grid_shape=grid_shape, tile_shape=tile_shape, dtype=dtype
     )
     for row in range(grid_shape[0]):
         for column in range(grid_shape[1]):
             # each tile will be filled with different constant values
-            data = np.zeros(shape=tile_shape) + row + column
+            data = np.zeros(shape=tile_shape, dtype=dtype) + row + column
             tiles.write_tile(data, row, column)
 
 
 # %%
 # Load the dataset
 
 with open_ome_zarr(store_path, layout="tiled", mode="r") as dataset:
@@ -46,7 +54,11 @@
     # check grid and tile shapes
     print(tiled.tiles, tiled.tile_shape)
     # read a tile
     tile_1_2 = tiled.get_tile(1, 2)
 
 # %%
 # Try viewing the images with napari-ome-zarr
+
+# %%
+# Clean up
+tmp_dir.cleanup()
```

### Comparing `iohub-0.1.0.dev3/iohub/cli/cli.py` & `iohub-0.1.0.dev4/iohub/cli/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,25 +2,32 @@
 
 from iohub._version import __version__
 from iohub.convert import TIFFConverter
 from iohub.reader import print_info
 
 VERSION = __version__
 
+_DATASET_PATH = click.Path(exists=True, file_okay=False, resolve_path=True)
+
 
 @click.group()
 @click.help_option("-h", "--help")
 @click.version_option(version=VERSION)
 def cli():
     """\u001b[34;1m iohub: N-dimensional bioimaging I/O \u001b[0m"""
 
 
 @cli.command()
 @click.help_option("-h", "--help")
-@click.argument("files", nargs=-1, required=True)
+@click.argument(
+    "files",
+    nargs=-1,
+    required=True,
+    type=_DATASET_PATH,
+)
 @click.option(
     "--verbose",
     "-v",
     is_flag=True,
     help="Show usage guide to open dataset in Python "
     "and full tree for HCS Plates in OME-Zarr",
 )
@@ -38,15 +45,15 @@
 
 @cli.command()
 @click.help_option("-h", "--help")
 @click.option(
     "--input",
     "-i",
     required=True,
-    type=click.Path(exists=True, file_okay=False, resolve_path=True),
+    type=_DATASET_PATH,
     help="Input Micro-Manager TIFF dataset directory",
 )
 @click.option(
     "--output",
     "-o",
     required=True,
     type=click.Path(exists=False, resolve_path=True),
@@ -56,30 +63,40 @@
     "--format",
     "-f",
     required=False,
     type=str,
     help="Data type, 'ometiff', 'ndtiff', 'singlepagetiff'",
 )
 @click.option(
+    "--scale-voxels",
+    "-s",
+    required=False,
+    type=bool,
+    default=True,
+    help="Write voxel size (XY pixel size and Z-step, in micrometers) "
+    "as scale coordinate transformation in NGFF. By default true.",
+)
+@click.option(
     "--grid-layout",
     "-g",
     required=False,
     is_flag=True,
-    help="Arrange positions in a HCS grid layout",
+    help="Arrange FOVs in a row/column grid layout for tiled acquisition",
 )
 @click.option(
     "--label-positions",
     "-p",
     required=False,
     is_flag=True,
     help="Dump postion labels in MM metadata to Omero metadata",
 )
-def convert(input, output, format, grid_layout, label_positions):
+def convert(input, output, format, scale_voxels, grid_layout, label_positions):
     """Converts Micro-Manager TIFF datasets to OME-Zarr"""
     converter = TIFFConverter(
         input_dir=input,
         output_dir=output,
         data_type=format,
+        scale_voxels=scale_voxels,
         grid_layout=grid_layout,
         label_positions=label_positions,
     )
     converter.run()
```

### Comparing `iohub-0.1.0.dev3/iohub/convert.py` & `iohub-0.1.0.dev4/iohub/convert.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,16 +4,22 @@
 from typing import Literal
 
 import numpy as np
 from numpy.typing import NDArray
 from tqdm import tqdm
 
 from iohub._version import version as iohub_version
-from iohub.ngff import open_ome_zarr
-from iohub.reader import MicromanagerSequenceReader, read_micromanager
+from iohub.ngff import Position, TransformationMeta, open_ome_zarr
+from iohub.reader import (
+    MicromanagerOmeTiffReader,
+    MicromanagerSequenceReader,
+    read_micromanager,
+)
+
+__all__ = ["TIFFConverter"]
 
 
 def _create_grid_from_coordinates(
     xy_coords: list[tuple[float, float]], rows: int, columns: int
 ):
     """Function to create a grid from XY-position coordinates.
     Useful for generating HCS Zarr metadata.
@@ -78,24 +84,34 @@
         (useful for tiled acquisitions), by default False
     chunks : tuple[int], optional
         Chunk size of the output Zarr arrays, by default None
         (chunk by XY planes, this is the fastest at converting time)
     label_positions : bool, optional
         Dump postion labels in MM metadata to Omero metadata,
         by default False
+    scale_voxels : bool, optional
+        Write voxel size (XY pixel size and Z-step) as scaling transform,
+        by default True
+    hcs_plate : bool, optional
+        Create NGFF HCS layout based on position names from the
+        HCS Site Generator in Micro-Manager (only available for OME-TIFF),
+        and is ignored for other formats, by default None
+        (attempt to apply to OME-TIFF datasets, disable this with ``False``)
     """
 
     def __init__(
         self,
         input_dir: str,
         output_dir: str,
         data_type: Literal["singlepagetiff", "ometiff", "ndtiff"] = None,
         grid_layout: int = False,
         chunks: tuple[int] = None,
         label_positions: bool = False,
+        scale_voxels: bool = True,
+        hcs_plate: bool = None,
     ):
         logging.debug("Checking output.")
         if not output_dir.strip("/").endswith(".zarr"):
             raise ValueError("Please specify .zarr at the end of your output")
         self.output_dir = output_dir
         logging.info("Initializing data.")
         self.reader = read_micromanager(
@@ -119,34 +135,60 @@
         self.c = self.reader.channels
         self.z = self.reader.slices
         self.y = self.reader.height
         self.x = self.reader.width
         self.dim = (self.p, self.t, self.c, self.z, self.y, self.x)
         self.prefix_list = []
         self.label_positions = label_positions
+        self.hcs_plate = hcs_plate
+        self._check_hcs_sites()
         self._get_pos_names()
         logging.info(
             f"Found Dataset {self.save_name} with "
             f"dimensions (P, T, C, Z, Y, X): {self.dim}"
         )
         self._gen_coordset()
         self.metadata = dict()
         self.metadata["iohub_version"] = iohub_version
         self.metadata["Summary"] = self.summary_metadata
         if grid_layout:
+            if hcs_plate:
+                raise ValueError(
+                    "grid_layout and hcs_plate must not be both true"
+                )
             logging.info("Generating HCS plate level grid.")
             try:
                 self.position_grid = _create_grid_from_coordinates(
                     *self._get_position_coords()
                 )
             except ValueError:
                 self._make_default_grid()
         else:
             self._make_default_grid()
         self.chunks = chunks if chunks else (1, 1, 1, self.y, self.x)
+        self.transform = self._scale_voxels() if scale_voxels else None
+
+    def _check_hcs_sites(self):
+        is_mmstack = isinstance(self.reader, MicromanagerOmeTiffReader)
+        if self.hcs_plate:
+            if is_mmstack:
+                self.hcs_sites = self.reader.hcs_position_labels
+            else:
+                raise ValueError(
+                    f"HCS plate position not supported for {type(self.reader)}"
+                )
+        elif self.hcs_plate is None and is_mmstack:
+            try:
+                self.hcs_sites = self.reader.hcs_position_labels
+                self.hcs_plate = True
+            except ValueError:
+                logging.debug(
+                    "HCS sites not detected, "
+                    "dumping all position into a single row."
+                )
 
     def _make_default_grid(self):
         self.position_grid = np.expand_dims(
             np.arange(self.p, dtype=int), axis=0
         )
 
     def _gen_coordset(self):
@@ -290,54 +332,106 @@
         if not cns and isinstance(self.reader, MicromanagerSequenceReader):
             logging.warning(
                 "Using an empty channel name for the single channel."
             )
             cns = [str(i) for i in range(self.c)]
         return cns
 
-    def _init_hcs_arrays(self):
+    def _scale_voxels(self):
+        z_um = self.reader.z_step_size
+        if self.z_dim > 1 and not z_um:
+            logging.warning(
+                "Z step size is not available. "
+                "Setting the Z axis scaling factor to 1."
+            )
+            z_um = 1.0
+        xy_warning = (
+            " Setting X and Y scaling factors to 1."
+            " Suppress this warning by setting `scale-voxels` to false."
+        )
+        if isinstance(self.reader, MicromanagerSequenceReader):
+            logging.warning(
+                "Pixel size detection is not supported for single-page TIFFs."
+                + xy_warning
+            )
+            xy_um = 1.0
+        else:
+            try:
+                xy_um = self.reader.xy_pixel_size
+            except AttributeError as e:
+                logging.warning(str(e) + xy_warning)
+                xy_um = 1.0
+        return [
+            TransformationMeta(
+                type="scale", scale=[1.0, 1.0, z_um, xy_um, xy_um]
+            )
+        ]
+
+    def _init_zarr_arrays(self):
         self.writer = open_ome_zarr(
             self.output_dir,
             layout="hcs",
             mode="w-",
             channel_names=self._get_channel_names(),
             version="0.4",
         )
-        self.well_list = []
+        self.zarr_position_names = []
+        arr_kwargs = {
+            "name": "0",
+            "shape": (
+                self.t if self.t != 0 else 1,
+                self.c if self.c != 0 else 1,
+                self.z if self.z != 0 else 1,
+                self.y,
+                self.x,
+            ),
+            "dtype": self.reader.dtype,
+            "chunks": self.chunks,
+            "transform": self.transform,
+        }
+        if self.hcs_plate:
+            self._init_hcs_arrays(arr_kwargs)
+        else:
+            self._init_grid_arrays(arr_kwargs)
+
+    def _init_hcs_arrays(self, arr_kwargs):
+        for row, col, fov in self.hcs_sites:
+            self._create_zeros_array(row, col, fov, arr_kwargs)
+        logging.info(
+            "Created HCS NGFF layout from Micro-Manager HCS position labels."
+        )
+        self.writer.print_tree()
+
+    def _init_grid_arrays(self, arr_kwargs):
         for row, columns in enumerate(self.position_grid):
             for column in columns:
-                pos_name = self.pos_names[len(self.well_list)]
-                pos = self.writer.create_position(row, column, pos_name="0")
-                self.well_list.append(os.path.join(str(row), str(column)))
-                _ = pos.zgroup.zeros(
-                    "0",
-                    shape=(
-                        self.t if self.t != 0 else 1,
-                        self.c if self.c != 0 else 1,
-                        self.z if self.z != 0 else 1,
-                        self.y,
-                        self.x,
-                    ),
-                    chunks=self.chunks,
-                )
-                pos._create_image_meta("0")
-                pos.metadata.omero.name = pos_name
-                pos.dump_meta()
+                self._create_zeros_array(row, column, "0", arr_kwargs)
+
+    def _create_zeros_array(
+        self, row_name: str, col_name: str, pos_name: str, arr_kwargs: dict
+    ) -> Position:
+        pos = self.writer.create_position(row_name, col_name, pos_name)
+        self.zarr_position_names.append(pos.zgroup.name)
+        _ = pos.create_zeros(**arr_kwargs)
+        pos.metadata.omero.name = self.pos_names[
+            len(self.zarr_position_names) - 1
+        ]
+        pos.dump_meta()
 
     def run(self, check_image: bool = True):
         """Runs the conversion.
 
         Parameters
         ----------
         check_image : bool, optional
             Whether to check that the written Zarr array has the same
             pixel values as in TIFF files, by default True
         """
         logging.debug("Setting up Zarr store.")
-        self._init_hcs_arrays()
+        self._init_zarr_arrays()
         bar_format = (
             "Status: |{bar:16}|{n_fmt}/{total_fmt} "
             "(Time Remaining: {remaining}), {rate_fmt}{postfix}]"
         )
         # Run through every coordinate and convert in acquisition order
         logging.info("Converting Images...")
         for coord in tqdm(self.coords, bar_format=bar_format):
@@ -346,14 +440,14 @@
             if img_raw is None or not getattr(img_raw, "shape", ()):
                 # Leave incomplete datasets zero-filled
                 logging.warning(
                     f"Cannot load image at PTCZ={coord_reorder}, "
                     "filling with zeros. Check if the raw data is incomplete."
                 )
                 continue
-            well = self.well_list[coord_reorder[0]]
-            zarr_img = self.writer[well]["0"]["0"]
+            pos_name = self.zarr_position_names[coord_reorder[0]]
+            zarr_img = self.writer[pos_name]["0"]
             zarr_img[coord_reorder[1:]] = img_raw
             if check_image:
                 self._perform_image_check(zarr_img[coord_reorder[1:]], img_raw)
         self.writer.zgroup.attrs.update(self.metadata)
         self.writer.close()
```

### Comparing `iohub-0.1.0.dev3/iohub/display_utils.py` & `iohub-0.1.0.dev4/iohub/display_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """ Utility functions for displaying data """
 
-from typing import Tuple
-
 import numpy as np
 from PIL.ImageColor import colormap
 
 from iohub.ngff_meta import ChannelMeta, WindowDict
 
 """ Dictionary with key works and most popular fluorescent probes """
 CHANNEL_COLORS = {
@@ -58,26 +56,26 @@
     str the HEX value in uppercase and without the '#'
     """
     return colormap[color][1:].upper()
 
 
 def channel_display_settings(
     chan_name: str,
-    clim: Tuple[float, float, float, float] = None,
+    clim: tuple[float, float, float, float] = None,
     first_chan: bool = False,
 ):
     """This will create a dictionary used for OME-zarr metadata.
     Allows custom contrast limits and channel.
     names for display. Defaults everything to grayscale.
 
     Parameters
     ----------
     chan_name : str
         Desired name of the channel for display
-    clim : Tuple[float, float, float, float], optional
+    clim : tuple[float, float, float, float], optional
         Contrast limits (start, end, min, max)
     first_chan : bool, optional
         Whether or not this is the first channel of the dataset
         (display will be set to active),
         by default False
 
     Returns
@@ -101,15 +99,17 @@
     if not clim:
         if chan_name in channel_settings.keys():
             clim = channel_settings[chan_name]
         else:
             clim = channel_settings["Other"]
     # Mapping channel name to color
     for key in CHANNEL_COLORS:
-        if chan_name in CHANNEL_COLORS[key]:
+        # Does chan_name have any of the values in the CHANNEL_COLORS[key]
+        # list as a substring?
+        if any([value in chan_name for value in CHANNEL_COLORS[key]]):
             display_color = color_to_hex(key)
             break
         else:
             display_color = color_to_hex("white")
 
     window = WindowDict(start=clim[0], end=clim[1], min=clim[2], max=clim[3])
     return ChannelMeta(
```

### Comparing `iohub-0.1.0.dev3/iohub/multipagetiff.py` & `iohub-0.1.0.dev4/iohub/multipagetiff.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import glob
+import logging
 import os
 from copy import copy
 
 import numpy as np
 import zarr
 from tifffile import TiffFile
 
@@ -30,31 +31,32 @@
                     f"Path {folder} contains no `.ome.tif` files, "
                     "please specify a valid input directory."
                 )
             )
 
         # Grab all image files
         self.data_directory = folder
-        self._files = glob.glob(os.path.join(self.data_directory, "*.ome.tif"))
+        self._files = sorted(
+            glob.glob(os.path.join(self.data_directory, "*.ome.tif"))
+        )
 
         # Generate Data Specific Properties
         self.coords = None
         self.coord_map = dict()
         self.pos_names = []
         self.position_arrays = dict()
         self.positions = 0
         self.frames = 0
         self.channels = 0
         self.slices = 0
         self.height = 0
         self.width = 0
-        self._set_dtype()
+        self._infer_image_meta()
 
         # Initialize MM attributes
-        self.z_step_size = None
         self.channel_names = []
 
         # Read MM data
         self._set_mm_meta()
 
         # Gather index map of file, page, byte offset
         self._gather_index_maps()
@@ -140,23 +142,23 @@
         """
         with TiffFile(self._files[0]) as tif:
             self.mm_meta = tif.micromanager_metadata
 
             mm_version = self.mm_meta["Summary"]["MicroManagerVersion"]
             if "beta" in mm_version:
                 if self.mm_meta["Summary"]["Positions"] > 1:
-                    self.stage_positions = []
+                    self._stage_positions = []
 
                     for p in range(
                         len(self.mm_meta["Summary"]["StagePositions"])
                     ):
                         pos = self._simplify_stage_position_beta(
                             self.mm_meta["Summary"]["StagePositions"][p]
                         )
-                        self.stage_positions.append(pos)
+                        self._stage_positions.append(pos)
 
                 # MM beta versions sometimes don't have 'ChNames',
                 # so I'm wrapping in a try-except and setting the
                 # channel names to empty strings if it fails.
                 try:
                     for ch in self.mm_meta["Summary"]["ChNames"]:
                         self.channel_names.append(ch)
@@ -169,21 +171,21 @@
 
             elif mm_version == "1.4.22":
                 for ch in self.mm_meta["Summary"]["ChNames"]:
                     self.channel_names.append(ch)
 
             else:
                 if self.mm_meta["Summary"]["Positions"] > 1:
-                    self.stage_positions = []
+                    self._stage_positions = []
 
                     for p in range(self.mm_meta["Summary"]["Positions"]):
                         pos = self._simplify_stage_position(
                             self.mm_meta["Summary"]["StagePositions"][p]
                         )
-                        self.stage_positions.append(pos)
+                        self._stage_positions.append(pos)
 
                 for ch in self.mm_meta["Summary"]["ChNames"]:
                     self.channel_names.append(ch)
 
             # dimensions based on mm metadata
             # do not reflect final written dimensions
             # these will change after data is loaded
@@ -276,27 +278,40 @@
         # is incomplete
         for p, t, c, z in self.coord_map.keys():
             if p == pos:
                 self.position_arrays[pos][t, c, z, :, :] = self.get_image(
                     pos, t, c, z
                 )
 
-    def _set_dtype(self):
+    def _infer_image_meta(self):
         """
-        gets the datatype from any image plane metadata
-
-        Returns
-        -------
-
+        Infer data type and pixel size from the first image plane metadata.
         """
+        with TiffFile(self._files[0]) as tf:
+            page = tf.pages[0]
+            self.dtype = page.dtype
+            for tag in page.tags.values():
+                if tag.name == "MicroManagerMetadata":
+                    # assuming X and Y pixel sizes are the same
+                    xy_size = tag.value.get("PixelSizeUm")
+                    self._xy_pixel_size = xy_size if xy_size else None
+                    return
+                else:
+                    continue
+            logging.warning(
+                "Micro-Manager image plane metadata cannot be loaded."
+            )
+            self._xy_pixel_size = None
 
-        tf = TiffFile(self._files[0])
-
-        self.dtype = tf.pages[0].dtype
-        tf.close()
+    @property
+    def xy_pixel_size(self):
+        """XY pixel size of the camera in micrometers."""
+        if self._xy_pixel_size is None:
+            raise AttributeError("XY pixel size cannot be determined.")
+        return self._xy_pixel_size
 
     def _get_dimensions(self, position):
         """
         Gets the max dimensions from the current position
         in case of incomplete datasets
 
         Parameters
@@ -398,7 +413,31 @@
 
         Returns
         -------
         number of positions     (int)
 
         """
         return self.positions
+
+    @property
+    def hcs_position_labels(self):
+        """Parse plate position labels generated by the HCS position generator,
+        e.g. 'A1-Site_0', and split into row, column, and FOV names.
+
+        Returns
+        -------
+        list[tuple[str, str, str]]
+            FOV name paths, e.g. ('A', '1', '0')
+        """
+        if not self.stage_positions:
+            raise ValueError("Stage position metadata not available.")
+        try:
+            labels = [
+                pos["Label"].split("-Site_") for pos in self.stage_positions
+            ]
+            return [(well[0], well[1:], fov) for well, fov in labels]
+        except Exception:
+            raise ValueError(
+                "HCS position labels are in the format of "
+                "'A1-Site_0', 'H12-Site_1', ... "
+                f"Got labels {[pos['Label'] for pos in self.stage_positions]}"
+            )
```

### Comparing `iohub-0.1.0.dev3/iohub/ndtiff.py` & `iohub-0.1.0.dev4/iohub/ndtiff.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import zarr
 from ndtiff import Dataset
 
 from iohub.reader_base import ReaderBase
 
 
 class NDTiffReader(ReaderBase):
+    """Reader for ND-TIFF datasets acquired with Micro/Pycro-Manager,
+    effectively a wrapper of the `ndtiff.Dataset` class.
+    """
+
     def __init__(self, data_path: str):
-        """Reader for ND-TIFF datasets acquired with Micro/Pycro-Manager,
-        effectively a wrapper of the `ndtiff.Dataset` class.
-        """
         super().__init__()
 
         self.dataset = Dataset(data_path)
         self._axes = self.dataset.axes
 
         self.frames = (
             len(self._axes["time"]) if "time" in self._axes.keys() else 1
@@ -28,14 +29,15 @@
         self.width = self.dataset.image_width
         self.dtype = self.dataset.dtype
 
         self.mm_meta = self._get_summary_metadata()
         self.channel_names = list(self.dataset.get_channel_names())
         self.stage_positions = self.mm_meta["Summary"]["StagePositions"]
         self.z_step_size = self.mm_meta["Summary"]["z-step_um"]
+        self.xy_pixel_size = self.mm_meta["Summary"]["PixelSize_um"]
 
     def _get_summary_metadata(self):
         pm_metadata = self.dataset.summary_metadata
         pm_metadata["MicroManagerVersion"] = "pycromanager"
         pm_metadata["Positions"] = self.get_num_positions()
 
         img_metadata = self.get_image_metadata(0, 0, 0, 0)
@@ -113,60 +115,50 @@
 
         if self.dataset.has_image(position=p, time=t, channel=c, z=z):
             image = self.dataset.read_image(position=p, time=t, channel=c, z=z)
 
         return image
 
     def get_zarr(self, position: int) -> zarr.array:
-        """
-        return a lazy-loaded dask array with shape TCZYX at the given position.
-        Data is not loaded into memory.
+        """.. danger::
+            The behavior of this function is different from other
+            ReaderBase children as it return a Dask array
+            rather than a zarr array.
 
-        Note: The behavior of this function is different from other
-        ReaderBase children as it return a Dask array rather than a zarr array.
+        Return a lazy-loaded dask array with shape TCZYX at the given position.
+        Data is not loaded into memory.
 
-        # TODO: try casting the dask array into a zarr array
-        # using `dask.array.to_zarr()`.
-        # Currently this call brings the data into memory
 
         Parameters
         ----------
         position:       (int) position index
 
         Returns
         -------
         position:       (zarr.array)
 
         """
-
-        ax = [
-            ax_
-            for ax_ in ["position", "time", "channel", "z"]
-            if ax_ in self._axes
-        ]
-
-        if "position" in self._axes.keys():
-            # da is Dask array
-            da = self.dataset.as_array(axes=ax, position=position)
-        else:
-            if position not in (0, None):
-                warnings.warn(
-                    f"Position index {position} is not part of this dataset."
-                    f" Returning data at default position."
-                )
-            da = self.dataset.as_array(axes=ax)
-
+        # TODO: try casting the dask array into a zarr array
+        # using `dask.array.to_zarr()`.
+        # Currently this call brings the data into memory
+        if "position" not in self._axes.keys() and position not in (0, None):
+            warnings.warn(
+                f"Position index {position} is not part of this dataset. "
+                "Returning data at the default position."
+            )
+            position = None
+        da = self.dataset.as_array(position=position)
         shape = (
             self.frames,
             self.channels,
             self.slices,
             self.height,
             self.width,
         )
-
+        # add singleton axes so output is 5D
         return da.reshape(shape)
 
     def get_array(self, position: int) -> np.ndarray:
         """
         return a numpy array with shape TCZYX at the given position
 
         Parameters
```

### Comparing `iohub-0.1.0.dev3/iohub/ngff.py` & `iohub-0.1.0.dev4/iohub/ngff.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # TODO: remove this in the future (PEP deferred for 3.11, now 3.12?)
 from __future__ import annotations
 
 import logging
+import math
 import os
-from typing import TYPE_CHECKING, Generator, List, Literal, Tuple, Union
+from copy import deepcopy
+from typing import TYPE_CHECKING, Generator, Literal, Sequence, Union
 
 import numpy as np
 import zarr
 from numcodecs import Blosc
 from numpy.typing import ArrayLike, DTypeLike, NDArray
 from pydantic import ValidationError
 from zarr.util import normalize_storage_path
@@ -68,14 +70,19 @@
     except Exception as e:
         raise RuntimeError(
             f"Cannot open Zarr root group at {store_path}"
         ) from e
     return root
 
 
+def _scale_integers(values: Sequence[int], factor: int) -> tuple[int, ...]:
+    """Computes the ceiling of the input sequence divided by the factor."""
+    return tuple(int(math.ceil(v / factor)) for v in values)
+
+
 class NGFFNode:
     """A node (group level in Zarr) in an NGFF dataset."""
 
     _MEMBER_TYPE = None
     _DEFAULT_AXES = [
         AxisMeta(name="T", type="time", unit="second"),
         AxisMeta(name="C", type="channel"),
@@ -486,17 +493,17 @@
     ----------
     version : Literal["0.1", "0.4"]
         OME-NGFF specification version
     zgroup : Group
         Root Zarr group holding arrays
     zattr : Attributes
         Zarr attributes of the group
-    channel_names : List[str]
+    channel_names : list[str]
         Name of the channels
-    axes : List[AxisMeta]
+    axes : list[AxisMeta]
         Axes metadata
     """
 
     _MEMBER_TYPE = ImageArray
 
     def __init__(
         self,
@@ -548,15 +555,15 @@
 
     @property
     def _member_names(self):
         return self.array_keys()
 
     @property
     def data(self):
-        """.. Warning:
+        """.. warning::
             This property does *NOT* aim to retrieve all the arrays.
             And it may also fail to retrive any data if arrays exist but
             are not named conventionally.
 
         Alias for an array named '0' in the position,
         which is usually the raw data (or the finest resolution in a pyramid).
 
@@ -621,29 +628,29 @@
         yield from self.iteritems()
 
     def create_image(
         self,
         name: str,
         data: NDArray,
         chunks: tuple[int] = None,
-        transform: List[TransformationMeta] = None,
+        transform: list[TransformationMeta] = None,
         check_shape: bool = True,
     ):
         """Create a new image array in the position.
 
         Parameters
         ----------
         name : str
             Name key of the new image.
         data : NDArray
             Image data.
         chunks : tuple[int], optional
             Chunk size, by default None.
             ZYX stack size will be used if not specified.
-        transform : List[TransformationMeta], optional
+        transform : list[TransformationMeta], optional
             List of coordinate transformations, by default None.
             Should be specified for a non-native resolution level.
         check_shape : bool, optional
             Whether to check if image shape matches dataset axes,
             by default True
 
         Returns
@@ -665,15 +672,15 @@
 
     def create_zeros(
         self,
         name: str,
         shape: tuple[int],
         dtype: DTypeLike,
         chunks: tuple[int] = None,
-        transform: List[TransformationMeta] = None,
+        transform: list[TransformationMeta] = None,
         check_shape: bool = True,
     ):
         """Create a new zero-filled image array in the position.
         Under default zarr-python settings of lazy writing,
         this will not write the array values,
         but only create a ``.zarray`` file.
         This is useful for writing larger-than-RAM images
@@ -686,15 +693,15 @@
         shape : tuple
             Image shape.
         dtype : DTypeLike
             Data type.
         chunks : tuple[int], optional
             Chunk size, by default None.
             ZYX stack size will be used if not specified.
-        transform : List[TransformationMeta], optional
+        transform : list[TransformationMeta], optional
             List of coordinate transformations, by default None.
             Should be specified for a non-native resolution level.
         check_shape : bool, optional
             Whether to check if image shape matches dataset axes,
             by default True
 
         Returns
@@ -744,15 +751,15 @@
                 "Dataset channel axis is not set. "
                 "Skipping channel shape check."
             )
 
     def _create_image_meta(
         self,
         name: str,
-        transform: List[TransformationMeta] = None,
+        transform: list[TransformationMeta] = None,
         extra_meta: dict = None,
     ):
         if not transform:
             transform = [TransformationMeta(type="identity")]
         dataset_meta = DatasetMeta(
             path=name, coordinate_transformations=transform
         )
@@ -777,15 +784,15 @@
             self.metadata.multiscales[0].datasets.append(dataset_meta)
         self.dump_meta()
 
     def _omero_meta(
         self,
         id: int,
         name: str,
-        clims: List[Tuple[float, float, float, float]] = None,
+        clims: list[tuple[float, float, float, float]] = None,
     ):
         if not clims:
             clims = [None] * len(self.channel_names)
         channels = []
         for i, (channel_name, clim) in enumerate(
             zip(self.channel_names, clims)
         ):
@@ -896,14 +903,106 @@
         img = self[target]
         ch_idx = self.get_channel_index(chan_name)
         ch_ax = self._get_channel_axis()
         ortho_sel = [slice(None)] * len(img.shape)
         ortho_sel[ch_ax] = ch_idx
         img.set_orthogonal_selection(tuple(ortho_sel), data)
 
+    def initialize_pyramid(self, levels: int) -> None:
+        """
+        Initializes the pyramid arrays with a down scaling of 2 per level.
+        Decimals shapes are rounded up to ceiling.
+        Scales metadata are also updated.
+
+        Parameters
+        ----------
+        levels : int
+            Number of down scaling levels, if levels is 1 nothing happens.
+        """
+        array = self.data
+        for level in range(1, levels):
+            factor = 2**level
+
+            shape = array.shape[:-3] + _scale_integers(
+                array.shape[-3:], factor
+            )
+
+            chunks = _pad_shape(
+                _scale_integers(array.shape[-3:], factor), len(shape)
+            )
+
+            transforms = deepcopy(
+                self.metadata.multiscales[0]
+                .datasets[0]
+                .coordinate_transformations
+            )
+            for tr in transforms:
+                if tr.type == "scale":
+                    for i in range(len(tr.scale))[-3:]:
+                        tr.scale[i] /= factor
+
+            self.create_zeros(
+                name=str(level),
+                shape=shape,
+                dtype=array.dtype,
+                chunks=chunks,
+                transform=transforms,
+            )
+
+    @property
+    def scale(self) -> list[float]:
+        """
+        Helper function for scale transform metadata of
+        highest resolution scale.
+        """
+        scale = [1] * self.data.ndim
+        transforms = (
+            self.metadata.multiscales[0].datasets[0].coordinate_transformations
+        )
+        for trans in transforms:
+            if trans.type == "scale":
+                if len(trans.scale) != len(scale):
+                    raise RuntimeError(
+                        f"Length of scale transformation {len(trans.scale)} "
+                        f"does not match data dimension {len(scale)}."
+                    )
+                scale = [s1 * s2 for s1, s2 in zip(scale, trans.scale)]
+        return scale
+
+    def set_transform(
+        self,
+        image: Union[str, Literal["*"]],
+        transform: list[TransformationMeta],
+    ):
+        """Set the coordinate transformations metadata
+        for one image array or the whole FOV.
+
+        Parameters
+        ----------
+        image : Union[str, Literal["*"]]
+            Name of one image array (e.g. "0") to transform,
+            or "*" for the whole FOV
+        transform : list[TransformationMeta]
+            List of transformations to apply
+            (:py:class:`iohub.ngff_meta.TransformationMeta`)
+        """
+        if image == "*":
+            self.metadata.multiscales[0].coordinate_transformations = transform
+        elif image in self:
+            for i, dataset_meta in enumerate(
+                self.metadata.multiscales[0].datasets
+            ):
+                if dataset_meta.path == image:
+                    self.metadata.multiscales[0].datasets[i] = DatasetMeta(
+                        path=image, coordinate_transformations=transform
+                    )
+        else:
+            raise ValueError(f"Key {image} not recognized.")
+        self.dump_meta()
+
 
 class TiledPosition(Position):
     """Variant of the NGFF position node
     with convenience methods to create and access tiled arrays.
     Other parameters and attributes are the same as
     :py:class:`iohub.ngff.Position`.
     """
@@ -912,15 +1011,15 @@
 
     def make_tiles(
         self,
         name: str,
         grid_shape: tuple[int, int],
         tile_shape: tuple[int],
         dtype: DTypeLike,
-        transform: List[TransformationMeta] = None,
+        transform: list[TransformationMeta] = None,
         chunk_dims: int = 2,
     ):
         """Make a tiled image array filled with zeros.
         Chunk size is inferred from tile shape.
 
         Parameters
         ----------
@@ -928,15 +1027,15 @@
             Name of the array.
         grid_shape : tuple[int, int]
             2-tuple of the tiling grid shape (rows, columns).
         tile_shape : tuple[int]
             Shape of each tile (up to 5D).
         dtype : DTypeLike
             Data type in NumPy convention
-        transform : List[TransformationMeta], optional
+        transform : list[TransformationMeta], optional
             List of coordinate transformations, by default None.
             Should be specified for a non-native resolution level.
         chunk_dims : int, optional
             Non-singleton dimensions of the chunksize,
             by default 2 (chunk by 2D (y, x) tile size).
 
         Returns
@@ -1136,22 +1235,95 @@
         # this node does not have NGFF metadata
         return
 
 
 class Plate(NGFFNode):
     _MEMBER_TYPE = Row
 
+    @classmethod
+    def from_positions(
+        cls,
+        store_path: StrOrBytesPath,
+        positions: dict[str, Position],
+    ) -> Plate:
+        """Create a new HCS store from existing OME-Zarr stores
+        by copying images and metadata from a dictionary of positions.
+
+        .. warning: This assumes same channel names and axes across the FOVs
+            and does not check for consistent shape and chunk size.
+
+        Parameters
+        ----------
+        store_path : StrOrBytesPath
+            Path of the new store
+        positions : dict[str, Position]
+            Dictionary where keys are destination path names ('row/column/fov')
+            and values are :py:class:`iohub.ngff.Position` objects.
+
+        Returns
+        -------
+        Plate
+            New plate with copied data
+
+        Examples
+        --------
+        Combine an HCS-layout store and an FOV-layout store:
+
+        >>> from iohub.ngff import open_ome_zarr, Plate
+
+        >>> with open_ome_zarr("hcs.zarr") as old_plate:
+        >>>     fovs = dict(old_plate.positions())
+
+        >>> with open_ome_zarr("fov.zarr") as old_position:
+        >>>     fovs["Z/1/0"] = old_position
+
+        >>> new_plate = Plate.from_positions("combined.zarr", fovs)
+        """
+        # get metadata from an arbitraty FOV
+        # deterministic because dicts are ordered
+        example_position = next(iter(positions.values()))
+        plate = open_ome_zarr(
+            store_path,
+            layout="hcs",
+            mode="w-",
+            channel_names=example_position.channel_names,
+            axes=example_position.axes,
+            version=example_position.version,
+        )
+        for name, src_pos in positions.items():
+            if not isinstance(src_pos, Position):
+                raise TypeError(
+                    f"Expected item type {type(Position)}, "
+                    f"got {type(src_pos)}"
+                )
+            name = normalize_storage_path(name)
+            if name in plate.zgroup:
+                raise FileExistsError(
+                    f"Duplicate name '{name}' after path normalization."
+                )
+            row, col, fov = name.split("/")
+            _ = plate.create_position(row, col, fov)
+            # overwrite position group
+            _ = zarr.copy_store(
+                src_pos.zgroup.store,
+                plate.zgroup.store,
+                source_path=src_pos.zgroup.name,
+                dest_path=name,
+                if_exists="replace",
+            )
+        return plate
+
     def __init__(
         self,
         group: zarr.Group,
         parse_meta: bool = True,
-        channel_names: List[str] = None,
+        channel_names: list[str] = None,
         axes: list[AxisMeta] = None,
         name: str = None,
-        acquisitions: List[AcquisitionMeta] = None,
+        acquisitions: list[AcquisitionMeta] = None,
         version: Literal["0.1", "0.4"] = "0.4",
         overwriting_creation: bool = False,
     ):
         super().__init__(
             group=group,
             parse_meta=parse_meta,
             channel_names=channel_names,
@@ -1159,16 +1331,14 @@
             version=version,
             overwriting_creation=overwriting_creation,
         )
         self._name = name
         self._acquisitions = (
             [AcquisitionMeta(id=0)] if not acquisitions else acquisitions
         )
-        self._rows = {}
-        self._cols = {}
 
     def _parse_meta(self):
         if plate_meta := self.zattrs.get("plate"):
             logging.debug(f"Loading HCS metadata from file: {plate_meta}")
             self.metadata = PlateMeta(**plate_meta)
         else:
             self._warn_invalid_meta()
@@ -1204,20 +1374,33 @@
             this operation can be expensive if there are many positions,
             by default False
         """
         if field_count:
             self.metadata.field_count = len(list(self.positions()))
         self.zattrs.update({"plate": self.metadata.dict(**TO_DICT_SETTINGS)})
 
-    @staticmethod
-    def _auto_idx(name: str, known: dict[str, int]):
-        if idx := known.get(name):
-            return idx
-        used = known.values()
-        return max(used) + 1 if used else 0
+    def _auto_idx(
+        self,
+        name: "str",
+        index: Union[int, None],
+        axis_name: Literal["row", "column"],
+    ):
+        if index is not None:
+            return index
+        elif not hasattr(self, "metadata"):
+            return 0
+        else:
+            part = ["row", "column"].index(axis_name)
+            all_indices = []
+            for well_index in self.metadata.wells:
+                index = getattr(well_index, f"{axis_name}_index")
+                if well_index.path.split("/")[part] == name:
+                    return index
+                all_indices.append(index)
+            return max(all_indices) + 1
 
     def _build_meta(
         self,
         first_row_meta: PlateAxisMeta,
         first_col_meta: PlateAxisMeta,
         first_well_meta: WellIndexMeta,
     ):
@@ -1261,41 +1444,39 @@
         -------
         Well
             Well node object
         """
         # normalize input
         row_name = normalize_storage_path(row_name)
         col_name = normalize_storage_path(col_name)
-        row_index = self._auto_idx(row_index, self._rows)
-        col_index = self._auto_idx(col_index, self._cols)
+        row_meta = PlateAxisMeta(name=row_name)
+        col_meta = PlateAxisMeta(name=col_name)
+        row_index = self._auto_idx(row_name, row_index, "row")
+        col_index = self._auto_idx(col_name, col_index, "column")
         # build well metadata
         well_index_meta = WellIndexMeta(
-            path='/'.join([row_name, col_name]),
+            path="/".join([row_name, col_name]),
             row_index=row_index,
             column_index=col_index,
         )
-        col_meta = PlateAxisMeta(name=col_name)
+        if not hasattr(self, "metadata"):
+            self._build_meta(row_meta, col_meta, well_index_meta)
+        else:
+            self.metadata.wells.append(well_index_meta)
         # create new row if needed
-        if row_name not in self._rows:
+        if row_name not in self:
             row_grp = self.zgroup.create_group(
-                row_name, overwrite=self._overwrite
+                row_meta.name, overwrite=self._overwrite
             )
-            row_meta = PlateAxisMeta(name=row_name)
-            self._rows[row_name] = row_index
-            if not hasattr(self, "metadata"):
-                self._build_meta(row_meta, col_meta, well_index_meta)
-            else:
+            if row_meta not in self.metadata.rows:
                 self.metadata.rows.append(row_meta)
-                self.metadata.wells.append(well_index_meta)
         else:
-            row_grp = self.zgroup[row_name]
-            self.metadata.wells.append(well_index_meta)
+            row_grp = self[row_name].zgroup
         if col_meta not in self.metadata.columns:
             self.metadata.columns.append(col_meta)
-            self._cols[col_name] = col_index
         # create well
         well_grp = row_grp.create_group(col_name, overwrite=self._overwrite)
         self.dump_meta()
         return Well(group=well_grp, parse_meta=False, **self._child_attrs)
 
     def create_position(
         self,
@@ -1363,15 +1544,15 @@
         [str, Well]
             Path and well object.
         """
         for _, row in self.rows():
             for _, well in row.wells():
                 yield well.zgroup.path, well
 
-    def positions(self):
+    def positions(self) -> Generator[tuple[str, Position], None, None]:
         """Returns a generator that iterate over the path and value
         of all the positions (along rows, columns, and wells) in the plate.
 
         Yields
         ------
         [str, Position]
             Path and position object.
@@ -1381,15 +1562,15 @@
                 yield position.zgroup.path, position
 
 
 def open_ome_zarr(
     store_path: StrOrBytesPath,
     layout: Literal["auto", "fov", "hcs", "tiled"] = "auto",
     mode: Literal["r", "r+", "a", "w", "w-"] = "r",
-    channel_names: List[str] = None,
+    channel_names: list[str] = None,
     axes: list[AxisMeta] = None,
     version: Literal["0.1", "0.4"] = "0.4",
     synchronizer: Union[
         zarr.ThreadSynchronizer, zarr.ProcessSynchronizer
     ] = None,
     **kwargs,
 ):
@@ -1412,15 +1593,15 @@
         Persistence mode:
         'r' means read only (must exist);
         'r+' means read/write (must exist);
         'a' means read/write (create if doesn't exist);
         'w' means create (overwrite if exists);
         'w-' means create (fail if exists),
         by default "r".
-    channel_names : List[str], optional
+    channel_names : list[str], optional
         Channel names used to create a new data store,
         ignored for existing stores,
         by default None
     axes : list[AxisMeta], optional
         OME axes metadata, by default None:
 
         .. code-block:: text
```

### Comparing `iohub-0.1.0.dev3/iohub/ngff_meta.py` & `iohub-0.1.0.dev4/iohub/ngff_meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,40 +4,31 @@
 
 Attributes are 'snake_case' with aliases to match NGFF names in JSON output.
 See https://ngff.openmicroscopy.org/0.4/index.html#naming-style
 about 'camelCase' inconsistency.
 """
 
 import re
-from typing import (
-    Any,
-    ClassVar,
-    Dict,
-    List,
-    Literal,
-    Optional,
-    TypedDict,
-    Union,
-)
+from typing import Any, ClassVar, Literal, Optional, TypedDict, Union
 
 import pandas as pd
 from pydantic import BaseModel, Field, root_validator, validator
 from pydantic.color import Color, ColorType
 
 
 def unique_validator(
-    data: List[Union[BaseModel, TypedDict]], field: Union[str, List[str]]
+    data: list[Union[BaseModel, TypedDict]], field: Union[str, list[str]]
 ):
     """Called by validators to ensure the uniqueness of certain fields.
 
     Parameters
     ----------
-    data : List[Union[BaseModel, TypedDict]]
+    data : list[Union[BaseModel, TypedDict]]
         list of pydantic models or typed dictionaries
-    field : Union[str, List[str]]
+    field : Union[str, list[str]]
         field(s) of the dataclass that must be unique
 
     Raises
     ------
     ValueError
         raised if any value is not unique
     """
@@ -161,16 +152,16 @@
 
 class TransformationMeta(MetaBase):
     """https://ngff.openmicroscopy.org/0.4/index.html#trafo-md"""
 
     # MUST
     type: Literal["identity", "translation", "scale"]
     # MUST? (keyword not found in spec for the fields below)
-    translation: Optional[List[float]] = None
-    scale: Optional[List[float]] = None
+    translation: Optional[list[float]] = None
+    scale: Optional[list[float]] = None
     path: Optional[str] = None
 
     @root_validator
     def no_extra_method(cls, values: dict):
         count = sum([bool(v) for _, v in values.items()])
         if values["type"] == "identity" and count > 1:
             raise ValueError(
@@ -185,15 +176,15 @@
 
 class DatasetMeta(MetaBase):
     """https://ngff.openmicroscopy.org/0.4/index.html#multiscale-md"""
 
     # MUST
     path: str
     # MUST
-    coordinate_transformations: List[TransformationMeta] = Field(
+    coordinate_transformations: list[TransformationMeta] = Field(
         alias="coordinateTransformations"
     )
 
 
 class VersionMeta(MetaBase):
     """OME-NGFF spec version. Default is the current version (0.4)."""
 
@@ -201,21 +192,21 @@
     version: Optional[Literal["0.1", "0.2", "0.3", "0.4"]]
 
 
 class MultiScaleMeta(VersionMeta):
     """https://ngff.openmicroscopy.org/0.4/index.html#multiscale-md"""
 
     # MUST
-    axes: List[AxisMeta]
+    axes: list[AxisMeta]
     # MUST
-    datasets: List[DatasetMeta]
+    datasets: list[DatasetMeta]
     # SHOULD
     name: Optional[str] = None
     # MAY
-    coordinate_transformations: Optional[List[TransformationMeta]] = Field(
+    coordinate_transformations: Optional[list[TransformationMeta]] = Field(
         alias="coordinateTransformations"
     )
     # SHOULD, describes the downscaling method (e.g. 'gaussian')
     type: Optional[str] = None
     # SHOULD, additional information about the downscaling method
     metadata: Optional[dict] = None
 
@@ -263,23 +254,23 @@
 
 
 class OMEROMeta(VersionMeta):
     """https://ngff.openmicroscopy.org/0.4/index.html#omero-md"""
 
     id: int
     name: Optional[str]
-    channels: Optional[List[ChannelMeta]]
+    channels: Optional[list[ChannelMeta]]
     rdefs: Optional[RDefsMeta]
 
 
 class ImagesMeta(MetaBase):
     """Metadata needed for 'Images' (or positions/FOVs) in an OME-NGFF dataset.
     https://ngff.openmicroscopy.org/0.4/index.html#image-layout"""
 
-    multiscales: List[MultiScaleMeta]
+    multiscales: list[MultiScaleMeta]
     omero: OMEROMeta
 
 
 class LabelsMeta(MetaBase):
     """https://ngff.openmicroscopy.org/0.4/index.html#labels-md"""
 
     # SHOULD? (keyword not found in spec)
@@ -301,19 +292,19 @@
         return v
 
 
 class ImageLabelMeta(VersionMeta):
     """https://ngff.openmicroscopy.org/0.4/index.html#label-md"""
 
     # SHOULD
-    colors: List[LabelColorMeta]
+    colors: list[LabelColorMeta]
     # MAY
-    properties: List[Dict[str, Any]]
+    properties: list[dict[str, Any]]
     # MAY
-    source: Dict[str, Any]
+    source: dict[str, Any]
 
     @validator("colors", "properties")
     def unique_label_value(cls, v):
         # MUST
         unique_validator(v, "label_value")
         return v
 
@@ -397,21 +388,21 @@
 class PlateMeta(VersionMeta):
     """OME-NGFF high-content screening plate metadata.
     https://ngff.openmicroscopy.org/0.4/index.html#plate-md"""
 
     # SHOULD
     name: Optional[str]
     # MAY
-    acquisitions: Optional[List[AcquisitionMeta]]
+    acquisitions: Optional[list[AcquisitionMeta]]
     # MUST
-    rows: List[PlateAxisMeta]
+    rows: list[PlateAxisMeta]
     # MUST
-    columns: List[PlateAxisMeta]
+    columns: list[PlateAxisMeta]
     # MUST
-    wells: List[WellIndexMeta]
+    wells: list[WellIndexMeta]
     # SHOULD
     field_count: Optional[int]
 
     @validator("acquisitions")
     def unique_id(cls, v):
         # MUST
         unique_validator(v, "id")
@@ -454,8 +445,8 @@
 
 
 class WellGroupMeta(VersionMeta):
     """OME-NGFF high-content screening well group metadata.
     https://ngff.openmicroscopy.org/0.4/index.html#well-md"""
 
     # MUST
-    images: List[ImageMeta]
+    images: list[ImageMeta]
```

### Comparing `iohub-0.1.0.dev3/iohub/reader.py` & `iohub-0.1.0.dev4/iohub/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,14 +303,15 @@
                     f"Column names:\t {[c.name for c in meta.columns]}",
                     f"Wells:\t\t {len(meta.wells)}",
                 ]
             )
         if verbose:
             msgs.extend(
                 [
+                    f"Positions:\t {len(list(reader.positions()))}",
                     code_msg,
                     ">>> from iohub import open_ome_zarr",
                     f">>> dataset = open_ome_zarr('{path}', mode='r')",
                 ]
             )
         if isinstance(reader, Position) or verbose:
             print("Zarr hierarchy:")
```

### Comparing `iohub-0.1.0.dev3/iohub/reader_base.py` & `iohub-0.1.0.dev4/iohub/reader_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,14 @@
         position : int
             position (aka ome-tiff scene)
 
         Returns
         -------
         NDArray
         """
-        pass
 
     def get_image(self, p: int, t: int, c: int, z: int) -> NDArray:
         """Get the image slice at dimension P, T, C, Z.
 
         Parameters
         ----------
         p : int
```

### Comparing `iohub-0.1.0.dev3/iohub/singlepagetiff.py` & `iohub-0.1.0.dev4/iohub/singlepagetiff.py`

 * *Files identical despite different names*

### Comparing `iohub-0.1.0.dev3/iohub/upti.py` & `iohub-0.1.0.dev4/iohub/upti.py`

 * *Files identical despite different names*

### Comparing `iohub-0.1.0.dev3/iohub/zarrfile.py` & `iohub-0.1.0.dev4/iohub/zarrfile.py`

 * *Files identical despite different names*

### Comparing `iohub-0.1.0.dev3/iohub.egg-info/PKG-INFO` & `iohub-0.1.0.dev4/iohub.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: iohub
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: N-dimensional bioimaging data I/O with OME metadata in Python
-Home-page: https://github.com/czbiohub/iohub
+Home-page: https://github.com/czbiohub-sf/iohub
 Author: CZ Biohub and iohub contributors
 Author-email: iohub@czbiohub.org
 License: BSD 3-Clause License
-Project-URL: Bug Tracker, https://github.com/czbiohub/iohub/issues
-Project-URL: Documentation, https://czbiohub.github.io/iohub
-Project-URL: Source Code, https://github.com/czbiohub/iohub
-Project-URL: User Support, https://github.com/czbiohub/iohub/issues
+Project-URL: Bug Tracker, https://github.com/czbiohub-sf/iohub/issues
+Project-URL: Documentation, https://czbiohub-sf.github.io/iohub
+Project-URL: Source Code, https://github.com/czbiohub-sf/iohub
+Project-URL: User Support, https://github.com/czbiohub-sf/iohub/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Operating System :: Microsoft :: Windows
@@ -34,31 +34,31 @@
 ## Supported formats
 
 ### Read
 
 - OME-Zarr ([OME-NGFF v0.4](https://ngff.openmicroscopy.org/0.4/))
 - Micro-Manager TIFF sequence, OME-TIFF (MMStack), and NDTiff datasets
 - Custom data formats generated by Biohub microscopes
-  - Supported: Falcon (PTI)
-  - WIP: Mantis, Dragonfly, Dorado
+  - Supported: Falcon (PTI), Dorado (ClearControl)
+  - WIP: Mantis, Dragonfly
   - TBA: DaXi
 
 ### Write
 
 - OME-Zarr
 - Multi-page TIFF stacks organized in a directory hierarchy that mimics OME-NGFF (WIP)
 
 ## Quick start
 
 ### Installation
 
 Install iohub with pip:
 
 ```sh
-git clone https://github.com/czbiohub/iohub.git
+git clone https://github.com/czbiohub-sf/iohub.git
 pip install /path/to/iohub
 ```
 
 > For more details about installation, see the [related section in the contribution guide](CONTRIBUTING.md#setting-up-developing-environment).
 
 ### Command-line interface
 
@@ -106,16 +106,16 @@
     )  # creates fov with the same path
     new_fov["0"] = raw_data.max(axis=1).reshape(
         (1, 1, 1, *raw_data.shape[2:])
     )  # max projection along Z axis and prepend dims to 5D
     dataset.print_tree()  # checks that new data has been written
 ```
 
-For more about API usage, refer to the [documentation](https://czbiohub.github.io/iohub/)
-and the [example scripts](https://github.com/czbiohub/iohub/tree/main/examples).
+For more about API usage, refer to the [documentation](https://czbiohub-sf.github.io/iohub/)
+and the [example scripts](https://github.com/czbiohub-sf/iohub/tree/main/examples).
 
 ### Reading Micro-Manager TIFF data
 
 Read a directory containing a TIFF dataset:
 
 ```py
 from iohub import read_micromanager
@@ -125,17 +125,17 @@
 ```
 
 ## Why iohub?
 
 This project is inspired by the existing Python libraries for bioimaging data I/O,
 including [ome-zarr-py](https://github.com/ome/ome-zarr-py), [tifffile](https://github.com/cgohlke/tifffile) and [aicsimageio](https://github.com/AllenCellModeling/aicsimageio).
 They support some of the most widely adopted and/or promising formats in microscopy,
-such as OME-Zarr and OME-Tiff.
+such as OME-Zarr and OME-TIFF.
 
 iohub bridges the gaps among them with the following features:
 
 - Efficient reading of data in various TIFF-based formats produced by the Micro-Manager/Pycro-Manager acquisition stack.
-- Efficient and customizable conversion of data and metadata from Tiff to OME-Zarr.
+- Efficient and customizable conversion of data and metadata from TIFF to OME-Zarr.
 - Pythonic and atomic access of OME-Zarr data with parallelized analysis in mind.
 - OME-Zarr metadata is automatically constructed and updated for writing,
 and verified against the specification when reading.
 - Adherence to the latest OME-NGFF specification (v0.4) whenever possible.
```

### Comparing `iohub-0.1.0.dev3/iohub.egg-info/SOURCES.txt` & `iohub-0.1.0.dev4/iohub.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 .git-blame-ignore-revs
 .gitignore
+.pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/docs.yml
 .github/workflows/pr.yml
 .github/workflows/test.yml
 docs/Makefile
+docs/gh-pages-redirect.html
+docs/examples/README.rst
+docs/examples/run_coordinate_transform.py
+docs/examples/run_large_array_ome_zarr.py
+docs/examples/run_multi_fov_hcs_ome_zarr.py
+docs/examples/run_single_fov_ome_zarr.py
+docs/examples/run_tiled_ome_zarr.py
+docs/examples/run_view_clearcontrol_dataset.py
+docs/source/api.rst
 docs/source/conf.py
+docs/source/contact_us.rst
+docs/source/getting_started.rst
 docs/source/index.rst
+docs/source/_static/switcher.json
+docs/source/api/clearcontrol.rst
 docs/source/api/mm_converter.rst
 docs/source/api/mm_ometiff_reader.rst
 docs/source/api/mm_reader.rst
 docs/source/api/mm_sequence_reader.rst
 docs/source/api/ndtiff.rst
 docs/source/api/ngff.rst
 docs/source/api/upti.rst
-docs/source/contact_us/github.rst
-docs/source/getting_started/install.rst
-docs/source/getting_started/why.rst
-examples/large_array_ome_zarr.py
-examples/multi_fov_hcs_ome_zarr.py
-examples/single_fov_ome_zarr.py
-examples/tiled_ome_zarr.py
 iohub/__init__.py
 iohub/_version.py
+iohub/clearcontrol.py
 iohub/convert.py
 iohub/display_utils.py
+iohub/fov.py
 iohub/multipagetiff.py
 iohub/ndtiff.py
 iohub/ngff.py
 iohub/ngff_meta.py
 iohub/reader.py
 iohub/reader_base.py
 iohub/singlepagetiff.py
@@ -47,17 +56,21 @@
 iohub.egg-info/top_level.txt
 iohub/cli/__init__.py
 iohub/cli/cli.py
 tests/__init__.py
 tests/conftest.py
 tests/test_converter.py
 tests/test_display_utils.py
+tests/clearcontrol/test_clearcontrol.py
 tests/cli/__init__.py
 tests/cli/test_cli.py
+tests/fov/test_fov.py
 tests/ngff/__init__.py
 tests/ngff/test_ngff.py
+tests/pyramid/__init__.py
+tests/pyramid/test_pyramid.py
 tests/reader/__init__.py
 tests/reader/test_multipagetiff.py
 tests/reader/test_pycromanager.py
 tests/reader/test_reader.py
 tests/reader/test_singlepagetiff.py
 tests/reader/test_zarrfile.py
```

### Comparing `iohub-0.1.0.dev3/setup.cfg` & `iohub-0.1.0.dev4/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = iohub
 author = CZ Biohub and iohub contributors
 author_email = iohub@czbiohub.org
-url = https://github.com/czbiohub/iohub
+url = https://github.com/czbiohub-sf/iohub
 license = BSD 3-Clause License
 description = N-dimensional bioimaging data I/O with OME metadata in Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
@@ -14,48 +14,52 @@
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Image Processing
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS :: MacOS X
 project_urls = 
-	Bug Tracker = https://github.com/czbiohub/iohub/issues
-	Documentation = https://czbiohub.github.io/iohub
-	Source Code = https://github.com/czbiohub/iohub
-	User Support = https://github.com/czbiohub/iohub/issues
+	Bug Tracker = https://github.com/czbiohub-sf/iohub/issues
+	Documentation = https://czbiohub-sf.github.io/iohub
+	Source Code = https://github.com/czbiohub-sf/iohub
+	User Support = https://github.com/czbiohub-sf/iohub/issues
 
 [options]
 package = find:
 include_package_data = True
 python_requires = >=3.9
 setup_requires = setuptools_scm
 install_requires = 
 	pandas>=1.5.2
-	pydantic>=1.10.2
+	pydantic>=1.10.2, <2
 	tifffile>=2023.2.3, <2023.3.15
 	natsort>=7.1.1
-	ndtiff>=1.9.0
-	zarr>=2.13
+	ndtiff>=2.1.0
+	zarr>=2.13, <2.16
 	tqdm
 	pillow>=9.4.0
+	blosc2
 
 [options.extras_require]
 dev = 
 	black
 	flake8
 	pytest>=5.0.0
 	pytest-cov
 	hypothesis>=6.61.0
 	requests>=2.22.0
 	wget>=3.2
 	ome-zarr>=0.6.1
 doc = 
+	matplotlib
 	numpydoc==1.1.0
 	sphinx==4.2.0
-	sphinx-rtd-theme==1.2.0
+	pydata-sphinx-theme==0.13.3
 	sphinx-copybutton==0.4.0
 	sphinx-multiversion==0.2.4
+	sphinx-sitemap==2.5.0
+	sphinx-gallery==0.13.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `iohub-0.1.0.dev3/tests/conftest.py` & `iohub-0.1.0.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `iohub-0.1.0.dev3/tests/ngff/test_ngff.py` & `iohub-0.1.0.dev4/tests/ngff/test_ngff.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,34 @@
 import shutil
 import string
 from contextlib import contextmanager
 from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING
 
 import hypothesis.extra.numpy as npst
+import hypothesis.strategies as st
 import pytest
 import zarr
 from hypothesis import HealthCheck, assume, given, settings
-from hypothesis import strategies as st
 from numpy.testing import assert_array_almost_equal
 from numpy.typing import NDArray
 from ome_zarr.io import parse_url
 from ome_zarr.reader import Reader
 
 if TYPE_CHECKING:
     from _typeshed import StrPath
 
-from iohub.ngff import _open_store, _pad_shape, open_ome_zarr
+from iohub.ngff import (
+    TO_DICT_SETTINGS,
+    Plate,
+    TransformationMeta,
+    _open_store,
+    _pad_shape,
+    open_ome_zarr,
+)
 
 short_text_st = st.text(min_size=1, max_size=16)
 t_dim_st = st.integers(1, 4)
 c_dim_st = st.integers(1, 4)
 z_dim_st = st.integers(1, 4)
 y_dim_st = st.integers(1, 32)
 x_dim_st = st.integers(1, 32)
@@ -141,15 +148,17 @@
             store_path, layout="fov", mode="w-", channel_names=channel_names
         )
         assert os.path.isdir(store_path)
         assert dataset.channel_names == channel_names
 
 
 @contextmanager
-def _temp_ome_zarr(image_5d: NDArray, channel_names: list[str], arr_name: str):
+def _temp_ome_zarr(
+    image_5d: NDArray, channel_names: list[str], arr_name: str, **kwargs
+):
     """Helper function to generate a temporary OME-Zarr store.
 
     Parameters
     ----------
     image_5d : NDArray
     channel_names : list[str]
     arr_name : str
@@ -162,15 +171,15 @@
         temp_dir = TemporaryDirectory()
         dataset = open_ome_zarr(
             os.path.join(temp_dir.name, "ome.zarr"),
             layout="fov",
             mode="a",
             channel_names=channel_names,
         )
-        dataset[arr_name] = image_5d
+        dataset.create_image(arr_name, image_5d, **kwargs)
         yield dataset
     finally:
         dataset.close()
         temp_dir.cleanup()
 
 
 @given(
@@ -196,15 +205,19 @@
         assert node.data[0].dtype == random_5d.dtype
 
 
 @given(
     ch_shape_dtype=_channels_and_random_5d_shape_and_dtype(),
     arr_name=short_alpha_numeric,
 )
-@settings(max_examples=16, deadline=2000)
+@settings(
+    max_examples=16,
+    deadline=2000,
+    suppress_health_check=[HealthCheck.data_too_large],
+)
 def test_create_zeros(ch_shape_dtype, arr_name):
     """Test `iohub.ngff.Position.create_zeros()`"""
     channel_names, shape, dtype = ch_shape_dtype
     with TemporaryDirectory() as temp_dir:
         store_path = os.path.join(temp_dir, "ome.zarr")
         dataset = open_ome_zarr(
             store_path, layout="fov", mode="w-", channel_names=channel_names
@@ -216,15 +229,19 @@
         assert dataset[arr_name].dtype == dtype
 
 
 @given(
     channels_and_random_5d=_channels_and_random_5d(),
     arr_name=short_alpha_numeric,
 )
-@settings(max_examples=16, deadline=2000)
+@settings(
+    max_examples=16,
+    deadline=2000,
+    suppress_health_check=[HealthCheck.data_too_large],
+)
 def test_position_data(channels_and_random_5d, arr_name):
     """Test `iohub.ngff.Position.data`"""
     channel_names, random_5d = channels_and_random_5d
     assume(arr_name != "0")
     with _temp_ome_zarr(random_5d, channel_names, "0") as dataset:
         assert_array_almost_equal(dataset.data.numpy(), random_5d)
     with pytest.raises(KeyError):
@@ -312,14 +329,83 @@
     channel_names, random_5d = channels_and_random_5d
     assume(len(channel_names) > 1)
     with pytest.raises(ValueError):
         with _temp_ome_zarr(random_5d, channel_names[:-1], arr_name) as _:
             pass
 
 
+@given(
+    ch_shape_dtype=_channels_and_random_5d_shape_and_dtype(),
+    arr_name=short_alpha_numeric,
+)
+def test_set_transform_image(ch_shape_dtype, arr_name):
+    """Test `iohub.ngff.Position.set_transform()`"""
+    channel_names, shape, dtype = ch_shape_dtype
+    transform = [
+        TransformationMeta(type="translation", translation=(1, 2, 3, 4, 5))
+    ] * len(channel_names)
+    with TemporaryDirectory() as temp_dir:
+        store_path = os.path.join(temp_dir, "ome.zarr")
+        with open_ome_zarr(
+            store_path, layout="fov", mode="w-", channel_names=channel_names
+        ) as dataset:
+            dataset.create_zeros(name=arr_name, shape=shape, dtype=dtype)
+            assert dataset.metadata.multiscales[0].datasets[
+                0
+            ].coordinate_transformations == [
+                TransformationMeta(type="identity")
+            ]
+            dataset.set_transform(image=arr_name, transform=transform)
+            assert (
+                dataset.metadata.multiscales[0]
+                .datasets[0]
+                .coordinate_transformations
+                == transform
+            )
+        # read data with an external reader
+        ext_reader = Reader(parse_url(dataset.zgroup.store.path))
+        node = list(ext_reader())[0]
+        assert node.metadata["coordinateTransformations"][0] == [
+            translate.dict(**TO_DICT_SETTINGS) for translate in transform
+        ]
+
+
+@given(
+    ch_shape_dtype=_channels_and_random_5d_shape_and_dtype(),
+    arr_name=short_alpha_numeric,
+)
+def test_set_transform_fov(ch_shape_dtype, arr_name):
+    """Test `iohub.ngff.Position.set_transform()`"""
+    channel_names, shape, dtype = ch_shape_dtype
+    transform = [
+        TransformationMeta(type="translation", translation=(1, 2, 3, 4, 5))
+    ] * len(channel_names)
+    with TemporaryDirectory() as temp_dir:
+        store_path = os.path.join(temp_dir, "ome.zarr")
+        with open_ome_zarr(
+            store_path, layout="fov", mode="w-", channel_names=channel_names
+        ) as dataset:
+            dataset.create_zeros(name=arr_name, shape=shape, dtype=dtype)
+            assert dataset.metadata.multiscales[
+                0
+            ].coordinate_transformations == [
+                TransformationMeta(type="identity")
+            ]
+            dataset.set_transform(image="*", transform=transform)
+            assert (
+                dataset.metadata.multiscales[0].coordinate_transformations
+                == transform
+            )
+        # read data with plain zarr
+        group = zarr.open(store_path)
+        assert group.attrs["multiscales"][0]["coordinateTransformations"] == [
+            translate.dict(**TO_DICT_SETTINGS) for translate in transform
+        ]
+
+
 @given(channel_names=channel_names_st)
 @settings(max_examples=16)
 def test_create_tiled(channel_names):
     """Test that `iohub.ngff.open_ome_zarr()` can create
     an empty OME-Zarr store with 'tiled' layout."""
     with TemporaryDirectory() as temp_dir:
         store_path = os.path.join(temp_dir, "tiled.zarr")
@@ -468,25 +554,34 @@
     assume(wrong_channel_name != "DAPI")
     with open_ome_zarr(setup_hcs_ref, layout="hcs", mode="r+") as dataset:
         assert dataset.get_channel_index("DAPI") == 0
         with pytest.raises(ValueError):
             _ = dataset.get_channel_index(wrong_channel_name)
 
 
-def test_modify_hcs_ref(setup_test_data, setup_hcs_ref):
+@given(
+    row=short_alpha_numeric, col=short_alpha_numeric, pos=short_alpha_numeric
+)
+@settings(max_examples=16, deadline=2000)
+def test_modify_hcs_ref(setup_test_data, setup_hcs_ref, row, col, pos):
     """Test `iohub.ngff.open_ome_zarr()`"""
     with _temp_copy(setup_hcs_ref) as store_path:
         with open_ome_zarr(store_path, layout="hcs", mode="r+") as dataset:
             assert dataset.axes[0].name == "c"
             assert dataset.channel_names == ["DAPI"]
             position = dataset["B/03/0"]
             assert position[0].shape == (1, 2, 2160, 5120)
             position.append_channel("GFP", resize_arrays=True)
             assert position.channel_names == ["DAPI", "GFP"]
             assert position[0].shape == (2, 2, 2160, 5120)
+            new_pos_path = "/".join([row, col, pos])
+            assume(new_pos_path not in dataset)
+            new_pos = dataset.create_position(row, col, pos)
+            new_pos.create_zeros("0", position[0].shape, position[0].dtype)
+            assert not dataset[f"{new_pos_path}/0"][:].any()
 
 
 @given(row_names=plate_axis_names_st, col_names=plate_axis_names_st)
 @settings(max_examples=16, deadline=2000)
 def test_create_well(row_names: list[str], col_names: list[str]):
     """Test `iohub.ngff.Plate.create_well()`"""
     with TemporaryDirectory() as temp_dir:
@@ -516,7 +611,38 @@
             store_path, layout="hcs", mode="a", channel_names=["GFP"]
         )
         _ = dataset.create_position(row_name=row, col_name=col, pos_name=pos)
         assert [c["name"] for c in dataset.zattrs["plate"]["columns"]] == [col]
         assert [r["name"] for r in dataset.zattrs["plate"]["rows"]] == [row]
         assert os.path.isdir(os.path.join(store_path, row, col, pos))
         assert dataset[row][col].metadata.images[0].path == pos
+
+
+@given(channels_and_random_5d=_channels_and_random_5d())
+def test_position_scale(channels_and_random_5d):
+    """Test `iohub.ngff.Position.scale`"""
+    channel_names, random_5d = channels_and_random_5d
+    scale = list(range(1, 6))
+    transform = [TransformationMeta(type="scale", scale=scale)]
+    with _temp_ome_zarr(
+        random_5d, channel_names, "0", transform=transform
+    ) as dataset:
+        # round-trip test with the offical reader implementation
+        assert dataset.scale == scale
+
+
+def test_combine_fovs_to_hcs(setup_test_data, setup_hcs_ref):
+    fovs = {}
+    fov_paths = ("A/1/0", "B/1/0", "H/12/9")
+    for path in fov_paths:
+        with open_ome_zarr(setup_hcs_ref) as hcs_store:
+            fovs[path] = hcs_store["B/03/0"]
+    with TemporaryDirectory() as temp_dir:
+        store_path = os.path.join(temp_dir, "combined.zarr")
+        combined_plate = Plate.from_positions(store_path, fovs)
+        # read data with an external reader
+        ext_reader = Reader(parse_url(combined_plate.zgroup.store.path))
+        node = list(ext_reader())[0]
+        plate_meta = node.metadata["metadata"]["plate"]
+        assert len(plate_meta["rows"]) == 3
+        assert len(plate_meta["columns"]) == 2
+        assert node.data[0].shape == (1, 2, 2160 * 3, 5120 * 2)
```

### Comparing `iohub-0.1.0.dev3/tests/reader/test_multipagetiff.py` & `iohub-0.1.0.dev4/tests/reader/test_multipagetiff.py`

 * *Files identical despite different names*

### Comparing `iohub-0.1.0.dev3/tests/reader/test_pycromanager.py` & `iohub-0.1.0.dev4/tests/reader/test_pycromanager.py`

 * *Files identical despite different names*

### Comparing `iohub-0.1.0.dev3/tests/reader/test_reader.py` & `iohub-0.1.0.dev4/tests/reader/test_reader.py`

 * *Files identical despite different names*

### Comparing `iohub-0.1.0.dev3/tests/reader/test_singlepagetiff.py` & `iohub-0.1.0.dev4/tests/reader/test_singlepagetiff.py`

 * *Files identical despite different names*

### Comparing `iohub-0.1.0.dev3/tests/reader/test_zarrfile.py` & `iohub-0.1.0.dev4/tests/reader/test_zarrfile.py`

 * *Files identical despite different names*

### Comparing `iohub-0.1.0.dev3/tests/test_display_utils.py` & `iohub-0.1.0.dev4/tests/test_display_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import numpy as np
-
 from iohub.display_utils import channel_display_settings
 
 
 def test_channel_display_settings():
     """Test if channel name exists in dictonary, then assigns a color"""
     channel_name = "GFP"
     channel_meta = channel_display_settings(channel_name)
     assert channel_meta.color == "00FF00"
+    channel_name = "GFP EX488 EM525-45"
+    channel_meta = channel_display_settings(channel_name)
+    assert channel_meta.color == "00FF00"
     channel_name = "S0"
     channel_meta = channel_display_settings(channel_name)
     assert channel_meta.color == "FFFFFF"
     channel_name = "TXR"
     channel_meta = channel_display_settings(channel_name)
     assert channel_meta.color == "FF00FF"
     channel_name = "RANDOM_CHANNEL"
```

