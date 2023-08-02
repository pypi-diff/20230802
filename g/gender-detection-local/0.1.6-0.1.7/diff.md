# Comparing `tmp/gender-detection-local-0.1.6.tar.gz` & `tmp/gender-detection-local-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gender-detection-local-0.1.6.tar", last modified: Wed Aug  2 15:14:07 2023, max compression
+gzip compressed data, was "gender-detection-local-0.1.7.tar", last modified: Wed Aug  2 15:20:51 2023, max compression
```

## Comparing `gender-detection-local-0.1.6.tar` & `gender-detection-local-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:14:07.582579 gender-detection-local-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:14:07.582579 gender-detection-local-0.1.6/CirclesGenderDetectionPython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/CirclesGenderDetectionPython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/CirclesGenderDetectionPython/gender_detection
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/CirclesGenderDetectionPython/gender_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/CirclesGenderDetectionPython/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 15:14:07.582579 gender-detection-local-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:14:07.582579 gender-detection-local-0.1.6/gender_detection_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 15:14:07.000000 gender-detection-local-0.1.6/gender_detection_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 15:14:07.000000 gender-detection-local-0.1.6/gender_detection_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:14:07.000000 gender-detection-local-0.1.6/gender_detection_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 15:14:07.000000 gender-detection-local-0.1.6/gender_detection_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:14:07.586579 gender-detection-local-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 15:13:55.000000 gender-detection-local-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:20:51.305804 gender-detection-local-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:20:51.305804 gender-detection-local-0.1.7/CirclesGenderDetectionPython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 15:20:37.000000 gender-detection-local-0.1.7/CirclesGenderDetectionPython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-08-02 15:20:37.000000 gender-detection-local-0.1.7/CirclesGenderDetectionPython/gender_detection
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-08-02 15:20:37.000000 gender-detection-local-0.1.7/CirclesGenderDetectionPython/gender_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-02 15:20:37.000000 gender-detection-local-0.1.7/CirclesGenderDetectionPython/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 15:20:51.305804 gender-detection-local-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 15:20:38.000000 gender-detection-local-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:20:51.305804 gender-detection-local-0.1.7/gender_detection_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 15:20:51.000000 gender-detection-local-0.1.7/gender_detection_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 15:20:51.000000 gender-detection-local-0.1.7/gender_detection_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:20:51.000000 gender-detection-local-0.1.7/gender_detection_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 15:20:51.000000 gender-detection-local-0.1.7/gender_detection_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 15:20:38.000000 gender-detection-local-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:20:51.305804 gender-detection-local-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 15:20:38.000000 gender-detection-local-0.1.7/setup.py
```

### Comparing `gender-detection-local-0.1.6/CirclesGenderDetectionPython/gender_detection` & `gender-detection-local-0.1.7/CirclesGenderDetectionPython/gender_detection`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.1.6/CirclesGenderDetectionPython/gender_detection.py` & `gender-detection-local-0.1.7/CirclesGenderDetectionPython/gender_detection.py`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.1.6/README.md` & `gender-detection-local-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.1.6/setup.py` & `gender-detection-local-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='gender-detection-local',  
-     version='0.1.6',
+     version='0.1.7',
      author="Circles",
      author_email="info@circles.zone",
      description="PyPI Package for gender detection",
      long_description="This is a package for running gender detection and predicting gender",
      long_description_content_type="text/markdown",
      url="https://github.com/circles-zone/gender-detection-local-python-package",
      packages=setuptools.find_packages(),
```

