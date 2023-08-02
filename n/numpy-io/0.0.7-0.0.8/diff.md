# Comparing `tmp/numpy_io-0.0.7-py3-none-any.whl.zip` & `tmp/numpy_io-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,32 +1,40 @@
-Zip file size: 27451 bytes, number of entries: 30
+Zip file size: 34641 bytes, number of entries: 38
+-rw-rw-rw-  2.0 fat       39 b- defN 23-Apr-27 06:30 numpy_io/.gitignore
+-rw-rw-rw-  2.0 fat     1662 b- defN 23-Aug-02 02:23 numpy_io/README.MD
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Apr-27 06:30 numpy_io/__init__.py
--rw-rw-rw-  2.0 fat      629 b- defN 23-Jul-10 07:47 numpy_io/setup.py
 -rw-rw-rw-  2.0 fat       80 b- defN 23-Apr-27 06:30 numpy_io/core/__init__.py
 -rw-rw-rw-  2.0 fat    19587 b- defN 23-Jul-10 07:41 numpy_io/core/numpyadapter.py
--rw-rw-rw-  2.0 fat     5619 b- defN 23-Jul-10 07:52 numpy_io/core/parallel.py
+-rw-rw-rw-  2.0 fat     5578 b- defN 23-Jul-13 00:58 numpy_io/core/parallel.py
 -rw-rw-rw-  2.0 fat     1894 b- defN 23-Apr-27 06:30 numpy_io/core/reader.py
 -rw-rw-rw-  2.0 fat     2268 b- defN 23-Jul-10 07:54 numpy_io/core/writer.py
+-rw-rw-rw-  2.0 fat     9635 b- defN 23-Apr-27 08:53 numpy_io/examples/README.md
 -rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-27 06:30 numpy_io/examples/__init__.py
 -rw-rw-rw-  2.0 fat     3236 b- defN 23-Jul-03 23:35 numpy_io/examples/auto_parallel_writer.py
 -rw-rw-rw-  2.0 fat     3241 b- defN 23-Apr-27 06:30 numpy_io/examples/auto_writer.py
+-rw-rw-rw-  2.0 fat     2313 b- defN 23-Jul-10 08:00 numpy_io/examples/demo_arrow_writer.py
+-rw-rw-rw-  2.0 fat     1378 b- defN 23-Jul-06 04:42 numpy_io/examples/demo_arrow_writer2.py
+-rw-rw-rw-  2.0 fat     2183 b- defN 23-Jul-10 08:00 numpy_io/examples/demo_parquet_writer.py
 -rw-rw-rw-  2.0 fat     1778 b- defN 23-Apr-27 07:23 numpy_io/examples/leveldb_readwriter_example.py
 -rw-rw-rw-  2.0 fat     2218 b- defN 23-Apr-28 00:25 numpy_io/examples/lmdb_readwriter_example.py
 -rw-rw-rw-  2.0 fat     1198 b- defN 23-Apr-27 06:30 numpy_io/examples/memory_raw_readwriter_example.py
 -rw-rw-rw-  2.0 fat     1285 b- defN 23-Apr-27 06:30 numpy_io/examples/memory_readwriter_example.py
 -rw-rw-rw-  2.0 fat     1586 b- defN 23-Apr-27 06:30 numpy_io/examples/record_numpywriter_example.py
 -rw-rw-rw-  2.0 fat     1353 b- defN 23-Apr-27 06:30 numpy_io/examples/record_reader_example.py
 -rw-rw-rw-  2.0 fat     1398 b- defN 23-Apr-27 06:30 numpy_io/examples/record_shuffle_example.py
 -rw-rw-rw-  2.0 fat     3056 b- defN 23-Apr-27 06:30 numpy_io/examples/record_writer_example.py
 -rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-27 06:30 numpy_io/examples/testing/__init__.py
+-rw-rw-rw-  2.0 fat     2313 b- defN 23-Jul-10 08:00 numpy_io/examples/testing/demo_arrow_writer.py
+-rw-rw-rw-  2.0 fat     1378 b- defN 23-Jul-06 04:42 numpy_io/examples/testing/demo_arrow_writer2.py
+-rw-rw-rw-  2.0 fat     2183 b- defN 23-Jul-10 08:00 numpy_io/examples/testing/demo_parquet_writer.py
 -rw-rw-rw-  2.0 fat     2658 b- defN 23-Apr-27 06:30 numpy_io/examples/testing/lmdb_test.py
 -rw-rw-rw-  2.0 fat      613 b- defN 23-Apr-27 06:30 numpy_io/examples/testing/test_mem.py
 -rw-rw-rw-  2.0 fat     2907 b- defN 23-Apr-27 07:08 numpy_io/examples/testing/test_mutiprocess.py
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Apr-28 00:25 numpy_io/pytorch_loader/__init__.py
--rw-rw-rw-  2.0 fat    10309 b- defN 23-Jul-04 03:24 numpy_io/pytorch_loader/data_helper.py
--rw-rw-rw-  2.0 fat     8940 b- defN 23-Jul-04 01:02 numpy_io/pytorch_loader/dataloaders.py
--rw-rw-rw-  2.0 fat     3780 b- defN 23-May-25 05:42 numpy_io/pytorch_loader/tokenizer_config_helper.py
--rw-rw-rw-  2.0 fat      390 b- defN 23-Jul-10 07:55 numpy_io-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-10 07:55 numpy_io-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-10 07:55 numpy_io-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2715 b- defN 23-Jul-10 07:55 numpy_io-0.0.7.dist-info/RECORD
-30 files, 83099 bytes uncompressed, 22999 bytes compressed:  72.3%
+-rw-rw-rw-  2.0 fat    10310 b- defN 23-Aug-02 02:31 numpy_io/pytorch_loader/data_helper.py
+-rw-rw-rw-  2.0 fat     8942 b- defN 23-Aug-02 02:33 numpy_io/pytorch_loader/dataloaders.py
+-rw-rw-rw-  2.0 fat     3824 b- defN 23-Jul-13 00:58 numpy_io/pytorch_loader/tokenizer_config_helper.py
+-rw-rw-rw-  2.0 fat      388 b- defN 23-Aug-02 02:35 numpy_io-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-02 02:35 numpy_io-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Aug-02 02:35 numpy_io-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     3475 b- defN 23-Aug-02 02:35 numpy_io-0.0.8.dist-info/RECORD
+38 files, 106318 bytes uncompressed, 28971 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -1,11 +1,14 @@
-Filename: numpy_io/__init__.py
+Filename: numpy_io/.gitignore
 Comment: 
 
-Filename: numpy_io/setup.py
+Filename: numpy_io/README.MD
+Comment: 
+
+Filename: numpy_io/__init__.py
 Comment: 
 
 Filename: numpy_io/core/__init__.py
 Comment: 
 
 Filename: numpy_io/core/numpyadapter.py
 Comment: 
@@ -15,23 +18,35 @@
 
 Filename: numpy_io/core/reader.py
 Comment: 
 
 Filename: numpy_io/core/writer.py
 Comment: 
 
+Filename: numpy_io/examples/README.md
+Comment: 
+
 Filename: numpy_io/examples/__init__.py
 Comment: 
 
 Filename: numpy_io/examples/auto_parallel_writer.py
 Comment: 
 
 Filename: numpy_io/examples/auto_writer.py
 Comment: 
 
+Filename: numpy_io/examples/demo_arrow_writer.py
+Comment: 
+
+Filename: numpy_io/examples/demo_arrow_writer2.py
+Comment: 
+
+Filename: numpy_io/examples/demo_parquet_writer.py
+Comment: 
+
 Filename: numpy_io/examples/leveldb_readwriter_example.py
 Comment: 
 
 Filename: numpy_io/examples/lmdb_readwriter_example.py
 Comment: 
 
 Filename: numpy_io/examples/memory_raw_readwriter_example.py
@@ -51,14 +66,23 @@
 
 Filename: numpy_io/examples/record_writer_example.py
 Comment: 
 
 Filename: numpy_io/examples/testing/__init__.py
 Comment: 
 
+Filename: numpy_io/examples/testing/demo_arrow_writer.py
+Comment: 
+
+Filename: numpy_io/examples/testing/demo_arrow_writer2.py
+Comment: 
+
+Filename: numpy_io/examples/testing/demo_parquet_writer.py
+Comment: 
+
 Filename: numpy_io/examples/testing/lmdb_test.py
 Comment: 
 
 Filename: numpy_io/examples/testing/test_mem.py
 Comment: 
 
 Filename: numpy_io/examples/testing/test_mutiprocess.py
@@ -72,20 +96,20 @@
 
 Filename: numpy_io/pytorch_loader/dataloaders.py
 Comment: 
 
 Filename: numpy_io/pytorch_loader/tokenizer_config_helper.py
 Comment: 
 
-Filename: numpy_io-0.0.7.dist-info/METADATA
+Filename: numpy_io-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: numpy_io-0.0.7.dist-info/WHEEL
+Filename: numpy_io-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: numpy_io-0.0.7.dist-info/top_level.txt
+Filename: numpy_io-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: numpy_io-0.0.7.dist-info/RECORD
+Filename: numpy_io-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## numpy_io/core/parallel.py

```diff
@@ -137,15 +137,15 @@
             ids = tqdm(ids, total=total, desc=parallel_node.desc if parallel_node.desc else 'parallel_apply')
         except:
             ...
 
 
 
     #生成消费都是多进程
-    if parallel_node.num_process_worker > 0 and parallel_node.num_process_worker > 0:
+    if parallel_node.num_process_worker > 0:
         pools = []
         for _ in range(parallel_node.num_process_worker):
             p = Process(target=produce_input,
                         args= (q_in,
                                q_out,
                                parallel_node.on_input_startup,
                                parallel_node.on_input_process,
```

## numpy_io/pytorch_loader/data_helper.py

```diff
@@ -147,30 +147,30 @@
                 leveldb_write_buffer_size = leveldb_write_buffer_size,
                 leveldb_max_file_size =leveldb_max_file_size,
                 lmdb_map_size = lmdb_map_size,
                 batch_size = batch_size)
         #写数据完成
         self.on_data_finalize()
 
-        # 返回制作特征数据的中间文件
-
+    # 返回制作特征数据的中间文件
     def get_intermediate_file(self, intermediate_name, mode):
         if self.backend.startswith('memory'):
             # 内存数据: list
             intermediate_output = []
             logging.info('make data {} {}...'.format(self.cache_dir,
                                                      intermediate_name + '-' + mode + '.' + self.backend))
         else:
             # 本地文件数据: 文件名
             intermediate_output = os.path.join(self.cache_dir,
                                                intermediate_name + '-' + mode + '.' + self.backend)
             logging.info('make data {}...'.format(intermediate_output))
         return intermediate_output
 
-    def make_dataset_with_args(self, input_files,
+    def make_dataset_with_args(self,
+                               input_files,
                                mode,
                                shuffle=False,
                                num_process_worker: int = 0,
                                overwrite: bool = False,
                                mixed_data=True,
                                dupe_factor=1,
                                **dataset_args):
@@ -230,45 +230,28 @@
                 for input_item in input_files:
                     contain_objs.append(input_item)
 
 
 
 
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
 def make_dataset(data: typing.List,
-               input_fn:typing.Callable[[int,typing.Any,tuple],typing.Union[typing.Dict,typing.List,typing.Tuple]],
-               input_fn_args:typing.Tuple,
-               outfile:str,
-               backend: str,
-               overwrite = False,
-               num_process_worker:int = 8,
-               options=None,
-               parquet_options=None,
-               schema=None,
-               leveldb_write_buffer_size=None,
-               leveldb_max_file_size=None,
-               lmdb_map_size=None,
-               batch_size=None
-                 ):
+                 input_fn:typing.Callable[[int,typing.Any,tuple],typing.Union[typing.Dict,typing.List,typing.Tuple]],
+                 input_fn_args:typing.Tuple,
+                 outfile:str,
+                 backend: str,
+                 overwrite = False,
+                 num_process_worker:int = 8,
+                 options=None,
+                 parquet_options=None,
+                 schema=None,
+                 leveldb_write_buffer_size=None,
+                 leveldb_max_file_size=None,
+                 lmdb_map_size=None,
+                 batch_size=None):
 
     if not os.path.exists(outfile) or overwrite:
         fw = DataWriteHelper(input_fn,input_fn_args,outfile,backend,num_process_worker)
         fw.save(data,
                 options=options,
                 parquet_options=parquet_options,
                 schema=schema,
```

## numpy_io/pytorch_loader/dataloaders.py

```diff
@@ -201,13 +201,14 @@
         transform_fn=transform_fn, check_dataset_file_fn=check_dataset_file_fn,
         limit_start=limit_start,
         limit_count=limit_count,
         dataset_loader_filter_fn=dataset_loader_filter_fn,
     )
     if dataset is None:
         return None
+
     return DataLoader(dataset, batch_size=batch_size,
                       shuffle=False if isinstance(dataset, IterableDataset) else shuffle,
                       collate_fn=collate_fn,
                       pin_memory=pin_memory, **kwargs)
```

## numpy_io/pytorch_loader/tokenizer_config_helper.py

```diff
@@ -27,15 +27,15 @@
     if do_lower_case is not None:
         tokenizer_kwargs['do_lower_case'] = do_lower_case
 
     if use_fast_tokenizer is not None:
         tokenizer_kwargs['use_fast'] = use_fast_tokenizer
 
     if class_name is not None:
-        tokenizer = class_name.from_pretrained(tokenizer_name, **tokenizer_kwargs)
+        tokenizer = class_name.from_pretrained(tokenizer_name or model_name_or_path, **tokenizer_kwargs)
     elif tokenizer_name:
         tokenizer = AutoTokenizer.from_pretrained(tokenizer_name, **tokenizer_kwargs)
     elif model_name_or_path:
         tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, **tokenizer_kwargs)
     else:
         raise ValueError(
             "You are instantiating a new tokenizer from scratch. This is not supported by this script."
@@ -75,15 +75,15 @@
     for k in list(tmp_kwargs.keys()):
         if tmp_kwargs[k] is None:
             tmp_kwargs.pop(k)
     if tmp_kwargs:
         config_kwargs.update(tmp_kwargs)
 
     if class_name is not None:
-        config = class_name.from_pretrained(config_name, **config_kwargs)
+        config = class_name.from_pretrained(config_name or model_name_or_path, **config_kwargs)
     elif isinstance(config_name,PretrainedConfig):
         for k,v in config_kwargs.items():
             setattr(config_name,k,v)
         config = config_name
 
     elif config_name:
         config = AutoConfig.from_pretrained(config_name, **config_kwargs)
```

## Comparing `numpy_io-0.0.7.dist-info/RECORD` & `numpy_io-0.0.8.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,38 @@
+numpy_io/.gitignore,sha256=lxgH3Lm9pVVy-oLsEQLl4IVSvx2c6adwEFENIXqE-Uo,39
+numpy_io/README.MD,sha256=Jr1S1Oi1MGOptud_OsmH9zllNNV5ABjlNoYbbt50mKU,1662
 numpy_io/__init__.py,sha256=aCtpF76c1Jz1-xvsEqeV_ze4a40-KqaqUtIrFy3BTcU,77
-numpy_io/setup.py,sha256=6TqGB3Ng4epHGUoDZslKtuRSB0nAR5ljlActQLaJsT0,629
 numpy_io/core/__init__.py,sha256=gvmkt5S6jF7SlAsFM1e9qGGXV96a5yTB5lBavIVjuKo,80
 numpy_io/core/numpyadapter.py,sha256=-hxHnhsbA4nF5HO-zytYUl3-UQOR1O4fqTwL9bbaVI0,19587
-numpy_io/core/parallel.py,sha256=-m_FKZegXe1q22A0nB3xgVE1edaRzjqYKlGroI0xgFA,5619
+numpy_io/core/parallel.py,sha256=kwrwZkP_3SzsMkNilXYV3PZeESdAEXzUQ2YFnyYqQ5k,5578
 numpy_io/core/reader.py,sha256=-i7NiW3s1gPFwaM03tDWT0NLVG6FEkz6fOuo_nWB3r8,1894
 numpy_io/core/writer.py,sha256=Oh81NqgmbesSEACUaymNKYm4YJln91rzELhLs9UjDWs,2268
+numpy_io/examples/README.md,sha256=cnFxCBeaZwargZ-9xXqTXo1ilTRc6yQrIWpdshlZ6iI,9635
 numpy_io/examples/__init__.py,sha256=H6PH5pOOHNUW3_RuUpgWfpv6_Pijqyy_3U1JCTLl6jg,54
 numpy_io/examples/auto_parallel_writer.py,sha256=geSpDCFHxe4skPd3Vk45lhc3azuJEPviGhcYtUlTid4,3236
 numpy_io/examples/auto_writer.py,sha256=vyvCXOJ5zroUweOOT0CFJnA8M_5nC8qJR0pxRv_8p88,3241
+numpy_io/examples/demo_arrow_writer.py,sha256=zvfELqj1PDHYuMUwZ6J4TXBU7tBMIwNXUrR9Wuxq6dY,2313
+numpy_io/examples/demo_arrow_writer2.py,sha256=Z_6-ED6aOzAZ-w-VT5AhRcqm7PWOcIosrmMLW_zQvG8,1378
+numpy_io/examples/demo_parquet_writer.py,sha256=8hXbV4IjDAXcb0hMTC6h7mGXZG51AL2yFJRVowaB-yI,2183
 numpy_io/examples/leveldb_readwriter_example.py,sha256=SKE4a3Wx67GPMbTmIlg8tIWT6JSxVc7QIRAi_gjOGvQ,1778
 numpy_io/examples/lmdb_readwriter_example.py,sha256=ZmZGfjy1o8c_O61JxXvKUrf6N_WSBGHHU1QCTK6DwH4,2218
 numpy_io/examples/memory_raw_readwriter_example.py,sha256=3LJzlLFFtDQdHyXM1dP7PupfnPb_0nM3qG4i7MF0MZg,1198
 numpy_io/examples/memory_readwriter_example.py,sha256=QAlov1poEZOYxmWNYgQkundKtST3VsFH10hTy3TE92w,1285
 numpy_io/examples/record_numpywriter_example.py,sha256=4VMeVDiA-0IwuBt0B_a0NNcs4OFyjkk1FOEmZlMavmc,1586
 numpy_io/examples/record_reader_example.py,sha256=Mv0uZyAVobFq6wGBJ-GQ0KvvEe9EjBZmGz5tXM9ChsQ,1353
 numpy_io/examples/record_shuffle_example.py,sha256=TFFnJOqgtOZZ8s8j4bZ2Ju16PyAt3Q5X17anhbfI9mg,1398
 numpy_io/examples/record_writer_example.py,sha256=VtgDxRxbs-tXVbNRo78TImVe48rioqvoKtOhTmwA1F8,3056
 numpy_io/examples/testing/__init__.py,sha256=Jj2ycuBs45i9qAcrC6iCm22QOY46Xujv9lzOSbeeZ_o,56
+numpy_io/examples/testing/demo_arrow_writer.py,sha256=zvfELqj1PDHYuMUwZ6J4TXBU7tBMIwNXUrR9Wuxq6dY,2313
+numpy_io/examples/testing/demo_arrow_writer2.py,sha256=Z_6-ED6aOzAZ-w-VT5AhRcqm7PWOcIosrmMLW_zQvG8,1378
+numpy_io/examples/testing/demo_parquet_writer.py,sha256=8hXbV4IjDAXcb0hMTC6h7mGXZG51AL2yFJRVowaB-yI,2183
 numpy_io/examples/testing/lmdb_test.py,sha256=rQvokJAIDW9esAesab9wHs03OcG2TPImAuybnCO-LBA,2658
 numpy_io/examples/testing/test_mem.py,sha256=gteaDLS79vwwfJETTeL-JCxn3VhRT3So59y5AV4ah9w,613
 numpy_io/examples/testing/test_mutiprocess.py,sha256=rgO758tNAycWGYxyJl2AM2jkffNQs-AjRU9peSotGzQ,2907
 numpy_io/pytorch_loader/__init__.py,sha256=oRU1cnNHyp22vA9HkEYfoPtpdQdU4D9scv9KtgxYVdE,73
-numpy_io/pytorch_loader/data_helper.py,sha256=oVjtyWRobAYx1DMc5FePqQRyiQnoCpS60iidwHxN6k4,10309
-numpy_io/pytorch_loader/dataloaders.py,sha256=ov1DvKCv8GO4QGuoj09-BdUlDFop_4DScXMNv4B-jl0,8940
-numpy_io/pytorch_loader/tokenizer_config_helper.py,sha256=8hoofhL7uMyE8pT-U_3WNKDyy5DBOqQhDwJMZri-InY,3780
-numpy_io-0.0.7.dist-info/METADATA,sha256=pn3IEZTtVh1PAzeiHFi22Ge32Xui9cblwLiQ4lpanaY,390
-numpy_io-0.0.7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-numpy_io-0.0.7.dist-info/top_level.txt,sha256=mV0ZVKt8HA3kBLuj9iZkff1sq-cR9hE36TgSw_7Mr4E,9
-numpy_io-0.0.7.dist-info/RECORD,,
+numpy_io/pytorch_loader/data_helper.py,sha256=TgJ7YARmbQA1bGSYwX85rNau1wnDjrO_36ZAibyYlTY,10310
+numpy_io/pytorch_loader/dataloaders.py,sha256=wvEHQKpS1QAehrxIPBgH-ZkUctN7aHbCfGOWpqQZLtE,8942
+numpy_io/pytorch_loader/tokenizer_config_helper.py,sha256=Ypji_c41GaZ2y2GAo4Lc7-cxt25kx9-KaREbFmb4T-Q,3824
+numpy_io-0.0.8.dist-info/METADATA,sha256=h1TkgTFih-XgiaI3udsgbUUJj-CRYI5k7mUnwCW0rE0,388
+numpy_io-0.0.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+numpy_io-0.0.8.dist-info/top_level.txt,sha256=mV0ZVKt8HA3kBLuj9iZkff1sq-cR9hE36TgSw_7Mr4E,9
+numpy_io-0.0.8.dist-info/RECORD,,
```

