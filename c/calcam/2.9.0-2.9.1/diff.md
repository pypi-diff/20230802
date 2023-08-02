# Comparing `tmp/calcam-2.9.0.tar.gz` & `tmp/calcam-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcam-2.9.0.tar", last modified: Sun Jul 17 09:47:48 2022, max compression
+gzip compressed data, was "calcam-2.9.1.tar", last modified: Sat Jul 23 13:12:54 2022, max compression
```

## Comparing `calcam-2.9.0.tar` & `calcam-2.9.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 09:47:48.118683 calcam-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    12877 2022-07-17 09:47:40.000000 calcam-2.9.0/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-07-17 09:47:48.118683 calcam-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-07-17 09:47:40.000000 calcam-2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 09:47:48.114683 calcam-2.9.0/calcam/
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/__version__
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 09:47:48.114683 calcam-2.9.0/calcam/builtin_image_sources/
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/builtin_image_sources/calcam_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/builtin_image_sources/imagefile.py
--rw-r--r--   0 runner    (1001) docker     (121)    32430 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/cadmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)   111264 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)     9899 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    19834 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/coordtransformer.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    67724 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 09:47:48.118683 calcam-2.9.0/calcam/gui/
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25951 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/alignment_calib.py
--rw-r--r--   0 runner    (1001) docker     (121)    49849 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/cad_edit.py
--rw-r--r--   0 runner    (1001) docker     (121)    83089 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    73428 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/fitting_calib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 09:47:48.118683 calcam-2.9.0/calcam/gui/icons/
--rw-r--r--   0 runner    (1001) docker     (121)   138513 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/icons/calcam-file.ico
--rw-r--r--   0 runner    (1001) docker     (121)    14956 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/icons/calcam-file.png
--rw-r--r--   0 runner    (1001) docker     (121)   144298 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/icons/calcam.ico
--rw-r--r--   0 runner    (1001) docker     (121)    26851 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/icons/calcam.png
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/icons/icons8.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/icons/info.png
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/icons/new.png
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/icons/open.png
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/icons/save.png
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/icons/saveas.png
--rw-r--r--   0 runner    (1001) docker     (121)    45377 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/image_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/launch_script.py
--rw-r--r--   0 runner    (1001) docker     (121)     5321 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/launcher.py
--rw-r--r--   0 runner    (1001) docker     (121)    69914 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    17694 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/movement_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 09:47:48.118683 calcam-2.9.0/calcam/gui/qt_designer_files/
--rw-r--r--   0 runner    (1001) docker     (121)    56229 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/alignment_calib_editor.ui
--rw-r--r--   0 runner    (1001) docker     (121)    41265 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/cad_edit.ui
--rw-r--r--   0 runner    (1001) docker     (121)    15704 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/chessboard_image_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (121)    58070 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/fitting_calib.ui
--rw-r--r--   0 runner    (1001) docker     (121)    49312 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/image_analyser.ui
--rw-r--r--   0 runner    (1001) docker     (121)     5942 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/launcher.ui
--rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/line_coords.ui
--rw-r--r--   0 runner    (1001) docker     (121)     9940 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/movement_corr_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/rendering_progress.ui
--rw-r--r--   0 runner    (1001) docker     (121)     6789 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/settings.ui
--rw-r--r--   0 runner    (1001) docker     (121)    16103 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/split_field_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (121)    72059 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/viewer.ui
--rw-r--r--   0 runner    (1001) docker     (121)    32054 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_designer_files/virtual_calib_editor.ui
--rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qt_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    21664 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/qvtkrenderwindowinteractor.py
--rw-r--r--   0 runner    (1001) docker     (121)     9102 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    45182 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)    17956 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/virtual_calib.py
--rw-r--r--   0 runner    (1001) docker     (121)    48398 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/gui/vtkinteractorstyles.py
--rw-r--r--   0 runner    (1001) docker     (121)     6965 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/image_enhancement.py
--rw-r--r--   0 runner    (1001) docker     (121)    10616 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    15055 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    24938 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/movement.py
--rw-r--r--   0 runner    (1001) docker     (121)     5843 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/pointpairs.py
--rw-r--r--   0 runner    (1001) docker     (121)    43666 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/raycast.py
--rw-r--r--   0 runner    (1001) docker     (121)    58151 2022-07-17 09:47:40.000000 calcam-2.9.0/calcam/render.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 09:47:48.114683 calcam-2.9.0/calcam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-07-17 09:47:48.000000 calcam-2.9.0/calcam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-07-17 09:47:48.000000 calcam-2.9.0/calcam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-17 09:47:48.000000 calcam-2.9.0/calcam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-17 09:47:48.000000 calcam-2.9.0/calcam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-17 09:47:48.000000 calcam-2.9.0/calcam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-17 09:47:48.000000 calcam-2.9.0/calcam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-17 09:47:48.000000 calcam-2.9.0/calcam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-17 09:47:48.118683 calcam-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    11152 2022-07-17 09:47:40.000000 calcam-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 13:12:54.492871 calcam-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    12877 2022-07-23 13:12:47.000000 calcam-2.9.1/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-07-23 13:12:54.492871 calcam-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-07-23 13:12:47.000000 calcam-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 13:12:54.480871 calcam-2.9.1/calcam/
+-rw-r--r--   0 runner    (1001) docker     (121)     2417 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/__version__
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 13:12:54.480871 calcam-2.9.1/calcam/builtin_image_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/builtin_image_sources/calcam_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3163 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/builtin_image_sources/imagefile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32430 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/cadmodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)   111264 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9899 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19834 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/coordtransformer.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    67724 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 13:12:54.484871 calcam-2.9.1/calcam/gui/
+-rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25951 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/alignment_calib.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49849 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/cad_edit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    83089 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    73428 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/fitting_calib.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 13:12:54.488871 calcam-2.9.1/calcam/gui/icons/
+-rw-r--r--   0 runner    (1001) docker     (121)   138513 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/icons/calcam-file.ico
+-rw-r--r--   0 runner    (1001) docker     (121)    14956 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/icons/calcam-file.png
+-rw-r--r--   0 runner    (1001) docker     (121)   144298 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/icons/calcam.ico
+-rw-r--r--   0 runner    (1001) docker     (121)    26851 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/icons/calcam.png
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/icons/icons8.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/icons/info.png
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/icons/new.png
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/icons/open.png
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/icons/save.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/icons/saveas.png
+-rw-r--r--   0 runner    (1001) docker     (121)    45377 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/image_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/launch_script.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5321 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)    69914 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)    17694 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/movement_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 13:12:54.492871 calcam-2.9.1/calcam/gui/qt_designer_files/
+-rw-r--r--   0 runner    (1001) docker     (121)    56229 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/alignment_calib_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (121)    41265 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/cad_edit.ui
+-rw-r--r--   0 runner    (1001) docker     (121)    15704 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/chessboard_image_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (121)    58070 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/fitting_calib.ui
+-rw-r--r--   0 runner    (1001) docker     (121)    49312 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/image_analyser.ui
+-rw-r--r--   0 runner    (1001) docker     (121)     5942 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/launcher.ui
+-rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/line_coords.ui
+-rw-r--r--   0 runner    (1001) docker     (121)     9940 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/movement_corr_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/rendering_progress.ui
+-rw-r--r--   0 runner    (1001) docker     (121)     6789 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/settings.ui
+-rw-r--r--   0 runner    (1001) docker     (121)    16103 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/split_field_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (121)    72059 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/viewer.ui
+-rw-r--r--   0 runner    (1001) docker     (121)    32054 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_designer_files/virtual_calib_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qt_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21540 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/qvtkrenderwindowinteractor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9156 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45182 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17956 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/virtual_calib.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48398 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/gui/vtkinteractorstyles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6965 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/image_enhancement.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10629 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15055 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24938 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/movement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5843 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/pointpairs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43723 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/raycast.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58151 2022-07-23 13:12:47.000000 calcam-2.9.1/calcam/render.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 13:12:54.480871 calcam-2.9.1/calcam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-07-23 13:12:54.000000 calcam-2.9.1/calcam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-07-23 13:12:54.000000 calcam-2.9.1/calcam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 13:12:54.000000 calcam-2.9.1/calcam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-23 13:12:54.000000 calcam-2.9.1/calcam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 13:12:54.000000 calcam-2.9.1/calcam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-23 13:12:54.000000 calcam-2.9.1/calcam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-23 13:12:54.000000 calcam-2.9.1/calcam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-23 13:12:54.492871 calcam-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)    11084 2022-07-23 13:12:47.000000 calcam-2.9.1/setup.py
```

### Comparing `calcam-2.9.0/LICENCE.txt` & `calcam-2.9.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/PKG-INFO` & `calcam-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcam
-Version: 2.9.0
+Version: 2.9.1
 Summary: Spatial calibration tools for science & engineering camera systems.
 Home-page: UNKNOWN
 Author: Scott Silburn et. al.
 Author-email: scott.silburn@ukaea.uk
 License: European Union Public License 1.1
 Project-URL: Documentation, https://euratom-software.github.io/calcam
 Project-URL: Source, https://github.com/euratom-software/calcam/
```

### Comparing `calcam-2.9.0/README.md` & `calcam-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/__init__.py` & `calcam-2.9.1/calcam/__init__.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/builtin_image_sources/calcam_file.py` & `calcam-2.9.1/calcam/builtin_image_sources/calcam_file.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/builtin_image_sources/imagefile.py` & `calcam-2.9.1/calcam/builtin_image_sources/imagefile.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/cadmodel.py` & `calcam-2.9.1/calcam/cadmodel.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/calibration.py` & `calcam-2.9.1/calcam/calibration.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/config.py` & `calcam-2.9.1/calcam/config.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/coordtransformer.py` & `calcam-2.9.1/calcam/coordtransformer.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gm.py` & `calcam-2.9.1/calcam/gm.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/__init__.py` & `calcam-2.9.1/calcam/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/alignment_calib.py` & `calcam-2.9.1/calcam/gui/alignment_calib.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/cad_edit.py` & `calcam-2.9.1/calcam/gui/cad_edit.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/core.py` & `calcam-2.9.1/calcam/gui/core.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/fitting_calib.py` & `calcam-2.9.1/calcam/gui/fitting_calib.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/icons/calcam-file.ico` & `calcam-2.9.1/calcam/gui/icons/calcam-file.ico`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/icons/calcam-file.png` & `calcam-2.9.1/calcam/gui/icons/calcam-file.png`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/icons/calcam.ico` & `calcam-2.9.1/calcam/gui/icons/calcam.ico`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/icons/calcam.png` & `calcam-2.9.1/calcam/gui/icons/calcam.png`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/icons/info.png` & `calcam-2.9.1/calcam/gui/icons/info.png`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/icons/open.png` & `calcam-2.9.1/calcam/gui/icons/open.png`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/icons/save.png` & `calcam-2.9.1/calcam/gui/icons/save.png`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/icons/saveas.png` & `calcam-2.9.1/calcam/gui/icons/saveas.png`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/image_analysis.py` & `calcam-2.9.1/calcam/gui/image_analysis.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/launch_script.py` & `calcam-2.9.1/calcam/gui/launch_script.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/launcher.py` & `calcam-2.9.1/calcam/gui/launcher.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/logo.png` & `calcam-2.9.1/calcam/gui/logo.png`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/movement_correction.py` & `calcam-2.9.1/calcam/gui/movement_correction.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/alignment_calib_editor.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/alignment_calib_editor.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/cad_edit.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/cad_edit.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/chessboard_image_dialog.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/chessboard_image_dialog.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/fitting_calib.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/fitting_calib.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/image_analyser.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/image_analyser.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/launcher.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/launcher.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/line_coords.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/line_coords.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/movement_corr_dialog.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/movement_corr_dialog.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/rendering_progress.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/rendering_progress.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/settings.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/settings.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/split_field_dialog.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/split_field_dialog.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/viewer.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/viewer.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_designer_files/virtual_calib_editor.ui` & `calcam-2.9.1/calcam/gui/qt_designer_files/virtual_calib_editor.ui`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qt_wrapper.py` & `calcam-2.9.1/calcam/gui/qt_wrapper.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/qvtkrenderwindowinteractor.py` & `calcam-2.9.1/calcam/gui/qvtkrenderwindowinteractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
         QVTKRWIBase = "QWidget"
 
     from PyQt6.QtWidgets import QWidget
     from PyQt6.QtWidgets import QSizePolicy
     from PyQt6.QtWidgets import QApplication
     from PyQt6.QtCore import Qt
     from PyQt6.QtCore import QTimer
-    from PyQt6.QtCore import QObject
     from PyQt6.QtCore import QSize
     from PyQt6.QtCore import QEvent
 
     Qt.NoButton = Qt.MouseButton.NoButton
     Qt.LeftButton = Qt.MouseButton.LeftButton
     Qt.RightButton = Qt.MouseButton.RightButton
     Qt.MidButton = Qt.MouseButton.MiddleButton
@@ -105,15 +104,14 @@
         QVTKRWIBase = "QWidget"
 
     from PyQt5.QtWidgets import QWidget
     from PyQt5.QtWidgets import QSizePolicy
     from PyQt5.QtWidgets import QApplication
     from PyQt5.QtCore import Qt
     from PyQt5.QtCore import QTimer
-    from PyQt5.QtCore import QObject
     from PyQt5.QtCore import QSize
     from PyQt5.QtCore import QEvent
     MouseButtonDblClick = QEvent.MouseButtonDblClick
 
 elif PyQtImpl == "PyQt4":
 
     try:
@@ -123,15 +121,14 @@
         QVTKRWIBase = "QWidget"
 
     from PyQt4.QtGui import QWidget
     from PyQt4.QtGui import QSizePolicy
     from PyQt4.QtGui import QApplication
     from PyQt4.QtCore import Qt
     from PyQt4.QtCore import QTimer
-    from PyQt4.QtCore import QObject
     from PyQt4.QtCore import QSize
     from PyQt4.QtCore import QEvent
 
     MouseButtonDblClick = QEvent.MouseButtonDblClick
 else:
     raise ImportError("Unknown PyQt implementation " + repr(PyQtImpl))
 
@@ -256,16 +253,18 @@
         except KeyError:
             rw = None
 
         # create base qt-level widget
         if QVTKRWIBase == "QWidget":
             if "wflags" in kw:
                 wflags = kw['wflags']
+
             else:
-                wflags = Qt.WindowFlags()
+                wflags = 0
+
             QWidget.__init__(self, parent, wflags | Qt.MSWindowsOwnDC)
         elif QVTKRWIBase == "QGLWidget":
             QGLWidget.__init__(self, parent)
 
         if rw: # user-supplied render window
             self._RenderWindow = rw
         else:
```

### Comparing `calcam-2.9.0/calcam/gui/settings.py` & `calcam-2.9.1/calcam/gui/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 from .. import __version__, vtk
 from .core import guipath
 from ..misc import DodgyDict, open_file
 from ..config import CalcamConfig
 from . import qt_wrapper as qt
 from .launcher import launch
 
+if qt.qt_ver < 6:
+    red = qt.Qt.red
+else:
+    red = qt.QColor('red')
+
 class Settings(qt.QMainWindow):
 
 
     def __init__(self, app, parent = None):
 
         # GUI initialisation
         qt.QMainWindow.__init__(self, parent)
@@ -181,15 +186,15 @@
 
         for path in sorted(self.config.cad_def_paths):
 
             listitem = qt.QListWidgetItem(path)
             listitem.setFlags(listitem.flags() | qt.Qt.ItemIsEditable | qt.Qt.ItemIsSelectable)
 
             if not os.path.isdir(path):
-                listitem.setForeground(qt.Qt.red)
+                listitem.setForeground(red)
                 listitem.setToolTip('Path does not exist or cannot be accessed.')
             
             self.cad_path_list.addItem(listitem)
             if path == to_select:
                 listitem.setSelected(True)
 
         try:
@@ -214,15 +219,15 @@
 
         for path in sorted(self.config.image_source_paths):
 
             listitem = qt.QListWidgetItem(path)
             listitem.setFlags(listitem.flags() | qt.Qt.ItemIsEditable | qt.Qt.ItemIsSelectable)
 
             if not os.path.isdir(path):
-                listitem.setForeground(qt.Qt.red)
+                listitem.setForeground(red)
                 listitem.setToolTip('Path does not exist or cannot be accessed.')
                 
             self.imsource_path_list.addItem(listitem)
             if path == to_select:
                 listitem.setSelected(True)  
 
         try:
@@ -233,15 +238,15 @@
         self.imsource_list.clear()
         self.imsource_paths = DodgyDict()
 
         for imsource in sorted(self.config.get_image_sources(meta_only=True)):
             listitem = qt.QListWidgetItem(imsource[0])
             self.imsource_paths[listitem] = imsource[1]
             if imsource[2]:
-                listitem.setForeground(qt.Qt.red)
+                listitem.setForeground(red)
                 listitem.setToolTip(imsource[2])
             elif imsource[1]:
                 listitem.setToolTip(imsource[1])
 
             self.imsource_list.addItem(listitem)
             if imsource[0] == to_select:
                 listitem.setSelected(True)
```

### Comparing `calcam-2.9.0/calcam/gui/viewer.py` & `calcam-2.9.1/calcam/gui/viewer.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/virtual_calib.py` & `calcam-2.9.1/calcam/gui/virtual_calib.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/gui/vtkinteractorstyles.py` & `calcam-2.9.1/calcam/gui/vtkinteractorstyles.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/image_enhancement.py` & `calcam-2.9.1/calcam/image_enhancement.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/io.py` & `calcam-2.9.1/calcam/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,18 @@
   express or implied.
 * See the Licence for the specific language governing
   permissions and limitations under the Licence.
 '''
 
 import zipfile
 import tempfile
-import sys
 import os
 import shutil
 import hashlib
 import atexit
-import inspect
 
 from .misc import import_source,unload_source
 
 # Get a list of directory contents, including sub-directories.
 # Returned list has absolute paths.
 def listdir(path):
 
@@ -169,14 +167,16 @@
 
             self.is_open = False
             
             # Tidy up the temp directory after ourselves
             shutil.rmtree(self.tempdir)
             self.tempdir = None
 
+        atexit.unregister(self.close)
+
 
 
     def update(self):
 
         with zipfile.ZipFile(self.filename,'w',zipfile.ZIP_DEFLATED,True) as zf:
             for fname in listdir(self.tempdir):
                 zf.write(fname,os.path.relpath(fname,self.tempdir))
```

### Comparing `calcam-2.9.0/calcam/misc.py` & `calcam-2.9.1/calcam/misc.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/movement.py` & `calcam-2.9.1/calcam/movement.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/pointpairs.py` & `calcam-2.9.1/calcam/pointpairs.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam/raycast.py` & `calcam-2.9.1/calcam/raycast.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,31 +403,31 @@
         Parameters:
 
             filename (str) : File name to load from.
         '''
         f = netcdf_file(filename, 'r',mmap=False)
         self.filename = filename
                
-        self.ray_end_coords = f.variables['RayEndCoords'].data
-        self.ray_start_coords = f.variables['RayStartCoords'].data
+        self.ray_end_coords = f.variables['RayEndCoords'].data.astype(np.float32)
+        self.ray_start_coords = f.variables['RayStartCoords'].data.astype(np.float32)
         self.binning = f.variables['Binning'].data[()]
 
         self.transform = coordtransformer.CoordTransformer()
         self.transform.set_transform_actions(eval(f.image_transform_actions))
         self.transform.x_pixels = f.variables['image_original_shape'][0]
         self.transform.y_pixels = f.variables['image_original_shape'][1]
         self.transform.pixel_aspectratio = f.variables['image_original_pixel_aspect'].data[()]
 
         try:
             self.transform.offset = f.variables['image_offset'][:]
         except KeyError:
             pass
 
         try:
-            self.model_normals = f.variables['ModelNormals'].data
+            self.model_normals = f.variables['ModelNormals'].data.astype(np.float32)
         except KeyError:
             self.model_normals = None
 
         try:
             self.history = f.history.decode('utf-8')
             self.fullchip = f.fullchip
             if not self.fullchip:
```

### Comparing `calcam-2.9.0/calcam/render.py` & `calcam-2.9.1/calcam/render.py`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/calcam.egg-info/PKG-INFO` & `calcam-2.9.1/calcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcam
-Version: 2.9.0
+Version: 2.9.1
 Summary: Spatial calibration tools for science & engineering camera systems.
 Home-page: UNKNOWN
 Author: Scott Silburn et. al.
 Author-email: scott.silburn@ukaea.uk
 License: European Union Public License 1.1
 Project-URL: Documentation, https://euratom-software.github.io/calcam
 Project-URL: Source, https://github.com/euratom-software/calcam/
```

### Comparing `calcam-2.9.0/calcam.egg-info/SOURCES.txt` & `calcam-2.9.1/calcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calcam-2.9.0/setup.py` & `calcam-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 '''
 
 import sys
 import os
 import subprocess
 
 if 'bdist_wheel' in sys.argv:
-    raise Exception("Looks like you are trying to build a wheel for Calcam. That would skip setup.py at install time which contains important setup logic, so I'm afraid I can't let you do that.")
+    raise Exception("Calcam currently cannot be distributed as wheels due to having important install-time logic in setup.py.")
 
 # Read version from the version file.
 with open(os.path.join(os.path.split(os.path.abspath(__file__))[0],'calcam','__version__'),'r') as ver_file:
     version = ver_file.readline().rstrip()
 
 # Read the readme.
 with open(os.path.join(os.path.split(os.path.abspath(__file__))[0],'README.md'),'r',encoding='utf-8') as readme_file:
```

