# Comparing `tmp/glassesValidator-1.0.0.tar.gz` & `tmp/glassesValidator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glassesValidator-1.0.0.tar", last modified: Wed Jun  7 06:50:09 2023, max compression
+gzip compressed data, was "glassesValidator-1.0.1.tar", last modified: Wed Jun 28 21:14:00 2023, max compression
```

## Comparing `glassesValidator-1.0.0.tar` & `glassesValidator-1.0.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.737289 glassesValidator-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-07 06:50:09.737289 glassesValidator-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    44073 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 06:50:09.737289 glassesValidator-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.725287 glassesValidator-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.725287 glassesValidator-1.0.0/src/glassesValidator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.729288 glassesValidator-1.0.0/src/glassesValidator/GUI/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_general_imgui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.729288 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/async_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    23666 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/filepicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)   122315 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/imagehelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/msgbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/process_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.729288 glassesValidator-1.0.0/src/glassesValidator/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/markerPositions.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.733288 glassesValidator-1.0.0/src/glassesValidator/config/poster/
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/poster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   218472 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/poster/poster.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/poster/poster.tex
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/targetPositions.csv
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/config/validationSetup.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.733288 glassesValidator-1.0.0/src/glassesValidator/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/preprocess/SMI_ETG.py
--rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/preprocess/SeeTrue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26420 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/preprocess/pupilLabs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/preprocess/tobii_G2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/preprocess/tobii_G3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.733288 glassesValidator-1.0.0/src/glassesValidator/process/
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/_image_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/b_codeMarkerInterval.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/c_detectMarkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/d_gazeToPoster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/e1_computeOffsetsToTargets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/e2_determineFixationIntervals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/process/f_calculateDataQuality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.733288 glassesValidator-1.0.0/src/glassesValidator/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.733288 glassesValidator-1.0.0/src/glassesValidator/resources/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/fonts/Karla-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   556216 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/fonts/NotoSans-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1243500 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/fonts/materialdesignicons-webfont.7.0.96.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.737289 glassesValidator-1.0.0/src/glassesValidator/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29894 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/icons/icon.icns
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/icons/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/resources/icons/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.737289 glassesValidator-1.0.0/src/glassesValidator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    53577 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/makeVideo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.737289 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    56886 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/iso.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/mpeglookups.py
--rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/non_iso.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-07 06:49:59.000000 glassesValidator-1.0.0/src/glassesValidator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:50:09.729288 glassesValidator-1.0.0/src/glassesValidator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-07 06:50:09.000000 glassesValidator-1.0.0/src/glassesValidator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-07 06:50:09.000000 glassesValidator-1.0.0/src/glassesValidator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:50:09.000000 glassesValidator-1.0.0/src/glassesValidator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 06:50:09.000000 glassesValidator-1.0.0/src/glassesValidator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-07 06:50:09.000000 glassesValidator-1.0.0/src/glassesValidator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 06:50:09.000000 glassesValidator-1.0.0/src/glassesValidator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.627852 glassesValidator-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    45682 2023-06-28 21:14:00.623852 glassesValidator-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43790 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 21:14:00.627852 glassesValidator-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.611852 glassesValidator-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.615852 glassesValidator-1.0.1/src/glassesValidator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.615852 glassesValidator-1.0.1/src/glassesValidator/GUI/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_general_imgui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.615852 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/async_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23666 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/filepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122315 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/imagehelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/msgbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/process_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.615852 glassesValidator-1.0.1/src/glassesValidator/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/config/markerPositions.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.619852 glassesValidator-1.0.1/src/glassesValidator/config/poster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/config/poster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   218472 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/config/poster/poster.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/config/poster/poster.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/config/targetPositions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/config/validationSetup.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.619852 glassesValidator-1.0.1/src/glassesValidator/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/preprocess/SMI_ETG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/preprocess/SeeTrue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26420 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/preprocess/pupilLabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/preprocess/tobii_G2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/preprocess/tobii_G3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.619852 glassesValidator-1.0.1/src/glassesValidator/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/process/_image_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/process/b_codeMarkerInterval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/process/c_detectMarkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/process/d_gazeToPoster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/process/e1_computeOffsetsToTargets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/process/e2_determineFixationIntervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/process/f_calculateDataQuality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.619852 glassesValidator-1.0.1/src/glassesValidator/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.619852 glassesValidator-1.0.1/src/glassesValidator/resources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/resources/fonts/Karla-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   556216 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/resources/fonts/NotoSans-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/resources/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1243500 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/resources/fonts/materialdesignicons-webfont.7.0.96.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.623852 glassesValidator-1.0.1/src/glassesValidator/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/resources/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29894 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/resources/icons/icon.icns
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/resources/icons/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/resources/icons/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.623852 glassesValidator-1.0.1/src/glassesValidator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    53577 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/utils/makeVideo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.623852 glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56886 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/iso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/mpeglookups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/non_iso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-28 21:13:49.000000 glassesValidator-1.0.1/src/glassesValidator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:00.615852 glassesValidator-1.0.1/src/glassesValidator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45682 2023-06-28 21:14:00.000000 glassesValidator-1.0.1/src/glassesValidator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-28 21:14:00.000000 glassesValidator-1.0.1/src/glassesValidator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 21:14:00.000000 glassesValidator-1.0.1/src/glassesValidator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-28 21:14:00.000000 glassesValidator-1.0.1/src/glassesValidator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-28 21:14:00.000000 glassesValidator-1.0.1/src/glassesValidator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-28 21:14:00.000000 glassesValidator-1.0.1/src/glassesValidator.egg-info/top_level.txt
```

### Comparing `glassesValidator-1.0.0/LICENSE` & `glassesValidator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/README.md` & `glassesValidator-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 [![PyPI Latest Release](https://img.shields.io/pypi/v/glassesValidator.svg)](https://pypi.org/project/glassesValidator/)
 [![image](https://img.shields.io/pypi/pyversions/glassesValidator.svg)](https://pypi.org/project/glassesValidator/)
 [![DOI](https://zenodo.org/badge/DOI/10.3758/s13428-023-02105-5.svg)](https://doi.org/10.3758/s13428-023-02105-5)
 
-# GlassesValidator v1.0.0
+# GlassesValidator v1.0.1
 Tool for automatic determination of data quality (accuracy and precision) of wearable eye tracker recordings.
 
-Please note that this software is currently in beta, and the accompanying paper is not yet published. As such,
-the software is potentially subject to change, and we urge users to carefully check the results generated by
-glassesValidator. Please provide us with feedback on *anything* you notice, *no matter how small*.
-
-A preliminary reference to the upcoming paper is:<br>
-Niehorster, D.C., Hessels, R.S., Benjamins, J.S., Nyström, M. and Hooge, I.T.C. (submitted). GlassesValidator:
-A data quality tool for eye tracking glasses.
-
-However, as long as the paper is not accepted, please cite this work as follows:<br>
-Niehorster, D.C., Hessels, R.S., Benjamins, J.S., Nyström, M. and Hooge, I.T.C. (2022). GlassesValidator:
-A data quality tool for eye tracking glasses. Available from https://github.com/dcnieho/glassesValidator
+If you use this tool or any of the code in this repository, please cite:<br>
+[Niehorster, D.C., Hessels, R.S., Benjamins, J.S., Nyström, M. and Hooge, I.T.C. (2023). GlassesValidator:
+A data quality tool for eye tracking glasses. Behavior Research Methods. doi: 10.3758/s13428-023-02105-5](https://doi.org/10.3758/s13428-023-02105-5)
 
 # How to acquire
-GlassesValidator is available from `https://github.com/dcnieho/glassesValidator`, and supports Windows, MacOS and Linux. Right
-now only Python 3.10 is supported. Support for Python 3.11 is forthcoming once some blocking bugs have been resolved by me
-and upstream.
+GlassesValidator is available from `https://github.com/dcnieho/glassesValidator`, and supports Python 3.10 and 3.11 on Windows, MacOS and Linux. 
 
 For Windows users who wish to use the glassesValidator GUI, the easiest way to acquire glassesValidator is to [download
 a standalone executable](https://github.com/dcnieho/glassesValidator/releases/latest). The standalone executable is not
 available for MacOS or Linux.
 
 For users on Windows, Mac or Linux who wish to use glassesValidator in their Python code, the easiest way to acquire
 glassesValidator is to install it directly into your Python distribution using the command
@@ -34,14 +24,20 @@
 
 Once pip-installed in your Python distribution, the GUI can be run on any of the supported operating systems by typing `glassesValidator` in
 the terminal. From Python, running the GUI requires only the following two lines of code:
 ```python
 import glassesValidator
 glassesValidator.GUI.run()
 ```
+If you use glassesValidator's GUI in a script, make sure to wrap your script in `if __name__=="__main__"`. This is required for correct operation from a script because the GUI uses multiprocessing functionality. Do as follows:
+```python
+if __name__=="__main__":
+    import glassesValidator
+    glassesValidator.GUI.run()
+```
 
 # Usage
 The glassesValidator validation procedure consists of two parts, 1) a poster and validation procedure that is used during a recording, and 2) Python software
 for offline processing of the recording to estimate data quality measures. The glassesValidator package includes a graphical user interface (GUI)
 that can be used to perform all processing. Below we describe an example workflow using the GUI. Advanced users can however opt to call all the GUI's
 functionality directly from their own Python scripts without making use of the graphical user interface. The interested reader is referred to the glassesValidator
 manual for further details regarding how to use the glassesValidator functionality directly from their own scripts.
@@ -95,15 +91,15 @@
 device support in [`glassesValidator.preprocess`](#glassesValidatorpreprocess) should be implemented and the new eye tracker added to
 the [`glassesValidator.utils.EyeTracker` `Enum`](#glassesValidatorutils).
 
 ### Required preprocessing outside glassesValidator
 For some eye trackers, the recording delivered by the eye tracker's recording unit or software can be directly imported into
 glassesValidator. Recordings from some other eye trackers however require some steps to be performed in the manufacturer's
 software before they can be imported into glassesValidator. These are:
-- *Pupil eye trackers*: Recordings should either be preprocessed using Pupil Player (*Pupil Core* and *Pupil Invisible*) or exported
+- *Pupil Labs eye trackers*: Recordings should either be preprocessed using Pupil Player (*Pupil Core* and *Pupil Invisible*) or exported
   from Pupil Cloud (*Pupil Invisible* and *Pupil Neon*).
   - Using Pupil Player (*Pupil Core* and *Pupil Invisible*): Each recording should 1) be opened in Pupil Player, and 2) an export of the
     recording (`e` hotkey) should be run from pupil player. Make sure to disable the `World Video Exporter` in the `Plugin Manager`
     before exporting, as the exported video is not used by glassesValidator and takes a long time to create. Note that importing a Pupil
     Player export of a Pupil Invisible export requires an internet connection, which is used to retrieve the scene camera calibration
     from Pupil Lab's servers.
   - Using Pupil Cloud (*Pupil Invisible* and *Pupil Neon*): Export the recordings using the `Timeseries data + Scene video` action.
```

### Comparing `glassesValidator-1.0.0/setup.py` & `glassesValidator-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import setuptools
 import runpy
 
 info = runpy.run_path("src/glassesValidator/version.py")
 
+with open('README.md') as f:
+    readme = f.read()
+
 with open('LICENSE') as f:
     license = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 required = []
@@ -21,29 +24,31 @@
 
 setuptools.setup(
     name=info['__title__'],
     version=info['__version__'],
     author=info['__author__'],
     author_email=info['__email__'],
     description=info['__description__'],
+    long_description=readme,
     long_description_content_type="text/markdown",
     url=info['__url__'],
     project_urls={
         "Source Code": info['__url__'],
     },
     classifiers=[
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     license=license,
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     include_package_data=True,
-    python_requires="==3.10.*",
+    python_requires=">=3.10",
     install_requires=required,
     entry_points={
         "gui_scripts": [
             "glassesValidator = glassesValidator.GUI:run",
         ],
     },
 )
```

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/__init__.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/_general_imgui.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/_general_imgui.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/async_thread.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/async_thread.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/callbacks.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/callbacks.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/db.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/db.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/filepicker.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/filepicker.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/globals.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/globals.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/gui.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/gui.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/imagehelper.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/imagehelper.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/msgbox.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/msgbox.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/process_pool.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/process_pool.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/structs.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/structs.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/GUI/_impl/utils.py` & `glassesValidator-1.0.1/src/glassesValidator/GUI/_impl/utils.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/config/__init__.py` & `glassesValidator-1.0.1/src/glassesValidator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/config/markerPositions.csv` & `glassesValidator-1.0.1/src/glassesValidator/config/markerPositions.csv`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/config/poster/__init__.py` & `glassesValidator-1.0.1/src/glassesValidator/config/poster/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/config/poster/poster.pdf` & `glassesValidator-1.0.1/src/glassesValidator/config/poster/poster.pdf`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/config/poster/poster.tex` & `glassesValidator-1.0.1/src/glassesValidator/config/poster/poster.tex`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/config/validationSetup.txt` & `glassesValidator-1.0.1/src/glassesValidator/config/validationSetup.txt`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/preprocess/SMI_ETG.py` & `glassesValidator-1.0.1/src/glassesValidator/preprocess/SMI_ETG.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/preprocess/SeeTrue.py` & `glassesValidator-1.0.1/src/glassesValidator/preprocess/SeeTrue.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/preprocess/__init__.py` & `glassesValidator-1.0.1/src/glassesValidator/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/preprocess/pupilLabs.py` & `glassesValidator-1.0.1/src/glassesValidator/preprocess/pupilLabs.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/preprocess/tobii_G2.py` & `glassesValidator-1.0.1/src/glassesValidator/preprocess/tobii_G2.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/preprocess/tobii_G3.py` & `glassesValidator-1.0.1/src/glassesValidator/preprocess/tobii_G3.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/process/__init__.py` & `glassesValidator-1.0.1/src/glassesValidator/process/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/process/_image_gui.py` & `glassesValidator-1.0.1/src/glassesValidator/process/_image_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from imgui_bundle import imgui, immapp, hello_imgui, glfw_window_hello_imgui
+from imgui_bundle import imgui, immapp, hello_imgui, glfw_utils
 import glfw
 import time
 import threading
 import numpy as np
 import OpenGL.GL as gl
 
 # simple GUI provider for viewer and coder windows in glassesValidator.process
@@ -127,15 +127,15 @@
         def post_init():
             imgui.get_io().config_viewports_no_decoration = False
             imgui.get_io().config_viewports_no_auto_merge = True
 
             glfw.swap_interval(0)
             self._dpi_fac = hello_imgui.dpi_window_size_factor()
             self._window_visible[self._get_main_window_id()] = False
-            glfw.set_window_close_callback(glfw_window_hello_imgui(), close_callback)
+            glfw.set_window_close_callback(glfw_utils.glfw_window_hello_imgui(), close_callback)
 
         params = hello_imgui.RunnerParams()
         params.app_window_params.window_geometry.size_auto = True
         params.app_window_params.restore_previous_geometry = False
         params.app_window_params.window_title = self._windows[self._get_main_window_id()]
         params.app_window_params.hidden = True
         params.fps_idling.fps_idle = 0
```

### Comparing `glassesValidator-1.0.0/src/glassesValidator/process/b_codeMarkerInterval.py` & `glassesValidator-1.0.1/src/glassesValidator/process/b_codeMarkerInterval.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/process/c_detectMarkers.py` & `glassesValidator-1.0.1/src/glassesValidator/process/c_detectMarkers.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/process/d_gazeToPoster.py` & `glassesValidator-1.0.1/src/glassesValidator/process/d_gazeToPoster.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/process/e1_computeOffsetsToTargets.py` & `glassesValidator-1.0.1/src/glassesValidator/process/e1_computeOffsetsToTargets.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/process/e2_determineFixationIntervals.py` & `glassesValidator-1.0.1/src/glassesValidator/process/e2_determineFixationIntervals.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/process/f_calculateDataQuality.py` & `glassesValidator-1.0.1/src/glassesValidator/process/f_calculateDataQuality.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/resources/fonts/Karla-Regular.ttf` & `glassesValidator-1.0.1/src/glassesValidator/resources/fonts/Karla-Regular.ttf`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/resources/fonts/NotoSans-Regular.ttf` & `glassesValidator-1.0.1/src/glassesValidator/resources/fonts/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/resources/fonts/materialdesignicons-webfont.7.0.96.ttf` & `glassesValidator-1.0.1/src/glassesValidator/resources/fonts/materialdesignicons-webfont.7.0.96.ttf`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/resources/icons/icon.icns` & `glassesValidator-1.0.1/src/glassesValidator/resources/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/resources/icons/icon.ico` & `glassesValidator-1.0.1/src/glassesValidator/resources/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/resources/icons/icon.png` & `glassesValidator-1.0.1/src/glassesValidator/resources/icons/icon.png`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/utils/__init__.py` & `glassesValidator-1.0.1/src/glassesValidator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/utils/makeVideo.py` & `glassesValidator-1.0.1/src/glassesValidator/utils/makeVideo.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/core.py` & `glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/core.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/iso.py` & `glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/iso.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/mpeglookups.py` & `glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/mpeglookups.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/non_iso.py` & `glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/non_iso.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/summary.py` & `glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/summary.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator/utils/mp4analyser/util.py` & `glassesValidator-1.0.1/src/glassesValidator/utils/mp4analyser/util.py`

 * *Files identical despite different names*

### Comparing `glassesValidator-1.0.0/src/glassesValidator.egg-info/SOURCES.txt` & `glassesValidator-1.0.1/src/glassesValidator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

