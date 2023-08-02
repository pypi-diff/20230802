# Comparing `tmp/gender-detection-local-0.1.0.tar.gz` & `tmp/gender-detection-local-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gender-detection-local-0.1.0.tar", last modified: Thu Jul 27 13:44:23 2023, max compression
+gzip compressed data, was "gender-detection-local-0.1.1.tar", last modified: Wed Aug  2 14:02:42 2023, max compression
```

## Comparing `gender-detection-local-0.1.0.tar` & `gender-detection-local-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:44:23.958087 gender-detection-local-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:44:23.958087 gender-detection-local-0.1.0/CirclesGenderDetectionPython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/CirclesGenderDetectionPython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/CirclesGenderDetectionPython/gender_detection
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/CirclesGenderDetectionPython/gender_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/CirclesGenderDetectionPython/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-27 13:44:23.958087 gender-detection-local-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:44:23.958087 gender-detection-local-0.1.0/gender_detection_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-27 13:44:23.000000 gender-detection-local-0.1.0/gender_detection_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-27 13:44:23.000000 gender-detection-local-0.1.0/gender_detection_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:44:23.000000 gender-detection-local-0.1.0/gender_detection_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 13:44:23.000000 gender-detection-local-0.1.0/gender_detection_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:44:23.958087 gender-detection-local-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:02:42.318808 gender-detection-local-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:02:42.318808 gender-detection-local-0.1.1/CirclesGenderDetectionPython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:02:30.000000 gender-detection-local-0.1.1/CirclesGenderDetectionPython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-08-02 14:02:30.000000 gender-detection-local-0.1.1/CirclesGenderDetectionPython/gender_detection
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-08-02 14:02:30.000000 gender-detection-local-0.1.1/CirclesGenderDetectionPython/gender_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-02 14:02:30.000000 gender-detection-local-0.1.1/CirclesGenderDetectionPython/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:02:42.318808 gender-detection-local-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 14:02:31.000000 gender-detection-local-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:02:42.318808 gender-detection-local-0.1.1/gender_detection_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:02:42.000000 gender-detection-local-0.1.1/gender_detection_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 14:02:42.000000 gender-detection-local-0.1.1/gender_detection_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:02:42.000000 gender-detection-local-0.1.1/gender_detection_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:02:42.000000 gender-detection-local-0.1.1/gender_detection_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 14:02:31.000000 gender-detection-local-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:02:42.318808 gender-detection-local-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 14:02:31.000000 gender-detection-local-0.1.1/setup.py
```

### Comparing `gender-detection-local-0.1.0/CirclesGenderDetectionPython/gender_detection` & `gender-detection-local-0.1.1/CirclesGenderDetectionPython/gender_detection`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.1.0/CirclesGenderDetectionPython/gender_detection.py` & `gender-detection-local-0.1.1/CirclesGenderDetectionPython/gender_detection.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from tensorflow.io import read_file
 from tensorflow.image import decode_jpeg,resize,flip_left_right
 from tensorflow.keras.utils import image_dataset_from_directory
 from keras.models import Model,Sequential,load_model
 from keras.layers import Input,Conv2D,MaxPooling2D,Dropout,Flatten,Dense,GlobalAveragePooling2D,BatchNormalization
 from dotenv import load_dotenv
 load_dotenv()
-from LoggerLocalPythonPackage.LoggerServiceSingleton import locallgr
+from logger_local_python_package.localLogger import _Local_Logger as local_logger
 
 
 
 
 
 
 
@@ -99,24 +99,25 @@
         """
         GenderClassifier is a class that detects the gender of a person through webcam images.
 
         Args:
             train (bool): a boolean indicating whether to train the model or not. Defaults to False.
             predict (bool): a boolean indicating whether to predict the gender or not. Defaults to True.
         """
-        self.lgrins = locallgr
+        self.lgrins=local_logger
+        self.lgrins.init({'component_id':"13"})
 
     def predict_gender(self,model_path,image_path=None):
         """
         This function captures an image from the webcam and predicts the gender of the person.
 
         Returns:
             str: a string indicating the predicted gender ('Male' or 'Female').
         """
-
+        self.lgrins.start()
         # Test Functionality
         if image_path is not None:
            # Read the contents of the image file
            image = read_file(image_path)
 
            # Decode the JPEG-encoded image into a tensor
            image = decode_jpeg(image)
@@ -145,31 +146,34 @@
             image = flip_left_right(image)
 
         model = load_model(model_path)
         prediction = model.predict(expand_dims(image, axis=0))[0]
         self.lgrins.info("Prediction Confidence (>0.5 Male,<=0.5 Female)",prediction)
         if prediction > 0.5:
             #print("Male")
+            self.lgrins.stop()
             return "Male"
         else:
             #print("Female")
+            self.lgrins.stop()
             return "Female"
 
 
 
 
 
 
     def train_model(self, save=True):
         """
         This function trains a model to detect the gender of a person through images.
 
         Args:
             save (bool): a boolean indicating whether to save the trained model or not. Defaults to True.
         """
+        self.lgrins.start()
         # Build Model With Transfer Learning from Pre-Trained VGG-Face
         model = create_model((178, 218, 3))
 
         train = image_dataset_from_directory("./Train", image_size=(178, 218))
         validation = image_dataset_from_directory("./Validation", image_size=(178, 218))
         test = image_dataset_from_directory("./Test", image_size=(178, 218))
 
@@ -179,7 +183,8 @@
         model.fit(train, epochs=10, batch_size=32, validation_data=validation)
 
         # Evaluate the performance of the model on a validation set
         loss, accuracy = model.evaluate(test)
         self.lgrins.info(loss, accuracy)
         if save is True:
             model.save("gender_detection", save_format='h5')
+        self.lgrins.stop()
```

### Comparing `gender-detection-local-0.1.0/README.md` & `gender-detection-local-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.1.0/setup.py` & `gender-detection-local-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='gender-detection-local',  
-     version='0.1.0',
+     version='0.1.1',
      author="Circles",
      author_email="info@circles.zone",
      description="PyPI Package for gender detection",
      long_description="This is a package for running gender detection and predicting gender",
      long_description_content_type="text/markdown",
      url="https://github.com/circles-zone/gender-detection-local-python-package",
      packages=setuptools.find_packages(),
```

