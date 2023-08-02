# Comparing `tmp/rclip-1.4.6.tar.gz` & `tmp/rclip-1.4.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.4.6.tar", max compression
+gzip compressed data, was "rclip-1.4.7a0.tar", max compression
```

## Comparing `rclip-1.4.6.tar` & `rclip-1.4.7a0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-08-01 09:22:23.983865 rclip-1.4.6/LICENSE
--rw-r--r--   0        0        0     5023 2023-08-01 09:22:23.983865 rclip-1.4.6/README.md
--rw-r--r--   0        0        0     1557 2023-08-01 09:22:23.983865 rclip-1.4.6/pyproject.toml
--rw-r--r--   0        0        0     2940 2023-08-01 09:22:23.983865 rclip-1.4.6/rclip/db.py
--rw-r--r--   0        0        0     5586 2023-08-01 09:22:23.983865 rclip-1.4.6/rclip/main.py
--rw-r--r--   0        0        0     5161 2023-08-01 09:22:23.983865 rclip-1.4.6/rclip/model.py
--rw-r--r--   0        0        0     4551 2023-08-01 09:22:23.983865 rclip-1.4.6/rclip/utils.py
--rw-r--r--   0        0        0     6529 1970-01-01 00:00:00.000000 rclip-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-02 07:11:08.082285 rclip-1.4.7a0/LICENSE
+-rw-r--r--   0        0        0     5023 2023-08-02 07:11:08.082285 rclip-1.4.7a0/README.md
+-rw-r--r--   0        0        0     1559 2023-08-02 07:11:08.082285 rclip-1.4.7a0/pyproject.toml
+-rw-r--r--   0        0        0     2940 2023-08-02 07:11:08.082285 rclip-1.4.7a0/rclip/db.py
+-rw-r--r--   0        0        0     5586 2023-08-02 07:11:08.082285 rclip-1.4.7a0/rclip/main.py
+-rw-r--r--   0        0        0     5212 2023-08-02 07:11:08.082285 rclip-1.4.7a0/rclip/model.py
+-rw-r--r--   0        0        0     4746 2023-08-02 07:11:08.082285 rclip-1.4.7a0/rclip/utils.py
+-rw-r--r--   0        0        0     6531 1970-01-01 00:00:00.000000 rclip-1.4.7a0/PKG-INFO
```

### Comparing `rclip-1.4.6/LICENSE` & `rclip-1.4.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.4.6/README.md` & `rclip-1.4.7a0/README.md`

 * *Files identical despite different names*

### Comparing `rclip-1.4.6/pyproject.toml` & `rclip-1.4.7a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.4.6"
+version = "1.4.7a0"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
```

### Comparing `rclip-1.4.6/rclip/db.py` & `rclip-1.4.7a0/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.6/rclip/main.py` & `rclip-1.4.7a0/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.4.6/rclip/model.py` & `rclip-1.4.7a0/rclip/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import re
 from typing import List, Tuple, Optional, cast
 import sys
 
-import open_clip
 import numpy as np
 from PIL import Image, UnidentifiedImageError
 from rclip import utils
-import torch
-import torch.nn
 
 QUERY_WITH_MULTIPLIER_RE = re.compile(r'^(?P<multiplier>(\d+(\.\d+)?|\.\d+|\d+\.)):(?P<query>.+)$')
 QueryWithMultiplier = Tuple[float, str]
 
 
 class Model:
   VECTOR_SIZE = 512
@@ -22,44 +19,49 @@
   def __init__(self):
     self.__model = None
     self.__preprocess = None
     self.__tokenizer = None
 
   @property
   def _tokenizer(self):
+    import open_clip
     if not self.__tokenizer:
       self.__tokenizer = open_clip.get_tokenizer(self._model_name)
     return self.__tokenizer
 
   @property
   def _model(self):
+    import open_clip
     if not self.__model:
       self.__model, _, self.__preprocess = open_clip.create_model_and_transforms(
         self._model_name,
         pretrained=self._checkpoint_name,
       )
     return self.__model
 
   @property
   def _preprocess(self):
+    import open_clip
     if not self.__preprocess:
       self.__model, _, self.__preprocess = open_clip.create_model_and_transforms(
         self._model_name,
         pretrained=self._checkpoint_name,
       )
     return self.__preprocess
 
   def compute_image_features(self, images: List[Image.Image]) -> np.ndarray:
+    import torch
     images_preprocessed = torch.stack([self._preprocess(thumb) for thumb in images]).to(self._device)
     with torch.no_grad():
       image_features = self._model.encode_image(images_preprocessed)
       image_features /= image_features.norm(dim=-1, keepdim=True)
     return image_features.cpu().numpy()
 
   def compute_text_features(self, text: List[str]) -> np.ndarray:
+    import torch
     with torch.no_grad():
       text_features = self._model.encode_text(self._tokenizer(text).to(self._device))
       text_features /= text_features.norm(dim=-1, keepdim=True)
     return text_features.cpu().numpy()
 
   @staticmethod
   def _extract_query_multiplier(query: str) -> QueryWithMultiplier:
```

### Comparing `rclip-1.4.6/rclip/utils.py` & `rclip-1.4.7a0/rclip/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import os
 import pathlib
 from PIL import Image, UnidentifiedImageError
 import re
 import requests
 import sys
+from importlib.metadata import version
 
 
 MAX_DOWNLOAD_SIZE_BYTES = 50_000_000
 DOWNLOAD_TIMEOUT_SECONDS = 60
 WIN_ABSOLUTE_FILE_PATH_REGEX = re.compile(r'^[a-z]:\\', re.I)
 
 
@@ -57,14 +58,16 @@
     prefix_chars='-+',
     epilog='hints:\n'
     '  relative file path should be prefixed with ./, e.g. "./cat.jpg", not "cat.jpg"\n'
     '  any query can be prefixed with a multiplier, e.g. "2:cat", "0.5:./cat-sleeps-on-a-chair.jpg";'
     ' adding a multiplier is especially useful when combining image and text queries because'
     ' image queries are usually weighted more than text ones\n',
   )
+  version_str = f'rclip {version("rclip")}'
+  parser.add_argument('--version', '-v', action='version', version=version_str, help=f'prints "{version_str}"')
   parser.add_argument('query', help='a text query or a path/URL to an image file')
   parser.add_argument('--add', '-a', '+', metavar='QUERY', action='append', default=[],
                       help='a text query or a path/URL to an image file to add to the "original" query,'
                       ' can be used multiple times')
   parser.add_argument('--subtract', '--sub', '-s', '-', metavar='QUERY', action='append', default=[],
                       help='a text query or a path/URL to an image file to add to the "original" query,'
                       ' can be used multiple times')
```

### Comparing `rclip-1.4.6/PKG-INFO` & `rclip-1.4.7a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.4.6
+Version: 1.4.7a0
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.8,<4.0
```

