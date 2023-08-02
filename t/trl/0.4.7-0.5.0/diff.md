# Comparing `tmp/trl-0.4.7.tar.gz` & `tmp/trl-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trl-0.4.7.tar", last modified: Thu Jul 13 08:26:56 2023, max compression
+gzip compressed data, was "trl-0.5.0.tar", last modified: Wed Aug  2 08:30:12 2023, max compression
```

## Comparing `trl-0.4.7.tar` & `trl-0.5.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.241035 trl-0.4.7/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2522 2023-07-12 12:43:13.000000 trl-0.4.7/CONTRIBUTING.md
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11357 2023-05-03 09:18:40.000000 trl-0.4.7/LICENSE
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      111 2023-05-03 09:18:40.000000 trl-0.4.7/MANIFEST.in
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9620 2023-07-13 08:26:56.241035 trl-0.4.7/PKG-INFO
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     8590 2023-07-12 12:43:13.000000 trl-0.4.7/README.md
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      257 2023-07-13 08:26:56.241035 trl-0.4.7/setup.cfg
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3759 2023-07-13 08:17:28.000000 trl-0.4.7/setup.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.237035 trl-0.4.7/tests/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-05-03 09:18:40.000000 trl-0.4.7/tests/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3162 2023-06-21 08:50:41.000000 trl-0.4.7/tests/test_best_of_n_sampler.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1561 2023-05-03 09:18:40.000000 trl-0.4.7/tests/test_core.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      152 2023-06-21 08:50:41.000000 trl-0.4.7/tests/test_e2e.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23191 2023-05-03 09:18:40.000000 trl-0.4.7/tests/test_modeling_value_head.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5439 2023-05-03 09:18:40.000000 trl-0.4.7/tests/test_no_peft.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9515 2023-06-19 11:54:46.000000 trl-0.4.7/tests/test_peft_models.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    42825 2023-07-12 12:43:13.000000 trl-0.4.7/tests/test_ppo_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9931 2023-07-11 07:11:15.000000 trl-0.4.7/tests/test_reward_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    18911 2023-06-23 08:12:16.000000 trl-0.4.7/tests/test_sft_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      799 2023-05-03 09:18:40.000000 trl-0.4.7/tests/testing_constants.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1555 2023-05-03 09:18:40.000000 trl-0.4.7/tests/testing_utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.237035 trl-0.4.7/trl/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      407 2023-07-13 08:17:35.000000 trl-0.4.7/trl/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     7920 2023-05-03 09:18:40.000000 trl-0.4.7/trl/core.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.241035 trl-0.4.7/trl/extras/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      668 2023-06-21 08:50:41.000000 trl-0.4.7/trl/extras/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5190 2023-06-21 08:50:41.000000 trl-0.4.7/trl/extras/best_of_n_sampler.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1120 2023-05-03 09:18:40.000000 trl-0.4.7/trl/import_utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.241035 trl-0.4.7/trl/models/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      910 2023-05-03 09:18:40.000000 trl-0.4.7/trl/models/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23980 2023-07-12 12:43:13.000000 trl-0.4.7/trl/models/modeling_base.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    18277 2023-07-12 12:43:13.000000 trl-0.4.7/trl/models/modeling_value_head.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.241035 trl-0.4.7/trl/trainer/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1035 2023-07-07 10:32:34.000000 trl-0.4.7/trl/trainer/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1772 2023-05-03 09:18:40.000000 trl-0.4.7/trl/trainer/base.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     8751 2023-07-12 12:43:13.000000 trl-0.4.7/trl/trainer/ppo_config.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    53529 2023-07-12 12:43:13.000000 trl-0.4.7/trl/trainer/ppo_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    10115 2023-07-12 12:37:45.000000 trl-0.4.7/trl/trainer/reward_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    13740 2023-07-13 08:15:02.000000 trl-0.4.7/trl/trainer/sft_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    12711 2023-07-12 12:43:13.000000 trl-0.4.7/trl/trainer/utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.241035 trl-0.4.7/trl.egg-info/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9620 2023-07-13 08:26:56.000000 trl-0.4.7/trl.egg-info/PKG-INFO
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      887 2023-07-13 08:26:56.000000 trl-0.4.7/trl.egg-info/SOURCES.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-07-13 08:26:56.000000 trl-0.4.7/trl.egg-info/dependency_links.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-05-17 08:26:30.000000 trl-0.4.7/trl.egg-info/not-zip-safe
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      210 2023-07-13 08:26:56.000000 trl-0.4.7/trl.egg-info/requires.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)       10 2023-07-13 08:26:56.000000 trl-0.4.7/trl.egg-info/top_level.txt
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-08-02 08:30:12.168131 trl-0.5.0/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2522 2023-07-12 12:43:13.000000 trl-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11357 2023-05-03 09:18:40.000000 trl-0.5.0/LICENSE
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      111 2023-05-03 09:18:40.000000 trl-0.5.0/MANIFEST.in
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9612 2023-08-02 08:30:12.168131 trl-0.5.0/PKG-INFO
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     8582 2023-07-14 11:23:16.000000 trl-0.5.0/README.md
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      257 2023-08-02 08:30:12.172132 trl-0.5.0/setup.cfg
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3759 2023-08-02 08:27:07.000000 trl-0.5.0/setup.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-08-02 08:30:12.164131 trl-0.5.0/tests/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-05-03 09:18:40.000000 trl-0.5.0/tests/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3162 2023-06-21 08:50:41.000000 trl-0.5.0/tests/test_best_of_n_sampler.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1561 2023-05-03 09:18:40.000000 trl-0.5.0/tests/test_core.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3657 2023-07-19 15:38:50.000000 trl-0.5.0/tests/test_dpo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      152 2023-06-21 08:50:41.000000 trl-0.5.0/tests/test_e2e.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23191 2023-05-03 09:18:40.000000 trl-0.5.0/tests/test_modeling_value_head.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5439 2023-05-03 09:18:40.000000 trl-0.5.0/tests/test_no_peft.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9515 2023-06-19 11:54:46.000000 trl-0.5.0/tests/test_peft_models.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    45640 2023-08-02 07:17:29.000000 trl-0.5.0/tests/test_ppo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9931 2023-07-11 07:11:15.000000 trl-0.5.0/tests/test_reward_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    22342 2023-08-02 07:17:29.000000 trl-0.5.0/tests/test_sft_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      799 2023-05-03 09:18:40.000000 trl-0.5.0/tests/testing_constants.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1555 2023-05-03 09:18:40.000000 trl-0.5.0/tests/testing_utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-08-02 08:30:12.164131 trl-0.5.0/trl/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      419 2023-08-02 08:27:03.000000 trl-0.5.0/trl/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     8389 2023-08-02 07:17:29.000000 trl-0.5.0/trl/core.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-08-02 08:30:12.168131 trl-0.5.0/trl/extras/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      668 2023-06-21 08:50:41.000000 trl-0.5.0/trl/extras/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5190 2023-06-21 08:50:41.000000 trl-0.5.0/trl/extras/best_of_n_sampler.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1120 2023-05-03 09:18:40.000000 trl-0.5.0/trl/import_utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-08-02 08:30:12.168131 trl-0.5.0/trl/models/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      910 2023-05-03 09:18:40.000000 trl-0.5.0/trl/models/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23933 2023-08-02 08:18:33.000000 trl-0.5.0/trl/models/modeling_base.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    18277 2023-07-12 12:43:13.000000 trl-0.5.0/trl/models/modeling_value_head.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-08-02 08:30:12.168131 trl-0.5.0/trl/trainer/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1071 2023-07-18 16:46:01.000000 trl-0.5.0/trl/trainer/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1772 2023-05-03 09:18:40.000000 trl-0.5.0/trl/trainer/base.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    21863 2023-07-27 13:20:03.000000 trl-0.5.0/trl/trainer/dpo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     8968 2023-08-02 07:17:29.000000 trl-0.5.0/trl/trainer/ppo_config.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    56481 2023-08-02 07:17:29.000000 trl-0.5.0/trl/trainer/ppo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    10165 2023-07-19 15:38:50.000000 trl-0.5.0/trl/trainer/reward_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    14868 2023-07-24 10:21:51.000000 trl-0.5.0/trl/trainer/sft_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23050 2023-08-02 07:17:29.000000 trl-0.5.0/trl/trainer/utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-08-02 08:30:12.164131 trl-0.5.0/trl.egg-info/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9612 2023-08-02 08:30:11.000000 trl-0.5.0/trl.egg-info/PKG-INFO
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      940 2023-08-02 08:30:12.000000 trl-0.5.0/trl.egg-info/SOURCES.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-08-02 08:30:11.000000 trl-0.5.0/trl.egg-info/dependency_links.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-05-17 08:26:30.000000 trl-0.5.0/trl.egg-info/not-zip-safe
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      210 2023-08-02 08:30:11.000000 trl-0.5.0/trl.egg-info/requires.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)       10 2023-08-02 08:30:11.000000 trl-0.5.0/trl.egg-info/top_level.txt
```

### Comparing `trl-0.4.7/CONTRIBUTING.md` & `trl-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/LICENSE` & `trl-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/PKG-INFO` & `trl-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trl
-Version: 0.4.7
+Version: 0.5.0
 Summary: A Pytorch implementation of Proximal Policy Optimization for transfomer language models.
 Home-page: https://github.com/lvwerra/trl
 Author: Leandro von Werra
 Author-email: leandro.vonwerra@gmail.com
 License: Apache 2.0
 Keywords: ppo,transformers,huggingface,gpt2,language modeling,rlhf
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -186,15 +186,15 @@
 reward = [torch.tensor(1.0)]
 
 # train model for one step with ppo
 train_stats = ppo_trainer.step([query_tensor[0]], [response_tensor[0]], reward)
 ```
 
 ### Advanced example: IMDB sentiment
-For a detailed example check out the example python script `examples/sentiment/scripts/gpt2-sentiment.py`, where GPT2 is fine-tuned to generate positive movie reviews. An few examples from the language models before and after optimisation are given below:
+For a detailed example check out the example python script `examples/scripts/sentiment_tuning.py`, where GPT2 is fine-tuned to generate positive movie reviews. An few examples from the language models before and after optimisation are given below:
 
 <div style="text-align: center">
 <img src="https://huggingface.co/datasets/trl-internal-testing/example-images/resolve/main/images/table_imdb_preview.png" width="800">
 <p style="text-align: center;"> <b>Figure:</b> A few review continuations before and after optimisation. </p>
 </div>
 
 Have a look at more examples inside [`examples/`](https://github.com/lvwerra/trl/tree/main/examples) folder.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trl Version: 0.4.7 Summary: A Pytorch
+Metadata-Version: 2.1 Name: trl Version: 0.5.0 Summary: A Pytorch
 implementation of Proximal Policy Optimization for transfomer language models.
 Home-page: https://github.com/lvwerra/trl Author: Leandro von Werra Author-
 email: leandro.vonwerra@gmail.com License: Apache 2.0 Keywords:
 ppo,transformers,huggingface,gpt2,language modeling,rlhf Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
@@ -99,16 +99,16 @@
 (query_txt, return_tensors="pt") # get model response response_tensor =
 respond_to_batch(model, query_tensor) # create a ppo trainer ppo_trainer =
 PPOTrainer(ppo_config, model, model_ref, tokenizer) # define a reward for
 response # (this could be any reward such as human feedback or output from
 another model) reward = [torch.tensor(1.0)] # train model for one step with ppo
 train_stats = ppo_trainer.step([query_tensor[0]], [response_tensor[0]], reward)
 ``` ### Advanced example: IMDB sentiment For a detailed example check out the
-example python script `examples/sentiment/scripts/gpt2-sentiment.py`, where
-GPT2 is fine-tuned to generate positive movie reviews. An few examples from the
+example python script `examples/scripts/sentiment_tuning.py`, where GPT2 is
+fine-tuned to generate positive movie reviews. An few examples from the
 language models before and after optimisation are given below:
 [https://huggingface.co/datasets/trl-internal-testing/example-images/resolve/
 main/images/table_imdb_preview.png]
 Figure: A few review continuations before and after optimisation.
 Have a look at more examples inside [`examples/`](https://github.com/lvwerra/
 trl/tree/main/examples) folder. ## References ### Proximal Policy Optimisation
 The PPO implementation largely follows the structure introduced in the paper
```

### Comparing `trl-0.4.7/README.md` & `trl-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 reward = [torch.tensor(1.0)]
 
 # train model for one step with ppo
 train_stats = ppo_trainer.step([query_tensor[0]], [response_tensor[0]], reward)
 ```
 
 ### Advanced example: IMDB sentiment
-For a detailed example check out the example python script `examples/sentiment/scripts/gpt2-sentiment.py`, where GPT2 is fine-tuned to generate positive movie reviews. An few examples from the language models before and after optimisation are given below:
+For a detailed example check out the example python script `examples/scripts/sentiment_tuning.py`, where GPT2 is fine-tuned to generate positive movie reviews. An few examples from the language models before and after optimisation are given below:
 
 <div style="text-align: center">
 <img src="https://huggingface.co/datasets/trl-internal-testing/example-images/resolve/main/images/table_imdb_preview.png" width="800">
 <p style="text-align: center;"> <b>Figure:</b> A few review continuations before and after optimisation. </p>
 </div>
 
 Have a look at more examples inside [`examples/`](https://github.com/lvwerra/trl/tree/main/examples) folder.
```

#### html2text {}

```diff
@@ -85,16 +85,16 @@
 (query_txt, return_tensors="pt") # get model response response_tensor =
 respond_to_batch(model, query_tensor) # create a ppo trainer ppo_trainer =
 PPOTrainer(ppo_config, model, model_ref, tokenizer) # define a reward for
 response # (this could be any reward such as human feedback or output from
 another model) reward = [torch.tensor(1.0)] # train model for one step with ppo
 train_stats = ppo_trainer.step([query_tensor[0]], [response_tensor[0]], reward)
 ``` ### Advanced example: IMDB sentiment For a detailed example check out the
-example python script `examples/sentiment/scripts/gpt2-sentiment.py`, where
-GPT2 is fine-tuned to generate positive movie reviews. An few examples from the
+example python script `examples/scripts/sentiment_tuning.py`, where GPT2 is
+fine-tuned to generate positive movie reviews. An few examples from the
 language models before and after optimisation are given below:
 [https://huggingface.co/datasets/trl-internal-testing/example-images/resolve/
 main/images/table_imdb_preview.png]
 Figure: A few review continuations before and after optimisation.
 Have a look at more examples inside [`examples/`](https://github.com/lvwerra/
 trl/tree/main/examples) folder. ## References ### Proximal Policy Optimisation
 The PPO implementation largely follows the structure introduced in the paper
```

### Comparing `trl-0.4.7/setup.py` & `trl-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 8. Change the version in __init__.py and setup.py to X.X.X+1.dev0 (e.g. VERSION=1.18.3 -> 1.18.4.dev0).
    Then push the change with a message 'set dev version'
 """
 
 from setuptools import find_packages, setup
 
 
-__version__ = "0.4.7"  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+__version__ = "0.5.0"  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
 
 REQUIRED_PKGS = [
     "torch>=1.4.0",
     "transformers>=4.18.0",
     "numpy>=1.18.2",
     "accelerate",
     "datasets",
```

### Comparing `trl-0.4.7/tests/test_best_of_n_sampler.py` & `trl-0.5.0/tests/test_best_of_n_sampler.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/tests/test_core.py` & `trl-0.5.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/tests/test_modeling_value_head.py` & `trl-0.5.0/tests/test_modeling_value_head.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/tests/test_no_peft.py` & `trl-0.5.0/tests/test_no_peft.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/tests/test_peft_models.py` & `trl-0.5.0/tests/test_peft_models.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/tests/test_ppo_trainer.py` & `trl-0.5.0/tests/test_ppo_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -543,41 +543,44 @@
 
         # dummy values
         ref_logprobs = all_logprobs + 1
         logits = torch.exp(all_logprobs)
         vpreds = values + 0.1
 
         score, non_score = ppo_trainer.compute_rewards(dummy_scores, all_logprobs, ref_logprobs, mask)
+        values, advantages, returns = ppo_trainer.compute_advantages(values, score, mask)
 
         # just make sure a dummy loss is computed
         idx = 0
         pg_loss, v_loss, _ = ppo_trainer.loss(
             all_logprobs[idx].unsqueeze(0),
             values[idx].unsqueeze(0),
-            score[idx].unsqueeze(0),
             logits[idx].unsqueeze(0),
             vpreds[idx].unsqueeze(0),
             ref_logprobs[idx].unsqueeze(0),
             mask[idx].unsqueeze(0),
+            advantages[idx].unsqueeze(0),
+            returns[idx].unsqueeze(0),
         )
 
-        self.assertAlmostEqual(pg_loss.item(), 0.62516, 4)
+        self.assertAlmostEqual(pg_loss.item(), 2.2868, 4)
         self.assertAlmostEqual(v_loss.item(), 0.09950, 4)
 
         # check if we get same results with masked parts removed
         pg_loss_unmasked, v_loss_unmasked, _ = ppo_trainer.loss(
             apply_mask(all_logprobs[idx], mask[idx]).unsqueeze(0),
             apply_mask(values[idx], mask[idx]).unsqueeze(0),
-            apply_mask(score[idx], mask[idx]).unsqueeze(0),
             apply_mask(logits[idx], mask[idx]).unsqueeze(0),
             apply_mask(vpreds[idx], mask[idx]).unsqueeze(0),
             apply_mask(ref_logprobs[idx], mask[idx]).unsqueeze(0),
             apply_mask(mask[idx], mask[idx]).unsqueeze(0),
+            apply_mask(advantages[idx], mask[idx]).unsqueeze(0),
+            apply_mask(returns[idx], mask[idx]).unsqueeze(0),
         )
-        self.assertAlmostEqual(pg_loss_unmasked.item(), 0.62516, 4)
+        self.assertAlmostEqual(pg_loss_unmasked.item(), 2.2868, 4)
         self.assertAlmostEqual(v_loss_unmasked.item(), 0.09950, 4)
 
     @parameterized.expand(
         [
             ["gpt2"],
             ["bloom"],
             ["t5"],
@@ -716,14 +719,106 @@
             tokenizer=self.gpt2_tokenizer,
             dataset=dummy_dataset,
         )
 
         expected_output = torch.Tensor([[0.0050, 0.0050, 0.0050], [0.0050, 0.0050, 0.0200]])
         self.assertTrue(torch.allclose(ppo_trainer._kl_penalty(log_probs, ref_log_probs), expected_output))
 
+    def test_ppo_trainer_full_kl_penalty(self):
+        # a few more extensive tests for the full kl option as it is more involved
+        dummy_dataset = self._init_dummy_dataset()
+
+        self.ppo_config.kl_penalty = "full"
+        ppo_trainer = PPOTrainer(
+            config=self.ppo_config,
+            model=self.gpt2_model,
+            ref_model=None,
+            tokenizer=self.gpt2_tokenizer,
+            dataset=dummy_dataset,
+        )
+
+        # Test on tensors for size B,S,T = (1,2,3)
+        # test for when the two dists are the same
+        log_probs = torch.Tensor(
+            [
+                [
+                    [0.1, 0.2, 0.7],
+                    [0.3, 0.4, 0.3],
+                ]
+            ]
+        ).exp()
+
+        ref_log_probs = torch.Tensor(
+            [
+                [
+                    [0.1, 0.2, 0.7],
+                    [0.3, 0.4, 0.3],
+                ]
+            ]
+        ).exp()
+
+        expected_output = torch.Tensor(
+            [[0.0, 0.0]],
+        )
+        output = ppo_trainer._kl_penalty(log_probs, ref_log_probs)
+        self.assertTrue(output.shape == (1, 2))
+        self.assertTrue(torch.allclose(output, expected_output))
+
+        # test for when the two dists are almost not overlapping
+        log_probs = torch.Tensor(
+            [
+                [
+                    [0.98, 0.01, 0.01],
+                    [0.01, 0.98, 0.01],
+                ]
+            ]
+        ).log()
+
+        ref_log_probs = torch.Tensor(
+            [
+                [
+                    [0.01, 0.01, 0.98],
+                    [0.01, 0.01, 0.98],
+                ]
+            ]
+        ).log()
+
+        expected_output = torch.Tensor(
+            [[4.4474, 4.4474]],
+        )
+        output = ppo_trainer._kl_penalty(log_probs, ref_log_probs)
+        self.assertTrue(output.shape == (1, 2))
+        self.assertTrue(torch.allclose(output, expected_output))
+
+        # test for when the two dists are almost not overlapping
+        log_probs = torch.Tensor(
+            [
+                [
+                    [0.49, 0.02, 0.49],
+                    [0.49, 0.02, 0.49],
+                ]
+            ]
+        ).log()
+
+        ref_log_probs = torch.Tensor(
+            [
+                [
+                    [0.01, 0.98, 0.01],
+                    [0.49, 0.02, 0.49],
+                ]
+            ]
+        ).log()
+
+        expected_output = torch.Tensor(
+            [[3.7361, 0.0]],
+        )
+        output = ppo_trainer._kl_penalty(log_probs, ref_log_probs)
+        self.assertTrue(output.shape == (1, 2))
+        self.assertTrue(torch.allclose(output, expected_output, atol=1e-4))
+
     @require_peft
     @mark.peft_test
     def test_peft_model_ppo_trainer(self):
         from peft import LoraConfig, get_peft_model
         from transformers import AutoModelForCausalLM
 
         lora_config = LoraConfig(
@@ -1033,18 +1128,18 @@
             # define a reward for response
             # (this could be any reward such as human feedback or output from another model)
             reward = [torch.tensor(1.0), torch.tensor(1.0)]
             # train model by running a step twice
             _ = ppo_trainer.step([q for q in query_tensor], [r for r in response_tensor], reward)
             break
 
-        model_grad = gpt2_model.v_head.summary.weight.grad.clone()
+        model_grad = gpt2_model.v_head.summary.weight
 
-        self.ppo_config.gradient_accumulation_steps = 2
         self.ppo_config.mini_batch_size = 1
+        self.ppo_config.gradient_accumulation_steps = 2
 
         ppo_trainer = PPOTrainer(
             config=self.ppo_config,
             model=gpt2_model_clone,
             ref_model=None,
             tokenizer=self.gpt2_tokenizer,
             dataset=dummy_dataset,
@@ -1057,15 +1152,15 @@
             # define a reward for response
             # (this could be any reward such as human feedback or output from another model)
             reward = [torch.tensor(1.0), torch.tensor(1.0)]
             # train model by running a step twice
             _ = ppo_trainer.step([q for q in query_tensor], [r for r in response_tensor], reward)
             break
 
-        model_grad_acc = gpt2_model_clone.v_head.summary.weight.grad.clone()
+        model_grad_acc = gpt2_model_clone.v_head.summary.weight
         self.assertTrue(torch.allclose(model_grad_acc, model_grad, rtol=1e-3, atol=1e-3))
 
     @unittest.skip("Fix by either patching `whomai()` to work in the staging endpoint or use a dummy prod user.")
     def test_push_to_hub_if_best_reward(self):
         REPO_NAME = "test-ppo-trainer"
         repo_id = f"{CI_HUB_USER}/{REPO_NAME}"
```

### Comparing `trl-0.4.7/tests/test_reward_trainer.py` & `trl-0.5.0/tests/test_reward_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/tests/test_sft_trainer.py` & `trl-0.5.0/tests/test_sft_trainer.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import copy
 import os
 import tempfile
 import unittest
 
 import numpy as np
 from datasets import Dataset
 from transformers import AutoModelForCausalLM, AutoTokenizer, TrainingArguments
@@ -409,23 +410,98 @@
 
     def test_data_collator_completion_lm(self):
         response_template = "### Response:\n"
         data_collator = DataCollatorForCompletionOnlyLM(response_template, tokenizer=self.tokenizer, mlm=False)
 
         text = """\n\n### Instructions:\nHello all this should be masked\n\n### Response:\nI have not been masked correctly."""
         encoded_text = self.tokenizer(text)
-        encoded_text["input_ids"] = encoded_text["input_ids"]
 
         examples = [encoded_text]
 
         batch = data_collator(examples)
         labels = batch["labels"]
         last_pad_idx = np.where(labels == -100)[1][-1]
         result_text = self.tokenizer.decode(batch["input_ids"][0, last_pad_idx + 1 :])
-        self.assertTrue(result_text == "I have not been masked correctly.")
+        self.assertEqual(result_text, "I have not been masked correctly.")
+
+    def test_data_collator_completion_lm_with_multiple_text(self):
+        tokenizer = copy.deepcopy(self.tokenizer)
+        tokenizer.padding_side = "left"
+
+        response_template = "### Response:\n"
+        data_collator = DataCollatorForCompletionOnlyLM(response_template, tokenizer=tokenizer, mlm=False)
+
+        text1 = """\n\n### Instructions:\nHello all this should be masked\n\n### Response:\nI have not been masked correctly."""
+        text2 = """\n\n### Instructions:\nThis is another longer text that should also be masked. This text is significantly longer than the previous one.\n\n### Response:\nI have not been masked correctly."""
+
+        encoded_text1 = tokenizer(text1)
+        encoded_text2 = tokenizer(text2)
+
+        examples = [encoded_text1, encoded_text2]
+
+        batch = data_collator(examples)
+
+        for i in range(2):
+            labels = batch["labels"][i]
+            last_pad_idx = np.where(labels == -100)[0][-1]
+            result_text = tokenizer.decode(batch["input_ids"][i, last_pad_idx + 1 :])
+            self.assertEqual(result_text, "I have not been masked correctly.")
+
+    def test_data_collator_chat_completion_lm(self):
+        instruction_template = "### Human:"
+        assistant_template = "### Assistant:"
+        data_collator = DataCollatorForCompletionOnlyLM(
+            response_template=assistant_template,
+            instruction_template=instruction_template,
+            tokenizer=self.tokenizer,
+            mlm=False,
+        )
+
+        text = """### Human: Hello all this should be masked.### Assistant: I should not be masked.### Human: All this should be masked too.### Assistant: I should not be masked too."""
+        encoded_text = self.tokenizer(text)
+
+        examples = [encoded_text]
+
+        batch = data_collator(examples)
+        labels = batch["labels"]
+        non_masked_tokens = batch["input_ids"][labels != -100]
+        result_text = self.tokenizer.decode(non_masked_tokens)
+        self.assertEqual(result_text, " I should not be masked. I should not be masked too.")
+
+    def test_data_collator_chat_completion_lm_with_multiple_text(self):
+        tokenizer = copy.deepcopy(self.tokenizer)
+        tokenizer.padding_side = "left"
+
+        instruction_template = "### Human:"
+        assistant_template = "### Assistant:"
+        data_collator = DataCollatorForCompletionOnlyLM(
+            response_template=assistant_template,
+            instruction_template=instruction_template,
+            tokenizer=tokenizer,
+            mlm=False,
+        )
+
+        text1 = """### Human: Hello all this should be masked.### Assistant: I should not be masked."""
+        text2 = """### Human: Hello all this should be masked.### Assistant: I should not be masked.### Human: All this should be masked too.### Assistant: I should not be masked too."""
+        encoded_text1 = tokenizer(text1)
+        encoded_text2 = tokenizer(text2)
+
+        examples = [encoded_text1, encoded_text2]
+
+        batch = data_collator(examples)
+        labels = batch["labels"]
+        input_ids = batch["input_ids"]
+
+        non_masked_tokens1 = input_ids[0][labels[0] != -100]
+        result_text1 = tokenizer.decode(non_masked_tokens1)
+        self.assertEqual(result_text1, " I should not be masked.")
+
+        non_masked_tokens2 = input_ids[1][labels[1] != -100]
+        result_text2 = tokenizer.decode(non_masked_tokens2)
+        self.assertEqual(result_text2, " I should not be masked. I should not be masked too.")
 
     def test_sft_trainer_infinite_with_model(self):
         with tempfile.TemporaryDirectory() as tmp_dir:
             training_args = TrainingArguments(
                 output_dir=tmp_dir,
                 dataloader_drop_last=True,
                 evaluation_strategy="steps",
```

### Comparing `trl-0.4.7/tests/testing_constants.py` & `trl-0.5.0/tests/testing_constants.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/tests/testing_utils.py` & `trl-0.5.0/tests/testing_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/trl/core.py` & `trl-0.5.0/trl/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,19 +84,22 @@
     t_size = tensor.size()[dim]
     if t_size == size:
         return tensor
     else:
         return torch.nn.functional.pad(tensor, (0, size - t_size), "constant", padding)
 
 
-def logprobs_from_logits(logits, labels):
+def logprobs_from_logits(logits, labels, gather=True):
     """
     See: https://github.com/pytorch/pytorch/issues/563#issuecomment-330103591
     """
     logp = F.log_softmax(logits, dim=2)
+
+    if not gather:
+        return logp
     logpy = torch.gather(logp, 2, labels.unsqueeze(2)).squeeze(-1)
     return logpy
 
 
 def whiten(values, shift_mean=True):
     """Whiten values."""
     mean, var = torch.mean(values), torch.var(values)
@@ -116,15 +119,23 @@
 
 def masked_var(values, mask, unbiased=True):
     """Compute variance of tensor with masked values."""
     mean = masked_mean(values, mask)
     centered_values = values - mean
     variance = masked_mean(centered_values**2, mask)
     if unbiased:
-        bessel_correction = mask.sum() / (mask.sum() - 1)
+        mask_sum = mask.sum()
+        if mask_sum == 0:
+            raise ValueError(
+                "The sum of the mask is zero, which can happen when `mini_batch_size=1`;"
+                "try increase the `mini_batch_size` or `gradient_accumulation_steps`"
+            )
+        # note that if mask_sum == 1, then there is a division by zero issue
+        # to avoid it you just need to use a larger minibatch_size
+        bessel_correction = mask_sum / (mask_sum - 1)
         variance = variance * bessel_correction
     return variance
 
 
 def masked_whiten(values, mask, shift_mean=True):
     """Whiten values with masked values."""
     mean, var = masked_mean(values, mask), masked_var(values, mask)
```

### Comparing `trl-0.4.7/trl/extras/__init__.py` & `trl-0.5.0/trl/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/trl/extras/best_of_n_sampler.py` & `trl-0.5.0/trl/extras/best_of_n_sampler.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/trl/import_utils.py` & `trl-0.5.0/trl/import_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/trl/models/__init__.py` & `trl-0.5.0/trl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/trl/models/modeling_base.py` & `trl-0.5.0/trl/models/modeling_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,25 +296,23 @@
             model.supports_rm_adapter = False
 
         return model
 
     @classmethod
     def _get_current_device(cls):
         r"""
-        Get the current device using the `Accelerate` object - We just return the
-        process index of the `Accelerate` object to handle corner cases when running scripts
-        in distributed setups.
+        Get the current device. For GPU, we return the local process index using the `Accelerator`
+        object to handle corner cases when running scripts in distributed environments.
 
         Returns:
-            current_device (`int`):
-                The current device index.
+            current_device (`Union[int, str]`):
+                The current device.
         """
         dummy_accelerator = Accelerator()
-        current_device = dummy_accelerator.process_index
-        return current_device if torch.cuda.is_available() else "cpu"
+        return dummy_accelerator.local_process_index if torch.cuda.is_available() else "cpu"
 
     @classmethod
     def _split_kwargs(cls, kwargs):
         """
         Separate the kwargs from the arguments that we support inside
         `supported_args` and the ones that we don't.
         """
```

### Comparing `trl-0.4.7/trl/models/modeling_value_head.py` & `trl-0.5.0/trl/models/modeling_value_head.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/trl/trainer/__init__.py` & `trl-0.5.0/trl/trainer/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 # There is a circular import in the PPOTrainer if we let isort sort these
 # isort: off
 from .utils import AdaptiveKLController, FixedKLController, ConstantLengthDataset, DataCollatorForCompletionOnlyLM
 
 # isort: on
 
 from .base import BaseTrainer
+from .dpo_trainer import DPOTrainer
 from .ppo_config import PPOConfig
 from .ppo_trainer import PPOTrainer
 from .reward_trainer import RewardTrainer, compute_accuracy
 from .sft_trainer import SFTTrainer
```

### Comparing `trl-0.4.7/trl/trainer/base.py` & `trl-0.5.0/trl/trainer/base.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.7/trl/trainer/ppo_config.py` & `trl-0.5.0/trl/trainer/ppo_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     init_kl_coef: Optional[float] = field(
         default=0.2,
         metadata={"help": "Initial KL penalty coefficient (used for adaptive and linear control)"},
     )
     kl_penalty: Optional[str] = field(
         default="kl",
         metadata={
-            "help": "kl penalty options: 'kl': model_logp - ref_logp,  'abs': abs(kl) and 'mse': mean squared error mse(kl)."
+            "help": "kl penalty options: 'kl': model_logp - ref_logp,  'abs': abs(kl),  'mse': mean squared error mse(kl) and 'full': the actual kl for all tokens in the distribution"
         },
     )
     target: Optional[float] = field(default=6, metadata={"help": "Target KL value for adaptive KL control"})
     horizon: Optional[float] = field(default=10000, metadata={"help": "Horizon for adaptive KL control"})
     gamma: Optional[float] = field(default=1, metadata={"help": "Gamma parameter for advantage calculation"})
     lam: Optional[float] = field(default=0.95, metadata={"help": "Lambda parameter for advantage calculation"})
     cliprange: Optional[float] = field(
@@ -96,15 +96,18 @@
     vf_coef: Optional[float] = field(default=0.1, metadata={"help": "Scaling factor for value loss"})
     batch_size: Optional[int] = field(default=256, metadata={"help": "Number of samples per optimisation step"})
     forward_batch_size: Optional[int] = field(
         default=None,
         metadata={"help": "Number of samples forward passed through model at a time"},
     )
     mini_batch_size: Optional[int] = field(
-        default=1, metadata={"help": "Number of samples optimized inside PPO together"}
+        default=1, metadata={"help": "Number of samples optimized in each mini batch"}
+    )
+    backward_batch_size: Optional[int] = field(
+        default=1, metadata={"help": "Number of samples optimized in an `optimizer.step()` call"}
     )
     gradient_accumulation_steps: Optional[int] = field(
         default=1, metadata={"help": "The number of gradient accumulation steps"}
     )
     ppo_epochs: Optional[int] = field(
         default=4,
         metadata={"help": "Number of optimisation epochs per batch of samples"},
@@ -183,14 +186,14 @@
                     logging.info(f"the following tags will be used for wandb logging: {os.environ['WANDB_TAGS']}")
             except ImportError:
                 raise ImportError(
                     "Please install wandb to use wandb logging. You can do this by running `pip install wandb`."
                 )
 
         self.total_ppo_epochs = int(np.ceil(self.steps / self.batch_size))
-        assert self.kl_penalty in ["kl", "abs", "mse"]
+        assert self.kl_penalty in ["kl", "abs", "mse", "full"]
 
     def to_dict(self):
         output_dict = {}
         for key, value in self.__dict__.items():
             output_dict[key] = value
         return flatten_dict(output_dict)
```

### Comparing `trl-0.4.7/trl/trainer/ppo_trainer.py` & `trl-0.5.0/trl/trainer/ppo_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import inspect
+import math
 import os
 import time
 import typing
 import warnings
 from typing import Callable, List, Optional, Union
 
 import datasets
+import numpy as np
 import torch
+import torch.nn.functional as F
 from accelerate import Accelerator
 from accelerate.utils import ProjectConfiguration
 from datasets import Dataset
 from huggingface_hub import whoami
 from packaging import version
-from requests.exceptions import HTTPError
 from torch.optim import Adam
 from transformers import (
     DataCollatorForLanguageModeling,
     PreTrainedTokenizer,
     PreTrainedTokenizerBase,
     PreTrainedTokenizerFast,
 )
@@ -198,14 +200,15 @@
         self.accelerator.init_trackers(
             config.tracker_project_name,
             config=dict(trl_ppo_trainer_config=config.to_dict()) if not is_using_tensorboard else config.to_dict(),
             init_kwargs=config.tracker_kwargs,
         )
 
         self.model = model
+        self.model_params = filter(lambda p: p.requires_grad, self.model.parameters())
         self.is_encoder_decoder = hasattr(self.model, "is_encoder_decoder")
         self.is_peft_model = getattr(self.model, "is_peft_model", False)
 
         if isinstance(ref_model, SUPPORTED_ARCHITECTURES):
             self.ref_model = ref_model
             if num_shared_layers is not None:
                 warnings.warn(
@@ -248,19 +251,22 @@
                 " refer to the documentation for more details.",
                 UserWarning,
             )
             self.dataloader = None
         else:
             self.dataloader = None
 
+        self.config.backward_batch_size = self.config.mini_batch_size * self.config.gradient_accumulation_steps
+
         # Step 3: Initialize optimizer and data collator
         self.data_collator = DataCollatorForLanguageModeling(self.tokenizer, mlm=False)
         if optimizer is None:
             self.optimizer = Adam(
-                filter(lambda p: p.requires_grad, self.model.parameters()), lr=self.config.learning_rate
+                filter(lambda p: p.requires_grad, self.model.parameters()),
+                lr=self.config.learning_rate,
             )
         else:
             self.optimizer = optimizer
 
         self.lr_scheduler = lr_scheduler
         if self.lr_scheduler is not None:
             lr_scheduler_class = (
@@ -287,24 +293,28 @@
         (
             self.model,
             self.optimizer,
             self.data_collator,
             self.dataloader,
             self.lr_scheduler,
         ) = self.accelerator.prepare(
-            self.model, self.optimizer, self.data_collator, self.dataloader, self.lr_scheduler
+            self.model,
+            self.optimizer,
+            self.data_collator,
+            self.dataloader,
+            self.lr_scheduler,
         )
         if is_deepspeed_used:
             # 8 bit models are already set on the correct device
             if not self.is_peft_model and not (
                 getattr(self.ref_model.pretrained_model, "is_loaded_in_8bit", False)
                 or getattr(self.ref_model.pretrained_model, "is_loaded_in_4bit", False)
             ):
                 # DS integration only allows for single model and as `ref_model` is only used for
-                # `KL devergence loss`,i.e, in eval model, just have it be on the respective device and
+                # `KL divergence loss`,i.e, in eval model, just have it be on the respective device and
                 # there is no need to pass it to the `accelerator.prepare` call
                 self.ref_model = self.ref_model.to(self.accelerator.device)
 
             # this hack seems to be needed for DS stage 3 to work
             if self.accelerator.state.deepspeed_plugin.zero_stage == 3:
                 self.model.train()
         else:
@@ -389,15 +399,17 @@
 
         ignored_columns = list(set(dataset.column_names) - set(signature_columns))
 
         columns = [k for k in signature_columns if k in dataset.column_names]
 
         if version.parse(datasets.__version__) < version.parse("1.4.0"):
             dataset.set_format(
-                type=dataset.format["type"], columns=columns, format_kwargs=dataset.format["format_kwargs"]
+                type=dataset.format["type"],
+                columns=columns,
+                format_kwargs=dataset.format["format_kwargs"],
             )
             return dataset
         else:
             return dataset.remove_columns(ignored_columns)
 
     def generate(
         self,
@@ -595,117 +607,149 @@
 
         model_inputs = self.prepare_model_inputs(queries, responses)
 
         if self.is_distributed:
             pad_first = self.tokenizer.padding_side == "left"
 
             model_inputs["input_ids"] = self.accelerator.pad_across_processes(
-                model_inputs["input_ids"], dim=1, pad_index=self.tokenizer.pad_token_id, pad_first=pad_first
+                model_inputs["input_ids"],
+                dim=1,
+                pad_index=self.tokenizer.pad_token_id,
+                pad_first=pad_first,
             )
             model_inputs["attention_mask"] = self.accelerator.pad_across_processes(
                 model_inputs["attention_mask"], dim=1, pad_index=0, pad_first=pad_first
             )
             if self.is_encoder_decoder:
                 model_inputs["decoder_input_ids"] = self.accelerator.pad_across_processes(
                     model_inputs["decoder_input_ids"],
                     dim=1,
                     pad_index=self.tokenizer.pad_token_id,
                     pad_first=pad_first,
                 )
                 model_inputs["decoder_attention_mask"] = self.accelerator.pad_across_processes(
-                    model_inputs["decoder_attention_mask"], dim=1, pad_index=0, pad_first=pad_first
+                    model_inputs["decoder_attention_mask"],
+                    dim=1,
+                    pad_index=0,
+                    pad_first=pad_first,
                 )
 
         model_inputs_names = list(model_inputs.keys())
 
+        full_kl_penalty = self.config.kl_penalty == "full"
+
         with torch.no_grad():
-            all_logprobs, _, values, masks = self.batched_forward_pass(self.model, queries, responses, model_inputs)
+            all_logprobs, logits_or_none, values, masks = self.batched_forward_pass(
+                self.model, queries, responses, model_inputs, return_logits=full_kl_penalty
+            )
 
             # for when the model is a peft model
             if self.is_peft_model and hasattr(
-                self.accelerator.unwrap_model(self.model).pretrained_model, "disable_adapter"
+                self.accelerator.unwrap_model(self.model).pretrained_model,
+                "disable_adapter",
             ):
                 with self.accelerator.unwrap_model(self.model).pretrained_model.disable_adapter():
-                    ref_logprobs, _, _, _ = self.batched_forward_pass(self.model, queries, responses, model_inputs)
+                    ref_logprobs, ref_logits_or_none, _, _ = self.batched_forward_pass(
+                        self.model, queries, responses, model_inputs, return_logits=full_kl_penalty
+                    )
             elif self.is_peft_model and not hasattr(self.model.pretrained_model, "disable_adapter"):
                 raise ValueError(
                     "You are using a `peft` version that does not support `disable_adapter`. Please update your `peft` version to the latest version."
                 )
 
             else:
-                ref_logprobs, _, _, _ = self.batched_forward_pass(self.ref_model, queries, responses, model_inputs)
+                ref_logprobs, ref_logits_or_none, _, _ = self.batched_forward_pass(
+                    self.ref_model, queries, responses, model_inputs, return_logits=full_kl_penalty
+                )
 
         timing["time/ppo/forward_pass"] = time.time() - t
 
-        t = time.time()
-        rewards, non_score_reward = self.compute_rewards(scores, all_logprobs, ref_logprobs, masks)
-        timing["time/ppo/compute_rewards"] = time.time() - t
+        with torch.no_grad():
+            t = time.time()
+            if full_kl_penalty:
+                active_full_logprobs = logprobs_from_logits(logits_or_none, None, gather=False)
+                ref_full_logprobs = logprobs_from_logits(ref_logits_or_none, None, gather=False)
+
+                rewards, non_score_reward = self.compute_rewards(
+                    scores, active_full_logprobs, ref_full_logprobs, masks
+                )
+            else:
+                rewards, non_score_reward = self.compute_rewards(scores, all_logprobs, ref_logprobs, masks)
+            timing["time/ppo/compute_rewards"] = time.time() - t
+
+            t = time.time()
+            values, advantages, returns = self.compute_advantages(values, rewards, masks)
+            timing["time/ppo/compute_advantages"] = time.time() - t
 
         # upcast to float32 to avoid dataset issues
-        mini_batch_dict = {
+        batch_dict = {
             "queries": queries,
             "responses": responses,
             "logprobs": all_logprobs.to(torch.float32),
             "values": values.to(torch.float32),
-            "rewards": rewards,
             "masks": masks,
+            "advantages": advantages,
+            "returns": returns,
         }
-
-        def collator(data):
-            return_dict = dict()
-            for key in data[0]:
-                if key in ["queries", "responses"]:
-                    return_dict[key] = [d[key] for d in data]
-                else:
-                    return_dict[key] = torch.stack([d[key] for d in data]).to(self.current_device)
-            return return_dict
-
-        mini_batch_dict.update(model_inputs)
-        mini_batch_data = Dataset.from_dict(mini_batch_dict)
-        mini_batch_data.set_format("torch")
-        mini_batch_dataloader = torch.utils.data.DataLoader(
-            mini_batch_data,
-            batch_size=self.config.mini_batch_size,
-            shuffle=True,
-            collate_fn=collator,
-        )
+        batch_dict.update(model_inputs)
 
         t = time.time()
         all_stats = []
         early_stop = False
         for _ in range(self.config.ppo_epochs):
             if early_stop:
                 break
-
-            for i, batch in enumerate(mini_batch_dataloader):
-                with self.accelerator.accumulate(self.model):
-                    model_inputs = {k: batch[k] for k in model_inputs_names}
-                    logprobs, logits, vpreds, _ = self.batched_forward_pass(
-                        self.model, batch["queries"], batch["responses"], model_inputs, return_logits=True
-                    )
-                    if (i % self.config.gradient_accumulation_steps) == 0:
-                        self.optimizer.zero_grad()
-
-                    train_stats = self.train_minibatch(
-                        batch["logprobs"],
-                        batch["values"],
-                        batch["rewards"],
-                        logprobs,
-                        logits,
-                        vpreds,
-                        batch["masks"],
-                    )
-
-                    all_stats.append(train_stats)
-
-                    if self.config.early_stopping:
-                        policykl = train_stats["policy/policykl"]
-                        early_stop = self._early_stop(policykl)
-                        if early_stop:
-                            break
+            b_inds = np.random.permutation(bs)
+            for backward_batch_start in range(0, bs, self.config.backward_batch_size):
+                backward_batch_end = backward_batch_start + self.config.backward_batch_size
+                backward_batch_inds = b_inds[backward_batch_start:backward_batch_end]
+
+                for mini_batch_start in range(0, self.config.backward_batch_size, self.config.mini_batch_size):
+                    mini_batch_end = mini_batch_start + self.config.mini_batch_size
+                    mini_batch_inds = backward_batch_inds[mini_batch_start:mini_batch_end]
+                    mini_batch_dict = {
+                        "logprobs": batch_dict["logprobs"][mini_batch_inds],
+                        "values": batch_dict["values"][mini_batch_inds],
+                        "masks": batch_dict["masks"][mini_batch_inds],
+                        # hacks: the queries and responses are ragged.
+                        "queries": [batch_dict["queries"][i] for i in mini_batch_inds],
+                        "responses": [batch_dict["responses"][i] for i in mini_batch_inds],
+                        "advantages": batch_dict["advantages"][mini_batch_inds],
+                        "returns": batch_dict["returns"][mini_batch_inds],
+                    }
+                    for k in model_inputs_names:
+                        mini_batch_dict[k] = batch_dict[k][mini_batch_inds]
+                    with self.accelerator.accumulate(self.model):
+                        model_inputs = {k: mini_batch_dict[k] for k in model_inputs_names}
+
+                        logprobs, logits, vpreds, _ = self.batched_forward_pass(
+                            self.model,
+                            mini_batch_dict["queries"],
+                            mini_batch_dict["responses"],
+                            model_inputs,
+                            return_logits=True,
+                        )
+                        train_stats = self.train_minibatch(
+                            mini_batch_dict["logprobs"],
+                            mini_batch_dict["values"],
+                            logprobs,
+                            logits,
+                            vpreds,
+                            mini_batch_dict["masks"],
+                            mini_batch_dict["advantages"],
+                            mini_batch_dict["returns"],
+                        )
+                        all_stats.append(train_stats)
+
+            # typically, early stopping is done at the epoch level
+            if self.config.early_stopping:
+                policykl = train_stats["policy/policykl"]
+                early_stop = self._early_stop(policykl)
+                if early_stop:
+                    break
 
         timing["time/ppo/optimize_step"] = time.time() - t
 
         t = time.time()
         train_stats = stack_dicts(all_stats)
 
         # reshape advantages/ratios such that they are not averaged.
@@ -728,15 +772,18 @@
         if self.is_distributed:
             stats = self.gather_stats(stats)
         stats = stats_to_np(stats)
         timing["time/ppo/calc_stats"] = time.time() - t
         stats["ppo/learning_rate"] = self.optimizer.param_groups[0]["lr"]
 
         # Update the KL control - multiply the batch_size by the number of processes
-        self.kl_ctl.update(stats["objective/kl"], self.config.batch_size * self.accelerator.num_processes)
+        self.kl_ctl.update(
+            stats["objective/kl"],
+            self.config.batch_size * self.accelerator.num_processes,
+        )
 
         # Log the total ppo time
         timing["time/ppo/total"] = time.time() - t0
         stats.update(timing)
 
         # post-process stats for tensorboard and other loggers
         if self.config.log_with != "wandb":
@@ -858,15 +905,15 @@
         bs = len(queries)
         fbs = self.config.mini_batch_size
         all_logprobs = []
         all_logits = []
         all_masks = []
         all_values = []
 
-        for i in range(int(bs / fbs)):
+        for i in range(math.ceil(bs / fbs)):
             input_kwargs = {key: value[i * fbs : (i + 1) * fbs] for key, value in model_inputs.items()}
             query_batch = queries[i * fbs : (i + 1) * fbs]
             response_batch = responses[i * fbs : (i + 1) * fbs]
             logits, _, values = model(**input_kwargs)
 
             if self.is_encoder_decoder:
                 input_ids = input_kwargs["decoder_input_ids"]
@@ -875,15 +922,15 @@
                 input_ids = input_kwargs["input_ids"]
                 attention_mask = input_kwargs["attention_mask"]
 
             logprobs = logprobs_from_logits(logits[:, :-1, :], input_ids[:, 1:])
             masks = torch.zeros_like(attention_mask)
             masks[:, :-1] = attention_mask[:, 1:]
 
-            for j in range(fbs):
+            for j in range(len(query_batch)):
                 if self.is_encoder_decoder:
                     # Decoder sentence starts always in the index 1 after padding in the Enc-Dec Models
                     start = 1
                     end = attention_mask[j, :].sum() - 1
                 else:
                     start = len(query_batch[j]) - 1
                     if attention_mask[j, 0] == 0:  # offset left padding
@@ -909,53 +956,52 @@
         )
 
     @PPODecorators.empty_cuda_cache()
     def train_minibatch(
         self,
         old_logprobs: torch.FloatTensor,
         values: torch.FloatTensor,
-        rewards: torch.FloatTensor,
         logprobs: torch.FloatTensor,
         logits: torch.FloatTensor,
         vpreds: torch.FloatTensor,
         mask: torch.LongTensor,
+        advantages: torch.FloatTensor,
+        returns: torch.FloatTensor,
     ):
         """
         Train one PPO minibatch
 
         Args:
             logprobs (`torch.FloatTensor`):
                 Log probabilities of the model, shape [batch_size, response_length]
             values (`torch.FloatTensor`):
                 Values of the value head, shape [batch_size, response_length]
-            rewards (`torch.FloatTensor`):
-                Rewards from the reward model, shape [batch_size, response_length]
             query (`torch.LongTensor`):
                 Encoded queries, shape [batch_size, query_length]
             response (`torch.LongTensor`):
                 Encoded responses, shape [batch_size, response_length]
             model_input (`torch.LongTensor`):
                 Concatenated queries and responses, shape [batch_size, query_length+response_length]
 
         Returns:
             train_stats (dict[str, `torch.Tensor`]):
                 Dictionary of training statistics
         """
-        loss_p, loss_v, train_stats = self.loss(old_logprobs, values, rewards, logits, vpreds, logprobs, mask)
+        loss_p, loss_v, train_stats = self.loss(
+            old_logprobs, values, logits, vpreds, logprobs, mask, advantages, returns
+        )
         loss = loss_p + loss_v
         self.accelerator.backward(loss)
-
         if self.config.max_grad_norm is not None:
-            torch.nn.utils.clip_grad_norm_(
-                filter(lambda p: p.requires_grad, self.model.parameters()), self.config.max_grad_norm
-            )
-
-        t = time.time()
+            if self.accelerator.sync_gradients:
+                self.accelerator.clip_grad_norm_(self.model_params, self.config.max_grad_norm)
         self.optimizer.step()
-        train_stats["time/ppo/optimizer_step"] = torch.Tensor([time.time() - t]).to(self.current_device)
+        # we call optimizer.zero_grad() every time and let `accelerator` handle accumulation
+        # see https://huggingface.co/docs/accelerate/usage_guides/gradient_accumulation#the-finished-code
+        self.optimizer.zero_grad()
         return train_stats
 
     def compute_rewards(
         self,
         scores: torch.FloatTensor,
         logprobs: torch.FloatTensor,
         ref_logprobs: torch.FloatTensor,
@@ -992,25 +1038,55 @@
 
         if self.config.kl_penalty == "abs":
             return (logprob - ref_logprob).abs()
 
         if self.config.kl_penalty == "mse":
             return 0.5 * (logprob - ref_logprob).square()
 
+        if self.config.kl_penalty == "full":
+            # Flip is required due to this issue? :https://github.com/pytorch/pytorch/issues/57459
+            return F.kl_div(ref_logprob, logprob, log_target=True, reduction="none").sum(-1)
+
         raise NotImplementedError
 
+    def compute_advantages(
+        self: torch.FloatTensor,
+        values: torch.FloatTensor,
+        rewards: torch.FloatTensor,
+        mask: torch.FloatTensor,
+    ):
+        lastgaelam = 0
+        advantages_reversed = []
+        gen_len = rewards.shape[-1]
+
+        values = values * mask
+        rewards = rewards * mask
+
+        for t in reversed(range(gen_len)):
+            nextvalues = values[:, t + 1] if t < gen_len - 1 else 0.0
+            delta = rewards[:, t] + self.config.gamma * nextvalues - values[:, t]
+            lastgaelam = delta + self.config.gamma * self.config.lam * lastgaelam
+            advantages_reversed.append(lastgaelam)
+        advantages = torch.stack(advantages_reversed[::-1]).transpose(0, 1)
+
+        returns = advantages + values
+        advantages = masked_whiten(advantages, mask)
+        advantages = advantages.detach()
+        return values, advantages, returns
+
     def loss(
         self,
         old_logprobs: torch.FloatTensor,
         values: torch.FloatTensor,
-        rewards: torch.FloatTensor,
         logits: torch.FloatTensor,
         vpreds: torch.FloatTensor,
         logprobs: torch.FloatTensor,
         mask: torch.LongTensor,
+        advantages: torch.FloatTensor,
+        returns: torch.FloatTensor,
     ):
         """
         Calculate policy and value losses.
 
         Args:
             old_logprobs (`torch.FloatTensor`):
                 Log probabilities of the model, shape (`batch_size`, `response_length`)
@@ -1021,34 +1097,19 @@
             logits (`torch.FloatTensor`):
                 Logits of the model, shape (`batch_size`, `response_length`, `vocab_size`)
             v_pred (`torch.FloatTensor`):
                 Values of the value head, shape (`batch_size`, `response_length`)
             logprobs (`torch.FloatTensor`):
                 Log probabilities of the model, shape (`batch_size`, `response_length`)
         """
-        lastgaelam = 0
-        advantages_reversed = []
-        gen_len = rewards.shape[-1]
-
-        values = values * mask
-        rewards = rewards * mask
-
-        for t in reversed(range(gen_len)):
-            nextvalues = values[:, t + 1] if t < gen_len - 1 else 0.0
-            delta = rewards[:, t] + self.config.gamma * nextvalues - values[:, t]
-            lastgaelam = delta + self.config.gamma * self.config.lam * lastgaelam
-            advantages_reversed.append(lastgaelam)
-        advantages = torch.stack(advantages_reversed[::-1]).transpose(0, 1)
-
-        returns = advantages + values
-        advantages = masked_whiten(advantages, mask)
-        advantages = advantages.detach()
 
         vpredclipped = clip_by_value(
-            vpreds, values - self.config.cliprange_value, values + self.config.cliprange_value
+            vpreds,
+            values - self.config.cliprange_value,
+            values + self.config.cliprange_value,
         )
 
         vf_losses1 = (vpreds - returns) ** 2
         vf_losses2 = (vpredclipped - returns) ** 2
         vf_loss = 0.5 * masked_mean(torch.max(vf_losses1, vf_losses2), mask)
         vf_clipfrac = masked_mean(torch.gt(vf_losses2, vf_losses1).float(), mask)
 
@@ -1224,15 +1285,18 @@
             logs["env/reward_std"] = torch.std(rewards).cpu().numpy().item()
             logs["env/reward_dist"] = rewards.cpu().numpy()
 
             if self.config.log_with == "tensorboard":
                 # update the current step
                 self.current_step += 1
 
-            self.accelerator.log(logs, step=self.current_step if self.config.log_with == "tensorboard" else None)
+            self.accelerator.log(
+                logs,
+                step=self.current_step if self.config.log_with == "tensorboard" else None,
+            )
 
         else:
             if self.is_distributed:
                 import torch.distributed as dist
 
                 if not isinstance(rewards, torch.Tensor):
                     rewards = torch.tensor(rewards).to(self.current_device)
@@ -1246,15 +1310,15 @@
         Args:
             path (`str`): The path to save the model card to.
             model_name (`str`, *optional*): The name of the model, defaults to `TRL Model`.
         """
         try:
             user = whoami()["name"]
         # handle the offline case
-        except HTTPError:
+        except:  # noqa
             warnings.warn("Cannot retrieve user information assuming you are running in offline mode.")
             return
 
         if not os.path.exists(path):
             os.makedirs(path)
 
         model_card_content = MODEL_CARD_TEMPLATE.format(model_name=model_name, model_id=f"{user}/{path}")
```

### Comparing `trl-0.4.7/trl/trainer/reward_trainer.py` & `trl-0.5.0/trl/trainer/reward_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,39 +10,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import warnings
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-import numpy as np
 import torch
 import torch.nn as nn
 from datasets import Dataset
 from transformers import DataCollator, PreTrainedModel, PreTrainedTokenizerBase, Trainer, TrainingArguments
 from transformers.trainer_callback import TrainerCallback
 from transformers.trainer_pt_utils import nested_detach
 from transformers.trainer_utils import EvalPrediction
 
 from ..import_utils import is_peft_available
-from .utils import PeftSavingCallback, RewardDataCollatorWithPadding
+from .utils import PeftSavingCallback, RewardDataCollatorWithPadding, compute_accuracy
 
 
 if is_peft_available():
-    from peft import PeftModel, get_peft_model
-
-
-def compute_accuracy(eval_pred) -> Dict[str, float]:
-    predictions, labels = eval_pred
-    # Here, predictions is rewards_chosen and rewards_rejected.
-    # We want to see how much of the time rewards_chosen > rewards_rejected.
-    predictions = np.argmax(predictions, axis=1)
-
-    accuracy = np.array(predictions == labels, dtype=float).mean().item()
-    return {"accuracy": accuracy}
+    from peft import PeftModel, get_peft_model, prepare_model_for_int8_training
 
 
 class RewardTrainer(Trainer):
     r"""
     The RewardTrainer can be used to train your custom Reward Model. It is a subclass of the
     `transformers.Trainer` class and inherits all of its attributes and methods. It is recommended to use
     an `AutoModelForSequenceClassification` as the reward model. The reward model should be trained on a dataset
@@ -65,15 +54,18 @@
         data_collator: Optional[DataCollator] = None,
         train_dataset: Optional[Dataset] = None,
         eval_dataset: Optional[Union[Dataset, Dict[str, Dataset]]] = None,
         tokenizer: Optional[PreTrainedTokenizerBase] = None,
         model_init: Optional[Callable[[], PreTrainedModel]] = None,
         compute_metrics: Optional[Callable[[EvalPrediction], Dict]] = None,
         callbacks: Optional[List[TrainerCallback]] = None,
-        optimizers: Tuple[torch.optim.Optimizer, torch.optim.lr_scheduler.LambdaLR] = (None, None),
+        optimizers: Tuple[torch.optim.Optimizer, torch.optim.lr_scheduler.LambdaLR] = (
+            None,
+            None,
+        ),
         preprocess_logits_for_metrics: Optional[Callable[[torch.Tensor, torch.Tensor], torch.Tensor]] = None,
         max_length: Optional[int] = None,
         peft_config: Optional[Dict] = None,
     ):
         """
         Initialize RewardTrainer.
 
@@ -107,14 +99,17 @@
                 The PEFT configuration to use for training. If you pass a PEFT configuration, the model will be wrapped in a PEFT model.
         """
         if not is_peft_available() and peft_config is not None:
             raise ValueError(
                 "PEFT is not installed and you passed a `peft_config` in the trainer's kwargs, please install it to use the PEFT models"
             )
         elif is_peft_available() and peft_config is not None:
+            if getattr(model, "is_loaded_in_8bit", False) or getattr(model, "is_quantized", False):
+                model = prepare_model_for_int8_training(model)
+
             model = get_peft_model(model, peft_config)
 
         if is_peft_available() and callbacks is None and isinstance(model, PeftModel):
             callbacks = [PeftSavingCallback()]
 
         if compute_metrics is None:
             compute_metrics = compute_accuracy
@@ -162,24 +157,33 @@
     def compute_loss(
         self,
         model: Union[PreTrainedModel, nn.Module],
         inputs: Dict[str, Union[torch.Tensor, Any]],
         return_outputs=False,
     ) -> Union[torch.Tensor, Tuple[torch.Tensor, Dict[str, torch.Tensor]]]:
         if not self.use_reward_data_collator:
-            raise NotImplementedError(
-                "compute_loss is only implemented for RewardDataCollatorWithPadding, please implement your own compute_loss method if you are using a custom data collator"
+            warnings.warn(
+                "The current compute_loss is implemented for RewardDataCollatorWithPadding,"
+                " if you are using a custom data collator make sure you know what you are doing or"
+                " implement your own compute_loss method."
             )
-        rewards_chosen = model(input_ids=inputs["input_ids_chosen"], attention_mask=inputs["attention_mask_chosen"])[0]
+        rewards_chosen = model(
+            input_ids=inputs["input_ids_chosen"],
+            attention_mask=inputs["attention_mask_chosen"],
+        )[0]
         rewards_rejected = model(
-            input_ids=inputs["input_ids_rejected"], attention_mask=inputs["attention_mask_rejected"]
+            input_ids=inputs["input_ids_rejected"],
+            attention_mask=inputs["attention_mask_rejected"],
         )[0]
         loss = -nn.functional.logsigmoid(rewards_chosen - rewards_rejected).mean()
         if return_outputs:
-            return loss, {"rewards_chosen": rewards_chosen, "rewards_rejected": rewards_rejected}
+            return loss, {
+                "rewards_chosen": rewards_chosen,
+                "rewards_rejected": rewards_rejected,
+            }
         return loss
 
     def prediction_step(
         self,
         model: Union[PreTrainedModel, nn.Module],
         inputs: Dict[str, Union[torch.Tensor, Any]],
         prediction_loss_only: bool,
@@ -202,9 +206,10 @@
         logits = tuple(v for k, v in logits_dict.items() if k not in ignore_keys)
         logits = nested_detach(logits)
         # Stack accepted against rejected, mean over logits
         # and softmax to get preferences between accepted and rejected to sum to 1
         logits = torch.stack(logits).mean(dim=2).softmax(dim=0).T
 
         labels = torch.zeros(logits.shape[0])
+        labels = self._prepare_inputs(labels)
 
         return loss, logits, labels
```

### Comparing `trl-0.4.7/trl/trainer/sft_trainer.py` & `trl-0.5.0/trl/trainer/sft_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,19 @@
             The number of sequences to use for the `ConstantLengthDataset`. Defaults to `1024`.
         chars_per_token (`Optional[float]`):
             The number of characters per token to use for the `ConstantLengthDataset`. Defaults to `3.6`. You can check how this is computed in the
             stack-llama example: https://github.com/lvwerra/trl/blob/08f550674c553c36c51d1027613c29f14f3676a5/examples/stack_llama/scripts/supervised_finetuning.py#L53.
         packing (`Optional[bool]`):
             Used only in case `dataset_text_field` is passed. This argument is used by the `ConstantLengthDataset` to pack the sequences
             of the dataset.
+        dataset_num_proc (`Optional[int]`):
+            The number of workers to use to tokenize the data. Only used when `packing=False`. Defaults to None.
+        dataset_batch_size (`int`):
+            The number of examples to tokenize per batch. If batch_size <= 0 or batch_size == None,
+            tokenize the full dataset as a single batch. Defaults to 1000.
     """
 
     def __init__(
         self,
         model: Union[PreTrainedModel, nn.Module, str] = None,
         args: TrainingArguments = None,
         data_collator: Optional[DataCollator] = None,
@@ -108,14 +113,16 @@
         dataset_text_field: Optional[str] = None,
         packing: Optional[bool] = False,
         formatting_func: Optional[Callable] = None,
         max_seq_length: Optional[int] = None,
         infinite: Optional[bool] = False,
         num_of_sequences: Optional[int] = 1024,
         chars_per_token: Optional[float] = 3.6,
+        dataset_num_proc: Optional[int] = None,
+        dataset_batch_size: int = 1000,
     ):
         if isinstance(model, str):
             warnings.warn(
                 "You passed a model_id to the SFTTrainer. This will automatically create an "
                 "`AutoModelForCausalLM` or a `PeftModel` (if you passed a `peft_config`) for you."
             )
 
@@ -156,14 +163,16 @@
             # to overcome some issues with broken tokenizers
             max_seq_length = min(tokenizer.model_max_length, 1024)
 
             warnings.warn(
                 f"You didn't pass a `max_seq_length` argument to the SFTTrainer, this will default to {max_seq_length}"
             )
 
+        self.dataset_num_proc = dataset_num_proc
+        self.dataset_batch_size = dataset_batch_size
         if not packing:
             if dataset_text_field is None and formatting_func is None:
                 raise ValueError(
                     "You passed `packing=False` to the SFTTrainer, but you didn't pass a `dataset_text_field` or `formatting_func` argument."
                 )
 
             if data_collator is None:
@@ -190,14 +199,20 @@
                 max_seq_length,
                 formatting_func,
                 infinite,
                 num_of_sequences,
                 chars_per_token,
             )
 
+        if tokenizer.padding_side is not None and tokenizer.padding_side != "right":
+            warnings.warn(
+                "You passed a tokenizer with `padding_side` not equal to `right` to the SFTTrainer. This might lead to some unexpected behaviour due to "
+                "overflow issues when training a model in half-precision. You might consider adding `tokenizer.padding_side = 'right'` to your code."
+            )
+
         super().__init__(
             model=model,
             args=args,
             data_collator=data_collator,
             train_dataset=train_dataset,
             eval_dataset=eval_dataset,
             tokenizer=tokenizer,
@@ -285,10 +300,16 @@
                         "The `formatting_func` should return a list of processed strings since it can lead to silent bugs."
                     )
                 else:
                     self._dataset_sanity_checked = True
 
             return {"input_ids": outputs["input_ids"], "attention_mask": outputs["attention_mask"]}
 
-        tokenized_dataset = dataset.map(tokenize, batched=True, remove_columns=dataset.column_names)
+        tokenized_dataset = dataset.map(
+            tokenize,
+            batched=True,
+            remove_columns=dataset.column_names,
+            num_proc=self.dataset_num_proc,
+            batch_size=self.dataset_batch_size,
+        )
 
         return tokenized_dataset
```

### Comparing `trl-0.4.7/trl.egg-info/PKG-INFO` & `trl-0.5.0/trl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trl
-Version: 0.4.7
+Version: 0.5.0
 Summary: A Pytorch implementation of Proximal Policy Optimization for transfomer language models.
 Home-page: https://github.com/lvwerra/trl
 Author: Leandro von Werra
 Author-email: leandro.vonwerra@gmail.com
 License: Apache 2.0
 Keywords: ppo,transformers,huggingface,gpt2,language modeling,rlhf
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -186,15 +186,15 @@
 reward = [torch.tensor(1.0)]
 
 # train model for one step with ppo
 train_stats = ppo_trainer.step([query_tensor[0]], [response_tensor[0]], reward)
 ```
 
 ### Advanced example: IMDB sentiment
-For a detailed example check out the example python script `examples/sentiment/scripts/gpt2-sentiment.py`, where GPT2 is fine-tuned to generate positive movie reviews. An few examples from the language models before and after optimisation are given below:
+For a detailed example check out the example python script `examples/scripts/sentiment_tuning.py`, where GPT2 is fine-tuned to generate positive movie reviews. An few examples from the language models before and after optimisation are given below:
 
 <div style="text-align: center">
 <img src="https://huggingface.co/datasets/trl-internal-testing/example-images/resolve/main/images/table_imdb_preview.png" width="800">
 <p style="text-align: center;"> <b>Figure:</b> A few review continuations before and after optimisation. </p>
 </div>
 
 Have a look at more examples inside [`examples/`](https://github.com/lvwerra/trl/tree/main/examples) folder.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trl Version: 0.4.7 Summary: A Pytorch
+Metadata-Version: 2.1 Name: trl Version: 0.5.0 Summary: A Pytorch
 implementation of Proximal Policy Optimization for transfomer language models.
 Home-page: https://github.com/lvwerra/trl Author: Leandro von Werra Author-
 email: leandro.vonwerra@gmail.com License: Apache 2.0 Keywords:
 ppo,transformers,huggingface,gpt2,language modeling,rlhf Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
@@ -99,16 +99,16 @@
 (query_txt, return_tensors="pt") # get model response response_tensor =
 respond_to_batch(model, query_tensor) # create a ppo trainer ppo_trainer =
 PPOTrainer(ppo_config, model, model_ref, tokenizer) # define a reward for
 response # (this could be any reward such as human feedback or output from
 another model) reward = [torch.tensor(1.0)] # train model for one step with ppo
 train_stats = ppo_trainer.step([query_tensor[0]], [response_tensor[0]], reward)
 ``` ### Advanced example: IMDB sentiment For a detailed example check out the
-example python script `examples/sentiment/scripts/gpt2-sentiment.py`, where
-GPT2 is fine-tuned to generate positive movie reviews. An few examples from the
+example python script `examples/scripts/sentiment_tuning.py`, where GPT2 is
+fine-tuned to generate positive movie reviews. An few examples from the
 language models before and after optimisation are given below:
 [https://huggingface.co/datasets/trl-internal-testing/example-images/resolve/
 main/images/table_imdb_preview.png]
 Figure: A few review continuations before and after optimisation.
 Have a look at more examples inside [`examples/`](https://github.com/lvwerra/
 trl/tree/main/examples) folder. ## References ### Proximal Policy Optimisation
 The PPO implementation largely follows the structure introduced in the paper
```

### Comparing `trl-0.4.7/trl.egg-info/SOURCES.txt` & `trl-0.5.0/trl.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 tests/__init__.py
 tests/test_best_of_n_sampler.py
 tests/test_core.py
+tests/test_dpo_trainer.py
 tests/test_e2e.py
 tests/test_modeling_value_head.py
 tests/test_no_peft.py
 tests/test_peft_models.py
 tests/test_ppo_trainer.py
 tests/test_reward_trainer.py
 tests/test_sft_trainer.py
@@ -28,12 +29,13 @@
 trl/extras/__init__.py
 trl/extras/best_of_n_sampler.py
 trl/models/__init__.py
 trl/models/modeling_base.py
 trl/models/modeling_value_head.py
 trl/trainer/__init__.py
 trl/trainer/base.py
+trl/trainer/dpo_trainer.py
 trl/trainer/ppo_config.py
 trl/trainer/ppo_trainer.py
 trl/trainer/reward_trainer.py
 trl/trainer/sft_trainer.py
 trl/trainer/utils.py
```

