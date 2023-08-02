# Comparing `tmp/ml-starter-0.1.44.tar.gz` & `tmp/ml-starter-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.44.tar", last modified: Tue Aug  1 22:39:20 2023, max compression
+gzip compressed data, was "ml-starter-0.1.45.tar", last modified: Wed Aug  2 19:28:08 2023, max compression
```

## Comparing `ml-starter-0.1.44.tar` & `ml-starter-0.1.45.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.734885 ml-starter-0.1.44/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-01 22:39:08.000000 ml-starter-0.1.44/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-01 22:39:08.000000 ml-starter-0.1.44/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-01 22:39:20.734885 ml-starter-0.1.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-01 22:39:08.000000 ml-starter-0.1.44/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.718885 ml-starter-0.1.44/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.718885 ml-starter-0.1.44/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.718885 ml-starter-0.1.44/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/launchers/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.718885 ml-starter-0.1.44/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.718885 ml-starter-0.1.44/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/lr_schedulers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.718885 ml-starter-0.1.44/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.722885 ml-starter-0.1.44/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.722885 ml-starter-0.1.44/ml/models/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/architectures/bifpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/architectures/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/codebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.722885 ml-starter-0.1.44/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/optimizers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.722885 ml-starter-0.1.44/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.722885 ml-starter-0.1.44/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.726885 ml-starter-0.1.44/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.726885 ml-starter-0.1.44/ml/tasks/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/diffusion/beta_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/diffusion/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.726885 ml-starter-0.1.44/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.726885 ml-starter-0.1.44/ml/tasks/gan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/gan/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.726885 ml-starter-0.1.44/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/losses/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/losses/kl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/losses/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.726885 ml-starter-0.1.44/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.726885 ml-starter-0.1.44/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.726885 ml-starter-0.1.44/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24976 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.730885 ml-starter-0.1.44/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.734885 ml-starter-0.1.44/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.734885 ml-starter-0.1.44/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.734885 ml-starter-0.1.44/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-01 22:39:08.000000 ml-starter-0.1.44/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:39:20.734885 ml-starter-0.1.44/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-01 22:39:20.000000 ml-starter-0.1.44/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-01 22:39:20.000000 ml-starter-0.1.44/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:39:20.000000 ml-starter-0.1.44/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-01 22:39:20.000000 ml-starter-0.1.44/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-01 22:39:20.000000 ml-starter-0.1.44/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-01 22:39:08.000000 ml-starter-0.1.44/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-01 22:39:20.734885 ml-starter-0.1.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-01 22:39:08.000000 ml-starter-0.1.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.282239 ml-starter-0.1.45/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 19:27:54.000000 ml-starter-0.1.45/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-02 19:27:54.000000 ml-starter-0.1.45/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-02 19:28:08.282239 ml-starter-0.1.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-02 19:27:54.000000 ml-starter-0.1.45/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.262239 ml-starter-0.1.45/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.262239 ml-starter-0.1.45/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.262239 ml-starter-0.1.45/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/launchers/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.262239 ml-starter-0.1.45/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.266239 ml-starter-0.1.45/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.266239 ml-starter-0.1.45/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.266239 ml-starter-0.1.45/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.266239 ml-starter-0.1.45/ml/models/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/architectures/bifpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/architectures/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/tasks/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/diffusion/beta_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/diffusion/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/tasks/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/gan/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.274239 ml-starter-0.1.45/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/losses/kl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/losses/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.274239 ml-starter-0.1.45/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.274239 ml-starter-0.1.45/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.274239 ml-starter-0.1.45/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27997 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.274239 ml-starter-0.1.45/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.278239 ml-starter-0.1.45/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.278239 ml-starter-0.1.45/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.282239 ml-starter-0.1.45/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.282239 ml-starter-0.1.45/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-02 19:28:08.000000 ml-starter-0.1.45/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-02 19:28:08.000000 ml-starter-0.1.45/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:28:08.000000 ml-starter-0.1.45/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-02 19:28:08.000000 ml-starter-0.1.45/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-02 19:28:08.000000 ml-starter-0.1.45/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-02 19:27:54.000000 ml-starter-0.1.45/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-02 19:28:08.282239 ml-starter-0.1.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-02 19:27:54.000000 ml-starter-0.1.45/setup.py
```

### Comparing `ml-starter-0.1.44/LICENSE` & `ml-starter-0.1.45/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/PKG-INFO` & `ml-starter-0.1.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.44
+Version: 0.1.45
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.44/README.md` & `ml-starter-0.1.45/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/api.py` & `ml-starter-0.1.45/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/core/common_types.py` & `ml-starter-0.1.45/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/core/config.py` & `ml-starter-0.1.45/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/core/env.py` & `ml-starter-0.1.45/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/core/registry.py` & `ml-starter-0.1.45/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/core/state.py` & `ml-starter-0.1.45/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/launchers/base.py` & `ml-starter-0.1.45/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/launchers/mp.py` & `ml-starter-0.1.45/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/launchers/sagemaker.py` & `ml-starter-0.1.45/ml/launchers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/launchers/slurm.py` & `ml-starter-0.1.45/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/launchers/torchrun.py` & `ml-starter-0.1.45/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/loggers/base.py` & `ml-starter-0.1.45/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/loggers/meter.py` & `ml-starter-0.1.45/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/loggers/multi.py` & `ml-starter-0.1.45/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/loggers/stdout.py` & `ml-starter-0.1.45/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/loggers/tensorboard.py` & `ml-starter-0.1.45/ml/loggers/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     rows_str = "\n".join(["| " + " | ".join(row) + " |" for row in rows])
     return "\n".join([header_str, header_sep_str, rows_str])
 
 
 @dataclass
 class TensorboardLoggerConfig(BaseLoggerConfig):
     flush_seconds: float = conf_field(10.0, help="How often to flush logs")
-    wait_seconds: float = conf_field(10.0, help="Time to wait before starting Tensorboard process")
+    wait_seconds: float = conf_field(0.0, help="Time to wait before starting Tensorboard process")
     log_id: str = conf_field(MISSING, help="Unique log ID")
     start_in_subprocess: bool = conf_field(True, help="Start TensorBoard subprocess")
 
     @classmethod
     def resolve(cls, config: "TensorboardLoggerConfig") -> None:
         if OmegaConf.is_missing(config, "log_id"):
             config.log_id = datetime.datetime.now().strftime("%H-%M-%S")
```

### Comparing `ml-starter-0.1.44/ml/lr_schedulers/base.py` & `ml-starter-0.1.45/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/lr_schedulers/constant.py` & `ml-starter-0.1.45/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.45/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.45/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/lr_schedulers/gan.py` & `ml-starter-0.1.45/ml/lr_schedulers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/lr_schedulers/linear.py` & `ml-starter-0.1.45/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.45/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.45/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/activations.py` & `ml-starter-0.1.45/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/architectures/bifpn.py` & `ml-starter-0.1.45/ml/models/architectures/bifpn.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/architectures/unet.py` & `ml-starter-0.1.45/ml/models/architectures/unet.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/base.py` & `ml-starter-0.1.45/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/codebook.py` & `ml-starter-0.1.45/ml/models/codebook.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/embeddings.py` & `ml-starter-0.1.45/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/gan.py` & `ml-starter-0.1.45/ml/models/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/init.py` & `ml-starter-0.1.45/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/kmeans.py` & `ml-starter-0.1.45/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/lora.py` & `ml-starter-0.1.45/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/modules.py` & `ml-starter-0.1.45/ml/models/modules.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/norms.py` & `ml-starter-0.1.45/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/models/parallel.py` & `ml-starter-0.1.45/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/optimizers/adam.py` & `ml-starter-0.1.45/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/optimizers/adan.py` & `ml-starter-0.1.45/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/optimizers/base.py` & `ml-starter-0.1.45/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/optimizers/common.py` & `ml-starter-0.1.45/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/optimizers/gan.py` & `ml-starter-0.1.45/ml/optimizers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/optimizers/lion.py` & `ml-starter-0.1.45/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/optimizers/sgd.py` & `ml-starter-0.1.45/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/optimizers/shampoo.py` & `ml-starter-0.1.45/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/scripts/cli.py` & `ml-starter-0.1.45/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/scripts/stage.py` & `ml-starter-0.1.45/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/scripts/train.py` & `ml-starter-0.1.45/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/base.py` & `ml-starter-0.1.45/ml/tasks/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,17 +477,14 @@
     def collate_fn(cls, items: list[Any], *, mode: CollateMode = "stack") -> Any | None:  # noqa: ANN401
         return collate(items, mode=mode)
 
     # -----
     # Hooks
     # -----
 
-    def on_after_load_checkpoint(self, ckpt: dict[str, Any]) -> None:
-        pass
-
     def on_after_save_checkpoint(self, ckpt_path: Path) -> None:
         pass
 
     def on_before_forward_step(self, model: ModelT, batch: Batch, state: State) -> None:
         pass
 
     def on_after_forward_step(self, model: ModelT, batch: Batch, output: Output, state: State) -> None:
```

### Comparing `ml-starter-0.1.44/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.45/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.45/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/datasets/collate.py` & `ml-starter-0.1.45/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.45/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.45/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.45/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.45/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.45/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.45/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/diffusion/beta_schedule.py` & `ml-starter-0.1.45/ml/tasks/diffusion/beta_schedule.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/diffusion/gaussian.py` & `ml-starter-0.1.45/ml/tasks/diffusion/gaussian.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/environments/base.py` & `ml-starter-0.1.45/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/environments/utils.py` & `ml-starter-0.1.45/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/environments/worker.py` & `ml-starter-0.1.45/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/gan/base.py` & `ml-starter-0.1.45/ml/tasks/gan/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/losses/audio.py` & `ml-starter-0.1.45/ml/tasks/losses/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/losses/image.py` & `ml-starter-0.1.45/ml/tasks/losses/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/losses/kl.py` & `ml-starter-0.1.45/ml/tasks/losses/kl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/losses/loss.py` & `ml-starter-0.1.45/ml/tasks/losses/loss.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/rl/base.py` & `ml-starter-0.1.45/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/rl/replay.py` & `ml-starter-0.1.45/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/tasks/sl/base.py` & `ml-starter-0.1.45/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/trainers/base.py` & `ml-starter-0.1.45/ml/trainers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 requires interacting with an environment, so you use the appropriate trainer
 for your task (they are defined in :mod:`ml.trainers.sl` and
 :mod:`ml.trainers.rl` respectively). The base trainer handles things like
 setting up the experiment directory, saving checkpoints, and logging.
 """
 
 import enum
+import itertools
+import json
 import logging
 import os
 import signal
 import time
 from dataclasses import asdict, dataclass
 from pathlib import Path
-from pickle import UnpicklingError
 from typing import Any, Callable, Generic, Literal, TypeVar, cast, get_args
 
+import safetensors
 import torch
 from omegaconf import II, MISSING, DictConfig, ListConfig, OmegaConf
-from torch import Tensor
+from safetensors.torch import _remove_duplicate_names, save_file as safetensors_save_file
+from torch import Tensor, nn
 from torch.optim.optimizer import Optimizer
-from torch.serialization import MAP_LOCATION
 
 from ml.core.config import BaseConfig, BaseObject, conf_field
 from ml.core.env import get_ml_config_path
 from ml.core.state import State
 from ml.loggers.base import BaseLogger
 from ml.loggers.multi import MultiLogger
 from ml.lr_schedulers.base import BaseLRScheduler, SchedulerAdapter
@@ -218,14 +220,16 @@
 
 @dataclass
 class CheckpointConfig:
     save_every_n_steps: int | None = conf_field(None, help="Save a checkpoint every N steps")
     save_every_n_seconds: int | None = conf_field(None, help="Save a checkpoint every N seconds")
     only_save_most_recent: bool = conf_field(False, help="Only keep the most recent checkpoint")
     load_from_ckpt_path: str | None = conf_field(None, help="If set, load initial model weights from this path")
+    save_no_grad: bool = conf_field(False, help="If set, also save tensors which don't require gradients")
+    load_strict: bool = conf_field(True, help="If set, only load weights for which have a matching key in the model")
 
 
 @dataclass
 class BaseTrainerConfig(BaseConfig):
     """Defines the base config for all trainers."""
 
     exp_name: str = conf_field(II("ml.exp_name:null"), help="The name of the training job")
@@ -340,109 +344,122 @@
             if cur_time - last_time >= self.checkpoint_config.save_every_n_seconds:
                 self.__last_ckpt_time = cur_time
                 return True
         return False
 
     def load_checkpoint(
         self,
-        ckpt: str | Path | dict,
+        ckpt: str | Path,
         task: TaskT,
         model: ModelT,
         optims: Optimizer | dict[str, Optimizer] | None = None,
         lr_scheds: SchedulerAdapter | dict[str, SchedulerAdapter] | None = None,
         *,
-        weights_only: bool = True,
-        map_location: MAP_LOCATION = None,
+        device: str = "cpu",
+        strict: bool | None = None,
     ) -> State:
         """Loads a given checkpoint, from a path or dictionary.
 
         Args:
             ckpt: The checkpoint to load.
             task: The task to load the checkpoint into.
             model: The model to load the checkpoint into.
             optims: The optimizer to load the checkpoint into.
             lr_scheds: The learning rate scheduler to load the checkpoint into.
             weights_only: If set, only load the model weights.
-            map_location: The location to map the loaded checkpoint to.
+            device: The device to load the checkpoint onto.
+            strict: If set, raise an error if the checkpoint contains keys which
+                don't exist in the model.
 
         Returns:
             The state loaded from the checkpoint.
 
         Raises:
             UnpicklingError: If there is some issue unpickling the checkpoint.
         """
+        strict_non_none = self.config.checkpoint.load_strict if strict is None else strict
+
         with Timer("loading checkpoint", spinner=True):
-            if isinstance(ckpt, (str, Path)):
-                try:
-                    ckpt = cast(dict, torch.load(ckpt, weights_only=weights_only, map_location=map_location))
-                except UnpicklingError:
-                    if weights_only:
-                        logger.warning("Failed to load checkpoint using `weights_only` flag, retrying without it")
-                        ckpt = cast(
-                            dict,
-                            torch.load(
-                                cast(str | Path, ckpt),
-                                weights_only=False,
-                                map_location=map_location,
-                            ),
-                        )
-                    else:
-                        raise
 
             def try_load_state_dict(model: ModelT, state_dict: dict[str, Any]) -> bool:
                 try:
-                    model.load_state_dict(state_dict)
+                    model.load_state_dict(state_dict, strict=strict_non_none)
                     return True
                 except RuntimeError as e:
                     if not str(e).startswith("Error(s) in loading state_dict for"):
                         raise
                     return False
 
-            def load_model_state_dict(model: ModelT, state_dict: dict[str, Any]) -> None:
+            def load_model_state_dict(model: ModelT, state_dict: dict[str, Tensor]) -> None:
                 if try_load_state_dict(model, state_dict):
                     return
 
                 for prefix in ("module.", "_orig_mod."):
                     if try_load_state_dict(model, {k[len(prefix) :]: v for k, v in state_dict.items()}):
                         return
                     if try_load_state_dict(model, {f"{prefix}{k}": v for k, v in state_dict.items()}):
                         return
 
                 # Final call, just to throw the error if it still fails.
-                model.load_state_dict(state_dict)
+                model.load_state_dict(state_dict, strict=strict_non_none)
 
-            task.on_after_load_checkpoint(ckpt)
-            if "model" in ckpt:
-                load_model_state_dict(model, ckpt["model"])
+            with safetensors.safe_open(ckpt, framework="pt", device=device) as f:
+                ckpt_tensors: dict[str, Tensor] = {}
+                for k in f.keys():
+                    ckpt_tensors[k] = f.get_tensor(k)
+                metadata = f.metadata()
+
+            # Copies back removed pointers.
+            if "removed" in metadata:
+                for removed_name, kept_name in json.loads(metadata["removed"]).items():
+                    if kept_name in ckpt_tensors:
+                        ckpt_tensors[removed_name] = ckpt_tensors[kept_name]
+
+            def has_prefix(prefix: str) -> bool:
+                return any(k.startswith(prefix) for k in itertools.chain(ckpt_tensors.keys(), metadata.keys()))
+
+            def prefixed_state_dict(key: str) -> dict[str, Any]:
+                prefix = f"{key}."
+                return {
+                    **{k[len(prefix) :]: v for k, v in ckpt_tensors.items() if k.startswith(prefix)},
+                    **json.loads(metadata.get(key, "{}")),
+                }
+
+            if has_prefix("model."):
+                load_model_state_dict(model, prefixed_state_dict("model"))
             else:
                 logger.warning("Checkpoint does not contain a model state dict")
-            if "task" in ckpt:
-                task.load_state_dict(ckpt["task"])
+
+            if has_prefix("task."):
+                task.load_state_dict(prefixed_state_dict("task"))
             else:
                 logger.warning("Checkpoint does not contain a task state dict")
+
             if optims is not None:
-                if "optim" in ckpt:
+                if has_prefix("optim."):
                     if isinstance(optims, dict):
                         for name, optim in optims.items():
-                            optim.load_state_dict(ckpt["optim"][name])
+                            optim.load_state_dict(prefixed_state_dict(f"optim.{name}"))
                     else:
-                        optims.load_state_dict(ckpt["optim"])
+                        optims.load_state_dict(prefixed_state_dict("optim"))
                 else:
                     logger.warning("Checkpoint does not contain an optimizer state dict")
+
             if lr_scheds is not None:
-                if "lr_sched" in ckpt:
+                if has_prefix("lr."):
                     if isinstance(lr_scheds, dict):
                         for name, lr_sched in lr_scheds.items():
-                            lr_sched.load_state_dict(ckpt["lr_sched"][name])
+                            lr_sched.load_state_dict(prefixed_state_dict(f"lr.{name}."))
                     else:
-                        lr_scheds.load_state_dict(ckpt["lr_sched"])
+                        lr_scheds.load_state_dict(prefixed_state_dict("lr."))
                 else:
                     logger.warning("Checkpoint does not contain a learning rate scheduler state dict")
-            self.load_state_dict(ckpt)
-            state = State(**ckpt["state"])
+
+            self.load_state_dict(ckpt_tensors, metadata)
+            state = State(**json.loads(metadata["state"]))
 
         return state
 
     def save_checkpoint(
         self,
         state: State,
         task: TaskT,
@@ -453,43 +470,78 @@
         ckpt_path = self.get_ckpt_path(state)
         if is_master():
             with Timer("saving checkpoint", spinner=True):
                 logger.info("Saving checkpoint to %s", ckpt_path)
                 last_ckpt_path = self.get_ckpt_path()
                 ckpt_path.parent.mkdir(exist_ok=True, parents=True)
 
-                state_dict: dict[str, Any] = {
-                    "model": model.state_dict(),
-                    "task": task.state_dict(),
-                    "state": asdict(state),
-                }
+                state_dict: dict[str, Tensor] = {}
+                metadata: dict[str, str] = {}
+
+                def get_flat_dict(d: dict[str, Any]) -> dict[str, Any]:
+                    return_dict = {}
+                    for k, v in d.items():
+                        if isinstance(v, dict):
+                            return_dict.update({f"{k}.{k2}": v2 for k2, v2 in get_flat_dict(v).items()})
+                        else:
+                            return_dict[k] = v
+                    return return_dict
+
+                def get_state_dict(module: nn.Module, prefix: str) -> dict[str, Any]:
+                    parameters = module.named_parameters(prefix=prefix, recurse=True, remove_duplicate=True)
+                    save_no_grad = self.config.checkpoint.save_no_grad
+                    return {k: v for k, v in parameters if save_no_grad or v.requires_grad}
+
+                def add_state_dict(key: str, sd: dict[str, Any]) -> None:
+                    sd = get_flat_dict(sd)
+                    state_dict.update({k: v for k, v in sd.items() if isinstance(v, Tensor)})
+                    metadata[key] = json.dumps({k: v for k, v in sd.items() if not isinstance(v, Tensor)})
+
+                add_state_dict("model", get_state_dict(model, "model"))
+                add_state_dict("task", get_state_dict(task, "task"))
+
+                metadata["state"] = json.dumps(asdict(state))
 
                 if optims is not None:
                     if isinstance(optims, dict):
-                        state_dict["optim"] = {k: v.state_dict() for k, v in optims.items()}
+                        osd = {f"optim.{k}.{kk}": vv for k, v in optims.items() for kk, vv in v.state_dict().items()}
                     else:
-                        state_dict["optim"] = optims.state_dict()
+                        osd = {f"optim.{k}": v for k, v in optims.state_dict().items()}
+                    add_state_dict("optim", osd)
 
                 if lr_scheds is not None:
                     if isinstance(lr_scheds, dict):
-                        state_dict["lr_sched"] = {k: v.state_dict() for k, v in lr_scheds.items()}
+                        lrsd = {f"lr.{k}.{kk}": vv for k, v in lr_scheds.items() for kk, vv in v.state_dict().items()}
                     else:
-                        state_dict["lr_sched"] = lr_scheds.state_dict()
+                        lrsd = {f"lr.{k}": v for k, v in lr_scheds.state_dict().items()}
+                    add_state_dict("lr", lrsd)
 
                 if self._raw_config is not None:
-                    state_dict["config"] = OmegaConf.to_container(self._raw_config, enum_to_str=True)
-                self.update_state_dict(state_dict)
+                    metadata["config"] = OmegaConf.to_yaml(self._raw_config)
+
+                # Removes duplicate tensors.
+                to_removes = _remove_duplicate_names(state_dict)
+                removed: dict[str, str] = {}
+                for kept_name, to_remove_group in to_removes.items():
+                    for to_remove in to_remove_group:
+                        if to_remove not in metadata:
+                            removed[to_remove] = kept_name
+                        del state_dict[to_remove]
+                metadata["removed"] = json.dumps(removed)
+
+                self.update_state_dict(state_dict, metadata)
 
                 if last_ckpt_path.exists():
                     if self.checkpoint_config.only_save_most_recent:
                         base_ckpt = last_ckpt_path.resolve()
                         if base_ckpt.is_file():
                             base_ckpt.unlink()
                     last_ckpt_path.unlink()
-                torch.save(state_dict, ckpt_path)
+
+                safetensors_save_file(state_dict, ckpt_path, metadata)
 
                 try:
                     last_ckpt_path.symlink_to(ckpt_path)
                 except FileExistsError:
                     logger.exception("Exception while trying to update %s", ckpt_path)
                 self.add_lock_file("ckpt", exists_ok=True)
                 task.on_after_save_checkpoint(ckpt_path)
@@ -514,26 +566,28 @@
         model.logger.write(self.loggers, state)
         task.logger.write(self.loggers, state)
         self.logger.write(self.loggers, state)
         for value_logger in self.loggers:
             if value_logger.should_write(state):
                 value_logger.write(state)
 
-    def load_state_dict(self, ckpt: dict[str, Any]) -> None:
+    def load_state_dict(self, ckpt: dict[str, Tensor], metadata: dict[str, str]) -> None:
         """Function for loading state dict keys for different components.
 
         Args:
-            ckpt: The loaded state dictionary
+            ckpt: The checkpoint being saved (overriders should mutate inplace)
+            metadata: The metadata being saved (overriders should mutate inplace)
         """
 
-    def update_state_dict(self, ckpt: dict[str, Any]) -> None:
+    def update_state_dict(self, ckpt: dict[str, Tensor], metadata: dict[str, str]) -> None:
         """Function for getting the checkpoint to save.
 
         Args:
             ckpt: The checkpoint being saved (overriders should mutate inplace)
+            metadata: The metadata being saved (overriders should mutate inplace)
         """
 
     def on_exit(
         self,
         sig: signal.Signals,
         state: State,
         task: TaskT,
```

### Comparing `ml-starter-0.1.44/ml/trainers/gan.py` & `ml-starter-0.1.45/ml/trainers/gan.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from ml.models.gan import GenerativeAdversarialNetworkModel
 from ml.optimizers.base import BaseOptimizer
 from ml.optimizers.gan import GenerativeAdversarialNetworkOptimizer
 from ml.tasks.gan.base import GenerativeAdversarialNetworkTask
 from ml.trainers.sl import EpochDoneError, SupervisedLearningTrainer, SupervisedLearningTrainerConfig
 from ml.utils.containers import recursive_chunk
 from ml.utils.device.base import InfinitePrefetcher
-from ml.utils.distributed import is_distributed
 from ml.utils.exceptions import TrainingFinishedError
 from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -189,20 +188,14 @@
                             self.on_step_start(state, task, model, optims, lr_scheds)
 
                         try:
                             is_gen = task.is_generator_step(state, "train")
                             optim = gen_optim if is_gen else dis_optim
                             lr_sched = gen_lr_sched if is_gen else dis_lr_sched
 
-                            # Only disable gradients for either model if we're
-                            # not doing distributed training, because the
-                            # DDP wrapper expects to get gradients every step.
-                            if not is_distributed():
-                                model.requires_grads_(is_gen, not is_gen)
-
                             with namespace_context(self._logging_key(task, state, "train")):
                                 loss_dict = train_step(
                                     task_model=task_model,
                                     batches=batch_iterator(),
                                     state=state,
                                     task=task,
                                     model=model,
```

### Comparing `ml-starter-0.1.44/ml/trainers/learning.py` & `ml-starter-0.1.45/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/trainers/mixins/compile.py` & `ml-starter-0.1.45/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.45/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.45/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.45/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.45/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.45/ml/trainers/mixins/mixed_precision.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 FP16 scaling is a technique for training with FP16 precision while maintaining
 FP32 precision for the model weights. This is done by scaling the loss by a
 large factor (e.g. 2^16) and then scaling the gradients by the inverse of that
 factor. So if the scale factor starts to decrease, it means that the loss is
 overflowing and training is diverging.
 """
 
+import json
 import logging
 from dataclasses import dataclass
 from typing import Any, TypeVar
 
 import torch
 from torch import Tensor, nn
 from torch.distributed.fsdp.fully_sharded_data_parallel import FullyShardedDataParallel as FSDP
@@ -138,20 +139,18 @@
             self.grad_scaler.update(new_scale)
 
     def log_mp_scale(self) -> None:
         if (scaler := self.grad_scaler) is not None and scaler._enabled:
             self.logger.log_scalar("scale", scaler.get_scale, namespace="⚖️ fp16")
             self.logger.log_scalar("growth", scaler._get_growth_tracker, namespace="⚖️ fp16")
 
-    def load_state_dict(self, ckpt: dict[str, Any]) -> None:
+    def load_state_dict(self, ckpt: dict[str, Tensor], metadata: dict[str, str]) -> None:
         if self.grad_scaler is not None:
-            self.grad_scaler.load_state_dict(ckpt["grad_scaler"])
+            assert "grad_scaler" in ckpt
+            self.grad_scaler.load_state_dict(json.loads(metadata["grad_scaler"]))
+        super().load_state_dict(ckpt, metadata)
 
-        super().load_state_dict(ckpt)
-
-    def update_state_dict(self, ckpt: dict[str, Any]) -> None:
+    def update_state_dict(self, ckpt: dict[str, Tensor], metadata: dict[str, str]) -> None:
         if self.grad_scaler is not None:
             assert "grad_scaler" not in ckpt
-
-            ckpt["grad_scaler"] = self.grad_scaler.state_dict()
-
-        super().update_state_dict(ckpt)
+            metadata["grad_scaler"] = json.dumps(self.grad_scaler.state_dict())
+        super().update_state_dict(ckpt, metadata)
```

### Comparing `ml-starter-0.1.44/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.45/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.45/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.45/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/trainers/rl.py` & `ml-starter-0.1.45/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/trainers/sl.py` & `ml-starter-0.1.45/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/amp.py` & `ml-starter-0.1.45/ml/utils/amp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/argparse.py` & `ml-starter-0.1.45/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/atomic.py` & `ml-starter-0.1.45/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/attention.py` & `ml-starter-0.1.45/ml/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/audio.py` & `ml-starter-0.1.45/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/augmentation.py` & `ml-starter-0.1.45/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/caching.py` & `ml-starter-0.1.45/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/checkpoint.py` & `ml-starter-0.1.45/ml/utils/checkpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 """
 
 import logging
 import tempfile
 from pathlib import Path
 from typing import Any, Mapping, TypeVar, cast
 
-import torch
+import safetensors
+import yaml
 from omegaconf import MISSING, Container, DictConfig, OmegaConf
+from omegaconf._utils import get_yaml_loader
 from torchvision.datasets.utils import download_url
 
 from ml.core.env import get_model_dir, set_ml_config_path
 from ml.core.registry import Objects, register_model, register_task
 from ml.models.base import BaseModel
 from ml.tasks.base import BaseTask
 from ml.trainers.base import BaseTrainer
@@ -100,74 +102,75 @@
 
 
 def load_model_and_task(
     config_path: str | Path | None = None,
     ckpt_path: str | Path | None = None,
     to_device: bool = True,
     missing_ckpt_okay: bool = False,
-    weights_only: bool = True,
 ) -> tuple[BaseModel, BaseTask]:
     """Loads a trained checkpoint from a config, and optional checkpoint path.
 
     Args:
         config_path: The path to the config file.
         ckpt_path: The path to the checkpoint file; if None, the latest
             checkpoint will be used. This defaults to first checking in an
-            adjacent `checkpoints` directory for a `ckpt.pt` file, or else
+            adjacent ``checkpoints`` directory for a ``ckpt.pt`` file, or else
             checking for the checkpoint file in the same directory as the
             config.
         to_device: Whether to move the model to the device specified in the
             config.
         missing_ckpt_okay: Whether to return a model and task even if the
             checkpoint is missing.
-        weights_only: Whether to load only the weights of the model, or the
-            entire model.
 
     Returns:
         The model and task loaded from the checkpoint
 
     Raises:
-        ValueError: If both `config_path` and `ckpt_path` are None.
+        ValueError: If both ``config_path`` and ``ckpt_path`` are None.
         RuntimeError: If the checkpoint is missing and `missing_ckpt_okay` is
             False.
     """
     with Timer("loading checkpoint"):
-        ckpt: str | Path | dict | None = None
+        concrete_ckpt_path: str | Path | None = None
 
         trainer: BaseTrainer
 
         if config_path is None:
             if ckpt_path is None:
                 raise ValueError("Must provide either a config path or a checkpoint path")
 
-            ckpt = cast(dict, torch.load(ckpt_path, map_location="cpu"))
-            if "config" not in ckpt:
-                raise ValueError("Could not find a config in the checkpoint")
-            set_ml_config_path(Path(ckpt_path).parent / "config.yaml")
-            config = OmegaConf.create(ckpt["config"])
+            with safetensors.safe_open(ckpt_path, framework="pt", device="cpu") as f:
+                metadata = f.metadata()
+                if "config" not in metadata:
+                    raise ValueError("Could not find a config in the checkpoint")
+                concrete_ckpt_path = ckpt_path
+                set_ml_config_path(Path(ckpt_path).parent / "config.yaml")
+                config_yaml = yaml.load(metadata["config"], Loader=get_yaml_loader())
+                config = OmegaConf.create(config_yaml)
+
             trainer = BaseTrainer(config.trainer)
 
         else:
             set_ml_config_path(Path(config_path))
             config = cast(DictConfig, OmegaConf.load(config_path))
             trainer = BaseTrainer(config.trainer)
 
             # Uses the dummy trainer to load the checkpoint.
             try:
-                ckpt = get_checkpoint_path(trainer, config_path, ckpt_path)
+                concrete_ckpt_path = get_checkpoint_path(trainer, config_path, ckpt_path)
             except RuntimeError:
                 if missing_ckpt_okay:
                     logger.exception("Could not load checkpoint")
                 else:
                     raise
 
         model = register_model.build_entry_non_null(config)
         task = register_task.build_entry_non_null(config)
-        if ckpt is not None:
-            trainer.load_checkpoint(ckpt, task, model, weights_only=weights_only)
+        if concrete_ckpt_path is not None:
+            trainer.load_checkpoint(concrete_ckpt_path, task, model)
 
         if to_device:
             device = detect_device()
             device.module_to(model)
             device.module_to(task)
 
     return model, task
```

### Comparing `ml-starter-0.1.44/ml/utils/cli.py` & `ml-starter-0.1.45/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/colors.py` & `ml-starter-0.1.45/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/containers.py` & `ml-starter-0.1.45/ml/utils/containers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/data.py` & `ml-starter-0.1.45/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/datetime.py` & `ml-starter-0.1.45/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/device/auto.py` & `ml-starter-0.1.45/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/device/base.py` & `ml-starter-0.1.45/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/device/cpu.py` & `ml-starter-0.1.45/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/device/gpu.py` & `ml-starter-0.1.45/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/device/metal.py` & `ml-starter-0.1.45/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/distributed.py` & `ml-starter-0.1.45/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/exceptions.py` & `ml-starter-0.1.45/ml/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/image.py` & `ml-starter-0.1.45/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/io.py` & `ml-starter-0.1.45/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/large_models.py` & `ml-starter-0.1.45/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/logging.py` & `ml-starter-0.1.45/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/meter.py` & `ml-starter-0.1.45/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/mixed_precision.py` & `ml-starter-0.1.45/ml/utils/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/networking.py` & `ml-starter-0.1.45/ml/utils/networking.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/numpy.py` & `ml-starter-0.1.45/ml/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/parallel.py` & `ml-starter-0.1.45/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/spectrogram.py` & `ml-starter-0.1.45/ml/utils/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/staging.py` & `ml-starter-0.1.45/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/testing.py` & `ml-starter-0.1.45/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/timer.py` & `ml-starter-0.1.45/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/tokens.py` & `ml-starter-0.1.45/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/torch_distributed.py` & `ml-starter-0.1.45/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/triton/kmeans.py` & `ml-starter-0.1.45/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/triton/lion.py` & `ml-starter-0.1.45/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml/utils/video.py` & `ml-starter-0.1.45/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.45/ml_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.44
+Version: 0.1.45
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.44/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.45/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.44/pyproject.toml` & `ml-starter-0.1.45/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 # For TorchScript stuff.
 disable_error_code = ["attr-defined"]
 
 [[tool.mypy.overrides]]
 
 module = [
     "av.*",
+    "safetensors.*",
     "torchaudio.*",
     "torchvision.*",
 ]
 
 ignore_missing_imports = true
 
 [tool.isort]
```

### Comparing `ml-starter-0.1.44/setup.py` & `ml-starter-0.1.45/setup.py`

 * *Files identical despite different names*

