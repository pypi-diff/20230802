# Comparing `tmp/emda-1.1.5.tar.gz` & `tmp/emda-1.1.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/emda-1.1.5.tar", last modified: Thu Aug 18 12:24:00 2022, max compression
+gzip compressed data, was "emda-1.1.6.post1.tar", last modified: Wed Aug  2 17:44:02 2023, max compression
```

## Comparing `emda-1.1.5.tar` & `emda-1.1.6.post1.tar`

### file list

```diff
@@ -1,86 +1,84 @@
-drwxr-xr-x   0 ranganaw   (501) staff       (20)        0 2022-08-18 12:24:00.735596 emda-1.1.5/
--rw-r--r--   0 ranganaw   (501) staff       (20)      685 2022-08-18 12:24:00.735145 emda-1.1.5/PKG-INFO
--rw-r--r--   0 ranganaw   (501) staff       (20)     1705 2022-03-11 09:36:25.000000 emda-1.1.5/README.txt
-drwxr-xr-x   0 ranganaw   (501) staff       (20)        0 2022-08-18 12:24:00.667288 emda-1.1.5/emda/
--rw-r--r--   0 ranganaw   (501) staff       (20)      270 2022-03-11 09:36:25.000000 emda-1.1.5/emda/__init__.py
--rw-r--r--   0 ranganaw   (501) staff       (20)      326 2022-08-18 12:22:12.000000 emda-1.1.5/emda/config.py
-drwxr-xr-x   0 ranganaw   (501) staff       (20)        0 2022-08-18 12:24:00.687753 emda-1.1.5/emda/core/
--rw-r--r--   0 ranganaw   (501) staff       (20)      267 2022-03-10 16:56:49.000000 emda-1.1.5/emda/core/__init__.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     2371 2022-03-10 16:56:49.000000 emda-1.1.5/emda/core/fsc.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    28109 2022-03-14 14:38:11.000000 emda-1.1.5/emda/core/iotools.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     5140 2022-03-10 16:56:49.000000 emda-1.1.5/emda/core/maptools.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     1322 2022-03-10 16:56:49.000000 emda-1.1.5/emda/core/modeltools.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     5709 2022-03-10 16:56:49.000000 emda-1.1.5/emda/core/mtz.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     9840 2022-03-10 16:56:49.000000 emda-1.1.5/emda/core/plotter.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     6902 2022-03-10 16:56:49.000000 emda-1.1.5/emda/core/quaternions.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     7538 2022-03-10 16:56:49.000000 emda-1.1.5/emda/core/restools.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    47292 2022-08-18 12:14:11.000000 emda-1.1.5/emda/emda_cmd_caller.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    83354 2022-08-18 12:16:23.000000 emda-1.1.5/emda/emda_methods.py
--rw-r--r--   0 ranganaw   (501) staff       (20)      470 2022-03-10 16:56:50.000000 emda-1.1.5/emda/emda_test.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     3457 2022-03-10 16:56:50.000000 emda-1.1.5/emda/emda_test_exhaust.py
-drwxr-xr-x   0 ranganaw   (501) staff       (20)        0 2022-08-18 12:24:00.713646 emda-1.1.5/emda/ext/
--rw-r--r--   0 ranganaw   (501) staff       (20)      202 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/__init__.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    17316 2022-08-17 16:12:48.000000 emda-1.1.5/emda/ext/atomic_cc.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    20609 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/axis_refinement.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     2464 2022-08-17 13:40:28.000000 emda-1.1.5/emda/ext/bestmap.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     1364 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/cc.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     3704 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/composite.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     2574 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/difference.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     7294 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/diffmap_snr.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    14567 2022-07-01 06:09:05.000000 emda-1.1.5/emda/ext/diffmap_with_fit.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     8126 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/downmap.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     1080 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/fakehalf.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     3554 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/fouriersp_local.py
--rw-r--r--   0 ranganaw   (501) staff       (20)      575 2022-08-16 11:24:47.000000 emda-1.1.5/emda/ext/half2full.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    16121 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/likelihood_map.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     1500 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/lowpass_map.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    15721 2022-08-15 11:10:04.000000 emda-1.1.5/emda/ext/magnification.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    19336 2022-08-03 19:41:23.000000 emda-1.1.5/emda/ext/magnification_new.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    15770 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/map_fsc.py
-drwxr-xr-x   0 ranganaw   (501) staff       (20)        0 2022-08-18 12:24:00.727278 emda-1.1.5/emda/ext/mapfit/
--rw-r--r--   0 ranganaw   (501) staff       (20)      207 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/__init__.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     3082 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/curve_fit_3.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     7944 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/derivatives.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    11854 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/emfit_class.py
--rw-r--r--   0 ranganaw   (501) staff       (20)      932 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/frequency_marching.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     1025 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/interp_derivatives.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     4905 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/linefit_class.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    51660 2022-08-18 11:28:44.000000 emda-1.1.5/emda/ext/mapfit/map_class.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     7382 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/mapaverage.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     6142 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/mapoverlay.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    22151 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/newsignal.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     1748 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/rdp_algo.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     1807 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/rotmat2quart.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     6786 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/run_fit.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    24892 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/mapfit/utils.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    10521 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/maskmap_class.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    42705 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/overlay.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    43248 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/overlay_dev.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    38939 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/overlay_x.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     6063 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/phase_randomize.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     5805 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/qq_plot.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    21352 2022-08-17 19:12:10.000000 emda-1.1.5/emda/ext/realsp_local.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     9495 2022-08-16 06:28:54.000000 emda-1.1.5/emda/ext/rebox_map.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     3344 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/scale_maps.py
-drwxr-xr-x   0 ranganaw   (501) staff       (20)        0 2022-08-18 12:24:00.734525 emda-1.1.5/emda/ext/sym/
--rw-r--r--   0 ranganaw   (501) staff       (20)    38905 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/sym/GenerateOperators_v9_ky4.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    39995 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/sym/GenerateOperators_v9_ky5.py
--rw-r--r--   0 ranganaw   (501) staff       (20)      202 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/sym/__init__.py
--rw-r--r--   0 ranganaw   (501) staff       (20)    51973 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/sym/refine_symaxis.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     4996 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/sym/run_proshade.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     3364 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/sym/symmetrize_map.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     7487 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/sym/symmetry.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     4831 2022-03-10 16:56:49.000000 emda-1.1.5/emda/ext/transform_map.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     3329 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/utils.py
--rw-r--r--   0 ranganaw   (501) staff       (20)     2212 2022-03-10 16:56:50.000000 emda-1.1.5/emda/ext/xmlclass.py
--rw-r--r--   0 ranganaw   (501) staff       (20)   143039 2022-07-28 13:40:47.000000 emda-1.1.5/emda/fcodes_fast.f90
-drwxr-xr-x   0 ranganaw   (501) staff       (20)        0 2022-08-18 12:24:00.680501 emda-1.1.5/emda.egg-info/
--rw-r--r--   0 ranganaw   (501) staff       (20)      685 2022-08-18 12:24:00.000000 emda-1.1.5/emda.egg-info/PKG-INFO
--rw-r--r--   0 ranganaw   (501) staff       (20)     1929 2022-08-18 12:24:00.000000 emda-1.1.5/emda.egg-info/SOURCES.txt
--rw-r--r--   0 ranganaw   (501) staff       (20)        1 2022-08-18 12:24:00.000000 emda-1.1.5/emda.egg-info/dependency_links.txt
--rw-r--r--   0 ranganaw   (501) staff       (20)      132 2022-08-18 12:24:00.000000 emda-1.1.5/emda.egg-info/entry_points.txt
--rw-r--r--   0 ranganaw   (501) staff       (20)        1 2022-03-14 13:41:23.000000 emda-1.1.5/emda.egg-info/not-zip-safe
--rw-r--r--   0 ranganaw   (501) staff       (20)       71 2022-08-18 12:24:00.000000 emda-1.1.5/emda.egg-info/requires.txt
--rw-r--r--   0 ranganaw   (501) staff       (20)       17 2022-08-18 12:24:00.000000 emda-1.1.5/emda.egg-info/top_level.txt
--rw-r--r--   0 ranganaw   (501) staff       (20)       38 2022-08-18 12:24:00.735830 emda-1.1.5/setup.cfg
--rw-r--r--   0 ranganaw   (501) staff       (20)     1464 2022-03-14 13:40:58.000000 emda-1.1.5/setup.py
+drwxr-xr-x   0 Rangana    (501) staff       (20)        0 2023-08-02 17:44:02.479799 emda-1.1.6.post1/
+-rw-r--r--   0 Rangana    (501) staff       (20)    16725 2023-04-26 07:24:22.000000 emda-1.1.6.post1/LICENSE.txt
+-rw-r--r--   0 Rangana    (501) staff       (20)      663 2023-08-02 17:44:02.479065 emda-1.1.6.post1/PKG-INFO
+-rw-r--r--   0 Rangana    (501) staff       (20)     1748 2023-08-02 17:42:29.000000 emda-1.1.6.post1/README.txt
+drwxr-xr-x   0 Rangana    (501) staff       (20)        0 2023-08-02 17:44:02.114836 emda-1.1.6.post1/emda/
+-rw-r--r--   0 Rangana    (501) staff       (20)      270 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/__init__.py
+-rw-r--r--   0 Rangana    (501) staff       (20)      332 2023-08-02 17:37:19.000000 emda-1.1.6.post1/emda/config.py
+drwxr-xr-x   0 Rangana    (501) staff       (20)        0 2023-08-02 17:44:02.239620 emda-1.1.6.post1/emda/core/
+-rw-r--r--   0 Rangana    (501) staff       (20)      267 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/core/__init__.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     2371 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/core/fsc.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    28121 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/core/iotools.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     5140 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/core/maptools.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     1322 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/core/modeltools.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     5709 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/core/mtz.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     9828 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/core/plotter.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     6902 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/core/quaternions.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     7538 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/core/restools.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    47286 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/emda_cmd_caller.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    83354 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/emda_methods.py
+-rw-r--r--   0 Rangana    (501) staff       (20)      470 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/emda_test.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     3457 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/emda_test_exhaust.py
+drwxr-xr-x   0 Rangana    (501) staff       (20)        0 2023-08-02 17:44:02.389793 emda-1.1.6.post1/emda/ext/
+-rw-r--r--   0 Rangana    (501) staff       (20)      202 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/__init__.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    17316 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/atomic_cc.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    20609 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/axis_refinement.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     2464 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/bestmap.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     1364 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/cc.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     3704 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/composite.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     2574 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/difference.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     7294 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/diffmap_snr.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    14567 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/diffmap_with_fit.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     8836 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/downmap.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     1080 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/fakehalf.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     3554 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/fouriersp_local.py
+-rw-r--r--   0 Rangana    (501) staff       (20)      575 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/half2full.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    15718 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/likelihood_map.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     1500 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/lowpass_map.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    15721 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/magnification.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    15770 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/map_fsc.py
+drwxr-xr-x   0 Rangana    (501) staff       (20)        0 2023-08-02 17:44:02.445751 emda-1.1.6.post1/emda/ext/mapfit/
+-rw-r--r--   0 Rangana    (501) staff       (20)      207 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/__init__.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     3082 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/curve_fit_3.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     7944 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/derivatives.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    11854 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/emfit_class.py
+-rw-r--r--   0 Rangana    (501) staff       (20)      932 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/frequency_marching.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     1025 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/interp_derivatives.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     4905 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/linefit_class.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    51660 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/map_class.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     6863 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/mapaverage.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     6142 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/mapoverlay.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    22058 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/newsignal.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     1748 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/rdp_algo.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     1807 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/rotmat2quart.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     6786 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/run_fit.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    24892 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/mapfit/utils.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    10521 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/maskmap_class.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    42731 2023-05-17 15:55:34.000000 emda-1.1.6.post1/emda/ext/overlay.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     6063 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/phase_randomize.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     5805 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/qq_plot.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    21393 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/realsp_local.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     9495 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/rebox_map.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     3344 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/scale_maps.py
+drwxr-xr-x   0 Rangana    (501) staff       (20)        0 2023-08-02 17:44:02.477056 emda-1.1.6.post1/emda/ext/sym/
+-rw-r--r--   0 Rangana    (501) staff       (20)    38905 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/sym/GenerateOperators_v9_ky4.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    39995 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/sym/GenerateOperators_v9_ky5.py
+-rw-r--r--   0 Rangana    (501) staff       (20)      202 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/sym/__init__.py
+-rw-r--r--   0 Rangana    (501) staff       (20)    49473 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/sym/refine_symaxis.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     4996 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/sym/run_proshade.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     3364 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/sym/symmetrize_map.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     7487 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/sym/symmetry.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     4831 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/transform_map.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     3329 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/utils.py
+-rw-r--r--   0 Rangana    (501) staff       (20)     2212 2023-04-26 07:24:22.000000 emda-1.1.6.post1/emda/ext/xmlclass.py
+-rw-r--r--   0 Rangana    (501) staff       (20)   143195 2023-05-17 15:49:22.000000 emda-1.1.6.post1/emda/fcodes_fast.f90
+drwxr-xr-x   0 Rangana    (501) staff       (20)        0 2023-08-02 17:44:02.146395 emda-1.1.6.post1/emda.egg-info/
+-rw-r--r--   0 Rangana    (501) staff       (20)      663 2023-08-02 17:44:01.000000 emda-1.1.6.post1/emda.egg-info/PKG-INFO
+-rw-r--r--   0 Rangana    (501) staff       (20)     1865 2023-08-02 17:44:01.000000 emda-1.1.6.post1/emda.egg-info/SOURCES.txt
+-rw-r--r--   0 Rangana    (501) staff       (20)        1 2023-08-02 17:44:01.000000 emda-1.1.6.post1/emda.egg-info/dependency_links.txt
+-rw-r--r--   0 Rangana    (501) staff       (20)      131 2023-08-02 17:44:01.000000 emda-1.1.6.post1/emda.egg-info/entry_points.txt
+-rw-r--r--   0 Rangana    (501) staff       (20)        1 2023-05-17 15:44:19.000000 emda-1.1.6.post1/emda.egg-info/not-zip-safe
+-rw-r--r--   0 Rangana    (501) staff       (20)       69 2023-08-02 17:44:01.000000 emda-1.1.6.post1/emda.egg-info/requires.txt
+-rw-r--r--   0 Rangana    (501) staff       (20)       17 2023-08-02 17:44:01.000000 emda-1.1.6.post1/emda.egg-info/top_level.txt
+-rw-r--r--   0 Rangana    (501) staff       (20)       38 2023-08-02 17:44:02.479976 emda-1.1.6.post1/setup.cfg
+-rw-r--r--   0 Rangana    (501) staff       (20)     1459 2023-08-02 17:33:34.000000 emda-1.1.6.post1/setup.py
```

### Comparing `emda-1.1.5/PKG-INFO` & `emda-1.1.6.post1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: emda
-Version: 1.1.5
+Version: 1.1.6.post1
 Summary: Electron Microscopy map and model manipulation tools
 Home-page: https://www2.mrc-lmb.cam.ac.uk/groups/murshudov/content/emda/emda.html
 Author: Rangana Warshamanage, Garib N. Murshudov
 Author-email: ranganaw@mrc-lmb.cam.ac.uk, garib@mrc-lmb.cam.ac.uk
 License: MPL-2.0
-Description:         Python library for Electron Microscopy Data Analysis (EMDA). 
-                EMDA supports MRC/CCP4.MAP and MTZ files as well as PDB and mmcif files. 
-                EMDA offeres a range of functions for downstream data analysis and
-                model building. Please refer emda.readthedocs.io for more information.
-Platform: UNKNOWN
+License-File: LICENSE.txt
+
+        Python library for Electron Microscopy Data Analysis (EMDA). 
+        EMDA supports MRC/CCP4.MAP and MTZ files as well as PDB and mmcif files. 
+        EMDA offeres a range of functions for downstream data analysis and
+        model building. Please refer emda.readthedocs.io for more information.
```

### Comparing `emda-1.1.5/README.txt` & `emda-1.1.6.post1/README.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-EMDA version 1.1.3
+EMDA version 1.1.6
 ===================
 
 EMDA is an importable Python library for Electron Microscopy map and model manipulations written in Python3.
 EMDA comes under MPL-2.0 license. 
 
 A selected set of EMDA’s core functionalities include:
 
@@ -24,15 +24,15 @@
 gemmi
 mrcfile
 matplotlib
 All dependencies will be automatically checked and installed, if necessary during
 EMDA installation.
 
 
-Installing EMDA version 1.1.3 
+Installing EMDA version 1.1.6 
 ===============================
 
 For installation you may need administrator permissions, 
 please consult your system administrator if needed.
 
 
 Installing from source
@@ -44,25 +44,31 @@
 After installation, you may check the installation by typing
 'emda_test' on your terminal. All tests must pass.
 
 
 License
 =======
 
-EMDA-1.1.2 comes under Mozilla Public License Version 2.0 licence.
+EMDA-1.1.6 comes under Mozilla Public License Version 2.0 licence.
 Please look at LICENSE.txt for more details.
 
 
 Citations
 =========
 
-Please contact authors: ranganaw@mrc-lmb.cam.ac.uk,
+Journal of Structural Biology 214 (2022) 107826
+
+
+Queries
+=======
+
+ranganaw@mrc-lmb.cam.ac.uk,
 garib@mrc-lmb.cam.ac.uk
 
 
 Acknowledgments
 ===============
 
 Wellcome Trust- Validation tools for Cryo EM grant (208398/Z/17/Z)
 
-This README file was last time modified on 02.09.2020
+This README file was last time modified on 02.08.2023
```

### Comparing `emda-1.1.5/emda/core/fsc.py` & `emda-1.1.6.post1/emda/core/fsc.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/core/iotools.py` & `emda-1.1.6.post1/emda/core/iotools.py`

 * *Files 1% similar despite different names*

```diff
@@ -769,9 +769,9 @@
         comoffset[1] = float(com.y) - mapcom[1]
         comoffset[2] = float(com.x) - mapcom[2]
         trans += comoffset """ 
     t = gemmi.Vec3(trans[2], trans[1], trans[0]) # ZYX --> XYZ
     mat33 = gemmi.Mat33(rotmat)
     trans = com - mat33.multiply(com) + t
     tr = gemmi.Transform(mat33, trans)
-    st[0].transform(tr)
+    st[0].transform_pos_and_adp(tr)
     st.make_mmcif_document().write_file(outfilename)
```

### Comparing `emda-1.1.5/emda/core/maptools.py` & `emda-1.1.6.post1/emda/core/maptools.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/core/modeltools.py` & `emda-1.1.6.post1/emda/core/modeltools.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/core/mtz.py` & `emda-1.1.6.post1/emda/core/mtz.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/core/plotter.py` & `emda-1.1.6.post1/emda/core/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     for icurve in range(len(list_arr)):
         data = list_arr[icurve]
         if curve_label is None:
             label = "Set#" + str(icurve)
             ax1.plot(bin_arr, np.log10(data), label=label, linewidth=2)
         else:
             ax1.plot(bin_arr, np.log10(data), label=curve_label[icurve], linewidth=2)
-    pos = np.array(ax1.get_xticks(), dtype=np.int)
+    pos = np.array(ax1.get_xticks(), dtype=int)
     n_bins = res_arr.shape[0]
     pos[pos < 0] = 0
     pos[pos >= n_bins] = n_bins - 1
     ax1.set_xticklabels(np.round(res_arr[pos], decimals=2))
     ax1.set_xlabel(xlabel)
     plt.ylabel(ylabel)
     #ax1.set_ylim([-2, 6])
@@ -81,15 +81,15 @@
     bin_arr = np.arange(len(res_arr))
     fig = plt.figure(figsize=(6, 4))
     ax1 = fig.add_subplot(111)
     ax1.plot(bin_arr, arr, linewidth=2)
     xmin = np.min(bin_arr)
     xmax = np.max(bin_arr)
     # plt.plot((xmin, xmax), (0.143, 0.143), 'k--')
-    pos = np.array(ax1.get_xticks(), dtype=np.int)
+    pos = np.array(ax1.get_xticks(), dtype=int)
     n_bins = res_arr.shape[0]
     pos[pos < 0] = 0
     pos[pos >= n_bins] = n_bins - 1
     ax1.set_xticklabels(np.round(res_arr[pos], decimals=2))
     ax1.set_xlabel("Resolution ($\AA$)")
     plt.ylabel("Fourier Shell Correlation")
     font = {"family": "serif", "color": "black", "weight": "bold", "size": 16}
@@ -118,15 +118,15 @@
         ax1.plot(bin_arr, list_arr[icurve], label=curve_label[icurve], linewidth=2)
     xmin = np.min(bin_arr)
     xmax = np.max(bin_arr)
     plt.plot(
         (xmin, xmax), (float(fscline), float(fscline)), color="gray", linestyle=":"
     )
     plt.plot((xmin, xmax), (0.0, 0.0), color="black", linestyle=":")
-    pos = np.array(ax1.get_xticks(), dtype=np.int)
+    pos = np.array(ax1.get_xticks(), dtype=int)
     n_bins = res_arr.shape[0]
     pos[pos < 0] = 0
     pos[pos >= n_bins] = n_bins - 1
     #
     import matplotlib.ticker as mticker
     label_format = '{:5.2f}'
     ax1.xaxis.set_major_locator(mticker.FixedLocator(pos))
@@ -157,15 +157,15 @@
     ax1 = fig.add_subplot(111)
     for icurve in range(len(list_arr)):
         ax1.plot(bin_arr, list_arr[icurve], label=curve_label[icurve], linewidth=2)
     xmin = np.min(bin_arr)
     xmax = np.max(bin_arr)
     plt.plot((xmin, xmax), (0.5, 0.5), "k--")
 
-    pos = np.array(ax1.get_xticks(), dtype=np.int)
+    pos = np.array(ax1.get_xticks(), dtype=int)
     n_bins = res_arr.shape[0]
     pos[pos < 0] = 0
     pos[pos >= n_bins] = n_bins - 1
     ax1.set_xticklabels(np.round(res_arr[pos], decimals=2))
     ax1.set_xlabel("Resolution (1/$\AA$)")
     plt.legend(loc=0)
     plt.ylabel("Fourier Shell Correlation")
```

### Comparing `emda-1.1.5/emda/core/quaternions.py` & `emda-1.1.6.post1/emda/core/quaternions.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/core/restools.py` & `emda-1.1.6.post1/emda/core/restools.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/emda_cmd_caller.py` & `emda-1.1.6.post1/emda/emda_cmd_caller.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
     help="target pixel size (A)"
 )
 resample_d.add_argument(
     "--dim",
     required=False,
     default=None,
     nargs="+",
-    type=np.int,
+    type=int,
     help="target map dimensions. e.g. 100 100 100 ",
 )
 resample_d.add_argument(
     "--cel",
     required=False,
     default=None,
     nargs="+",
@@ -617,15 +617,15 @@
 
 model2map = subparsers.add_parser(
     "model2map", description="calculate model based map")
 model2map.add_argument("--mdl", required=True, help="input atomic model")
 model2map.add_argument("--res", required=True,
                        type=float, help="Resolution (A)")
 model2map.add_argument("--dim", required=True, nargs="+",
-                       type=np.int, help="map dim ")
+                       type=int, help="map dim ")
 model2map.add_argument(
     "--cel", required=True, nargs="+", type=np.float, help="cell parameters "
 )
 model2map.add_argument(
     "--lgf", required=False, default=None, type=str, help="ligand description file"
 )
 model2map.add_argument(
```

### Comparing `emda-1.1.5/emda/emda_methods.py` & `emda-1.1.6.post1/emda/emda_methods.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/emda_test_exhaust.py` & `emda-1.1.6.post1/emda/emda_test_exhaust.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/atomic_cc.py` & `emda-1.1.6.post1/emda/ext/atomic_cc.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/axis_refinement.py` & `emda-1.1.6.post1/emda/ext/axis_refinement.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/bestmap.py` & `emda-1.1.6.post1/emda/ext/bestmap.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/cc.py` & `emda-1.1.6.post1/emda/ext/cc.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/composite.py` & `emda-1.1.6.post1/emda/ext/composite.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/difference.py` & `emda-1.1.6.post1/emda/ext/difference.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/diffmap_snr.py` & `emda-1.1.6.post1/emda/ext/diffmap_snr.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/diffmap_with_fit.py` & `emda-1.1.6.post1/emda/ext/diffmap_with_fit.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/downmap.py` & `emda-1.1.6.post1/emda/ext/downmap.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,67 @@
-import os, gzip, shutil
-import urllib.request
+"""
+Author: "Rangana Warshamanage, Garib N. Murshudov"
+MRC Laboratory of Molecular Biology
+    
+This software is released under the
+Mozilla Public License, version 2.0; see LICENSE.
+"""
+
+# download data from EMDB
+
+from __future__ import absolute_import, division, print_function, unicode_literals
+import os, gzip, shutil, io
+#import urllib.request
 from contextlib import closing
 import xml.etree.ElementTree as ET
 
+try:
+    from urllib.request import urlopen
+except:
+    from urllib import urlopen
 
 def fetch_data(emdbid):
+    emdbid = emdbid.strip()
     headerxml = (
         "ftp://ftp.ebi.ac.uk/pub/databases/emdb/structures/EMD-%s/header/emd-%s.xml"
         % (emdbid, emdbid)
     )
-    header30xml = (
-        "ftp://ftp.ebi.ac.uk/pub/databases/emdb/structures/EMD-%s/header/emd%s-v30.xml"
-        % (emdbid, emdbid)
-    )
+    outmap = None
+    outcif = None
+    model = None
+    claimed_resol = None
 
-    outmap = None; outcif = None; claimed_resol = None
+    print(emdbid)
 
-    with closing(urllib.request.urlopen(headerxml)) as r:
+    #with closing(urllib.request.urlopen(headerxml)) as r:
+    with closing(urlopen(headerxml)) as r:
         with open("file.xml", "wb") as f:
             shutil.copyfileobj(r, f)
 
     tree = ET.parse("file.xml")
     root = tree.getroot()
 
-    model = None
-    for deposition in root.findall("deposition"):
-        for fittedPDBEntryIdList in deposition.findall("fittedPDBEntryIdList"):
-            for fittedPDBEntryId in fittedPDBEntryIdList.findall("fittedPDBEntryId"):
-                model = fittedPDBEntryId.text
-
-    for processing in root.findall("processing"):
-        for reconstruction in processing.findall("reconstruction"):
-            for resolutionByAuthor in reconstruction.findall("resolutionByAuthor"):
-                claimed_resol = resolutionByAuthor.text
+    for crossreferences in root.findall("crossreferences"):
+        for pdb_list in crossreferences.findall("pdb_list"):
+            for pdb_reference in pdb_list.findall("pdb_reference"):
+                for pdb_id in pdb_reference.findall("pdb_id"):
+                    model = pdb_id.text
+
+    if model is not None:
+        print(model)
+
+    for structure_determination_list in root.findall("structure_determination_list"):
+        for structure_determination in structure_determination_list.findall("structure_determination"):
+            for singleparticle_processing in structure_determination.findall("singleparticle_processing"):
+                for final_reconstruction in singleparticle_processing.findall("final_reconstruction"):
+                    for resolution in final_reconstruction.findall("resolution"):
+                        claimed_resol = resolution.text
+    print('Resolution: ', claimed_resol)
 
     # create a directory with EMDBID
-    #path = "/Users/sandy/MRC/REFMAC/COVID19/EMD-%s/" % (emdbid)
     path = os.getcwd() + "/EMD-%s/" % (emdbid)
     try:
         os.mkdir(path)
     except OSError:
         if os.path.isdir(path):
             print("Directory exists!")
         else:
@@ -52,59 +74,51 @@
             cifftplink = "ftp://ftp.ebi.ac.uk/pub/databases/pdb/data/structures/all/mmCIF/{}.cif.gz".format(
                 model
             )
             outcif = "%s.cif" % (model)
         except Exception as e:
             print(e)
         try:
-            with urllib.request.urlopen(cifftplink) as response:
+            #with urllib.request.urlopen(cifftplink) as response:
+            with urlopen(cifftplink) as response:
                 with gzip.GzipFile(fileobj=response) as uncompressed:
                     file_content = uncompressed.read()
             with open(path + outcif, "wb") as f:
                 f.write(file_content)
         except Exception as e:
             print(e)
     mapftplink = (
         "ftp://ftp.ebi.ac.uk/pub/databases/emdb/structures/EMD-%s/map/emd_%s.map.gz"
         % (emdbid, emdbid)
     )
 
     outmap = "emd_%s.map" % (emdbid)
     try:
-        with urllib.request.urlopen(mapftplink) as response:
+        #with urllib.request.urlopen(mapftplink) as response:
+        with urlopen(mapftplink) as response:
             with gzip.GzipFile(fileobj=response) as uncompressed:
                 file_content = uncompressed.read()
         with open(path + outmap, "wb") as f:
             f.write(file_content)
     except Exception as e:
         print(e)
 
 
 def fetch_all_data(emdid):
     name_list = []
     headerxml = (
         "ftp://ftp.ebi.ac.uk/pub/databases/emdb/structures/EMD-%s/header/emd-%s.xml"
         % (emdid, emdid)
     )
-    header30xml = (
-        "ftp://ftp.ebi.ac.uk/pub/databases/emdb/structures/EMD-%s/header/emd-%s-v30.xml"
-        % (emdid, emdid)
-    )
-    with closing(urllib.request.urlopen(headerxml)) as r:
+    with closing(urlopen(headerxml)) as r:
         with open("file.xml", "wb") as f:
             shutil.copyfileobj(r, f)
     tree1 = ET.parse("file.xml")
     root1 = tree1.getroot()
-
-    with closing(urllib.request.urlopen(header30xml)) as r:
-        with open("file30.xml", "wb") as f:
-            shutil.copyfileobj(r, f)
-    tree2 = ET.parse("file30.xml")
-    root2 = tree2.getroot()
-    
+    root = root1
     path = os.getcwd() + "/EMD-%s/" % (emdid)
     try:
         os.mkdir(path)
     except OSError:
         if os.path.isdir(path):
             print("Directory exists!")
         else:
@@ -113,99 +127,104 @@
         print("Successfully created the directory %s " % path)
 
     model = None
     maskid = None
     half1id = None
     half2id = None
     claimed_resol = None
-    mapname = None
-    maskname = None
-    half1name = None
-    half2name = None
-    modelname = None
-    for deposition in root1.findall("deposition"):
-        for fittedPDBEntryIdList in deposition.findall("fittedPDBEntryIdList"):
-            for fittedPDBEntryId in fittedPDBEntryIdList.findall("fittedPDBEntryId"):
-                model = fittedPDBEntryId.text
-    for map in root1.findall("map"):
-        for file in map.findall("file"):
-            mapid = file.text
-    for processing in root1.findall("processing"):
-        for reconstruction in processing.findall("reconstruction"):
-            for resolutionByAuthor in reconstruction.findall("resolutionByAuthor"):
-                claimed_resol = resolutionByAuthor.text
-    for interpretation in root2.findall("interpretation"):
+
+    for crossreferences in root.findall("crossreferences"):
+        for pdb_list in crossreferences.findall("pdb_list"):
+            for pdb_reference in pdb_list.findall("pdb_reference"):
+                for pdb_id in pdb_reference.findall("pdb_id"):
+                    model = pdb_id.text
+
+    for structure_determination_list in root.findall("structure_determination_list"):
+        for structure_determination in structure_determination_list.findall("structure_determination"):
+            for singleparticle_processing in structure_determination.findall("singleparticle_processing"):
+                for final_reconstruction in singleparticle_processing.findall("final_reconstruction"):
+                    for resolution in final_reconstruction.findall("resolution"):
+                        claimed_resol = resolution.text
+
+    for interpretation in root.findall("interpretation"):
         for segmentation_list in interpretation.findall("segmentation_list"):
             for segmentation in segmentation_list.findall("segmentation"):
                 for file in segmentation.findall("file"):
                     maskid = file.text
+
         for half_map_list in interpretation.findall("half_map_list"):
             for i, half_map in enumerate(half_map_list.findall("half_map")):
                 if i == 0:
                     for file in half_map.findall("file"):
                         half1id = file.text
                 if i == 1:
                     for file in half_map.findall("file"):
                         half2id = file.text
 
+    for map in root.findall("map"):
+        for file in map.findall("file"):
+            mapid = file.text
+
     print("claimed resol ", claimed_resol)
     print("Mask Id: ", maskid)
     print("Half1id: ", half1id)
     print("Half2id: ", half2id)
+
     if model is not None:
         try:
             cifftplink = "ftp://ftp.ebi.ac.uk/pub/databases/pdb/data/structures/all/mmCIF/{}.cif.gz".format(
                 model
             )
             outcif = "%s.cif" % (model)
         except Exception as e:
             print(e)
         try:
-            with urllib.request.urlopen(cifftplink) as response:
+            #with urllib.request.urlopen(cifftplink) as response:
+            with urlopen(cifftplink) as response:
                 with gzip.GzipFile(fileobj=response) as uncompressed:
                     file_content = uncompressed.read()
             with open(path + outcif, "wb") as f:
                 f.write(file_content)
         except Exception as e:
             print(e)
 
     readname_list = []
     writename_list = []
     readname_list.append("EMD-%s/map/%s" % (emdid, mapid))
     writename_list.append("emd_%s.map" % (emdid))
-    mapname = path + "emd_%s.map" % (emdid)
     if maskid is not None:
         readname_list.append("EMD-%s/masks/%s" % (emdid, maskid))
         writename_list.append("emd_%s_mask.map" % (emdid))
-        maskname = path + "emd_%s_mask.map" % (emdid)
     if half1id is not None:
         readname_list.append("EMD-%s/other/%s" % (emdid, half1id))
-        writename_list.append("emd_%s_half1.map" % (emdid))
-        half1name = path + "emd_%s_half1.map" % (emdid)
+        writename_list.append("emd_%s_half_map_1.map" % (emdid))
         readname_list.append("EMD-%s/other/%s" % (emdid, half2id))
-        writename_list.append("emd_%s_half2.map" % (emdid))
-        half2name = path + "emd_%s_half2.map" % (emdid)
+        writename_list.append("emd_%s_half_map_2.map" % (emdid))
 
     ftplink = (
         "ftp://ftp.ebi.ac.uk/pub/databases/emdb/structures/"
     )
     for readname, writename in zip(readname_list, writename_list):
         name_list.append(path + writename)
         try:
             fid = ftplink+readname
             if fid.endswith((".map")):
-                with closing(urllib.request.urlopen(fid)) as r:
+                #with closing(urllib.request.urlopen(fid)) as r:
+                with closing(urlopen(fid)) as r:
                     with open(path + writename, 'wb') as f:
                         shutil.copyfileobj(r, f)
+                        print('%s was written' %writename)
             elif fid.endswith((".gz")):
-                with urllib.request.urlopen(ftplink+readname) as response:
+                #with urllib.request.urlopen(ftplink+readname) as response:
+                with urlopen(ftplink+readname) as response:
                     with gzip.GzipFile(fileobj=response) as uncompressed:
                         file_content = uncompressed.read()
                 with open(path + writename, "wb") as f:
                     f.write(file_content)
+                    print('%s was written' %writename)
         except Exception as e:
             print(e)
 
 
 def main(emdbidList, alldata=False):
     for emdbid in emdbidList:
         if alldata:
```

### Comparing `emda-1.1.5/emda/ext/fakehalf.py` & `emda-1.1.6.post1/emda/ext/fakehalf.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/fouriersp_local.py` & `emda-1.1.6.post1/emda/ext/fouriersp_local.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/half2full.py` & `emda-1.1.6.post1/emda/ext/half2full.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/likelihood_map.py` & `emda-1.1.6.post1/emda/ext/likelihood_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,37 +132,33 @@
 ):
     import fcodes_fast
     import emda.core as core
     debug_mode = 0
 
     ######## smoothening signals
     """ from emda.ext.mapfit.newsignal import get_extended_signal
-    from emda.ext.mapfit.utils import moving_average
     #res_arr, signal, bin_fsc, fobj=None
     fobj = open('test.txt', '+w')
     for i, signal in enumerate(sgnl_var):
-        hffsc_i = np.zeros(hffsc[i].shape[0], 'float')
-        bin_fsc = moving_average(hffsc[i])
-        hffsc_i[:bin_fsc.shape[0]] = bin_fsc
         sgnl_var[i] = get_extended_signal(res_arr=res_arr,
-            signal=sgnl_var[i], bin_fsc=hffsc_i, fobj=fobj, fsc_cutoff=0.2)
+            signal=sgnl_var[i], bin_fsc=hffsc[i], fobj=fobj, fsc_cutoff=0.3)
     covar[0] = get_extended_signal(res_arr=res_arr,
             signal=covar[0], bin_fsc=covar[1], fobj=fobj, fsc_cutoff=0.3) """
 
     ######## test input data
-    print(len(sgnl_var))
+    """ print(len(sgnl_var))
     print(len(totl_var))
     print(len(covar))
     cc = covar[0]/np.sqrt(sgnl_var[0] * sgnl_var[1])
     cc2 = covar[0]/np.sqrt(totl_var[0] * totl_var[1])
     for i, _ in enumerate(sgnl_var[0]):
         print(res_arr[i], sgnl_var[0][i], sgnl_var[1][i], covar[0][i], cc[i])
     print('T')
     for i, _ in enumerate(totl_var[0]):
-        print(res_arr[i], totl_var[0][i], totl_var[1][i], covar[0][i], cc2[i])
+        print(res_arr[i], totl_var[0][i], totl_var[1][i], covar[0][i], cc2[i]) """
 
 
     ######### average and difference map calculation
 
     nx, ny, nz = maps2avg[0].shape
     nmaps = len(maps2avg)
     unit_cell = uc
@@ -177,29 +173,25 @@
 
     #### if signal-fsc is below zero, make all zero thereafter
     from emda.ext.mapfit.mapaverage import set_array
 
     covariance = set_array(covar[0])
     signal1 = set_array(sgnl_var[0])
     signal2 = set_array(sgnl_var[1])
-    # imposing resolution limit on signals and covaraince
-    """ covariance = covariance * (res_arr > 3.36)
-    signal1 = signal1 * (res_arr > 3.36)
-    signal2 = signal2 * (res_arr > 3.36) """
-    #if not (np.sqrt(signal1 * signal2) >= covariance).all():
-    #    print("There is a problem in signal variances and covariance.")
-    #    print("Trucated data will be used in the calculation")
-    #    prod = np.sqrt(signal1 * signal2)
-    #    for i, cv in enumerate(covariance):
-    #        if prod[i] < cv:
-    #            break
-    #    covariance = set_array(covariance, cv)
-    #    for i, cv in enumerate(covariance):
-    #        print(res_arr[i], signal1[i], signal2[i], prod[i], cv)        
-    #    #raise SystemExit("Problem in signal variances and covariance.")
+    if not (np.sqrt(signal1 * signal2) >= covariance).all():
+        print("There is a problem in signal variances and covariance.")
+        print("Trucated data will be used in the calculation")
+        prod = np.sqrt(signal1 * signal2)
+        for i, cv in enumerate(covariance):
+            if prod[i] < cv:
+                break
+        covariance = set_array(covariance, cv)
+        for i, cv in enumerate(covariance):
+            print(res_arr[i], signal1[i], signal2[i], prod[i], cv)        
+        #raise SystemExit("Problem in signal variances and covariance.")
     total1, total2 = totl_var[0], totl_var[1]
     if not (total1 > 0.).all():
         raise SystemExit("Problems in total variance in map 1")
     if not (total2 > 0.).all():
         raise SystemExit("Problems in total variance in map 2")
     if not (np.sqrt(total1 * total2) >= covariance).all():
         raise SystemExit("Problem in total variances and covariance.")    
@@ -360,15 +352,15 @@
     # 4. calculate average map
     from emda.ext.mapfit.utils import output_maps #, avg_and_diffmaps
     averagemaps = avg_and_diffmaps(maps2avg=[stats1[0], stats2[0]],
                                 uc=uc,
                                 nbin=nbin,
                                 sgnl_var=[stats1[3],stats2[3]],
                                 totl_var=[stats1[4],stats2[4]],
-                                covar=[stats3[3],stats3[5]],
+                                covar=[stats3[3]],
                                 hffsc=[stats1[5], stats2[5]],
                                 bin_idx=bin_idx,
                                 s_grid=s_grid,
                                 res_arr=res_arr,
                                 Bf_arr=[0.0])
     # 5. output maps
     output_maps(averagemaps=averagemaps,
```

### Comparing `emda-1.1.5/emda/ext/lowpass_map.py` & `emda-1.1.6.post1/emda/ext/lowpass_map.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/magnification.py` & `emda-1.1.6.post1/emda/ext/magnification.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/magnification_new.py` & `emda-1.1.6.post1/emda/ext/realsp_local.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,551 +2,573 @@
 Author: "Rangana Warshamanage, Garib N. Murshudov"
 MRC Laboratory of Molecular Biology
     
 This software is released under the
 Mozilla Public License, version 2.0; see LICENSE.
 """
 
+# local correlation in real space
+
 from __future__ import absolute_import, division, print_function, unicode_literals
 import numpy as np
-from emda.core import iotools, restools
-import fcodes_fast as fcodes
 from emda import core
+import emda.emda_methods as em
+import fcodes_fast
+import traceback
 
-
-class LineFit:
+class RealspaceLocalCC:
     def __init__(self):
-        self.e0_lf = None
-        self.step = None
-        self.e1_lf = None
-        self.cbin_idx_lf = None
-        self.cbin_lf = None
-        self.w_grid = None
-        self.res_arr = None
-        self.mode = "model"
+        self.hfmap1name = None
+        self.hfmap2name = None
+        self.maskname = None
+        self.uc = None
+        self.bfac = None
+        self.origin = None
+        self.kern_rad = 5
+        self.norm=False
+        self.model=None
+        self.model_resol=None
+        self.lgf=None
+        self.arr1 = None
+        self.arr2 = None
+        self.mask = None
+        self.hfmapcc = None
+        self.fullmapcc = None
+        self.mapmodelcc = None
+        self.truemapmodelcc = None
+
+    def check_inputs(self):
+        if self.model is not None:
+            if self.model.endswith((".pdb", ".ent", ".cif")):
+                if self.model_resol is None:
+                    raise SystemExit(
+                        "Please input resolution for model-based map!")
+
+    def get_fullmapcor(self):
+        import numpy.ma as ma
+
+        hfmap_corr_ma = ma.masked_less_equal(self.hfmapcc, 0.0)
+        ccf_ma = 2 * hfmap_corr_ma / (1.0 + hfmap_corr_ma)
+        self.mapmodelcc = ccf_ma.filled(0.0)
+
+    def truemap_model_cc(self):
+        import numpy.ma as ma
+
+        # To prevent large numbers in truemapmodelcc
+        mapmodelcc_ma = ma.masked_less_equal(self.mapmodelcc, 0.3)
+        fullmapcc_ma = ma.masked_less_equal(self.fullmapcc, 0.3)
+        truemapmodelcc_ma = mapmodelcc_ma / np.sqrt(fullmapcc_ma)
+        truemapmodelcc = core.iotools.mask_by_value_greater(
+            truemapmodelcc_ma.filled(0.0), masking_value=1.0
+        )
+        self.truemapmodelcc = truemapmodelcc #* (truemapmodelcc > 0.0)
 
-    def get_linefit_static_data(self, e0, cbin_idx, res_arr, smax):
-        (
-            self.e0_lf,
-            self.cbin_idx_lf,
-            self.cbin_lf,
-        ) = restools.cut_resolution_for_linefit(e0, cbin_idx, res_arr, smax)
-        self.res_arr = res_arr[: self.cbin_lf]
-
-    def f(self, kini):
-        import emda.ext.mapfit.utils as utils
-
-        nx, ny, nz = self.e0_lf.shape
-        ncopies = 1
-        k = self.k + kini[0] * self.step
-        eck = fcodes.tricubic_zoom(
-            float(k), self.e1_lf, 0, ncopies, nx, ny, nz)
-        eckt = eck[:, :, :, 0]
-        w_grid = utils.get_fsc_wght(
-            self.e0_lf, eckt, self.cbin_idx_lf, self.cbin_lf)
-        fval = np.sum(w_grid * self.e0_lf * np.conjugate(eckt))
-        return -fval.real
-
-    def fn2(self, kini):
-        nx, ny, nz = self.e0_lf.shape
-        ncopies = 1
-        #k = self.k + kini[0] * self.step
-        k = self.k + kini * self.step
-        fcks = fcodes.tricubic_zoom(
-            float(k), self.e1_lf, 0, ncopies, nx, ny, nz)
-        fckt = fcks[:, :, :, 0]
-        _, _, _, fval = fcodes.scalesigmafval_full(
-            self.e0_lf,
-            fckt,
-            self.cbin_idx_lf,
-            self.res_arr,
-            0,
-            self.cbin_lf,
-            nx,
-            ny,
-            nz,
+    def outputmaps(self, data, outname):
+        core.iotools.write_mrc(
+            mapdata=data,
+            filename=outname + str(self.kern_rad) + ".mrc",
+            unit_cell=self.uc,
+            map_origin=self.origin,
+            label=True,
         )
-        return fval.real
 
-    def calc_fval_for_different_kvalues_at_this_step(self, k=1.0, e1=None):
-        from scipy import optimize
+    def rcc(self):
+        self.check_inputs()
+        model = self.model
+        print("Calculating 3D correlation. Please wait...")
+        uc, arr1, origin = core.iotools.read_map(self.hfmap1name)
+        uc, arr2, origin = core.iotools.read_map(self.hfmap2name)
+        self.uc, self.origin = uc, origin
+        if self.maskname is not None:
+            _, cc_mask, _ = core.iotools.read_map(self.maskname)
+            cc_mask_binary = cc_mask > 0.01 # binary mask
+        else:
+            cc_mask = 1
+            cc_mask_binary = 1
+        self.mask = cc_mask
+        nx, ny, nz = arr1.shape
+        kern_sphere_soft = core.restools.create_soft_edged_kernel_pxl(self.kern_rad)
+        f_hf1, f_hf2 = np.fft.fftn(arr1*self.mask), np.fft.fftn(arr2*self.mask)
+        print("Calculating 3D correlation...")
+        if self.norm:
+            hf1, hf2 = np.fft.fftshift(f_hf1), np.fft.fftshift(f_hf2)
+            print("Normalising maps...")
+            nm = NormalizedMaps(hf1=hf1, hf2=hf2, cell=uc)
+            if self.bfac is not None:
+                nm.bfac = float(self.bfac)
+            nm.get_normdata()
+            nbin, bin_idx = nm.nbin, nm.bin_idx
+            normfull = nm.normfull
+            em.write_mrc(nm.normmap1, "bin_normalized_halfmap1.mrc", uc, origin)
+            em.write_mrc(nm.normmap2, "bin_normalized_halfmap2.mrc", uc, origin)
+            em.write_mrc(normfull, "bin_normalized_fullmap.mrc", uc, origin)
+            # Real space correlation maps
+            print("Calculating 3D correlation using normalized maps...")
+            halfmapscc = get_3d_realspcorrelation(
+                half1=nm.normmap1 * cc_mask,
+                half2=nm.normmap2 * cc_mask,
+                kern=kern_sphere_soft,
+            )
+        if not self.norm:
+            halfmapscc = get_3d_realspcorrelation(
+                half1=arr1 * self.mask, 
+                half2=arr2 * self.mask, 
+                kern=kern_sphere_soft
+            )
+        fullmapcc = 2 * halfmapscc / (1.0 + halfmapscc)
+        self.hfmapcc = halfmapscc 
+        self.fullmapcc = fullmapcc
+        print("Writing out correlation maps...")
+        self.outputmaps(self.hfmapcc * cc_mask_binary, "rcc_halfmap_smax")
+        self.outputmaps(self.fullmapcc * cc_mask_binary, "rcc_fullmap_smax")
+        self.outputmaps(np.sqrt(
+                        np.where(self.fullmapcc <= 0.0, 0.0, self.fullmapcc))
+                        * cc_mask_binary, "rcc_fullmap_star_smax")
+        # Map-model correlation
+        if model is not None:
+            print("\nMap-model correlation!\n")
+            dim = [nx, ny, nz]
+            if model.endswith((".pdb", ".ent", ".cif")):
+                print("Map will be calculated up to " 
+                      + str(self.model_resol) + "A")
+                print("Calculating map from model. Please wait...")
+                model_arr = calculate_modelmap(
+                    modelxyz=model, 
+                    dim=dim, 
+                    resol=self.model_resol, 
+                    uc=uc, 
+                    maporigin=origin,
+                    lgf=self.lgf)
+            elif model.lower().endswith((".mrcs", ".mrc", ".map")):
+                _, model_arr, _ = core.iotools.read_map(model)
+            elif model.lower().endswith(".mtz"):
+                model_arr = core.maptools.mtz2map(model, (nx, ny, nz))
+            em.write_mrc(model_arr, "modelmap.mrc", uc, origin)
+            if self.norm:
+                print("Calculating model-map correlation...\n")
+                normmodel = normalized_modelmap(
+                                modelmap=model_arr, 
+                                fsc_grid_str=nm.fsc_grid_str, 
+                                bin_idx=bin_idx, 
+                                nbin=nbin,
+                                bfac=self.bfac,
+                                uc=uc
+                            )
+                em.write_mrc(normmodel, "bin_normalized_modelmap.mrc", uc, origin)
+                print("Calculating model-map correlation...\n")
+                mapmodelcc = get_3d_realspcorrelation(
+                    half1=normfull * cc_mask,
+                    half2=normmodel * cc_mask,
+                    kern=kern_sphere_soft,
+                )
+            if not self.norm:
+                f_fullmap = (f_hf1 + f_hf2) / 2.0
+                fullmap = np.real(np.fft.ifftn(f_fullmap))
+                print("Calculating model-map correlation...\n")
+                mapmodelcc= get_3d_realspcorrelation(fullmap, model_arr, kern_sphere_soft)
+            self.mapmodelcc = mapmodelcc
+            self.outputmaps(self.mapmodelcc * cc_mask_binary, "rcc_mapmodel_smax")
+            print("Calculating truemap-model correlation...")
+            #self.truemap_model_cc()
+            #self.outputmaps(self.truemapmodelcc * cc_mask_binary, "rcc_truemapmodel_smax")
+            print("Map-model correlation calculated! Maps were writted!")
+            # calculating residue correlation
+            from emda.ext import atomic_cc
+            atomic_cc.main_helper_for_rcc(
+                uc=uc, 
+                rcc_map=fullmapcc, 
+                rcc_mapmodel=mapmodelcc, 
+                modelname=model)
+
+def apply_bfac(f, bv, uc):
+    nx, ny, nz = f.shape
+    bf_arr = [bv]
+    nbf = len(bf_arr)
+    all_mapout = fcodes_fast.apply_bfactor_to_map(
+        f, bf_arr, uc, 0, nx, ny, nz, nbf
+        )
+    f_bv = all_mapout[:, :, :, 0]
+    return f_bv
+
+
+def get_3d_realspcorrelation(half1, half2, kern, mask=None):
+    import scipy.signal
+    from scipy.stats import mode
+
+    loc3_A = scipy.signal.fftconvolve(half1, kern, "same")
+    loc3_A2 = scipy.signal.fftconvolve(half1 * half1, kern, "same")
+    loc3_B = scipy.signal.fftconvolve(half2, kern, "same")
+    loc3_B2 = scipy.signal.fftconvolve(half2 * half2, kern, "same")
+    loc3_AB = scipy.signal.fftconvolve(half1 * half2, kern, "same")
+    cov3_AB = loc3_AB - loc3_A * loc3_B
+    var3_A = loc3_A2 - loc3_A ** 2
+    var3_B = loc3_B2 - loc3_B ** 2
+    # regularization
+    #reg_a = mode(var3_A)[0][0][0][0] / 100
+    #reg_b = mode(var3_B)[0][0][0][0] / 100
+    reg_a = np.max(var3_A) / 1000
+    reg_b = np.max(var3_B) / 1000
+    var3_A = np.where(var3_A < reg_a, reg_a, var3_A)
+    var3_B = np.where(var3_B < reg_b, reg_b, var3_B) 
+    halfmaps_cc = cov3_AB / np.sqrt(var3_A * var3_B) 
+    return halfmaps_cc
+
 
-        # start = timer()
-        nx, ny, nz = e1.shape
-        cx = self.e0_lf.shape[0] // 2
-        cy = cz = cx
-        dx = int((nx - 2 * cx) / 2)
-        dy = int((ny - 2 * cy) / 2)
-        dz = int((nz - 2 * cz) / 2)
-        self.e1_lf = e1[dx: dx + 2 * cx, dy: dy + 2 * cy, dz: dz + 2 * cz]
-        assert self.e1_lf.shape == self.e0_lf.shape
-        init_guess = [k]
-        self.k = k
-        if self.mode == "map":  # for map-map
-            minimum = optimize.minimize(self.f, init_guess, method="Powell")
-        if self.mode == "model":  # for map-model
-            #minimum = optimize.minimize(self.fn2, init_guess, method="Powell")
-            minimum = optimize.minimize_scalar(self.fn2, method="brent")
-        # end = timer()
-        # print(' time for line search: ', end-start)
-        return minimum.x
-
-
-def create_xyz_grid(uc, nxyz):
-    x = np.fft.fftfreq(nxyz[0])  # * uc[0]
-    y = np.fft.fftfreq(nxyz[1])  # * uc[1]
-    z = np.fft.fftfreq(nxyz[2])  # * uc[2]
-    xv, yv, zv = np.meshgrid(x, y, z)
-    xyz = [yv, xv, zv]
-    for i in range(3):
-        xyz[i] = np.fft.ifftshift(xyz[i])
-    return xyz
-
-
-def get_xyz_sum(xyz):
-    xyz_sum = np.zeros(shape=(6), dtype="float")
-    n = -1
-    for i in range(3):
-        for j in range(3):
-            if i == 0:
-                sumxyz = np.sum(xyz[i] * xyz[j])
-            elif i > 0 and j >= i:
-                sumxyz = np.sum(xyz[i] * xyz[j])
-            else:
-                continue
-            n = n + 1
-            xyz_sum[n] = sumxyz
-    return xyz_sum
-
-
-def dFks(mapin, uc):
-    xyz = create_xyz_grid(uc, mapin.shape)
-    vol = uc[0] * uc[1] * uc[2]
-
-    # Calculating dFC(ks)/dk using FFT
-    dfk = np.zeros(mapin.shape, np.complex64)
-    xyz_sum = 0.0
-    for i in range(3):
-        xyz_sum = xyz_sum + np.sum(xyz[i])
-    # dfk = np.fft.fftshift((-1/vol) * 2j * np.pi * np.fft.fftn(mapin * xyz_sum))
-    dfk = np.fft.fftshift(-2j * np.pi * np.fft.fftn(mapin * xyz_sum))
-
-    # second derivative
-    xyz_sum = 0.0
-    tp2 = (2.0 * np.pi) ** 2
-    """ for i in range(3):
-        for j in range(3):
-            xyz_sum = xyz_sum + np.sum(xyz[i] * xyz[j]) """
-    xyz_sum = np.sum(get_xyz_sum(xyz))
-    # ddfk = -(tp2/vol) * np.fft.fftshift(np.fft.fftn(mapin * xyz_sum))
-    ddfk = -(tp2) * np.fft.fftshift(np.fft.fftn(mapin * xyz_sum))
-    return dfk, ddfk
-
-
-def dFts(Fc, sv):
-    nx, ny, nz = Fc.shape
-    tp2 = (2.0 * np.pi) ** 2
-    dt_arr = np.zeros(shape=(nx, ny, nz, 3), dtype="complex")
-    ddt_arr = np.zeros(shape=(nx, ny, nz, 3, 3), dtype="complex")
-    for i in range(3):
-        # 1st derivative
-        dfs = 2.0 * 1j * np.pi * sv[i] * Fc
-        dt_arr[:, :, :, i] = dfs
-        # 2nd derivative
-        for j in range(3):
-            if i == 0:
-                ddfs = -tp2 * sv[i] * sv[j] * Fc
-            elif i > 0 and j >= i:
-                ddfs = -tp2 * sv[i] * sv[j] * Fc
-            else:
-                ddfs = ddt_arr[:, :, :, j, i]
-            ddt_arr[:, :, :, i, j] = ddfs
-    return dt_arr, ddt_arr
-
-
-#def get_ll(emmap1, fmaplist, bin_idx, res_arr, nbin, k, smax):
-#    fref = fmaplist[0]
-#    ftar = fmaplist[1]
-#    nx, ny, nz = fref.shape  # model
-#
-#    ncopies = 1
-#    fcks = fcodes.tricubic_zoom(k, fref, 0, ncopies, nx, ny, nz)
-#    map1 = np.real(np.fft.ifftshift(np.fft.ifftn(np.fft.ifftshift(fref))))
-#    iotools.write_mrc(map1, 'fref.mrc', emmap1.map_unit_cell)
-#    map2 = np.real(np.fft.ifftshift(np.fft.ifftn(np.fft.ifftshift(ftar))))
-#    iotools.write_mrc(map2, 'ftar.mrc', emmap1.map_unit_cell)
-#    map3 = np.real(np.fft.ifftshift(np.fft.ifftn(np.fft.ifftshift(fcks[:,:,:,0]))))
-#    iotools.write_mrc(map3, 'interpolated.mrc', emmap1.map_unit_cell)
-#    # optimize translation
-#    t = np.array([0.0, 0.0, 0.0], 'float')
-#    f1 = fcks[:, :, :, 0]
-#    """ t = optimise_translation(
-#        f0=f1, 
-#        f1=ftar, 
-#        t=t, 
-#        bin_idx=bin_idx, 
-#        nbin=nbin, 
-#        res_arr=res_arr, 
-#        smax_lf=smax,
-#        pixsize=emmap1.pixsize
-#        ) """
-#    t = -np.asarray(t) # testing the sign of t
-#    st, s1, s2, s3 = fcodes.get_st(nx, ny, nz, t)
-#    sv = np.array([s1, s2, s3])
-#    #
-#    fckt = fcks[:, :, :, 0] * st
-#    # test output map
-#    map1 = np.real(np.fft.ifftshift(np.fft.ifftn(np.fft.ifftshift(fckt))))
-#    iotools.write_mrc(map1, 'test.mrc', emmap1.map_unit_cell)
-#    #
-#    if len(fmaplist) == 2:
-#        scale_d, sigma, totalvar, fval = fcodes.scalesigmafval_full(
-#            ftar, fckt, bin_idx, res_arr, 1, nbin, nx, ny, nz
-#        )
-#        return ftar, fckt, scale_d, sigma, totalvar, fval, sv, t
-
-def get_ll(emmap1, fmaplist, bin_idx, res_arr, nbin, k, smax):
-    fref = fmaplist[0]
-    ftar = fmaplist[1]
-    nx, ny, nz = fref.shape  # model
-    fcks = fcodes.tricubic_zoom2(k, fref, 0, nx, ny, nz)
-    map1 = np.real(np.fft.ifftshift(np.fft.ifftn(np.fft.ifftshift(fref))))
-    iotools.write_mrc(map1, 'fref.mrc', emmap1.map_unit_cell)
-    map2 = np.real(np.fft.ifftshift(np.fft.ifftn(np.fft.ifftshift(ftar))))
-    iotools.write_mrc(map2, 'ftar.mrc', emmap1.map_unit_cell)
-    map3 = np.real(np.fft.ifftshift(np.fft.ifftn(np.fft.ifftshift(fcks))))
-    iotools.write_mrc(map3, 'interpolated.mrc', emmap1.map_unit_cell)
-    # optimize translation
-    t = np.array([0.0, 0.0, 0.0], 'float')
-    f1 = fcks
-    t = optimise_translation(
-        f0=f1, 
-        f1=ftar, 
-        t=t, 
-        bin_idx=bin_idx, 
-        nbin=nbin, 
-        res_arr=res_arr, 
-        smax_lf=smax,
-        pixsize=emmap1.pixsize
+
+def calculate_modelmap(modelxyz, dim, resol, uc, refmac=False, lgf=None, maporigin=None):
+    if refmac:
+        print('Modelmap calculation using REFMAC')
+        modelmap = em.model2map(
+            modelxyz=modelxyz,
+            dim=dim,
+            resol=resol,
+            cell=uc,
+            ligfile=lgf,
+            maporigin=maporigin,
         )
-    t = np.asarray(t) # testing the sign of t
-    st, s1, s2, s3 = fcodes.get_st(nx, ny, nz, t)
-    sv = np.array([s1, s2, s3])
-    fckt = fcks * st
-    # testing the direction of translation
-    fsc_plus = core.fsc.anytwomaps_fsc_covariance(ftar, fckt, bin_idx, nbin)[0]
-    st, s1, s2, s3 = fcodes.get_st(nx, ny, nz, -np.asarray(t))
-    sv = np.array([s1, s2, s3])
-    fckt = fcks * st
-    fsc_minus = core.fsc.anytwomaps_fsc_covariance(ftar, fckt, bin_idx, nbin)[0]
-    """ print("bin#   Plus   Minus")
-    for i in range(len(fsc_plus)):
-        print(i, fsc_plus[i], fsc_minus[i]) """
-    # test output map
-    map1 = np.real(np.fft.ifftshift(np.fft.ifftn(np.fft.ifftshift(fckt))))
-    iotools.write_mrc(map1, 'test.mrc', emmap1.map_unit_cell)
-    #
-    if len(fmaplist) == 2:
-        scale_d, sigma, totalvar, fval = fcodes.scalesigmafval_full(
-            ftar, fckt, bin_idx, res_arr, 1, nbin, nx, ny, nz
+    else:
+        # use gemmi for modelmap calculation
+        print('Modelmap calculation using GEMMI')
+        modelmap = em.model2map_gm(
+            modelxyz=modelxyz,
+            dim=dim,
+            resol=resol,
+            cell=uc,
+            maporigin=maporigin,
+        )  
+        # check if modelmap dims are OK
+        curnt_pix = [float(round(uc[i]/shape, 5)) for i, shape in enumerate(modelmap.shape)]
+        targt_pix = [float(round(uc[i]/dim[i], 5)) for i in range(3)]
+        modelmap = em.resample_data(
+            curnt_pix=curnt_pix, targt_pix=targt_pix, targt_dim=dim, arr=modelmap
         )
-        return ftar, fckt, scale_d, sigma, totalvar, fval, sv, t
+    return modelmap
 
 
-def derivatives_mapmodel(fo, fc, bin_idx, sv, D, totalvar, uc):
-    # 1. Calculate dFc/dk and dFc/dT
-    mapin = np.fft.ifftn(np.fft.ifftshift(fc))
-    dk, ddk = dFks(mapin, uc)
-    # dt, ddt = dFts(fc,sv)
-
-    nbin = len(totalvar)
-    nx, ny, nz = fc.shape
-    dll, ddll = fcodes.ll_derivatives(
-        fo, fc, bin_idx, D, totalvar, 1, nbin, nx, ny, nz)
-
-    # 1st derivatives
-    df_val = np.zeros(shape=(4), dtype="float")
-    df_val[0] = np.sum(np.real(dll * np.conjugate(dk)))
-    """ for i in range(3):
-        df_val[i+1] = np.sum(np.real(dll * np.conjugate(2j * np.pi * sv[i] * fc))) """
-
-    # 2nd derivatives
-    ddf_val = np.zeros(shape=(4, 4), dtype="float")
-    ddf_val[0, 0] = np.sum(np.real(ddll * np.conjugate(ddk)))
-    """ tp2 = (2.0 * np.pi)**2
-    for i in range(3):
-        for j in range(3):
-            ddf_val[i+1,j+1] = -tp2 * np.sum(np.real(ddll * \
-                np.conjugate(fc * sv[i] * sv[j]))) """
-    ddf_val_inv = np.linalg.pinv(ddf_val)
-    step = ddf_val_inv.dot(-df_val)
-    return step
-
-
-def calc_fsc_t(fstatic, frotated, t, bin_idx, nbin):
-    cx, cy, cz = fstatic.shape
-    st, s1, s2, s3 = fcodes.get_st(cx, cy, cz, t)
-    sv = np.array([s1, s2, s3])
-    frt = frotated * st
-    fsc = core.fsc.anytwomaps_fsc_covariance(fstatic, frt, bin_idx, nbin)[
-        0
-    ]
-    return frt, fsc, sv
-
-
-def get_wght(f0, fsc, bin_idx, nbin):
-    cx, cy, cz = f0.shape
-    w_grid = fcodes.read_into_grid(
-        bin_idx,
-        fsc,  # fsc / (1 - fsc ** 2),
-        nbin,
-        cx,
-        cy,
-        cz,
+def make_c_B_table(s_max, dat_out=None):
+    import scipy.special
+    t = lambda B: np.sqrt(np.abs(B)/2)*s_max
+    w = lambda z: np.exp(-z**2)*(1-1j*scipy.special.erfi(-z))
+    fp = lambda x: 3/2*(np.sqrt(np.pi)/2*scipy.special.erf(t(x))-t(x)*np.exp(-t(x)**2))/t(x)**3
+    fn = lambda x: 3/4*np.exp(t(x)**2)*(2*t(x)-np.sqrt(np.pi)*np.imag(w(t(x))))/t(x)**3
+
+    Bn = np.arange(-300,0)
+    cn = fn(Bn)
+    Bp = np.arange(1, 600)
+    cp = fp(Bp)
+
+    Bs = np.concatenate((Bn, [0.], Bp))
+    cs = np.concatenate((cn, [1.], cp))
+
+    order = np.argsort(cs)
+    Bs, cs = Bs[order], cs[order]
+
+    if dat_out:
+      with open(dat_out, "w") as ofs:
+        ofs.write("# s_max= {}\n".format(s_max))
+        ofs.write("c B\n")
+        for i in range(len(Bs)):
+          ofs.write("{:.5e} {:.1f}\n".format(cs[i], Bs[i]))
+
+    return Bs, cs
+
+def bfromcc(
+    half1_map,
+    half2_map,
+    kernel_size,
+    resol,
+    mask_map=None,
+):
+    import emda.emda_methods as em
+
+    hf1, hf2 = None, None
+    bin_idx = None
+    print(
+        "Calculating 3D correlation between half maps. \
+            Please wait..."
+    )
+    uc, arr1, origin = core.iotools.read_map(half1_map)
+    uc, arr2, origin = core.iotools.read_map(half2_map)
+
+    # mask taking into account
+    if mask_map is not None:
+        _, cc_mask, _ = core.iotools.read_map(mask_map)
+    else:
+        # creating ccmask from half data
+        print("Mask is not given. EMDA will generate cc_mask.mrc and be used.")
+        print("Please take a look at this automatic mask. It may be suboptimal.")
+        cc_mask = em.mask_from_halfmaps(uc, arr1, arr2, radius=7, thresh=0.65)
+        em.write_mrc(cc_mask, "cc_mask.mrc", uc, origin)
+
+    cc_mask = cc_mask * (cc_mask > 0.0)
+    # Creating soft-edged mask
+    kern_sphere_soft = core.restools.create_soft_edged_kernel_pxl(kernel_size)
+
+    # Lowpass
+    f_hf1, arr1 = em.lowpass_map(uc=uc, arr1=arr1, resol=resol)
+    f_hf2, arr2 = em.lowpass_map(uc=uc, arr1=arr2, resol=resol)
+
+    # Real space correlation maps
+    print("Calculating 3D correlation...")
+    halfmapscc, fullmapcc = get_3d_realspcorrelation(
+        half1=arr1 * cc_mask, half2=arr2 * cc_mask, kern=kern_sphere_soft
     )
-    fsc_sqd = fsc ** 2
-    fsc_combi = fsc_sqd,  # fsc_sqd / (1 - fsc_sqd)
-    w2_grid = fcodes.read_into_grid(
-        bin_idx, fsc_combi, nbin, cx, cy, cz
+
+    overall_cc = np.corrcoef((arr1*cc_mask).flatten(), (arr2*cc_mask).flatten())[1,0]
+    print("Overall CC=", overall_cc)
+
+    c = (1.-overall_cc)/overall_cc * halfmapscc/(1.-halfmapscc)
+    print("c range: {:.4e} to {:.4e}".format(c.min(), c.max()))
+    core.iotools.write_mrc(c,'c_for_localB'+str(kernel_size)+'.mrc',uc,origin)
+
+    table_B, table_c = make_c_B_table(1./resol, dat_out="c_B.dat")
+    print("c to B table made for c= {:.4e} to {:.4e} and B= {:.1f} to {:.1f}".format(min(table_c), max(table_c), min(table_B), max(table_B)))
+    B = np.interp(c, table_c, table_B)
+    print("Writing out local B map")
+    core.iotools.write_mrc(mapdata=B,filename='localB'+str(kernel_size)+'.mrc',unit_cell=uc,map_origin=origin)
+
+    print("Writing out correlation maps")
+    core.iotools.write_mrc(
+        mapdata=halfmapscc * cc_mask,
+        filename="rcc_halfmap_smax" + str(kernel_size) + ".mrc",
+        unit_cell=uc,
+        map_origin=origin,
+        label=True,
     )
-    return w_grid, w2_grid
 
 
-def optimise_translation(f0, f1, t, bin_idx, nbin, res_arr, smax_lf, pixsize, ncy=10):
-    from emda.ext.sym.refine_symaxis import derivatives_translation, linefit2
+def scale_model2map(fullmap, model_arr, uc):
+    from emda.ext.scale_maps import scale_twomaps_by_power, transfer_power
+
+    f1 = np.fft.fftshift(np.fft.fftn(np.fft.fftshift(fullmap)))
+    f2 = np.fft.fftshift(np.fft.fftn(np.fft.fftshift(model_arr)))
+    nbin, res_arr, bin_idx = core.restools.get_resolution_array(uc, f1)
+    scale_grid = transfer_power(
+        bin_idx,
+        res_arr,
+        scale_twomaps_by_power(f1, f2, bin_idx=bin_idx, res_arr=res_arr),
+    )
+    scaled_model = np.real(np.fft.ifftn(np.fft.ifftshift(f2 * scale_grid)))
+    return scaled_model
+
 
-    tol = 1e-2 # tolerence for refinement convergence
-    nx, ny, nz = f0.shape
-    # convert fo to eo
-    """ import fcodes2
-    e0 = fcodes2.get_normalized_sf_singlemap(
-        fo=f0,
-        bin_idx=bin_idx,
-        nbin=nbin,
-        mode=0,
-        nx=nx,ny=ny,nz=nz,
+def mapmodel_rcc(
+    fullmap,
+    model,
+    resol,
+    kernel_size=5,
+    norm=False,
+    mask_map=None,
+    lgf=None,
+):
+    try:
+        print(
+            "Calculating 3D correlation between map and model. Please wait..."
         )
-    e1 = fcodes2.get_normalized_sf_singlemap(
-        fo=f1,
-        bin_idx=bin_idx,
-        nbin=nbin,
-        mode=0,
-        nx=nx,ny=ny,nz=nz,
+        uc, arr1, origin = core.iotools.read_map(fullmap)
+        nx, ny, nz = arr1.shape
+        # lowpass filter the map to given resolution
+        _, arr1 = em.lowpass_map(
+            uc=uc, 
+            arr1=arr1, 
+            resol=resol, 
+            filter='butterworth')
+        if mask_map is not None:
+            print("Correlation is calculated using a mask.")
+            print("Input map is masked before calculating correlation.")
+            _, mask, _ = core.iotools.read_map(mask_map)
+            mask_binary = mask > 0.
+        else:
+            mask = 1
+            mask_binary = 1
+        print("\nMap-model correlation!\n")
+        dim = [nx, ny, nz]
+        if model.endswith((".pdb", ".ent", ".cif")):
+            print("map will be calculated up to " + str(resol) + "A")
+            print("Calculating map from the model.")
+            model_arr = calculate_modelmap(
+                modelxyz=model, 
+                dim=dim, 
+                resol=resol, 
+                uc=uc, 
+                lgf=lgf, 
+                maporigin=origin,
+            )
+        elif model.lower().endswith((".mrc", ".map")):
+            _, model_arr, _ = core.iotools.read_map(model)
+            _, model_arr = em.lowpass_map(
+                uc=uc, 
+                arr1=model_arr, 
+                resol=resol, 
+                filter='butterworth')
+        elif model.lower().endswith(".mtz"):
+            model_arr = core.maptools.mtz2map(model, (nx, ny, nz))
+            _, model_arr = em.lowpass_map(
+                uc=uc, 
+                arr1=model_arr, 
+                resol=resol, 
+                filter='butterworth')
+        core.iotools.write_mrc(
+            mapdata=model_arr, filename="modelmap.mrc", unit_cell=uc, map_origin=origin
         )
-    f0, f1 = e0, e1 """
-    print("Translation optimisation..")
-    print('Cycle#    Fval.    Trans (A)')
-    for i in range(ncy):
-        frt, fsc, sv = calc_fsc_t(f0, f1, t, bin_idx, nbin)
-        avgfsc = np.average(fsc)
-        w_grid, w2_grid = get_wght(f0, fsc, bin_idx, nbin)
-        fval = np.real(np.sum(w_grid * f0 * np.conjugate(frt)))
-        t_angs = t * pixsize * nx
-        if i == 0:
-            fval_previous = fval
-        if i > 0 and abs(fval_previous - fval) > tol or i == ncy - 1:
-            print("{:5d} {:8.4f} {:6.3f} {}".format(i, fval, avgfsc, t_angs))
-        if i > 0 and abs(fval - fval_previous) <= tol or i == ncy - 1:
-            print("{:5d} {:8.4f} {:6.3f} {}".format(i, fval, avgfsc, t_angs))
-            break
-        step = derivatives_translation(f0, frt, w_grid, w2_grid, sv)
-        lft = linefit2()
-        lft.get_linefit_static_data(
-            [f0, frt], bin_idx, res_arr, smax_lf
+        print("Calculating model-map correlation...\n")
+        kern_sphere_soft = core.restools.create_soft_edged_kernel_pxl(kernel_size)
+        if norm:
+            print("Normalisation needs half maps. If you have half maps, then \
+                use rcc instead of mmcc. For now, local cc map-model will be \
+                    calculated using un-normalized map and model.")
+        mapmodelcc = get_3d_realspcorrelation(
+                arr1 * mask, model_arr, kern_sphere_soft
+            )
+        core.iotools.write_mrc(
+            mapdata=mapmodelcc * mask_binary,
+            filename="mmcc_mapmodel.mrc",
+            unit_cell=uc,
+            map_origin=origin,
+            label=True,
         )
-        lft.step = step
-        alpha = lft.scalar_opt_trans()
-        t = t + step * alpha
-        fval_previous = fval
-    return t
-
-
-def apply_transformation(folist, rmlist):
-    assert len(rmlist) == len(folist)
-    #print(len(folist))
-    #print(folist[0].shape)
-    nx, ny, nz = folist[0].shape
-    frs = fcodes.trilinearn(np.stack((folist[0], folist[1]), axis = 0),
-                            np.stack((rmlist[0], rmlist[1]), axis = 0),
-                            0,
-                            len(folist),
-                            nx, ny, nz)
-    #print(frs.shape)
-    return frs
-
-
-def apply_translation(fo, t):
-    nx, ny, nz = fo.shape
-    st, _, _, _ = fcodes.get_st(nx, ny, nz, t)    
-    return fo * st
-
-
-def cut_resolution_for_linefit(farr, bin_idx, res_arr, smax):
-    # Making data for map fitting
-    ncopies, nx, ny, nz = farr.shape
-    cbin = cx = smax
-    dx = int((nx - 2 * cx) / 2)
-    dy = int((ny - 2 * cx) / 2)
-    dz = int((nz - 2 * cx) / 2)
-    cBIdx = bin_idx[dx : dx + 2 * cx, dy : dy + 2 * cx, dz : dz + 2 * cx]
-    fout = fcodes.cutmap_arr(
-        farr, bin_idx, cbin, 0, len(res_arr), nx, ny, nz, ncopies
-    )[:, dx : dx + 2 * cx, dy : dy + 2 * cx, dz : dz + 2 * cx]
-    return fout, cBIdx, cbin
-
-
-def minimizer_mapmodel(emmap1, resol=4.0, ncycles=10, rmlist=None, tlist=None):
-    print('\nOptimising map magnification...')
-    tol = 1e-2 # tolerence for refinement convergence
-    # apply transformation
-    frs = apply_transformation(folist=emmap1.fo_lst, rmlist=rmlist)
-    # output reference map
-    refmap = np.fft.fftshift(
-        (np.fft.ifftn(np.fft.ifftshift(frs[0,:,:,:]))).real)
-    iotools.write_mrc(refmap, 'reference.mrc', emmap1.map_unit_cell)
-
-    # find the bin for given resolution for fit
-    dist = np.sqrt((emmap1.res_arr[:emmap1.nbin] - resol) ** 2)
-    smax = np.argmin(dist)
-    # cut data
-    fout, cBIdx, cbin = cut_resolution_for_linefit(
-        frs, emmap1.bin_idx, emmap1.res_arr, smax)
-
-    # parameters for magnification refinement
-    bin_idx = cBIdx
-    res_arr = emmap1.res_arr[:cbin]
-    nbin = cbin
-    uc = emmap1.map_unit_cell
-
-    for ifit in range(1, fout.shape[0]):
-        # output moving map before magref refinement
-        movingmap = apply_translation(frs[ifit,:,:,:], tlist[ifit])
-        refmap = np.fft.fftshift(
-                    (np.fft.ifftn(np.fft.ifftshift(movingmap))).real)
-        iotools.write_mrc(refmap, 'startmap_'+str(ifit)+'.mrc', uc)
-        # use cutdata in mag. refinement
-        maplist = [fout[0,:,:,:], apply_translation(fout[ifit,:,:,:], tlist[ifit])]
-        # initial parameters
-        t = [0.0, 0.0, 0.0]
-        k = k_previous = 1.0
-        for i in range(ncycles):
-            fo, fckt, scale_d, sigma, totalvar, fval, sv, t = get_ll(
-                emmap1, maplist, bin_idx, res_arr, nbin, k, smax)
-            fsc = core.fsc.anytwomaps_fsc_covariance(fo, fckt, bin_idx, nbin)[0]
-            avgfsc = np.average(fsc)
-            if i == 0:
-                fval_previous = fval
-                print()
-                print("ifit    cycle#    func val.   fsc    magnification")
-                print(
-                    "{:5d} {:5d} {:8.4f} {:6.3f} {:6.4f}".format(
-                        ifit, i, fval, avgfsc, k
-                    )
-                )
-            if i > 0 and abs(fval_previous - fval) > tol or i == ncycles - 1:
-                print(
-                    "{:5d} {:5d} {:8.4f} {:6.3f} {:6.4f}".format(
-                        ifit, i, fval, avgfsc, k
-                    )
-                )
-                k_previous = k
-            if i > 0 and abs(fval - fval_previous) <= tol or i == ncycles - 1:
-                print(
-                    "{:5d} {:5d} {:8.4f} {:6.4f}".format(
-                        ifit, i, fval, k
-                    )
-                )
-                # output map after mag. refinement
-                magerror = abs(k_previous - 1.0) * 100.0
-                print("magnification error (%): ", "{:.3f}".format(magerror))
-                _, nx, ny, nz = frs.shape
-                fck = fcodes.tricubic_zoom(
-                    float(1 / k_previous), frs[ifit,:,:,:], 0, 1, nx, ny, nz)[:, :, :, 0]
-                t = optimise_translation(
-                    f0=frs[0,:,:,:], 
-                    f1=fck, 
-                    t=t, 
-                    bin_idx=emmap1.bin_idx, 
-                    nbin=emmap1.nbin, 
-                    res_arr=emmap1.res_arr, 
-                    smax_lf=smax, 
-                    pixsize=emmap1.pixsize
-                    )
-                fckt = fck * fcodes.get_st(nx, ny, nz, t)[0]
-                zoomedmap = np.fft.fftshift(
-                    (np.fft.ifftn(np.fft.ifftshift(fckt))).real)
-                mapname = "emda_magcorretedmap_" + str(ifit) + ".mrc"
-                iotools.write_mrc(zoomedmap, mapname, uc)
-                print("Magnification corrected map %s was written." %(mapname) )
-                break
-            step = derivatives_mapmodel(
-                fo, fckt, bin_idx, sv, scale_d, sigma, uc)
-            if i == 0:
-                linefit = LineFit()
-                linefit.get_linefit_static_data(
-                    e0=fo, cbin_idx=bin_idx, res_arr=res_arr, smax=smax
-                )
-            linefit.step = step[0]
-            alpha = linefit.calc_fval_for_different_kvalues_at_this_step(
-                k=k, e1=maplist[0])
-            k = k + alpha * step[0]
-            fval_previous = fval
+        print("Map-model correlation calculated! Maps were written!")
+    except:
+        print('Input error!')
+        print(traceback.format_exc())
 
 
-def prepare_data(maplist, masklist=None):
-    from emda.ext.overlay import EmmapOverlay
-    try:
-        emmap1 = EmmapOverlay(map_list=maplist, mask_list=masklist, nocom=True)
-    except:
-        emmap1 = EmmapOverlay(maplist)
-    emmap1.com = False
-    emmap1.load_maps()
-    emmap1.calc_fsc_from_maps()
-    return emmap1
-
-
-def optimize_superposition(emmap1, ncycles=50):
-    from emda.ext.overlay import run_fit
-    from emda.core.quaternions import get_RM
-
-    print("\nOptimising overlay.....\n")
-    rotmat = np.identity(3)
-    t = [0.0, 0.0, 0.0]
-    rotmat_list = []
-    trans_list = []
-    fobj = open("EMDA_overlay.txt", "w")
-    rotmat_list.append(rotmat)
-    trans_list.append(t)
-    for ifit in range(1, len(emmap1.eo_lst)):
-        t, q_final = run_fit(
-                emmap1,
-                rotmat,
-                t,
-                ncycles,
-                ifit,
-            )
-        rotmat_list.append(get_RM(q_final))
-        trans_list.append(t)
-    print("Optimising overlay.....Done")
-    return rotmat_list, trans_list
-
-def main(maplist, fit_optimize=True, masklist=None, resol=None):
-    emmap1 = prepare_data(maplist, masklist)
-    if fit_optimize:
-        rm_list, t_list = optimize_superposition(emmap1)
-    else:
-        rm_list = []
-        t_list = []
-        for _ in range(len(maplist)):
-            rm_list.append(np.identity(3))
-            t_list.append(np.array([0., 0., 0.], 'float'))
-    minimizer_mapmodel(emmap1=emmap1, resol=resol, rmlist=rm_list, tlist=t_list)
-
-
-if __name__ == "__main__":
-    maplist = ["/Users/ranganaw/MRC/REFMAC/haemoglobin/EMD-3651/other/emd_3651_half_map_1.map",
-                "/Users/ranganaw/MRC/REFMAC/haemoglobin/EMD-3651/emda_test/magnification/data_for_emda-paper/emd_3651_half1_k095.mrc"]
-    #maplist = [
-    #    "/Users/ranganaw/MRC/REFMAC/beta_gal/magref_for_paper/xtallography_reference.mrc",
-    #    "/Users/ranganaw/MRC/REFMAC/beta_gal/magref_for_paper/emd_10574_fullmap_resampled2staticmap_pca.map",
-    #           ]
-    main(maplist)
+def normalized(map, bin_idx=None, nbin=None, uc=None):
+    import fcodes_fast as fc
+
+    # normalise in resol bins
+    if bin_idx is None:
+        if uc is not None:
+            nbin, res_arr, bin_idx = core.restools.get_resolution_array(uc, map)
+    hf1 = np.fft.fftshift(np.fft.fftn(map))
+    binfsc, _, _, totalvar, _, eo = core.fsc.halfmaps_fsc_variance(
+        hf1, hf1, bin_idx, nbin
+    )
+    binfsc = binfsc * (totalvar > 1e-5)
+    nx, ny, nz = eo.shape
+    fsc_frid = fc.read_into_grid(bin_idx, binfsc, nbin, nx, ny, nz)
+    norm_map = np.real(np.fft.ifftn(np.fft.ifftshift(eo * fsc_frid)))
+    return norm_map
+
+
+""" def normalized_modelmap(modelmap, f_fullmap, bin_idx=None, nbin=None, uc=None):
+    import fcodes_fast as fc
+
+    # normalise in resol bins
+    if bin_idx is None:
+        if uc is not None:
+            nbin, res_arr, bin_idx = core.restools.get_resolution_array(uc, modelmap)
+    f1 = np.fft.fftshift(np.fft.fftn(modelmap))
+    f_fullmap = np.fft.fftshift(f_fullmap)
+    #_, _, _, _, _, eo = core.fsc.halfmaps_fsc_variance(f1, f1, bin_idx, nbin)
+    #binfsc, _, _, _, _, _ = core.fsc.halfmaps_fsc_variance(f1, f_fullmap, bin_idx, nbin)
+    nx, ny, nz = f1.shape
+    eo, _, _, totalvar, binfsc, _ = fc.get_normalized_sf(
+        f1, f_fullmap, bin_idx, nbin, 0, nx, ny, nz
+    )
+    e1 = eo[:, :, :, 0]
+    #fsc_frid = fc.read_into_grid(bin_idx, binfsc, nbin, nx, ny, nz)
+    #norm_map = np.real(np.fft.ifftn(np.fft.ifftshift(e1 * fsc_frid)))
+    norm_map = np.real(np.fft.ifftn(np.fft.ifftshift(e1))) # not mulpiplying by fsc becoz no noise in the model
+    return norm_map """
+
+def normalized_modelmap(modelmap, fsc_grid_str, bin_idx=None, nbin=None, uc=None, bfac=None):
+    import fcodes_fast as fc
+
+    # normalise in resol bins
+    if bin_idx is None:
+        if uc is not None:
+            nbin, res_arr, bin_idx = core.restools.get_resolution_array(uc, modelmap)
+    f1 = np.fft.fftshift(np.fft.fftn(modelmap))
+    nx, ny, nz = f1.shape
+    eo = fc.get_normalized_sf(f1, f1, bin_idx, nbin, 0, nx, ny, nz)[0]
+    e1 = eo[:, :, :, 0]
+    if bfac is not None:
+        e1 = apply_bfac(f=e1, bv=bfac, uc=uc)
+    norm_map = np.real(np.fft.ifftn(np.fft.ifftshift(fsc_grid_str * e1)))
+    return norm_map
+
+
+def hfdata_normalized(hf1, hf2, bin_idx=None, nbin=None, uc=None):
+    # normalise in resol bins
+    import fcodes_fast as fc
+
+    print("Normalising maps...")
+    nm = NormalizedMaps(hf1=hf1, hf2=hf2, cell=uc)
+    nm.get_normdata()
+    return nm.normmap1, nm.normmap2
+
+
+class NormalizedMaps:
+    def __init__(self, hf1=None, hf2=None, bin_idx=None, nbin=None, cell=None):
+        self.hf1 = hf1
+        self.hf2 = hf2
+        self.e0 = None
+        self.e1 = None
+        self.e2 = None
+        self.bfac = None
+        self.normmap1 = None
+        self.normmap2 = None
+        self.normfull = None
+        self.bin_idx = bin_idx
+        self.cell = cell
+        self.nbin = nbin
+        self.binfsc = None
+        self.res_arr = None
+        self.totalvar = None
+        self.fsc_grid_str = None
+
+    def get_parameters(self):
+        if self.bin_idx is None:
+            if self.cell is not None:
+                (
+                    self.nbin,
+                    self.res_arr,
+                    self.bin_idx,
+                ) = core.restools.get_resolution_array(self.cell, self.hf1)
+
+    def get_normdata(self):
+        import fcodes_fast as fc
+        from emda.ext.mapfit.mapaverage import set_array
+
+        if self.bin_idx is None:
+            self.get_parameters()
+        nx, ny, nz = self.hf1.shape
+        eo, _, _, self.totalvar, self.binfsc, _ = fc.get_normalized_sf(
+            self.hf1, self.hf2, self.bin_idx, self.nbin, 0, nx, ny, nz
+        )
+        self.e1 = eo[:, :, :, 0]
+        self.e2 = eo[:, :, :, 1]
+        self.e0 = eo[:, :, :, 2]
+        fsc_half = set_array(arr=self.binfsc, thresh=0.01)
+        fsc_ful = 2 * fsc_half / (1 + fsc_half)
+        fsc_full_grid = fc.read_into_grid(self.bin_idx, fsc_ful, self.nbin, nx, ny, nz)
+        fsc_grid_str = np.sqrt(fsc_full_grid)
+        self.fsc_grid_str = fsc_grid_str
+        if self.bfac is not None:
+            self.e0 = apply_bfac(f=self.e0, bv=float(self.bfac), uc=self.cell)
+            self.e1 = apply_bfac(f=self.e1, bv=float(self.bfac), uc=self.cell)
+            self.e2 = apply_bfac(f=self.e2, bv=float(self.bfac), uc=self.cell)
+        # apply bfactor
+        self.normmap1 = np.real(np.fft.ifftn(np.fft.ifftshift(self.e1 * fsc_grid_str)))
+        self.normmap2 = np.real(np.fft.ifftn(np.fft.ifftshift(self.e2 * fsc_grid_str)))
+        self.normfull = np.real(np.fft.ifftn(np.fft.ifftshift(self.e0 * fsc_grid_str)))
+
+
+if __name__=="__main__":
+    #path = "/Users/ranganaw/MRC/REFMAC/EMD-6952/emda_test/test_mmcc/new_mmcc/"
+    #fullmap = "emd_6952.map"
+    #model = "modelmap.mrc"
+    resol = 4.
+    path = "/Users/ranganaw/MRC/REFMAC/COVID19/EMD-11203/test_rcc/"
+    halfmap1 = path + "emd_11203_half1.map"
+    halfmap2 = path + "emd_11203_half2.map"
+
+    #mapmodel_rcc(fullmap, model, resol)
+    mapmodel_rcc(halfmap1, halfmap2, resol)
+
+    # calculating RCC
+    #rcc = RealspaceLocalCC()
+    #rcc.hfmap1name = halfmap1
+    #rcc.hfmap2name = halfmap2
+    #rcc.rcc()
+
```

### Comparing `emda-1.1.5/emda/ext/map_fsc.py` & `emda-1.1.6.post1/emda/ext/map_fsc.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/mapfit/curve_fit_3.py` & `emda-1.1.6.post1/emda/ext/mapfit/curve_fit_3.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/mapfit/derivatives.py` & `emda-1.1.6.post1/emda/ext/mapfit/derivatives.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/mapfit/emfit_class.py` & `emda-1.1.6.post1/emda/ext/mapfit/emfit_class.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/mapfit/frequency_marching.py` & `emda-1.1.6.post1/emda/ext/mapfit/frequency_marching.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/mapfit/interp_derivatives.py` & `emda-1.1.6.post1/emda/ext/mapfit/interp_derivatives.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/mapfit/linefit_class.py` & `emda-1.1.6.post1/emda/ext/mapfit/linefit_class.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/mapfit/map_class.py` & `emda-1.1.6.post1/emda/ext/mapfit/map_class.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/mapfit/mapaverage.py` & `emda-1.1.6.post1/emda/ext/mapfit/mapaverage.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 from emda.ext.mapfit import map_class, emfit_class
 
 
 def get_resol(bin_fsc, res_arr):
     bin_fsc = bin_fsc[bin_fsc > 0.1]
     if len(bin_fsc) > 0:
         dist = np.sqrt((bin_fsc - 0.143) ** 2)
-        return res_arr[np.argmin(dist)]
-    else:
-        raise SystemExit("Length of FSC array is zero!!!")
+    return res_arr[np.argmin(dist)]
 
 
 def get_bfac(res_arr, signal):
     from scipy import stats
 
     high_res = 5.5  # Angstrom. This is a hard cutoff.
     res_ub = np.sqrt((res_arr - high_res) ** 2)
@@ -152,66 +150,56 @@
     if slf % 2 != 0:
         slf = slf - 1
     slf = min([len(dist), slf])
     #
     if fit:
         for ifit in range(1, len(emmap1.eo_lst)):
             fobj.write("Fitting set#: " + str(ifit) + " \n")
-            fit = run_fit.run_fit(
+            rotmat, t = run_fit.run_fit(
                 emmap1, smax, rotmat, t, slf, ncycles, ifit, fobj, interp
             )
-            rotmat_lst.append(fit.rotmat)
-            transl_lst.append(fit.t_accum)
+            rotmat_lst.append(rotmat)
+            transl_lst.append(t)
 
         """newsignal.output_rotated_maps(emmap1,
                             rotmat_lst,
                             transl_lst,
                             fobj=fobj)"""
         """newsignal.output_rotated_maps_using_fo(emmap1,
                             rotmat_lst,
                             transl_lst,
                             fobj=fobj)"""
         newsignal.output_rotated_maps_using_fo_allmaps(
             emmap1, rotmat_lst, transl_lst, fobj=fobj
         )
     if not fit:
-        # using normalized Fourier coeffi
+        """# using normalized Fourier coeffi
         cov_lst = []
         # estimating covaraince between current map vs. static map
         for frt in emmap1.fo_lst[1:]:
             bin_stats = \
-                core.fsc.anytwomaps_fsc_covariance(emmap1.fo_lst[0], \
+                fsc.anytwomaps_fsc_covariance(emmap1.fo_lst[0], \
                     frt,emmap1.bin_idx, emmap1.nbin)
             f1f2_fsc, f1f2_covar = bin_stats[0], bin_stats[1]
             # mask f1f2_covar so that anything beyond zero get zeros
             f1f2_covar = set_array(f1f2_covar)
-            cov_lst.append(f1f2_covar) 
-            print(f1f2_fsc)      
-
-        _, _,_,totalvar1,_,eo,= core.fsc.halfmaps_fsc_variance(
-            emmap1.fo_lst[0], emmap1.fo_lst[0], emmap1.bin_idx, emmap1.nbin
-            )
-        _, _,_,totalvar2,_,e1,= core.fsc.halfmaps_fsc_variance(
-            emmap1.fo_lst[1], emmap1.fo_lst[1], emmap1.bin_idx, emmap1.nbin
-            )
-        totalvar = [totalvar1, totalvar2]
+            cov_lst.append(f1f2_covar)        
         averagemaps = utils.avg_and_diffmaps(maps2avg=emmap1.eo_lst,
                                         uc=emmap1.map_unit_cell,
                                         nbin=emmap1.nbin,
                                         sgnl_var=emmap1.signalvar_lst,
-                                        #totl_var=emmap1.totalvar_lst,
-                                        totl_var=totalvar,
+                                        totl_var=emmap1.totalvar_lst,
                                         covar=cov_lst,
                                         hffsc=emmap1.hffsc_lst,
                                         bin_idx=emmap1.bin_idx,
                                         s_grid=emmap1.s_grid,
                                         res_arr=emmap1.res_arr,
-                                        Bf_arr=Bf_arr)
+                                        Bf_arr=Bf_arr)"""
         # using un-normalized Fourier coeffi.
-        #averagemaps = newsignal.avgmaps_using_fo_nofit(emmap1=emmap1, fobj=fobj)
+        averagemaps = newsignal.avgmaps_using_fo_nofit(emmap1=emmap1, fobj=fobj)
         # averagemap output
         utils.output_maps(
             averagemaps=averagemaps,
             com_lst=[],
             t_lst=[],
             r_lst=[],
             unit_cell=emmap1.map_unit_cell,
```

### Comparing `emda-1.1.5/emda/ext/mapfit/mapoverlay.py` & `emda-1.1.6.post1/emda/ext/mapfit/mapoverlay.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/mapfit/newsignal.py` & `emda-1.1.6.post1/emda/ext/mapfit/newsignal.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,27 +408,25 @@
                 q = core.quaternions.get_quaternion(theta_init)
                 q = q / np.sqrt(np.dot(q, q))
                 rotmat = core.quaternions.get_RM(q)
                 if len(emmap1.res_arr) < 50:
                     slf = len(emmap1.res_arr)
                 else:
                     slf = 50
-                fit = run_fit.run_fit(
+                rotmat, trans = run_fit.run_fit(
                     emmap1=emmap1,
                     smax=smax,
                     rotmat=rotmat,
                     t=t_init,
                     slf=slf,
                     ncycles=ncycles,
                     ifit=0,
                     fobj=fobj,
                     interp="linear",
                 )
-                rotmat = fit.rotmat
-                trans = fit.t_accum
                 st, _, _, _ = fcodes_fast.get_st(nx, ny, nz, trans)
                 frt_j_new = utils.get_FRS(cell, rotmat, frt_j * st)[:, :, :, 0]
                 # scale 1st map to 2nd map
                 _, f1f2_fsc = fcodes_fast.calc_covar_and_fsc_betwn_anytwomaps(
                     frt_i, frt_j_new, bin_idx, nbin, 0, nx, ny, nz
                 )
                 # get resolution from fsc
@@ -549,35 +547,35 @@
         emmap1.s_grid,
         res_arr,
         Bf_arr,
     )
     return averagemaps
 
 
-def get_extended_signal(res_arr, signal, bin_fsc, fsc_cutoff=0.3, fobj=None):
+def get_extended_signal(res_arr, signal, bin_fsc, fobj=None):
     from scipy import stats
     from emda.ext.mapfit import rdp_algo
 
     fobj.write("\nSignal extended using B-factor \n")
     bin_fsc_masked = bin_fsc[bin_fsc > 0.0]
     res_arr_masked = res_arr[bin_fsc > 0.0]
-    dist2 = np.sqrt((bin_fsc_masked - fsc_cutoff) ** 2)
+    dist2 = np.sqrt((bin_fsc_masked - 0.3) ** 2)
     uplim = np.argmin(dist2)
     # Need to determine the low and high limits
     x = 1.0 / res_arr_masked[:uplim]
     y = signal[:uplim]
     xc, _ = rdp_algo.run_rdp(x, np.log(y), epsilon=0.01)
     upl = np.argmin(np.sqrt((x - xc[-1]) ** 2))
     lwl = np.argmin(np.sqrt((x - xc[-2]) ** 2))
     s1 = x[lwl:upl]
     sig1 = y[lwl:upl]
     fobj.write("low resol. limit: " + str(res_arr[signal > 0.0][lwl]) + " (A) \n")
     fobj.write("high resol. limit: " + str(res_arr[signal > 0.0][upl]) + " (A) \n")
     slope, intercept, _, _, _ = stats.linregress((s1 * s1) / 4.0, np.log(sig1))
-    bfac = -(abs(slope))
+    bfac = slope
     print("B factor = ", bfac, "Intercept = ", intercept)
     fobj.write("B-factor: " + str(bfac) + " \n")
     fobj.write("Intercept: " + str(intercept) + " \n")
     s = 1.0 / res_arr
     signal_pred = np.exp((bfac / 4) * s ** 2 + intercept)
     new_signal = signal
     new_signal[upl:] = signal_pred[upl:]
```

### Comparing `emda-1.1.5/emda/ext/mapfit/rdp_algo.py` & `emda-1.1.6.post1/emda/ext/mapfit/rdp_algo.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/mapfit/rotmat2quart.py` & `emda-1.1.6.post1/emda/ext/mapfit/rotmat2quart.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/mapfit/run_fit.py` & `emda-1.1.6.post1/emda/ext/mapfit/run_fit.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/mapfit/utils.py` & `emda-1.1.6.post1/emda/ext/mapfit/utils.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/maskmap_class.py` & `emda-1.1.6.post1/emda/ext/maskmap_class.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/overlay.py` & `emda-1.1.6.post1/emda/ext/overlay.py`

 * *Files identical despite different names*

```diff
@@ -630,17 +630,18 @@
             ibin = i
             if ibin % 2 != 0:
                 ibin = ibin - 1
             break
     return ibin
 
 
-def determine_ibin(bin_fsc, cutoff=0.15):
+def determine_ibin(bin_fsc, cutoff=0.05):
     bin_fsc = filter_fsc(bin_fsc)
-    ibin = get_ibin(bin_fsc, cutoff)        
+    ibin = get_ibin(bin_fsc, cutoff)    
+    print("ibin= ", ibin)    
     i = 0
     while ibin < 5:
         cutoff -= 0.01
         ibin = get_ibin(bin_fsc, max([cutoff, 0.1]))
         i += 1
         if i > 100:
             print("Fit starting configurations are too far.")
```

### Comparing `emda-1.1.5/emda/ext/overlay_dev.py` & `emda-1.1.6.post1/emda/ext/sym/refine_symaxis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,250 +1,88 @@
-"""
-Author: "Rangana Warshamanage, Garib N. Murshudov"
-MRC Laboratory of Molecular Biology
-    
-This software is released under the
-Mozilla Public License, version 2.0; see LICENSE.
-"""
-
+# lock rotation
 from __future__ import absolute_import, division, print_function, unicode_literals
 from timeit import default_timer as timer
 import numpy as np
+import sys, math
 import fcodes_fast
-import emda.ext.utils as utils
 import emda.emda_methods as em
-from numpy.fft import fftn, fftshift, ifftshift, ifftn, ifftshift
+from numpy.fft import fftn, ifftn, fftshift, ifftshift
+from emda.ext.mapfit import map_class
 from emda import core
 from emda.core import quaternions
-from emda.ext.mapfit import utils as maputils
-
-timeit = False
+from emda.ext.mapfit.utils import (
+    get_FRS,
+    create_xyz_grid,
+    get_xyz_sum,
+    set_dim_even,
+)
+from emda.core.quaternions import derivatives_wrt_q
+from emda.ext.mapfit.derivatives import get_dqda, new_dFs2
+from scipy.optimize import minimize_scalar
+from matplotlib import pyplot as plt
+from emda.ext.mapfit import frequency_marching
+from emda.ext.sym import run_proshade as proshade
+from more_itertools import sort_together
+#from rebox_map import reboxmap
 
+mapout = True
 
 class EmmapOverlay:
-    def __init__(self, map_list, nocom=False, mask_list=None, modelres=None):
-        self.map_list = map_list
-        self.mask_list = mask_list
-        self.modelres = modelres
+    def __init__(self, imap, imask=None):
+        self.imap = imap
+        self.imask = imask
         self.map_unit_cell = None
         self.map_origin = None
         self.map_dim = None
         self.pixsize = None
         self.arr_lst = []
-        self.msk_lst = []
-        self.carr_lst = []
+        self.arr_original = None
         self.ceo_lst = None
         self.cfo_lst = None
         self.cbin_idx = None
         self.cdim = None
         self.cbin = None
-        self.com = not(nocom)
+        self.com = True
         self.com1 = None
-        self.comlist = []
         self.box_centr = None
-        self.fhf_lst = None
+        self.fhf_lst = []
         self.nbin = None
         self.res_arr = None
         self.bin_idx = None
         self.fo_lst = None
         self.eo_lst = None
         self.totalvar_lst = None
-        self.gemmi = False
+        self.q_init_list = []
 
-    def _check_inputs(self):
-        if not self.map_list:
-            raise SystemExit("Map list is empty.")
-        if len(self.map_list) < 2:
-            raise SystemExit("At least 2 maps are needed.")
-        for istr in self.map_list:
-            if istr.endswith((".cif", ".pdb", ".ent")):
-                if self.modelres is None:
-                    raise SystemExit("Please specify resolution for modelbased map.")
-        if self.mask_list is not None:
-            if len(self.map_list) != len(self.mask_list):
-                raise SystemExit("map_list and mask_list must have the same size!")  
-
-    def load_maps(self):
-        from scipy import ndimage
-        from scipy.ndimage.interpolation import shift
-
-        cmask = False
-        fhf_lst = []
-        self._check_inputs()
-        if self.mask_list is not None:
-            for i in range(len(self.mask_list)):
-                if i == 0:
-                    _, mask, _ = em.get_data(self.mask_list[i])
-                    mask = maputils.set_dim_even(mask)
-                    uc, arr, origin = em.get_data(self.map_list[i])
-                    arr = maputils.set_dim_even(arr)
-                    try:
-                        assert arr.shape == mask.shape
-                    except AssertionError:
-                        print('arr shape: ', arr.shape)
-                        print('mask shape', mask.shape)
-                        raise SystemExit("Map and Mask Dimension mismatched!")
-                    arr = arr * mask
-                    nx, ny, nz = arr.shape
-                    map_origin = origin
-                    uc_target = uc
-                    target_dim = arr.shape
-                    target_pix_size = []
-                    for j in range(3):
-                        target_pix_size.append(uc_target[j] / target_dim[j])
-                    if cmask:
-                        corner_mask = maputils.remove_unwanted_corners(uc, target_dim)
-                    else:
-                        corner_mask = 1.0
-                    if self.com:
-                        com1 = ndimage.measurements.center_of_mass(arr * (arr >= 0.0))
-                        print("COM: ", com1)
-                        box_centr = (nx // 2, ny // 2, nz // 2)
-                        self.com1, self.box_centr = com1, box_centr
-                        self.comlist.append(com1)
-                        arr_mvd = shift(arr, np.subtract(box_centr, com1))
-                        mask_mvd = shift(mask, np.subtract(box_centr, com1))
-                        self.arr_lst.append(arr_mvd * corner_mask)
-                        self.msk_lst.append(mask_mvd)
-                        fhf_lst.append(fftshift(fftn(fftshift(arr_mvd * corner_mask))))
-                    else:
-                        self.arr_lst.append(arr * corner_mask)
-                        self.msk_lst.append(mask)
-                        fhf_lst.append(fftshift(fftn(fftshift(arr * corner_mask))))
-                else:
-                    uc, arr, origin = em.get_data(
-                        self.map_list[i],
-                        resol=self.modelres,
-                        dim=target_dim,
-                        uc=uc_target,
-                        maporigin=map_origin,
-                        gemmi=self.gemmi,
-                    )
-                    arr = maputils.set_dim_even(arr)
-                    print("origin: ", origin)
-                    _, mask, _ = em.get_data(self.mask_list[i])
-                    mask = maputils.set_dim_even(mask)
-                    try:
-                        assert arr.shape == mask.shape
-                    except AssertionError:
-                        print('arr shape: ', arr.shape)
-                        print('mask shape', mask.shape)
-                        raise SystemExit("Map and Mask Dimension mismatched!")
-                    arr = arr * mask
-                    curnt_pix_size = []
-                    for j in range(3):
-                        curnt_pix_size.append(uc[j] / arr.shape[j])
-                    arr = core.iotools.resample2staticmap(
-                        curnt_pix=curnt_pix_size,
-                        targt_pix=target_pix_size,
-                        targt_dim=target_dim,
-                        arr=arr,
-                    )
-                    mask = core.iotools.resample2staticmap(
-                        curnt_pix=curnt_pix_size,
-                        targt_pix=target_pix_size,
-                        targt_dim=target_dim,
-                        arr=mask,
-                    )
-                    if self.com:
-                        com1 = ndimage.measurements.center_of_mass(arr * (arr >= 0.0))
-                        print("COM: ", com1)
-                        self.comlist.append(com1)
-                        arr = shift(arr, np.subtract(box_centr, com1))
-                        mask = shift(mask, np.subtract(box_centr, com1))
-                    self.arr_lst.append(arr * corner_mask)
-                    self.msk_lst.append(mask)
-                    fhf_lst.append(fftshift(fftn(fftshift(arr * corner_mask))))
-            self.pixsize = target_pix_size
-            self.map_origin = map_origin
-            self.map_unit_cell = uc_target
-            self.map_dim = target_dim
-            self.fhf_lst = fhf_lst
-        else:
-            for i in range(len(self.map_list)):
-                if i == 0:
-                    uc, arr, origin = em.get_data(self.map_list[i])
-                    # threshold map
-                    #arr = threshold_map(arr=arr, dthresh=0.03)
-                    arr = maputils.set_dim_even(arr)
-                    print("origin: ", origin)
-                    nx, ny, nz = arr.shape
-                    map_origin = origin
-                    uc_target = uc
-                    target_dim = arr.shape
-                    target_pix_size = []
-                    for j in range(3):
-                        target_pix_size.append(uc_target[j] / target_dim[j])
-                    if self.com:
-                        com1 = ndimage.measurements.center_of_mass(arr * (arr >= 0.0))
-                        self.comlist.append(com1)
-                        print("COM before centering: ", com1)
-                        box_centr = (nx // 2, ny // 2, nz // 2)
-                        print("BOX center: ", box_centr)
-                        self.com1 = com1
-                        self.box_centr = box_centr
-                        arr = shift(arr, np.subtract(box_centr, com1))
-                        self.arr_lst.append(arr)
-                        core.iotools.write_mrc(
-                            arr, "static_centered.mrc", uc_target, map_origin
-                        )
-                        print(
-                            "COM after centering: ",
-                            ndimage.measurements.center_of_mass(arr * (arr >= 0.0)),
-                        )
-                    self.arr_lst.append(arr)
-                    fhf_lst.append(fftshift(fftn(fftshift(arr))))
-                else:
-                    uc, arr, origin = em.get_data(
-                        self.map_list[i],
-                        resol=self.modelres,
-                        dim=target_dim,
-                        uc=uc_target,
-                        maporigin=map_origin,
-                        gemmi=self.gemmi,
-                    )
-                    #arr = threshold_map(arr=arr) # threshold map
-                    arr = maputils.set_dim_even(arr)
-                    curnt_pix_size = []
-                    for j in range(3):
-                        curnt_pix_size.append(uc[j] / arr.shape[j])
-                    arr = core.iotools.resample2staticmap(
-                        curnt_pix=curnt_pix_size,
-                        targt_pix=target_pix_size,
-                        targt_dim=target_dim,
-                        arr=arr,
-                    )
-                    if self.com:
-                        com1 = ndimage.measurements.center_of_mass(arr * (arr >= 0.0))
-                        self.comlist.append(com1)
-                        print("COM: ", com1)
-                        arr = shift(arr, np.subtract(box_centr, com1))
-                        core.iotools.write_mrc(
-                            arr, "moving_centered.mrc", uc_target, map_origin
-                        )
-                        print(
-                            "COM after centering: ",
-                            ndimage.measurements.center_of_mass(arr * (arr >= 0.0)),
-                        )
-                    self.arr_lst.append(arr)
-                    fhf_lst.append(fftshift(fftn(fftshift(arr))))
-            self.pixsize = target_pix_size
-            self.map_origin = map_origin
-            self.map_unit_cell = uc_target
-            self.map_dim = target_dim
-            self.fhf_lst = fhf_lst
+    def get_maps(self):
+        uc, arr, origin = em.get_data(self.imap)
+        arr = set_dim_even(arr)
+        self.arr_original = arr
+        com = em.center_of_mass_density(arr)
+        print("com:", com)
+        nx, ny, nz = arr.shape
+        box_centr = (nx // 2, ny // 2, nz // 2)
+        self.box_centr = box_centr
+        self.com1 = com
+        if self.com:
+            arr = em.shift_density(arr, np.subtract(box_centr, com))
+            print("com after centering:", em.center_of_mass_density(arr))
+        self.arr_lst.append(arr)
+        self.fhf_lst.append(fftshift(fftn(fftshift(arr))))
+        self.pixsize = uc[0] / arr.shape[0]
+        self.map_origin = origin
+        self.map_unit_cell = uc
+        self.map_dim = arr.shape
 
     def calc_fsc_from_maps(self):
         # function for only two maps fitting
         nmaps = len(self.fhf_lst)
-        print('nmaps: ', nmaps)
         fFo_lst = []
         fEo_lst = []
         fBTV_lst = []
-
         self.nbin, self.res_arr, self.bin_idx = core.restools.get_resolution_array(
             self.map_unit_cell, self.fhf_lst[0]
         )
         for i in range(nmaps):
             _, _, _, totalvar, fo, eo = core.fsc.halfmaps_fsc_variance(
                 self.fhf_lst[i], self.fhf_lst[i], self.bin_idx, self.nbin
             )
@@ -254,791 +92,1211 @@
         self.fo_lst = fFo_lst
         self.eo_lst = fEo_lst
         self.totalvar_lst = fBTV_lst
 
 
 def cut_resolution_for_linefit(f_list, bin_idx, res_arr, smax):
     # Making data for map fitting
-    f_arr = np.asarray(f_list, dtype='complex')
+    f_arr = np.asarray(f_list, dtype="complex")
     nx, ny, nz = f_list[0].shape
     cbin = cx = smax
     dx = int((nx - 2 * cx) / 2)
     dy = int((ny - 2 * cx) / 2)
     dz = int((nz - 2 * cx) / 2)
-    cBIdx = bin_idx[dx : dx + 2 * cx, dy : dy + 2 * cx, dz : dz + 2 * cx]
+    cBIdx = bin_idx[dx: dx + 2 * cx, dy: dy + 2 * cx, dz: dz + 2 * cx]
     fout = fcodes_fast.cutmap_arr(
         f_arr, bin_idx, cbin, 0, len(res_arr), nx, ny, nz, len(f_list)
-    )[:, dx : dx + 2 * cx, dy : dy + 2 * cx, dz : dz + 2 * cx]
+    )[:, dx: dx + 2 * cx, dy: dy + 2 * cx, dz: dz + 2 * cx]
     return fout, cBIdx, cbin
 
 
 class linefit:
     def __init__(self):
         self.e0 = None
         self.e1 = None
         self.bin_idx = None
         self.nbin = None
-        self.step = None
-        self.q_prev = None
-        self.t = None
-        self.q_init = np.array([1.0, 0.0, 0.0, 0.0], dtype=np.float64)
+        self.axis = None
+        self.angle_list = []
+        self.step_axis = None
+        self.step_t = None
+        self.t_ini = None
+        self.alpha_t = None
+        self.axis_ini = None
 
     def get_linefit_static_data(self, e_list, bin_idx, res_arr, smax):
         if len(e_list) == 2:
-            eout, self.bin_idx, self.nbin = cut_resolution_for_linefit(e_list, bin_idx, res_arr, smax)
+            eout, self.bin_idx, self.nbin = cut_resolution_for_linefit(
+                e_list, bin_idx, res_arr, smax
+            )
         else:
             print("len(e_list: ", len(e_list))
             raise SystemExit()
-        self.e0 = eout[0,:,:,:]
-        self.e1 = eout[1,:,:,:]
+        self.e0 = eout[0, :, :, :]
+        self.e1 = eout[1, :, :, :]
+
+    def get_quaternion(self, axis, angle_i):
+        rv = axis
+        s = math.sin(angle_i / 2.0)
+        q1, q2, q3 = rv[0] * s, rv[1] * s, rv[2] * s
+        q0 = math.cos(angle_i / 2.0)
+        q = np.array([q0, q1, q2, q3], dtype=np.float64)
+        return q
 
     def get_fsc_wght(self, e0, ert, bin_idx, nbin):
         cx, cy, cz = e0.shape
         bin_stats = core.fsc.anytwomaps_fsc_covariance(e0, ert, bin_idx, nbin)
         fsc, _ = bin_stats[0], bin_stats[1]
-        #fsc = np.array(fsc, dtype=np.float64, copy=False)
-        fsc = fsc - 1e-5 # as aregularizer
-        fsc = fsc / (1 - fsc)#**2)
+        fsc = np.array(fsc, dtype=np.float64, copy=False)
         w_grid = fcodes_fast.read_into_grid(bin_idx, fsc, nbin, cx, cy, cz)
-        #w_grid = np.array(w_grid, dtype=np.float64, copy=False)
-        """ w_grid = fcodes_fast.fsc_weight_calculation(f1=e0,
-                                    f2=ert,
-                                    bin_idx=bin_idx,
-                                    nbin=nbin,
-                                    mode=0,
-                                    nx=cx,
-                                    ny=cy,
-                                    nz=cz) """
+        w_grid = np.array(w_grid, dtype=np.float64, copy=False)
         return w_grid
 
     def func(self, i):
-        tmp = np.insert(np.asarray(self.step, 'float') * i, 0, 0.0)
-        q = tmp + np.asarray(self.q_prev, 'float')
-        q = q / np.sqrt(np.dot(q, q))
-        rotmat = quaternions.get_RM(q)
-        ers = maputils.get_FRS(rotmat, self.e1, interp="linear")
-        w_grid = self.get_fsc_wght(self.e0, ers[:, :, :, 0], self.bin_idx, self.nbin) 
-        #w_grid = 1.0  
-        fval = np.real(np.sum(w_grid * self.e0 * np.conjugate(ers[:, :, :, 0])))
+        step_ax = self.step_axis * i
+        self.axis = getaxis(self.axis_ini, step_ax)
+        fval = 0.0
+        q_i = self.get_quaternion(self.axis, self.angle_list[0])
+        rotmat = core.quaternions.get_RM(q_i)
+        ers = get_FRS(rotmat, self.e0, interp="linear")
+        w_grid = self.get_fsc_wght(
+            self.e0, ers[:, :, :, 0], self.bin_idx, self.nbin)
+        fval = np.real(np.sum(w_grid * self.e0 *
+                              np.conjugate(ers[:, :, :, 0])))
         return -fval
 
     def scalar_opt(self, t=None):
-        from scipy.optimize import minimize_scalar
-
         f = self.func
-        res = minimize_scalar(f, method="golden", bracket=(-1, 1))
+        res = minimize_scalar(f, method="brent")
         return res.x
 
-    def func_t(self, i):
-        nx, ny, nz = self.e0.shape
-        #t = self.t + self.step * i
-        t = np.asarray(self.step, 'float') * i
-        st, _, _, _ = fcodes_fast.get_st(nx, ny, nz, t)
-        e1_t = self.e1 * st
-        w_grid = self.get_fsc_wght(self.e0, e1_t, self.bin_idx, self.nbin)
-        fval = np.sum(w_grid * self.e0 * np.conjugate(e1_t))
-        return -fval.real
 
-    def scalar_opt_trans(self):
-        from scipy.optimize import minimize_scalar
+def derivatives(e0, e1, w_grid, w2_grid, q, sv, xyz, xyz_sum, vol):
 
-        start = timer()
-        f = self.func_t
-        res = minimize_scalar(f, method="brent")
-        end = timer()
-        #print("time for trans linefit: ", end-start)
-        return res.x
+
+    nx, ny, nz = e0.shape
+    sv_np = np.zeros((nx, ny, nz, 3), dtype=np.float64)
+    for i in range(3):
+        sv_np[:, :, :, i] = sv[i]
+    dRdq = derivatives_wrt_q(q)
+    dqda = get_dqda(q)
+    dFRs = new_dFs2(np.real(np.fft.ifftn(np.fft.ifftshift(e1))), xyz, vol)
+    df_val, ddf_val = fcodes_fast.calc_derivatives(
+        e0, e1, w_grid, w2_grid, sv_np, dFRs, dRdq, xyz_sum, vol, nx, ny, nz
+    )
+    ddf_val_inv = np.linalg.pinv(ddf_val)
+    step = ddf_val_inv.dot(-df_val)
+    # get axis derivatives
+    df_ax = np.zeros(3, dtype="float")
+    ddf_ax = np.zeros((3, 3), dtype="float")
+    dqda = get_dqda(q)
+    for i in range(len(dqda)):
+        df_ax[i] = df_val[3 + i] * dqda[i]
+        for j in range(len(dqda)):
+            ddf_ax[i, j] = ddf_val[3 + i, 3 + j] * dqda[i] * dqda[j]
+    ddf_ax_inv = np.linalg.pinv(ddf_ax)
+    step_ax = ddf_ax_inv.dot(-df_ax)
+    return step[:3], step_ax
+
+
+def derivatives_translation(e0, e1, wgrid, w2grid, sv):
+    PI = np.pi
+    tp2 = (2.0 * PI) ** 2
+    tpi = 2.0 * PI * 1j
+    # translation derivatives
+    df = np.zeros(3, dtype="float")
+    ddf = np.zeros((3, 3), dtype="float")
+    for i in range(3):
+        df[i] = np.real(
+            np.sum(wgrid * e0 * np.conjugate(e1 * tpi * sv[i, :, :, :])))
+        for j in range(3):
+            if i == 0 or (i > 0 and j >= i):
+                ddf[i, j] = -tp2 * \
+                    np.sum(w2grid * sv[i, :, :, :] * sv[j, :, :, :])
+            else:
+                ddf[i, j] = ddf[j, i]
+    ddf_inv = np.linalg.pinv(ddf)
+    step = ddf_inv.dot(-df)
+    return step
+
+
+def getaxis(axis_ini, step_ax):
+    axmax = np.argmax(abs(axis_ini))
+    if axmax == 0:
+        ay, az = axis_ini[1] + step_ax[1], axis_ini[2] + step_ax[2]
+        ax = np.sqrt(1.0 - ay * ay - az * az)
+    elif axmax == 1:
+        ax, az = axis_ini[0] + step_ax[0], axis_ini[2] + step_ax[2]
+        ay = np.sqrt(1.0 - ax * ax - az * az)
+    elif axmax == 2:
+        ax, ay = axis_ini[0] + step_ax[0], axis_ini[1] + step_ax[1]
+        az = np.sqrt(1.0 - ax * ax - ay * ay)
+    return np.array([ax, ay, az], dtype="float")
 
 
-class Bfgs:
+class linefit2:
     def __init__(self):
         self.e0 = None
-        #self.e1 = None
-        self.ert = None
-        self.wgrid = None
-        self.sv = None
-        self.q = None
-        self.xyz = None
+        self.e1 = None
         self.bin_idx = None
         self.nbin = None
-        self.binfsc = None
-        self.avgfsc = None
         self.step = None
         self.q_prev = None
-        self.cell = None
+        self.t = None
+        self.q_init = np.array([1.0, 0.0, 0.0, 0.0], dtype=np.float64)
 
     def get_linefit_static_data(self, e_list, bin_idx, res_arr, smax):
         if len(e_list) == 2:
-            eout, self.bin_idx, self.nbin = cut_resolution_for_linefit(e_list, bin_idx, res_arr, smax)
+            eout, self.bin_idx, self.nbin = cut_resolution_for_linefit(
+                e_list, bin_idx, res_arr, smax
+            )
         else:
             print("len(e_list: ", len(e_list))
             raise SystemExit()
-        self.e0 = eout[0,:,:,:]
-        self.ert = eout[1,:,:,:]
-        t = np.array([0.0, 0.0, 0.0], dtype="float")
-        nx, ny, nz = self.e0.shape
-        _, s1, s2, s3 = fcodes_fast.get_st(nx, ny, nz, t)
-        self.sv = np.array([s1, s2, s3])
+        self.e0 = eout[0, :, :, :]
+        self.e1 = eout[1, :, :, :]
+
+    def get_fsc_wght(self, e0, ert, bin_idx, nbin):
+        cx, cy, cz = e0.shape
+        bin_stats = core.fsc.anytwomaps_fsc_covariance(e0, ert, bin_idx, nbin)
+        fsc, _ = bin_stats[0], bin_stats[1]
+        fsc = np.array(fsc, dtype=np.float64, copy=False)
+        w_grid = fcodes_fast.read_into_grid(bin_idx, fsc, nbin, cx, cy, cz)
+        w_grid = np.array(w_grid, dtype=np.float64, copy=False)
+        return w_grid
 
-    def derivatives_rotation(self):
-        from emda.core.quaternions import derivatives_wrt_q
-        from emda.ext.overlay import get_dfs
-        # rotation derivatives
+    def func_t(self, i):
         nx, ny, nz = self.e0.shape
-        vol = nx * ny * nz
-        self.xyz = maputils.create_xyz_grid(self.cell, self.e0.shape)
-        dFRS = get_dfs(np.real(np.fft.ifftn(np.fft.ifftshift(self.ert))), self.xyz, vol)
-        dRdq = derivatives_wrt_q(self.q)
-        df = np.zeros(3, dtype="float")
-        for i in range(3):
-            a = np.zeros((3, 3), dtype="float")
-            for k in range(3):
-                for l in range(3):
-                    if k == 0 or (k > 0 and l >= k):
-                        a[k, l] = np.sum(
-                            self.wgrid
-                            * np.real(
-                                np.conjugate(self.e0)
-                                * (dFRS[:, :, :, k] * self.sv[l, :, :, :] * dRdq[i, k, l])
-                            )
-                        )
-                    else:
-                        a[k, l] = a[l, k]
-            df[i] = np.sum(a)
-        return df
-
-    def derivatives_translation(self):
-        # translation derivatives
-        tpi = (2.0 * np.pi * 1j)
-        df = np.zeros(3, dtype='float')
-        for i in range(3):
-            df[i] = np.real(np.sum(self.wgrid * self.e0 * np.conjugate(self.ert * tpi * self.sv[i,:,:,:])))
-        print(df)
-        return df
-
-    def gradient(self):
-        df_r = self.derivatives_rotation()
-        #df_t = self.derivatives_translation()
-        #return np.concatenate((df_r, df_t), axis=0)
-        return df_r
-
-    def calc_fsc(self):
-        binfsc, _, bincounts = core.fsc.anytwomaps_fsc_covariance(
-            self.e0, self.ert, self.bin_idx, self.nbin)
-        #print('binfsc:', binfsc)
-        #print('bincount', bincounts)
-        self.binfsc = binfsc
-        self.avgfsc = utils.get_avg_fsc(binfsc=binfsc, bincounts=bincounts)
-
-    def get_wght(self): 
-        nz, ny, nx = self.e0.shape
-        val_arr = np.zeros((self.nbin, 2), dtype='float')
-        val_arr[:,0] = self.binfsc #/ (1 - self.binfsc ** 2)
-        self.wgrid = fcodes_fast.read_into_grid2(self.bin_idx,
-            val_arr, self.nbin, nz, ny, nx)[:,:,:,0]
-
-    #3. functional
-    def functional(self, x0):
-        tmp = np.insert(np.asarray(self.step, 'float') * x0[0], 0, 0.0)
-        q = tmp + np.asarray(self.q_prev, 'float')
-        q = q / np.sqrt(np.dot(q, q))
-        rotmat = core.quaternions.get_RM(q)
-        self.ert = maputils.get_FRS(rotmat, self.ert, interp="linear")[:, :, :, 0]
-        self.calc_fsc()
-        self.get_wght()
-        #w_grid = self.get_fsc_wght(self.e0, ers[:, :, :, 0], self.bin_idx, self.nbin)   
-        #fval = np.real(np.sum(w_grid * self.e0 * np.conjugate(ers[:, :, :, 0])))
-        fval = np.sum(self.wgrid * self.e0 * np.conjugate(self.ert))
-        print('fval: ', fval.real)
+        t = self.step * i
+        st, _, _, _ = fcodes_fast.get_st(nx, ny, nz, t)
+        e1_t = self.e1 * st
+        w_grid = self.get_fsc_wght(self.e0, e1_t, self.bin_idx, self.nbin)
+        fval = np.sum(w_grid * self.e0 * np.conjugate(e1_t))
         return -fval.real
 
-    #3. optimize using BFGS
-    def optimize(self):
-        from scipy.optimize import minimize
-        self.calc_fsc()
-        self.get_wght()
-        f = self.functional
-        grad = self.gradient()
-        result = minimize(fun=f, x0=np.array([1.0], 'float'), method='BFGS', jac=self.gradient)
-        return result.x
-
-
-
-def get_dfs(mapin, xyz, vol):
-    nx, ny, nz = mapin.shape
-    dfs = np.zeros(shape=(nx, ny, nz, 3), dtype=np.complex64)
-    for i in range(3):
-        #dfs[:, :, :, i] = np.fft.fftshift(
-        #    (1 / vol) * 2j * np.pi * np.fft.fftn(mapin * xyz[i])
-        #)
-        dfs[:, :, :, i] = np.fft.fftshift(
-            2j * np.pi * np.fft.fftn(mapin * xyz[i])
-        )
-        #dfs[:, :, :, i] = np.fft.fftshift(
-        #    (np.pi / vol) * 2j * np.fft.fftn(mapin * xyz[:,:,:,i])
-        #)
-    return dfs
-
-
-def derivatives_rotation(e0, e1, cfo, wgrid, sv, q, xyz, xyz_sum, pix=None):
-    from emda.core.quaternions import derivatives_wrt_q
-
-    # rotation derivatives
-    tp2 = (2.0 * np.pi) ** 2
-    nx, ny, nz = e0.shape
-    vol = nx * ny * nz
-    #vol = nx * pix[0] * ny * pix[1] * nz * pix[2]
-    dFRS = get_dfs(np.real(np.fft.ifftn(np.fft.ifftshift(e1))), xyz, vol)
-    #dFRS = get_dfs(np.real(np.fft.ifftn(np.fft.ifftshift(cfo))), xyz, vol)
-    dRdq = derivatives_wrt_q(q)
-    df = np.zeros(3, dtype="float")
-    ddf = np.zeros((3, 3), dtype="float")
-    for i in range(3):
-        a = np.zeros((3, 3), dtype="float")
-        for k in range(3):
-            for l in range(3):
-                if k == 0 or (k > 0 and l >= k):
-                    a[k, l] = np.sum(
-                        wgrid
-                        * np.real(
-                            np.conjugate(e0)
-                            * (dFRS[:, :, :, k] * sv[l, :, :, :] * dRdq[i, k, l])
-                        )
-                    )
-                else:
-                    a[k, l] = a[l, k]
-        df[i] = np.sum(a)
-    """ wfsc = wgrid * np.real(np.conjugate(e0) * e1)
-    for i in range(3):
-        for j in range(3):
-            if i == 0 or (i > 0 and j >= i):
-                b = np.zeros((3, 3), dtype="float")
-                n = -1
-                for k in range(3):
-                    for l in range(3):
-                        if k == 0 or (k > 0 and l >= k):
-                            n += 1
-                            b[k, l] = (
-                                (-tp2 / vol)
-                                * xyz_sum[n]
-                                * np.sum(
-                                    wfsc
-                                    * sv[k, :, :, :]
-                                    * sv[l, :, :, :]
-                                    * dRdq[i, k, l]
-                                    * dRdq[j, k, l]
-                                )
-                            )
-                        else:
-                            b[k, l] = b[l, k]
-                ddf[i, j] = np.sum(b)
-            else:
-                ddf[i, j] = ddf[j, i] """
-    from emda.ext.mapfit.derivatives import rotation2nd_derivative
-    ddf = rotation2nd_derivative(e0, e1, wgrid, sv, q, xyz, vol)
-    ddf_inv = np.linalg.pinv(ddf)
-    step = ddf_inv.dot(-df)
-    return step
-
-
-def derivatives_translation(e0, e1, wgrid, w2grid, sv):
-    PI = np.pi
-    tp2 = (2.0 * PI)**2
-    tpi = (2.0 * PI * 1j)
-    start = timer()
-    # translation derivatives
-    df = np.zeros(3, dtype='float')
-    ddf = np.zeros((3,3), dtype='float')
-    for i in range(3):
-        df[i] = np.real(np.sum(wgrid * e0 * np.conjugate(e1 * tpi * sv[i,:,:,:])))
-        for j in range(3):
-            if(i==0 or (i>0 and j>=i)):
-                ddf[i,j] = -tp2 * np.sum(w2grid * sv[i,:,:,:] * sv[j,:,:,:])
-            else:
-                ddf[i,j] = ddf[j,i]
-    ddf_inv = np.linalg.pinv(ddf)
-    step = ddf_inv.dot(-df)
-    end = timer()
-    #print("time for trans deriv. ", end-start)
-    return step
+    def scalar_opt_trans(self):
+        f = self.func_t
+        res = minimize_scalar(f, method="brent")
+        return res.x
 
 
 class EmFit:
     def __init__(self, mapobj, interp="linear", dfs=None):
         self.mapobj = mapobj
-        self.cut_dim = mapobj.cdim
         self.ful_dim = mapobj.map_dim
         self.cell = mapobj.map_unit_cell
         self.pixsize = mapobj.pixsize
         self.origin = mapobj.map_origin
         self.interp = interp
         self.dfs = dfs
+        self.cut_dim = mapobj.cdim  # mapobj.map_dim
+        self.nbin = mapobj.cbin  # mapobj.nbin
+        self.bin_idx = mapobj.cbin_idx  # mapobj.bin_idx
+        self.res_arr = mapobj.res_arr[: self.nbin]  # mapobj.res_arr
         self.w_grid = None
         self.fsc = None
         self.sv = None
         self.t = None
         self.st = None
         self.step = None
         self.q = None
-        self.q_accum = None
-        self.q_final_list = []
+        self.axis = None
+        self.angle = None
         self.rotmat = None
         self.t_accum = None
         self.ert = None
         self.frt = None
-        self.cfo = None
-        self.crt = None
         self.e0 = None
         self.e1 = None
         self.w2_grid = None
         self.fsc_lst = []
-        self.le0 = None
-        self.le1 = None
-        self.lbinindx = None
-        self.lnbin = None
-
-    def calc_fsc(self):
-        binfsc, _, bincounts = core.fsc.anytwomaps_fsc_covariance(
-            self.e0, self.ert, self.mapobj.cbin_idx, self.mapobj.cbin)
-        #print('binfsc:', binfsc)
-        #print('bincount', bincounts)
-        fsc_avg = utils.get_avg_fsc(binfsc=binfsc, bincounts=bincounts)
-        return [binfsc, fsc_avg]
+        self.avg_fsc = None
+        self.q_final_list = []
+        self.t_final_list = []
+        self.axis_final_list = []
+
+    def calc_fsc(self, e1):
+        fsc = core.fsc.anytwomaps_fsc_covariance(self.e0, e1, self.bin_idx, self.nbin)[
+            0
+        ]
+        return fsc
+
+    def calc_fsc_t(self, fstatic, frotated, t):
+        cx, cy, cz = fstatic.shape
+        st, s1, s2, s3 = fcodes_fast.get_st(cx, cy, cz, t)
+        sv = np.array([s1, s2, s3])
+        frt = frotated * st
+        fsc = core.fsc.anytwomaps_fsc_covariance(fstatic, frt, self.bin_idx, self.nbin)[
+            0
+        ]
+        return frt, fsc, sv
+
+    def rotatemap(self, rotmat, t, smax_lf):
+        estatic = self.mapobj.ceo_lst[0]
+        fstatic = self.mapobj.cfo_lst[0]
+        erotated = get_FRS(rotmat, estatic, interp=self.interp)[:, :, :, 0]
+        frotated = get_FRS(rotmat, fstatic, interp=self.interp)[:, :, :, 0]
+        # optimize translation
+        for i in range(1):
+            ert, fsc, sv = self.calc_fsc_t(estatic, erotated, t)
+            w_grid, w2_grid = self.get_wght(fsc)
+            fval = np.sum(w_grid * estatic * np.conjugate(ert))
+            # print(i, fval.real, t)
+            step = derivatives_translation(estatic, ert, w_grid, w2_grid, sv)
+            lft = linefit2()
+            lft.get_linefit_static_data(
+                [estatic, ert], self.bin_idx, self.mapobj.res_arr, smax_lf
+            )
+            lft.step = step
+            alpha = lft.scalar_opt_trans()
+            t = t + step * alpha
+        cx, cy, cz = fstatic.shape
+        st, s1, s2, s3 = fcodes_fast.get_st(cx, cy, cz, t)
+        ert = erotated * st
+        return ert, sv, t
 
-    def get_wght(self): 
+    def get_wght(self, fsc):
         cx, cy, cz = self.e0.shape
-        val_arr = np.zeros((self.mapobj.cbin, 2), dtype='float')
-        val_arr[:,0] = self.fsc #/ (1 - self.fsc ** 2)
-        fsc_sqd = self.fsc ** 2
-        fsc_combi = fsc_sqd #/ (1 - fsc_sqd)
-        val_arr[:,1] = fsc_combi
-        wgrid = fcodes_fast.read_into_grid2(self.mapobj.cbin_idx,val_arr, self.mapobj.cbin, cx, cy, cz)
-        return wgrid[:,:,:,0], wgrid[:,:,:,1]
+        w_grid = fcodes_fast.read_into_grid(
+            self.bin_idx,
+            fsc,  # fsc / (1 - fsc ** 2),
+            self.nbin,
+            cx,
+            cy,
+            cz,
+        )
+        fsc_sqd = fsc ** 2
+        fsc_combi = fsc_sqd,  # fsc_sqd / (1 - fsc_sqd)
+        w2_grid = fcodes_fast.read_into_grid(
+            self.bin_idx, fsc_combi, self.nbin, cx, cy, cz
+        )
+        return w_grid, w2_grid
 
-    def functional(self):
-        fval = np.sum(self.w_grid * self.e0 * np.conjugate(self.ert))
+    def functional(self, w_grid, ert):
+        fval = np.sum(w_grid * self.e0 * np.conjugate(ert))
         return fval.real
 
-    def minimizer(self, ncycles, t, rotmat, ifit, smax_lf, fobj=None, q_init=None):
-        tol = 1e-2
+    def get_quaternion(self, angle_i):
+        rv = self.axis
+        s = math.sin(angle_i / 2.0)
+        q1, q2, q3 = rv[0] * s, rv[1] * s, rv[2] * s
+        q0 = math.cos(angle_i / 2.0)
+        q = np.array([q0, q1, q2, q3], dtype=np.float64)
+        return q
+
+    def minimizer(self, ncycles, t_init, q_init_list, smax_lf):
         fsc_lst = []
         fval_list = []
-        t = np.asarray(t, 'float')
-        self.e0 = self.mapobj.ceo_lst[0]  # Static map e-data for fit
-        self.e1 = self.mapobj.ceo_lst[1]
-        self.cfo = self.mapobj.cfo_lst[0]
-        cx, cy, cz = self.e0.shape
-        xyz = maputils.create_xyz_grid(self.cell, self.cut_dim)
-        #xyz = fcodes_fast.get_xyz(self.cell, cx, cy, cz)
-        xyz_sum = maputils.get_xyz_sum(xyz)
-        if q_init is None:
-            q_init = np.array([1.0, 0.0, 0.0, 0.0], dtype=np.float64)
-        print("Cycle#   ", "Fval  ", "Rot(deg)  ", "Trans(A)  ", "avg(FSC)")
-        assert np.ndim(rotmat) == 2
-        q0 = quaternions.rot2quart(rotmat)
+        q_list = []
+        t_list = []
+        nfit = len(q_init_list)
+        print("Refinement started...")
+        self.e0 = self.mapobj.ceo_lst[0]
+        self.e1 = self.e0
+        fstatic = self.mapobj.cfo_lst[0]
+        if mapout:
+            print("Saving static map")
+            data2write = np.real(ifftshift(ifftn(ifftshift(fstatic))))
+            core.iotools.write_mrc(data2write, "static_map.mrc", self.cell)
+        xyz = create_xyz_grid(self.cell, self.cut_dim)
+        vol = self.cut_dim[0] * self.cut_dim[0] * self.cut_dim[0]
+        xyz_sum = get_xyz_sum(xyz)
+        print("Cycle#   ", "Fval  ", "avg(FSC)")
+        self.t = np.asarray(t_init, dtype="float")
+        angle_list = []
+        nfit = 1
+        q = q_init_list[0]
+        axis_ang = np.asarray(quaternions.quart2axis(q), dtype="float")
+        angle_list.append(axis_ang[-1])
+        print("Initial angle: ", axis_ang[-1])
+        axis_ini = np.array(axis_ang[:3], dtype="float")
+        self.axis = axis_ini
+        rotmat = quaternions.get_RM(q)
         for i in range(ncycles):
-            start = timer()
-            if i == 0:
-                self.t = np.array([0.0, 0.0, 0.0], dtype="float")
-                self.st, s1, s2, s3 = fcodes_fast.get_st(cx, cy, cz, self.t)
-                self.sv = np.array([s1/self.cell[0], s2/self.cell[1], s3/self.cell[2]])
-                self.q = q_init
-                q_current = q_init
-                self.rotmat = core.quaternions.get_RM(self.q)
-                self.ert = self.e1
-                self.crt = self.cfo
-            else:
-                # first rotate
-                self.rotmat = core.quaternions.get_RM(self.q)
-                maps2send = np.stack((self.e1, self.cfo), axis = -1)
-                #bin_idx = self.mapobj.cbin_idx
-                #nbin = self.mapobj.cbin
-                #maps = fcodes_fast.trilinear2(maps2send,bin_idx,self.rotmat,nbin,0,2,cx, cy, cz)
-                maps = fcodes_fast.tricubic(rm=self.rotmat,
-                                    f=maps2send,
-                                    mode=0,
-                                    nc=2,
-                                    nx=cx, ny=cy, nz=cz)        
-                # then translate
-                self.st, s1, s2, s3 = fcodes_fast.get_st(cx, cy, cz, self.t)
-                #self.sv = np.array([s1, s2, s3])
-                self.ert = maps[:, :, :, 0] * self.st
-                self.crt = maps[:, :, :, 1] * self.st
-            self.fsc, fsc_avg = self.calc_fsc()
-            fsc_lst.append(self.fsc)
-            self.w_grid, self.w2_grid = self.get_wght()
-            fval = self.functional()
+            e1, sv, self.t = self.rotatemap(rotmat, self.t, smax_lf)
+            fsc = self.calc_fsc(e1)
+            avg_fsc = np.average(fsc)
+            # print(fsc)
+            w_grid, w2_grid = self.get_wght(fsc)
+            fval = self.functional(w_grid, e1)
             fval_list.append(fval)
-            # current rotation and translation to print
-            q = quaternions.quaternion_multiply(self.q, q0)
-            q = q / np.sqrt(np.dot(q, q))
-            theta2 = np.arccos((np.trace(quaternions.get_RM(q)) - 1) / 2) * 180.0 / np.pi
-            print('rotation in Euler angles:')
-            print(np.rad2deg(quaternions.rotationMatrixToEulerAngles(quaternions.get_RM(q))))
-            t_accum_angstrom = (t + self.t) * self.pixsize[0] * self.mapobj.map_dim[0]
-            translation_vec = np.sqrt(np.dot(t_accum_angstrom, t_accum_angstrom))
-            print(
-                "{:5d} {:8.4f} {:6.4f} {:6.4f} {:6.4f}".format(
-                    i, fval, theta2, translation_vec, fsc_avg
+            print("{:5d} {:8.4f} {:6.4f}".format(i, fval, avg_fsc))
+            print(self.axis)
+            if i > 1 and avg_fsc < 0.2:
+                print(
+                    "Average FSC is lower than 0.4. The axis being refined may not be correct"
                 )
-            )
-            if i > 0 and abs(fval_list[-1] - fval_list[-2]) < tol:
                 break
+            _, step_ax = derivatives(
+                self.e0,
+                e1,
+                w_grid,
+                w2_grid,
+                q,
+                sv,
+                xyz,
+                xyz_sum,
+                vol,
+            )
+            lft = linefit()
+            lft.angle_list = angle_list
+            lft.axis_ini = self.axis
+            lft.step_axis = step_ax
+            lft.get_linefit_static_data(
+                [self.e0, self.e0], self.bin_idx, self.res_arr, smax_lf
+            )
+            alpha = lft.scalar_opt()
+            step_ax = step_ax * alpha
+            print(step_ax)
+            self.axis = getaxis(self.axis, step_ax)
+            q = self.get_quaternion(angle_list[0])
+            rotmat = quaternions.get_RM(q)
+        # Final FSC plot
+        print("Refinement finished.")
+        q = self.get_quaternion(angle_list[0])
+        rotmat = quaternions.get_RM(q)
+        cx, cy, cz = fstatic.shape
+        st, _, _, _ = fcodes_fast.get_st(cx, cy, cz, self.t)
+        frotated = get_FRS(rotmat, fstatic, interp=self.interp)[:, :, :, 0]
+        if mapout:
+            data2write = np.real(ifftshift(ifftn(ifftshift(frotated * st))))
+            outmap = emdcode + "_symrefined_map_fold" + str(fold) + ".mrc"
+            core.iotools.write_mrc(data2write, outmap, self.cell)
+            print("Written ", outmap)
+        print("Now calculating final FSC...")
+        fsc = core.fsc.anytwomaps_fsc_covariance(
+            fstatic, frotated * st, self.bin_idx, self.nbin
+        )[0]
+        self.avg_fsc = np.average(fsc)
+        fscfile = emdcode + "_fsc" + str(fold) + ".eps"
+        core.plotter.plot_nlines(
+            self.res_arr,
+            [fsc],
+            fscfile,
+            ["FSC after"],
+        )
+        print("FSC file was written: ", fscfile)
+        # plot fval vs ncycle for clarity
+        fig = plt.figure(figsize=(6, 4))
+        ax1 = fig.add_subplot(111)
+        ax1.plot(fval_list, label="fval", linewidth=2)
+        plt.savefig("fval_vs_cycle.eps", format="eps", dpi=300)
 
-            if i == 0:
-                rotate = True
-                translate = False
-                if self.mapobj.com:
-                    translate = True # translate first
-                    rotate = False # rotate second
-
-            if rotate:
-                # rotation optimisation
-                rotate = False
-                translate = True
-                """ self.step = derivatives_rotation(
-                    self.e0, self.ert, self.crt, self.w_grid, self.sv, self.q, xyz, xyz_sum) """
-                self.step = derivatives_rotation(
-                    self.e0, self.ert, self.crt, self.w_grid, self.sv, q_current, xyz, xyz_sum, self.pixsize)
-                print('rotation step: ', self.step)
-                lft = linefit()
-                """ lft.get_linefit_static_data(
-                    [self.e0, self.e1], self.mapobj.cbin_idx, self.mapobj.res_arr, smax_lf) """
-                lft.get_linefit_static_data(
-                    [self.e0, self.ert], self.mapobj.cbin_idx, self.mapobj.res_arr, smax_lf)
-                lft.step = self.step
-                """ lft.q_prev = self.q """
-                lft.q_prev = q_init#q_current
-                alpha_r = lft.scalar_opt()
-                print('alpha_r: ', alpha_r)
-                q_current += np.insert(self.step * alpha_r, 0, 0.0)
-                q_current = q_current / np.sqrt(np.dot(q_current, q_current))
-                self.q += np.insert(self.step * alpha_r, 0, 0.0)
-                self.q = self.q / np.sqrt(np.dot(self.q, self.q))
-                #from emda.ext.overlay_x import ndlinefit
-                #lft = ndlinefit()
-                #lft.get_linefit_static_data(
-                #    [self.e0, self.ert], self.mapobj.cbin_idx, self.mapobj.res_arr, smax_lf)
-                #lft.step = self.step
-                #lft.q_prev = q_init#q_current
-                #alpha_r = lft.scalar_opt()
-                #print('alpha_r: ', alpha_r)
-                #q_current += np.insert(self.step * np.asarray(alpha_r, 'float'), 0, 0.0)
-                #q_current = q_current / np.sqrt(np.dot(q_current, q_current))
-                #self.q += np.insert(self.step * np.asarray(alpha_r, 'float'), 0, 0.0)
-                #self.q = self.q / np.sqrt(np.dot(self.q, self.q))
-                """ lft = Bfgs()
-                lft.get_linefit_static_data(
-                    [self.e0, self.ert], self.mapobj.cbin_idx, self.mapobj.res_arr, smax_lf)
-                lft.step = self.step
-                lft.q_prev = q_current
-                lft.q = q_current
-                lft.cell = self.cell
-                alpha_r = lft.optimize()[0]
-                print('alpha_r: ', alpha_r)
-                q_current += np.insert(self.step * alpha_r, 0, 0.0)
-                q_current = q_current / np.sqrt(np.dot(q_current, q_current))
-                self.q += np.insert(self.step * alpha_r, 0, 0.0)
-                self.q = self.q / np.sqrt(np.dot(self.q, self.q)) """
-
-                """ self.rotmat = core.quaternions.get_RM(self.q)
-                maps2send = np.stack((self.e1, self.cfo), axis = -1)
-                maps = fcodes_fast.tricubic(rm=self.rotmat,
-                                    f=maps2send,
-                                    mode=0,
-                                    nc=2,
-                                    nx=cx, ny=cy, nz=cz)
-                self.ert = maps[:, :, :, 0] * self.st
-                self.crt = maps[:, :, :, 1] * self.st """
-
-            if translate:
-                # translation optimisation
-                translate = False
-                rotate = True
-                self.step = derivatives_translation(
-                    self.e0, self.ert, self.w_grid, self.w2_grid, self.sv)
-                lft = linefit()
-                lft.get_linefit_static_data(
-                    [self.e0, self.ert], self.mapobj.cbin_idx, self.mapobj.res_arr, smax_lf)
-                lft.step = self.step
-                alpha_t = lft.scalar_opt_trans()
-                self.t += self.step * alpha_t
-                self.t = np.array([0., 0., 0.], 'float') # turning off t
-
-                """ self.st, s1, s2, s3 = fcodes_fast.get_st(cx, cy, cz, self.t)
-                if i == 0:
-                    self.ert = self.ert * self.st
-                    self.crt = self.crt * self.st  
-                if i > 0:                  
-                    self.ert = maps[:, :, :, 0] * self.st
-                    self.crt = maps[:, :, :, 1] * self.st """
-
-            end = timer()
-            if timeit:
-                print("time for one cycle:", end - start)
+
+def fsc_between_static_and_transfomed_map(
+    staticmap, movingmap, bin_idx, rm, t, cell, nbin
+):
+    nx, ny, nz = staticmap.shape
+    st, _, _, _ = fcodes_fast.get_st(nx, ny, nz, t)
+    frt_full = get_FRS(rm, movingmap * st, interp="linear")[:, :, :, 0]
+    f1f2_fsc = core.fsc.anytwomaps_fsc_covariance(
+        staticmap, frt_full, bin_idx, nbin)[0]
+    return f1f2_fsc
+
+
+def get_ibin(bin_fsc, thresh=0.5):
+    print('thresh:', thresh)
+    # new search from rear end
+    for i, ifsc in reversed(list(enumerate(bin_fsc))):
+        if ifsc > thresh:
+            ibin = i
+            if ibin % 2 != 0:
+                ibin = ibin - 1
+            break
+    return ibin
 
 
+# frequency marching
 def run_fit(
     emmap1,
     rotmat,
     t,
     ncycles,
     ifit,
+    fitfsc=0.5,
+    nmarchingcycles=10,
     fobj=None,
+    interp=None,
     fitres=None,
 ):
-    from emda.core.quaternions import rot2quart
 
+    q_init = quaternions.rot2quart(rotmat)
+    axis_ang = quaternions.quart2axis(q_init)
+    axis_ini = axis_ang[:3]
+    angle = axis_ang[-1]
     if fitres is not None:
         if fitres <= emmap1.res_arr[-1]:
             fitbin = len(emmap1.res_arr) - 1
         else:
             dist = np.sqrt((emmap1.res_arr - fitres) ** 2)
             ibin = np.argmin(dist)
             if ibin % 2 != 0:
                 ibin = ibin - 1
             fitbin = min([len(dist), ibin])
-    else:
+    if fitres is None:
         fitbin = len(emmap1.res_arr) - 1
     fsc_lst = []
-    #
-    q = rot2quart(rotmat)
-    for i in range(10):
-        print("Resolution cycle #: ", i)
+    for i in range(nmarchingcycles):
         if i == 0:
-            f1f2_fsc, frt, ert, fsc_avg = utils.fsc_between_static_and_transfomed_map(
-                maps = [emmap1.fo_lst[0], emmap1.fo_lst[ifit], emmap1.eo_lst[ifit]],
+            f1f2_fsc = fsc_between_static_and_transfomed_map(
+                staticmap=emmap1.fo_lst[0],
+                movingmap=emmap1.fo_lst[ifit],
                 bin_idx=emmap1.bin_idx,
                 rm=rotmat,
                 t=t,
+                cell=emmap1.map_unit_cell,
                 nbin=emmap1.nbin,
             )
-            ibin = utils.determine_ibin(f1f2_fsc, fsc_avg)
-            if fitbin < ibin:
-                ibin = fitbin
-            ibin_old = ibin
-            print("Fitting starts at ", emmap1.res_arr[ibin], " (A)")
             fsc_lst.append(f1f2_fsc)
-            if fsc_avg > 0.999:
+            # if np.average(f1f2_fsc) > 0.999:
+            if fitfsc > 0.999:
                 rotmat = rotmat
-                t = t
-                q_final = quaternions.rot2quart(rotmat)
-                fsc_lst.append(f1f2_fsc)
+                final_tran = t
+                final_axis = axis_ini
+                avg_fsc = fitfsc  # np.average(f1f2_fsc)
                 print("\n***FSC between static and moving maps***\n")
                 print("bin#     resolution(A)      start-FSC     end-FSC\n")
                 for j in range(len(emmap1.res_arr)):
                     print(
                         "{:5d} {:6.2f} {:8.4f} {:8.4f}".format(
-                            j, emmap1.res_arr[j], fsc_lst[1][j], fsc_lst[0][j]
+                            j, emmap1.res_arr[j], fsc_lst[0][j], fsc_lst[0][j]
                         )
                     )
                 break
+            ibin = get_ibin(f1f2_fsc, thresh=fitfsc)
+            if fitbin < ibin:
+                ibin = fitbin
+            ibin_old = ibin
+            q = q_init
+            print("Fitting starts at ", emmap1.res_arr[ibin], " (A)")
         else:
             # Apply initial rotation and translation to calculate fsc
-            f1f2_fsc, frt, ert, fsc_avg = utils.fsc_between_static_and_transfomed_map(
-                maps = [emmap1.fo_lst[0], emmap1.fo_lst[ifit], emmap1.eo_lst[ifit]],
-                bin_idx=emmap1.bin_idx,
-                rm=rotmat,
-                t=t,
-                nbin=emmap1.nbin,
+            f1f2_fsc = fsc_between_static_and_transfomed_map(
+                emmap1.fo_lst[0],
+                emmap1.fo_lst[ifit],
+                emmap1.bin_idx,
+                rotmat,
+                t,
+                emmap1.map_unit_cell,
+                emmap1.nbin,
             )
-            ibin = utils.determine_ibin(f1f2_fsc, fsc_avg)
+            ibin = get_ibin(f1f2_fsc, thresh=fitfsc)
             if fitbin < ibin:
                 ibin = fitbin
-            print("Fitting resolution: ", emmap1.res_arr[ibin], " (A)")
             if ibin_old == ibin:
                 fsc_lst.append(f1f2_fsc)
                 q_final = quaternions.rot2quart(rotmat)
+                res_arr = emmap1.res_arr[:ibin_old]
+                fsc_bef = fsc_lst[0][:ibin_old]
+                fsc_aft = fsc_lst[1][:ibin_old]
                 print("\n***FSC between static and moving maps***\n")
                 print("bin#     resolution(A)      start-FSC     end-FSC\n")
-                for j in range(len(emmap1.res_arr)):
+                for j in range(len(res_arr)):
                     print(
                         "{:5d} {:6.2f} {:8.4f} {:8.4f}".format(
-                            j, emmap1.res_arr[j], fsc_lst[0][j], fsc_lst[1][j]
+                            j, res_arr[j], fsc_bef[j], fsc_aft[j]
                         )
                     )
                 break
             else:
                 ibin_old = ibin
+                print("Fitting starts at ", emmap1.res_arr[ibin], " (A)")
         if ibin == 0:
-            print("ibin = 0")
-            raise SystemExit("Cannot proceed! Stopping now...")
-        e_list = [emmap1.eo_lst[0], ert, frt]
+            print("ibin = 0, Cannot proceed! Stopping current axis refinement.")
+            fobj.write(
+                "ibin = 0, Cannot proceed! Stopping current axis refinement.\n")
+            break
+        e_list = [emmap1.eo_lst[0], emmap1.fo_lst[0]]
         eout, cBIdx, cbin = cut_resolution_for_linefit(
             e_list, emmap1.bin_idx, emmap1.res_arr, ibin
         )
-        emmap1.ceo_lst = [eout[0, :, :, :], eout[1, :, :, :]]
-        emmap1.cfo_lst = [eout[2, :, :, :]]
+        #static_cutmap = eout[0, :, :, :]
+        static_cutmap = eout[1, :, :, :]  # use Fo instead of Eo for fitting.
+        fstatic_cutmap = eout[1, :, :, :]
+        moving_cutmap = static_cutmap
+        emmap1.ceo_lst = [static_cutmap, moving_cutmap]
+        emmap1.cfo_lst = [fstatic_cutmap]
         emmap1.cbin_idx = cBIdx
-        emmap1.cdim = eout[1, :, :, :].shape
+        emmap1.cdim = moving_cutmap.shape
         emmap1.cbin = cbin
-        rfit = EmFit(emmap1)
+        fit = EmFit(emmap1)
         slf = ibin
-        slf = min([ibin, 100])
-        rfit.minimizer(ncycles, t, rotmat, ifit, smax_lf=slf, fobj=fobj)
-        t += rfit.t
-        q = quaternions.quaternion_multiply(rfit.q, q)
-        #print("q: ", q)
-        q = q / np.sqrt(np.dot(q, q))
+        fit.minimizer(ncycles=ncycles, t_init=t, smax_lf=slf, q_init_list=[q])
+        ncycles = ncycles
+        final_axis = fit.axis
+        final_tran = fit.t
+        avg_fsc = fit.avg_fsc
+        q = quaternions.get_quaternion(
+            [[final_axis[0], final_axis[1], final_axis[2]],
+                [np.rad2deg(angle)]]
+        )
         rotmat = quaternions.get_RM(q)
-    return t, q_final
+    return final_axis, final_tran, avg_fsc
 
 
 def overlay(
-    maplist,
-    tlist,
-    qlist,
-    ncycles=100,
-    modelres=None,
-    masklist=None,
-    modellist=None,
-    fitres=None,
-    nocom=False,
-    fobj=None
+    emdcode,
+    imap,
+    rotaxis,
+    symorder,
+    fitfsc=0.5,
+    ncycles=10,
+    t_init=[0.0, 0.0, 0.0],
+    theta_init=0.0,
+    smax=7,
+    interp="linear",
+    imask=None,
+    fobj=None,
+    halfmaps=False,
+    dfs_interp=False,
+    usemodel=False,
+    fitres=5,
 ):
-    fobj.write("\n This is EMDA map overlay \n")
+    axis = np.asarray(rotaxis)
+    axis = axis / math.sqrt(np.dot(axis, axis))
+    initial_axis = axis
+    print("Initial axis and fold: ", axis, symorder)
+    fobj.write("Initial axis and fold: " + str(axis) + str(symorder) + "\n")
+    print(" ")
+    print("Preparing data for axis refinement...")
     try:
-        emmap1 = EmmapOverlay(map_list=maplist, mask_list=masklist, modelres=modelres, nocom=nocom)
+        emmap1 = EmmapOverlay(imap=imap, imask=imask)
     except:
-        emmap1 = EmmapOverlay(map_list=maplist, modelres=modelres, nocom=nocom)
-    emmap1.load_maps()
+        emmap1 = EmmapOverlay(imap=imap)
+    emmap1.get_maps()
     emmap1.calc_fsc_from_maps()
+    print(" Number of refinement cycles:", ncycles)
+    print("Data resolution for refinement: ", fitres)
+    fobj.write(" Number of refinement cycles: " + str(ncycles) + "\n")
+    fobj.write("Data resolution for refinement: " + str(fitres) + "\n")
+    q_init_list = []
+    q_final_list = []
+    avg_fsc_list = []
+    angle_list = []
     rotmat_list = []
+    axis_list = []
     trans_list = []
-    for ifit in range(1, len(emmap1.eo_lst)):
-        t, q_final = run_fit(
+    print("Initial axis and angles:")
+    fobj.write("Initial axis and angles: \n")
+    for n in range(1, symorder):
+        theta = float(n * 360.0 / symorder)
+        print("   ", axis, theta)
+        fobj.write("   " + str(axis) + str(theta) + "\n")
+        angle_list.append(theta)
+        q = quaternions.get_quaternion([[axis[2], axis[1], axis[0]], [theta]])
+        # print(q)
+        q_init_list.append(q)
+
+    for ifit in range(len(emmap1.eo_lst)):
+        rotmat_init = quaternions.get_RM(q_init_list[ifit])
+        final_axis, final_tran, avg_fsc = run_fit(
             emmap1=emmap1,
-            rotmat=quaternions.get_RM(qlist[ifit-1]),
-            t=[itm / emmap1.pixsize[i] for i, itm in enumerate(tlist[ifit-1])],
+            rotmat=rotmat_init,
+            t=np.asarray(t_init, dtype="float"),
             ncycles=ncycles,
             ifit=ifit,
+            interp=interp,
             fitres=fitres,
+            fobj=fobj,
+            fitfsc=fitfsc,
         )
-        rotmat = quaternions.get_RM(q_final)
-        rotmat_list.append(rotmat)
-        trans_list.append(t)
-    # output maps
-    output_rotated_maps(emmap1, rotmat_list, trans_list)
-    output_rotated_models(emmap1, maplist, rotmat_list, trans_list, modellist)
-    return emmap1, rotmat_list, trans_list
-
-
-def output_rotated_maps(emmap1, r_lst, t_lst):
-    fo_lst = emmap1.fo_lst
-    cell = emmap1.map_unit_cell
-    comlist = emmap1.comlist
-    bin_idx = emmap1.bin_idx
-    nbin = emmap1.nbin
-    f_static = fo_lst[0]
-    nx, ny, nz = f_static.shape
-    data2write = np.real(ifftshift(ifftn(ifftshift(f_static))))
-    print('comlist:', comlist)
-    if len(comlist) > 0:
-        data2write = em.shift_density(data2write, shift=np.subtract(comlist[0], emmap1.box_centr))
-    core.iotools.write_mrc(data2write, "static_map.mrc", cell)
-    i = 0
-    for fo, t, rotmat in zip(fo_lst[1:], t_lst, r_lst):
-        i += 1
-        f1f2_fsc_unaligned = core.fsc.anytwomaps_fsc_covariance(
-            f_static, fo, bin_idx, nbin
-        )[0]
-        frt = maputils.get_FRS(rotmat, fo, interp="cubic")[:, :, :, 0]
-        st, _, _, _ = fcodes_fast.get_st(nx, ny, nz, t)
-        frt = frt * st
-        # estimating covaraince between current map vs. static map
-        f1f2_fsc = core.fsc.anytwomaps_fsc_covariance(f_static, frt, bin_idx, nbin)[0]
-        data2write = np.real(ifftshift(ifftn(ifftshift(frt))))
-        if len(comlist) > 0:
-            print(comlist)
-            data2write = em.shift_density(data2write, shift=np.subtract(comlist[0], emmap1.box_centr))        
-        core.iotools.write_mrc(
-            data2write,
-            "{0}_{1}.{2}".format("fitted_map", str(i), "mrc"),
-            cell,
-        )
-        core.plotter.plot_nlines(
-            emmap1.res_arr,
-            [f1f2_fsc_unaligned[: emmap1.nbin], f1f2_fsc[: emmap1.nbin]],
-            "{0}_{1}.{2}".format("fsc", str(i), "eps"),
-            ["FSC before", "FSC after"],
-        )
-
-
-def output_rotated_models(emmap1, maplist, r_lst, t_lst, modellist=None):
-    from emda.core.iotools import model_transform_gm
-
-    pixsize = emmap1.pixsize
-    comlist = emmap1.comlist
-    if len(comlist) > 0:
-        assert len(comlist) == len(maplist)
-    i = 0
-    for model, t, rotmat in zip(maplist[1:], t_lst, r_lst):
-        i += 1
-        t = np.asarray(t, 'float') *  pixsize * np.asarray(emmap1.map_dim, 'int')
-        # calculate the vector from com to box_center in Angstroms
-        if len(comlist) > 0:
-            shift = np.subtract(comlist[i], comlist[0]) * pixsize
-            t = t + shift
-        rotmat = maputils.rm_zyx2xyz(rotmat)
-        if model.endswith((".mrc", ".map")):
-            continue
-        else:
-            outcifname = "emda_transformed_model_" + str(i) + ".cif"
-            model_transform_gm(mmcif_file=model,rotmat=rotmat, trans=-t, outfilename=outcifname)
-    if modellist is not None:
-        i = 0
-        for model, t, rotmat in zip(modellist, t_lst, r_lst):
+        axis_list.append(final_axis)
+        trans_list.append(final_tran)
+        avg_fsc_list.append(avg_fsc)
+    for ax, tr, avgfsc in zip(axis_list, trans_list, avg_fsc_list):
+        final_axis = ax
+        final_tran = tr
+        # print("Final axis: ", final_axis[::-1])
+        # print("Final translation (A): ", final_tran * emmap1.pixsize)
+        # fobj.write("   Final axis: " + str(final_axis[::-1]) + "\n")
+    return initial_axis, final_axis[::-1], avgfsc
+
+
+def get_intial_axis(imap):
+    #fold, x, y, z, peakh = proshade.get_symmops_from_proshade(imap)
+    results = proshade.get_symmops_from_proshade(imap)
+    return results
+
+
+def prime_factors(n):
+    # https://stackoverflow.com/questions/15347174/python-finding-prime-factors
+    i = 2
+    factors = []
+    while i * i <= n:
+        if n % i:
             i += 1
-            t = np.asarray(t, 'float') *  pixsize * np.asarray(emmap1.map_dim, 'int')
-            # calculate the vector from com to box_center in Angstroms
-            if len(comlist) > 0:
-                shift = np.subtract(comlist[i], comlist[0]) * pixsize
-                t = t + shift
-            rotmat = maputils.rm_zyx2xyz(rotmat)
-            outcifname = "emda_transformed_model_" + str(i) + ".cif"
-            mapcom = np.asarray(comlist[i]) * pixsize
-            model_transform_gm(mmcif_file=model, rotmat=rotmat, trans=-t, mapcom=mapcom, outfilename=outcifname)
+        else:
+            n //= i
+            factors.append(i)
+    if n > 1:
+        factors.append(n)
+    return factors
+
+
+def filter_axes(imap, resol, use_proshade_peakheight=True, use_fsc=False,
+                peak_cutoff=0.8, fsc_cutoff=0.7, ang_tol=5.0, fobj=None):
+
+    uc, arr, orig = em.get_data(imap)
+    #arr, uc = reboxmap(arr=arr, uc=uc)
+    arr = set_dim_even(arr)
+    f1 = fftshift(fftn(fftshift(arr)))
+    nbin, res_arr, bin_idx = core.restools.get_resolution_array(uc, f1)
+    resol = float(resol) * 1.1
+    dist = np.sqrt((res_arr - resol) ** 2)
+    ibin = np.argmin(dist)
+    # get initial axes list from ProSHADE
+    proshade_results = get_intial_axis(imap)
+    symorder = proshade_results[0]
+    x = proshade_results[1]
+    y = proshade_results[2]
+    z = proshade_results[3]
+    peakh = proshade_results[4]
+    proshade_pg = proshade_results[5]
+    #symorder, x, y, z, peakh = get_intial_axis(imap)
+    fobj.write("ProSHADE peak table \n")
+    if len(symorder) < 1:
+        print("proshade peak table is empty.")
+        return []
+        #SystemExit()
+    for i, odr in enumerate(symorder):
+        fobj.write(str(symorder[i]) +" ["+ str(x[i]) +" "+ str(y[i]) 
+            +" "+ str(z[i]) +"] "+ str(peakh[i]) + "\n")
+    fobj.write("Proshade Point group: "+ proshade_pg + "\n")
+    #
+    # find the peak_cutoff if igen cutoff is too high
+    peakcutoff_np = np.asarray(peakh, 'float')
+    peakcutoff_best = np.max(peakcutoff_np) - 0.1
+    if peak_cutoff > np.max(peakcutoff_np):
+        peak_cutoff = peakcutoff_best
+        print("new peak cutoff: ", peak_cutoff)
+        fobj.write("new peak cutoff: "+ str(peak_cutoff) + "\n")
+    axes_list = []
+    order_list = []
+    avgfsc_list = []
+    if use_proshade_peakheight and use_fsc:
+        use_proshade_peakheight = False
+    if use_proshade_peakheight:
+        use_fsc = False
+        for ix, iy, iz, order, score in zip(x, y, z, symorder, peakh):
+            # using proshade peak height to decide point group
+            if score > peak_cutoff:
+                axis = np.asarray([ix, iy, iz], 'float')
+                axis = axis / math.sqrt(np.dot(axis, axis))
+                axes_list.append(axis)
+                order_list.append(order)
+                avgfsc_list.append(score)
+    if use_fsc:
+        print("ORDER     FSC(avg)       P.H      AXIS")
+        fobj.write("ORDER     FSC(avg)       P.H      AXIS \n")
+        for ix, iy, iz, order, score in zip(x, y, z, symorder, peakh):
+            # using proshade peak height to decide point group
+            if score > 0.1:
+                axis = np.asarray([ix, iy, iz], 'float')
+                axis = axis / math.sqrt(np.dot(axis, axis))
+                # calculate FSC, because score is not good enough to decide the pg
+                theta = float(360.0 / order)
+                q = quaternions.get_quaternion(
+                    [[axis[2], axis[1], axis[0]], [theta]])
+                rotmat = quaternions.get_RM(q)
+                frt = get_FRS(rotmat, f1, interp="linear")[:, :, :, 0]
+                fsc = core.fsc.anytwomaps_fsc_covariance(
+                    f1, frt, bin_idx, nbin)[0]
+                avg_fsc = np.average(fsc[:ibin])
+                print(order, avg_fsc, score, axis)
+                fobj.write(str(order) +" "+ str(avg_fsc) +" "+ str(score) +" "+ str(axis) + "\n")
+                if avg_fsc > fsc_cutoff:
+                    axes_list.append(axis)
+                    order_list.append(order)
+                    avgfsc_list.append(avg_fsc)
+    # sort all lists by order
+    sorted_list = sort_together([order_list, axes_list, avgfsc_list])
+    sorted_odrlist, sorted_axlist, sorted_fsclist = sorted_list
+    # remove duplicate axes
+    duplicate_list = []
+    for i, odr1 in enumerate(sorted_odrlist):
+        for j, odr2 in enumerate(sorted_odrlist):
+            if i < j:
+                angle = cosine_angle(sorted_axlist[i], sorted_axlist[j])
+                if angle < ang_tol or (180. - angle) < ang_tol:
+                    if odr1 == odr2:
+                        duplicate_list.append(j)
+                    elif odr1 < odr2:
+                        duplicate_list.append(i)
+                    elif odr1 > odr2:
+                        duplicate_list.append(j)
+    print(duplicate_list)
+    cleaned_axlist = []
+    cleaned_odrlist = []
+    cleaned_fsclist = []
+    for i, ax in enumerate(sorted_axlist):
+        if not np.any(i == np.asarray(duplicate_list)):
+            print(i, ax, sorted_odrlist[i], sorted_fsclist[i])
+            cleaned_axlist.append(ax)
+            cleaned_odrlist.append(sorted_odrlist[i])
+            cleaned_fsclist.append(sorted_fsclist[i])
+    return [cleaned_axlist, cleaned_odrlist, cleaned_fsclist, f1, ibin, nbin, bin_idx, proshade_pg]
+
+
+def prefilter_order(f1, axis, order, ibin, nbin, bin_idx):
+    # prime factorization
+    factors = prime_factors(order)
+    filtered_order_list = []
+    if len(factors) == 1:
+        filtered_order_list.append(order)
+    else:
+        axis = np.asarray(axis)
+        axis = axis / math.sqrt(np.dot(axis, axis))
+        rotmat_list = []
+        for fac in factors:
+            theta = float(360.0 / fac)
+            q = quaternions.get_quaternion(
+                [[axis[2], axis[1], axis[0]], [theta]])
+            rotmat = quaternions.get_RM(q)
+            frt = get_FRS(rotmat, f1, interp="linear")[:, :, :, 0]
+            fsc = core.fsc.anytwomaps_fsc_covariance(f1, frt, bin_idx, nbin)[0]
+            avg_fsc = np.average(fsc[:ibin])
+            print('fac, Avg FSC: ', fac, avg_fsc)
+            if avg_fsc > 0.8:
+                filtered_order_list.append(fac)
+    true_order = np.prod(np.asarray(filtered_order_list), dtype='int')
+    return true_order
+
+
+""" def prefilter_order(imap, axis, order, resol=None):
+    # prime factorization
+    factors = prime_factors(order)
+    filtered_order_list = []
+    if len(factors) == 1:
+        filtered_order_list.append(order)
+    else:
+        axis = np.asarray(axis)
+        axis = axis / math.sqrt(np.dot(axis, axis))
+        uc, arr, orig = em.get_data(imap)
+        arr = set_dim_even(arr)
+        f1 = fftshift(fftn(fftshift(arr)))
+        nbin, res_arr, bin_idx = core.restools.get_resolution_array(uc, f1)
+        rotmat_list = []
+        if resol is not None:
+            dist = np.sqrt((res_arr - resol) ** 2)
+            ibin = np.argmin(dist)
+            # cut map
+            #f1, bin_idx, nbin = cut_resolution_for_linefit(
+            #[f1], bin_idx, res_arr, ibin)
+        else:
+            ibin = nbin
 
+        for fac in factors:
+            theta = float(360.0 / fac)
+            q = quaternions.get_quaternion([[axis[2], axis[1], axis[0]], [theta]])
+            rotmat = quaternions.get_RM(q)
+            frt = get_FRS(rotmat, f1, interp="linear")[:, :, :, 0]
+            fsc = core.fsc.anytwomaps_fsc_covariance(f1, frt, bin_idx, nbin)[0]
+            avg_fsc = np.average(fsc[:ibin])
+            print('fac, Avg FSC: ', fac, avg_fsc)
+            if avg_fsc > 0.8:
+                filtered_order_list.append(fac)
+    true_order = np.prod(np.asarray(filtered_order_list), dtype='int')
+    return true_order """
+
+
+def cosine_angle(ax1, ax2):
+    vec_a = np.asarray(ax1, 'float')
+    vec_b = np.asarray(ax2, 'float')
+    dotp = np.dot(vec_a, vec_b)
+    #assert -1.0 <= dotp <= 1.0
+    if -1.0 <= dotp <= 1.0:
+        angle = math.acos(dotp)
+    else:
+        print("Problem, dotp: ", dotp)
+        print("axes:", vec_a, vec_b)
+        angle = 0.0
+    return np.rad2deg(angle)
+
+
+def decide_pointgroup(axeslist, orderlist):
+    # TODO- Current group generator axes are not correct.
+    # need to identify correct axes for refinement.
+
+    # check for cyclic sym of n-order
+    order_arr = np.asarray(orderlist)
+    dic = {i: (order_arr == i).nonzero()[0] for i in np.unique(order_arr)}
+    uniqorder = np.fromiter(dic.keys(), dtype='int')
+    #uniqorder = np.unique(np.asarray(orderlist), 'int')
+    anglist = []
+    point_group = None
+    gp_generator_ax1 = None
+    gp_generator_ax2 = None
+    order1 = order2 = 0
+    ang_tol = 5.0  # Degrees
+    print("uniqorders: ", uniqorder)
+    if len(uniqorder) == 1:
+        print("Len of uniqorder: ", 1)
+        if uniqorder[0] == 1:
+            print("Unsymmetrized map")
+            point_group = 'C1'
+            order1 = 1
+        elif uniqorder[0] != 1:
+            odrn = dic[uniqorder[0]]
+            if len(odrn) == 1:
+                point_group = 'C'+str(uniqorder[0])
+                gp_generator_ax1 = axeslist[0]
+                order1 = uniqorder[0]
+            elif len(odrn) > 1:
+                if uniqorder[0] == 2:
+                    print("Checking for D symmetry...")
+                    for i in odrn:
+                        for j in odrn:
+                            if i != j:
+                                angle = cosine_angle(axeslist[i], axeslist[j])
+                                anglist.append(angle)
+                    angarr = np.asarray(anglist, 'float')
+                    if np.all(abs(angarr - 90.0) <= ang_tol):
+                        point_group = 'D2'
+                        gp_generator_ax1 = axeslist[odrn[0]]
+                        gp_generator_ax2 = axeslist[odrn[1]]
+                        order1 = order2 = 2
+                    else:
+                        print("Unknown symmetry")
+                        point_group = 'Unkown'
+                elif uniqorder[0] == 3:
+                    print("Checking for T symmetry...")
+                    for i in odrn:
+                        for j in odrn:
+                            if i != j:
+                                angle = cosine_angle(axeslist[i], axeslist[j])
+                                anglist.append(angle)
+                    angarr = np.asarray(anglist, 'float')
+                    condition2 = angarr[np.logical_not(
+                        abs(angarr - 109.47) <= ang_tol)]
+                    if np.all(abs(condition2 - 70.53) <= ang_tol):
+                        point_group = 'T'
+                        gp_generator_ax1 = axeslist[odrn[0]]
+                        gp_generator_ax2 = axeslist[odrn[1]]
+                        order1 = order2 = 3
+                    else:
+                        print("test1")
+                        print("Unknown point group.")
+                        point_group = 'Unkown'
+                elif uniqorder[0] == 4:
+                    print("Checking for O symmetry...")
+                    for i in odrn:
+                        for j in odrn:
+                            if i != j:
+                                angle = cosine_angle(axeslist[i], axeslist[j])
+                                anglist.append(angle)
+                    angarr = np.asarray(anglist, 'float')
+                    if np.all(abs(angarr - 90.0) <= ang_tol):
+                        point_group = 'O'
+                        gp_generator_ax1 = axeslist[odrn[0]]
+                        gp_generator_ax2 = axeslist[odrn[1]]
+                        order1 = order2 = 4
+                    else:
+                        print("Unknown symmetry")
+                        point_group = 'Unkown'
+                elif uniqorder[0] == 5:
+                    print("Checking for I symmetry...")
+                    for i in odrn:
+                        for j in odrn:
+                            if i != j:
+                                angle = cosine_angle(axeslist[i], axeslist[j])
+                                anglist.append(angle)
+                    angarr = np.asarray(anglist, 'float')
+                    condition2 = angarr[np.logical_not(
+                        abs(angarr - 63.47) <= ang_tol)]
+                    if np.all(abs(condition2 - 116.57) <= ang_tol):
+                        point_group = 'I'
+                        gp_generator_ax1 = axeslist[odrn[0]]
+                        gp_generator_ax2 = axeslist[odrn[1]]
+                        order1 = order2 = 5
+                    else:
+                        print("Unknown symmetry")
+                        point_group = 'Unkown'
+                else:
+                    print("Unknown symmetry")
+                    point_group = 'Unkown'
+    elif len(uniqorder) == 2:
+        if np.any(uniqorder == 2):
+            odr2 = dic[2]
+            if np.any(uniqorder == 3):
+                odr3 = dic[3]  # get all 3-fold axes locations
+                if len(odr3) == 1:
+                    print("Ckecking for D symmetry...")
+                    for i in odr2:
+                        for j in odr3:
+                            angle = cosine_angle(axeslist[i], axeslist[j])
+                            anglist.append(angle)
+                    angarr = np.asarray(anglist, 'float')
+                    if np.all(abs(angarr - 90.0) <= ang_tol):
+                        point_group = 'D3'
+                        gp_generator_ax1 = axeslist[odr2[0]]
+                        gp_generator_ax2 = axeslist[odr3[0]]
+                        order1 = 2
+                        order2 = 3
+                    else:
+                        print("Unknown symmetry")
+                        point_group = 'Unkown'
+                if len(odr3) > 1:
+                    print("Checking for T symmetry...")
+                    for i in odr3:
+                        for j in odr3:
+                            if i != j:
+                                angle = cosine_angle(axeslist[i], axeslist[j])
+                                anglist.append(angle)
+                    angarr = np.asarray(anglist, 'float')
+                    #condition1 = angarr[abs(angarr - 109.47) <= ang_tol]
+                    condition2 = angarr[np.logical_not(
+                        abs(angarr - 109.47) <= ang_tol)]
+                    if np.all(abs(condition2 - 70.53) <= ang_tol):
+                        point_group = 'T'
+                        gp_generator_ax1 = axeslist[odr3[0]]
+                        gp_generator_ax2 = axeslist[odr3[1]]
+                        order1 = order2 = 3
+                    else:
+                        print("test2")
+                        print("Unknown point group.")
+                        point_group = 'Unkown'
+            elif np.any(uniqorder == 4):
+                odr4 = dic[4]
+                if len(odr4) == 1:
+                    print("Checking for D symmetry...")
+                    for i in odr2:
+                        for j in odr4:
+                            angle = cosine_angle(axeslist[i], axeslist[j])
+                            anglist.append(angle)
+                    angarr = np.asarray(anglist, 'float')
+                    if np.all(abs(angarr - 90.0) <= ang_tol):
+                        point_group = 'D4'
+                        gp_generator_ax1 = axeslist[odr2[0]]
+                        gp_generator_ax2 = axeslist[odr4[0]]
+                        order1 = 2
+                        order2 = 4
+                    else:
+                        print("Unknown symmetry")
+                        point_group = 'Unkown'
+                elif len(odr4) > 1:
+                    print("Checking for O symmetry...")
+                    for i in odr4:
+                        for j in odr4:
+                            if i != j:
+                                angle = cosine_angle(axeslist[i], axeslist[j])
+                                anglist.append(angle)
+                    angarr = np.asarray(anglist, 'float')
+                    if np.all(abs(angarr - 90.0) <= ang_tol):
+                        point_group = 'O'
+                        gp_generator_ax1 = axeslist[odr4[0]]
+                        gp_generator_ax2 = axeslist[odr4[1]]
+                        order1 = order2 = 4
+                    else:
+                        print("Unknown symmetry")
+                        point_group = 'Unkown'
+            elif np.any(uniqorder == 5):
+                odr5 = dic[5]
+                if len(odr5) == 1:
+                    print("Checking for D symmetry...")
+                    for i in odr2:
+                        for j in odr5:
+                            angle = cosine_angle(axeslist[i], axeslist[j])
+                            anglist.append(angle)
+                    angarr = np.asarray(anglist, 'float')
+                    if np.all(abs(angarr - 90.0) <= ang_tol):
+                        point_group = 'D5'
+                        gp_generator_ax1 = axeslist[odr2[0]]
+                        gp_generator_ax2 = axeslist[odr5[0]]
+                        order1 = 2
+                        order2 = 5
+                    else:
+                        print("Unknown symmetry")
+                        point_group = 'Unkown'
+                if len(odr5) > 1:
+                    print("Checking for I symmetry...")
+                    for i in odr5:
+                        for j in odr5:
+                            if i != j:
+                                angle = cosine_angle(axeslist[i], axeslist[j])
+                                anglist.append(angle)
+                    angarr = np.asarray(anglist, 'float')
+                    condition2 = angarr[np.logical_not(
+                        abs(angarr - 63.47) <= ang_tol)]
+                    if np.all(abs(condition2 - 116.57) <= ang_tol):
+                        point_group = 'I'
+                        gp_generator_ax1 = axeslist[odr5[0]]
+                        gp_generator_ax2 = axeslist[odr5[1]]
+                        order1 = order2 = 5
+                    else:
+                        print("Unknown symmetry")
+                        point_group = 'Unkown'
+            else:
+                n = uniqorder[uniqorder != 2][0]
+                odrn = dic[n]
+                print("Ckecking for D symmetry...")
+                for i in odr2:
+                    for j in odrn:
+                        angle = cosine_angle(axeslist[i], axeslist[j])
+                        anglist.append(angle)
+                angarr = np.asarray(anglist, 'float')
+                if np.all(abs(angarr - 90.0) <= ang_tol):
+                    point_group = 'D' + str(n)
+                    gp_generator_ax1 = axeslist[odr2[0]]
+                    gp_generator_ax2 = axeslist[odrn[0]]
+                    order1 = 2
+                    order2 = n
+                else:
+                    print("Unknown symmetry")
+                    point_group = 'Unkown'
+    elif len(uniqorder) > 2:
+        # groups must belong to O or I
+        if np.any(uniqorder == 2):
+            odr2 = dic[2]
+            if np.any(uniqorder == 3):
+                odr3 = dic[3]
+                if np.any(uniqorder == 4):
+                    odr4 = dic[4]
+                    print("Ckecking for O symmetry...")
+                    for i in odr4:
+                        for j in odr4:
+                            if i != j:
+                                angle = cosine_angle(axeslist[i], axeslist[j])
+                                anglist.append(angle)
+                    angarr = np.asarray(anglist, 'float')
+                    if np.all(abs(angarr - 90.0) <= ang_tol):
+                        point_group = 'O'
+                        gp_generator_ax1 = axeslist[odr4[0]]
+                        gp_generator_ax2 = axeslist[odr4[1]]
+                        order1 = order2 = 4
+                    else:
+                        print("Unknown point group.")
+                        point_group = 'Unkown'
+                elif np.any(uniqorder == 5):
+                    # I symmetry
+                    odr5 = dic[5]
+                    print("Ckecking for I symmetry...")
+                    for i in odr5:
+                        for j in odr5:
+                            if i != j:
+                                angle = cosine_angle(axeslist[i], axeslist[j])
+                                anglist.append(angle)
+                    angarr = np.asarray(anglist, 'float')
+                    #condition1 = angarr[abs(angarr - 63.47) <= ang_tol]
+                    condition2 = angarr[np.logical_not(
+                        abs(angarr - 63.47) <= ang_tol)]
+                    if np.all(abs(condition2 - 116.57) <= ang_tol):
+                        point_group = 'I'
+                        gp_generator_ax1 = axeslist[odr5[0]]
+                        gp_generator_ax2 = axeslist[odr5[1]]
+                        order1 = order2 = 5
+                    else:
+                        print("Unknown point group.")
+                        point_group = 'Unkown'
+        else:
+            print("Unknown symmetry")
+            point_group = 'Unkown'
+    return point_group, [order1, order2, gp_generator_ax1, gp_generator_ax2]
+
+
+def get_pg(imap, resol, use_peakheight, peak_cutoff, use_fsc, fsc_cutoff, ang_tol, fobj=None):
+    results = filter_axes(imap=imap,
+                          resol=resol,
+                          use_proshade_peakheight=use_peakheight,
+                          use_fsc=use_fsc,
+                          peak_cutoff=peak_cutoff,
+                          fsc_cutoff=fsc_cutoff,
+                          ang_tol=ang_tol,
+                          fobj=fobj)
+    if len(results) < 1:
+        return []
+    cleaned_axlist, cleaned_odrlist = results[0], results[1]
+    proshade_pg = results[7]
+    pg, gp_generators = decide_pointgroup(
+        axeslist=cleaned_axlist, orderlist=cleaned_odrlist)
+    print("Point group detected from the map: ", pg)
+    fobj.write("Point group detected from the map: " + str(pg) + "\n")
+    gen_axlist = [gp_generators[2], gp_generators[3]]
+    gen_odrlist = [gp_generators[0], gp_generators[1]]
+    return [proshade_pg, pg, gen_odrlist, gen_axlist]
+
+
+def refine_pg_generator_axes(imap, axlist, odrlist, fobj, fitres=5.0, fitfsc=0.7, emdid=None):
+    global fold, emdcode
+    if emdid is None:
+        emdcode = "EMD-0000"
+    else:
+        emdcode = "EMD-"+str(emdid)
+    iniaxlst = []
+    fnlaxlst = []
+    foldlst = []
+    fsclst = []
+    for ax, fold in zip(axlist, odrlist):
+        if fold != 0:
+            foldlst.append(fold)
+            initial_axis, final_axis, avg_fsc = overlay(
+                emdcode=emdcode, imap=imap, rotaxis=ax, symorder=fold, fobj=fobj, fitfsc=fitfsc, fitres=fitres)
+            iniaxlst.append(ax)
+            fnlaxlst.append(final_axis)
+            fsclst.append(avg_fsc)
+    print("**Refined results**")
+    print("Initial ax, Refined ax, FSC_avg")
+    for i, _ in enumerate(foldlst):
+        print(foldlst[i], iniaxlst[i], fnlaxlst[i], fsclst[i])
+    return [foldlst, fnlaxlst]
+
+
+def analyse_nmaps(maplist, reslist, use_peakheight=True, peak_cutoff=0.8,
+                  use_fsc=False, fsc_cutoff=0.7, ang_tol=5.0, refine_axes=False,emdlist=None):
+    fobj = open("EMDA_symref.txt", "w")
+    pglist = []
+    foldlist = []
+    initaxlist = []
+    fnlaxlist = []
+
+    assert len(maplist) == len(reslist)
+    if emdbidlist is not None:
+        assert len(emdbidlist) == len(maplist)
+    else:
+        ids = np.arange(len(maplist))
+        emdbidlist = [",".join(item) for item in ids.astype(str)]
 
+    for i, imap in enumerate(maplist):
+        emdcode = "EMD-" + emdlist[i]
+        resol = float(reslist[i]) * 1.1
+        print("Map: ", imap)
+        print("emdcode: ", emdcode)
+        fobj.write("\n")
+        fobj.write("Map: " + imap + "\n")
+        fobj.write("emdcode: " + emdcode + "\n")
+        print(" ")
+        # get the point group in map
+        pg, gen_odrs, gen_axes = get_pg(imap=imap,
+                                        resol=resol,
+                                        use_peakheight=use_peakheight,
+                                        peak_cutoff=peak_cutoff,
+                                        use_fsc=use_fsc,
+                                        fsc_cutoff=fsc_cutoff,
+                                        ang_tol=ang_tol)
+        pglist.append(pg)
+        initaxlist.append(gen_axes)
+        # refine gp generator axes
+        if refine_axes:
+            folds, fnlaxes = refine_pg_generator_axes(
+                imap, gen_axlist, gen_odrlist, fobj, fitres=resol, fitfsc=0.7)
+            foldlist.append(folds)
+            fnlaxlist.append(fnlaxes)
+    if refine_axes:
+        return pglist, foldlist, initaxlist, fnlaxlist
+    else:
+        return pglist
 
 
 if __name__ == "__main__":
-    maplist = [
-        #"/Users/ranganaw/MRC/REFMAC/haemoglobin/EMD-3651/emda_test/map_transform/emd_3651.map",
-        #"/Users/ranganaw/MRC/REFMAC/haemoglobin/EMD-3651/emda_test/map_transform/transformed.mrc"
-        #"/Users/ranganaw/MRC/REFMAC/EMD-6952/emda_test/map_transform/emd_6952.map",
-        #"/Users/ranganaw/MRC/REFMAC/EMD-6952/emda_test/map_transform/transformed.mrc",
-        #"/Users/ranganaw/MRC/REFMAC/Vinoth/emda_test/diffmap/postprocess_nat.mrc",
-        #"/Users/ranganaw/MRC/REFMAC/Vinoth/emda_test/diffmap/postprocess_lig.mrc",
-        #"/Users/ranganaw/MRC/REFMAC/Takanori_ATPase/EMD-9931/emd_9931.map",
-        #"/Users/ranganaw/MRC/REFMAC/Takanori_ATPase/EMD-9934/emd_9934.map",
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/emd_21997.map",
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/emd_21999.map",
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/extracted_rbds/proshade_fit/ProShade_1/rotStr.map"
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/extracted_rbds/21997_RDB.mrc",
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/extracted_rbds/21999_RDB.mrc"
-        #"/Users/ranganaw/MRC/REFMAC/crop_refmactools_01/outward/postprocess_masked_cut.mrc",
-        #"/Users/ranganaw/MRC/REFMAC/crop_refmactools_01/melphalan/postprocess_masked_cut.mrc"
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/test3/fitted_map_1.mrc",
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/test3/6x2a.cif"
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/test3/21999_coordinate_fit/closed_rbd_fit/21997.mrc",
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/test3/21999_coordinate_fit/closed_rbd_fit/21999_fitted_on_21997.mrc"
-        "/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/test3/21999_coordinate_fit/closed_rbd_fit/coordinate_fit/21999_closed_RBD_fitted.mrc",
-        "/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/test3/21999_coordinate_fit/closed_rbd_fit/coordinate_fit/6x2a_closed_RBD.pdb"
-    ]
-
-    masklist = [
-        #"/Users/ranganaw/MRC/REFMAC/Takanori_ATPase/DomainMasks/6k7g-9931_A_mask.mrc",
-        #"/Users/ranganaw/MRC/REFMAC/Takanori_ATPase/DomainMasks/6k7i-9934_A_mask.mrc"
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/rdb_fit/emda_atomic_mask_6x29_RDB.mrc",
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/rdb_fit/emda_atomic_mask_6x2a_RDB.mrc"
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/test3/21999_coordinate_fit/closed_rbd_fit/emda_atomic_mask_6x29_closed_RBD.mrc",
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/test3/21999_coordinate_fit/closed_rbd_fit/emda_atomic_mask_6x2a_closed_RBD.mrc"
-    ]
-
-    modellist = [
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997//reworked_RBDmasks/6x2a_transformed_RDB_trimmed.pdb"
-        #"/Users/ranganaw/MRC/REFMAC/COVID19/EMD-21997/6x2a.cif"
-        ]
-    #emmap1, rotmat_lst, transl_lst = overlay(maplist=maplist, masklist=masklist)
-    #emmap1, rotmat_lst, transl_lst = overlay(maplist=maplist, modellist=modellist)
-    emmap1, rotmat_lst, transl_lst = overlay(maplist=maplist, modelres=3.5)
+    """ maplist = [
+        "/Users/ranganaw/MRC/REFMAC/EMD-0882/map/emd_0882.map",
+        "/Users/ranganaw/MRC/REFMAC/EMD-0882/emda_test/group_rotation/test_pipeline/emd_0959.map",
+        "/Users/ranganaw/MRC/REFMAC/EMD-6952//map/emd_6952.map",
+    ] """
+    map1, resol = sys.argv[1:]
+
+    maplist = []
+    maplist.append(map1)
+    reslist = []
+    reslist.append(float(resol))
+    print(maplist, reslist)
+    main(maplist, reslist)
+    #filter_axes(map1, resol)
```

### Comparing `emda-1.1.5/emda/ext/phase_randomize.py` & `emda-1.1.6.post1/emda/ext/phase_randomize.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/qq_plot.py` & `emda-1.1.6.post1/emda/ext/qq_plot.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/rebox_map.py` & `emda-1.1.6.post1/emda/ext/rebox_map.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/scale_maps.py` & `emda-1.1.6.post1/emda/ext/scale_maps.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/sym/GenerateOperators_v9_ky4.py` & `emda-1.1.6.post1/emda/ext/sym/GenerateOperators_v9_ky4.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/sym/GenerateOperators_v9_ky5.py` & `emda-1.1.6.post1/emda/ext/sym/GenerateOperators_v9_ky5.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/sym/run_proshade.py` & `emda-1.1.6.post1/emda/ext/sym/run_proshade.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/sym/symmetrize_map.py` & `emda-1.1.6.post1/emda/ext/sym/symmetrize_map.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/sym/symmetry.py` & `emda-1.1.6.post1/emda/ext/sym/symmetry.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/transform_map.py` & `emda-1.1.6.post1/emda/ext/transform_map.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/utils.py` & `emda-1.1.6.post1/emda/ext/utils.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/ext/xmlclass.py` & `emda-1.1.6.post1/emda/ext/xmlclass.py`

 * *Files identical despite different names*

### Comparing `emda-1.1.5/emda/fcodes_fast.f90` & `emda-1.1.6.post1/emda/fcodes_fast.f90`

 * *Files 1% similar despite different names*

```diff
@@ -35,43 +35,43 @@
    xymin(2) = int(-nxy(2)/2)
    xymax    = -(xymin+1)
    if(debug) print*, 'xymin = ', xymin
    if(debug) print*, 'xymax = ', xymax(1), xymax(2), 0
    if(debug) print*, 'unit cell = ', uc
    call get_resol(uc,real(xymax(1)),0.0,0.0,r(1))
    call get_resol(uc,0.0,real(xymax(2)),0.0,r(2))
-   print*,'a-max, b-max = ', r
+   if(debug) print*,'a-max, b-max = ', r
    !
    sloc = minloc(r,1)
    hk = 0
    do i = 1, 2
       if(sloc == i) hk(i) = sloc/sloc
    end do
    nbin = 0
    do i = 2, xymax(sloc)-1
       step = (i + 0.5) * hk
       call get_resol(uc,step(1),step(2),0.0,resol)
-      print*, i,step(1),step(2),0.0,resol
+      if(debug) print*, i,step(1),step(2),0.0,resol
       res_arr(nbin) = resol
       nbin = nbin + 1
    end do
-   print*, 'nbin=', nbin
+   if(debug) print*, 'nbin=', nbin
    high_res = res_arr(nbin-1)
    call get_resol(uc,0.0,0.0,0.0,low_res)
  
-   print*, 'Creating resolution grid. Please wait...'
+   if(debug) print*, 'Creating resolution grid. Please wait...'
  
   ! Friedel's Law
    do i=xymin(1), xymax(1)
       do j=xymin(2), xymax(2)
          call get_resol(uc,real(i),real(j),0.0,resol)
          if(resol < high_res .or. resol > low_res) cycle
          ! Find the matching bin to resol
          do ibin = 0, nbin - 1
-            val = sqrt((res_arr(ibin) - resol)**2)
+            val = abs((res_arr(ibin) - resol))
             if(ibin == 0)then
                tmp_val = val; tmp_min = val
                mnloc = ibin 
             else
                tmp_val = val
                if(tmp_val < tmp_min)then
                   tmp_min = val
@@ -141,24 +141,24 @@
 
   do i = 0, xyzmax(sloc)-1
      !step = (i + 1.5) * hkl
      step = (i + 2.5) * hkl
      call get_resol(uc,step(1),step(2),step(3),resol)
      if(debug) print*, i,step(1),step(2),step(3),resol
      !print*, i,step(1),step(2),step(3),resol
-     print*, i,resol
+     if(debug) print*, i,resol
      res_arr(i) = resol
      nbin = i + 1
   end do
-  print*, 'nbin=', nbin
+  if(debug) print*, 'nbin=', nbin
   high_res = res_arr(nbin-1)
   call get_resol(uc,0.0,0.0,0.0,low_res)
-  !print*,"Low res=",low_res,"High res=",high_res ,'A'
+  if(debug) print*,"Low res=",low_res,"High res=",high_res ,'A'
 
-  print*, 'Creating resolution grid. Please wait...'
+  if(debug) print*, 'Creating resolution grid. Please wait...'
 
   ! Friedel's Law
   do i=xyzmin(1), xyzmax(1)
      do j=xyzmin(2), xyzmax(2)
         do k=xyzmin(3), 0 !xyzmax(3)
            call get_resol(uc,real(i),real(j),real(k),resol)
            s_grid(i,j,k) = 1.0/resol
@@ -171,15 +171,15 @@
 !!$           !mnloc  = 1
 !!$           !if(mnloc < 0 .or. mnloc > nbin-1) cycle
 !!$           bin_idx(i,j,k) = mnloc
 !!$           if(k == xyzmin(3) .or. j == xyzmin(2) .or. i == xyzmin(1)) cycle
 !!$           bin_idx(-i,-j,-k) = mnloc
            ! Find the matching bin to resol
            do ibin = 0, nbin - 1
-              val = sqrt((res_arr(ibin) - resol)**2)
+              val = abs((res_arr(ibin) - resol))
               if(ibin == 0)then
                  tmp_val = val; tmp_min = val
                  mnloc = ibin 
               else
                  tmp_val = val
                  if(tmp_val < tmp_min)then
                     tmp_min = val
@@ -223,35 +223,35 @@
    xyzmin = 0; xyzmax = 0
    nxyz = (/ nx, ny, nz /)
    xyzmin(1) = int(-nxyz(1)/2)
    xyzmin(2) = int(-nxyz(2)/2)
    xyzmin(3) = int(-nxyz(3)/2)
    xyzmax    = -(xyzmin+1)
    !
-   print*, 'nbin=', nbin
+   if(debug) print*, 'nbin=', nbin
    high_res = res_arr(nbin-1)
    !call get_reciprocal_basis(uc, ucstar)
    call get_resol(uc,0.0,0.0,0.0,low_res)
    !call get_resol2(ucstar,0.0,0.0,0.0,low_res)
-   print*,"Low res=",low_res,"High res=",high_res ,'A'
-   print*, 'Creating resolution grid. Please wait...'
+   if(debug) print*,"Low res=",low_res,"High res=",high_res ,'A'
+   if(debug) print*, 'Creating resolution grid. Please wait...'
    ! Friedel's Law
    do i=xyzmin(1), xyzmax(1)
       do j=xyzmin(2), xyzmax(2)
          do k=xyzmin(3), 0 !xyzmax(3)
             call get_resol(uc,real(i),real(j),real(k),resol)
             !call get_resol2(ucstar,real(i),real(j),real(k),resol)
             s_grid(i,j,k) = 1.0/resol
             if(k/=xyzmin(3) .and. j/=xyzmin(2) .and. i/=xyzmin(1))then
                s_grid(-i,-j,-k) = s_grid(i,j,k)
             end if
             if(resol < high_res .or. resol > low_res) cycle
             ! Find the matching bin to resol
             do ibin = 0, nbin - 1
-               val = sqrt((res_arr(ibin) - resol)**2)
+               val = abs((res_arr(ibin) - resol))
                if(ibin == 0)then
                   tmp_val = val; tmp_min = val
                   mnloc = ibin 
                else
                   tmp_val = val
                   if(tmp_val < tmp_min)then
                      tmp_min = val
@@ -323,25 +323,25 @@
 
   do i = 0, xyzmax(sloc)-1
      !step = (i + 1.5) * hkl
      step = (i + 2.5) * hkl
      call get_resol(uc,step(1),step(2),step(3),resol)
      if(debug) print*, i,step(1),step(2),step(3),resol
      !print*, i,step(1),step(2),step(3),resol
-     print*, i,resol
+     if(debug) print*, i,resol
      res_arr(i) = resol
      bin_arr(i) = i + 2.5
      nbin = i + 1
   end do
-  print*, 'nbin=', nbin
+  if(debug) print*, 'nbin=', nbin
   high_res = res_arr(nbin-1)
   call get_resol(uc,0.0,0.0,0.0,low_res)
-  !print*,"Low res=",low_res,"High res=",high_res ,'A'
+  if(debug) print*,"Low res=",low_res,"High res=",high_res ,'A'
 
-  print*, 'Creating resolution grid. Please wait...'
+  if(debug) print*, 'Creating resolution grid. Please wait...'
 
   ! Friedel's Law
   do i=xyzmin(1), xyzmax(1)
      do j=xyzmin(2), xyzmax(2)
         outer: do k=xyzmin(3), 0 !xyzmax(3)
            do ib=0, nbin-1
               if(sqrt(real(k)**2 + real(j)**2 + real(i)**2) .le. bin_arr(ib))then
@@ -393,16 +393,16 @@
   xyzmin(2) = int(-nxyz(2)/2)
   xyzmin(3) = int(-nxyz(3)/2)
   xyzmax    = -(xyzmin+1)
   if(debug) print*, 'xyzmin = ', xyzmin
   if(debug) print*, 'xyzmax = ', xyzmax
   if(debug) print*, 'unit cell = ', uc
 
-  print*, 'Creating resolution grid. Please wait...'
-  print*, 'High resolution cutoff: ', highres, 'A'
+  if(debug) print*, 'Creating resolution grid. Please wait...'
+  if(debug) print*, 'High resolution cutoff: ', highres, 'A'
 
   do i=xyzmin(1), xyzmax(1)
      do j=xyzmin(2), xyzmax(2)
         do k=xyzmin(3), 0 !xyzmax(3)
            call get_resol(uc,real(i),real(j),real(k),resol)
            if(resol < highres) cycle
            mask(i,j,k) = 1
```

### Comparing `emda-1.1.5/emda.egg-info/PKG-INFO` & `emda-1.1.6.post1/emda.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: emda
-Version: 1.1.5
+Version: 1.1.6.post1
 Summary: Electron Microscopy map and model manipulation tools
 Home-page: https://www2.mrc-lmb.cam.ac.uk/groups/murshudov/content/emda/emda.html
 Author: Rangana Warshamanage, Garib N. Murshudov
 Author-email: ranganaw@mrc-lmb.cam.ac.uk, garib@mrc-lmb.cam.ac.uk
 License: MPL-2.0
-Description:         Python library for Electron Microscopy Data Analysis (EMDA). 
-                EMDA supports MRC/CCP4.MAP and MTZ files as well as PDB and mmcif files. 
-                EMDA offeres a range of functions for downstream data analysis and
-                model building. Please refer emda.readthedocs.io for more information.
-Platform: UNKNOWN
+License-File: LICENSE.txt
+
+        Python library for Electron Microscopy Data Analysis (EMDA). 
+        EMDA supports MRC/CCP4.MAP and MTZ files as well as PDB and mmcif files. 
+        EMDA offeres a range of functions for downstream data analysis and
+        model building. Please refer emda.readthedocs.io for more information.
```

### Comparing `emda-1.1.5/emda.egg-info/SOURCES.txt` & `emda-1.1.6.post1/emda.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.txt
 setup.py
 emda/__init__.py
 emda/config.py
 emda/emda_cmd_caller.py
 emda/emda_methods.py
 emda/emda_test.py
@@ -35,20 +36,17 @@
 emda/ext/downmap.py
 emda/ext/fakehalf.py
 emda/ext/fouriersp_local.py
 emda/ext/half2full.py
 emda/ext/likelihood_map.py
 emda/ext/lowpass_map.py
 emda/ext/magnification.py
-emda/ext/magnification_new.py
 emda/ext/map_fsc.py
 emda/ext/maskmap_class.py
 emda/ext/overlay.py
-emda/ext/overlay_dev.py
-emda/ext/overlay_x.py
 emda/ext/phase_randomize.py
 emda/ext/qq_plot.py
 emda/ext/realsp_local.py
 emda/ext/rebox_map.py
 emda/ext/scale_maps.py
 emda/ext/transform_map.py
 emda/ext/utils.py
```

### Comparing `emda-1.1.5/setup.py` & `emda-1.1.6.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         model building. Please refer emda.readthedocs.io for more information.''',
     url='https://www2.mrc-lmb.cam.ac.uk/groups/murshudov/content/emda/emda.html',
     author='Rangana Warshamanage, Garib N. Murshudov',
     author_email='ranganaw@mrc-lmb.cam.ac.uk, garib@mrc-lmb.cam.ac.uk',
     license='MPL-2.0',
     packages=setuptools.find_packages(),
     ext_modules =[ex1],
-    install_requires=['pandas>=0.23.4','mrcfile','matplotlib','numpy','scipy','gemmi','servalcat', 'proshade'],
+    install_requires=['pandas>=0.23.4','mrcfile','matplotlib','numpy','scipy','gemmi==0.5.4','servalcat'],
     test_suite='emda.tests',
     entry_points={
       'console_scripts': [
           'emda_test = emda.emda_test:main',
           'emda_test_exhaust = emda.emda_test_exhaust:main',
           'emda = emda.emda_cmd_caller:main',
                           ],
```

