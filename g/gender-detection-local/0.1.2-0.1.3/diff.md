# Comparing `tmp/gender-detection-local-0.1.2.tar.gz` & `tmp/gender-detection-local-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gender-detection-local-0.1.2.tar", last modified: Wed Aug  2 14:15:35 2023, max compression
+gzip compressed data, was "gender-detection-local-0.1.3.tar", last modified: Wed Aug  2 14:25:04 2023, max compression
```

## Comparing `gender-detection-local-0.1.2.tar` & `gender-detection-local-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:35.146825 gender-detection-local-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:35.142825 gender-detection-local-0.1.2/CirclesGenderDetectionPython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:12.000000 gender-detection-local-0.1.2/CirclesGenderDetectionPython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-08-02 14:15:12.000000 gender-detection-local-0.1.2/CirclesGenderDetectionPython/gender_detection
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-08-02 14:15:12.000000 gender-detection-local-0.1.2/CirclesGenderDetectionPython/gender_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-02 14:15:12.000000 gender-detection-local-0.1.2/CirclesGenderDetectionPython/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:15:35.146825 gender-detection-local-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 14:15:13.000000 gender-detection-local-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:35.146825 gender-detection-local-0.1.2/gender_detection_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:15:35.000000 gender-detection-local-0.1.2/gender_detection_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 14:15:35.000000 gender-detection-local-0.1.2/gender_detection_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:15:35.000000 gender-detection-local-0.1.2/gender_detection_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:15:35.000000 gender-detection-local-0.1.2/gender_detection_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 14:15:13.000000 gender-detection-local-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:15:35.146825 gender-detection-local-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 14:15:13.000000 gender-detection-local-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:25:04.131306 gender-detection-local-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:25:04.127306 gender-detection-local-0.1.3/CirclesGenderDetectionPython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:24:53.000000 gender-detection-local-0.1.3/CirclesGenderDetectionPython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-08-02 14:24:53.000000 gender-detection-local-0.1.3/CirclesGenderDetectionPython/gender_detection
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-08-02 14:24:53.000000 gender-detection-local-0.1.3/CirclesGenderDetectionPython/gender_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-02 14:24:53.000000 gender-detection-local-0.1.3/CirclesGenderDetectionPython/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:25:04.131306 gender-detection-local-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 14:24:53.000000 gender-detection-local-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:25:04.127306 gender-detection-local-0.1.3/gender_detection_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:25:04.000000 gender-detection-local-0.1.3/gender_detection_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 14:25:04.000000 gender-detection-local-0.1.3/gender_detection_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:25:04.000000 gender-detection-local-0.1.3/gender_detection_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:25:04.000000 gender-detection-local-0.1.3/gender_detection_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 14:24:53.000000 gender-detection-local-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:25:04.131306 gender-detection-local-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 14:24:53.000000 gender-detection-local-0.1.3/setup.py
```

### Comparing `gender-detection-local-0.1.2/CirclesGenderDetectionPython/gender_detection` & `gender-detection-local-0.1.3/CirclesGenderDetectionPython/gender_detection`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.1.2/CirclesGenderDetectionPython/gender_detection.py` & `gender-detection-local-0.1.3/CirclesGenderDetectionPython/gender_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 load_dotenv()
 from logger_local.LoggerService import LoggerService
 
 
 
 
 
-
 def create_model(input_shape):
     """
     Function to create a CNN model with multiple Convolutional, MaxPooling, and Dense layers. The model takes
     as input an image tensor of shape (input_shape) and outputs a prediction vector of shape (1,). 
 
     Args:
         input_shape (tuple): A tuple representing the shape of input tensor of an image.
```

### Comparing `gender-detection-local-0.1.2/README.md` & `gender-detection-local-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.1.2/setup.py` & `gender-detection-local-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='gender-detection-local',  
-     version='0.1.2',
+     version='0.1.3',
      author="Circles",
      author_email="info@circles.zone",
      description="PyPI Package for gender detection",
      long_description="This is a package for running gender detection and predicting gender",
      long_description_content_type="text/markdown",
      url="https://github.com/circles-zone/gender-detection-local-python-package",
      packages=setuptools.find_packages(),
```

