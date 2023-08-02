# Comparing `tmp/gender-detection-local-0.1.5.tar.gz` & `tmp/gender-detection-local-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gender-detection-local-0.1.5.tar", last modified: Wed Aug  2 14:59:31 2023, max compression
+gzip compressed data, was "gender-detection-local-0.1.6.tar", last modified: Wed Aug  2 15:14:07 2023, max compression
```

## Comparing `gender-detection-local-0.1.5.tar` & `gender-detection-local-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:59:31.031217 gender-detection-local-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:59:31.031217 gender-detection-local-0.1.5/CirclesGenderDetectionPython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:59:16.000000 gender-detection-local-0.1.5/CirclesGenderDetectionPython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-08-02 14:59:16.000000 gender-detection-local-0.1.5/CirclesGenderDetectionPython/gender_detection
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-08-02 14:59:16.000000 gender-detection-local-0.1.5/CirclesGenderDetectionPython/gender_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-02 14:59:16.000000 gender-detection-local-0.1.5/CirclesGenderDetectionPython/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:59:31.031217 gender-detection-local-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 14:59:16.000000 gender-detection-local-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:59:31.031217 gender-detection-local-0.1.5/gender_detection_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:59:31.000000 gender-detection-local-0.1.5/gender_detection_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 14:59:31.000000 gender-detection-local-0.1.5/gender_detection_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:59:31.000000 gender-detection-local-0.1.5/gender_detection_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:59:31.000000 gender-detection-local-0.1.5/gender_detection_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 14:59:16.000000 gender-detection-local-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:59:31.031217 gender-detection-local-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 14:59:16.000000 gender-detection-local-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:14:07.582579 gender-detection-local-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:14:07.582579 gender-detection-local-0.1.6/CirclesGenderDetectionPython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/CirclesGenderDetectionPython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/CirclesGenderDetectionPython/gender_detection
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/CirclesGenderDetectionPython/gender_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/CirclesGenderDetectionPython/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 15:14:07.582579 gender-detection-local-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:14:07.582579 gender-detection-local-0.1.6/gender_detection_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 15:14:07.000000 gender-detection-local-0.1.6/gender_detection_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 15:14:07.000000 gender-detection-local-0.1.6/gender_detection_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:14:07.000000 gender-detection-local-0.1.6/gender_detection_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 15:14:07.000000 gender-detection-local-0.1.6/gender_detection_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:14:07.586579 gender-detection-local-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/setup.py
```

### Comparing `gender-detection-local-0.1.5/CirclesGenderDetectionPython/gender_detection` & `gender-detection-local-0.1.6/CirclesGenderDetectionPython/gender_detection`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.1.5/CirclesGenderDetectionPython/gender_detection.py` & `gender-detection-local-0.1.6/CirclesGenderDetectionPython/gender_detection.py`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.1.5/README.md` & `gender-detection-local-0.1.6/README.md`

 * *Files identical despite different names*

