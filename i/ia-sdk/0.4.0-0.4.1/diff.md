# Comparing `tmp/ia-sdk-0.4.0.tar.gz` & `tmp/ia-sdk-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia-sdk-0.4.0.tar", last modified: Tue Aug  1 21:00:01 2023, max compression
+gzip compressed data, was "ia-sdk-0.4.1.tar", last modified: Wed Aug  2 12:28:06 2023, max compression
```

## Comparing `ia-sdk-0.4.0.tar` & `ia-sdk-0.4.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1256 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/PKG-INFO
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      751 2023-02-02 14:25:09.000000 ia-sdk-0.4.0/README.md
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       22 2023-08-01 17:28:22.000000 ia-sdk-0.4.0/ia/__init__.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia/gaius/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       79 2022-05-26 13:05:31.000000 ia-sdk-0.4.0/ia/gaius/__init__.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    75273 2023-08-01 15:18:51.000000 ia-sdk-0.4.0/ia/gaius/agent_client.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    22819 2023-05-08 22:12:27.000000 ia-sdk-0.4.0/ia/gaius/back_testing.py
--rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    12451 2023-07-25 14:50:28.000000 ia-sdk-0.4.0/ia/gaius/comcom_client.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      858 2023-04-14 14:57:27.000000 ia-sdk-0.4.0/ia/gaius/data_language.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     9361 2023-08-01 19:37:22.000000 ia-sdk-0.4.0/ia/gaius/data_ops.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    17348 2023-07-19 12:51:12.000000 ia-sdk-0.4.0/ia/gaius/data_structures.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia/gaius/experimental/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2023-07-14 15:07:29.000000 ia-sdk-0.4.0/ia/gaius/experimental/__init__.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    11085 2023-07-14 15:07:29.000000 ia-sdk-0.4.0/ia/gaius/experimental/genome_optimizer.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     3217 2023-06-08 15:56:58.000000 ia-sdk-0.4.0/ia/gaius/genome_info.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    27195 2023-08-01 15:18:51.000000 ia-sdk-0.4.0/ia/gaius/kb_ops.py
--rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    36330 2023-07-25 14:03:17.000000 ia-sdk-0.4.0/ia/gaius/manager.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     8771 2023-06-08 15:56:58.000000 ia-sdk-0.4.0/ia/gaius/prediction_models.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia/gaius/pvt/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    76162 2023-08-01 20:44:52.000000 ia-sdk-0.4.0/ia/gaius/pvt/__init__.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    26516 2023-08-01 19:14:20.000000 ia-sdk-0.4.0/ia/gaius/pvt/mongo_interface.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    10707 2023-08-01 15:18:46.000000 ia-sdk-0.4.0/ia/gaius/pvt/offline_sio.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    17596 2023-08-01 18:42:47.000000 ia-sdk-0.4.0/ia/gaius/pvt/pvt_utils.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia/gaius/tests/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2022-05-26 13:05:31.000000 ia-sdk-0.4.0/ia/gaius/tests/__init__.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2786 2023-06-08 15:56:58.000000 ia-sdk-0.4.0/ia/gaius/tests/classification.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2679 2023-06-08 15:56:58.000000 ia-sdk-0.4.0/ia/gaius/tests/utility.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    11002 2023-06-08 15:56:58.000000 ia-sdk-0.4.0/ia/gaius/utils.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia/scripts/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2023-03-24 19:12:06.000000 ia-sdk-0.4.0/ia/scripts/__init__.py
--rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    40560 2023-08-01 17:33:50.000000 ia-sdk-0.4.0/ia/scripts/spawn_agent.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2762 2023-07-25 13:21:37.000000 ia-sdk-0.4.0/ia/scripts/spawn_general.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia_sdk.egg-info/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1256 2023-08-01 21:00:01.000000 ia-sdk-0.4.0/ia_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      825 2023-08-01 21:00:01.000000 ia-sdk-0.4.0/ia_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        1 2023-08-01 21:00:01.000000 ia-sdk-0.4.0/ia_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      139 2023-08-01 21:00:01.000000 ia-sdk-0.4.0/ia_sdk.egg-info/requires.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        3 2023-08-01 21:00:01.000000 ia-sdk-0.4.0/ia_sdk.egg-info/top_level.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      110 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/setup.cfg
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1176 2023-07-18 13:37:42.000000 ia-sdk-0.4.0/setup.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1256 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/PKG-INFO
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      751 2023-02-02 14:25:09.000000 ia-sdk-0.4.1/README.md
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       22 2023-08-02 12:25:48.000000 ia-sdk-0.4.1/ia/__init__.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia/gaius/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       79 2022-05-26 13:05:31.000000 ia-sdk-0.4.1/ia/gaius/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    75273 2023-08-01 15:18:51.000000 ia-sdk-0.4.1/ia/gaius/agent_client.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    22819 2023-05-08 22:12:27.000000 ia-sdk-0.4.1/ia/gaius/back_testing.py
+-rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    12451 2023-07-25 14:50:28.000000 ia-sdk-0.4.1/ia/gaius/comcom_client.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      858 2023-04-14 14:57:27.000000 ia-sdk-0.4.1/ia/gaius/data_language.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     9361 2023-08-01 19:37:22.000000 ia-sdk-0.4.1/ia/gaius/data_ops.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    17348 2023-07-19 12:51:12.000000 ia-sdk-0.4.1/ia/gaius/data_structures.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia/gaius/experimental/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2023-07-14 15:07:29.000000 ia-sdk-0.4.1/ia/gaius/experimental/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    11085 2023-07-14 15:07:29.000000 ia-sdk-0.4.1/ia/gaius/experimental/genome_optimizer.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     3217 2023-06-08 15:56:58.000000 ia-sdk-0.4.1/ia/gaius/genome_info.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    27195 2023-08-01 15:18:51.000000 ia-sdk-0.4.1/ia/gaius/kb_ops.py
+-rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    36330 2023-07-25 14:03:17.000000 ia-sdk-0.4.1/ia/gaius/manager.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     8771 2023-06-08 15:56:58.000000 ia-sdk-0.4.1/ia/gaius/prediction_models.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia/gaius/pvt/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    76162 2023-08-01 20:44:52.000000 ia-sdk-0.4.1/ia/gaius/pvt/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    26516 2023-08-01 19:14:20.000000 ia-sdk-0.4.1/ia/gaius/pvt/mongo_interface.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    10707 2023-08-01 15:18:46.000000 ia-sdk-0.4.1/ia/gaius/pvt/offline_sio.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    17775 2023-08-01 21:14:21.000000 ia-sdk-0.4.1/ia/gaius/pvt/pvt_utils.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia/gaius/tests/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2022-05-26 13:05:31.000000 ia-sdk-0.4.1/ia/gaius/tests/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2786 2023-06-08 15:56:58.000000 ia-sdk-0.4.1/ia/gaius/tests/classification.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2679 2023-06-08 15:56:58.000000 ia-sdk-0.4.1/ia/gaius/tests/utility.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    11002 2023-06-08 15:56:58.000000 ia-sdk-0.4.1/ia/gaius/utils.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia/scripts/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2023-03-24 19:12:06.000000 ia-sdk-0.4.1/ia/scripts/__init__.py
+-rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    40560 2023-08-01 17:33:50.000000 ia-sdk-0.4.1/ia/scripts/spawn_agent.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2762 2023-07-25 13:21:37.000000 ia-sdk-0.4.1/ia/scripts/spawn_general.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia_sdk.egg-info/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1256 2023-08-02 12:28:06.000000 ia-sdk-0.4.1/ia_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      825 2023-08-02 12:28:06.000000 ia-sdk-0.4.1/ia_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        1 2023-08-02 12:28:06.000000 ia-sdk-0.4.1/ia_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      139 2023-08-02 12:28:06.000000 ia-sdk-0.4.1/ia_sdk.egg-info/requires.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        3 2023-08-02 12:28:06.000000 ia-sdk-0.4.1/ia_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      110 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/setup.cfg
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1176 2023-07-18 13:37:42.000000 ia-sdk-0.4.1/setup.py
```

### Comparing `ia-sdk-0.4.0/PKG-INFO` & `ia-sdk-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-sdk
-Version: 0.4.0
+Version: 0.4.1
 Summary: SDK for Intelligent Artifact's GAIuS agents.
 Home-page: https://intelligent-artifacts.com
 Author: Intelligent Artifacts
 Author-email: support@intelligent-artifacts.com
 Project-URL: Documentation, https://intelligent-artifacts.bitbucket.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ia-sdk-0.4.0/README.md` & `ia-sdk-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/agent_client.py` & `ia-sdk-0.4.1/ia/gaius/agent_client.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/back_testing.py` & `ia-sdk-0.4.1/ia/gaius/back_testing.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/comcom_client.py` & `ia-sdk-0.4.1/ia/gaius/comcom_client.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/data_language.py` & `ia-sdk-0.4.1/ia/gaius/data_language.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/data_ops.py` & `ia-sdk-0.4.1/ia/gaius/data_ops.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/data_structures.py` & `ia-sdk-0.4.1/ia/gaius/data_structures.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/experimental/genome_optimizer.py` & `ia-sdk-0.4.1/ia/gaius/experimental/genome_optimizer.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/genome_info.py` & `ia-sdk-0.4.1/ia/gaius/genome_info.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/kb_ops.py` & `ia-sdk-0.4.1/ia/gaius/kb_ops.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/manager.py` & `ia-sdk-0.4.1/ia/gaius/manager.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/prediction_models.py` & `ia-sdk-0.4.1/ia/gaius/prediction_models.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/pvt/__init__.py` & `ia-sdk-0.4.1/ia/gaius/pvt/__init__.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/pvt/mongo_interface.py` & `ia-sdk-0.4.1/ia/gaius/pvt/mongo_interface.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/pvt/offline_sio.py` & `ia-sdk-0.4.1/ia/gaius/pvt/offline_sio.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/pvt/pvt_utils.py` & `ia-sdk-0.4.1/ia/gaius/pvt/pvt_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,26 +409,30 @@
     Takes a node classification test to create a confusion matrix.
     This version includes the i_dont_know or unknown label.
     """
 
     for node_name, class_metrics_data in class_metrics_data_structures.items():
         # print(f'-------------Test#{test_num}-{node_name}-Plots-------------')
         sorted_labels = deepcopy(class_metrics_data['labels'])
+        label_set = set(sorted_labels).union(class_metrics_data['predictions'])
+        
         sorted_labels = [str(label)
-                         for label in sorted_labels if label is not None]
+                         for label in label_set if label is not None]
         sorted_labels.append(str(None))
         # sorted_labels = sorted(class_metrics_data['labels'])
         actuals = [[str(elem) for elem in act]
                    for act in class_metrics_data['actuals']]
         preds = [str(pred) for pred in class_metrics_data['predictions']]
         try:
             cm = confusion_matrix(actuals,  # TODO: each "actual" is a list, to support multiclass labels. Need to find solution here
                                   preds,
                                   labels=sorted_labels)
-        except ValueError:  # thrown when there are no predictions, and nothing to plot
+        except ValueError as e:  # thrown when there are no predictions, and nothing to plot
+            print(str(e))
+            logger.exception("broke in plot_confusion_matrix")
             return
         disp = ConfusionMatrixDisplay(confusion_matrix=cm,
                                       display_labels=sorted_labels)
 
         disp.plot()
         disp.ax_.set_title(f'Test#{test_num}-{node_name} Confusion Matrix')
         current_figure = plt.gcf()
```

### Comparing `ia-sdk-0.4.0/ia/gaius/tests/classification.py` & `ia-sdk-0.4.1/ia/gaius/tests/classification.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/tests/utility.py` & `ia-sdk-0.4.1/ia/gaius/tests/utility.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/gaius/utils.py` & `ia-sdk-0.4.1/ia/gaius/utils.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/scripts/spawn_agent.py` & `ia-sdk-0.4.1/ia/scripts/spawn_agent.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia/scripts/spawn_general.py` & `ia-sdk-0.4.1/ia/scripts/spawn_general.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/ia_sdk.egg-info/PKG-INFO` & `ia-sdk-0.4.1/ia_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-sdk
-Version: 0.4.0
+Version: 0.4.1
 Summary: SDK for Intelligent Artifact's GAIuS agents.
 Home-page: https://intelligent-artifacts.com
 Author: Intelligent Artifacts
 Author-email: support@intelligent-artifacts.com
 Project-URL: Documentation, https://intelligent-artifacts.bitbucket.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ia-sdk-0.4.0/ia_sdk.egg-info/SOURCES.txt` & `ia-sdk-0.4.1/ia_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.0/setup.py` & `ia-sdk-0.4.1/setup.py`

 * *Files identical despite different names*

