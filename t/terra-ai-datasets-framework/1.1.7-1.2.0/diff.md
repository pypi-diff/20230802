# Comparing `tmp/terra_ai_datasets_framework-1.1.7.tar.gz` & `tmp/terra_ai_datasets_framework-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terra_ai_datasets_framework-1.1.7.tar", last modified: Mon Apr 17 11:40:42 2023, max compression
+gzip compressed data, was "terra_ai_datasets_framework-1.2.0.tar", last modified: Wed Aug  2 07:56:03 2023, max compression
```

## Comparing `terra_ai_datasets_framework-1.1.7.tar` & `terra_ai_datasets_framework-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:42.578578 terra_ai_datasets_framework-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-17 11:40:42.578578 terra_ai_datasets_framework-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 11:40:42.578578 terra_ai_datasets_framework-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:42.574578 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:42.574578 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/preprocessings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:42.574578 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/creation_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:42.574578 terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-17 11:40:42.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 11:40:42.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:40:42.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-17 11:40:42.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 11:40:42.000000 terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:42.578578 terra_ai_datasets_framework-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-17 11:40:31.000000 terra_ai_datasets_framework-1.1.7/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:56:03.148731 terra_ai_datasets_framework-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-02 07:56:03.148731 terra_ai_datasets_framework-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 07:56:03.148731 terra_ai_datasets_framework-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:56:03.136731 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21378 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:56:03.140731 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14691 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34149 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/preprocessings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:56:03.144731 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/augmentation_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/creation_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:56:03.144731 terra_ai_datasets_framework-1.2.0/terra_ai_datasets_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-02 07:56:03.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-02 07:56:03.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 07:56:03.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-02 07:56:03.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 07:56:03.000000 terra_ai_datasets_framework-1.2.0/terra_ai_datasets_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:56:03.148731 terra_ai_datasets_framework-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-02 07:55:53.000000 terra_ai_datasets_framework-1.2.0/tests/test_timeseries.py
```

### Comparing `terra_ai_datasets_framework-1.1.7/setup.py` & `terra_ai_datasets_framework-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-__version__ = "1.1.7"
-
 from setuptools import setup, find_packages
+from terra_ai_datasets import __version__
 
 DESCRIPTION = "Framework to create a dataset to train a neural network."
 LONG_DESCRIPTION = "terra_ai_datasets is a framework to create " \
                    "a dataset to train a neural network model based on a Keras."
 
 setup(
     name="terra_ai_datasets_framework",
```

### Comparing `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/create.py` & `terra_ai_datasets_framework-1.2.0/terra_ai_datasets/create.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-import os.path
 from typing import Dict, Union, Any
 
+import numpy as np
+import pandas as pd
+from imgaug import SegmentationMapsOnImage
+from tqdm import tqdm
+
+from terra_ai_datasets.creation.augmentation import create_image_augmentation
 from terra_ai_datasets.creation.dataset import CreateDataset, CreateClassificationDataset
-from terra_ai_datasets.creation.utils import get_classes_annotation, get_classes_autosearch
-from terra_ai_datasets.creation.validators.creation_data import InputData, OutputData
+from terra_ai_datasets.creation.utils import get_classes_annotation, get_classes_autosearch, logger
+from terra_ai_datasets.creation.validators.creation_data import InputData, OutputData, InputInstructionsData, \
+    OutputInstructionsData
 from terra_ai_datasets.creation.validators import inputs as val_inputs
 from terra_ai_datasets.creation.validators import outputs as val_outputs
 from terra_ai_datasets.creation.validators.inputs import ImageScalers, TextModeTypes, TextProcessTypes
 from terra_ai_datasets.creation.validators.tasks import LayerInputTypeChoice, LayerOutputTypeChoice, \
     LayerSelectTypeChoice
 
 
@@ -20,30 +26,34 @@
             source_path: list,
             train_size: float,
             width: int,
             height: int,
             network: str,
             process: str,
             preprocessing: str = ImageScalers.none,
-            one_hot_encoding: bool = True
+            one_hot_encoding: bool = True,
+            augmentation: str = None,
+            augmentation_coef: float = 0
     ):
         """
         Класс подготовки датасета для задачи классификации изображений.
 
         :param source_path: Список относительных путей до папок с изображениями;
         :param train_size: Соотношение обучающей выборки к валидационной;
         :param width: Ширина изображений;
         :param height: Высота изображений;
         :param process: Метод обработки изображений при изменении размерности. Варианты: "Stretch", "Fit", "Cut";
         :param network: Постобработка массивов под определенный вид нейронной сети. Варианты: "Convolutional", "Linear";
         :param preprocessing: Выбор скейлера. Варианты: "None", "MinMaxScaler", "TerraImageScaler";
         :param one_hot_encoding: Перевод Y массивов в формат One-Hot Encoding.
+        :param augmentation: Словарь с параметрами для аугментации изображений.
         """
         super().__init__(source_path=source_path, train_size=train_size, width=width, height=height, process=process,
-                         network=network, preprocessing=preprocessing, one_hot_encoding=one_hot_encoding)
+                         network=network, preprocessing=preprocessing, one_hot_encoding=one_hot_encoding,
+                         augmentation=augmentation, augmentation_coef=augmentation_coef)
 
 
 class ImageSegmentation(CreateDataset):
     input_type = LayerInputTypeChoice.Image
     output_type = LayerOutputTypeChoice.Segmentation
 
     def __init__(
@@ -55,15 +65,17 @@
             height: int,
             network: str,
             process: str,
             rgb_range: int,
             classes: Dict[str, list] = None,
             num_classes: int = None,
             classes_path: str = None,
-            preprocessing: str = ImageScalers.none
+            preprocessing: str = ImageScalers.none,
+            augmentation: str = None,
+            augmentation_coef: float = 0
     ):
         """
         Класс подготовки датасета для задачи сегментации изображений.
 
         :param source_path: Список относительных путей до папок с изображениями;
         :param target_path: Список относительных путей до папок с масками сегментации;
         :param train_size: Соотношение обучающей выборки к валидационной;
@@ -71,37 +83,63 @@
         :param height: Высота изображений;
         :param process: Метод обработки изображений при изменении размерности. Варианты: "Stretch", "Fit", "Cut";
         :param network: Постобработка массивов под определенный вид нейронной сети. Варианты: "Convolutional", "Linear";
         :param preprocessing: Выбор скейлера. Варианты: "None", "MinMaxScaler", "TerraImageScaler";
         :param rgb_range: Диапазон, при котором пиксели будут отнесены к классу;
         :param classes: Названия классов и их RGB значения в виде словаря;
         :param classes_path: Путь к txt файлу с указанием названия классов и их RGB значений.
+        :param augmentation: Словарь с параметрами для аугментации изображений.
         """
         if not classes and not classes_path and num_classes:
             classes = get_classes_autosearch(source=target_path, num_classes=num_classes, mask_range=rgb_range,
                                              height=height, width=width, frame_mode=process)
         elif not classes and classes_path:
             classes = get_classes_annotation(classes_path)
 
         super().__init__(source_path=source_path, target_path=target_path, train_size=train_size,  width=width,
                          height=height, process=process, network=network, preprocessing=preprocessing,
-                         rgb_range=rgb_range, classes=classes)
+                         rgb_range=rgb_range, classes=classes, augmentation=augmentation,
+                         augmentation_coef=augmentation_coef)
 
     def preprocess_put_data(self, data, data_type: LayerSelectTypeChoice):
         puts_data = super().preprocess_put_data(data, data_type)
 
         puts_data[2][f"2_{self.output_type.value}"].parameters.height = \
             puts_data[1][f"1_{self.input_type.value}"].parameters.height
         puts_data[2][f"2_{self.output_type.value}"].parameters.width = \
             puts_data[1][f"1_{self.input_type.value}"].parameters.width
         puts_data[2][f"2_{self.output_type.value}"].parameters.process = \
             puts_data[1][f"1_{self.input_type.value}"].parameters.process
 
         return puts_data
 
+    def create(self, use_generator: bool = False, verbose: int = 1):
+        super().create(use_generator=use_generator, verbose=verbose)
+        if not use_generator:
+            if verbose == 0:
+                logger.info(f"Выполняется аугментация изображений и масок сегментации")
+
+            aug_idx = self.dataframe["train"]["1_Image"].str.contains("augm").tolist()
+            orig_shape = self.X['train']['input_1'][0].shape
+            for i, val in enumerate(aug_idx):
+                if val == True:  # Не менять!
+                    x_sample = self.X['train']['input_1'][i]
+                    y_sample = self.Y['train']['output_1'][i]
+                    if self.preprocessing.get("1_Image"):
+                        x_sample = self.preprocessing["1_Image"].inverse_transform(x_sample.reshape(-1, 1)).reshape(orig_shape).astype(np.uint8)
+                    y_maps = SegmentationMapsOnImage(y_sample, shape=y_sample.shape)
+                    x_sample, y_sample = self.augmentation["1_Image"](image=x_sample, segmentation_maps=y_maps)
+                    if self.preprocessing.get("1_Image"):
+                        x_sample = self.preprocessing["1_Image"].transform(x_sample.reshape(-1, 1)).reshape(orig_shape)
+                    self.X["train"]["input_1"][i] = x_sample
+                    self.Y["train"]["output_1"][i] = y_sample.arr
+
+            if verbose == 0:
+                logger.info(f"Готово!")
+
 
 class TextClassification(CreateClassificationDataset):
     input_type = LayerInputTypeChoice.Text
     output_type = LayerOutputTypeChoice.Classification
 
     def __init__(
             self,
```

### Comparing `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/arrays.py` & `terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/arrays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+from pathlib import Path
 from typing import Any
 
 import cv2
 import numpy as np
 import librosa.feature as librosa_feature
 from librosa import load as librosa_load
 from PIL import Image
@@ -120,17 +121,17 @@
     @abstractmethod
     def preprocess(self, array: np.ndarray, preprocess: Any, parameters: Any):
         pass
 
 
 class ImageArray(Array):
 
-    def create(self, source: str, parameters: ImageValidator):
+    def create(self, source: Path, parameters: ImageValidator):
 
-        image = Image.open(source)
+        image = Image.open(str(source).split(";")[0])
         array = np.asarray(image)
         if array.ndim == 2:
             array = np.stack([array, array, array], axis=-1)
         array = resize_frame(image_array=array,
                              target_shape=(parameters.height, parameters.width),
                              frame_mode=parameters.process)
         if parameters.network == ImageNetworkTypes.linear:
```

### Comparing `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/dataset.py` & `terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/dataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import json
 from pathlib import Path
 from datetime import datetime
-from typing import Union, Dict, Any
+from typing import Union, Dict, List, Any, NoReturn
 
 from IPython.display import display
+from sklearn.utils import resample
 from tensorflow.python.data.ops.dataset_ops import DatasetV2 as Dataset
 from tensorflow import TensorSpec
 from tqdm import tqdm
 import numpy as np
 import pandas as pd
 import joblib
 
-from terra_ai_datasets.creation import preprocessings, utils, visualize
+from terra_ai_datasets.creation import preprocessings, utils, visualize, augmentation
+from terra_ai_datasets.creation.augmentation import create_image_augmentation
 from terra_ai_datasets.creation.utils import apply_pymorphy, process_directory_paths, decamelize, create_put_array, \
     preprocess_put_array
 from terra_ai_datasets.creation.validators import creation_data
 from terra_ai_datasets.creation.validators.creation_data import InputData, OutputData, InputInstructionsData, \
     OutputInstructionsData
 from terra_ai_datasets.creation.validators import dataset
 from terra_ai_datasets.creation.validators import inputs, outputs
-from terra_ai_datasets.creation.validators.inputs import CategoricalValidator, ImageScalers, TextProcessTypes
+from terra_ai_datasets.creation.validators.inputs import CategoricalValidator, ImageScalers, TextProcessTypes, \
+    AugmentationData
 from terra_ai_datasets.creation.validators.structure import DatasetData
 
 from terra_ai_datasets.creation.validators.tasks import LayerInputTypeChoice, LayerOutputTypeChoice, \
     LayerSelectTypeChoice
 
 
 def postprocess_put_array(put_arr: list, put_data_type: Union[LayerInputTypeChoice, LayerOutputTypeChoice]) \
@@ -46,26 +49,39 @@
 
 class TerraDataset:
 
     def __init__(self):
         self.X: Dict[str, Dict[str, np.ndarray]] = {"train": {}, "val": {}}
         self.Y: Dict[str, Dict[str, np.ndarray]] = {"train": {}, "val": {}}
         self.preprocessing: Dict[str, Any] = {}
+        self.augmentation: Dict[str, Any] = {}
         self.dataframe: Dict[str, pd.DataFrame] = {}
         self.dataset_data: DatasetData = None
         self.put_instructions: Dict[int, Dict[str, Union[InputInstructionsData, OutputInstructionsData]]] = {}
 
         self._dataset: Dict[str, Dataset] = {"train": None, "val": None}
 
     @property
     def dataset(self):
         if not self._dataset["train"] and not self._dataset["val"]:
             return 'Массивы не были созданы. Вызовите метод .create(use_generator: bool = False)'
         return self._dataset
 
+    @property
+    def train(self):
+        if not self._dataset["train"]:
+            return 'Массивы не были созданы. Вызовите метод .create(use_generator: bool = False)'
+        return self._dataset["train"]
+
+    @property
+    def val(self):
+        if not self._dataset["val"]:
+            return 'Массивы не были созданы. Вызовите метод .create(use_generator: bool = False)'
+        return self._dataset["val"]
+
     @staticmethod
     def create_dataset_object_from_arrays(x_arrays: Dict[str, np.ndarray], y_arrays: Dict[str, np.ndarray]) -> Dataset:
         return Dataset.from_tensor_slices((x_arrays, y_arrays))
 
     def create_dataset_object_from_instructions(self, put_instr, dataframe) -> Dataset:
 
         output_signature = [{}, {}]
@@ -143,15 +159,24 @@
                     inp_id += 1
                 else:
                     out_dict[f"output_{out_id}"] = put_array
                     out_id += 1
 
             yield inp_dict, out_dict
 
-    def create(self, use_generator: bool = False):
+    def create(self, use_generator: bool = False, verbose: int = 1):
+
+        if verbose not in [0, 1]:
+            raise ValueError("Параметр verbose принимает значение 0 или 1")
+
+        if verbose == 0:
+            disable = True
+            utils.logger.info(f"Выполняется процесс создания датасетов")
+        else:
+            disable = False
 
         for split, dataframe in self.dataframe.items():
             inp_id, out_id = 1, 1
             for put_id, cols_dict in self.put_instructions.items():
                 if use_generator and split != "train":
                     continue
                 for col_name, put_data in cols_dict.items():
@@ -178,15 +203,16 @@
                         total_samples -= length * 2
                         if put_data.type in [LayerOutputTypeChoice.Depth, LayerOutputTypeChoice.Trend]:
                             offset = put_data.parameters.length
                             if put_data.type == LayerOutputTypeChoice.Trend:
                                 offset -= 1
                     for row_idx in tqdm(
                             range(0, total_samples, step),
-                            desc=f"{datetime.now().strftime('%H:%M:%S')} | Формирование массивов {split} - {put_data.type} - {col_name}"
+                            desc=f"{datetime.now().strftime('%H:%M:%S')} | Формирование массивов {split} - {put_data.type} - {col_name}",
+                            disable=disable
                     ):
                         data_to_send = dataframe.loc[row_idx+offset:row_idx+offset+length-1, col_name].to_list()
                         data_to_send = data_to_send[0] if len(data_to_send) == 1 else data_to_send
                         sample_array = create_put_array(data_to_send, put_data)
                         if self.preprocessing.get(col_name) and split == "train":
                             if put_data.type == LayerInputTypeChoice.Text:
                                 pass
@@ -200,14 +226,22 @@
                             )
 
                     if self.preprocessing.get(col_name) and split == "train":
                         if put_data.type == LayerInputTypeChoice.Text:
                             if put_data.parameters.preprocessing in [TextProcessTypes.embedding, TextProcessTypes.bag_of_words]:
                                 self.preprocessing[col_name].fit_on_texts(col_array)
 
+                    if self.augmentation.get(col_name) and split == "train":
+                        if put_data.type == LayerInputTypeChoice.Image:
+                            aug_idx = dataframe[col_name].str.contains("augm").tolist()
+                            if not self.output_type == LayerOutputTypeChoice.Segmentation:
+                                for i, val in enumerate(aug_idx):
+                                    if val:
+                                        col_array[i] = self.augmentation[col_name](image=np.array(col_array[i]))
+
                     if self.preprocessing.get(col_name) and not use_generator:
                         col_array = preprocess_put_array(
                             np.array(col_array), put_data, self.preprocessing[col_name]
                         )
                     if not use_generator:
                         put_array.append(col_array if len(col_array) > 1 else col_array[0])
 
@@ -223,26 +257,56 @@
             if not use_generator:
                 self._dataset[split] = self.create_dataset_object_from_arrays(self.X[split], self.Y[split])
             else:
                 self._dataset[split] = self.create_dataset_object_from_instructions(
                     self.put_instructions, dataframe
                 )
         self.dataset_data.is_created = True
+        if verbose == 0:
+            utils.logger.info(f"Готово!")
 
     def visualize(self):
         getattr(visualize, f"visualize_{decamelize(self.dataset_data.task)}")(
+            dataframe=self.dataframe["train"],
             put_instructions=self.put_instructions,
-            preprocessing=self.preprocessing
+            preprocessing=self.preprocessing,
+            augmentation=self.augmentation
         )
 
     def evaluate_on_model(self, model, batch_size: int):
         for inp, out in self.dataset["val"].batch(batch_size):
             pred = model.predict(inp)
             yield inp, out, pred
 
+    def create_input_array(self, *args: List[str]) -> Dict[str, np.ndarray]:
+        args_idx = 0
+        input_dict = {}
+        for put_id, cols_dict in self.put_instructions.items():
+            put_array = []
+            add_to_input_dict = False
+            for col_name, put_data in cols_dict.items():
+                if put_data.type in LayerInputTypeChoice:
+                    data_to_send = args[args_idx]
+                    if put_data.type == LayerInputTypeChoice.Text:
+                        data_to_send = [data_to_send]
+                    col_array = create_put_array(data_to_send, put_data)
+                    if self.augmentation.get(col_name):
+                        col_array = self.augmentation[col_name](image=col_array)
+                    if self.preprocessing.get(col_name):
+                        col_array = preprocess_put_array(
+                            np.array(col_array), put_data, self.preprocessing[col_name]
+                        )
+                    put_array.append(col_array if len(col_array) > 1 else col_array[0])
+                    args_idx += 1
+                    add_to_input_dict = True
+            if add_to_input_dict:
+                put_array = postprocess_put_array(put_array, put_data.type)
+                input_dict[f"input_{put_id}"] = np.expand_dims(np.array(put_array), 0)
+        return input_dict
+
     def summary(self):
 
         display(self.dataframe['train'].head())
         print(f"\n\033[1mКол-во примеров в train выборке:\033[0m {len(self.dataframe['train'])}\n"
               f"\033[1mКол-во примеров в val выборке:\033[0m {len(self.dataframe['val'])}")
         print()
         if self.dataset_data.is_created:
@@ -323,18 +387,21 @@
             getattr(dataset, f"{self.input_type}{self.output_type}Validator"), **kwargs
         )
         self.put_data = self.preprocess_put_data(
             data=self.data, data_type=LayerSelectTypeChoice.table
             if self.input_type == LayerInputTypeChoice.Dataframe else LayerSelectTypeChoice.folder
         )
         self.put_instructions = self.create_put_instructions(put_data=self.put_data)
+        self.augmentation = self.create_augmentation(self.put_instructions)
         self.dataframe = self.create_table(
             self.put_instructions,
             train_size=self.data.train_size,
-            shuffle=True if self.input_type != LayerInputTypeChoice.Timeseries else False
+            shuffle=True if self.input_type != LayerInputTypeChoice.Timeseries else False,
+            aug_coef=self.data.augmentation_coef,
+            aug_data=self.augmentation
         )
 
         self.dataset_data = DatasetData(
             task=self.input_type.value + self.output_type.value,
             use_generator=False,
             is_created=False,
         )
@@ -417,16 +484,29 @@
                 new_put_data[put_id][col_name] = getattr(creation_data, f"{put_type}InstructionsData")(
                     type=put_data.type, parameters=parameters, data=data_to_pass
                 )
 
         return new_put_data
 
     @staticmethod
+    def create_augmentation(put_instructions: Dict[int, Dict[str, Union[InputInstructionsData, OutputInstructionsData]]]):
+        augmentation_data = {}
+        for put_id, cols_dict in put_instructions.items():
+            for col_name, put_data in cols_dict.items():
+                if "augmentation" in put_data.parameters.dict() and put_data.parameters.augmentation:
+                    aug_data = AugmentationData(aug_type=put_data.type, mode=put_data.parameters.augmentation)
+                    augmentation_data[col_name] = \
+                        getattr(augmentation, f"create_{put_data.type.lower()}_augmentation")(aug_data)
+        return augmentation_data
+
+    @staticmethod
     def create_table(put_instructions: Dict[int, Dict[str, Union[InputInstructionsData, OutputInstructionsData]]],
                      train_size: int,
+                     aug_data: dict,
+                     aug_coef: float,
                      shuffle: bool = True,
                      ) -> Dict[str, pd.DataFrame]:
 
         csv_data = {}
         for put_id, cols_dict in put_instructions.items():
             for col_name, put_data in cols_dict.items():
                 csv_data[col_name] = put_data.data
@@ -435,25 +515,114 @@
 
         if shuffle:
             dataframe = dataframe.sample(frac=1)
 
         train_dataframe, val_dataframe = np.split(
             dataframe, [int(train_size * len(dataframe))]
         )
+
+        if aug_data:
+            for col_name, augm_data in aug_data.items():
+                augm_df = train_dataframe.sample(int(len(train_dataframe) * aug_coef),
+                                                 replace=False if aug_coef < 1 else True)
+                augm_df[col_name] = augm_df[col_name].astype('str') + ";augm"
+                train_dataframe = pd.concat([train_dataframe, augm_df], axis=0)
+                train_dataframe = train_dataframe.sample(frac=1)
+
         dataframe = {"train": train_dataframe.reset_index(drop=True), "val": val_dataframe.reset_index(drop=True)}
 
         return dataframe
 
 
 class CreateClassificationDataset(CreateDataset):
 
     def __init__(self, **kwargs):
         self.y_classes = []
         super().__init__(**kwargs)
 
+    def balance_classes(self, balance_type: str) -> NoReturn:
+        """
+        В качестве аргумента option задаем способ балансирования классов
+        Один из способов должен заключаться в копировании данных для уравнивания классов.
+        Таким образом, массивы в генераторе будут содержать одинаковое количество классов.
+        Другой способ - аугментация (при классификации изображений) с режимом Light
+        - copy
+        - augmentation
+        :return:
+        """
+
+        if self.X["train"] and self.X["val"]:
+            return "Балансирование классов возможна только перед вызовом метода .create(use_generator: bool = False)"
+
+        dataframe = self.dataframe['train'].copy()
+        image_col, cls_col = None, None
+        for put_id, put_data in self.put_instructions.items():
+            for col_name, col_data in put_data.items():
+                if col_data.type == LayerInputTypeChoice.Image:
+                    image_col = col_name
+                elif col_data.type == LayerOutputTypeChoice.Classification:
+                    cls_col = col_name
+        if balance_type == "upsampling":
+            classes_list = dataframe[cls_col].unique().tolist()
+            classes_length = [len(dataframe[dataframe[cls_col] == cl_name])
+                              for cl_name in classes_list]
+            max_length = max(classes_length)
+            df_list = []
+            for cl_name in classes_list:
+                df_list.append(resample(
+                    dataframe[dataframe[cls_col] == cl_name],
+                    replace=True,
+                    n_samples=max_length)
+                )
+            self.dataframe['train'] = pd.concat(df_list).sample(frac=1).reset_index(drop=True)
+            print(f"Максимальное количество примеров одного класса - {max_length} ({classes_list[classes_length.index(max_length)]}).")
+            for cl_name, cl_length in zip(classes_list, classes_length):
+                print(f"{cl_name}: {cl_length} - {max_length}")
+
+        elif balance_type == "undersampling":
+            dataframe = dataframe.groupby(cls_col)
+            classes_list = dataframe.size().index.tolist()
+            classes_length = dataframe.size().tolist()
+            min_length = min(classes_length)
+            self.dataframe['train'] = dataframe.apply(lambda x: x.sample(min_length))\
+                .sample(frac=1).reset_index(drop=True)
+            print(f"Минимальное количество примеров одного класса - {min_length} ({classes_list[classes_length.index(min_length)]}).")
+            for cl_name, cl_length in zip(classes_list, classes_length):
+                print(f"{cl_name}: {cl_length} - {min_length}")
+
+        elif balance_type == "augmentation":
+            if image_col:
+                aug_data = AugmentationData(aug_type="Image", mode="Maximum")
+                self.augmentation[image_col] = create_image_augmentation(image_augmentation_data=aug_data)
+                classes_list = dataframe[cls_col].unique().tolist()
+                classes_length = [len(dataframe[dataframe[cls_col] == cl_name])
+                                  for cl_name in classes_list]
+                max_length = max(classes_length)
+                df_list = []
+                for cl_name in classes_list:
+                    data = dataframe[dataframe[cls_col] == cl_name]
+                    cl_samples = classes_length[classes_list.index(cl_name)]
+                    samples_to_add = max_length - cl_samples
+                    if samples_to_add:
+                        add_data = data.sample(samples_to_add)
+                        add_data[image_col][~add_data[image_col].str.contains("augm")] = \
+                            add_data[image_col][~add_data[image_col].str.contains("augm")] + ";augm"
+                        data = pd.concat([data, add_data])
+                    df_list.append(data)
+                self.dataframe['train'] = pd.concat(df_list).sample(frac=1).reset_index(drop=True)
+                print(f"Максимальное количество примеров одного класса - {max_length} ({classes_list[classes_length.index(max_length)]}).")
+                for cl_name, cl_length in zip(classes_list, classes_length):
+                    print(f"{cl_name}: {cl_length} - {max_length}")
+            else:
+                print('Способ балансировки классов "augmentation" доступен только для изображений')
+
+        else:
+            raise ValueError(f"Неизвестный способ балансировки классов: {balance_type}. "
+                             f"Доступны: 'undersampling', 'upsampling', 'augmentation'")
+
     def create_put_instructions(self, put_data) -> \
             Dict[int, Dict[str, Union[InputInstructionsData, OutputInstructionsData]]]:
 
         new_put_data = {}
         for put_id, cols_dict in put_data.items():
             new_put_data[put_id] = {}
             for col_name, put_data in cols_dict.items():
```

### Comparing `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/preprocessings.py` & `terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/preprocessings.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/utils.py` & `terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import logging
 import os
 import re
 from enum import Enum
 from typing import Union, List, Any
 
-import cv2
 import librosa
 import numpy as np
 import pandas as pd
 import pymorphy2
 from pathlib import Path
 from PIL import Image
 
 from sklearn.cluster import KMeans
 from tensorflow.keras.preprocessing.text import text_to_word_sequence
 
 from terra_ai_datasets.creation import arrays
 from terra_ai_datasets.creation.arrays import resize_frame
 from terra_ai_datasets.creation.validators.creation_data import InputInstructionsData, OutputInstructionsData
-from terra_ai_datasets.creation.validators.inputs import ImageProcessTypes, TextValidator, TextModeTypes, \
-    ImageValidator, AudioValidator
+from terra_ai_datasets.creation.validators.inputs import TextValidator, TextModeTypes, ImageValidator, AudioValidator
 from terra_ai_datasets.creation.validators.outputs import SegmentationValidator
 
 logger_formatter = logging.Formatter(f"%(asctime)s | %(message)s", "%H:%M:%S")
 stream_handler = logging.StreamHandler()
 stream_handler.setFormatter(logger_formatter)
 
 logger = logging.getLogger(__name__)
+if logger.hasHandlers():
+    logger.handlers.clear()
 logger.addHandler(stream_handler)
 logger.setLevel("INFO")
 
 ANNOTATION_SEPARATOR = ":"
 ANNOTATION_LABEL_NAME = "# label"
 ANNOTATION_COLOR_RGB = "color_rgb"
```

### Comparing `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/creation_data.py` & `terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/creation_data.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/dataset.py` & `terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import errno
 import os
 from pathlib import Path
 from typing import List
 
 from pydantic import BaseModel, validator
+from pydantic.types import PositiveFloat
 
 from terra_ai_datasets.creation.validators import inputs, outputs
 from terra_ai_datasets.creation.validators.tasks import LayerInputTypeChoice, LayerOutputTypeChoice
 
 
 # --- Common validators ---
 class CommonValidator(BaseModel):
     train_size: float
+    augmentation_coef: float = 0.0
 
     @validator('train_size')
     def train_size_range(cls, v):
         if not 0.0 < v <= 1.0:
-            raise ValueError('Ensure train_size is in range between 0.0 and 1.0')
+            raise ValueError('Ensure "train_size" is in range between 0.0 and 1.0')
+        return v
+
+    @validator('augmentation_coef')
+    def train_size_range(cls, v):
+        if not 0.0 <= v:
+            raise ValueError('Ensure "augmentation_coef" is greater than 0')
         return v
 
     class Config:
         use_enum_values = True
 
 
 class SourceFolderPathValidator(CommonValidator):
```

### Comparing `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/inputs.py` & `terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/inputs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,32 @@
 from enum import Enum
-from typing import Optional, List
+from typing import Optional, List, Tuple, Dict, Any
 
 from pydantic import BaseModel, validator
 from pydantic.types import PositiveInt, PositiveFloat
 
-# from terra_ai_datasets.creation.validators.dataset import DataframeInputData
+from terra_ai_datasets.creation.validators import augmentation_params
+from terra_ai_datasets.creation.validators.augmentation_params import AugmentationMode
+
+
+class BaseAugmentation(BaseModel):
+    augmentation_coef: PositiveFloat = 0.0
+
+    # @validator("augmentation_coef")
+    # def apply_coef_range(cls, v):
+    #     if not 0.0 < v:
+    #         raise ValueError('Ensure "augmentation_coef" is positive')
+    #     return v
+
+    class Config:
+        use_enum_values = True
+
+
+class AugmentationTypes(str, Enum):
+    image = "Image"
 
 
 # --- Image validators ---
 class ImageScalers(str, Enum):
     none = None
     min_max_scaler = "MinMaxScaler"
     terra_image_scaler = "TerraImageScaler"
@@ -21,20 +39,34 @@
 
 class ImageProcessTypes(str, Enum):
     stretch = "Stretch"
     fit = "Fit"
     cut = "Cut"
 
 
+class AugmentationData(BaseAugmentation):
+    aug_type: AugmentationTypes
+    mode: AugmentationMode
+    parameters: Any = None
+
+    @validator("parameters", always=True)
+    def validate_date(cls, value, values):
+        if values.get("mode"):
+            return getattr(augmentation_params, f"{values.get('aug_type')}AugmentationParameters")(
+                **getattr(augmentation_params, f"{values.get('aug_type').lower()}_mode_config")[values["mode"]]
+            )
+
+
 class ImageValidator(BaseModel):
     height: PositiveInt
     width: PositiveInt
     network: ImageNetworkTypes = ImageNetworkTypes.convolutional
     process: ImageProcessTypes = ImageProcessTypes.stretch
     preprocessing: ImageScalers = ImageScalers.none
+    augmentation: Optional[AugmentationMode]
 
 
 # --- Text validators ---
 class TextModeTypes(str, Enum):
     full = "Full"
     length_and_step = "Length and step"
```

### Comparing `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/outputs.py` & `terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/outputs.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/creation/validators/tasks.py` & `terra_ai_datasets_framework-1.2.0/terra_ai_datasets/creation/validators/tasks.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.7/terra_ai_datasets/load.py` & `terra_ai_datasets_framework-1.2.0/terra_ai_datasets/load.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.7/terra_ai_datasets_framework.egg-info/SOURCES.txt` & `terra_ai_datasets_framework-1.2.0/terra_ai_datasets_framework.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 README.md
 setup.py
 terra_ai_datasets/__init__.py
 terra_ai_datasets/create.py
 terra_ai_datasets/load.py
 terra_ai_datasets/creation/__init__.py
 terra_ai_datasets/creation/arrays.py
+terra_ai_datasets/creation/augmentation.py
 terra_ai_datasets/creation/dataset.py
 terra_ai_datasets/creation/preprocessings.py
 terra_ai_datasets/creation/utils.py
 terra_ai_datasets/creation/visualize.py
 terra_ai_datasets/creation/validators/__init__.py
+terra_ai_datasets/creation/validators/augmentation_params.py
 terra_ai_datasets/creation/validators/creation_data.py
 terra_ai_datasets/creation/validators/dataset.py
 terra_ai_datasets/creation/validators/inputs.py
 terra_ai_datasets/creation/validators/outputs.py
 terra_ai_datasets/creation/validators/structure.py
 terra_ai_datasets/creation/validators/tasks.py
 terra_ai_datasets_framework.egg-info/PKG-INFO
```

### Comparing `terra_ai_datasets_framework-1.1.7/tests/test_classification.py` & `terra_ai_datasets_framework-1.2.0/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.7/tests/test_regression.py` & `terra_ai_datasets_framework-1.2.0/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.7/tests/test_segmentation.py` & `terra_ai_datasets_framework-1.2.0/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets_framework-1.1.7/tests/test_timeseries.py` & `terra_ai_datasets_framework-1.2.0/tests/test_timeseries.py`

 * *Files identical despite different names*

