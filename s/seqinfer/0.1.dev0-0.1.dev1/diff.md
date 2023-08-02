# Comparing `tmp/seqinfer-0.1.dev0.tar.gz` & `tmp/seqinfer-0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqinfer-0.1.dev0.tar", max compression
+gzip compressed data, was "seqinfer-0.1.dev1.tar", max compression
```

## Comparing `seqinfer-0.1.dev0.tar` & `seqinfer-0.1.dev1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1068 2023-08-02 19:02:18.329223 seqinfer-0.1.dev0/LICENSE
--rw-r--r--   0        0        0     3517 2023-07-22 00:12:05.271579 seqinfer-0.1.dev0/README.md
--rw-r--r--   0        0        0      895 2023-08-02 19:18:01.926341 seqinfer-0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 04:19:02.460114 seqinfer-0.1.dev0/src/seqinfer/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 18:21:00.782218 seqinfer-0.1.dev0/src/seqinfer/infer/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 02:29:59.411139 seqinfer-0.1.dev0/src/seqinfer/infer/classifiers.py
--rw-r--r--   0        0        0        0 2023-07-21 04:53:31.047407 seqinfer-0.1.dev0/src/seqinfer/infer/components/__init__.py
--rw-r--r--   0        0        0     3795 2023-07-21 20:17:32.615013 seqinfer-0.1.dev0/src/seqinfer/infer/components/architectures.py
--rw-r--r--   0        0        0        0 2023-07-21 02:22:21.831912 seqinfer-0.1.dev0/src/seqinfer/infer/components/callbacks.py
--rw-r--r--   0        0        0        0 2023-07-21 02:22:04.793339 seqinfer-0.1.dev0/src/seqinfer/infer/components/losses.py
--rw-r--r--   0        0        0        0 2023-07-21 02:31:36.439829 seqinfer-0.1.dev0/src/seqinfer/infer/decoders.py
--rw-r--r--   0        0        0      159 2023-08-02 19:08:09.972600 seqinfer-0.1.dev0/src/seqinfer/infer/encoders.py
--rw-r--r--   0        0        0        0 2023-07-21 02:30:13.083990 seqinfer-0.1.dev0/src/seqinfer/infer/regressors.py
--rw-r--r--   0        0        0        0 2023-07-09 18:20:57.571447 seqinfer-0.1.dev0/src/seqinfer/seq/__init__.py
--rw-r--r--   0        0        0     3620 2023-07-13 04:17:19.275984 seqinfer-0.1.dev0/src/seqinfer/seq/datasets.py
--rw-r--r--   0        0        0    20675 2023-07-21 23:53:51.417615 seqinfer-0.1.dev0/src/seqinfer/seq/transforms.py
--rw-r--r--   0        0        0     2053 2023-07-18 03:19:24.298702 seqinfer-0.1.dev0/src/seqinfer/seq/vocabularies.py
--rw-r--r--   0        0        0        0 2023-07-11 18:37:40.047448 seqinfer-0.1.dev0/src/seqinfer/utils/__init__.py
--rw-r--r--   0        0        0     1899 2023-07-17 05:35:14.525428 seqinfer-0.1.dev0/src/seqinfer/utils/logger.py
--rw-r--r--   0        0        0     1205 2023-07-21 03:50:53.927911 seqinfer-0.1.dev0/src/seqinfer/utils/misc.py
--rw-r--r--   0        0        0      683 2023-07-11 18:37:35.604989 seqinfer-0.1.dev0/src/seqinfer/utils/seq_utils.py
--rw-r--r--   0        0        0     4180 1970-01-01 00:00:00.000000 seqinfer-0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-02 19:02:18.329223 seqinfer-0.1.dev1/LICENSE
+-rw-r--r--   0        0        0     3342 2023-08-02 19:45:11.424623 seqinfer-0.1.dev1/README.md
+-rw-r--r--   0        0        0      895 2023-08-02 19:48:37.091427 seqinfer-0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 04:19:02.460114 seqinfer-0.1.dev1/src/seqinfer/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:21:00.782218 seqinfer-0.1.dev1/src/seqinfer/infer/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 02:29:59.411139 seqinfer-0.1.dev1/src/seqinfer/infer/classifiers.py
+-rw-r--r--   0        0        0        0 2023-07-21 04:53:31.047407 seqinfer-0.1.dev1/src/seqinfer/infer/components/__init__.py
+-rw-r--r--   0        0        0     3795 2023-07-21 20:17:32.615013 seqinfer-0.1.dev1/src/seqinfer/infer/components/architectures.py
+-rw-r--r--   0        0        0        0 2023-07-21 02:22:21.831912 seqinfer-0.1.dev1/src/seqinfer/infer/components/callbacks.py
+-rw-r--r--   0        0        0        0 2023-07-21 02:22:04.793339 seqinfer-0.1.dev1/src/seqinfer/infer/components/losses.py
+-rw-r--r--   0        0        0        0 2023-07-21 02:31:36.439829 seqinfer-0.1.dev1/src/seqinfer/infer/decoders.py
+-rw-r--r--   0        0        0      159 2023-08-02 19:08:09.972600 seqinfer-0.1.dev1/src/seqinfer/infer/encoders.py
+-rw-r--r--   0        0        0        0 2023-07-21 02:30:13.083990 seqinfer-0.1.dev1/src/seqinfer/infer/regressors.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:20:57.571447 seqinfer-0.1.dev1/src/seqinfer/seq/__init__.py
+-rw-r--r--   0        0        0     3620 2023-07-13 04:17:19.275984 seqinfer-0.1.dev1/src/seqinfer/seq/datasets.py
+-rw-r--r--   0        0        0    20675 2023-07-21 23:53:51.417615 seqinfer-0.1.dev1/src/seqinfer/seq/transforms.py
+-rw-r--r--   0        0        0     2053 2023-07-18 03:19:24.298702 seqinfer-0.1.dev1/src/seqinfer/seq/vocabularies.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:37:40.047448 seqinfer-0.1.dev1/src/seqinfer/utils/__init__.py
+-rw-r--r--   0        0        0     1899 2023-07-17 05:35:14.525428 seqinfer-0.1.dev1/src/seqinfer/utils/logger.py
+-rw-r--r--   0        0        0     1205 2023-07-21 03:50:53.927911 seqinfer-0.1.dev1/src/seqinfer/utils/misc.py
+-rw-r--r--   0        0        0      683 2023-07-11 18:37:35.604989 seqinfer-0.1.dev1/src/seqinfer/utils/seq_utils.py
+-rw-r--r--   0        0        0     4005 1970-01-01 00:00:00.000000 seqinfer-0.1.dev1/PKG-INFO
```

### Comparing `seqinfer-0.1.dev0/LICENSE` & `seqinfer-0.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `seqinfer-0.1.dev0/README.md` & `seqinfer-0.1.dev1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,49 +18,31 @@
 -   [Usage](README.md#usage)
 -   [Project Structure](README.md#project-structure)
 -   [Examples](README.md#examples)
 -   [Contributing](README.md#contributing)
 -   [License](README.md#license)
 
 ## Installation
-
-
-1. Clone seqinfer repository
-```
-git clone https://github.com/jiajiexiao/seqinfer.git
-cd seqinfer/
-```
-
-2. Install in development mode
-### Install in “develop” or “editable” mode:
-```
-python setup.py develop
-```
-or
-```
-pip install -e ./
-```
-
-
-<!-- You can install SeqInfer using pip:
-
-`pip install seqinfer`  -->
+You can install `SeqInfer` using pip:
+`pip install seqinfer` 
+Or 
+`pip install git+https://github.com/jiajiexiao/seqinfer.git`
 
 ## Usage
 
 To use SeqInfer, simply import the desired modules from the `seqs` and `learners` sub-packages.
 
 For example, you can prepare the data as below: 
 ```python
 from seqinfer.seq.datasets import SeqFromFileDataset
 from seqinfer.seq.transforms import Compose, KmerTokenizer, OneHotEncoder, ToTensor
 from seqinfer.seq.vocabularies import unambiguous_dna_vocabulary_dict
 
 seq_dataset = SeqFromFileDataset(
-    seq_file="examples/aptamers/pos.fasta",
+    seq_file="examples/toys/CCA-TXXAGG-AG-TGG-TC-A-T/pos.fasta",
     seq_file_fmt="fasta",
     transform_sequences=Compose(
         [
             KmerTokenizer(
                 k=1,
                 stride=1,
                 vocab_dict=unambiguous_dna_vocabulary_dict,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `seqinfer-0.1.dev0/pyproject.toml` & `seqinfer-0.1.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seqinfer"
-version = "0.1.dev0"
+version = "0.1.dev1"
 description = "A Python library for sequence inference."
 authors = ["jjxiao <jiajiexiao@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `seqinfer-0.1.dev0/src/seqinfer/infer/components/architectures.py` & `seqinfer-0.1.dev1/src/seqinfer/infer/components/architectures.py`

 * *Files identical despite different names*

### Comparing `seqinfer-0.1.dev0/src/seqinfer/seq/datasets.py` & `seqinfer-0.1.dev1/src/seqinfer/seq/datasets.py`

 * *Files identical despite different names*

### Comparing `seqinfer-0.1.dev0/src/seqinfer/seq/transforms.py` & `seqinfer-0.1.dev1/src/seqinfer/seq/transforms.py`

 * *Files identical despite different names*

### Comparing `seqinfer-0.1.dev0/src/seqinfer/seq/vocabularies.py` & `seqinfer-0.1.dev1/src/seqinfer/seq/vocabularies.py`

 * *Files identical despite different names*

### Comparing `seqinfer-0.1.dev0/src/seqinfer/utils/logger.py` & `seqinfer-0.1.dev1/src/seqinfer/utils/logger.py`

 * *Files identical despite different names*

### Comparing `seqinfer-0.1.dev0/src/seqinfer/utils/misc.py` & `seqinfer-0.1.dev1/src/seqinfer/utils/misc.py`

 * *Files identical despite different names*

### Comparing `seqinfer-0.1.dev0/src/seqinfer/utils/seq_utils.py` & `seqinfer-0.1.dev1/src/seqinfer/utils/seq_utils.py`

 * *Files identical despite different names*

### Comparing `seqinfer-0.1.dev0/PKG-INFO` & `seqinfer-0.1.dev1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqinfer
-Version: 0.1.dev0
+Version: 0.1.dev1
 Summary: A Python library for sequence inference.
 License: MIT
 Author: jjxiao
 Author-email: jiajiexiao@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,49 +37,31 @@
 -   [Usage](README.md#usage)
 -   [Project Structure](README.md#project-structure)
 -   [Examples](README.md#examples)
 -   [Contributing](README.md#contributing)
 -   [License](README.md#license)
 
 ## Installation
-
-
-1. Clone seqinfer repository
-```
-git clone https://github.com/jiajiexiao/seqinfer.git
-cd seqinfer/
-```
-
-2. Install in development mode
-### Install in “develop” or “editable” mode:
-```
-python setup.py develop
-```
-or
-```
-pip install -e ./
-```
-
-
-<!-- You can install SeqInfer using pip:
-
-`pip install seqinfer`  -->
+You can install `SeqInfer` using pip:
+`pip install seqinfer` 
+Or 
+`pip install git+https://github.com/jiajiexiao/seqinfer.git`
 
 ## Usage
 
 To use SeqInfer, simply import the desired modules from the `seqs` and `learners` sub-packages.
 
 For example, you can prepare the data as below: 
 ```python
 from seqinfer.seq.datasets import SeqFromFileDataset
 from seqinfer.seq.transforms import Compose, KmerTokenizer, OneHotEncoder, ToTensor
 from seqinfer.seq.vocabularies import unambiguous_dna_vocabulary_dict
 
 seq_dataset = SeqFromFileDataset(
-    seq_file="examples/aptamers/pos.fasta",
+    seq_file="examples/toys/CCA-TXXAGG-AG-TGG-TC-A-T/pos.fasta",
     seq_file_fmt="fasta",
     transform_sequences=Compose(
         [
             KmerTokenizer(
                 k=1,
                 stride=1,
                 vocab_dict=unambiguous_dna_vocabulary_dict,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

