# Comparing `tmp/habitat-baselines-0.2.520230729.tar.gz` & `tmp/habitat-baselines-0.2.520230802.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habitat-baselines-0.2.520230729.tar", last modified: Sat Jul 29 05:48:39 2023, max compression
+gzip compressed data, was "habitat-baselines-0.2.520230802.tar", last modified: Wed Aug  2 17:23:09 2023, max compression
```

## Comparing `habitat-baselines-0.2.520230729.tar` & `habitat-baselines-0.2.520230802.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.712374 habitat-baselines-0.2.520230729/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       88 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5936 2023-07-29 05:48:39.712374 habitat-baselines-0.2.520230729/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4857 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.700369 habitat-baselines-0.2.520230729/habitat_baselines/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1049 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.700369 habitat-baselines-0.2.520230729/habitat_baselines/agents/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      280 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/agents/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5517 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/agents/ppo_agents.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4929 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/agents/simple_agents.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3386 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/base_il_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13480 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/base_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5711 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/baseline_registry.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1210 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/env_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      534 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/env_spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4697 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/habitat_env_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      511 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    47017 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/obs_transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9561 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/rollout_storage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1027 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/storage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12061 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/tensor_dict.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/tensorboard_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2141 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/windowed_running_mean.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1604 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/config/default.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15549 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/config/default_structured_configs.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/il/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/il/data/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/data/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9286 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/data/data.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6001 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/data/eqa_cnn_pretrain_data.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19248 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/data/nav_data.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3620 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/metrics.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/il/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23402 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/models/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       30 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/requirements.txt
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9920 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/eqa_cnn_pretrain_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26493 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/pacman_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14516 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/vqa_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       79 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/py.typed
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/rl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/algo/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/algo/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5451 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/algo/ddppo.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14526 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/ddp_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      301 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8222 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/resnet.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26845 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/resnet_policy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2891 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/running_mean_and_var.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        6 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/requirements.txt
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.708372 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      387 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22462 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hierarchical_policy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.708372 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      304 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4359 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/fixed_policy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3763 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/high_level_policy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7469 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/neural_policy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3925 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hrl_ppo.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7858 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hrl_rollout_storage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.708372 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1080 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2212 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/art_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2712 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/nav.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7676 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/nn_skill.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      980 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/noop.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4882 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/oracle_nav.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2114 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/pick.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2005 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/place.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3009 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/reset.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11880 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/skill.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1423 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      937 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.708372 habitat-baselines-0.2.520230729/habitat_baselines/rl/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4610 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/models/action_embedding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14957 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/models/rnn_state_encoder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5488 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/models/simple_cnn.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.708372 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      528 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3849 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/agent_access_mgr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11534 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/cpc_aux_loss.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15171 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/policy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12710 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/ppo.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    44038 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/ppo_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10138 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/single_agent_access_mgr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      732 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/updater.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       76 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/requirements.txt
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.712374 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10806 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/environment_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20944 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/inference_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14349 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/preemption_decider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1708 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14483 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/report_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/requirements.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1192 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/task_enums.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23285 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/ver_rollout_storage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20595 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/ver_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6394 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/worker_common.py
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     2660 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/run.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.712374 habitat-baselines-0.2.520230729/habitat_baselines/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      258 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24850 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2201 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/utils/info_dict.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3157 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/utils/timing.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.712374 habitat-baselines-0.2.520230729/habitat_baselines/utils/visualizations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      284 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/utils/visualizations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4229 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/utils/visualizations/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/version.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.700369 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5936 2023-07-29 05:48:39.000000 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4278 2023-07-29 05:48:39.000000 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-29 05:48:39.000000 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       65 2023-07-29 05:48:39.000000 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      152 2023-07-29 05:48:39.000000 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       18 2023-07-29 05:48:39.000000 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       46 2023-07-29 05:48:39.712374 habitat-baselines-0.2.520230729/setup.cfg
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2558 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.546354 habitat-baselines-0.2.520230802/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       88 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5936 2023-08-02 17:23:09.546354 habitat-baselines-0.2.520230802/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4857 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.534353 habitat-baselines-0.2.520230802/habitat_baselines/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1049 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.534353 habitat-baselines-0.2.520230802/habitat_baselines/agents/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      280 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/agents/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5517 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/agents/ppo_agents.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4929 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/agents/simple_agents.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.538353 habitat-baselines-0.2.520230802/habitat_baselines/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3386 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/base_il_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13480 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/base_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5711 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/baseline_registry.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1210 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/env_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      534 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/env_spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4697 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/habitat_env_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      511 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47017 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/obs_transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9561 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/rollout_storage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1027 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/storage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12061 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/tensor_dict.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/tensorboard_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2141 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/common/windowed_running_mean.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.538353 habitat-baselines-0.2.520230802/habitat_baselines/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1604 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/config/default.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15549 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/config/default_structured_configs.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.538353 habitat-baselines-0.2.520230802/habitat_baselines/il/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.538353 habitat-baselines-0.2.520230802/habitat_baselines/il/data/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/data/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9286 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/data/data.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6001 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/data/eqa_cnn_pretrain_data.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19248 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/data/nav_data.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3620 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/metrics.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.538353 habitat-baselines-0.2.520230802/habitat_baselines/il/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23402 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/models/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       30 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/requirements.txt
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.538353 habitat-baselines-0.2.520230802/habitat_baselines/il/trainers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/trainers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9920 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/trainers/eqa_cnn_pretrain_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26493 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/trainers/pacman_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14516 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/il/trainers/vqa_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       79 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/py.typed
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.538353 habitat-baselines-0.2.520230802/habitat_baselines/rl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.542353 habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.542353 habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/algo/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/algo/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5451 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/algo/ddppo.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14526 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/ddp_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.542353 habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/policy/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      301 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/policy/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8222 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/policy/resnet.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26845 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/policy/resnet_policy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2891 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/policy/running_mean_and_var.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        6 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/requirements.txt
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.542353 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      387 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22462 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hierarchical_policy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.542353 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      304 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4359 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hl/fixed_policy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3763 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hl/high_level_policy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7469 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hl/neural_policy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3925 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hrl_ppo.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7858 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hrl_rollout_storage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.542353 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1080 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2212 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/art_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2712 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/nav.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7676 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/nn_skill.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      980 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/noop.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4882 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/oracle_nav.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2114 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/pick.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2005 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/place.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3009 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/reset.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11880 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/skill.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1423 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      937 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.546354 habitat-baselines-0.2.520230802/habitat_baselines/rl/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4610 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/models/action_embedding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14957 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/models/rnn_state_encoder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5488 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/models/simple_cnn.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.546354 habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      528 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3849 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/agent_access_mgr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11534 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/cpc_aux_loss.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15171 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/policy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12710 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/ppo.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    44038 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/ppo_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10138 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/single_agent_access_mgr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      732 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/updater.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       76 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/requirements.txt
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.546354 habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10806 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/environment_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20944 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/inference_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14349 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/preemption_decider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1708 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14483 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/report_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/requirements.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1192 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/task_enums.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23285 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/ver_rollout_storage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20595 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/ver_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6394 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/worker_common.py
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     2660 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/run.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.546354 habitat-baselines-0.2.520230802/habitat_baselines/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      258 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24850 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2201 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/utils/info_dict.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3157 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/utils/timing.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.546354 habitat-baselines-0.2.520230802/habitat_baselines/utils/visualizations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      284 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/utils/visualizations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4229 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/utils/visualizations/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/habitat_baselines/version.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:23:09.534353 habitat-baselines-0.2.520230802/habitat_baselines.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5936 2023-08-02 17:23:09.000000 habitat-baselines-0.2.520230802/habitat_baselines.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4278 2023-08-02 17:23:09.000000 habitat-baselines-0.2.520230802/habitat_baselines.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 17:23:09.000000 habitat-baselines-0.2.520230802/habitat_baselines.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       65 2023-08-02 17:23:09.000000 habitat-baselines-0.2.520230802/habitat_baselines.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      152 2023-08-02 17:23:09.000000 habitat-baselines-0.2.520230802/habitat_baselines.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       18 2023-08-02 17:23:09.000000 habitat-baselines-0.2.520230802/habitat_baselines.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       46 2023-08-02 17:23:09.546354 habitat-baselines-0.2.520230802/setup.cfg
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2558 2023-08-02 17:22:34.000000 habitat-baselines-0.2.520230802/setup.py
```

### Comparing `habitat-baselines-0.2.520230729/PKG-INFO` & `habitat-baselines-0.2.520230802/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habitat-baselines
-Version: 0.2.520230729
+Version: 0.2.520230802
 Summary: Habitat-Baselines: Embodied AI baselines.
 Home-page: https://aihabitat.org
 Author: Meta AI Research
 License: MIT License
 Project-URL: GitHub repo, https://github.com/facebookresearch/habitat-lab/
 Project-URL: Bug Tracker, https://github.com/facebookresearch/habitat-lab/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `habitat-baselines-0.2.520230729/README.md` & `habitat-baselines-0.2.520230802/README.md`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/__init__.py` & `habitat-baselines-0.2.520230802/habitat_baselines/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/agents/ppo_agents.py` & `habitat-baselines-0.2.520230802/habitat_baselines/agents/ppo_agents.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/agents/simple_agents.py` & `habitat-baselines-0.2.520230802/habitat_baselines/agents/simple_agents.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/common/base_il_trainer.py` & `habitat-baselines-0.2.520230802/habitat_baselines/common/base_il_trainer.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/common/base_trainer.py` & `habitat-baselines-0.2.520230802/habitat_baselines/common/base_trainer.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/common/baseline_registry.py` & `habitat-baselines-0.2.520230802/habitat_baselines/common/baseline_registry.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/common/env_factory.py` & `habitat-baselines-0.2.520230802/habitat_baselines/common/env_factory.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/common/env_spec.py` & `habitat-baselines-0.2.520230802/habitat_baselines/common/env_spec.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/common/habitat_env_factory.py` & `habitat-baselines-0.2.520230802/habitat_baselines/common/habitat_env_factory.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/common/obs_transformers.py` & `habitat-baselines-0.2.520230802/habitat_baselines/common/obs_transformers.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/common/rollout_storage.py` & `habitat-baselines-0.2.520230802/habitat_baselines/common/rollout_storage.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/common/storage.py` & `habitat-baselines-0.2.520230802/habitat_baselines/common/storage.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/common/tensor_dict.py` & `habitat-baselines-0.2.520230802/habitat_baselines/common/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/common/tensorboard_utils.py` & `habitat-baselines-0.2.520230802/habitat_baselines/common/tensorboard_utils.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/common/windowed_running_mean.py` & `habitat-baselines-0.2.520230802/habitat_baselines/common/windowed_running_mean.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/config/default.py` & `habitat-baselines-0.2.520230802/habitat_baselines/config/default.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/config/default_structured_configs.py` & `habitat-baselines-0.2.520230802/habitat_baselines/config/default_structured_configs.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/il/data/data.py` & `habitat-baselines-0.2.520230802/habitat_baselines/il/data/data.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/il/data/eqa_cnn_pretrain_data.py` & `habitat-baselines-0.2.520230802/habitat_baselines/il/data/eqa_cnn_pretrain_data.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/il/data/nav_data.py` & `habitat-baselines-0.2.520230802/habitat_baselines/il/data/nav_data.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/il/metrics.py` & `habitat-baselines-0.2.520230802/habitat_baselines/il/metrics.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/il/models/models.py` & `habitat-baselines-0.2.520230802/habitat_baselines/il/models/models.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/eqa_cnn_pretrain_trainer.py` & `habitat-baselines-0.2.520230802/habitat_baselines/il/trainers/eqa_cnn_pretrain_trainer.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/pacman_trainer.py` & `habitat-baselines-0.2.520230802/habitat_baselines/il/trainers/pacman_trainer.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/vqa_trainer.py` & `habitat-baselines-0.2.520230802/habitat_baselines/il/trainers/vqa_trainer.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/algo/ddppo.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/algo/ddppo.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/ddp_utils.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/ddp_utils.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/resnet.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/policy/resnet.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/resnet_policy.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/policy/resnet_policy.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/running_mean_and_var.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ddppo/policy/running_mean_and_var.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hierarchical_policy.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hierarchical_policy.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/fixed_policy.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hl/fixed_policy.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/high_level_policy.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hl/high_level_policy.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/neural_policy.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hl/neural_policy.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hrl_ppo.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hrl_ppo.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hrl_rollout_storage.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/hrl_rollout_storage.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/__init__.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/art_obj.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/art_obj.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/nav.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/nav.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/nn_skill.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/nn_skill.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/noop.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/noop.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/oracle_nav.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/oracle_nav.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/pick.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/pick.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/place.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/place.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/reset.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/reset.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/skill.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/skill.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/wait.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/skills/wait.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/utils.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/hrl/utils.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/models/action_embedding.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/models/action_embedding.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/models/rnn_state_encoder.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/models/rnn_state_encoder.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/models/simple_cnn.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/models/simple_cnn.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/__init__.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/agent_access_mgr.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/agent_access_mgr.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/cpc_aux_loss.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/cpc_aux_loss.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/policy.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/policy.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/ppo.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/ppo.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/ppo_trainer.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/ppo_trainer.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/single_agent_access_mgr.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/single_agent_access_mgr.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/updater.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ppo/updater.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/environment_worker.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/environment_worker.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/inference_worker.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/inference_worker.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/preemption_decider.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/preemption_decider.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/queue.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/queue.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/report_worker.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/report_worker.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/task_enums.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/task_enums.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/ver_rollout_storage.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/ver_rollout_storage.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/ver_trainer.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/ver_trainer.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/worker_common.py` & `habitat-baselines-0.2.520230802/habitat_baselines/rl/ver/worker_common.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/run.py` & `habitat-baselines-0.2.520230802/habitat_baselines/run.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/utils/common.py` & `habitat-baselines-0.2.520230802/habitat_baselines/utils/common.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/utils/info_dict.py` & `habitat-baselines-0.2.520230802/habitat_baselines/utils/info_dict.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/utils/timing.py` & `habitat-baselines-0.2.520230802/habitat_baselines/utils/timing.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines/utils/visualizations/utils.py` & `habitat-baselines-0.2.520230802/habitat_baselines/utils/visualizations/utils.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines.egg-info/PKG-INFO` & `habitat-baselines-0.2.520230802/habitat_baselines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habitat-baselines
-Version: 0.2.520230729
+Version: 0.2.520230802
 Summary: Habitat-Baselines: Embodied AI baselines.
 Home-page: https://aihabitat.org
 Author: Meta AI Research
 License: MIT License
 Project-URL: GitHub repo, https://github.com/facebookresearch/habitat-lab/
 Project-URL: Bug Tracker, https://github.com/facebookresearch/habitat-lab/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `habitat-baselines-0.2.520230729/habitat_baselines.egg-info/SOURCES.txt` & `habitat-baselines-0.2.520230802/habitat_baselines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.520230729/setup.py` & `habitat-baselines-0.2.520230802/setup.py`

 * *Files identical despite different names*

