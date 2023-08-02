# Comparing `tmp/rl4co-0.1.0.tar.gz` & `tmp/rl4co-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl4co-0.1.0.tar", last modified: Sat Jul 22 20:09:57 2023, max compression
+gzip compressed data, was "rl4co-0.1.1.tar", last modified: Wed Aug  2 12:52:23 2023, max compression
```

## Comparing `rl4co-0.1.0.tar` & `rl4co-0.1.1.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.069568 rl4co-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-22 20:09:42.000000 rl4co-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-07-22 20:09:57.069568 rl4co-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-07-22 20:09:42.000000 rl4co-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-22 20:09:42.000000 rl4co-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.045568 rl4co-0.1.0/rl4co/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.049568 rl4co-0.1.0/rl4co/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/data/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/data/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.049568 rl4co-0.1.0/rl4co/envs/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/atsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.049568 rl4co-0.1.0/rl4co/envs/common/
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/common/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/cvrp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15199 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/dpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/ffsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/mdpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/mpdp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13117 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/mtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/op.py
--rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/pctsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/pdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/sdvrp.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/spctsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.049568 rl4co-0.1.0/rl4co/models/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.053568 rl4co-0.1.0/rl4co/models/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.053568 rl4co-0.1.0/rl4co/models/nn/env_embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/env_embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/env_embeddings/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/env_embeddings/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/env_embeddings/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/flash_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.053568 rl4co-0.1.0/rl4co/models/nn/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/graph/attnnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/graph/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/graph/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.053568 rl4co-0.1.0/rl4co/models/rl/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/rl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.053568 rl4co-0.1.0/rl4co/models/rl/common/
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/rl/common/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/rl/common/critic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.053568 rl4co-0.1.0/rl4co/models/rl/ppo/
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/rl/ppo/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.057568 rl4co-0.1.0/rl4co/models/rl/reinforce/
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/rl/reinforce/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/rl/reinforce/reinforce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.041568 rl4co-0.1.0/rl4co/models/zoo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.057568 rl4co-0.1.0/rl4co/models/zoo/am/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/am/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/am/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/am/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.041568 rl4co-0.1.0/rl4co/models/zoo/common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.057568 rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.057568 rl4co-0.1.0/rl4co/models/zoo/et/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/et/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/et/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/et/positional_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.057568 rl4co-0.1.0/rl4co/models/zoo/ham/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ham/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ham/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ham/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ham/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ham/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.061568 rl4co-0.1.0/rl4co/models/zoo/mdam/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/mdam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/mdam/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/mdam/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/mdam/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/mdam/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.061568 rl4co-0.1.0/rl4co/models/zoo/pomo/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/pomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/pomo/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/pomo/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/pomo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/pomo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.061568 rl4co-0.1.0/rl4co/models/zoo/ppo/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ppo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ppo/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ppo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ppo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.061568 rl4co-0.1.0/rl4co/models/zoo/ptrnet/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ptrnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ptrnet/critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ptrnet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ptrnet/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ptrnet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ptrnet/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.065568 rl4co-0.1.0/rl4co/models/zoo/symnco/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/symnco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/symnco/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/symnco/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/symnco/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.065568 rl4co-0.1.0/rl4co/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/tasks/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/tasks/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.065568 rl4co-0.1.0/rl4co/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.065568 rl4co-0.1.0/rl4co/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/callbacks/speed_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.069568 rl4co-0.1.0/rl4co/utils/download/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/download/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/download/gdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/download/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/instantiators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/optim_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/param_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/pylogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.045568 rl4co-0.1.0/rl4co.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-07-22 20:09:57.000000 rl4co-0.1.0/rl4co.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-22 20:09:57.000000 rl4co-0.1.0/rl4co.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:09:57.000000 rl4co-0.1.0/rl4co.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-22 20:09:57.000000 rl4co-0.1.0/rl4co.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 20:09:57.000000 rl4co-0.1.0/rl4co.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:09:57.069568 rl4co-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.069568 rl4co-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-22 20:09:42.000000 rl4co-0.1.0/tests/test_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-22 20:09:42.000000 rl4co-0.1.0/tests/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-22 20:09:42.000000 rl4co-0.1.0/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-22 20:09:42.000000 rl4co-0.1.0/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-22 20:09:42.000000 rl4co-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.862234 rl4co-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-08-02 12:52:14.000000 rl4co-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20861 2023-08-02 12:52:23.862234 rl4co-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-08-02 12:52:14.000000 rl4co-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-02 12:52:14.000000 rl4co-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.846234 rl4co-0.1.1/rl4co/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.850234 rl4co-0.1.1/rl4co/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/data/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/data/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.850234 rl4co-0.1.1/rl4co/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/atsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.850234 rl4co-0.1.1/rl4co/envs/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/cvrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15199 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/dpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/ffsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/mdpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/mpdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13117 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/mtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/pctsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/pdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/sdvrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/spctsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/envs/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.850234 rl4co-0.1.1/rl4co/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.850234 rl4co-0.1.1/rl4co/models/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/nn/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.854234 rl4co-0.1.1/rl4co/models/nn/env_embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/nn/env_embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/nn/env_embeddings/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/nn/env_embeddings/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/nn/env_embeddings/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/nn/flash_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.854234 rl4co-0.1.1/rl4co/models/nn/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/nn/graph/attnnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/nn/graph/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/nn/graph/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/nn/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/nn/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.854234 rl4co-0.1.1/rl4co/models/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/rl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.854234 rl4co-0.1.1/rl4co/models/rl/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/rl/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/rl/common/critic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.854234 rl4co-0.1.1/rl4co/models/rl/ppo/
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/rl/ppo/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.854234 rl4co-0.1.1/rl4co/models/rl/reinforce/
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/rl/reinforce/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/rl/reinforce/reinforce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.846234 rl4co-0.1.1/rl4co/models/zoo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.854234 rl4co-0.1.1/rl4co/models/zoo/am/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/am/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/am/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/am/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.846234 rl4co-0.1.1/rl4co/models/zoo/common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.854234 rl4co-0.1.1/rl4co/models/zoo/common/autoregressive/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/common/autoregressive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/common/autoregressive/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/common/autoregressive/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/common/autoregressive/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.854234 rl4co-0.1.1/rl4co/models/zoo/et/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/et/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/et/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/et/positional_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.854234 rl4co-0.1.1/rl4co/models/zoo/ham/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ham/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ham/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ham/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ham/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ham/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.854234 rl4co-0.1.1/rl4co/models/zoo/mdam/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/mdam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/mdam/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/mdam/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/mdam/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/mdam/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.858234 rl4co-0.1.1/rl4co/models/zoo/pomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/pomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/pomo/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/pomo/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/pomo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/pomo/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.858234 rl4co-0.1.1/rl4co/models/zoo/ppo/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ppo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ppo/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ppo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ppo/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.858234 rl4co-0.1.1/rl4co/models/zoo/ptrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ptrnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ptrnet/critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ptrnet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ptrnet/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ptrnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/ptrnet/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.858234 rl4co-0.1.1/rl4co/models/zoo/symnco/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/symnco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/symnco/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/symnco/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/models/zoo/symnco/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.858234 rl4co-0.1.1/rl4co/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/tasks/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/tasks/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.862234 rl4co-0.1.1/rl4co/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.862234 rl4co-0.1.1/rl4co/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/callbacks/speed_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.862234 rl4co-0.1.1/rl4co/utils/download/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/download/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/download/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/download/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/download/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/optim_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/param_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/pylogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-08-02 12:52:14.000000 rl4co-0.1.1/rl4co/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.846234 rl4co-0.1.1/rl4co.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20861 2023-08-02 12:52:23.000000 rl4co-0.1.1/rl4co.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-08-02 12:52:23.000000 rl4co-0.1.1/rl4co.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:52:23.000000 rl4co-0.1.1/rl4co.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-02 12:52:23.000000 rl4co-0.1.1/rl4co.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 12:52:23.000000 rl4co-0.1.1/rl4co.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 12:52:23.862234 rl4co-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:52:23.862234 rl4co-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-02 12:52:14.000000 rl4co-0.1.1/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-02 12:52:14.000000 rl4co-0.1.1/tests/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-02 12:52:14.000000 rl4co-0.1.1/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-02 12:52:14.000000 rl4co-0.1.1/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-02 12:52:14.000000 rl4co-0.1.1/tests/test_utils.py
```

### Comparing `rl4co-0.1.0/LICENSE` & `rl4co-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/PKG-INFO` & `rl4co-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.1.0
+Version: 0.1.1
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -297,35 +297,35 @@
 
 
 <details>
     <summary>Change experiment</summary>
 
 Train model with chosen experiment configuration from [configs/experiment/](configs/experiment/) (e.g. tsp/am, and environment with 42 cities)
 ```bash
-python run.py experiment=tsp/am env.num_loc=42
+python run.py experiment=routing/am env.num_loc=42
 ```
 </details>
 
 
 <details>
     <summary>Disable logging</summary>
 
 ```bash
-python run.py experiment=test/am logger=none '~callbacks.learning_rate_monitor'
+python run.py experiment=routing/am logger=none '~callbacks.learning_rate_monitor'
 ```
 Note that `~` is used to disable a callback that would need a logger.
 
 </details>
 
 
 <details>
     <summary>Create a sweep over hyperparameters (-m for multirun)</summary>
 
 ```bash
-python run.py -m experiment=tsp/am  train.optimizer.lr=1e-3,1e-4,1e-5
+python run.py -m experiment=routing/am  train.optimizer.lr=1e-3,1e-4,1e-5
 ```
 </details>
 
 
 
 ### Minimalistic Example
```

### Comparing `rl4co-0.1.0/README.md` & `rl4co-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -74,35 +74,35 @@
 
 
 <details>
     <summary>Change experiment</summary>
 
 Train model with chosen experiment configuration from [configs/experiment/](configs/experiment/) (e.g. tsp/am, and environment with 42 cities)
 ```bash
-python run.py experiment=tsp/am env.num_loc=42
+python run.py experiment=routing/am env.num_loc=42
 ```
 </details>
 
 
 <details>
     <summary>Disable logging</summary>
 
 ```bash
-python run.py experiment=test/am logger=none '~callbacks.learning_rate_monitor'
+python run.py experiment=routing/am logger=none '~callbacks.learning_rate_monitor'
 ```
 Note that `~` is used to disable a callback that would need a logger.
 
 </details>
 
 
 <details>
     <summary>Create a sweep over hyperparameters (-m for multirun)</summary>
 
 ```bash
-python run.py -m experiment=tsp/am  train.optimizer.lr=1e-3,1e-4,1e-5
+python run.py -m experiment=routing/am  train.optimizer.lr=1e-3,1e-4,1e-5
 ```
 </details>
 
 
 
 ### Minimalistic Example
```

#### html2text {}

```diff
@@ -35,20 +35,20 @@
 candidate for hassle-free installation of PyTorch: check out the [PyTorch
 website](https://pytorch.org/get-started/locally/) for more details.  To get
 started, we recommend checking out our [quickstart notebook](notebooks/1-
 quickstart.ipynb) or the [minimalistic example](#minimalistic-example) below.
 ## Usage Train model with default configuration (AM on TSP environment):
 ```bash python run.py ```  Change experiment Train model with chosen experiment
 configuration from [configs/experiment/](configs/experiment/) (e.g. tsp/am, and
-environment with 42 cities) ```bash python run.py experiment=tsp/am
-env.num_loc=42 ```   Disable logging ```bash python run.py experiment=test/am
-logger=none '~callbacks.learning_rate_monitor' ``` Note that `~` is used to
+environment with 42 cities) ```bash python run.py experiment=routing/am
+env.num_loc=42 ```   Disable logging ```bash python run.py experiment=routing/
+am logger=none '~callbacks.learning_rate_monitor' ``` Note that `~` is used to
 disable a callback that would need a logger.   Create a sweep over
-hyperparameters (-m for multirun) ```bash python run.py -m experiment=tsp/am
-train.optimizer.lr=1e-3,1e-4,1e-5 ```  ### Minimalistic Example Here is a
+hyperparameters (-m for multirun) ```bash python run.py -m experiment=routing/
+am train.optimizer.lr=1e-3,1e-4,1e-5 ```  ### Minimalistic Example Here is a
 minimalistic example training the Attention Model with greedy rollout baseline
 on TSP in less than 30 lines of code: ```python from rl4co.envs import TSPEnv
 from rl4co.models import AttentionModel from rl4co.utils import RL4COTrainer #
 Environment, Model, and Lightning Module env = TSPEnv(num_loc=20) model =
 AttentionModel(env, baseline="rollout", train_data_size=100_000,
 test_data_size=10_000, optimizer_kwargs={'lr': 1e-4} ) # Trainer trainer =
 RL4COTrainer(max_epochs=3) # Fit the model trainer.fit(model) # Test the model
```

### Comparing `rl4co-0.1.0/pyproject.toml` & `rl4co-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/data/generate_data.py` & `rl4co-0.1.1/rl4co/data/generate_data.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/data/transforms.py` & `rl4co-0.1.1/rl4co/data/transforms.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/data/utils.py` & `rl4co-0.1.1/rl4co/data/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/__init__.py` & `rl4co-0.1.1/rl4co/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/atsp.py` & `rl4co-0.1.1/rl4co/envs/atsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/common/base.py` & `rl4co-0.1.1/rl4co/envs/common/base.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/common/utils.py` & `rl4co-0.1.1/rl4co/envs/common/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/cvrp.py` & `rl4co-0.1.1/rl4co/envs/cvrp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/dpp.py` & `rl4co-0.1.1/rl4co/envs/dpp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/ffsp.py` & `rl4co-0.1.1/rl4co/envs/ffsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/mdpp.py` & `rl4co-0.1.1/rl4co/envs/mdpp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/mpdp.py` & `rl4co-0.1.1/rl4co/envs/mpdp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/mtsp.py` & `rl4co-0.1.1/rl4co/envs/mtsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/op.py` & `rl4co-0.1.1/rl4co/envs/op.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/pctsp.py` & `rl4co-0.1.1/rl4co/envs/pctsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/pdp.py` & `rl4co-0.1.1/rl4co/envs/pdp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/sdvrp.py` & `rl4co-0.1.1/rl4co/envs/sdvrp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/spctsp.py` & `rl4co-0.1.1/rl4co/envs/spctsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/envs/tsp.py` & `rl4co-0.1.1/rl4co/envs/tsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/nn/attention.py` & `rl4co-0.1.1/rl4co/models/nn/attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/nn/env_embeddings/context.py` & `rl4co-0.1.1/rl4co/models/nn/env_embeddings/context.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/nn/env_embeddings/dynamic.py` & `rl4co-0.1.1/rl4co/models/nn/env_embeddings/dynamic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/nn/env_embeddings/init.py` & `rl4co-0.1.1/rl4co/models/nn/env_embeddings/init.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/nn/flash_attention.py` & `rl4co-0.1.1/rl4co/models/nn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/nn/graph/attnnet.py` & `rl4co-0.1.1/rl4co/models/nn/graph/attnnet.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/nn/graph/gcn.py` & `rl4co-0.1.1/rl4co/models/nn/graph/gcn.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/nn/graph/mpnn.py` & `rl4co-0.1.1/rl4co/models/nn/graph/mpnn.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/nn/mlp.py` & `rl4co-0.1.1/rl4co/models/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/nn/ops.py` & `rl4co-0.1.1/rl4co/models/nn/ops.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/nn/utils.py` & `rl4co-0.1.1/rl4co/models/nn/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/rl/common/base.py` & `rl4co-0.1.1/rl4co/models/rl/common/base.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/rl/common/critic.py` & `rl4co-0.1.1/rl4co/models/rl/common/critic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/rl/ppo/ppo.py` & `rl4co-0.1.1/rl4co/models/rl/ppo/ppo.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,39 +22,43 @@
     as part of the MDP transition. While many Neural Combinatorial Optimization (NCO) studies model decoding steps
     as transitions in a solution-construction MDP, we treat autoregressive solution construction as an algorithmic
     choice for tractable CO solution generation. This choice aligns with the Attention Model (AM)
     (https://openreview.net/forum?id=ByxBFsRqYm), which treats decoding steps as a single-step MDP in Equation 9.
 
     Modeling autoregressive decoding steps as a single-step MDP introduces significant changes to the PPO implementation,
     including:
-    - Generalized Advantage Estimation (GAE) (https://arxiv.org/abs/1506.02438) is not applicable since we are dealing
-      with a single-step MDP.
+    - Generalized Advantage Estimation (GAE) (https://arxiv.org/abs/1506.02438) is not applicable since we are dealing with a single-step MDP.
     - The definition of policy entropy can differ from the commonly implemented manner.
 
     The commonly implemented definition of policy entropy is the entropy of the policy distribution, given by:
-        H(pi(a|x_t)) = - sum_a pi(a|x_t) log pi(a|x_t), where x_t represents the given state at step t.
+
+    .. math:: H(\\pi(x_t)) = - \\sum_{a_t \\in A_t} \\pi(a_t|x_t) \\log \\pi(a_t|x_t)
+
+    where :math:`x_t` represents the given state at step :math:`t`, :math:`A_t` is the set of all (admisible) actions
+    at step :math:`t`, and :math:`a_t` is the action taken at step :math:`t`.
 
     If we interpret autoregressive decoding steps as transition steps of an MDP, the entropy for the entire decoding
     process can be defined as the sum of entropies for each decoding step:
-        H(pi) = sum_t H(pi(a|x_t))
+
+    .. math:: H(\\pi) = \\sum_t H(\\pi(x_t))
 
     However, if we consider autoregressive decoding steps as an algorithmic choice, the entropy for the entire decoding
     process is defined as:
-        H(pi) = sum_a in A pi(a|x) log pi(a|x),
-        where x represents the given CO problem instance, and A is the set of all feasible solutions.
+
+    .. math:: H(\\pi) = - \\sum_{a \\in A} \\pi(a|x) \\log \\pi(a|x)
+
+    where :math:`x` represents the given CO problem instance, and :math:`A` is the set of all feasible solutions.
 
     Due to the intractability of computing the entropy of the policy distribution over all feasible solutions,
     we approximate it by computing the entropy over solutions generated by the policy itself. This approximation serves
     as a proxy for the second definition of entropy, utilizing Monte Carlo sampling.
 
     It is worth noting that our modeling of decoding steps and the implementation of the PPO algorithm align with recent
     work in the Natural Language Processing (NLP) community, specifically RL with Human Feedback (RLHF)
     (e.g., https://github.com/lucidrains/PaLM-rlhf-pytorch).
-
-
     """
 
     def __init__(
         self,
         env: RL4COEnvBase,
         policy: nn.Module,
         critic: nn.Module,
```

### Comparing `rl4co-0.1.0/rl4co/models/rl/reinforce/baselines.py` & `rl4co-0.1.1/rl4co/models/rl/reinforce/baselines.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
     def setup(self, model, env, **kwargs):
         if self.critic is None:
             log.info("Creating critic network for {}".format(env.name))
             self.critic = CriticNetwork(env.name, **kwargs)
 
     def eval(self, x, c, env=None):
-        v = self.critic(x)
+        v = self.critic(x).squeeze(-1)
         # detach v since actor should not backprop through baseline, only for neg_loss
         return v.detach(), -F.mse_loss(v, c.detach())
 
 
 class RolloutBaseline(REINFORCEBaseline):
     """Rollout baseline: use greedy rollout as baseline
 
@@ -221,22 +221,22 @@
 
         model.eval()
         model = model.to(device)
 
         def eval_model(batch):
             with torch.no_grad():
                 batch = env.reset(batch.to(device))
-                return model(batch, env, decode_type="greedy")["reward"].data.cpu()
+                return model(batch, env, decode_type="greedy")["reward"]
 
         dl = DataLoader(dataset, batch_size=batch_size, collate_fn=tensordict_collate_fn)
 
-        retval = torch.cat(
+        rewards = torch.cat(
             [eval_model(batch) for batch in tqdm(dl, disable=not self.progress_bar)], 0
         )
-        return retval
+        return rewards
 
     def wrap_dataset(self, dataset, env, batch_size=64, device="cpu", **kw):
         """Wrap the dataset in a baseline dataset
 
         Note:
             This is an alternative to `eval` that does not require the model to be passed
             at every call but just once. Values are added to the dataset. This also allows for
```

### Comparing `rl4co-0.1.0/rl4co/models/rl/reinforce/reinforce.py` & `rl4co-0.1.1/rl4co/models/rl/reinforce/reinforce.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         td = self.env.reset(batch)
         # Perform forward pass (i.e., constructing solution and computing log-likelihoods)
         out = self.policy(td, self.env, phase=phase)
 
         # Compute loss
         if phase == "train":
             # Extra: this is used for additional loss terms, e.g., REINFORCE baseline
-            extra = td.get("extra", None)
+            extra = batch.get("extra", None)
 
             bl_val, bl_neg_loss = (
                 self.baseline.eval(td, out["reward"], self.env)
                 if extra is None
                 else (extra, 0)
             )
```

### Comparing `rl4co-0.1.0/rl4co/models/zoo/am/model.py` & `rl4co-0.1.1/rl4co/models/zoo/am/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/am/policy.py` & `rl4co-0.1.1/rl4co/models/zoo/am/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/decoder.py` & `rl4co-0.1.1/rl4co/models/zoo/common/autoregressive/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/encoder.py` & `rl4co-0.1.1/rl4co/models/zoo/common/autoregressive/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/policy.py` & `rl4co-0.1.1/rl4co/models/zoo/common/autoregressive/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/et/model.py` & `rl4co-0.1.1/rl4co/models/zoo/et/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/et/policy.py` & `rl4co-0.1.1/rl4co/models/zoo/et/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/et/positional_encoding.py` & `rl4co-0.1.1/rl4co/models/zoo/et/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/ham/attention.py` & `rl4co-0.1.1/rl4co/models/zoo/ham/attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/ham/encoder.py` & `rl4co-0.1.1/rl4co/models/zoo/ham/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/ham/model.py` & `rl4co-0.1.1/rl4co/models/zoo/ham/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/ham/policy.py` & `rl4co-0.1.1/rl4co/models/zoo/ham/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/mdam/decoder.py` & `rl4co-0.1.1/rl4co/models/zoo/mdam/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/mdam/encoder.py` & `rl4co-0.1.1/rl4co/models/zoo/mdam/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/mdam/model.py` & `rl4co-0.1.1/rl4co/models/zoo/mdam/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/mdam/policy.py` & `rl4co-0.1.1/rl4co/models/zoo/mdam/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/pomo/augmentations.py` & `rl4co-0.1.1/rl4co/models/zoo/pomo/augmentations.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/pomo/decoder.py` & `rl4co-0.1.1/rl4co/models/zoo/pomo/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/pomo/model.py` & `rl4co-0.1.1/rl4co/models/zoo/pomo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/pomo/policy.py` & `rl4co-0.1.1/rl4co/models/zoo/pomo/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/ppo/decoder.py` & `rl4co-0.1.1/rl4co/models/zoo/ppo/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/ppo/model.py` & `rl4co-0.1.1/rl4co/models/zoo/ppo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/ppo/policy.py` & `rl4co-0.1.1/rl4co/models/zoo/ppo/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/ptrnet/critic.py` & `rl4co-0.1.1/rl4co/models/zoo/ptrnet/critic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/ptrnet/decoder.py` & `rl4co-0.1.1/rl4co/models/zoo/ptrnet/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/ptrnet/encoder.py` & `rl4co-0.1.1/rl4co/models/zoo/ptrnet/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/ptrnet/model.py` & `rl4co-0.1.1/rl4co/models/zoo/ptrnet/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.models.rl import REINFORCE
 from rl4co.models.rl.reinforce.baselines import REINFORCEBaseline
 from rl4co.models.zoo.ptrnet.policy import PointerNetworkPolicy
 
 
 class PointerNetwork(REINFORCE):
-    """
-    Pointer Network for neural combinatorial optimization based on REINFORCE
+    """Pointer Network for neural combinatorial optimization based on REINFORCE
     Based on Vinyals et al. (2015) https://arxiv.org/abs/1506.03134
     Refactored from reference implementation: https://github.com/wouterkool/attention-learn-to-route
+
     Args:
         env: Environment to use for the algorithm
         policy: Policy to use for the algorithm
         baseline: REINFORCE baseline. Defaults to rollout (1 epoch of exponential, then greedy rollout baseline)
         policy_kwargs: Keyword arguments for policy
         baseline_kwargs: Keyword arguments for baseline
         **kwargs: Keyword arguments passed to the superclass
```

### Comparing `rl4co-0.1.0/rl4co/models/zoo/ptrnet/policy.py` & `rl4co-0.1.1/rl4co/models/zoo/ptrnet/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/symnco/losses.py` & `rl4co-0.1.1/rl4co/models/zoo/symnco/losses.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/symnco/model.py` & `rl4co-0.1.1/rl4co/models/zoo/symnco/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/models/zoo/symnco/policy.py` & `rl4co-0.1.1/rl4co/models/zoo/symnco/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/tasks/eval.py` & `rl4co-0.1.1/rl4co/tasks/eval.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import numpy as np
 import torch
 
 from torch.utils.data import DataLoader
 from tqdm.auto import tqdm
 
 from rl4co.data.dataset import tensordict_collate_fn
-from rl4co.models.zoo.pomo.augmentations import (
-    StateAugmentation as Dihedral8StateAugmentation,
-)
-from rl4co.models.zoo.symnco.augmentations import (
-    StateAugmentation as SymmetricStateAugmentation,
-)
+from rl4co.data.transforms import StateAugmentation
 from rl4co.utils.ops import batchify, gather_by_index, unbatchify
 
 
 def check_unused_kwargs(class_, kwargs):
     if len(kwargs) > 0 and not (len(kwargs) == 1 and "progress" in kwargs):
         print(f"Warning: {class_.__class__.__name__} does not use kwargs {kwargs}")
 
@@ -125,26 +120,17 @@
     """
 
     name = "augmentation"
 
     def __init__(self, env, num_augment=8, force_dihedral_8=False, **kwargs):
         check_unused_kwargs(self, kwargs)
         super().__init__(env, kwargs.get("progress", True))
-
-        assert not (
-            num_augment != 8 and force_dihedral_8
-        ), "Cannot force dihedral when num_augment != 8"
-        if num_augment == 8 and not force_dihedral_8:
-            self.augmentation = Dihedral8StateAugmentation(
-                env.name, num_augment=num_augment
-            )
-        else:
-            self.augmentation = SymmetricStateAugmentation(
-                env.name, num_augment=num_augment
-            )
+        self.augmentation = StateAugmentation(
+            env.name, num_augment=num_augment, use_dihedral_8=force_dihedral_8
+        )
 
     def _inner(self, policy, td, num_augment=None):
         if num_augment is None:
             num_augment = self.augmentation.num_augment
         td_init = td.clone()
         td = self.augmentation(td, num_augment=num_augment)
         out = policy(td.clone(), decode_type="greedy", num_starts=0, return_actions=True)
@@ -260,22 +246,17 @@
         super().__init__(env, kwargs.get("progress", True))
 
         assert num_starts is not None, "Must specify num_starts"
         self.num_starts = num_starts
         assert not (
             num_augment != 8 and force_dihedral_8
         ), "Cannot force dihedral 8 when num_augment != 8"
-        if num_augment == 8 and not force_dihedral_8:
-            self.augmentation = Dihedral8StateAugmentation(
-                env.name, num_augment=num_augment
-            )
-        else:
-            self.augmentation = SymmetricStateAugmentation(
-                env.name, num_augment=num_augment
-            )
+        self.augmentation = StateAugmentation(
+            env.name, num_augment=num_augment, use_dihedral_8=force_dihedral_8
+        )
 
     def _inner(self, policy, td, num_augment=None):
         if num_augment is None:
             num_augment = self.augmentation.num_augment
 
         td_init = td.clone()
```

### Comparing `rl4co-0.1.0/rl4co/tasks/train.py` & `rl4co-0.1.1/rl4co/tasks/train.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/callbacks/speed_monitor.py` & `rl4co-0.1.1/rl4co/utils/callbacks/speed_monitor.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/download/downloader.py` & `rl4co-0.1.1/rl4co/utils/download/downloader.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/download/gdrive.py` & `rl4co-0.1.1/rl4co/utils/download/gdrive.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/download/s3.py` & `rl4co-0.1.1/rl4co/utils/download/s3.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/instantiators.py` & `rl4co-0.1.1/rl4co/utils/instantiators.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/lightning.py` & `rl4co-0.1.1/rl4co/utils/lightning.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/ops.py` & `rl4co-0.1.1/rl4co/utils/ops.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/optim_helpers.py` & `rl4co-0.1.1/rl4co/utils/optim_helpers.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/param_grouping.py` & `rl4co-0.1.1/rl4co/utils/param_grouping.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/pylogger.py` & `rl4co-0.1.1/rl4co/utils/pylogger.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/rich_utils.py` & `rl4co-0.1.1/rl4co/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/test_utils.py` & `rl4co-0.1.1/rl4co/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/trainer.py` & `rl4co-0.1.1/rl4co/utils/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import Iterable, List, Optional, Sequence, Union
+from typing import Iterable, List, Optional, Union
 
 import torch
 
 from lightning import Callback, Trainer
+from lightning.fabric.accelerators.cuda import num_cuda_devices
 from lightning.pytorch.accelerators import Accelerator
 from lightning.pytorch.loggers import Logger
 from lightning.pytorch.strategies import DDPStrategy, Strategy
 
 from rl4co import utils
 
 log = utils.get_pylogger(__name__)
@@ -46,33 +47,38 @@
         logger: Optional[Union[Logger, Iterable[Logger]]] = None,
         min_epochs: Optional[int] = None,
         max_epochs: Optional[int] = None,
         strategy: Union[str, Strategy] = "auto",
         devices: Union[List[int], str, int] = "auto",
         gradient_clip_val: Union[int, float] = 1.0,
         precision: Union[str, int] = "16-mixed",
+        reload_dataloaders_every_n_epochs: int = 1,
         disable_profiling_executor: bool = True,
         auto_configure_ddp: bool = True,
-        reload_dataloaders_every_n_epochs: int = 1,
         matmul_precision: Union[str, int] = "medium",
         **kwargs,
     ):
         # Disable JIT profiling executor. This reduces memory and increases speed.
         # Reference: https://github.com/HazyResearch/safari/blob/111d2726e7e2b8d57726b7a8b932ad8a4b2ad660/train.py#LL124-L129C17
         if disable_profiling_executor:
             try:
                 torch._C._jit_set_profiling_executor(False)
                 torch._C._jit_set_profiling_mode(False)
             except AttributeError:
                 pass
 
         # Configure DDP automatically
-        if auto_configure_ddp and isinstance(devices, Sequence):
-            n_devices = len(devices)
-            if n_devices > 1 and strategy is None:
+        if auto_configure_ddp and strategy == "auto":
+            if devices == "auto":
+                n_devices = num_cuda_devices()
+            elif isinstance(devices, list):
+                n_devices = len(devices)
+            else:
+                n_devices = devices
+            if n_devices > 1:
                 log.info("Configuring DDP strategy automatically")
                 strategy = DDPStrategy(
                     find_unused_parameters=True,  # We set to True due to RL envs
                     gradient_as_bucket_view=True,  # https://pytorch-lightning.readthedocs.io/en/stable/advanced/advanced_gpu.html#ddp-optimizations
                 )
 
         # Set matmul precision for faster inference https://pytorch.org/docs/stable/generated/torch.set_float32_matmul_precision.html#torch.set_float32_matmul_precision
@@ -96,11 +102,13 @@
         super().__init__(
             accelerator=accelerator,
             callbacks=callbacks,
             logger=logger,
             min_epochs=min_epochs,
             max_epochs=max_epochs,
             strategy=strategy,
+            gradient_clip_val=gradient_clip_val,
             devices=devices,
             precision=precision,
+            reload_dataloaders_every_n_epochs=reload_dataloaders_every_n_epochs,
             **kwargs,
         )
```

### Comparing `rl4co-0.1.0/rl4co/utils/transfer.py` & `rl4co-0.1.1/rl4co/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co/utils/utils.py` & `rl4co-0.1.1/rl4co/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/rl4co.egg-info/PKG-INFO` & `rl4co-0.1.1/rl4co.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.1.0
+Version: 0.1.1
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -297,35 +297,35 @@
 
 
 <details>
     <summary>Change experiment</summary>
 
 Train model with chosen experiment configuration from [configs/experiment/](configs/experiment/) (e.g. tsp/am, and environment with 42 cities)
 ```bash
-python run.py experiment=tsp/am env.num_loc=42
+python run.py experiment=routing/am env.num_loc=42
 ```
 </details>
 
 
 <details>
     <summary>Disable logging</summary>
 
 ```bash
-python run.py experiment=test/am logger=none '~callbacks.learning_rate_monitor'
+python run.py experiment=routing/am logger=none '~callbacks.learning_rate_monitor'
 ```
 Note that `~` is used to disable a callback that would need a logger.
 
 </details>
 
 
 <details>
     <summary>Create a sweep over hyperparameters (-m for multirun)</summary>
 
 ```bash
-python run.py -m experiment=tsp/am  train.optimizer.lr=1e-3,1e-4,1e-5
+python run.py -m experiment=routing/am  train.optimizer.lr=1e-3,1e-4,1e-5
 ```
 </details>
 
 
 
 ### Minimalistic Example
```

### Comparing `rl4co-0.1.0/rl4co.egg-info/SOURCES.txt` & `rl4co-0.1.1/rl4co.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/tests/test_envs.py` & `rl4co-0.1.1/tests/test_envs.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/tests/test_policy.py` & `rl4co-0.1.1/tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/tests/test_tasks.py` & `rl4co-0.1.1/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.1.0/tests/test_training.py` & `rl4co-0.1.1/tests/test_training.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     trainer.fit(model)
     trainer.test(model)
 
 
 def test_ppo():
     env = TSPEnv(num_loc=20)
     model = PPOModel(env, train_data_size=10, val_data_size=10, test_data_size=10)
-    trainer = RL4COTrainer(max_epochs=1)
+    trainer = RL4COTrainer(max_epochs=1, gradient_clip_val=None)
     trainer.fit(model)
     trainer.test(model)
 
 
 def test_symnco():
     env = TSPEnv(num_loc=20)
     model = SymNCO(
```

### Comparing `rl4co-0.1.0/tests/test_utils.py` & `rl4co-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

