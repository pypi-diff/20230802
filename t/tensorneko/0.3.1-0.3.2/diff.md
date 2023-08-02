# Comparing `tmp/tensorneko-0.3.1.tar.gz` & `tmp/tensorneko-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorneko-0.3.1.tar", last modified: Fri Jul 28 09:05:59 2023, max compression
+gzip compressed data, was "tensorneko-0.3.2.tar", last modified: Wed Aug  2 12:19:56 2023, max compression
```

## Comparing `tensorneko-0.3.1.tar` & `tensorneko-0.3.2.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.803948 tensorneko-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-28 09:03:02.000000 tensorneko-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    18248 2023-07-28 09:05:59.799948 tensorneko-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17201 2023-07-28 09:03:02.000000 tensorneko-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-28 09:05:59.803948 tensorneko-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-07-28 09:03:02.000000 tensorneko-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.775948 tensorneko-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.775948 tensorneko-0.3.1/src/tensorneko/
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.783948 tensorneko-0.3.1/src/tensorneko/arch/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/arch/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)     7205 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/arch/gan.py
--rw-r--r--   0 runner    (1001) docker     (122)     3730 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/arch/vqvae.py
--rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/arch/wgan.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.783948 tensorneko-0.3.1/src/tensorneko/backend/
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.783948 tensorneko-0.3.1/src/tensorneko/callback/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/display_metrics_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/earlystop_lr.py
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/epoch_num_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/epoch_time_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/gpu_stats_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/lr_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/nil_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/callback/system_stats_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.787948 tensorneko-0.3.1/src/tensorneko/dataset/
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      942 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/dataset/nested_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/dataset/round_robin_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.787948 tensorneko-0.3.1/src/tensorneko/debug/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/debug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.787948 tensorneko-0.3.1/src/tensorneko/evaluation/
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/evaluation/enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/evaluation/fid.py
--rw-r--r--   0 runner    (1001) docker     (122)     2914 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/evaluation/iou.py
--rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/evaluation/psnr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/evaluation/ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.787948 tensorneko-0.3.1/src/tensorneko/io/
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.787948 tensorneko-0.3.1/src/tensorneko/io/mesh/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/io/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/io/mesh/mesh_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/io/mesh/mesh_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/io/reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/io/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.791948 tensorneko-0.3.1/src/tensorneko/layer/
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1177 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (122)     6360 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/attention.py
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/conv.py
--rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     4796 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/masked_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/noise.py
--rw-r--r--   0 runner    (1001) docker     (122)     6585 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/patching.py
--rw-r--r--   0 runner    (1001) docker     (122)     4283 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/positional_embedding.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/reshape.py
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/stack.py
--rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/layer/vector_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.795948 tensorneko-0.3.1/src/tensorneko/module/
--rw-r--r--   0 runner    (1001) docker     (122)      403 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/dense.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/gated_conv.py
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/inception.py
--rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/mlp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/residual.py
--rw-r--r--   0 runner    (1001) docker     (122)     7602 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/module/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     9927 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/neko_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/neko_module.py
--rw-r--r--   0 runner    (1001) docker     (122)    10007 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/neko_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.795948 tensorneko-0.3.1/src/tensorneko/notebook/
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.795948 tensorneko-0.3.1/src/tensorneko/optim/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.795948 tensorneko-0.3.1/src/tensorneko/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/optim/lr_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.795948 tensorneko-0.3.1/src/tensorneko/preprocess/
--rw-r--r--   0 runner    (1001) docker     (122)      808 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/preprocess/crop.py
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/preprocess/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.795948 tensorneko-0.3.1/src/tensorneko/preprocess/face_detector/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/preprocess/face_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/preprocess/pad.py
--rw-r--r--   0 runner    (1001) docker     (122)     3469 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/preprocess/resize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.799948 tensorneko-0.3.1/src/tensorneko/util/
--rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/dispatched_misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4565 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/string_getter.py
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/util/type.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-28 09:05:59.000000 tensorneko-0.3.1/src/tensorneko/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.799948 tensorneko-0.3.1/src/tensorneko/visualization/
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.799948 tensorneko-0.3.1/src/tensorneko/visualization/image_browser/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/visualization/image_browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/visualization/log_graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/visualization/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.799948 tensorneko-0.3.1/src/tensorneko/visualization/watcher/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-28 09:03:02.000000 tensorneko-0.3.1/src/tensorneko/visualization/watcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.775948 tensorneko-0.3.1/src/tensorneko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    18248 2023-07-28 09:05:59.000000 tensorneko-0.3.1/src/tensorneko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-28 09:05:59.000000 tensorneko-0.3.1/src/tensorneko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 09:05:59.000000 tensorneko-0.3.1/src/tensorneko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-28 09:05:59.000000 tensorneko-0.3.1/src/tensorneko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-28 09:05:59.000000 tensorneko-0.3.1/src/tensorneko.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:59.799948 tensorneko-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-28 09:03:02.000000 tensorneko-0.3.1/test/test_library_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-28 09:03:02.000000 tensorneko-0.3.1/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.366519 tensorneko-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-08-02 12:16:45.000000 tensorneko-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    18248 2023-08-02 12:19:56.366519 tensorneko-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17201 2023-08-02 12:16:45.000000 tensorneko-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-02 12:19:56.366519 tensorneko-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-08-02 12:16:45.000000 tensorneko-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.334516 tensorneko-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.338516 tensorneko-0.3.2/src/tensorneko/
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.342517 tensorneko-0.3.2/src/tensorneko/arch/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/arch/auto_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7205 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/arch/gan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3730 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/arch/vqvae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/arch/wgan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.342517 tensorneko-0.3.2/src/tensorneko/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.346517 tensorneko-0.3.2/src/tensorneko/callback/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/callback/display_metrics_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/callback/earlystop_lr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/callback/epoch_num_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/callback/epoch_time_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/callback/gpu_stats_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/callback/lr_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/callback/nil_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/callback/system_stats_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.346517 tensorneko-0.3.2/src/tensorneko/dataset/
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/dataset/nested_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/dataset/round_robin_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.346517 tensorneko-0.3.2/src/tensorneko/debug/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/debug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.350518 tensorneko-0.3.2/src/tensorneko/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/evaluation/enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/evaluation/fid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2914 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/evaluation/iou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/evaluation/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/evaluation/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.350518 tensorneko-0.3.2/src/tensorneko/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.350518 tensorneko-0.3.2/src/tensorneko/io/mesh/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/io/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/io/mesh/mesh_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/io/mesh/mesh_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      705 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/io/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.358518 tensorneko-0.3.2/src/tensorneko/layer/
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1177 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6360 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4796 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/masked_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/noise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6585 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4283 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/positional_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/stack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/layer/vector_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.358518 tensorneko-0.3.2/src/tensorneko/module/
+-rw-r--r--   0 runner    (1001) docker     (122)      403 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/module/dense.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/module/gated_conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/module/inception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/module/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/module/residual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7602 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/module/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10105 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/neko_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/neko_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9972 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/neko_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.358518 tensorneko-0.3.2/src/tensorneko/notebook/
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.362519 tensorneko-0.3.2/src/tensorneko/optim/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.362519 tensorneko-0.3.2/src/tensorneko/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/optim/lr_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.362519 tensorneko-0.3.2/src/tensorneko/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (122)      808 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/preprocess/crop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/preprocess/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.362519 tensorneko-0.3.2/src/tensorneko/preprocess/face_detector/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/preprocess/face_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/preprocess/pad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3469 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/preprocess/resize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.366519 tensorneko-0.3.2/src/tensorneko/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/util/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/util/dispatched_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4565 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/util/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/util/string_getter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/util/type.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-02 12:19:56.000000 tensorneko-0.3.2/src/tensorneko/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.366519 tensorneko-0.3.2/src/tensorneko/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.366519 tensorneko-0.3.2/src/tensorneko/visualization/image_browser/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/visualization/image_browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/visualization/log_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/visualization/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.366519 tensorneko-0.3.2/src/tensorneko/visualization/watcher/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-08-02 12:16:45.000000 tensorneko-0.3.2/src/tensorneko/visualization/watcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.338516 tensorneko-0.3.2/src/tensorneko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    18248 2023-08-02 12:19:56.000000 tensorneko-0.3.2/src/tensorneko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-08-02 12:19:56.000000 tensorneko-0.3.2/src/tensorneko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 12:19:56.000000 tensorneko-0.3.2/src/tensorneko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-08-02 12:19:56.000000 tensorneko-0.3.2/src/tensorneko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-08-02 12:19:56.000000 tensorneko-0.3.2/src/tensorneko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:56.366519 tensorneko-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-08-02 12:16:45.000000 tensorneko-0.3.2/test/test_library_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-08-02 12:16:45.000000 tensorneko-0.3.2/test/test_version.py
```

### Comparing `tensorneko-0.3.1/LICENSE` & `tensorneko-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/PKG-INFO` & `tensorneko-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorneko
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
```

### Comparing `tensorneko-0.3.1/README.md` & `tensorneko-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/setup.py` & `tensorneko-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/__init__.py` & `tensorneko-0.3.2/src/tensorneko/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/arch/auto_encoder.py` & `tensorneko-0.3.2/src/tensorneko/arch/auto_encoder.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/arch/gan.py` & `tensorneko-0.3.2/src/tensorneko/arch/gan.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/arch/vqvae.py` & `tensorneko-0.3.2/src/tensorneko/arch/vqvae.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/arch/wgan.py` & `tensorneko-0.3.2/src/tensorneko/arch/wgan.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/callback/__init__.py` & `tensorneko-0.3.2/src/tensorneko/callback/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/callback/earlystop_lr.py` & `tensorneko-0.3.2/src/tensorneko/callback/earlystop_lr.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/callback/epoch_time_logger.py` & `tensorneko-0.3.2/src/tensorneko/callback/epoch_time_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/callback/gpu_stats_logger.py` & `tensorneko-0.3.2/src/tensorneko/callback/gpu_stats_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,11 +21,11 @@
                 f"gpu{gpu.index}_memory_used": gpu.memory_used / 1024,
                 f"gpu{gpu.index}_memory_total": gpu.memory_total / 1024,
                 f"gpu{gpu.index}_memory_util": gpu.memory_used / gpu.memory_total,
                 f"gpu{gpu.index}_temperature": float(gpu.temperature),
                 f"gpu{gpu.index}_utilization": gpu.utilization / 100,
                 f"gpu{gpu.index}_power_draw": float(gpu.power_draw),
                 f"gpu{gpu.index}_power_percentage": gpu.power_draw / gpu.power_limit,
-                f"gpu{gpu.index}_fan_speed": float(gpu.fan_speed),
+                f"gpu{gpu.index}_fan_speed": float(gpu.fan_speed) if gpu.fan_speed is not None else 0.,
             }
             pl_module.logger.log_metrics(logged_info, step=trainer.global_step)
             pl_module.log_dict(logged_info, logger=False, sync_dist=pl_module.distributed)
```

### Comparing `tensorneko-0.3.1/src/tensorneko/callback/lr_logger.py` & `tensorneko-0.3.2/src/tensorneko/callback/lr_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/callback/system_stats_logger.py` & `tensorneko-0.3.2/src/tensorneko/callback/system_stats_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/dataset/nested_dataset.py` & `tensorneko-0.3.2/src/tensorneko/dataset/nested_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/dataset/round_robin_dataset.py` & `tensorneko-0.3.2/src/tensorneko/dataset/round_robin_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/evaluation/fid.py` & `tensorneko-0.3.2/src/tensorneko/evaluation/fid.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/evaluation/iou.py` & `tensorneko-0.3.2/src/tensorneko/evaluation/iou.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/evaluation/psnr.py` & `tensorneko-0.3.2/src/tensorneko/evaluation/psnr.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/evaluation/ssim.py` & `tensorneko-0.3.2/src/tensorneko/evaluation/ssim.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/io/reader.py` & `tensorneko-0.3.2/src/tensorneko/io/reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/io/writer.py` & `tensorneko-0.3.2/src/tensorneko/io/writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/__init__.py` & `tensorneko-0.3.2/src/tensorneko/layer/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/aggregation.py` & `tensorneko-0.3.2/src/tensorneko/layer/aggregation.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/attention.py` & `tensorneko-0.3.2/src/tensorneko/layer/attention.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/concatenate.py` & `tensorneko-0.3.2/src/tensorneko/layer/concatenate.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/conv.py` & `tensorneko-0.3.2/src/tensorneko/layer/conv.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/linear.py` & `tensorneko-0.3.2/src/tensorneko/layer/linear.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/log.py` & `tensorneko-0.3.2/src/tensorneko/layer/log.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/masked_conv2d.py` & `tensorneko-0.3.2/src/tensorneko/layer/masked_conv2d.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/noise.py` & `tensorneko-0.3.2/src/tensorneko/layer/noise.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/patching.py` & `tensorneko-0.3.2/src/tensorneko/layer/patching.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/positional_embedding.py` & `tensorneko-0.3.2/src/tensorneko/layer/positional_embedding.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/reshape.py` & `tensorneko-0.3.2/src/tensorneko/layer/reshape.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/stack.py` & `tensorneko-0.3.2/src/tensorneko/layer/stack.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/layer/vector_quantizer.py` & `tensorneko-0.3.2/src/tensorneko/layer/vector_quantizer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/module/dense.py` & `tensorneko-0.3.2/src/tensorneko/module/dense.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/module/gated_conv.py` & `tensorneko-0.3.2/src/tensorneko/module/gated_conv.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/module/inception.py` & `tensorneko-0.3.2/src/tensorneko/module/inception.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/module/mlp.py` & `tensorneko-0.3.2/src/tensorneko/module/mlp.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/module/residual.py` & `tensorneko-0.3.2/src/tensorneko/module/residual.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/module/transformer.py` & `tensorneko-0.3.2/src/tensorneko/module/transformer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/neko_model.py` & `tensorneko-0.3.2/src/tensorneko/neko_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -239,7 +239,11 @@
 
     def log_image(self, name: str, image: torch.Tensor) -> None:
         """Log an image to the logger"""
         if self.logger is None:
             return
 
         self.logger.experiment.add_image(name, torch.clip(image, 0, 1), self.trainer.global_step)
+
+    def on_train_start(self) -> None:
+        """Log the model graph to tensorboard when the input shape is set"""
+        self.logger.log_graph(self, self.example_input_array)
```

### Comparing `tensorneko-0.3.1/src/tensorneko/neko_module.py` & `tensorneko-0.3.2/src/tensorneko/neko_module.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/neko_trainer.py` & `tensorneko-0.3.2/src/tensorneko/neko_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,16 +211,15 @@
         #     move_metrics_to_cpu=move_metrics_to_cpu,
         #     multiple_trainloader_mode=multiple_trainloader_mode
         # )
         # init loggers for training and validation
         self.has_no_logger = logger is None
 
         self.logger_train = TensorBoardLogger(save_dir=self.default_root_dir, name="logs",
-            version=os.path.join(self.log_name, "train"), log_graph=False
-            # TODO: Fix log_Graph
+            version=os.path.join(self.log_name, "train"), log_graph=True
         ) if self.has_no_logger is not None else None
         self.logger_val = TensorBoardLogger(save_dir=self.default_root_dir, name="logs",
             version=os.path.join(self.log_name, "val"), log_graph=False
         ) if self.has_no_logger is not None else None
         self._loggers = []
 
     @property
```

### Comparing `tensorneko-0.3.1/src/tensorneko/preprocess/__init__.py` & `tensorneko-0.3.2/src/tensorneko/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/preprocess/crop.py` & `tensorneko-0.3.2/src/tensorneko/preprocess/crop.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/preprocess/enum.py` & `tensorneko-0.3.2/src/tensorneko/preprocess/enum.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/preprocess/pad.py` & `tensorneko-0.3.2/src/tensorneko/preprocess/pad.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/preprocess/resize.py` & `tensorneko-0.3.2/src/tensorneko/preprocess/resize.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/util/__init__.py` & `tensorneko-0.3.2/src/tensorneko/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/util/configuration.py` & `tensorneko-0.3.2/src/tensorneko/util/configuration.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/util/dispatched_misc.py` & `tensorneko-0.3.2/src/tensorneko/util/dispatched_misc.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/util/misc.py` & `tensorneko-0.3.2/src/tensorneko/util/misc.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/util/reproducibility.py` & `tensorneko-0.3.2/src/tensorneko/util/reproducibility.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/util/string_getter.py` & `tensorneko-0.3.2/src/tensorneko/util/string_getter.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/util/type.py` & `tensorneko-0.3.2/src/tensorneko/util/type.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/visualization/__init__.py` & `tensorneko-0.3.2/src/tensorneko/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/visualization/log_graph.py` & `tensorneko-0.3.2/src/tensorneko/visualization/log_graph.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko/visualization/matplotlib.py` & `tensorneko-0.3.2/src/tensorneko/visualization/matplotlib.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/src/tensorneko.egg-info/PKG-INFO` & `tensorneko-0.3.2/src/tensorneko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorneko
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
```

### Comparing `tensorneko-0.3.1/src/tensorneko.egg-info/SOURCES.txt` & `tensorneko-0.3.2/src/tensorneko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.1/test/test_version.py` & `tensorneko-0.3.2/test/test_version.py`

 * *Files identical despite different names*

