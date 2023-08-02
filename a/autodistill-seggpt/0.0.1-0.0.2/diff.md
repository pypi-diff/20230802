# Comparing `tmp/autodistill-seggpt-0.0.1.tar.gz` & `tmp/autodistill-seggpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autodistill-seggpt-0.0.1.tar", last modified: Tue Aug  1 23:02:14 2023, max compression
+gzip compressed data, was "dist/autodistill-seggpt-0.0.2.tar", last modified: Wed Aug  2 08:45:36 2023, max compression
```

## Comparing `autodistill-seggpt-0.0.1.tar` & `autodistill-seggpt-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 andrewhealey  (1005) andrewhealey  (1006)        0 2023-08-01 23:02:14.000000 autodistill-seggpt-0.0.1/
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     3657 2023-08-01 23:02:14.000000 autodistill-seggpt-0.0.1/PKG-INFO
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     3206 2023-08-01 22:30:52.000000 autodistill-seggpt-0.0.1/README.md
-drwxr-xr-x   0 andrewhealey  (1005) andrewhealey  (1006)        0 2023-08-01 23:02:14.000000 autodistill-seggpt-0.0.1/autodistill_seggpt/
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)      231 2023-08-01 22:55:29.000000 autodistill-seggpt-0.0.1/autodistill_seggpt/__init__.py
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)      666 2023-08-01 17:33:34.000000 autodistill-seggpt-0.0.1/autodistill_seggpt/colors.py
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     3264 2023-08-01 22:55:29.000000 autodistill-seggpt-0.0.1/autodistill_seggpt/dataset_utils.py
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     5130 2023-08-01 22:55:28.000000 autodistill-seggpt-0.0.1/autodistill_seggpt/few_shot_ontology.py
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     4616 2023-08-01 22:55:29.000000 autodistill-seggpt-0.0.1/autodistill_seggpt/find_best_examples.py
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     2911 2023-08-01 02:18:53.000000 autodistill-seggpt-0.0.1/autodistill_seggpt/metrics.py
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     1866 2023-08-01 22:55:28.000000 autodistill-seggpt-0.0.1/autodistill_seggpt/postprocessing.py
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     4214 2023-08-01 22:55:29.000000 autodistill-seggpt-0.0.1/autodistill_seggpt/sam_refine.py
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     8939 2023-08-01 22:55:29.000000 autodistill-seggpt-0.0.1/autodistill_seggpt/seggpt.py
-drwxr-xr-x   0 andrewhealey  (1005) andrewhealey  (1006)        0 2023-08-01 23:02:14.000000 autodistill-seggpt-0.0.1/autodistill_seggpt.egg-info/
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     3657 2023-08-01 23:02:14.000000 autodistill-seggpt-0.0.1/autodistill_seggpt.egg-info/PKG-INFO
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)      533 2023-08-01 23:02:14.000000 autodistill-seggpt-0.0.1/autodistill_seggpt.egg-info/SOURCES.txt
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)       55 2023-08-01 23:02:14.000000 autodistill-seggpt-0.0.1/autodistill_seggpt.egg-info/dependency_links.txt
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)      173 2023-08-01 23:02:14.000000 autodistill-seggpt-0.0.1/autodistill_seggpt.egg-info/requires.txt
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)       19 2023-08-01 23:02:14.000000 autodistill-seggpt-0.0.1/autodistill_seggpt.egg-info/top_level.txt
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)       38 2023-08-01 23:02:14.000000 autodistill-seggpt-0.0.1/setup.cfg
--rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     1392 2023-08-01 21:56:38.000000 autodistill-seggpt-0.0.1/setup.py
+drwxr-xr-x   0 andrewhealey  (1005) andrewhealey  (1006)        0 2023-08-02 08:45:36.000000 autodistill-seggpt-0.0.2/
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     3679 2023-08-02 08:45:36.000000 autodistill-seggpt-0.0.2/PKG-INFO
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     3229 2023-08-02 07:59:40.000000 autodistill-seggpt-0.0.2/README.md
+drwxr-xr-x   0 andrewhealey  (1005) andrewhealey  (1006)        0 2023-08-02 08:45:36.000000 autodistill-seggpt-0.0.2/autodistill_seggpt/
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)      231 2023-08-02 08:44:11.000000 autodistill-seggpt-0.0.2/autodistill_seggpt/__init__.py
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)      666 2023-08-01 17:33:34.000000 autodistill-seggpt-0.0.2/autodistill_seggpt/colors.py
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     3264 2023-08-01 22:55:29.000000 autodistill-seggpt-0.0.2/autodistill_seggpt/dataset_utils.py
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     5392 2023-08-02 08:39:51.000000 autodistill-seggpt-0.0.2/autodistill_seggpt/few_shot_ontology.py
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     4795 2023-08-02 08:40:55.000000 autodistill-seggpt-0.0.2/autodistill_seggpt/find_best_examples.py
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     2911 2023-08-01 02:18:53.000000 autodistill-seggpt-0.0.2/autodistill_seggpt/metrics.py
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     1866 2023-08-01 22:55:28.000000 autodistill-seggpt-0.0.2/autodistill_seggpt/postprocessing.py
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     4214 2023-08-01 22:55:29.000000 autodistill-seggpt-0.0.2/autodistill_seggpt/sam_refine.py
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     8939 2023-08-01 22:55:29.000000 autodistill-seggpt-0.0.2/autodistill_seggpt/seggpt.py
+drwxr-xr-x   0 andrewhealey  (1005) andrewhealey  (1006)        0 2023-08-02 08:45:36.000000 autodistill-seggpt-0.0.2/autodistill_seggpt.egg-info/
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     3679 2023-08-02 08:45:36.000000 autodistill-seggpt-0.0.2/autodistill_seggpt.egg-info/PKG-INFO
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)      533 2023-08-02 08:45:36.000000 autodistill-seggpt-0.0.2/autodistill_seggpt.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)       55 2023-08-02 08:45:36.000000 autodistill-seggpt-0.0.2/autodistill_seggpt.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)      173 2023-08-02 08:45:36.000000 autodistill-seggpt-0.0.2/autodistill_seggpt.egg-info/requires.txt
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)       19 2023-08-02 08:45:36.000000 autodistill-seggpt-0.0.2/autodistill_seggpt.egg-info/top_level.txt
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)       38 2023-08-02 08:45:36.000000 autodistill-seggpt-0.0.2/setup.cfg
+-rw-r--r--   0 andrewhealey  (1005) andrewhealey  (1006)     1392 2023-08-01 21:56:38.000000 autodistill-seggpt-0.0.2/setup.py
```

### Comparing `autodistill-seggpt-0.0.1/PKG-INFO` & `autodistill-seggpt-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill-seggpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: SegGPT for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-seggpt
 Author: andrew-healey
 Author-email: andrew@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -86,15 +86,16 @@
 To import your dataset into Autodistill, run the following:
 
 ```py
 import supervision as sv
 supervision_dataset = sv.DetectionDataset.from_yolo(
     images_directory_path=f"{dataset.location}/train/images",
     annotations_directory_path=f"{dataset.location}/train/labels",
-    data_yaml_path=f"{dataset.location}/data.yaml"
+    data_yaml_path=f"{dataset.location}/data.yaml",
+    force_masks=True
 )
 ```
 
 ## License
 
 The code in this repository is licensed under an [MIT license](LICENSE).
```

### Comparing `autodistill-seggpt-0.0.1/README.md` & `autodistill-seggpt-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,20 +72,21 @@
 To import your dataset into Autodistill, run the following:
 
 ```py
 import supervision as sv
 supervision_dataset = sv.DetectionDataset.from_yolo(
     images_directory_path=f"{dataset.location}/train/images",
     annotations_directory_path=f"{dataset.location}/train/labels",
-    data_yaml_path=f"{dataset.location}/data.yaml"
+    data_yaml_path=f"{dataset.location}/data.yaml",
+    force_masks=True
 )
 ```
 
 ## License
 
 The code in this repository is licensed under an [MIT license](LICENSE).
 
 See the SegGPT repository for more information on the [SegGPT license](https://github.com/baaivision/Painter/tree/main).
 
 ## 🏆 Contributing
 
-We love your input! Please see the core Autodistill [contributing guide](https://github.com/autodistill/autodistill/blob/main/CONTRIBUTING.md) to get started. Thank you 🙏 to all our contributors!
+We love your input! Please see the core Autodistill [contributing guide](https://github.com/autodistill/autodistill/blob/main/CONTRIBUTING.md) to get started. Thank you 🙏 to all our contributors!
```

### Comparing `autodistill-seggpt-0.0.1/autodistill_seggpt/colors.py` & `autodistill-seggpt-0.0.2/autodistill_seggpt/colors.py`

 * *Files identical despite different names*

### Comparing `autodistill-seggpt-0.0.1/autodistill_seggpt/dataset_utils.py` & `autodistill-seggpt-0.0.2/autodistill_seggpt/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `autodistill-seggpt-0.0.1/autodistill_seggpt/few_shot_ontology.py` & `autodistill-seggpt-0.0.2/autodistill_seggpt/few_shot_ontology.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 from supervision import Detections
 from supervision.dataset.core import DetectionDataset
 
 # TODO turn FewShotOntology into a thin wrapper around DetectionDataset
 # move the searching/etc. logic into find_best_examples.
 # Maybe also try to make nice/quick serialization for shareability.
 
+def default_model(ontology: FewShotOntology) -> DetectionBaseModel:
+    from .seggpt import SegGPT
+
+    return SegGPT(
+        ontology=ontology,
+        refine_detections=False, # disable this since we don't use SAM feature map caching (or MobileSAM) yet. So SAM slows us down big-time.
+    )
 
 @dataclass
 class FewShotOntology(DetectionOntology):
     def __init__(
         self,
         ref_dataset: DetectionDataset,
         # each tuple in the list has form:
@@ -46,17 +53,16 @@
                 {
                     f"{i}-{cls_name}": cls_name
                     for cls_name, i in class_name_to_id.items()
                 }
             )
 
             from .find_best_examples import find_best_examples
-            from .seggpt import SegGPT
 
-            best_examples = find_best_examples(ref_dataset, SegGPT)
+            best_examples = find_best_examples(ref_dataset, default_model)
             print("best_examples", best_examples)
             ontology = FewShotOntology.examples_to_tuples(ontology, best_examples)
 
         self.ontology = ontology
         rich_ontology = self.enrich_ontology(ontology)
         self.rich_ontology = rich_ontology
```

### Comparing `autodistill-seggpt-0.0.1/autodistill_seggpt/find_best_examples.py` & `autodistill-seggpt-0.0.2/autodistill_seggpt/find_best_examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Given a dataset of a few images, find the best training examples from it.
 # An ontology has k example images for each class.
 # Try a bunch of random k-example-image-sets for each class, then pick the one which generalizes best to the rest of the images.
 # Then combine those best-performing k-example-image-sets into a single ontology.
 import math
 from random import sample
-from typing import List, Type, Union
+from typing import List, Type, Union, Callable
 
 import numpy as np
 import supervision as sv
 from autodistill.detection import CaptionOntology, DetectionBaseModel
 from supervision.dataset.core import DetectionDataset
 from tqdm import tqdm
 
@@ -46,15 +46,15 @@
             cls_name = cls_names[i]
             examples[cls_name].append(img_name)
     return examples
 
 
 def find_best_examples(
     ref_dataset: DetectionDataset,
-    model_class: Type[DetectionBaseModel],
+    model_class: Callable[[FewShotOntology], DetectionBaseModel],
     num_examples: int = 2,
     num_trials: int = 5,
     max_test_imgs: int = 10,
     which_metric: Union[str, Metric] = "iou",
 ):
     best_examples = {}
 
@@ -79,36 +79,36 @@
 
         # TODO use CLIP to find a small AND diverse valid set.
         gt_dataset = shrink_dataset_to_size(gt_dataset, max_test_imgs)
 
         if len(positive_examples) == 0:
             best_examples[cls_deduped] = []
             continue
+        
+        curr_num_examples = min(num_examples, len(positive_examples))
 
-        num_combos = choose(len(positive_examples), num_examples)
+        num_combos = choose(len(positive_examples), curr_num_examples)
 
         num_iters = min(num_combos, num_trials)
         combo_hashes = range(num_combos)
         sub_combo_hashes = sample(combo_hashes, num_iters)
 
         print(f"Finding best examples for class {cls_deduped}.")
 
         combo_pbar = tqdm(sub_combo_hashes)
         max_score = -math.inf
 
         for combo_hash in combo_pbar:
             image_choices = combo_hash_to_choices(
-                combo_hash, positive_examples, num_examples
+                combo_hash, positive_examples, curr_num_examples
             )
             onto_tuples = [((cls_deduped, image_choices), cls)]
 
             ontology = FewShotOntology(ref_dataset, onto_tuples)
-            model = model_class(
-                ontology
-            )  # model must take only an Ontology as a parameter
+            model = model_class(ontology)  # model must take only an Ontology as a parameter
             pred_dataset = label_dataset(gt_dataset, model)
             score = metric(gt_dataset, pred_dataset).tolist()
 
             examples_scores.append((image_choices, score))
             max_or_min = max if metric_direction == 1 else min
             max_score = max_or_min(max_score, score)
             combo_pbar.set_description(f"Best {metric_name}: {round(max_score,2)}")
@@ -117,17 +117,19 @@
         best_examples[cls_deduped] = my_best_examples
     return best_examples
 
 
 def combo_hash_to_choices(
     fact: int, candidates: List[any], num_choices: int
 ) -> List[any]:
+    assert len(candidates) >= num_choices, "Not enough candidates to choose from."
+
     chosen = []
     curr_fact = fact
-    remaining_candidates = candidates
+    remaining_candidates = [*candidates]
     for i in range(num_choices, 0, -1):
         which_remaining_candidate = curr_fact % i
         chosen.append(remaining_candidates.pop(which_remaining_candidate))
         curr_fact = curr_fact // i
     return chosen
```

### Comparing `autodistill-seggpt-0.0.1/autodistill_seggpt/metrics.py` & `autodistill-seggpt-0.0.2/autodistill_seggpt/metrics.py`

 * *Files identical despite different names*

### Comparing `autodistill-seggpt-0.0.1/autodistill_seggpt/postprocessing.py` & `autodistill-seggpt-0.0.2/autodistill_seggpt/postprocessing.py`

 * *Files identical despite different names*

### Comparing `autodistill-seggpt-0.0.1/autodistill_seggpt/sam_refine.py` & `autodistill-seggpt-0.0.2/autodistill_seggpt/sam_refine.py`

 * *Files identical despite different names*

### Comparing `autodistill-seggpt-0.0.1/autodistill_seggpt/seggpt.py` & `autodistill-seggpt-0.0.2/autodistill_seggpt/seggpt.py`

 * *Files identical despite different names*

### Comparing `autodistill-seggpt-0.0.1/autodistill_seggpt.egg-info/PKG-INFO` & `autodistill-seggpt-0.0.2/autodistill_seggpt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill-seggpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: SegGPT for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-seggpt
 Author: andrew-healey
 Author-email: andrew@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -86,15 +86,16 @@
 To import your dataset into Autodistill, run the following:
 
 ```py
 import supervision as sv
 supervision_dataset = sv.DetectionDataset.from_yolo(
     images_directory_path=f"{dataset.location}/train/images",
     annotations_directory_path=f"{dataset.location}/train/labels",
-    data_yaml_path=f"{dataset.location}/data.yaml"
+    data_yaml_path=f"{dataset.location}/data.yaml",
+    force_masks=True
 )
 ```
 
 ## License
 
 The code in this repository is licensed under an [MIT license](LICENSE).
```

### Comparing `autodistill-seggpt-0.0.1/autodistill_seggpt.egg-info/SOURCES.txt` & `autodistill-seggpt-0.0.2/autodistill_seggpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autodistill-seggpt-0.0.1/setup.py` & `autodistill-seggpt-0.0.2/setup.py`

 * *Files identical despite different names*

