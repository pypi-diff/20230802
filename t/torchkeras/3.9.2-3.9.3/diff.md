# Comparing `tmp/torchkeras-3.9.2.tar.gz` & `tmp/torchkeras-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchkeras-3.9.2.tar", last modified: Sun Jul 23 12:17:22 2023, max compression
+gzip compressed data, was "dist/torchkeras-3.9.3.tar", last modified: Wed Aug  2 02:55:09 2023, max compression
```

## Comparing `torchkeras-3.9.2.tar` & `torchkeras-3.9.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-23 12:17:22.227069 torchkeras-3.9.2/
--rw-r--r--   0 liangyun2   (502) staff       (20)    11325 2023-02-09 16:00:16.000000 torchkeras-3.9.2/LICENSE
--rw-r--r--   0 liangyun2   (502) staff       (20)      357 2023-02-09 16:55:42.000000 torchkeras-3.9.2/MANIFEST.in
--rw-r--r--   0 liangyun2   (502) staff       (20)     7122 2023-07-23 12:17:22.226632 torchkeras-3.9.2/PKG-INFO
--rw-r--r--   0 liangyun2   (502) staff       (20)    13125 2023-07-23 04:17:19.000000 torchkeras-3.9.2/README.md
--rw-r--r--   0 liangyun2   (502) staff       (20)       38 2023-07-23 12:17:22.227177 torchkeras-3.9.2/setup.cfg
--rw-r--r--   0 liangyun2   (502) staff       (20)     1273 2023-06-30 07:06:01.000000 torchkeras-3.9.2/setup.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-23 12:17:22.198447 torchkeras-3.9.2/torchkeras/
--rw-r--r--   0 liangyun2   (502) staff       (20)      246 2023-07-23 03:23:40.000000 torchkeras-3.9.2/torchkeras/__init__.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-23 12:17:22.218750 torchkeras-3.9.2/torchkeras/assets/
--rw-r--r--   0 liangyun2   (502) staff       (20) 10043912 2023-02-09 16:00:16.000000 torchkeras-3.9.2/torchkeras/assets/SimHei.ttf
--rw-r--r--   0 liangyun2   (502) staff       (20)  1012077 2023-02-09 16:00:16.000000 torchkeras-3.9.2/torchkeras/assets/park.jpg
--rw-r--r--   0 liangyun2   (502) staff       (20)   168949 2023-02-09 16:00:16.000000 torchkeras-3.9.2/torchkeras/assets/zidane.jpg
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-23 12:17:22.222030 torchkeras-3.9.2/torchkeras/chat/
--rw-r--r--   0 liangyun2   (502) staff       (20)       57 2023-07-06 21:05:16.000000 torchkeras-3.9.2/torchkeras/chat/__init__.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     2651 2023-07-15 08:08:54.000000 torchkeras-3.9.2/torchkeras/chat/chatglm.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     4178 2023-05-14 01:50:00.000000 torchkeras-3.9.2/torchkeras/chat/chatgpt.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     8621 2023-06-30 01:34:56.000000 torchkeras-3.9.2/torchkeras/data.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5222 2023-04-13 09:25:41.000000 torchkeras-3.9.2/torchkeras/eda.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     1628 2023-04-13 07:46:39.000000 torchkeras-3.9.2/torchkeras/email.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    12561 2023-07-14 01:20:16.000000 torchkeras-3.9.2/torchkeras/hugmodel.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    11284 2023-07-23 00:40:35.000000 torchkeras-3.9.2/torchkeras/kerascallbacks.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    13985 2023-07-23 00:24:34.000000 torchkeras-3.9.2/torchkeras/kerasmodel.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     7316 2023-02-22 02:34:47.000000 torchkeras-3.9.2/torchkeras/metrics.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-23 12:17:22.225432 torchkeras-3.9.2/torchkeras/models/
--rw-r--r--   0 liangyun2   (502) staff       (20)       75 2023-03-10 08:21:36.000000 torchkeras-3.9.2/torchkeras/models/__init__.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     4088 2023-02-24 04:01:48.000000 torchkeras-3.9.2/torchkeras/models/resnet.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    31333 2023-05-20 15:18:08.000000 torchkeras-3.9.2/torchkeras/models/ssd.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     3374 2023-02-21 12:33:54.000000 torchkeras-3.9.2/torchkeras/models/unet.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5592 2023-07-19 10:25:15.000000 torchkeras-3.9.2/torchkeras/pbar.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    10676 2023-06-10 15:29:22.000000 torchkeras-3.9.2/torchkeras/plots.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5737 2023-05-12 10:11:52.000000 torchkeras-3.9.2/torchkeras/soup.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5256 2023-05-28 13:14:40.000000 torchkeras-3.9.2/torchkeras/summary.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-23 12:17:22.226132 torchkeras-3.9.2/torchkeras/tools/
--rw-r--r--   0 liangyun2   (502) staff       (20)     3740 2023-07-12 02:27:21.000000 torchkeras-3.9.2/torchkeras/tools/catboost.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     3845 2023-07-19 10:25:57.000000 torchkeras-3.9.2/torchkeras/utils.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-23 12:17:22.201361 torchkeras-3.9.2/torchkeras.egg-info/
--rw-r--r--   0 liangyun2   (502) staff       (20)     7122 2023-07-23 12:17:22.000000 torchkeras-3.9.2/torchkeras.egg-info/PKG-INFO
--rw-r--r--   0 liangyun2   (502) staff       (20)      791 2023-07-23 12:17:22.000000 torchkeras-3.9.2/torchkeras.egg-info/SOURCES.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)        1 2023-07-23 12:17:22.000000 torchkeras-3.9.2/torchkeras.egg-info/dependency_links.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)       16 2023-07-23 12:17:22.000000 torchkeras-3.9.2/torchkeras.egg-info/requires.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)       26 2023-07-23 12:17:22.000000 torchkeras-3.9.2/torchkeras.egg-info/top_level.txt
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-08-02 02:55:09.831984 torchkeras-3.9.3/
+-rw-r--r--   0 liangyun2   (502) staff       (20)    11325 2023-02-09 16:00:16.000000 torchkeras-3.9.3/LICENSE
+-rw-r--r--   0 liangyun2   (502) staff       (20)      357 2023-02-09 16:55:42.000000 torchkeras-3.9.3/MANIFEST.in
+-rw-r--r--   0 liangyun2   (502) staff       (20)     7095 2023-08-02 02:55:09.831645 torchkeras-3.9.3/PKG-INFO
+-rw-r--r--   0 liangyun2   (502) staff       (20)    13222 2023-08-01 14:39:41.000000 torchkeras-3.9.3/README.md
+-rw-r--r--   0 liangyun2   (502) staff       (20)       38 2023-08-02 02:55:09.832038 torchkeras-3.9.3/setup.cfg
+-rw-r--r--   0 liangyun2   (502) staff       (20)     1281 2023-07-24 10:32:02.000000 torchkeras-3.9.3/setup.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-08-02 02:55:09.805450 torchkeras-3.9.3/torchkeras/
+-rw-r--r--   0 liangyun2   (502) staff       (20)      246 2023-07-25 15:12:03.000000 torchkeras-3.9.3/torchkeras/__init__.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-08-02 02:55:09.825578 torchkeras-3.9.3/torchkeras/assets/
+-rw-r--r--   0 liangyun2   (502) staff       (20) 10043912 2023-02-09 16:00:16.000000 torchkeras-3.9.3/torchkeras/assets/SimHei.ttf
+-rw-r--r--   0 liangyun2   (502) staff       (20)  1012077 2023-02-09 16:00:16.000000 torchkeras-3.9.3/torchkeras/assets/park.jpg
+-rw-r--r--   0 liangyun2   (502) staff       (20)   168949 2023-02-09 16:00:16.000000 torchkeras-3.9.3/torchkeras/assets/zidane.jpg
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-08-02 02:55:09.828137 torchkeras-3.9.3/torchkeras/chat/
+-rw-r--r--   0 liangyun2   (502) staff       (20)       57 2023-07-06 21:05:16.000000 torchkeras-3.9.3/torchkeras/chat/__init__.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     2651 2023-07-15 08:08:54.000000 torchkeras-3.9.3/torchkeras/chat/chatglm.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     4178 2023-05-14 01:50:00.000000 torchkeras-3.9.3/torchkeras/chat/chatgpt.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     8621 2023-06-30 01:34:56.000000 torchkeras-3.9.3/torchkeras/data.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5222 2023-04-13 09:25:41.000000 torchkeras-3.9.3/torchkeras/eda.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     1628 2023-04-13 07:46:39.000000 torchkeras-3.9.3/torchkeras/email.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    12561 2023-07-14 01:20:16.000000 torchkeras-3.9.3/torchkeras/hugmodel.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    11817 2023-08-02 02:37:16.000000 torchkeras-3.9.3/torchkeras/kerascallbacks.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    13196 2023-08-02 02:50:03.000000 torchkeras-3.9.3/torchkeras/kerasmodel.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     7316 2023-02-22 02:34:47.000000 torchkeras-3.9.3/torchkeras/metrics.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-08-02 02:55:09.830753 torchkeras-3.9.3/torchkeras/models/
+-rw-r--r--   0 liangyun2   (502) staff       (20)       75 2023-03-10 08:21:36.000000 torchkeras-3.9.3/torchkeras/models/__init__.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     4088 2023-02-24 04:01:48.000000 torchkeras-3.9.3/torchkeras/models/resnet.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    31333 2023-05-20 15:18:08.000000 torchkeras-3.9.3/torchkeras/models/ssd.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     3374 2023-02-21 12:33:54.000000 torchkeras-3.9.3/torchkeras/models/unet.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     6918 2023-07-26 05:50:16.000000 torchkeras-3.9.3/torchkeras/pbar.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    10717 2023-07-29 04:58:12.000000 torchkeras-3.9.3/torchkeras/plots.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5737 2023-05-12 10:11:52.000000 torchkeras-3.9.3/torchkeras/soup.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5256 2023-05-28 13:14:40.000000 torchkeras-3.9.3/torchkeras/summary.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-08-02 02:55:09.831273 torchkeras-3.9.3/torchkeras/tools/
+-rw-r--r--   0 liangyun2   (502) staff       (20)     3740 2023-07-12 02:27:21.000000 torchkeras-3.9.3/torchkeras/tools/catboost.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     3845 2023-07-19 10:25:57.000000 torchkeras-3.9.3/torchkeras/utils.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-08-02 02:55:09.809546 torchkeras-3.9.3/torchkeras.egg-info/
+-rw-r--r--   0 liangyun2   (502) staff       (20)     7095 2023-08-02 02:55:09.000000 torchkeras-3.9.3/torchkeras.egg-info/PKG-INFO
+-rw-r--r--   0 liangyun2   (502) staff       (20)      791 2023-08-02 02:55:09.000000 torchkeras-3.9.3/torchkeras.egg-info/SOURCES.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)        1 2023-08-02 02:55:09.000000 torchkeras-3.9.3/torchkeras.egg-info/dependency_links.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)       24 2023-08-02 02:55:09.000000 torchkeras-3.9.3/torchkeras.egg-info/requires.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)       26 2023-08-02 02:55:09.000000 torchkeras-3.9.3/torchkeras.egg-info/top_level.txt
```

### Comparing `torchkeras-3.9.2/LICENSE` & `torchkeras-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/PKG-INFO` & `torchkeras-3.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchkeras
-Version: 3.9.2
+Version: 3.9.3
 Summary: pytorch❤️keras
 Home-page: https://github.com/lyhue1991/torchkeras
 Author: PythonAiRoad, Laugh
 Author-email: lyhue1991@163.com
 Keywords: machine-learning,deep-learning,ML,DL,pytorch,torch,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -134,17 +134,17 @@
 |ObjectDetection——FasterRCNN| torchvision  |  [FasterRCNN](./examples/FasterRCNN——vision.ipynb) | 
 |ImageSegmentation——DeepLabV3++ | segmentation_models_pytorch |  [Deeplabv3++](./examples/Deeplabv3plus——smp.ipynb) |
 |InstanceSegmentation——MaskRCNN | detectron2 |  [MaskRCNN](./examples/MaskRCNN——detectron2.ipynb) |
 |ObjectDetection——YOLOv8 🔥🔥| ultralytics |  [YOLOv8](./examples/YOLOv8——ultralytics.ipynb) |
 |ImageClassification——SwinTransformer|timm| [Swin](./examples/SwinTransformer——timm.ipynb)|
 ||||
 |**NLP**|||
-|TextClassification——BERT 🔥🔥| transformers |  [BERT](./examples/BERT——transformers.ipynb) |
+|Seq2Seq——Transformer🔥🔥| - |  [Transformer](./examples/Dive_into_Transformer.ipynb) |
+|TextClassification——BERT | transformers |  [BERT](./examples/BERT——transformers.ipynb) |
 |TokenClassification——BERT | transformers |  [BERT_NER](./examples/BERT_NER——transformers.ipynb) |
-|FinetuneLLM——ChatGLM2 🔥🔥🔥| transformers |  [ChatGLM2](./examples/ChatGLM2——transformers.ipynb) |
 |FinetuneLLM——ChatGLM2_LoRA 🔥🔥🔥| transformers,peft |  [ChatGLM2_LoRA](./examples/ChatGLM2_LoRA——transformers.ipynb) |
 |FinetuneLLM——ChatGLM2_AdaLoRA 🔥🔥🔥| transformers,peft |  [ChatGLM2_AdaLoRA](./examples/ChatGLM2_AdaLoRA——transformers.ipynb) |
 |FinetuneLLM——ChatGLM2_QLoRA 🔥🔥🔥| transformers |  [ChatGLM2_QLoRA_Kaggle](./examples/ChatGLM2_QLoRA_Kaggle——transformers.ipynb) |
 |FinetuneLLM——BaiChuan13B_QLoRA 🔥🔥🔥| transformers |  [BaiChuan13B_QLoRA](./examples/BaiChuan13B_QLoRA——transformers.ipynb) |
 |FinetuneLLM——BaiChuan13B_NER 🔥🔥🔥| transformers |  [BaiChuan13B_NER](./examples/BaiChuan13B_NER——transformers.ipynb) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchkeras Version: 3.9.2 Summary:
+Metadata-Version: 2.1 Name: torchkeras Version: 3.9.3 Summary:
 pytorchâ¤ï¸keras Home-page: https://github.com/lyhue1991/torchkeras Author:
 PythonAiRoad, Laugh Author-email: lyhue1991@163.com Keywords: machine-
 learning,deep-learning,ML,DL,pytorch,torch,keras Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE #
 Pytorchâ¤ï¸Keras English | [ç®ä½ä¸­æ](README.md) The torchkeras library
@@ -67,19 +67,19 @@
 | segmentation_models_pytorch | [Deeplabv3++](./examples/
 Deeplabv3plusââsmp.ipynb) | |InstanceSegmentationââMaskRCNN |
 detectron2 | [MaskRCNN](./examples/MaskRCNNââdetectron2.ipynb) |
 |ObjectDetectionââYOLOv8 ð¥ð¥| ultralytics | [YOLOv8](./examples/
 YOLOv8ââultralytics.ipynb) |
 |ImageClassificationââSwinTransformer|timm| [Swin](./examples/
 SwinTransformerââtimm.ipynb)| |||| |**NLP**|||
-|TextClassificationââBERT ð¥ð¥| transformers | [BERT](./examples/
-BERTââtransformers.ipynb) | |TokenClassificationââBERT | transformers |
-[BERT_NER](./examples/BERT_NERââtransformers.ipynb) |
-|FinetuneLLMââChatGLM2 ð¥ð¥ð¥| transformers | [ChatGLM2](./examples/
-ChatGLM2ââtransformers.ipynb) | |FinetuneLLMââChatGLM2_LoRA
+|Seq2SeqââTransformerð¥ð¥| - | [Transformer](./examples/
+Dive_into_Transformer.ipynb) | |TextClassificationââBERT | transformers |
+[BERT](./examples/BERTââtransformers.ipynb) |
+|TokenClassificationââBERT | transformers | [BERT_NER](./examples/
+BERT_NERââtransformers.ipynb) | |FinetuneLLMââChatGLM2_LoRA
 ð¥ð¥ð¥| transformers,peft | [ChatGLM2_LoRA](./examples/
 ChatGLM2_LoRAââtransformers.ipynb) | |FinetuneLLMââChatGLM2_AdaLoRA
 ð¥ð¥ð¥| transformers,peft | [ChatGLM2_AdaLoRA](./examples/
 ChatGLM2_AdaLoRAââtransformers.ipynb) | |FinetuneLLMââChatGLM2_QLoRA
 ð¥ð¥ð¥| transformers | [ChatGLM2_QLoRA_Kaggle](./examples/
 ChatGLM2_QLoRA_Kaggleââtransformers.ipynb) |
 |FinetuneLLMââBaiChuan13B_QLoRA ð¥ð¥ð¥| transformers |
```

### Comparing `torchkeras-3.9.2/README.md` & `torchkeras-3.9.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -286,15 +286,16 @@
 |目标检测——FasterRCNN| torchvision  |  [FasterRCNN](./examples/FasterRCNN——vision.ipynb) | 
 |语义分割——DeepLabV3++ | segmentation_models_pytorch |  [Deeplabv3++](./examples/Deeplabv3plus——smp.ipynb) |
 |实例分割——MaskRCNN | detectron2 |  [MaskRCNN](./examples/MaskRCNN——detectron2.ipynb) |
 |目标检测——YOLOv8 🔥🔥| ultralytics |  [YOLOv8](./examples/YOLOv8——ultralytics.ipynb) |
 |图片分类——SwinTransformer|timm| [Swin](./examples/SwinTransformer——timm.ipynb)|
 ||||
 |**NLP**|||
-|文本分类——BERT🔥| transformers |  [BERT](./examples/BERT——transformers.ipynb) |
+|序列翻译——Transformer🔥🔥| - |  [Transformer](./examples/Dive_into_Transformer.ipynb) |
+|文本分类——BERT| transformers |  [BERT](./examples/BERT——transformers.ipynb) |
 |命名实体识别——BERT | transformers |  [BERT_NER](./examples/BERT_NER——transformers.ipynb) |
 |LLM微调——ChatGLM2_LoRA 🔥🔥🔥| transformers |  [ChatGLM2_LoRA](./examples/ChatGLM2_LoRA——transformers.ipynb) |
 |LLM微调——ChatGLM2_AdaLoRA 🔥🔥🔥| transformers |  [ChatGLM2_AdaLoRA](./examples/ChatGLM2_AdaLoRA——transformers.ipynb) |
 |LLM微调——ChatGLM2_QLoRA 🔥🔥🔥| transformers |  [ChatGLM2_QLoRA_Kaggle](./examples/ChatGLM2_QLoRA_Kaggle——transformers.ipynb) |
 |LLM微调——BaiChuan13B_QLoRA 🔥🔥🔥| transformers |  [BaiChuan13B_QLoRA](./examples/BaiChuan13B_QLoRA——transformers.ipynb) |
 |LLM微调——BaiChuan13B_NER 🔥🔥🔥| transformers |  [BaiChuan13B_NER](./examples/BaiChuan13B_NER——transformers.ipynb) |
```

### Comparing `torchkeras-3.9.2/setup.py` & `torchkeras-3.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     name="torchkeras",
     version=get_version(),
     author="PythonAiRoad, Laugh",
     author_email="lyhue1991@163.com",
     description="pytorch❤️keras",
     long_description=README,
     install_requires=[           
-         'accelerate',
+         'accelerate>=0.20.3',
          'tqdm',
          #'torch',
          #'torchmetrics',
          #'plotly',
          #'wandb'
        ],
     long_description_content_type="text/markdown",
```

### Comparing `torchkeras-3.9.2/torchkeras/assets/SimHei.ttf` & `torchkeras-3.9.3/torchkeras/assets/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/assets/park.jpg` & `torchkeras-3.9.3/torchkeras/assets/park.jpg`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/assets/zidane.jpg` & `torchkeras-3.9.3/torchkeras/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/chat/chatglm.py` & `torchkeras-3.9.3/torchkeras/chat/chatglm.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/chat/chatgpt.py` & `torchkeras-3.9.3/torchkeras/chat/chatgpt.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/data.py` & `torchkeras-3.9.3/torchkeras/data.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/eda.py` & `torchkeras-3.9.3/torchkeras/eda.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/email.py` & `torchkeras-3.9.3/torchkeras/email.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/hugmodel.py` & `torchkeras-3.9.3/torchkeras/hugmodel.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/kerascallbacks.py` & `torchkeras-3.9.3/torchkeras/kerascallbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,25 +116,32 @@
         #save dfhistory
         dfhistory = pd.DataFrame(model.history)
         dfhistory.to_csv(os.path.join(self.wb.run.dir,'dfhistory.csv'),index=None) 
         
         #save ckpt
         if self.save_ckpt:
             arti_model = self.wb.Artifact('checkpoint', type='model')
-            arti_model.add_file(model.ckpt_path)
+            if os.path.isdir(model.ckpt_path):
+                arti_model.add_dir(model.ckpt_path)
+            else:
+                arti_model.add_file(model.ckpt_path)
             self.wb.log_artifact(arti_model)
 
         run_dir = self.wb.run.dir
         self.wb.finish()
 
         #local save
-        import shutil
-        shutil.copy(model.ckpt_path,os.path.join(run_dir,os.path.basename(model.ckpt_path)))
-    
-
+        try:
+            import shutil
+            copy_fn = shutil.copytree if os.path.isdir(model.ckpt_path) else shutil.copy
+            copy_fn(model.ckpt_path,os.path.join(run_dir,os.path.basename(model.ckpt_path)))
+        except Exception as err:
+            print(err)
+            
+            
 class VisProgress:
     def __init__(self):
         pass
         
     def on_fit_start(self,model: 'KerasModel'):
         from .pbar import ProgressBar
         self.progress = ProgressBar(range(model.epochs)) 
@@ -143,29 +150,31 @@
     def on_train_epoch_end(self,model:'KerasModel'):
         pass
     
     def on_validation_epoch_end(self, model:"KerasModel"):
         dfhistory = pd.DataFrame(model.history)
         self.progress.update(dfhistory['epoch'].iloc[-1])
 
-           
     def on_fit_end(self,  model:"KerasModel"):
         dfhistory = pd.DataFrame(model.history)
         if dfhistory['epoch'].max()<model.epochs:
-            self.progress.on_interrupt(msg='earlystopping')
+            self.progress.on_interrupt(msg='')
         self.progress.display=False
             
+            
 class VisMetric:
     def __init__(self,figsize = (6,4),
                  save_path='history.png'):
         self.figsize = (6,4)
         self.save_path = save_path
         self.in_jupyter = is_jupyter()
         
     def on_fit_start(self,model: 'KerasModel'):
+        if not self.in_jupyter:
+            print('\nView dynamic loss/metric plot: \n'+os.path.abspath(self.save_path))
         self.metric =  model.monitor.replace('val_','')
         dfhistory = pd.DataFrame(model.history)
         x_bounds = [0, min(10,model.epochs)]
         title = f'best {model.monitor} = ?'
         self.update_graph(model, title=title, x_bounds = x_bounds)
         
     def on_train_epoch_end(self,model:'KerasModel'):
@@ -189,15 +198,15 @@
         arr_scores = dfhistory[model.monitor]
         best_score = np.max(arr_scores) if model.mode=="max" else np.min(arr_scores)
         best_epoch = dfhistory.loc[arr_scores==best_score,'epoch'].tolist()[0]
         return (best_epoch, best_score)
         
     def get_title(self,  model:'KerasModel'):
         best_epoch,best_score = self.get_best_score(model)
-        title = f'best {model.monitor} = {best_score:.4f} (@epoch {best_epoch})'
+        title = f'best {model.monitor}={best_score:.4f} (@epoch {best_epoch})'
         return title
 
     def update_graph(self, model:'KerasModel', title=None, x_bounds=None, y_bounds=None):
         import matplotlib.pyplot as plt
         self.plt = plt
         if not hasattr(self, 'graph_fig'):
             self.graph_fig, self.graph_ax = plt.subplots(1, figsize=self.figsize)
@@ -221,28 +230,29 @@
         if self.metric in dfhistory.columns:
             metric_values = dfhistory[self.metric]
             self.graph_ax.plot(epochs, metric_values,'co-', label = self.metric,clip_on=False)
 
         self.graph_ax.set_xlabel("epoch")
         self.graph_ax.set_ylabel(self.metric)  
         if title:
-             self.graph_ax.set_title(title)
+            self.graph_ax.set_title(title)
+            if not self.in_jupyter and hasattr(model.EpochRunner,'progress'):
+                model.EpochRunner.progress.comment_tail = title
         if m1 in dfhistory.columns or m2 in dfhistory.columns or self.metric in dfhistory.columns:
             self.graph_ax.legend(loc='best')
             
         if len(epochs)>0:
             best_epoch, best_score = self.get_best_score(model)
             self.graph_ax.plot(best_epoch,best_score,'r*',markersize=15,clip_on=False)
 
         if x_bounds is not None: self.graph_ax.set_xlim(*x_bounds)
         if y_bounds is not None: self.graph_ax.set_ylim(*y_bounds)
         if self.in_jupyter:
             self.graph_out.update(self.graph_ax.figure)
-        else:
-            self.graph_fig.savefig(self.save_path)
+        self.graph_fig.savefig(self.save_path)
         self.plt.close();
         
 
 class VisDisplay:
     def __init__(self,display_fn,model=None,init_display=True,dis_period=1):
         from ipywidgets import Output 
         self.display_fn = display_fn
```

### Comparing `torchkeras-3.9.2/torchkeras/kerasmodel.py` & `torchkeras-3.9.3/torchkeras/kerasmodel.py`

 * *Files 9% similar despite different names*

```diff
@@ -113,81 +113,77 @@
         super().__init__()
         self.net,self.loss_fn,self.metrics_dict = net, loss_fn, torch.nn.ModuleDict(metrics_dict) 
         self.optimizer = optimizer if optimizer is not None else torch.optim.Adam(
             self.net.parameters(), lr=3e-4)
         self.lr_scheduler = lr_scheduler
         self.from_scratch = True
         
-    def save_ckpt(self, ckpt_path='checkpoint', accelerator= None):
+    def save_ckpt(self, ckpt_path=None, accelerator= None):
         accelerator = accelerator if accelerator is not None else self.accelerator
         net_dict = accelerator.get_state_dict(self.net)
-        accelerator.save(net_dict,ckpt_path)
+        accelerator.save(net_dict,ckpt_path if ckpt_path is not None else self.ckpt_path)
       
-    def load_ckpt(self, ckpt_path='checkpoint'):
-        self.net.load_state_dict(torch.load(ckpt_path,map_location='cpu'))
+    def load_ckpt(self, ckpt_path=None):
+        self.net.load_state_dict(
+            torch.load(ckpt_path if ckpt_path is not None else self.ckpt_path,
+            map_location='cpu'))
         self.from_scratch = False
 
     def forward(self, x):
         return self.net.forward(x)
     
     def fit(self, train_data, val_data=None, epochs=10, ckpt_path='checkpoint',
             patience=5, monitor="val_loss", mode="min", callbacks=None, 
             plot=True,  wandb=False, quiet=None, 
             mixed_precision='no', cpu=False, gradient_accumulation_steps=1):
         from torchkeras.utils import colorful,is_jupyter
-        
         self.__dict__.update(locals())
         self.accelerator = Accelerator(mixed_precision=mixed_precision,cpu=cpu,
             gradient_accumulation_steps=gradient_accumulation_steps)
         device = str(self.accelerator.device)
         device_type = '🐌'  if 'cpu' in device else ('⚡️' if 'cuda' in device else '🚀')
         self.accelerator.print(
             colorful("<<<<<< "+device_type +" "+ device +" is used >>>>>>"))
     
         self.net,self.loss_fn,self.metrics_dict,self.optimizer,self.lr_scheduler= self.accelerator.prepare(
             self.net,self.loss_fn,self.metrics_dict,self.optimizer,self.lr_scheduler)
         
         train_dataloader,val_dataloader = self.accelerator.prepare(train_data,val_data)
         train_dataloader.size = train_data.size if hasattr(train_data,'size') else len(train_data)
+        train_dataloader.size = min(train_dataloader.size,len(train_dataloader))
+        
         if val_data:
             val_dataloader.size = val_data.size if hasattr(val_data,'size') else len(val_data)
-        
+            val_dataloader.size = min(val_dataloader.size,len(val_dataloader))
         
         self.history = {}
         callbacks = callbacks if callbacks is not None else []
         
         if bool(plot):
-            if is_jupyter():
-                from torchkeras.kerascallbacks import VisProgress
-                callbacks = [VisProgress()]+callbacks
-            from torchkeras.kerascallbacks import VisMetric
-            callbacks = [VisMetric()]+callbacks
+            from torchkeras.kerascallbacks import VisProgress,VisMetric
+            callbacks = [VisMetric(),VisProgress()]+callbacks
             
         if wandb!=False:
             from torchkeras.kerascallbacks import WandbCallback
             project = wandb if isinstance(wandb,str) else 'torchkeras'
             callbacks.append(WandbCallback(project=project))
             
         self.callbacks = [self.accelerator.prepare(x) for x in callbacks]
         
         if self.accelerator.is_local_main_process:
             [cb.on_fit_start(model = self) for cb in self.callbacks if hasattr(cb,'on_fit_start')]
                 
         start_epoch = 1 if self.from_scratch else 0
         
-        if quiet is None:
-            if is_jupyter():
-                quiet = True
-            else:
-                quiet = False
+        if bool(plot) or quiet is None:
+            quiet = True
         
         quiet_fn = (lambda epoch:quiet) if isinstance(quiet,bool) else (
             (lambda epoch:epoch>quiet) if isinstance(quiet,int) else quiet)
         
-            
         for epoch in range(start_epoch,epochs+1):
             should_quiet = quiet_fn(epoch)
         
             if not should_quiet:
                 nowtime = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
                 self.accelerator.print("\n"+"=========="*8 + "%s"%nowtime)
                 self.accelerator.print("Epoch {0} / {1}".format(epoch, epochs)+"\n")
@@ -242,69 +238,50 @@
             if best_score_idx==len(arr_scores)-1 and self.accelerator.is_local_main_process:
                 self.save_ckpt(ckpt_path,accelerator = self.accelerator)
                 if not should_quiet:
                     self.accelerator.print(colorful("<<<<<< reach best {0} : {1} >>>>>>".format(
                         monitor,arr_scores[best_score_idx])))
 
             if len(arr_scores)-best_score_idx>patience:
-                self.accelerator.print(colorful(
-                    "<<<<<< {} without improvement in {} epoch,""early stopping >>>>>>"
-                ).format(monitor,patience))
-                break; 
+                break
                 
         if self.accelerator.is_local_main_process:   
             dfhistory = pd.DataFrame(self.history)
             [cb.on_fit_end(model = self) for cb in self.callbacks 
                  if hasattr(cb,'on_fit_end')]
+            if epoch<epochs:
+                self.accelerator.print(colorful(
+                        "<<<<<< {} without improvement in {} epoch,""early stopping >>>>>> \n"
+                    ).format(monitor,patience))
             self.net = self.accelerator.unwrap_model(self.net)
             self.net.cpu()
             self.load_ckpt(ckpt_path)
-            torch.save(dfhistory,'dfhistory.pt')
             return dfhistory
         
     def evaluate(self, val_data, quiet=False):
         accelerator = Accelerator() if not hasattr(self,'accelerator') else self.accelerator
         self.net,self.loss_fn,self.metrics_dict = accelerator.prepare(
             self.net,self.loss_fn,self.metrics_dict)
         val_data = accelerator.prepare(val_data)
         val_step_runner = self.StepRunner(net = self.net,stage="val",
                     loss_fn = self.loss_fn,metrics_dict=deepcopy(self.metrics_dict),
                     accelerator = accelerator)
         val_epoch_runner = self.EpochRunner(val_step_runner,quiet=quiet)
         with torch.no_grad():
             val_metrics = val_epoch_runner(val_data)
-        if accelerator.is_local_main_process:
-            torch.save(val_metrics,'val_metrics.pt')
         return val_metrics
     
     def fit_ddp(self,num_processes,train_data,
             val_data=None, epochs=10, ckpt_path='checkpoint',
             patience=5, monitor="val_loss", mode="min", callbacks=None, 
             plot=True, wandb=False, quiet=None, 
             mixed_precision='no', cpu=False, gradient_accumulation_steps=1
            ):
         from accelerate import notebook_launcher
-        train_size = train_data.size if hasattr(train_data,'size') else len(train_data)
-        train_data.size = train_size//num_processes
-        if val_data:
-            val_size = val_data.size if hasattr(val_data,'size') else len(val_data)
-            val_data.size = val_size//num_processes
-            
         args = (train_data,val_data,epochs,ckpt_path,patience,monitor,mode,
             callbacks,plot,wandb,quiet,mixed_precision,cpu,gradient_accumulation_steps)
         notebook_launcher(self.fit, args, num_processes=num_processes)
-        dfhistory = torch.load('dfhistory.pt')
-        
-        train_data.size = train_size 
-        if val_data:
-            val_data.size = val_size 
-        return dfhistory
     
     def evaluate_ddp(self, num_processes, val_data, quiet=False):
         from accelerate import notebook_launcher
-        val_size = val_data.size if hasattr(val_data,'size') else len(val_data)
-        val_data.size = val_size//num_processes
         args = (val_data,quiet)
-        notebook_launcher(self.evaluate, args, num_processes=num_processes)
-        val_metrics = torch.load('val_metrics.pt')
-        val_data.size = val_size
-        return val_metrics
+        notebook_launcher(self.evaluate, args, num_processes=num_processes)
```

### Comparing `torchkeras-3.9.2/torchkeras/metrics.py` & `torchkeras-3.9.3/torchkeras/metrics.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/models/resnet.py` & `torchkeras-3.9.3/torchkeras/models/resnet.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/models/ssd.py` & `torchkeras-3.9.3/torchkeras/models/ssd.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/models/unet.py` & `torchkeras-3.9.3/torchkeras/models/unet.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/pbar.py` & `torchkeras-3.9.3/torchkeras/pbar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 
 '''
 reference from https://github.com/fastai/fastprogress/
 '''
-import time
+import time,sys
 from IPython.display import clear_output, display, HTML
+from torchkeras.utils import is_jupyter
 
+from tqdm.utils import _term_move_up
+move_up = _term_move_up()
 
 def format_time(t):
     "Format `t` (in seconds) to (h):mm:ss"
     t = int(t)
     h,m,s = t//3600, (t//60)%60, t%60
     if h!= 0: return f'{h}:{m:02d}:{s:02d}'
     else:     return f'{m:02d}:{s:02d}'
@@ -46,64 +49,91 @@
       <progress {val} class='{bar_style}' max='{total}' style='width:300px; height:20px; vertical-align: middle;'></progress>
       {label}
       <br>
       {postfix}
     </div>
     """
 
+
+def text_progress_bar(value, total, label='', postfix='', interrupted=False):
+    bar_style = "🟦" if interrupted else "⬜️"  #"🟥","⬜️" "○", "*"'🟦''⬛️'
+    percentage = round(value / total * 20)
+    finished = "🟩" * (percentage)  #"🟩","●"
+    unfinished = bar_style * (20 - percentage)
+    bar = "\r{}{} {}".format(finished,unfinished,label)+" "*20+"\t"*50+f"{postfix}"+" "*20+"\t"*50
+    return bar
+
 class ProgressBar:
     update_every,first_its,lt = 0.2,5,'<'
-    def __init__(self, gen, total=None, 
-                 display=True, comment=''):
-        self.gen,self.comment = gen,comment
+    def __init__(self, gen, total=None, comment='', comment_tail=''):
+        self.gen,self.comment,self.comment_tail = gen,comment,comment_tail
         self.postfix = ''
         self.total = None if total=='noinfer' else len(gen) if total is None else total
         self.last_v = 0
-        self.display = display
         self.last_v = None
+        self.display = True
+        self.in_jupyter = is_jupyter()
         self.update(0)
         
+        
     def update(self, val):
         if self.last_v is None:
             self.on_iter_begin()
             self.last_v = 0
         if val == 0:
             self.start_t = self.last_t = time.time()
             self.pred_t,self.last_v,self.wait_for = None,0,1
             self.update_bar(0)
         elif val <= self.first_its or val >= self.last_v + self.wait_for or (self.total and val >= self.total):
             cur_t = time.time()
             avg_t = (cur_t - self.start_t) / val
             self.wait_for = max(int(self.update_every / (avg_t+1e-8)),1)
             self.pred_t = None if self.total is None else avg_t * self.total
             self.last_v,self.last_t = val,cur_t
-            self.update_bar(val)
             if self.total is not None and val >= self.total:
                 self.on_iter_end()
-                self.last_v = None
+                self.last_v = self.total
+            else:
+                self.update_bar(val)
                 
     def on_iter_begin(self):
-        self.html_code = '\n'.join([html_progress_bar(0, self.total, ""), ""])
-        display(HTML(html_progress_bar_styles))
-        self.out = display(HTML(self.html_code), display_id=True)
+        if self.in_jupyter:
+            self.html_code = '\n'.join([html_progress_bar(0, self.total, ""), ""])
+            display(HTML(html_progress_bar_styles))
+            self.out = display(HTML(self.html_code), display_id=True)
+        else:
+            print('\n')
 
     def on_iter_end(self):
         total_time = format_time(time.time() - self.start_t)
-        self.comment = f'[{total_time}]' 
-        if hasattr(self, 'out'): 
-            self.on_update(self.total,self.comment,self.postfix)
-
-    def on_update(self, val, comment='', postfix='', interrupted=False): 
-        self.progress = html_progress_bar(val, self.total,comment,postfix,interrupted)
-        if self.display: 
-            self.out.update(HTML(self.progress))
-            
+        self.comment = f'100% [{self.total}/{self.total}] [{total_time}]'   
+        self.on_update(self.total,self.comment,self.postfix,False,1)
+        self.display = False
+        if not self.in_jupyter:
+            print('\n')
+
+    def on_update(self, val, comment='', postfix='', interrupted=False, up=1): 
+        if not self.display:
+            return 
+        if self.in_jupyter:
+                self.progress = html_progress_bar(val,self.total,comment,postfix,interrupted)
+                self.out.update(HTML(self.progress))
+        else:
+            if self.comment_tail:
+                comment = comment+f' [{self.comment_tail}]'
+            progress = text_progress_bar(val, self.total, comment, postfix, interrupted)
+            print(move_up*up+progress,end='')
+                
     def on_interrupt(self,msg='interrupted'):
-        self.on_update(self.last_v,self.comment+f'[{msg}]',interrupted=True)
-
+        comment = self.comment+f' [{msg}]' if msg else self.comment
+        self.on_update(self.last_v,comment,self.postfix,interrupted=True,up=1)
+        self.display = False
+        if not self.in_jupyter:
+            print('\n')
+        
     def __iter__(self):
         if self.total != 0: self.update(0)
         try:
             for i,o in enumerate(self.gen):
                 if self.total and i >= self.total: break
                 yield o
                 self.update(i+1)
@@ -117,36 +147,38 @@
     def update_bar(self, val):
         if self.total == 0:
             warn("Your generator is empty.")
             return self.on_update(0, '100% [0/0]')
         if val ==0:
             self.comment = f'0% [0/{self.total}]'
             return self.on_update(0, self.comment)
-        pct = '' if self.total is None else f'{100 * val/self.total:.2f}% '
+        pct = '' if self.total is None else f'{100 * val/self.total:.2f}%'
         tot = '?' if self.total is None else str(self.total)
         elapsed_t = self.last_t - self.start_t
         remaining_t = '?' if self.pred_t is None else format_time(self.pred_t - elapsed_t)
         elapsed_t = format_time(elapsed_t)
-        self.comment = f'{pct}[{val}/{tot} {elapsed_t}{self.lt}{remaining_t}]'
+        self.comment = f'{pct} [{val}/{tot}] [{elapsed_t}{self.lt}{remaining_t}]'
         self.on_update(val, self.comment, self.postfix)
     
     def set_postfix(self,**kwargs):
+        if not self.display:
+            return 
         postfix = ''
         if 'i' in kwargs and 'n' in kwargs:
             from tqdm.std import Bar 
             i,n = kwargs['i'],kwargs['n']
             kwargs.pop('i')
             kwargs.pop('n')
             ratio = i/n
             postfix+=format(Bar(ratio,default_len=20))
             postfix+=f'{100 * i/n:.2f}%'
-            postfix+=f' [{i}/{n}] '
+            postfix+=f' [{i}/{n}]'
         if kwargs:
-            postfix+='['
+            postfix+=' ['
             for i,(key,value) in enumerate(kwargs.items()):
                 if isinstance(value,float):
-                    postfix = postfix+f'{key}={format_number(value)},'
+                    postfix = postfix+f'{key}={format_number(value)}, '
                 else:
-                    postfix = postfix+f'{key}={value},'
-            postfix = postfix[:-1]+']'
+                    postfix = postfix+f'{key}={value}, '
+            postfix = postfix[:-2]+']'
         self.postfix = postfix
         self.on_update(self.last_v,self.comment,self.postfix)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchkeras-3.9.2/torchkeras/plots.py` & `torchkeras-3.9.3/torchkeras/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 import PIL
 from PIL import Image,ImageDraw,ImageFont
 from pathlib import Path
 import sys 
 
 simhei_file = str(Path(__file__).parent/"assets/SimHei.ttf")
 
-
 def set_matplotlib_font(font_size=15):
     import matplotlib as mpl
     import matplotlib.pyplot as plt
-    import shutil
-    shutil.rmtree(mpl.get_cachedir())
+    try:
+        import shutil
+        shutil.rmtree(mpl.get_cachedir())
+    except:
+        pass
     simhei_file = Path(__file__).parent/"assets/SimHei.ttf"
     ttf_dir = Path(mpl.__path__[0])/'mpl-data'/'fonts'/'ttf'
     shutil.copy(str(simhei_file),str(ttf_dir))
     plt.rcParams['font.family'] = ['sans-serif']
     plt.rcParams['font.size'] = str(font_size)
     plt.rcParams['font.sans-serif'] = ['SimHei']
     plt.rcParams['axes.unicode_minus'] = False
```

### Comparing `torchkeras-3.9.2/torchkeras/soup.py` & `torchkeras-3.9.3/torchkeras/soup.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/summary.py` & `torchkeras-3.9.3/torchkeras/summary.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/tools/catboost.py` & `torchkeras-3.9.3/torchkeras/tools/catboost.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras/utils.py` & `torchkeras-3.9.3/torchkeras/utils.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.2/torchkeras.egg-info/PKG-INFO` & `torchkeras-3.9.3/torchkeras.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchkeras
-Version: 3.9.2
+Version: 3.9.3
 Summary: pytorch❤️keras
 Home-page: https://github.com/lyhue1991/torchkeras
 Author: PythonAiRoad, Laugh
 Author-email: lyhue1991@163.com
 Keywords: machine-learning,deep-learning,ML,DL,pytorch,torch,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -134,17 +134,17 @@
 |ObjectDetection——FasterRCNN| torchvision  |  [FasterRCNN](./examples/FasterRCNN——vision.ipynb) | 
 |ImageSegmentation——DeepLabV3++ | segmentation_models_pytorch |  [Deeplabv3++](./examples/Deeplabv3plus——smp.ipynb) |
 |InstanceSegmentation——MaskRCNN | detectron2 |  [MaskRCNN](./examples/MaskRCNN——detectron2.ipynb) |
 |ObjectDetection——YOLOv8 🔥🔥| ultralytics |  [YOLOv8](./examples/YOLOv8——ultralytics.ipynb) |
 |ImageClassification——SwinTransformer|timm| [Swin](./examples/SwinTransformer——timm.ipynb)|
 ||||
 |**NLP**|||
-|TextClassification——BERT 🔥🔥| transformers |  [BERT](./examples/BERT——transformers.ipynb) |
+|Seq2Seq——Transformer🔥🔥| - |  [Transformer](./examples/Dive_into_Transformer.ipynb) |
+|TextClassification——BERT | transformers |  [BERT](./examples/BERT——transformers.ipynb) |
 |TokenClassification——BERT | transformers |  [BERT_NER](./examples/BERT_NER——transformers.ipynb) |
-|FinetuneLLM——ChatGLM2 🔥🔥🔥| transformers |  [ChatGLM2](./examples/ChatGLM2——transformers.ipynb) |
 |FinetuneLLM——ChatGLM2_LoRA 🔥🔥🔥| transformers,peft |  [ChatGLM2_LoRA](./examples/ChatGLM2_LoRA——transformers.ipynb) |
 |FinetuneLLM——ChatGLM2_AdaLoRA 🔥🔥🔥| transformers,peft |  [ChatGLM2_AdaLoRA](./examples/ChatGLM2_AdaLoRA——transformers.ipynb) |
 |FinetuneLLM——ChatGLM2_QLoRA 🔥🔥🔥| transformers |  [ChatGLM2_QLoRA_Kaggle](./examples/ChatGLM2_QLoRA_Kaggle——transformers.ipynb) |
 |FinetuneLLM——BaiChuan13B_QLoRA 🔥🔥🔥| transformers |  [BaiChuan13B_QLoRA](./examples/BaiChuan13B_QLoRA——transformers.ipynb) |
 |FinetuneLLM——BaiChuan13B_NER 🔥🔥🔥| transformers |  [BaiChuan13B_NER](./examples/BaiChuan13B_NER——transformers.ipynb) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchkeras Version: 3.9.2 Summary:
+Metadata-Version: 2.1 Name: torchkeras Version: 3.9.3 Summary:
 pytorchâ¤ï¸keras Home-page: https://github.com/lyhue1991/torchkeras Author:
 PythonAiRoad, Laugh Author-email: lyhue1991@163.com Keywords: machine-
 learning,deep-learning,ML,DL,pytorch,torch,keras Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE #
 Pytorchâ¤ï¸Keras English | [ç®ä½ä¸­æ](README.md) The torchkeras library
@@ -67,19 +67,19 @@
 | segmentation_models_pytorch | [Deeplabv3++](./examples/
 Deeplabv3plusââsmp.ipynb) | |InstanceSegmentationââMaskRCNN |
 detectron2 | [MaskRCNN](./examples/MaskRCNNââdetectron2.ipynb) |
 |ObjectDetectionââYOLOv8 ð¥ð¥| ultralytics | [YOLOv8](./examples/
 YOLOv8ââultralytics.ipynb) |
 |ImageClassificationââSwinTransformer|timm| [Swin](./examples/
 SwinTransformerââtimm.ipynb)| |||| |**NLP**|||
-|TextClassificationââBERT ð¥ð¥| transformers | [BERT](./examples/
-BERTââtransformers.ipynb) | |TokenClassificationââBERT | transformers |
-[BERT_NER](./examples/BERT_NERââtransformers.ipynb) |
-|FinetuneLLMââChatGLM2 ð¥ð¥ð¥| transformers | [ChatGLM2](./examples/
-ChatGLM2ââtransformers.ipynb) | |FinetuneLLMââChatGLM2_LoRA
+|Seq2SeqââTransformerð¥ð¥| - | [Transformer](./examples/
+Dive_into_Transformer.ipynb) | |TextClassificationââBERT | transformers |
+[BERT](./examples/BERTââtransformers.ipynb) |
+|TokenClassificationââBERT | transformers | [BERT_NER](./examples/
+BERT_NERââtransformers.ipynb) | |FinetuneLLMââChatGLM2_LoRA
 ð¥ð¥ð¥| transformers,peft | [ChatGLM2_LoRA](./examples/
 ChatGLM2_LoRAââtransformers.ipynb) | |FinetuneLLMââChatGLM2_AdaLoRA
 ð¥ð¥ð¥| transformers,peft | [ChatGLM2_AdaLoRA](./examples/
 ChatGLM2_AdaLoRAââtransformers.ipynb) | |FinetuneLLMââChatGLM2_QLoRA
 ð¥ð¥ð¥| transformers | [ChatGLM2_QLoRA_Kaggle](./examples/
 ChatGLM2_QLoRA_Kaggleââtransformers.ipynb) |
 |FinetuneLLMââBaiChuan13B_QLoRA ð¥ð¥ð¥| transformers |
```

### Comparing `torchkeras-3.9.2/torchkeras.egg-info/SOURCES.txt` & `torchkeras-3.9.3/torchkeras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

