# Comparing `tmp/nlubridge-1.0.1.tar.gz` & `tmp/nlubridge-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlubridge-1.0.1.tar", last modified: Mon May  8 12:56:19 2023, max compression
+gzip compressed data, was "nlubridge-1.0.2.tar", last modified: Wed Aug  2 15:29:55 2023, max compression
```

## Comparing `nlubridge-1.0.1.tar` & `nlubridge-1.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.050644 nlubridge-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-08 12:56:05.000000 nlubridge-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 12:56:05.000000 nlubridge-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-08 12:56:19.050644 nlubridge-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-05-08 12:56:05.000000 nlubridge-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.046643 nlubridge-1.0.1/nlubridge/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.046643 nlubridge-1.0.1/nlubridge/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/dataloaders/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/dataloaders/luis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/dataloaders/rasa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/dataloaders/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/dataloaders/watson_assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/nlu_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.050644 nlubridge-1.0.1/nlubridge/vendors/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/char_ngram_intent_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.050644 nlubridge-1.0.1/nlubridge/vendors/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/config/rasa_nlu_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     3522 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/luis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7122 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/rasa2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/rasa3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/spacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/tfidf_intent_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-05-08 12:56:05.000000 nlubridge-1.0.1/nlubridge/vendors/watson_assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.046643 nlubridge-1.0.1/nlubridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-08 12:56:19.000000 nlubridge-1.0.1/nlubridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-08 12:56:19.000000 nlubridge-1.0.1/nlubridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:56:19.000000 nlubridge-1.0.1/nlubridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 12:56:19.000000 nlubridge-1.0.1/nlubridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 12:56:19.000000 nlubridge-1.0.1/nlubridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-08 12:56:05.000000 nlubridge-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 12:56:19.050644 nlubridge-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-08 12:56:05.000000 nlubridge-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:56:19.050644 nlubridge-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-08 12:56:05.000000 nlubridge-1.0.1/tests/test_dataset_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-05-08 12:56:05.000000 nlubridge-1.0.1/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-08 12:56:05.000000 nlubridge-1.0.1/tests/test_vendors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-08 12:56:05.000000 nlubridge-1.0.1/tests/test_watson_vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-05-08 12:56:05.000000 nlubridge-1.0.1/tests/test_watson_vendor_mocked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-08 12:56:05.000000 nlubridge-1.0.1/tests/testing_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:29:55.320332 nlubridge-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-02 15:29:44.000000 nlubridge-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 15:29:44.000000 nlubridge-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-08-02 15:29:55.320332 nlubridge-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-08-02 15:29:44.000000 nlubridge-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:29:55.312332 nlubridge-1.0.2/nlubridge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:29:55.316332 nlubridge-1.0.2/nlubridge/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/dataloaders/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/dataloaders/luis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/dataloaders/rasa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/dataloaders/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/dataloaders/watson_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/nlu_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:29:55.316332 nlubridge-1.0.2/nlubridge/vendors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/vendors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/vendors/char_ngram_intent_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:29:55.316332 nlubridge-1.0.2/nlubridge/vendors/config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/vendors/config/rasa_nlu_config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3522 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/vendors/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/vendors/luis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7122 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/vendors/rasa2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/vendors/rasa3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/vendors/spacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/vendors/tfidf_intent_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/vendors/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-08-02 15:29:44.000000 nlubridge-1.0.2/nlubridge/vendors/watson_assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:29:55.316332 nlubridge-1.0.2/nlubridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-08-02 15:29:55.000000 nlubridge-1.0.2/nlubridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-02 15:29:55.000000 nlubridge-1.0.2/nlubridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:29:55.000000 nlubridge-1.0.2/nlubridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-02 15:29:55.000000 nlubridge-1.0.2/nlubridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 15:29:55.000000 nlubridge-1.0.2/nlubridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-02 15:29:44.000000 nlubridge-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-02 15:29:55.320332 nlubridge-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-08-02 15:29:44.000000 nlubridge-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:29:55.320332 nlubridge-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-08-02 15:29:44.000000 nlubridge-1.0.2/tests/test_dataset_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-08-02 15:29:44.000000 nlubridge-1.0.2/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-08-02 15:29:44.000000 nlubridge-1.0.2/tests/test_vendors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-08-02 15:29:44.000000 nlubridge-1.0.2/tests/test_watson_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-08-02 15:29:44.000000 nlubridge-1.0.2/tests/test_watson_vendor_mocked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-02 15:29:44.000000 nlubridge-1.0.2/tests/testing_data.py
```

### Comparing `nlubridge-1.0.1/LICENSE` & `nlubridge-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/PKG-INFO` & `nlubridge-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nlubridge
-Version: 1.0.1
+Version: 1.0.2
 Summary: Provides a unified API to several popular intent recognition applications
 Home-page: https://github.com/telekom/nlu-bridge
 Author: Klaus-Peter Engelbrecht
 Author-email: k.engelbrecht@telekom.de
 Maintainer: Klaus-Peter Engelbrecht
 Project-URL: Bug Tracker, https://github.com/telekom/nlu-bridge/issues
 Project-URL: Source Code, https://github.com/telekom/nlu-bridge
 Project-URL: Contributing, https://github.com/telekom/nlu-bridge/blob/main/CONTRIBUTING.md
 Project-URL: Code of Conduct, https://github.com/telekom/nlu-bridge/blob/main/CODE_OF_CONDUCT.md
 Keywords: nlu,intent recognition,natural language understanding,evaluation,performance
-Requires-Python: >=3, <3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: watson
 Provides-Extra: fasttext
 Provides-Extra: luis
 Provides-Extra: rasa2
 Provides-Extra: rasa3
 Provides-Extra: spacy
@@ -44,21 +44,24 @@
 The goal of this project is to provide a unified API to several popular intent recognition
 applications.
 
 ## About this component
 
 ### Installation
 
-The core package including NLUdataset and Baseline vendors can be installed for Python\<=3.8
-using pip
+The core package including NLUdataset and Baseline vendors can be installed for
+Python>=3.8 using pip
 
 ```
 pip install nlubridge
 ```
 
+Note that some vendors come with restrictions regarding the Python version, e.g. Rasa3
+requires Python\<3.11.
+
 To include optional dependencies for the vendors, e.g. Watson Assistant, type
 
 ```
 pip install nlubridge[watson]
 ```
 
 Following install options are available:
```

#### html2text {}

```diff
@@ -1,114 +1,115 @@
-Metadata-Version: 2.1 Name: nlubridge Version: 1.0.1 Summary: Provides a
+Metadata-Version: 2.1 Name: nlubridge Version: 1.0.2 Summary: Provides a
 unified API to several popular intent recognition applications Home-page:
 https://github.com/telekom/nlu-bridge Author: Klaus-Peter Engelbrecht Author-
 email: k.engelbrecht@telekom.de Maintainer: Klaus-Peter Engelbrecht Project-
 URL: Bug Tracker, https://github.com/telekom/nlu-bridge/issues Project-URL:
 Source Code, https://github.com/telekom/nlu-bridge Project-URL: Contributing,
 https://github.com/telekom/nlu-bridge/blob/main/CONTRIBUTING.md Project-URL:
 Code of Conduct, https://github.com/telekom/nlu-bridge/blob/main/
 CODE_OF_CONDUCT.md Keywords: nlu,intent recognition,natural language
-understanding,evaluation,performance Requires-Python: >=3, <3.9 Description-
+understanding,evaluation,performance Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: watson Provides-Extra: fasttext
 Provides-Extra: luis Provides-Extra: rasa2 Provides-Extra: rasa3 Provides-
 Extra: spacy Provides-Extra: huggingface Provides-Extra: develop License-File:
 LICENSE
                        ****** Telekom NLU Bridge ******
   [https://img.shields.io/github/last-commit/telekom/nlu-bridge?style=flat]
 [https://img.shields.io/github/issues/telekom/nlu-bridge?style=flat] [https://
             img.shields.io/badge/License-MIT-green.svg?style=flat]
     Development â¢ Documentation â¢ Support â¢ Contribute â¢ Licensing
 The goal of this project is to provide a unified API to several popular intent
 recognition applications. ## About this component ### Installation The core
 package including NLUdataset and Baseline vendors can be installed for
-Python\<=3.8 using pip ``` pip install nlubridge ``` To include optional
-dependencies for the vendors, e.g. Watson Assistant, type ``` pip install
-nlubridge[watson] ``` Following install options are available: - `watson` -
-`fasttext` - `luis` - `rasa2` - `rasa3` - `spacy` - `huggingface` Development
-tools can be installed with option `develop`. Some vendors require access
-credentials like API tokens, URLs etc. These can be passed on construction of
-the objects. Alternatively, such arguments can be passed as environment
-variables, where the vendor will look for variables named variable
-VENDORNAME_PARAM_NAME. Some vendors require additional dependencies. E.g.,
-Spacy requires a model that can be downloaded (for the model de_core_news_sm)
-with ``` python -m spacy download de_core_news_sm ``` ### Migration from v0
-With realease 1.0.0 we introduce a couple of changes to the names of files and
-vendor classes(see also https://github.com/telekom/nlu-bridge/issues/18). Most
-notably: - datasets.NLUdataset -> nlu_dataset.NluDataset -
-vendors.vendors.Vendor -> - vendors.vendor.Vendor - new supackage `dataloaders`
-that holds all functions for loading data into an NluDataset - new function
-`nlu_dataset.concat` to concatenate NluDatasets passed in a list - can load
-dataloaders, NluDataset, Vendor, OUT_OF_SCOPE_TOKEN, EntityKeys, concat,
-directly from nlubridge like `from nlubridge import Vendor` - Load vendors like
-`from nlubridge.vendors import Rasa3` - former `TelekomModel` now called
-`CharNgramIntentClassifier` - Some vendor names changed for clarity and
-consistency (see "List of supported vendors" for the new names) ### Usage Here
-is an example for the TfidfIntentClassifier: ```python import os import pandas
-as pd from nlubridge.vendors import TfidfIntentClassifier from nlubridge import
-NluDataset dataset = NluDataset(texts, intents) dataset = dataset.shuffle()
-classifier = TfidfIntentClassifier() train, test = dataset.train_test_split
-(test_size=0.25, random_state=0) classifier = classifier.train_intent(train)
-predicted = classifier.test_intent(test) res = pd.DataFrame(list(zip
-(test.intents, predicted)), columns=['true', 'predicted']) ``` If you need to
-configure **stratification**, use the `stratification` parameter (defaults to
-`"intents"` and uses the intents in the dataset as stratification basis;
-whatever _else_ you pass along has to conform to
-`sklearn.model_selection.train_test_split(stratify=)`: ```python train, test =
-dataset.train_test_split(test_size=0.25, random_state=0, stratification=None) #
-deactivate stratification (sklearn default for train_test_split) ``` To compare
-your own vendor or algorithm to existing vendors in this package, you can write
-a Vendor Subclass for your vendor, and possibly a dataloader function. Feel
-free to share your implementation using this repo. Similarly, fixes and
-extensions for the existing vendors are always welcome. ### Logging Most of the
-code uses python logging to report its progress. To get logs printed out to
-console or Jupyter notebook, a logger needs to be configured, before the
-nlutests code. Usually, log messages are on INFO level. This can be configured
-like this: ```python import logging logger = logging.getLogger()
-logger.setLevel(logging.INFO) logger.addHandler(logging.StreamHandler()) ```
-### Concepts / Architecture - **Vendors**\ The [`vendors`](/nlubridge/vendors/
-) subpackage implements standardized interfaces to the specific vendors. A
-specific `Vendor` instance is in charge of dealing with converting the data to
-the required format, uploading data to the cloud if applicable, training models
-and making predictions. - **Datasets**\ The [`nlu_dataset`](/nlubridge/
-nlu_dataset/) module provides a standard interface to NLU data. Data stored in
-different vendor's custom format can be loaded as a dataset and provided to any
-different vendor. - **Data Loaders**\ The [`dataloaders`](/nlubridge/
-dataloaders/) subpackage provides functions to load data that are in a vendor-
-specific format as NluDataset. ### List of supported vendors | Vendor Class |
-Status | Intents | Entities | Algorithm | | ------ | ------ | ------- | -------
-- | --------- | | [TfidfIntentClassifier](/nlubridge/vendors/
-tfidf_intent_classifier.py) | â | â | â | TFIDF on words + SVM | |
-[FastText](https://fasttext.cc) | â | â | â | fasttext | | [Spacy](https:
-//spacy.io/usage/training#section-textcat) | â | â | â | BoW linear + CNN
-| | [WatsonAssistant](https://www.ibm.com/watson/services/conversation/) | â
-| â | â | Propietary (probably LR) | | [Luis](https://www.luis.ai/home) |
-needs testing | â | â | Propietary (probably LR) | |
-[CharNgramIntentClassifier](/nlubridge/vendors/char_ngram_intent_classifier.py)
-| â | â | â | tf-idf on char n-grams + SGD | | [Rasa2](https://
-github.com/RasaHQ/rasa) | â | â | â | configurable | | [Rasa3](https://
-github.com/RasaHQ/rasa) | â | â | â | configurable | ### Features -
-Abstract class for Vendors with convenience methods (ex: scoring and scikit-
-learn compatibility) - Abstract class for datasets with convenience methods
-(ex: train_test_split, indexing, iteration) - Rate limiting to comply with
-cloud providers requirements ## Development _TBD_ ### Build _TBD_ ## Code of
-Conduct This project has adopted the [Contributor Covenant](https://
-www.contributor-covenant.org/) in version 2.0 as our code of conduct. Please
-see the details in our [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md). All
-contributors must abide by the code of conduct. ## Working Language We decided
-to apply _English_ as the primary project language. Consequently, all content
-will be made available primarily in English. We also ask all interested people
-to use English as language to create issues, in their code (comments,
-documentation etc.) and when you send requests to us. The application itself
-and all end-user facing content will be made available in other languages as
-needed. ## Documentation The full documentation for the telekom nlu-bridge can
-be found in _TBD_ ## Support and Feedback The following channels are available
-for discussions, feedback, and support requests: | Type | Channel | | ---------
---------------- | ------------------------------------------------------ | |
-**Issues** | [https://img.shields.io/github/issues/telekom/nlu-
-bridge?style=flat-square]
+Python>=3.8 using pip ``` pip install nlubridge ``` Note that some vendors come
+with restrictions regarding the Python version, e.g. Rasa3 requires
+Python\<3.11. To include optional dependencies for the vendors, e.g. Watson
+Assistant, type ``` pip install nlubridge[watson] ``` Following install options
+are available: - `watson` - `fasttext` - `luis` - `rasa2` - `rasa3` - `spacy` -
+`huggingface` Development tools can be installed with option `develop`. Some
+vendors require access credentials like API tokens, URLs etc. These can be
+passed on construction of the objects. Alternatively, such arguments can be
+passed as environment variables, where the vendor will look for variables named
+variable VENDORNAME_PARAM_NAME. Some vendors require additional dependencies.
+E.g., Spacy requires a model that can be downloaded (for the model
+de_core_news_sm) with ``` python -m spacy download de_core_news_sm ``` ###
+Migration from v0 With realease 1.0.0 we introduce a couple of changes to the
+names of files and vendor classes(see also https://github.com/telekom/nlu-
+bridge/issues/18). Most notably: - datasets.NLUdataset -
+> nlu_dataset.NluDataset - vendors.vendors.Vendor -> - vendors.vendor.Vendor -
+new supackage `dataloaders` that holds all functions for loading data into an
+NluDataset - new function `nlu_dataset.concat` to concatenate NluDatasets
+passed in a list - can load dataloaders, NluDataset, Vendor,
+OUT_OF_SCOPE_TOKEN, EntityKeys, concat, directly from nlubridge like `from
+nlubridge import Vendor` - Load vendors like `from nlubridge.vendors import
+Rasa3` - former `TelekomModel` now called `CharNgramIntentClassifier` - Some
+vendor names changed for clarity and consistency (see "List of supported
+vendors" for the new names) ### Usage Here is an example for the
+TfidfIntentClassifier: ```python import os import pandas as pd from
+nlubridge.vendors import TfidfIntentClassifier from nlubridge import NluDataset
+dataset = NluDataset(texts, intents) dataset = dataset.shuffle() classifier =
+TfidfIntentClassifier() train, test = dataset.train_test_split(test_size=0.25,
+random_state=0) classifier = classifier.train_intent(train) predicted =
+classifier.test_intent(test) res = pd.DataFrame(list(zip(test.intents,
+predicted)), columns=['true', 'predicted']) ``` If you need to configure
+**stratification**, use the `stratification` parameter (defaults to `"intents"`
+and uses the intents in the dataset as stratification basis; whatever _else_
+you pass along has to conform to `sklearn.model_selection.train_test_split
+(stratify=)`: ```python train, test = dataset.train_test_split(test_size=0.25,
+random_state=0, stratification=None) # deactivate stratification (sklearn
+default for train_test_split) ``` To compare your own vendor or algorithm to
+existing vendors in this package, you can write a Vendor Subclass for your
+vendor, and possibly a dataloader function. Feel free to share your
+implementation using this repo. Similarly, fixes and extensions for the
+existing vendors are always welcome. ### Logging Most of the code uses python
+logging to report its progress. To get logs printed out to console or Jupyter
+notebook, a logger needs to be configured, before the nlutests code. Usually,
+log messages are on INFO level. This can be configured like this: ```python
+import logging logger = logging.getLogger() logger.setLevel(logging.INFO)
+logger.addHandler(logging.StreamHandler()) ``` ### Concepts / Architecture -
+**Vendors**\ The [`vendors`](/nlubridge/vendors/) subpackage implements
+standardized interfaces to the specific vendors. A specific `Vendor` instance
+is in charge of dealing with converting the data to the required format,
+uploading data to the cloud if applicable, training models and making
+predictions. - **Datasets**\ The [`nlu_dataset`](/nlubridge/nlu_dataset/
+) module provides a standard interface to NLU data. Data stored in different
+vendor's custom format can be loaded as a dataset and provided to any different
+vendor. - **Data Loaders**\ The [`dataloaders`](/nlubridge/dataloaders/
+) subpackage provides functions to load data that are in a vendor-specific
+format as NluDataset. ### List of supported vendors | Vendor Class | Status |
+Intents | Entities | Algorithm | | ------ | ------ | ------- | -------- | -----
+---- | | [TfidfIntentClassifier](/nlubridge/vendors/tfidf_intent_classifier.py)
+| â | â | â | TFIDF on words + SVM | | [FastText](https://fasttext.cc) |
+â | â | â | fasttext | | [Spacy](https://spacy.io/usage/training#section-
+textcat) | â | â | â | BoW linear + CNN | | [WatsonAssistant](https://
+www.ibm.com/watson/services/conversation/) | â | â | â | Propietary
+(probably LR) | | [Luis](https://www.luis.ai/home) | needs testing | â | â
+| Propietary (probably LR) | | [CharNgramIntentClassifier](/nlubridge/vendors/
+char_ngram_intent_classifier.py) | â | â | â | tf-idf on char n-grams +
+SGD | | [Rasa2](https://github.com/RasaHQ/rasa) | â | â | â |
+configurable | | [Rasa3](https://github.com/RasaHQ/rasa) | â | â | â |
+configurable | ### Features - Abstract class for Vendors with convenience
+methods (ex: scoring and scikit-learn compatibility) - Abstract class for
+datasets with convenience methods (ex: train_test_split, indexing, iteration) -
+Rate limiting to comply with cloud providers requirements ## Development _TBD_
+### Build _TBD_ ## Code of Conduct This project has adopted the [Contributor
+Covenant](https://www.contributor-covenant.org/) in version 2.0 as our code of
+conduct. Please see the details in our [CODE_OF_CONDUCT.md]
+(CODE_OF_CONDUCT.md). All contributors must abide by the code of conduct. ##
+Working Language We decided to apply _English_ as the primary project language.
+Consequently, all content will be made available primarily in English. We also
+ask all interested people to use English as language to create issues, in their
+code (comments, documentation etc.) and when you send requests to us. The
+application itself and all end-user facing content will be made available in
+other languages as needed. ## Documentation The full documentation for the
+telekom nlu-bridge can be found in _TBD_ ## Support and Feedback The following
+channels are available for discussions, feedback, and support requests: | Type
+| Channel | | ------------------------ | --------------------------------------
+---------------- | | **Issues** | [https://img.shields.io/github/issues/
+telekom/nlu-bridge?style=flat-square]
  | | **Other Requests** | [https://img.shields.io/badge/email-
 Open%20Source%20Team-green?logo=mail.ru&style=flat-square&logoColor=white] | ##
 How to Contribute Contribution and feedback is encouraged and always welcome.
 For more information about how to contribute, the project structure, as well as
 additional contribution information, see our [Contribution Guidelines](./
 CONTRIBUTING.md). By participating in this project, you agree to abide by its
 [Code of Conduct](./CODE_OF_CONDUCT.md) at all times. ## Licensing Copyright
```

### Comparing `nlubridge-1.0.1/README.md` & `nlubridge-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,24 @@
 The goal of this project is to provide a unified API to several popular intent recognition
 applications.
 
 ## About this component
 
 ### Installation
 
-The core package including NLUdataset and Baseline vendors can be installed for Python\<=3.8
-using pip
+The core package including NLUdataset and Baseline vendors can be installed for
+Python>=3.8 using pip
 
 ```
 pip install nlubridge
 ```
 
+Note that some vendors come with restrictions regarding the Python version, e.g. Rasa3
+requires Python\<3.11.
+
 To include optional dependencies for the vendors, e.g. Watson Assistant, type
 
 ```
 pip install nlubridge[watson]
 ```
 
 Following install options are available:
```

#### html2text {}

```diff
@@ -2,99 +2,100 @@
   [https://img.shields.io/github/last-commit/telekom/nlu-bridge?style=flat]
 [https://img.shields.io/github/issues/telekom/nlu-bridge?style=flat] [https://
             img.shields.io/badge/License-MIT-green.svg?style=flat]
     Development â¢ Documentation â¢ Support â¢ Contribute â¢ Licensing
 The goal of this project is to provide a unified API to several popular intent
 recognition applications. ## About this component ### Installation The core
 package including NLUdataset and Baseline vendors can be installed for
-Python\<=3.8 using pip ``` pip install nlubridge ``` To include optional
-dependencies for the vendors, e.g. Watson Assistant, type ``` pip install
-nlubridge[watson] ``` Following install options are available: - `watson` -
-`fasttext` - `luis` - `rasa2` - `rasa3` - `spacy` - `huggingface` Development
-tools can be installed with option `develop`. Some vendors require access
-credentials like API tokens, URLs etc. These can be passed on construction of
-the objects. Alternatively, such arguments can be passed as environment
-variables, where the vendor will look for variables named variable
-VENDORNAME_PARAM_NAME. Some vendors require additional dependencies. E.g.,
-Spacy requires a model that can be downloaded (for the model de_core_news_sm)
-with ``` python -m spacy download de_core_news_sm ``` ### Migration from v0
-With realease 1.0.0 we introduce a couple of changes to the names of files and
-vendor classes(see also https://github.com/telekom/nlu-bridge/issues/18). Most
-notably: - datasets.NLUdataset -> nlu_dataset.NluDataset -
-vendors.vendors.Vendor -> - vendors.vendor.Vendor - new supackage `dataloaders`
-that holds all functions for loading data into an NluDataset - new function
-`nlu_dataset.concat` to concatenate NluDatasets passed in a list - can load
-dataloaders, NluDataset, Vendor, OUT_OF_SCOPE_TOKEN, EntityKeys, concat,
-directly from nlubridge like `from nlubridge import Vendor` - Load vendors like
-`from nlubridge.vendors import Rasa3` - former `TelekomModel` now called
-`CharNgramIntentClassifier` - Some vendor names changed for clarity and
-consistency (see "List of supported vendors" for the new names) ### Usage Here
-is an example for the TfidfIntentClassifier: ```python import os import pandas
-as pd from nlubridge.vendors import TfidfIntentClassifier from nlubridge import
-NluDataset dataset = NluDataset(texts, intents) dataset = dataset.shuffle()
-classifier = TfidfIntentClassifier() train, test = dataset.train_test_split
-(test_size=0.25, random_state=0) classifier = classifier.train_intent(train)
-predicted = classifier.test_intent(test) res = pd.DataFrame(list(zip
-(test.intents, predicted)), columns=['true', 'predicted']) ``` If you need to
-configure **stratification**, use the `stratification` parameter (defaults to
-`"intents"` and uses the intents in the dataset as stratification basis;
-whatever _else_ you pass along has to conform to
-`sklearn.model_selection.train_test_split(stratify=)`: ```python train, test =
-dataset.train_test_split(test_size=0.25, random_state=0, stratification=None) #
-deactivate stratification (sklearn default for train_test_split) ``` To compare
-your own vendor or algorithm to existing vendors in this package, you can write
-a Vendor Subclass for your vendor, and possibly a dataloader function. Feel
-free to share your implementation using this repo. Similarly, fixes and
-extensions for the existing vendors are always welcome. ### Logging Most of the
-code uses python logging to report its progress. To get logs printed out to
-console or Jupyter notebook, a logger needs to be configured, before the
-nlutests code. Usually, log messages are on INFO level. This can be configured
-like this: ```python import logging logger = logging.getLogger()
-logger.setLevel(logging.INFO) logger.addHandler(logging.StreamHandler()) ```
-### Concepts / Architecture - **Vendors**\ The [`vendors`](/nlubridge/vendors/
-) subpackage implements standardized interfaces to the specific vendors. A
-specific `Vendor` instance is in charge of dealing with converting the data to
-the required format, uploading data to the cloud if applicable, training models
-and making predictions. - **Datasets**\ The [`nlu_dataset`](/nlubridge/
-nlu_dataset/) module provides a standard interface to NLU data. Data stored in
-different vendor's custom format can be loaded as a dataset and provided to any
-different vendor. - **Data Loaders**\ The [`dataloaders`](/nlubridge/
-dataloaders/) subpackage provides functions to load data that are in a vendor-
-specific format as NluDataset. ### List of supported vendors | Vendor Class |
-Status | Intents | Entities | Algorithm | | ------ | ------ | ------- | -------
-- | --------- | | [TfidfIntentClassifier](/nlubridge/vendors/
-tfidf_intent_classifier.py) | â | â | â | TFIDF on words + SVM | |
-[FastText](https://fasttext.cc) | â | â | â | fasttext | | [Spacy](https:
-//spacy.io/usage/training#section-textcat) | â | â | â | BoW linear + CNN
-| | [WatsonAssistant](https://www.ibm.com/watson/services/conversation/) | â
-| â | â | Propietary (probably LR) | | [Luis](https://www.luis.ai/home) |
-needs testing | â | â | Propietary (probably LR) | |
-[CharNgramIntentClassifier](/nlubridge/vendors/char_ngram_intent_classifier.py)
-| â | â | â | tf-idf on char n-grams + SGD | | [Rasa2](https://
-github.com/RasaHQ/rasa) | â | â | â | configurable | | [Rasa3](https://
-github.com/RasaHQ/rasa) | â | â | â | configurable | ### Features -
-Abstract class for Vendors with convenience methods (ex: scoring and scikit-
-learn compatibility) - Abstract class for datasets with convenience methods
-(ex: train_test_split, indexing, iteration) - Rate limiting to comply with
-cloud providers requirements ## Development _TBD_ ### Build _TBD_ ## Code of
-Conduct This project has adopted the [Contributor Covenant](https://
-www.contributor-covenant.org/) in version 2.0 as our code of conduct. Please
-see the details in our [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md). All
-contributors must abide by the code of conduct. ## Working Language We decided
-to apply _English_ as the primary project language. Consequently, all content
-will be made available primarily in English. We also ask all interested people
-to use English as language to create issues, in their code (comments,
-documentation etc.) and when you send requests to us. The application itself
-and all end-user facing content will be made available in other languages as
-needed. ## Documentation The full documentation for the telekom nlu-bridge can
-be found in _TBD_ ## Support and Feedback The following channels are available
-for discussions, feedback, and support requests: | Type | Channel | | ---------
---------------- | ------------------------------------------------------ | |
-**Issues** | [https://img.shields.io/github/issues/telekom/nlu-
-bridge?style=flat-square]
+Python>=3.8 using pip ``` pip install nlubridge ``` Note that some vendors come
+with restrictions regarding the Python version, e.g. Rasa3 requires
+Python\<3.11. To include optional dependencies for the vendors, e.g. Watson
+Assistant, type ``` pip install nlubridge[watson] ``` Following install options
+are available: - `watson` - `fasttext` - `luis` - `rasa2` - `rasa3` - `spacy` -
+`huggingface` Development tools can be installed with option `develop`. Some
+vendors require access credentials like API tokens, URLs etc. These can be
+passed on construction of the objects. Alternatively, such arguments can be
+passed as environment variables, where the vendor will look for variables named
+variable VENDORNAME_PARAM_NAME. Some vendors require additional dependencies.
+E.g., Spacy requires a model that can be downloaded (for the model
+de_core_news_sm) with ``` python -m spacy download de_core_news_sm ``` ###
+Migration from v0 With realease 1.0.0 we introduce a couple of changes to the
+names of files and vendor classes(see also https://github.com/telekom/nlu-
+bridge/issues/18). Most notably: - datasets.NLUdataset -
+> nlu_dataset.NluDataset - vendors.vendors.Vendor -> - vendors.vendor.Vendor -
+new supackage `dataloaders` that holds all functions for loading data into an
+NluDataset - new function `nlu_dataset.concat` to concatenate NluDatasets
+passed in a list - can load dataloaders, NluDataset, Vendor,
+OUT_OF_SCOPE_TOKEN, EntityKeys, concat, directly from nlubridge like `from
+nlubridge import Vendor` - Load vendors like `from nlubridge.vendors import
+Rasa3` - former `TelekomModel` now called `CharNgramIntentClassifier` - Some
+vendor names changed for clarity and consistency (see "List of supported
+vendors" for the new names) ### Usage Here is an example for the
+TfidfIntentClassifier: ```python import os import pandas as pd from
+nlubridge.vendors import TfidfIntentClassifier from nlubridge import NluDataset
+dataset = NluDataset(texts, intents) dataset = dataset.shuffle() classifier =
+TfidfIntentClassifier() train, test = dataset.train_test_split(test_size=0.25,
+random_state=0) classifier = classifier.train_intent(train) predicted =
+classifier.test_intent(test) res = pd.DataFrame(list(zip(test.intents,
+predicted)), columns=['true', 'predicted']) ``` If you need to configure
+**stratification**, use the `stratification` parameter (defaults to `"intents"`
+and uses the intents in the dataset as stratification basis; whatever _else_
+you pass along has to conform to `sklearn.model_selection.train_test_split
+(stratify=)`: ```python train, test = dataset.train_test_split(test_size=0.25,
+random_state=0, stratification=None) # deactivate stratification (sklearn
+default for train_test_split) ``` To compare your own vendor or algorithm to
+existing vendors in this package, you can write a Vendor Subclass for your
+vendor, and possibly a dataloader function. Feel free to share your
+implementation using this repo. Similarly, fixes and extensions for the
+existing vendors are always welcome. ### Logging Most of the code uses python
+logging to report its progress. To get logs printed out to console or Jupyter
+notebook, a logger needs to be configured, before the nlutests code. Usually,
+log messages are on INFO level. This can be configured like this: ```python
+import logging logger = logging.getLogger() logger.setLevel(logging.INFO)
+logger.addHandler(logging.StreamHandler()) ``` ### Concepts / Architecture -
+**Vendors**\ The [`vendors`](/nlubridge/vendors/) subpackage implements
+standardized interfaces to the specific vendors. A specific `Vendor` instance
+is in charge of dealing with converting the data to the required format,
+uploading data to the cloud if applicable, training models and making
+predictions. - **Datasets**\ The [`nlu_dataset`](/nlubridge/nlu_dataset/
+) module provides a standard interface to NLU data. Data stored in different
+vendor's custom format can be loaded as a dataset and provided to any different
+vendor. - **Data Loaders**\ The [`dataloaders`](/nlubridge/dataloaders/
+) subpackage provides functions to load data that are in a vendor-specific
+format as NluDataset. ### List of supported vendors | Vendor Class | Status |
+Intents | Entities | Algorithm | | ------ | ------ | ------- | -------- | -----
+---- | | [TfidfIntentClassifier](/nlubridge/vendors/tfidf_intent_classifier.py)
+| â | â | â | TFIDF on words + SVM | | [FastText](https://fasttext.cc) |
+â | â | â | fasttext | | [Spacy](https://spacy.io/usage/training#section-
+textcat) | â | â | â | BoW linear + CNN | | [WatsonAssistant](https://
+www.ibm.com/watson/services/conversation/) | â | â | â | Propietary
+(probably LR) | | [Luis](https://www.luis.ai/home) | needs testing | â | â
+| Propietary (probably LR) | | [CharNgramIntentClassifier](/nlubridge/vendors/
+char_ngram_intent_classifier.py) | â | â | â | tf-idf on char n-grams +
+SGD | | [Rasa2](https://github.com/RasaHQ/rasa) | â | â | â |
+configurable | | [Rasa3](https://github.com/RasaHQ/rasa) | â | â | â |
+configurable | ### Features - Abstract class for Vendors with convenience
+methods (ex: scoring and scikit-learn compatibility) - Abstract class for
+datasets with convenience methods (ex: train_test_split, indexing, iteration) -
+Rate limiting to comply with cloud providers requirements ## Development _TBD_
+### Build _TBD_ ## Code of Conduct This project has adopted the [Contributor
+Covenant](https://www.contributor-covenant.org/) in version 2.0 as our code of
+conduct. Please see the details in our [CODE_OF_CONDUCT.md]
+(CODE_OF_CONDUCT.md). All contributors must abide by the code of conduct. ##
+Working Language We decided to apply _English_ as the primary project language.
+Consequently, all content will be made available primarily in English. We also
+ask all interested people to use English as language to create issues, in their
+code (comments, documentation etc.) and when you send requests to us. The
+application itself and all end-user facing content will be made available in
+other languages as needed. ## Documentation The full documentation for the
+telekom nlu-bridge can be found in _TBD_ ## Support and Feedback The following
+channels are available for discussions, feedback, and support requests: | Type
+| Channel | | ------------------------ | --------------------------------------
+---------------- | | **Issues** | [https://img.shields.io/github/issues/
+telekom/nlu-bridge?style=flat-square]
  | | **Other Requests** | [https://img.shields.io/badge/email-
 Open%20Source%20Team-green?logo=mail.ru&style=flat-square&logoColor=white] | ##
 How to Contribute Contribution and feedback is encouraged and always welcome.
 For more information about how to contribute, the project structure, as well as
 additional contribution information, see our [Contribution Guidelines](./
 CONTRIBUTING.md). By participating in this project, you agree to abide by its
 [Code of Conduct](./CODE_OF_CONDUCT.md) at all times. ## Licensing Copyright
```

### Comparing `nlubridge-1.0.1/nlubridge/__init__.py` & `nlubridge-1.0.2/nlubridge/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import sys
 from typing import TYPE_CHECKING
 
 from lazy_imports import LazyImporter
 
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 
 if TYPE_CHECKING:
     from .dataloaders.huggingface import from_huggingface  # noqa: F401
     from .dataloaders.luis import from_luis  # noqa: F401
     from .dataloaders.rasa import from_rasa, to_rasa  # noqa: F401, F811
     from .dataloaders.utils import from_csv, from_json  # noqa: F401
```

### Comparing `nlubridge-1.0.1/nlubridge/dataloaders/huggingface.py` & `nlubridge-1.0.2/nlubridge/dataloaders/huggingface.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/dataloaders/luis.py` & `nlubridge-1.0.2/nlubridge/dataloaders/luis.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/dataloaders/rasa.py` & `nlubridge-1.0.2/nlubridge/dataloaders/rasa.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/dataloaders/utils.py` & `nlubridge-1.0.2/nlubridge/dataloaders/utils.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/datasets.py` & `nlubridge-1.0.2/nlubridge/datasets.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/nlu_dataset.py` & `nlubridge-1.0.2/nlubridge/nlu_dataset.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/vendors/__init__.py` & `nlubridge-1.0.2/nlubridge/vendors/__init__.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/vendors/char_ngram_intent_classifier.py` & `nlubridge-1.0.2/nlubridge/vendors/char_ngram_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/vendors/config/rasa_nlu_config.yml` & `nlubridge-1.0.2/nlubridge/vendors/config/rasa_nlu_config.yml`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/vendors/fasttext.py` & `nlubridge-1.0.2/nlubridge/vendors/fasttext.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/vendors/luis.py` & `nlubridge-1.0.2/nlubridge/vendors/luis.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/vendors/rasa2.py` & `nlubridge-1.0.2/nlubridge/vendors/rasa2.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/vendors/rasa3.py` & `nlubridge-1.0.2/nlubridge/vendors/rasa3.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/vendors/spacy.py` & `nlubridge-1.0.2/nlubridge/vendors/spacy.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/vendors/tfidf_intent_classifier.py` & `nlubridge-1.0.2/nlubridge/vendors/tfidf_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/vendors/vendor.py` & `nlubridge-1.0.2/nlubridge/vendors/vendor.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge/vendors/watson_assistant.py` & `nlubridge-1.0.2/nlubridge/vendors/watson_assistant.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/nlubridge.egg-info/PKG-INFO` & `nlubridge-1.0.2/nlubridge.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nlubridge
-Version: 1.0.1
+Version: 1.0.2
 Summary: Provides a unified API to several popular intent recognition applications
 Home-page: https://github.com/telekom/nlu-bridge
 Author: Klaus-Peter Engelbrecht
 Author-email: k.engelbrecht@telekom.de
 Maintainer: Klaus-Peter Engelbrecht
 Project-URL: Bug Tracker, https://github.com/telekom/nlu-bridge/issues
 Project-URL: Source Code, https://github.com/telekom/nlu-bridge
 Project-URL: Contributing, https://github.com/telekom/nlu-bridge/blob/main/CONTRIBUTING.md
 Project-URL: Code of Conduct, https://github.com/telekom/nlu-bridge/blob/main/CODE_OF_CONDUCT.md
 Keywords: nlu,intent recognition,natural language understanding,evaluation,performance
-Requires-Python: >=3, <3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: watson
 Provides-Extra: fasttext
 Provides-Extra: luis
 Provides-Extra: rasa2
 Provides-Extra: rasa3
 Provides-Extra: spacy
@@ -44,21 +44,24 @@
 The goal of this project is to provide a unified API to several popular intent recognition
 applications.
 
 ## About this component
 
 ### Installation
 
-The core package including NLUdataset and Baseline vendors can be installed for Python\<=3.8
-using pip
+The core package including NLUdataset and Baseline vendors can be installed for
+Python>=3.8 using pip
 
 ```
 pip install nlubridge
 ```
 
+Note that some vendors come with restrictions regarding the Python version, e.g. Rasa3
+requires Python\<3.11.
+
 To include optional dependencies for the vendors, e.g. Watson Assistant, type
 
 ```
 pip install nlubridge[watson]
 ```
 
 Following install options are available:
```

#### html2text {}

```diff
@@ -1,114 +1,115 @@
-Metadata-Version: 2.1 Name: nlubridge Version: 1.0.1 Summary: Provides a
+Metadata-Version: 2.1 Name: nlubridge Version: 1.0.2 Summary: Provides a
 unified API to several popular intent recognition applications Home-page:
 https://github.com/telekom/nlu-bridge Author: Klaus-Peter Engelbrecht Author-
 email: k.engelbrecht@telekom.de Maintainer: Klaus-Peter Engelbrecht Project-
 URL: Bug Tracker, https://github.com/telekom/nlu-bridge/issues Project-URL:
 Source Code, https://github.com/telekom/nlu-bridge Project-URL: Contributing,
 https://github.com/telekom/nlu-bridge/blob/main/CONTRIBUTING.md Project-URL:
 Code of Conduct, https://github.com/telekom/nlu-bridge/blob/main/
 CODE_OF_CONDUCT.md Keywords: nlu,intent recognition,natural language
-understanding,evaluation,performance Requires-Python: >=3, <3.9 Description-
+understanding,evaluation,performance Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: watson Provides-Extra: fasttext
 Provides-Extra: luis Provides-Extra: rasa2 Provides-Extra: rasa3 Provides-
 Extra: spacy Provides-Extra: huggingface Provides-Extra: develop License-File:
 LICENSE
                        ****** Telekom NLU Bridge ******
   [https://img.shields.io/github/last-commit/telekom/nlu-bridge?style=flat]
 [https://img.shields.io/github/issues/telekom/nlu-bridge?style=flat] [https://
             img.shields.io/badge/License-MIT-green.svg?style=flat]
     Development â¢ Documentation â¢ Support â¢ Contribute â¢ Licensing
 The goal of this project is to provide a unified API to several popular intent
 recognition applications. ## About this component ### Installation The core
 package including NLUdataset and Baseline vendors can be installed for
-Python\<=3.8 using pip ``` pip install nlubridge ``` To include optional
-dependencies for the vendors, e.g. Watson Assistant, type ``` pip install
-nlubridge[watson] ``` Following install options are available: - `watson` -
-`fasttext` - `luis` - `rasa2` - `rasa3` - `spacy` - `huggingface` Development
-tools can be installed with option `develop`. Some vendors require access
-credentials like API tokens, URLs etc. These can be passed on construction of
-the objects. Alternatively, such arguments can be passed as environment
-variables, where the vendor will look for variables named variable
-VENDORNAME_PARAM_NAME. Some vendors require additional dependencies. E.g.,
-Spacy requires a model that can be downloaded (for the model de_core_news_sm)
-with ``` python -m spacy download de_core_news_sm ``` ### Migration from v0
-With realease 1.0.0 we introduce a couple of changes to the names of files and
-vendor classes(see also https://github.com/telekom/nlu-bridge/issues/18). Most
-notably: - datasets.NLUdataset -> nlu_dataset.NluDataset -
-vendors.vendors.Vendor -> - vendors.vendor.Vendor - new supackage `dataloaders`
-that holds all functions for loading data into an NluDataset - new function
-`nlu_dataset.concat` to concatenate NluDatasets passed in a list - can load
-dataloaders, NluDataset, Vendor, OUT_OF_SCOPE_TOKEN, EntityKeys, concat,
-directly from nlubridge like `from nlubridge import Vendor` - Load vendors like
-`from nlubridge.vendors import Rasa3` - former `TelekomModel` now called
-`CharNgramIntentClassifier` - Some vendor names changed for clarity and
-consistency (see "List of supported vendors" for the new names) ### Usage Here
-is an example for the TfidfIntentClassifier: ```python import os import pandas
-as pd from nlubridge.vendors import TfidfIntentClassifier from nlubridge import
-NluDataset dataset = NluDataset(texts, intents) dataset = dataset.shuffle()
-classifier = TfidfIntentClassifier() train, test = dataset.train_test_split
-(test_size=0.25, random_state=0) classifier = classifier.train_intent(train)
-predicted = classifier.test_intent(test) res = pd.DataFrame(list(zip
-(test.intents, predicted)), columns=['true', 'predicted']) ``` If you need to
-configure **stratification**, use the `stratification` parameter (defaults to
-`"intents"` and uses the intents in the dataset as stratification basis;
-whatever _else_ you pass along has to conform to
-`sklearn.model_selection.train_test_split(stratify=)`: ```python train, test =
-dataset.train_test_split(test_size=0.25, random_state=0, stratification=None) #
-deactivate stratification (sklearn default for train_test_split) ``` To compare
-your own vendor or algorithm to existing vendors in this package, you can write
-a Vendor Subclass for your vendor, and possibly a dataloader function. Feel
-free to share your implementation using this repo. Similarly, fixes and
-extensions for the existing vendors are always welcome. ### Logging Most of the
-code uses python logging to report its progress. To get logs printed out to
-console or Jupyter notebook, a logger needs to be configured, before the
-nlutests code. Usually, log messages are on INFO level. This can be configured
-like this: ```python import logging logger = logging.getLogger()
-logger.setLevel(logging.INFO) logger.addHandler(logging.StreamHandler()) ```
-### Concepts / Architecture - **Vendors**\ The [`vendors`](/nlubridge/vendors/
-) subpackage implements standardized interfaces to the specific vendors. A
-specific `Vendor` instance is in charge of dealing with converting the data to
-the required format, uploading data to the cloud if applicable, training models
-and making predictions. - **Datasets**\ The [`nlu_dataset`](/nlubridge/
-nlu_dataset/) module provides a standard interface to NLU data. Data stored in
-different vendor's custom format can be loaded as a dataset and provided to any
-different vendor. - **Data Loaders**\ The [`dataloaders`](/nlubridge/
-dataloaders/) subpackage provides functions to load data that are in a vendor-
-specific format as NluDataset. ### List of supported vendors | Vendor Class |
-Status | Intents | Entities | Algorithm | | ------ | ------ | ------- | -------
-- | --------- | | [TfidfIntentClassifier](/nlubridge/vendors/
-tfidf_intent_classifier.py) | â | â | â | TFIDF on words + SVM | |
-[FastText](https://fasttext.cc) | â | â | â | fasttext | | [Spacy](https:
-//spacy.io/usage/training#section-textcat) | â | â | â | BoW linear + CNN
-| | [WatsonAssistant](https://www.ibm.com/watson/services/conversation/) | â
-| â | â | Propietary (probably LR) | | [Luis](https://www.luis.ai/home) |
-needs testing | â | â | Propietary (probably LR) | |
-[CharNgramIntentClassifier](/nlubridge/vendors/char_ngram_intent_classifier.py)
-| â | â | â | tf-idf on char n-grams + SGD | | [Rasa2](https://
-github.com/RasaHQ/rasa) | â | â | â | configurable | | [Rasa3](https://
-github.com/RasaHQ/rasa) | â | â | â | configurable | ### Features -
-Abstract class for Vendors with convenience methods (ex: scoring and scikit-
-learn compatibility) - Abstract class for datasets with convenience methods
-(ex: train_test_split, indexing, iteration) - Rate limiting to comply with
-cloud providers requirements ## Development _TBD_ ### Build _TBD_ ## Code of
-Conduct This project has adopted the [Contributor Covenant](https://
-www.contributor-covenant.org/) in version 2.0 as our code of conduct. Please
-see the details in our [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md). All
-contributors must abide by the code of conduct. ## Working Language We decided
-to apply _English_ as the primary project language. Consequently, all content
-will be made available primarily in English. We also ask all interested people
-to use English as language to create issues, in their code (comments,
-documentation etc.) and when you send requests to us. The application itself
-and all end-user facing content will be made available in other languages as
-needed. ## Documentation The full documentation for the telekom nlu-bridge can
-be found in _TBD_ ## Support and Feedback The following channels are available
-for discussions, feedback, and support requests: | Type | Channel | | ---------
---------------- | ------------------------------------------------------ | |
-**Issues** | [https://img.shields.io/github/issues/telekom/nlu-
-bridge?style=flat-square]
+Python>=3.8 using pip ``` pip install nlubridge ``` Note that some vendors come
+with restrictions regarding the Python version, e.g. Rasa3 requires
+Python\<3.11. To include optional dependencies for the vendors, e.g. Watson
+Assistant, type ``` pip install nlubridge[watson] ``` Following install options
+are available: - `watson` - `fasttext` - `luis` - `rasa2` - `rasa3` - `spacy` -
+`huggingface` Development tools can be installed with option `develop`. Some
+vendors require access credentials like API tokens, URLs etc. These can be
+passed on construction of the objects. Alternatively, such arguments can be
+passed as environment variables, where the vendor will look for variables named
+variable VENDORNAME_PARAM_NAME. Some vendors require additional dependencies.
+E.g., Spacy requires a model that can be downloaded (for the model
+de_core_news_sm) with ``` python -m spacy download de_core_news_sm ``` ###
+Migration from v0 With realease 1.0.0 we introduce a couple of changes to the
+names of files and vendor classes(see also https://github.com/telekom/nlu-
+bridge/issues/18). Most notably: - datasets.NLUdataset -
+> nlu_dataset.NluDataset - vendors.vendors.Vendor -> - vendors.vendor.Vendor -
+new supackage `dataloaders` that holds all functions for loading data into an
+NluDataset - new function `nlu_dataset.concat` to concatenate NluDatasets
+passed in a list - can load dataloaders, NluDataset, Vendor,
+OUT_OF_SCOPE_TOKEN, EntityKeys, concat, directly from nlubridge like `from
+nlubridge import Vendor` - Load vendors like `from nlubridge.vendors import
+Rasa3` - former `TelekomModel` now called `CharNgramIntentClassifier` - Some
+vendor names changed for clarity and consistency (see "List of supported
+vendors" for the new names) ### Usage Here is an example for the
+TfidfIntentClassifier: ```python import os import pandas as pd from
+nlubridge.vendors import TfidfIntentClassifier from nlubridge import NluDataset
+dataset = NluDataset(texts, intents) dataset = dataset.shuffle() classifier =
+TfidfIntentClassifier() train, test = dataset.train_test_split(test_size=0.25,
+random_state=0) classifier = classifier.train_intent(train) predicted =
+classifier.test_intent(test) res = pd.DataFrame(list(zip(test.intents,
+predicted)), columns=['true', 'predicted']) ``` If you need to configure
+**stratification**, use the `stratification` parameter (defaults to `"intents"`
+and uses the intents in the dataset as stratification basis; whatever _else_
+you pass along has to conform to `sklearn.model_selection.train_test_split
+(stratify=)`: ```python train, test = dataset.train_test_split(test_size=0.25,
+random_state=0, stratification=None) # deactivate stratification (sklearn
+default for train_test_split) ``` To compare your own vendor or algorithm to
+existing vendors in this package, you can write a Vendor Subclass for your
+vendor, and possibly a dataloader function. Feel free to share your
+implementation using this repo. Similarly, fixes and extensions for the
+existing vendors are always welcome. ### Logging Most of the code uses python
+logging to report its progress. To get logs printed out to console or Jupyter
+notebook, a logger needs to be configured, before the nlutests code. Usually,
+log messages are on INFO level. This can be configured like this: ```python
+import logging logger = logging.getLogger() logger.setLevel(logging.INFO)
+logger.addHandler(logging.StreamHandler()) ``` ### Concepts / Architecture -
+**Vendors**\ The [`vendors`](/nlubridge/vendors/) subpackage implements
+standardized interfaces to the specific vendors. A specific `Vendor` instance
+is in charge of dealing with converting the data to the required format,
+uploading data to the cloud if applicable, training models and making
+predictions. - **Datasets**\ The [`nlu_dataset`](/nlubridge/nlu_dataset/
+) module provides a standard interface to NLU data. Data stored in different
+vendor's custom format can be loaded as a dataset and provided to any different
+vendor. - **Data Loaders**\ The [`dataloaders`](/nlubridge/dataloaders/
+) subpackage provides functions to load data that are in a vendor-specific
+format as NluDataset. ### List of supported vendors | Vendor Class | Status |
+Intents | Entities | Algorithm | | ------ | ------ | ------- | -------- | -----
+---- | | [TfidfIntentClassifier](/nlubridge/vendors/tfidf_intent_classifier.py)
+| â | â | â | TFIDF on words + SVM | | [FastText](https://fasttext.cc) |
+â | â | â | fasttext | | [Spacy](https://spacy.io/usage/training#section-
+textcat) | â | â | â | BoW linear + CNN | | [WatsonAssistant](https://
+www.ibm.com/watson/services/conversation/) | â | â | â | Propietary
+(probably LR) | | [Luis](https://www.luis.ai/home) | needs testing | â | â
+| Propietary (probably LR) | | [CharNgramIntentClassifier](/nlubridge/vendors/
+char_ngram_intent_classifier.py) | â | â | â | tf-idf on char n-grams +
+SGD | | [Rasa2](https://github.com/RasaHQ/rasa) | â | â | â |
+configurable | | [Rasa3](https://github.com/RasaHQ/rasa) | â | â | â |
+configurable | ### Features - Abstract class for Vendors with convenience
+methods (ex: scoring and scikit-learn compatibility) - Abstract class for
+datasets with convenience methods (ex: train_test_split, indexing, iteration) -
+Rate limiting to comply with cloud providers requirements ## Development _TBD_
+### Build _TBD_ ## Code of Conduct This project has adopted the [Contributor
+Covenant](https://www.contributor-covenant.org/) in version 2.0 as our code of
+conduct. Please see the details in our [CODE_OF_CONDUCT.md]
+(CODE_OF_CONDUCT.md). All contributors must abide by the code of conduct. ##
+Working Language We decided to apply _English_ as the primary project language.
+Consequently, all content will be made available primarily in English. We also
+ask all interested people to use English as language to create issues, in their
+code (comments, documentation etc.) and when you send requests to us. The
+application itself and all end-user facing content will be made available in
+other languages as needed. ## Documentation The full documentation for the
+telekom nlu-bridge can be found in _TBD_ ## Support and Feedback The following
+channels are available for discussions, feedback, and support requests: | Type
+| Channel | | ------------------------ | --------------------------------------
+---------------- | | **Issues** | [https://img.shields.io/github/issues/
+telekom/nlu-bridge?style=flat-square]
  | | **Other Requests** | [https://img.shields.io/badge/email-
 Open%20Source%20Team-green?logo=mail.ru&style=flat-square&logoColor=white] | ##
 How to Contribute Contribution and feedback is encouraged and always welcome.
 For more information about how to contribute, the project structure, as well as
 additional contribution information, see our [Contribution Guidelines](./
 CONTRIBUTING.md). By participating in this project, you agree to abide by its
 [Code of Conduct](./CODE_OF_CONDUCT.md) at all times. ## Licensing Copyright
```

### Comparing `nlubridge-1.0.1/nlubridge.egg-info/SOURCES.txt` & `nlubridge-1.0.2/nlubridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/setup.py` & `nlubridge-1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,24 +53,24 @@
         "Bug Tracker": source_code + "/issues",
         # "Documentation": "https://telekom.github.io/HPOflow/",
         "Source Code": source_code,
         "Contributing": source_code + "/blob/main/CONTRIBUTING.md",
         "Code of Conduct": source_code + "/blob/main/CODE_OF_CONDUCT.md",
     },
     packages=find_packages(),
-    python_requires=">=3, <3.9",
+    python_requires=">=3.8",
     install_requires=["scikit-learn", "python-dotenv", "lazy-imports", "ratelimit"],
     extras_require={
         "watson": ["ibm_watson", "tqdm", "requests"],
         "fasttext": ["fasttext"],
         "luis": ["requests", "ratelimit"],
-        "rasa2": ["rasa~=2.0", "websockets~=10.4"],
-        "rasa3": ["rasa~=3.0"],
+        "rasa2": ["rasa~=2.8.0", "websockets~=10.4"],
+        "rasa3": ["rasa==3.4.4", "websockets~=10.4"],
         "spacy": ["spacy==3.1.3"],
-        "huggingface": ["datasets~=1.0"],
+        "huggingface": ["datasets~=1.18"],
         "develop": [
             "pytest-cov",
             "pytest-mock",
             "flake8",
             "black",
             "pydocstyle",
             "setuptools",
```

### Comparing `nlubridge-1.0.1/tests/test_dataset_loaders.py` & `nlubridge-1.0.2/tests/test_dataset_loaders.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/tests/test_datasets.py` & `nlubridge-1.0.2/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/tests/test_vendors.py` & `nlubridge-1.0.2/tests/test_vendors.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/tests/test_watson_vendor.py` & `nlubridge-1.0.2/tests/test_watson_vendor.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/tests/test_watson_vendor_mocked.py` & `nlubridge-1.0.2/tests/test_watson_vendor_mocked.py`

 * *Files identical despite different names*

### Comparing `nlubridge-1.0.1/tests/testing_data.py` & `nlubridge-1.0.2/tests/testing_data.py`

 * *Files identical despite different names*

