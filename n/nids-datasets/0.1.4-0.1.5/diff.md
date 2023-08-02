# Comparing `tmp/nids_datasets-0.1.4.tar.gz` & `tmp/nids_datasets-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nids_datasets-0.1.4.tar", last modified: Tue Aug  1 15:52:18 2023, max compression
+gzip compressed data, was "nids_datasets-0.1.5.tar", last modified: Wed Aug  2 19:29:12 2023, max compression
```

## Comparing `nids_datasets-0.1.4.tar` & `nids_datasets-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-08-01 15:52:18.739567 nids_datasets-0.1.4/
--rw-r--r--   0 rdp        (501) staff       (20)     8083 2023-08-01 15:52:18.739398 nids_datasets-0.1.4/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)     7489 2023-07-21 03:51:07.000000 nids_datasets-0.1.4/README.md
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-08-01 15:52:18.738392 nids_datasets-0.1.4/nids_datasets/
--rw-r--r--   0 rdp        (501) staff       (20)       41 2023-07-17 06:28:22.000000 nids_datasets-0.1.4/nids_datasets/__init__.py
--rw-r--r--   0 rdp        (501) staff       (20)    12966 2023-08-01 15:34:32.000000 nids_datasets-0.1.4/nids_datasets/dataset.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-08-01 15:52:18.739195 nids_datasets-0.1.4/nids_datasets.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)     8083 2023-08-01 15:52:18.000000 nids_datasets-0.1.4/nids_datasets.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      253 2023-08-01 15:52:18.000000 nids_datasets-0.1.4/nids_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-08-01 15:52:18.000000 nids_datasets-0.1.4/nids_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)       98 2023-08-01 15:52:18.000000 nids_datasets-0.1.4/nids_datasets.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       14 2023-08-01 15:52:18.000000 nids_datasets-0.1.4/nids_datasets.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-08-01 15:52:18.739616 nids_datasets-0.1.4/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      967 2023-08-01 15:52:04.000000 nids_datasets-0.1.4/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-08-02 19:29:12.356304 nids_datasets-0.1.5/
+-rw-r--r--   0 rdp        (501) staff       (20)     9000 2023-08-02 19:29:12.356108 nids_datasets-0.1.5/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)     8406 2023-08-02 19:28:47.000000 nids_datasets-0.1.5/README.md
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-08-02 19:29:12.355118 nids_datasets-0.1.5/nids_datasets/
+-rw-r--r--   0 rdp        (501) staff       (20)       41 2023-07-17 06:28:22.000000 nids_datasets-0.1.5/nids_datasets/__init__.py
+-rw-r--r--   0 rdp        (501) staff       (20)    13122 2023-08-02 19:11:04.000000 nids_datasets-0.1.5/nids_datasets/dataset.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-08-02 19:29:12.355902 nids_datasets-0.1.5/nids_datasets.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)     9000 2023-08-02 19:29:12.000000 nids_datasets-0.1.5/nids_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      253 2023-08-02 19:29:12.000000 nids_datasets-0.1.5/nids_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-08-02 19:29:12.000000 nids_datasets-0.1.5/nids_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       98 2023-08-02 19:29:12.000000 nids_datasets-0.1.5/nids_datasets.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       14 2023-08-02 19:29:12.000000 nids_datasets-0.1.5/nids_datasets.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-08-02 19:29:12.356350 nids_datasets-0.1.5/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      967 2023-08-02 19:29:06.000000 nids_datasets-0.1.5/setup.py
```

### Comparing `nids_datasets-0.1.4/PKG-INFO` & `nids_datasets-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nids_datasets
-Version: 0.1.4
+Version: 0.1.5
 Summary: Download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets
 Home-page: https://github.com/rdpahalavan/nids-datasets
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: Apache License 2.0
 Keywords: Dataset NIDS UNSW-NB15 CIC-IDS2017
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 
 # NIDS Datasets
 
-The `nids-datasets` package provides functionality to download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets. These datasets, which initially were only flow datasets, have been enhanced to include packet-level information from the raw PCAP files. The dataset contains both packet-level and flow-level data for over 230 million packets, with 179 million packets from UNSW-NB15 and 54 million packets from CIC-IDS2017.
+The `nids-datasets` package provides functionality to download and utilize specially curated and extracted datasets from the original CIC-IDS2017 and UNSW-NB15 datasets. These datasets, which initially were only flow datasets, have been enhanced to include packet-level information from the raw PCAP files. The dataset contains both packet-level and flow-level data for over 230 million packets, with 179 million packets from UNSW-NB15 and 54 million packets from CIC-IDS2017.
 
 ## Installation
 
 Install the `nids-datasets` package using pip:
 
 ```shell
 pip install nids-datasets
@@ -168,28 +168,47 @@
     ├───Payload_Bytes_File_3.parquet
     ├───Payload_Bytes_File_5.parquet
     └───Payload_Bytes_File_10.parquet
 ```
 
 ## Reading the Datasets
 
-The `read()` method allows you to read files using Hugging Face's `load_dataset` method, one subset at a time. The dataset and files parameters are optional if the same details are used to instantiate the `Dataset` class.
+The `read()` method allows you to read files using Hugging Face's [`load_dataset`](https://huggingface.co/docs/datasets/loading) method, one subset at a time. This method can be used directly without the `download()` method, as downloading happens automatically. The dataset and files parameters are optional if the same details are used to instantiate the `Dataset` class.
 
 ```python
 dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2])
 ```
 
 The `read()` method returns a dataset that you can convert to a pandas dataframe or save to a CSV, parquet, or any other desired file format:
 
 ```python
 df = dataset.to_pandas()
 dataset.to_csv('file_path_to_save.csv')
 dataset.to_parquet('file_path_to_save.parquet')
 ```
 
+To get specific packets using their index, you can use the `packets` parameter.
+
+```python
+dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], packets='100:600')
+# This will return 100th packet to 599th packet (total of 500 packets)
+
+dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], packets=':10%')
+# This will return the first 10 percent of packets.
+
+dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], packets='20%:30%')
+# This will return the packets from 20th percent to 30th percent.
+```
+
+To use multiprocessing, pass how many processes to use in the `num_proc` parameter.
+
+```python
+dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], num_proc=2)
+```
+
 For scenarios where you want to process one packet at a time, you can use the `stream=True` parameter:
 
 ```python
 dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], stream=True)
 print(next(iter(dataset)))
 ```
```

### Comparing `nids_datasets-0.1.4/README.md` & `nids_datasets-0.1.5/nids_datasets.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,25 @@
+Metadata-Version: 2.1
+Name: nids-datasets
+Version: 0.1.5
+Summary: Download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets
+Home-page: https://github.com/rdpahalavan/nids-datasets
+Author: Pahalavan R D
+Author-email: rdpahalavan24@gmail.com
+License: Apache License 2.0
+Keywords: Dataset NIDS UNSW-NB15 CIC-IDS2017
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+
 # NIDS Datasets
 
-The `nids-datasets` package provides functionality to download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets. These datasets, which initially were only flow datasets, have been enhanced to include packet-level information from the raw PCAP files. The dataset contains both packet-level and flow-level data for over 230 million packets, with 179 million packets from UNSW-NB15 and 54 million packets from CIC-IDS2017.
+The `nids-datasets` package provides functionality to download and utilize specially curated and extracted datasets from the original CIC-IDS2017 and UNSW-NB15 datasets. These datasets, which initially were only flow datasets, have been enhanced to include packet-level information from the raw PCAP files. The dataset contains both packet-level and flow-level data for over 230 million packets, with 179 million packets from UNSW-NB15 and 54 million packets from CIC-IDS2017.
 
 ## Installation
 
 Install the `nids-datasets` package using pip:
 
 ```shell
 pip install nids-datasets
@@ -153,28 +168,47 @@
     ├───Payload_Bytes_File_3.parquet
     ├───Payload_Bytes_File_5.parquet
     └───Payload_Bytes_File_10.parquet
 ```
 
 ## Reading the Datasets
 
-The `read()` method allows you to read files using Hugging Face's `load_dataset` method, one subset at a time. The dataset and files parameters are optional if the same details are used to instantiate the `Dataset` class.
+The `read()` method allows you to read files using Hugging Face's [`load_dataset`](https://huggingface.co/docs/datasets/loading) method, one subset at a time. This method can be used directly without the `download()` method, as downloading happens automatically. The dataset and files parameters are optional if the same details are used to instantiate the `Dataset` class.
 
 ```python
 dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2])
 ```
 
 The `read()` method returns a dataset that you can convert to a pandas dataframe or save to a CSV, parquet, or any other desired file format:
 
 ```python
 df = dataset.to_pandas()
 dataset.to_csv('file_path_to_save.csv')
 dataset.to_parquet('file_path_to_save.parquet')
 ```
 
+To get specific packets using their index, you can use the `packets` parameter.
+
+```python
+dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], packets='100:600')
+# This will return 100th packet to 599th packet (total of 500 packets)
+
+dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], packets=':10%')
+# This will return the first 10 percent of packets.
+
+dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], packets='20%:30%')
+# This will return the packets from 20th percent to 30th percent.
+```
+
+To use multiprocessing, pass how many processes to use in the `num_proc` parameter.
+
+```python
+dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], num_proc=2)
+```
+
 For scenarios where you want to process one packet at a time, you can use the `stream=True` parameter:
 
 ```python
 dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], stream=True)
 print(next(iter(dataset)))
 ```
```

### Comparing `nids_datasets-0.1.4/nids_datasets/dataset.py` & `nids_datasets-0.1.5/nids_datasets/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,18 +106,22 @@
             df_final = pd.concat([df[['packet_id', 'flow_id', 'source_ip', 'source_port', 'destination_ip',
                                       'destination_port', 'protocol']], df_final], axis=1)
             df_final['attack_label'] = df['attack_label']
             df_final.to_parquet(f"{self.dataset}/{col_name.split('_')[0].capitalize()}-Bytes-{max_bytes}/{col_name.split('_')[0].capitalize()}_Bytes_File_{file}.parquet", index=False)
             del df_final
             del df
 
-    def read(self, dataset=None, subset=None, files=None, stream=False):
+    def read(self, dataset=None, subset=None, files=None, packets=None, num_proc=None, stream=False):
         if dataset is None:
             dataset = self.dataset
         if subset is None:
             subset = self.subset[0]
         if files is None:
             files = self.files
+        if packets is None:
+            split = 'train'
+        else:
+            split = f'train[{packets}]'
         files = [f"{subset.replace('-', '_')}_File_{file}.parquet" for file in files]
-        dataset = load_dataset(path=f"rdpahalavan/{dataset}", data_dir=subset, data_files=files, split='train',
+        dataset = load_dataset(path=f"rdpahalavan/{dataset}", data_dir=subset, data_files=files, split=split, num_proc=num_proc,
                                streaming=stream)
         return dataset
```

### Comparing `nids_datasets-0.1.4/nids_datasets.egg-info/PKG-INFO` & `nids_datasets-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,10 @@
-Metadata-Version: 2.1
-Name: nids-datasets
-Version: 0.1.4
-Summary: Download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets
-Home-page: https://github.com/rdpahalavan/nids-datasets
-Author: Pahalavan R D
-Author-email: rdpahalavan24@gmail.com
-License: Apache License 2.0
-Keywords: Dataset NIDS UNSW-NB15 CIC-IDS2017
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-
 # NIDS Datasets
 
-The `nids-datasets` package provides functionality to download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets. These datasets, which initially were only flow datasets, have been enhanced to include packet-level information from the raw PCAP files. The dataset contains both packet-level and flow-level data for over 230 million packets, with 179 million packets from UNSW-NB15 and 54 million packets from CIC-IDS2017.
+The `nids-datasets` package provides functionality to download and utilize specially curated and extracted datasets from the original CIC-IDS2017 and UNSW-NB15 datasets. These datasets, which initially were only flow datasets, have been enhanced to include packet-level information from the raw PCAP files. The dataset contains both packet-level and flow-level data for over 230 million packets, with 179 million packets from UNSW-NB15 and 54 million packets from CIC-IDS2017.
 
 ## Installation
 
 Install the `nids-datasets` package using pip:
 
 ```shell
 pip install nids-datasets
@@ -168,28 +153,47 @@
     ├───Payload_Bytes_File_3.parquet
     ├───Payload_Bytes_File_5.parquet
     └───Payload_Bytes_File_10.parquet
 ```
 
 ## Reading the Datasets
 
-The `read()` method allows you to read files using Hugging Face's `load_dataset` method, one subset at a time. The dataset and files parameters are optional if the same details are used to instantiate the `Dataset` class.
+The `read()` method allows you to read files using Hugging Face's [`load_dataset`](https://huggingface.co/docs/datasets/loading) method, one subset at a time. This method can be used directly without the `download()` method, as downloading happens automatically. The dataset and files parameters are optional if the same details are used to instantiate the `Dataset` class.
 
 ```python
 dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2])
 ```
 
 The `read()` method returns a dataset that you can convert to a pandas dataframe or save to a CSV, parquet, or any other desired file format:
 
 ```python
 df = dataset.to_pandas()
 dataset.to_csv('file_path_to_save.csv')
 dataset.to_parquet('file_path_to_save.parquet')
 ```
 
+To get specific packets using their index, you can use the `packets` parameter.
+
+```python
+dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], packets='100:600')
+# This will return 100th packet to 599th packet (total of 500 packets)
+
+dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], packets=':10%')
+# This will return the first 10 percent of packets.
+
+dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], packets='20%:30%')
+# This will return the packets from 20th percent to 30th percent.
+```
+
+To use multiprocessing, pass how many processes to use in the `num_proc` parameter.
+
+```python
+dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], num_proc=2)
+```
+
 For scenarios where you want to process one packet at a time, you can use the `stream=True` parameter:
 
 ```python
 dataset = data.read(dataset='UNSW-NB15', subset='Packet-Fields', files=[1,2], stream=True)
 print(next(iter(dataset)))
 ```
```

### Comparing `nids_datasets-0.1.4/setup.py` & `nids_datasets-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='nids_datasets',
-    version='0.1.4',
+    version='0.1.5',
     description="Download and utilize specially curated and extracted datasets from the original UNSW-NB15 and CIC-IDS2017 datasets",
     keywords="Dataset NIDS UNSW-NB15 CIC-IDS2017",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

